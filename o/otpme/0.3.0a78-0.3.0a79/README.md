# Comparing `tmp/otpme-0.3.0a78.tar.gz` & `tmp/otpme-0.3.0a79.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otpme-0.3.0a78.tar", last modified: Fri May 24 14:06:58 2024, max compression
+gzip compressed data, was "otpme-0.3.0a79.tar", last modified: Mon Jun  3 13:51:56 2024, max compression
```

## Comparing `otpme-0.3.0a78.tar` & `otpme-0.3.0a79.tar`

### file list

```diff
@@ -1,515 +1,515 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.809777 otpme-0.3.0a78/
--rw-r--r--   0 root         (0) root         (0)    35121 2024-05-24 14:06:57.000000 otpme-0.3.0a78/LICENSE
--rw-r--r--   0 root         (0) root         (0)      665 2024-05-24 14:06:57.000000 otpme-0.3.0a78/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    44568 2024-05-24 14:06:58.809777 otpme-0.3.0a78/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1685 2024-05-24 14:06:57.000000 otpme-0.3.0a78/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.761776 otpme-0.3.0a78/bash_completion/
--rw-r--r--   0 root         (0) root         (0)     1937 2024-05-24 14:06:57.000000 otpme-0.3.0a78/bash_completion/otpme
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.761776 otpme-0.3.0a78/deploy/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.765776 otpme-0.3.0a78/deploy/dicts/
--rw-r--r--   0 root         (0) root         (0)     2535 2024-05-24 14:06:57.000000 otpme-0.3.0a78/deploy/dicts/abbreviations-it.gz
--rw-r--r--   0 root         (0) root         (0)    18683 2024-05-24 14:06:57.000000 otpme-0.3.0a78/deploy/dicts/at-surnames.gz
--rw-r--r--   0 root         (0) root         (0)   197269 2024-05-24 14:06:57.000000 otpme-0.3.0a78/deploy/dicts/common-passwords.gz
--rwxr-xr-x   0 root         (0) root         (0)      532 2024-05-24 14:06:57.000000 otpme-0.3.0a78/deploy/dicts/convert_dict.sh
--rw-r--r--   0 root         (0) root         (0)     3286 2024-05-24 14:06:57.000000 otpme-0.3.0a78/deploy/dicts/de-female.gz
--rw-r--r--   0 root         (0) root         (0)     3070 2024-05-24 14:06:57.000000 otpme-0.3.0a78/deploy/dicts/de-male.gz
--rw-r--r--   0 root         (0) root         (0)    11343 2024-05-24 14:06:57.000000 otpme-0.3.0a78/deploy/dicts/de-surnames.gz
--rw-r--r--   0 root         (0) root         (0)    34845 2024-05-24 14:06:57.000000 otpme-0.3.0a78/deploy/dicts/de-top10000.gz
--rw-r--r--   0 root         (0) root         (0)    30600 2024-05-24 14:06:57.000000 otpme-0.3.0a78/deploy/dicts/en-top10000.gz
--rw-r--r--   0 root         (0) root         (0)   127983 2024-05-24 14:06:57.000000 otpme-0.3.0a78/deploy/dicts/english-guessing.gz
--rw-r--r--   0 root         (0) root         (0)  1041710 2024-05-24 14:06:57.000000 otpme-0.3.0a78/deploy/dicts/english.gz
--rw-r--r--   0 root         (0) root         (0)   547291 2024-05-24 14:06:57.000000 otpme-0.3.0a78/deploy/dicts/german-guessing.gz
--rw-r--r--   0 root         (0) root         (0)   544600 2024-05-24 14:06:57.000000 otpme-0.3.0a78/deploy/dicts/german.gz
--rw-r--r--   0 root         (0) root         (0)    13539 2024-05-24 14:06:57.000000 otpme-0.3.0a78/deploy/dicts/us-female.gz
--rw-r--r--   0 root         (0) root         (0)     4089 2024-05-24 14:06:57.000000 otpme-0.3.0a78/deploy/dicts/us-male.gz
--rw-r--r--   0 root         (0) root         (0)    35682 2024-05-24 14:06:57.000000 otpme-0.3.0a78/deploy/dicts/us-surnames.gz
--rw-r--r--   0 root         (0) root         (0)    13331 2024-05-24 14:06:57.000000 otpme-0.3.0a78/deploy/otpme.conf.dist
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.765776 otpme-0.3.0a78/deploy/pam/
--rw-r--r--   0 root         (0) root         (0)     2301 2024-05-24 14:06:57.000000 otpme-0.3.0a78/deploy/pam/README
--rw-r--r--   0 root         (0) root         (0)      155 2024-05-24 14:06:57.000000 otpme-0.3.0a78/deploy/pam/otpme-account
--rw-r--r--   0 root         (0) root         (0)      437 2024-05-24 14:06:57.000000 otpme-0.3.0a78/deploy/pam/otpme-auth
--rw-r--r--   0 root         (0) root         (0)      296 2024-05-24 14:06:57.000000 otpme-0.3.0a78/deploy/pam/otpme-session
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.765776 otpme-0.3.0a78/deploy/pam/pam-python/
--rw-r--r--   0 root         (0) root         (0)      542 2024-05-24 14:06:57.000000 otpme-0.3.0a78/deploy/pam/pam-python/README
--rw-r--r--   0 root         (0) root         (0)     2436 2024-05-24 14:06:57.000000 otpme-0.3.0a78/deploy/pam/pam_otpme.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.765776 otpme-0.3.0a78/deploy/radius/
--rw-r--r--   0 root         (0) root         (0)    13085 2024-05-24 14:06:57.000000 otpme-0.3.0a78/deploy/radius/dictionary
--rw-r--r--   0 root         (0) root         (0)     3851 2024-05-24 14:06:57.000000 otpme-0.3.0a78/deploy/radius/dictionary.freeradius
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.765776 otpme-0.3.0a78/deploy/schema/
--rw-r--r--   0 root         (0) root         (0)    21610 2024-05-24 14:06:57.000000 otpme-0.3.0a78/deploy/schema/core.schema
--rw-r--r--   0 root         (0) root         (0)    73993 2024-05-24 14:06:57.000000 otpme-0.3.0a78/deploy/schema/cosine.schema
--rw-r--r--   0 root         (0) root         (0)     6267 2024-05-24 14:06:57.000000 otpme-0.3.0a78/deploy/schema/inetorgperson.schema
--rw-r--r--   0 root         (0) root         (0)     7632 2024-05-24 14:06:57.000000 otpme-0.3.0a78/deploy/schema/nis.schema
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.765776 otpme-0.3.0a78/deploy/scripts/
--rw-r--r--   0 root         (0) root         (0)     8600 2024-05-24 14:06:57.000000 otpme-0.3.0a78/deploy/scripts/agent_script.sh
--rw-r--r--   0 root         (0) root         (0)       20 2024-05-24 14:06:57.000000 otpme-0.3.0a78/deploy/scripts/auth_script.sh
--rw-r--r--   0 root         (0) root         (0)    21045 2024-05-24 14:06:57.000000 otpme-0.3.0a78/deploy/scripts/key_script.sh
--rw-r--r--   0 root         (0) root         (0)       20 2024-05-24 14:06:57.000000 otpme-0.3.0a78/deploy/scripts/login_script.sh
--rw-r--r--   0 root         (0) root         (0)       20 2024-05-24 14:06:57.000000 otpme-0.3.0a78/deploy/scripts/node_vote_script.sh
--rw-r--r--   0 root         (0) root         (0)       20 2024-05-24 14:06:57.000000 otpme-0.3.0a78/deploy/scripts/push_script.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.765776 otpme-0.3.0a78/otpme/
--rw-r--r--   0 root         (0) root         (0)     1555 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    12650 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/command.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.769776 otpme-0.3.0a78/otpme/lib/
--rw-r--r--   0 root         (0) root         (0)    10420 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1970 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/arp.py
--rw-r--r--   0 root         (0) root         (0)     3502 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/auth_script.py
--rw-r--r--   0 root         (0) root         (0)    48043 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/backend.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.769776 otpme-0.3.0a78/otpme/lib/backends/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/backends/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.773777 otpme-0.3.0a78/otpme/lib/backends/file/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/backends/file/__init__.py
--rw-r--r--   0 root         (0) root         (0)    90185 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/backends/file/file.py
--rw-r--r--   0 root         (0) root         (0)    12946 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/backends/file/index.py
--rw-r--r--   0 root         (0) root         (0)     5831 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/backends/file/models.py
--rw-r--r--   0 root         (0) root         (0)    67194 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/backends/file/transaction.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.773777 otpme-0.3.0a78/otpme/lib/cache/
--rw-r--r--   0 root         (0) root         (0)    27567 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/cache/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3159 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/cache/dogpile.py
--rw-r--r--   0 root         (0) root         (0)    19444 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/cache/funccache.py
--rw-r--r--   0 root         (0) root         (0)     3448 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/cache/lru.py
--rw-r--r--   0 root         (0) root         (0)    14349 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/cache/memcache.py
--rw-r--r--   0 root         (0) root         (0)     6433 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/cache/memcached.py
--rw-r--r--   0 root         (0) root         (0)     7277 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/cache/memcachedb.py
--rw-r--r--   0 root         (0) root         (0)    27128 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/cache/redis.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.777777 otpme-0.3.0a78/otpme/lib/classes/
--rw-r--r--   0 root         (0) root         (0)      890 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/classes/__init__.py
--rw-r--r--   0 root         (0) root         (0)    86180 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/classes/accessgroup.py
--rw-r--r--   0 root         (0) root         (0)    14807 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/classes/agent_conn.py
--rw-r--r--   0 root         (0) root         (0)   126434 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/classes/auth_handler.py
--rw-r--r--   0 root         (0) root         (0)    56607 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/classes/ca.py
--rw-r--r--   0 root         (0) root         (0)    40741 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/classes/client.py
--rw-r--r--   0 root         (0) root         (0)   228970 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/classes/command_handler.py
--rw-r--r--   0 root         (0) root         (0)     8663 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/classes/conn_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.777777 otpme-0.3.0a78/otpme/lib/classes/data_objects/
--rw-r--r--   0 root         (0) root         (0)      813 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/classes/data_objects/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2319 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/classes/data_objects/cert.py
--rw-r--r--   0 root         (0) root         (0)     6798 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/classes/data_objects/data_revision.py
--rw-r--r--   0 root         (0) root         (0)     6813 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/classes/data_objects/failed_pass.py
--rw-r--r--   0 root         (0) root         (0)     8058 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/classes/data_objects/last_assigned_id.py
--rw-r--r--   0 root         (0) root         (0)    10512 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/classes/data_objects/revoked_signature.py
--rw-r--r--   0 root         (0) root         (0)     2503 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/classes/data_objects/rsa_key.py
--rw-r--r--   0 root         (0) root         (0)     6953 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/classes/data_objects/skip_sync.py
--rw-r--r--   0 root         (0) root         (0)     5744 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/classes/data_objects/token_counter.py
--rw-r--r--   0 root         (0) root         (0)     5579 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/classes/data_objects/used_hash.py
--rw-r--r--   0 root         (0) root         (0)     5922 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/classes/data_objects/used_otp.py
--rw-r--r--   0 root         (0) root         (0)     5930 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/classes/data_objects/used_slp.py
--rw-r--r--   0 root         (0) root         (0)     5925 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/classes/data_objects/used_sotp.py
--rw-r--r--   0 root         (0) root         (0)    28615 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/classes/dictionary.py
--rw-r--r--   0 root         (0) root         (0)    39118 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/classes/group.py
--rw-r--r--   0 root         (0) root         (0)    51998 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/classes/host.py
--rw-r--r--   0 root         (0) root         (0)    12229 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/classes/login_handler.py
--rw-r--r--   0 root         (0) root         (0)     5303 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/classes/mgmt_client.py
--rw-r--r--   0 root         (0) root         (0)    38791 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/classes/node.py
--rw-r--r--   0 root         (0) root         (0)    24374 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/classes/object_config.py
--rw-r--r--   0 root         (0) root         (0)    77062 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/classes/otpme_agent.py
--rw-r--r--   0 root         (0) root         (0)    49637 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/classes/otpme_host.py
--rw-r--r--   0 root         (0) root         (0)   318795 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/classes/otpme_object.py
--rw-r--r--   0 root         (0) root         (0)    23290 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/classes/policy.py
--rw-r--r--   0 root         (0) root         (0)    62426 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/classes/realm.py
--rw-r--r--   0 root         (0) root         (0)    74411 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/classes/resolver.py
--rw-r--r--   0 root         (0) root         (0)    45000 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/classes/role.py
--rw-r--r--   0 root         (0) root         (0)    34173 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/classes/script.py
--rw-r--r--   0 root         (0) root         (0)    52532 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/classes/session.py
--rw-r--r--   0 root         (0) root         (0)    31418 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/classes/signing.py
--rw-r--r--   0 root         (0) root         (0)   107184 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/classes/site.py
--rw-r--r--   0 root         (0) root         (0)     6987 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/classes/ssh_agent.py
--rw-r--r--   0 root         (0) root         (0)   134938 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/classes/token.py
--rw-r--r--   0 root         (0) root         (0)    49395 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/classes/unit.py
--rw-r--r--   0 root         (0) root         (0)   182450 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/classes/user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.781777 otpme-0.3.0a78/otpme/lib/cli/
--rw-r--r--   0 root         (0) root         (0)    64574 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12885 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/cli/accessgroup.py
--rw-r--r--   0 root         (0) root         (0)     7119 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/cli/ca.py
--rw-r--r--   0 root         (0) root         (0)    13242 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/cli/client.py
--rw-r--r--   0 root         (0) root         (0)     5643 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/cli/dictionary.py
--rw-r--r--   0 root         (0) root         (0)    12993 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/cli/group.py
--rw-r--r--   0 root         (0) root         (0)    13057 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/cli/host.py
--rw-r--r--   0 root         (0) root         (0)    10974 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/cli/node.py
--rw-r--r--   0 root         (0) root         (0)     6165 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/cli/policy.py
--rw-r--r--   0 root         (0) root         (0)     6174 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/cli/realm.py
--rw-r--r--   0 root         (0) root         (0)     6600 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/cli/resolver.py
--rw-r--r--   0 root         (0) root         (0)    20248 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/cli/role.py
--rw-r--r--   0 root         (0) root         (0)     7383 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/cli/script.py
--rw-r--r--   0 root         (0) root         (0)     7524 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/cli/site.py
--rw-r--r--   0 root         (0) root         (0)    17354 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/cli/token.py
--rw-r--r--   0 root         (0) root         (0)     5423 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/cli/unit.py
--rw-r--r--   0 root         (0) root         (0)     7596 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/cli/user.py
--rw-r--r--   0 root         (0) root         (0)    24867 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/compgen.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.781777 otpme-0.3.0a78/otpme/lib/compression/
--rw-r--r--   0 root         (0) root         (0)      447 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/compression/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4082 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/compression/base.py
--rw-r--r--   0 root         (0) root         (0)    14277 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/connections.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.781777 otpme-0.3.0a78/otpme/lib/daemon/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/daemon/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3785 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/daemon/authd.py
--rw-r--r--   0 root         (0) root         (0)   108965 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/daemon/clusterd.py
--rw-r--r--   0 root         (0) root         (0)    47551 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/daemon/controld.py
--rw-r--r--   0 root         (0) root         (0)    76763 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/daemon/hostd.py
--rw-r--r--   0 root         (0) root         (0)     3074 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/daemon/joind.py
--rw-r--r--   0 root         (0) root         (0)     6713 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/daemon/ldapd.py
--rw-r--r--   0 root         (0) root         (0)     3003 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/daemon/mgmtd.py
--rw-r--r--   0 root         (0) root         (0)    15876 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/daemon/otpme_daemon.py
--rw-r--r--   0 root         (0) root         (0)    11391 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/daemon/scriptd.py
--rw-r--r--   0 root         (0) root         (0)     3017 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/daemon/syncd.py
--rw-r--r--   0 root         (0) root         (0)     6941 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/daemon/unix_daemon.py
--rw-r--r--   0 root         (0) root         (0)    19005 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/debug.py
--rw-r--r--   0 root         (0) root         (0)     2090 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/doc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.781777 otpme-0.3.0a78/otpme/lib/encoding/
--rw-r--r--   0 root         (0) root         (0)      429 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/encoding/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1779 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/encoding/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.781777 otpme-0.3.0a78/otpme/lib/encryption/
--rw-r--r--   0 root         (0) root         (0)     3953 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/encryption/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3296 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/encryption/aes.py
--rw-r--r--   0 root         (0) root         (0)     1479 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/encryption/aes_cfb.py
--rw-r--r--   0 root         (0) root         (0)     7900 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/encryption/argon2.py
--rw-r--r--   0 root         (0) root         (0)    10240 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/encryption/asymmetric_key_handler.py
--rw-r--r--   0 root         (0) root         (0)     4251 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/encryption/ec.py
--rw-r--r--   0 root         (0) root         (0)     2912 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/encryption/fernet.py
--rw-r--r--   0 root         (0) root         (0)     3237 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/encryption/hkdf.py
--rw-r--r--   0 root         (0) root         (0)     3727 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/encryption/pbkdf2.py
--rw-r--r--   0 root         (0) root         (0)     7824 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/encryption/rsa.py
--rw-r--r--   0 root         (0) root         (0)     4324 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.785777 otpme-0.3.0a78/otpme/lib/extensions/
--rw-r--r--   0 root         (0) root         (0)      329 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/extensions/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.785777 otpme-0.3.0a78/otpme/lib/extensions/base/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/extensions/base/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12278 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/extensions/base/base.py
--rw-r--r--   0 root         (0) root         (0)    40152 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/extensions/ldif_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.785777 otpme-0.3.0a78/otpme/lib/extensions/posix/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/extensions/posix/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14286 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/extensions/posix/posix.py
--rw-r--r--   0 root         (0) root         (0)     3640 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/extensions/utils.py
--rw-r--r--   0 root         (0) root         (0)    34081 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/filetools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.785777 otpme-0.3.0a78/otpme/lib/freeradius/
--rw-r--r--   0 root         (0) root         (0)     9119 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/freeradius/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18685 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/freeradius/otpme.py
--rw-r--r--   0 root         (0) root         (0)     1297 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/freeradius/radiusd.py
--rw-r--r--   0 root         (0) root         (0)     1203 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/freeradius/radiusd_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.785777 otpme-0.3.0a78/otpme/lib/gpg/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/gpg/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    28498 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/gpg/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.785777 otpme-0.3.0a78/otpme/lib/help/
--rwxr-xr-x   0 root         (0) root         (0)    26529 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/help/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22986 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/help/accessgroup.py
--rw-r--r--   0 root         (0) root         (0)     5485 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/help/agent.py
--rw-r--r--   0 root         (0) root         (0)     1857 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/help/auth.py
--rw-r--r--   0 root         (0) root         (0)    15707 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/help/ca.py
--rw-r--r--   0 root         (0) root         (0)    16924 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/help/client.py
--rw-r--r--   0 root         (0) root         (0)     1568 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/help/cluster.py
--rw-r--r--   0 root         (0) root         (0)     5785 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/help/controld.py
--rw-r--r--   0 root         (0) root         (0)    11388 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/help/dictionary.py
--rw-r--r--   0 root         (0) root         (0)      522 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/help/get_authorized_keys.py
--rw-r--r--   0 root         (0) root         (0)    19872 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/help/group.py
--rw-r--r--   0 root         (0) root         (0)    24436 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/help/host.py
--rw-r--r--   0 root         (0) root         (0)    21309 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/help/node.py
--rw-r--r--   0 root         (0) root         (0)      477 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/help/pinentry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.789777 otpme-0.3.0a78/otpme/lib/help/policy/
--rw-r--r--   0 root         (0) root         (0)     8386 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/help/policy/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3710 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/help/policy/authonaction.py
--rw-r--r--   0 root         (0) root         (0)     1247 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/help/policy/autodisable.py
--rw-r--r--   0 root         (0) root         (0)     1751 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/help/policy/defaultgroups.py
--rw-r--r--   0 root         (0) root         (0)     1559 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/help/policy/defaultpolicies.py
--rw-r--r--   0 root         (0) root         (0)     1421 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/help/policy/defaultroles.py
--rw-r--r--   0 root         (0) root         (0)     1836 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/help/policy/defaultunits.py
--rw-r--r--   0 root         (0) root         (0)     1492 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/help/policy/forcetoken.py
--rw-r--r--   0 root         (0) root         (0)     2230 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/help/policy/idrange.py
--rw-r--r--   0 root         (0) root         (0)     1831 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/help/policy/logintimes.py
--rw-r--r--   0 root         (0) root         (0)     1098 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/help/policy/objecttemplates.py
--rw-r--r--   0 root         (0) root         (0)     3463 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/help/policy/password.py
--rw-r--r--   0 root         (0) root         (0)     2779 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/help/policy/tokenacls.py
--rw-r--r--   0 root         (0) root         (0)    20037 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/help/realm.py
--rw-r--r--   0 root         (0) root         (0)     1441 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/help/register.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.789777 otpme-0.3.0a78/otpme/lib/help/resolver/
--rw-r--r--   0 root         (0) root         (0)    12522 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/help/resolver/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4465 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/help/resolver/ldap.py
--rw-r--r--   0 root         (0) root         (0)    18198 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/help/role.py
--rw-r--r--   0 root         (0) root         (0)    15111 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/help/script.py
--rw-r--r--   0 root         (0) root         (0)     2844 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/help/session.py
--rw-r--r--   0 root         (0) root         (0)    22488 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/help/site.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.789777 otpme-0.3.0a78/otpme/lib/help/token/
--rw-r--r--   0 root         (0) root         (0)    20503 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/help/token/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1385 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/help/token/fido2.py
--rw-r--r--   0 root         (0) root         (0)     5752 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/help/token/hotp.py
--rw-r--r--   0 root         (0) root         (0)     6339 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/help/token/motp.py
--rw-r--r--   0 root         (0) root         (0)     1991 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/help/token/otp_push.py
--rw-r--r--   0 root         (0) root         (0)     4951 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/help/token/otpme.py
--rw-r--r--   0 root         (0) root         (0)     4029 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/help/token/password.py
--rw-r--r--   0 root         (0) root         (0)     7251 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/help/token/ssh.py
--rw-r--r--   0 root         (0) root         (0)     5977 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/help/token/totp.py
--rw-r--r--   0 root         (0) root         (0)     5803 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/help/token/yubikey_hmac.py
--rw-r--r--   0 root         (0) root         (0)     1252 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/help/token/yubikey_hotp.py
--rw-r--r--   0 root         (0) root         (0)    24935 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/help/tool.py
--rw-r--r--   0 root         (0) root         (0)    15168 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/help/unit.py
--rw-r--r--   0 root         (0) root         (0)    29509 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/help/user.py
--rw-r--r--   0 root         (0) root         (0)    16341 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/host.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.789777 otpme-0.3.0a78/otpme/lib/humanize/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/humanize/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4191 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/humanize/units.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.789777 otpme-0.3.0a78/otpme/lib/index/
--rw-r--r--   0 root         (0) root         (0)      382 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/index/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23948 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/index/mysql.py
--rw-r--r--   0 root         (0) root         (0)    24542 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/index/postgres.py
--rw-r--r--   0 root         (0) root         (0)     8336 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/index/sqlite3.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.789777 otpme-0.3.0a78/otpme/lib/job/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/job/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20681 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/job/callback.py
--rw-r--r--   0 root         (0) root         (0)    12849 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/job/otpme_job.py
--rw-r--r--   0 root         (0) root         (0)    37097 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/join.py
--rw-r--r--   0 root         (0) root         (0)     4857 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/json.py
--rw-r--r--   0 root         (0) root         (0)     1942 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/jwt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.789777 otpme-0.3.0a78/otpme/lib/ldap/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/ldap/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1354 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/ldap/client.py
--rw-r--r--   0 root         (0) root         (0)    11062 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/ldap/schema.py
--rw-r--r--   0 root         (0) root         (0)    50483 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/ldap/server.py
--rw-r--r--   0 root         (0) root         (0)    19709 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/locking.py
--rw-r--r--   0 root         (0) root         (0)     9430 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/log.py
--rw-r--r--   0 root         (0) root         (0)     1529 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/messages.py
--rw-r--r--   0 root         (0) root         (0)     5981 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/mschap.py
--rw-r--r--   0 root         (0) root         (0)     2366 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/mschap_util.py
--rw-r--r--   0 root         (0) root         (0)    35744 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/multiprocessing.py
--rw-r--r--   0 root         (0) root         (0)    10250 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/net.py
--rw-r--r--   0 root         (0) root         (0)    27144 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/nsscache.py
--rw-r--r--   0 root         (0) root         (0)    63328 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/offline_token.py
--rw-r--r--   0 root         (0) root         (0)    23778 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/oid.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.789777 otpme-0.3.0a78/otpme/lib/otp/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/otp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.789777 otpme-0.3.0a78/otpme/lib/otp/oath/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/otp/oath/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1727 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/otp/oath/hotp.py
--rw-r--r--   0 root         (0) root         (0)     1581 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/otp/oath/totp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.793777 otpme-0.3.0a78/otpme/lib/otp/otpme/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/otp/otpme/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3087 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/otp/otpme/otpme.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.793777 otpme-0.3.0a78/otpme/lib/otp/yubico/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/otp/yubico/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3026 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/otp/yubico/yubiotp.py
--rw-r--r--   0 root         (0) root         (0)    19837 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/otpme_acl.py
--rw-r--r--   0 root         (0) root         (0)   115772 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/otpme_config.py
--rw-r--r--   0 root         (0) root         (0)     3519 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/otpme_pass.py
--rw-r--r--   0 root         (0) root         (0)    70359 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/pam.py
--rw-r--r--   0 root         (0) root         (0)     1975 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/pickle.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.793777 otpme-0.3.0a78/otpme/lib/pinentry/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/pinentry/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27465 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/pinentry/pinentry.py
--rwxr-xr-x   0 root         (0) root         (0)     7880 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/pinentry/wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.793777 otpme-0.3.0a78/otpme/lib/pki/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/pki/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9797 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/pki/cert.py
--rw-r--r--   0 root         (0) root         (0)    23150 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/pki/utils.py
--rw-r--r--   0 root         (0) root         (0)    16890 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/pki/utils_openssl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.793777 otpme-0.3.0a78/otpme/lib/policy/
--rw-r--r--   0 root         (0) root         (0)     2099 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/policy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.793777 otpme-0.3.0a78/otpme/lib/policy/authonaction/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/policy/authonaction/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32663 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/policy/authonaction/authonaction.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.793777 otpme-0.3.0a78/otpme/lib/policy/autodisable/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/policy/autodisable/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15718 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/policy/autodisable/autodisable.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.793777 otpme-0.3.0a78/otpme/lib/policy/defaultgroups/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/policy/defaultgroups/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17570 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/policy/defaultgroups/defaultgroups.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.793777 otpme-0.3.0a78/otpme/lib/policy/defaultpolicies/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/policy/defaultpolicies/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14510 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/policy/defaultpolicies/defaultpolicies.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.793777 otpme-0.3.0a78/otpme/lib/policy/defaultroles/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/policy/defaultroles/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14217 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/policy/defaultroles/defaultroles.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.793777 otpme-0.3.0a78/otpme/lib/policy/defaultunits/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/policy/defaultunits/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15637 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/policy/defaultunits/defaultunits.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.793777 otpme-0.3.0a78/otpme/lib/policy/forcetoken/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/policy/forcetoken/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14202 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/policy/forcetoken/forcetoken.py
--rw-r--r--   0 root         (0) root         (0)     1176 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/policy/get_class.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.793777 otpme-0.3.0a78/otpme/lib/policy/idrange/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/policy/idrange/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27256 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/policy/idrange/idrange.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.793777 otpme-0.3.0a78/otpme/lib/policy/logintimes/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/policy/logintimes/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18083 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/policy/logintimes/logintimes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.793777 otpme-0.3.0a78/otpme/lib/policy/objecttemplates/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/policy/objecttemplates/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14954 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/policy/objecttemplates/objecttemplates.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.793777 otpme-0.3.0a78/otpme/lib/policy/password/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/policy/password/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29128 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/policy/password/password.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.793777 otpme-0.3.0a78/otpme/lib/policy/tokenacls/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/policy/tokenacls/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24897 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/policy/tokenacls/tokenacls.py
--rw-r--r--   0 root         (0) root         (0)      491 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/policy/utils.py
--rw-r--r--   0 root         (0) root         (0)     9332 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/preload.py
--rw-r--r--   0 root         (0) root         (0)     2466 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/progress.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.797777 otpme-0.3.0a78/otpme/lib/protocols/
--rw-r--r--   0 root         (0) root         (0)      304 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/protocols/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.797777 otpme-0.3.0a78/otpme/lib/protocols/client/
--rw-r--r--   0 root         (0) root         (0)      655 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/protocols/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1887 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/protocols/client/agent1.py
--rw-r--r--   0 root         (0) root         (0)      832 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/protocols/client/auth1.py
--rw-r--r--   0 root         (0) root         (0)    14301 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/protocols/client/cluster1.py
--rw-r--r--   0 root         (0) root         (0)     1046 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/protocols/client/get_class.py
--rw-r--r--   0 root         (0) root         (0)     4645 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/protocols/client/host1.py
--rw-r--r--   0 root         (0) root         (0)      832 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/protocols/client/join1.py
--rwxr-xr-x   0 root         (0) root         (0)    11305 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/protocols/client/mgmt1.py
--rw-r--r--   0 root         (0) root         (0)    67975 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/protocols/client/sync1.py
--rw-r--r--   0 root         (0) root         (0)   160693 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/protocols/otpme_client.py
--rw-r--r--   0 root         (0) root         (0)    81420 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/protocols/otpme_server.py
--rw-r--r--   0 root         (0) root         (0)     1601 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/protocols/request.py
--rw-r--r--   0 root         (0) root         (0)     1770 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/protocols/response.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.797777 otpme-0.3.0a78/otpme/lib/protocols/server/
--rw-r--r--   0 root         (0) root         (0)      827 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/protocols/server/__init__.py
--rw-r--r--   0 root         (0) root         (0)    40219 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/protocols/server/agent1.py
--rw-r--r--   0 root         (0) root         (0)    12842 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/protocols/server/auth1.py
--rw-r--r--   0 root         (0) root         (0)    32302 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/protocols/server/cluster1.py
--rw-r--r--   0 root         (0) root         (0)     1912 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/protocols/server/get_class.py
--rw-r--r--   0 root         (0) root         (0)    26608 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/protocols/server/host1.py
--rw-r--r--   0 root         (0) root         (0)    52562 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/protocols/server/join1.py
--rw-r--r--   0 root         (0) root         (0)    70866 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/protocols/server/mgmt1.py
--rw-r--r--   0 root         (0) root         (0)    45433 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/protocols/server/sync1.py
--rw-r--r--   0 root         (0) root         (0)      527 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/protocols/status_codes.py
--rw-r--r--   0 root         (0) root         (0)     6937 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/protocols/utils.py
--rw-r--r--   0 root         (0) root         (0)     2157 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/push_script.py
--rw-r--r--   0 root         (0) root         (0)     1139 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/qrcode.py
--rw-r--r--   0 root         (0) root         (0)      478 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/re.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.797777 otpme-0.3.0a78/otpme/lib/register/
--rw-r--r--   0 root         (0) root         (0)     9716 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/register/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.797777 otpme-0.3.0a78/otpme/lib/resolver/
--rw-r--r--   0 root         (0) root         (0)      485 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/resolver/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1158 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/resolver/get_class.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.797777 otpme-0.3.0a78/otpme/lib/resolver/ldap/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/resolver/ldap/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39438 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/resolver/ldap/ldap.py
--rw-r--r--   0 root         (0) root         (0)      451 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/resolver/utils.py
--rw-r--r--   0 root         (0) root         (0)    10019 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/script.py
--rw-r--r--   0 root         (0) root         (0)     3005 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/sign_key_cache.py
--rw-r--r--   0 root         (0) root         (0)      537 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/slp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.797777 otpme-0.3.0a78/otpme/lib/smartcard/
--rw-r--r--   0 root         (0) root         (0)      623 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/smartcard/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.797777 otpme-0.3.0a78/otpme/lib/smartcard/fido2/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/smartcard/fido2/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10161 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/smartcard/fido2/fido2.py
--rw-r--r--   0 root         (0) root         (0)      858 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/smartcard/get_class.py
--rw-r--r--   0 root         (0) root         (0)     1666 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/smartcard/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.801777 otpme-0.3.0a78/otpme/lib/smartcard/yubikey/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/smartcard/yubikey/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11951 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/smartcard/yubikey/deploy.py
--rw-r--r--   0 root         (0) root         (0)     1982 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/smartcard/yubikey/usb.py
--rw-r--r--   0 root         (0) root         (0)     8075 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/smartcard/yubikey/yubikey.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.801777 otpme-0.3.0a78/otpme/lib/smartcard/yubikey_gpg/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/smartcard/yubikey_gpg/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6364 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/smartcard/yubikey_gpg/yubikey_gpg.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.801777 otpme-0.3.0a78/otpme/lib/smartcard/yubikey_hmac/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/smartcard/yubikey_hmac/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11955 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/smartcard/yubikey_hmac/yubikey_hmac.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.801777 otpme-0.3.0a78/otpme/lib/smartcard/yubikey_hotp/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/smartcard/yubikey_hotp/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5032 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/smartcard/yubikey_hotp/yubikey_hotp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.801777 otpme-0.3.0a78/otpme/lib/socket/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/socket/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13152 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/socket/connect.py
--rw-r--r--   0 root         (0) root         (0)     8450 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/socket/handler.py
--rw-r--r--   0 root         (0) root         (0)    30962 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/socket/listen.py
--rw-r--r--   0 root         (0) root         (0)     2830 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/socket/send_recv1.py
--rw-r--r--   0 root         (0) root         (0)     4408 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/sotp.py
--rwxr-xr-x   0 root         (0) root         (0)    37113 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/spsc.py
--rw-r--r--   0 root         (0) root         (0)      544 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/srp.py
--rw-r--r--   0 root         (0) root         (0)    23454 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/ssh.py
--rw-r--r--   0 root         (0) root         (0)    63673 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/stuff.py
--rw-r--r--   0 root         (0) root         (0)    12338 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/sync_cache.py
--rw-r--r--   0 root         (0) root         (0)     4636 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/system_command.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.801777 otpme-0.3.0a78/otpme/lib/third_party/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/third_party/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.801777 otpme-0.3.0a78/otpme/lib/third_party/dogpile_caching/
--rw-r--r--   0 root         (0) root         (0)     1981 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/third_party/dogpile_caching/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3021 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/third_party/dogpile_caching/advanced.py
--rw-r--r--   0 root         (0) root         (0)     9859 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/third_party/dogpile_caching/caching_query.py
--rw-r--r--   0 root         (0) root         (0)     2250 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/third_party/dogpile_caching/environment.py
--rw-r--r--   0 root         (0) root         (0)     1764 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/third_party/dogpile_caching/fixture_data.py
--rw-r--r--   0 root         (0) root         (0)     2248 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/third_party/dogpile_caching/helloworld.py
--rw-r--r--   0 root         (0) root         (0)     3310 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/third_party/dogpile_caching/local_session_caching.py
--rw-r--r--   0 root         (0) root         (0)     3033 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/third_party/dogpile_caching/model.py
--rw-r--r--   0 root         (0) root         (0)     1040 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/third_party/dogpile_caching/relationship_caching.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.801777 otpme-0.3.0a78/otpme/lib/third_party/nss_cache/
--rw-r--r--   0 root         (0) root         (0)     1140 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/third_party/nss_cache/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.801777 otpme-0.3.0a78/otpme/lib/third_party/nss_cache/caches/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/third_party/nss_cache/caches/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9083 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/third_party/nss_cache/caches/caches.py
--rw-r--r--   0 root         (0) root         (0)    14341 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/third_party/nss_cache/caches/files.py
--rw-r--r--   0 root         (0) root         (0)     1044 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/third_party/nss_cache/config.py
--rw-r--r--   0 root         (0) root         (0)     1959 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/third_party/nss_cache/error.py
--rw-r--r--   0 root         (0) root         (0)     7963 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/third_party/nss_cache/lock.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.801777 otpme-0.3.0a78/otpme/lib/third_party/nss_cache/maps/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/third_party/nss_cache/maps/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2389 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/third_party/nss_cache/maps/group.py
--rw-r--r--   0 root         (0) root         (0)    11745 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/third_party/nss_cache/maps/maps.py
--rw-r--r--   0 root         (0) root         (0)     2554 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/third_party/nss_cache/maps/passwd.py
--rw-r--r--   0 root         (0) root         (0)     2387 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/third_party/nss_cache/maps/shadow.py
--rw-r--r--   0 root         (0) root         (0)     4140 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/third_party/nss_cache/nss.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.805777 otpme-0.3.0a78/otpme/lib/third_party/nss_cache/update/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/third_party/nss_cache/update/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5487 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/third_party/nss_cache/update/files_updater.py
--rw-r--r--   0 root         (0) root         (0)     5826 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/third_party/nss_cache/update/map_updater.py
--rw-r--r--   0 root         (0) root         (0)    10980 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/third_party/nss_cache/update/updater.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.805777 otpme-0.3.0a78/otpme/lib/third_party/nss_cache/util/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/third_party/nss_cache/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4117 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/third_party/nss_cache/util/file_formats.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.805777 otpme-0.3.0a78/otpme/lib/third_party/oath_toolkit/
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/third_party/oath_toolkit/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1592 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/third_party/oath_toolkit/_compat.py
--rw-r--r--   0 root         (0) root         (0)     1772 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/third_party/oath_toolkit/uri.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.805777 otpme-0.3.0a78/otpme/lib/token/
--rw-r--r--   0 root         (0) root         (0)      953 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/token/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.805777 otpme-0.3.0a78/otpme/lib/token/fido2/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/token/fido2/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14939 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/token/fido2/fido2.py
--rw-r--r--   0 root         (0) root         (0)     1056 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/token/get_class.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.805777 otpme-0.3.0a78/otpme/lib/token/hotp/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/token/hotp/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39346 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/token/hotp/hotp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.805777 otpme-0.3.0a78/otpme/lib/token/link/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/token/link/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9656 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/token/link/link.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.805777 otpme-0.3.0a78/otpme/lib/token/motp/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/token/motp/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27770 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/token/motp/motp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.805777 otpme-0.3.0a78/otpme/lib/token/oath/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/token/oath/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19667 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/token/oath/oath.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.805777 otpme-0.3.0a78/otpme/lib/token/otp_push/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/token/otp_push/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23393 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/token/otp_push/otp_push.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.805777 otpme-0.3.0a78/otpme/lib/token/otpme/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/token/otpme/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24704 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/token/otpme/otpme.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.805777 otpme-0.3.0a78/otpme/lib/token/password/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/token/password/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26906 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/token/password/password.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.805777 otpme-0.3.0a78/otpme/lib/token/script_otp/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/token/script_otp/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9677 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/token/script_otp/script_otp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.805777 otpme-0.3.0a78/otpme/lib/token/script_static/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/token/script_static/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9677 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/token/script_static/script_static.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.805777 otpme-0.3.0a78/otpme/lib/token/ssh/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/token/ssh/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39547 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/token/ssh/ssh.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.805777 otpme-0.3.0a78/otpme/lib/token/totp/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/token/totp/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35398 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/token/totp/totp.py
--rw-r--r--   0 root         (0) root         (0)      480 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/token/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.805777 otpme-0.3.0a78/otpme/lib/token/yubikey_hmac/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/token/yubikey_hmac/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25111 2024-05-24 14:06:57.000000 otpme-0.3.0a78/otpme/lib/token/yubikey_hmac/yubikey_hmac.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:06:58.805777 otpme-0.3.0a78/otpme.egg-info/
--rw-r--r--   0 root         (0) root         (0)    44568 2024-05-24 14:06:58.000000 otpme-0.3.0a78/otpme.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    13484 2024-05-24 14:06:58.000000 otpme-0.3.0a78/otpme.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-24 14:06:58.000000 otpme-0.3.0a78/otpme.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1080 2024-05-24 14:06:58.000000 otpme-0.3.0a78/otpme.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-24 14:06:58.000000 otpme-0.3.0a78/otpme.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      924 2024-05-24 14:06:58.000000 otpme-0.3.0a78/otpme.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-05-24 14:06:58.000000 otpme-0.3.0a78/otpme.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2249 2024-05-24 14:06:57.000000 otpme-0.3.0a78/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1310 2024-05-24 14:06:57.000000 otpme-0.3.0a78/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-24 14:06:58.809777 otpme-0.3.0a78/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     9305 2024-05-24 14:06:57.000000 otpme-0.3.0a78/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.940491 otpme-0.3.0a79/
+-rw-r--r--   0 root         (0) root         (0)    35121 2024-06-03 13:51:55.000000 otpme-0.3.0a79/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      665 2024-06-03 13:51:55.000000 otpme-0.3.0a79/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    44692 2024-06-03 13:51:56.940491 otpme-0.3.0a79/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1685 2024-06-03 13:51:55.000000 otpme-0.3.0a79/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.884490 otpme-0.3.0a79/bash_completion/
+-rw-r--r--   0 root         (0) root         (0)     1937 2024-06-03 13:51:55.000000 otpme-0.3.0a79/bash_completion/otpme
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.884490 otpme-0.3.0a79/deploy/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.896490 otpme-0.3.0a79/deploy/dicts/
+-rw-r--r--   0 root         (0) root         (0)     2535 2024-06-03 13:51:55.000000 otpme-0.3.0a79/deploy/dicts/abbreviations-it.gz
+-rw-r--r--   0 root         (0) root         (0)    18683 2024-06-03 13:51:55.000000 otpme-0.3.0a79/deploy/dicts/at-surnames.gz
+-rw-r--r--   0 root         (0) root         (0)   197269 2024-06-03 13:51:55.000000 otpme-0.3.0a79/deploy/dicts/common-passwords.gz
+-rwxr-xr-x   0 root         (0) root         (0)      532 2024-06-03 13:51:55.000000 otpme-0.3.0a79/deploy/dicts/convert_dict.sh
+-rw-r--r--   0 root         (0) root         (0)     3286 2024-06-03 13:51:55.000000 otpme-0.3.0a79/deploy/dicts/de-female.gz
+-rw-r--r--   0 root         (0) root         (0)     3070 2024-06-03 13:51:55.000000 otpme-0.3.0a79/deploy/dicts/de-male.gz
+-rw-r--r--   0 root         (0) root         (0)    11343 2024-06-03 13:51:55.000000 otpme-0.3.0a79/deploy/dicts/de-surnames.gz
+-rw-r--r--   0 root         (0) root         (0)    34845 2024-06-03 13:51:55.000000 otpme-0.3.0a79/deploy/dicts/de-top10000.gz
+-rw-r--r--   0 root         (0) root         (0)    30600 2024-06-03 13:51:55.000000 otpme-0.3.0a79/deploy/dicts/en-top10000.gz
+-rw-r--r--   0 root         (0) root         (0)   127983 2024-06-03 13:51:55.000000 otpme-0.3.0a79/deploy/dicts/english-guessing.gz
+-rw-r--r--   0 root         (0) root         (0)  1041710 2024-06-03 13:51:55.000000 otpme-0.3.0a79/deploy/dicts/english.gz
+-rw-r--r--   0 root         (0) root         (0)   547291 2024-06-03 13:51:55.000000 otpme-0.3.0a79/deploy/dicts/german-guessing.gz
+-rw-r--r--   0 root         (0) root         (0)   544600 2024-06-03 13:51:55.000000 otpme-0.3.0a79/deploy/dicts/german.gz
+-rw-r--r--   0 root         (0) root         (0)    13539 2024-06-03 13:51:55.000000 otpme-0.3.0a79/deploy/dicts/us-female.gz
+-rw-r--r--   0 root         (0) root         (0)     4089 2024-06-03 13:51:55.000000 otpme-0.3.0a79/deploy/dicts/us-male.gz
+-rw-r--r--   0 root         (0) root         (0)    35682 2024-06-03 13:51:55.000000 otpme-0.3.0a79/deploy/dicts/us-surnames.gz
+-rw-r--r--   0 root         (0) root         (0)    13331 2024-06-03 13:51:55.000000 otpme-0.3.0a79/deploy/otpme.conf.dist
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.896490 otpme-0.3.0a79/deploy/pam/
+-rw-r--r--   0 root         (0) root         (0)     2301 2024-06-03 13:51:55.000000 otpme-0.3.0a79/deploy/pam/README
+-rw-r--r--   0 root         (0) root         (0)      155 2024-06-03 13:51:55.000000 otpme-0.3.0a79/deploy/pam/otpme-account
+-rw-r--r--   0 root         (0) root         (0)      437 2024-06-03 13:51:55.000000 otpme-0.3.0a79/deploy/pam/otpme-auth
+-rw-r--r--   0 root         (0) root         (0)      296 2024-06-03 13:51:55.000000 otpme-0.3.0a79/deploy/pam/otpme-session
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.896490 otpme-0.3.0a79/deploy/pam/pam-python/
+-rw-r--r--   0 root         (0) root         (0)      542 2024-06-03 13:51:55.000000 otpme-0.3.0a79/deploy/pam/pam-python/README
+-rw-r--r--   0 root         (0) root         (0)     2436 2024-06-03 13:51:55.000000 otpme-0.3.0a79/deploy/pam/pam_otpme.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.896490 otpme-0.3.0a79/deploy/radius/
+-rw-r--r--   0 root         (0) root         (0)    13085 2024-06-03 13:51:55.000000 otpme-0.3.0a79/deploy/radius/dictionary
+-rw-r--r--   0 root         (0) root         (0)     3851 2024-06-03 13:51:55.000000 otpme-0.3.0a79/deploy/radius/dictionary.freeradius
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.896490 otpme-0.3.0a79/deploy/schema/
+-rw-r--r--   0 root         (0) root         (0)    21610 2024-06-03 13:51:55.000000 otpme-0.3.0a79/deploy/schema/core.schema
+-rw-r--r--   0 root         (0) root         (0)    73993 2024-06-03 13:51:55.000000 otpme-0.3.0a79/deploy/schema/cosine.schema
+-rw-r--r--   0 root         (0) root         (0)     6267 2024-06-03 13:51:55.000000 otpme-0.3.0a79/deploy/schema/inetorgperson.schema
+-rw-r--r--   0 root         (0) root         (0)     7632 2024-06-03 13:51:55.000000 otpme-0.3.0a79/deploy/schema/nis.schema
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.896490 otpme-0.3.0a79/deploy/scripts/
+-rw-r--r--   0 root         (0) root         (0)     8600 2024-06-03 13:51:55.000000 otpme-0.3.0a79/deploy/scripts/agent_script.sh
+-rw-r--r--   0 root         (0) root         (0)       20 2024-06-03 13:51:55.000000 otpme-0.3.0a79/deploy/scripts/auth_script.sh
+-rw-r--r--   0 root         (0) root         (0)    21045 2024-06-03 13:51:55.000000 otpme-0.3.0a79/deploy/scripts/key_script.sh
+-rw-r--r--   0 root         (0) root         (0)       20 2024-06-03 13:51:55.000000 otpme-0.3.0a79/deploy/scripts/login_script.sh
+-rw-r--r--   0 root         (0) root         (0)       20 2024-06-03 13:51:55.000000 otpme-0.3.0a79/deploy/scripts/node_vote_script.sh
+-rw-r--r--   0 root         (0) root         (0)       20 2024-06-03 13:51:55.000000 otpme-0.3.0a79/deploy/scripts/push_script.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.896490 otpme-0.3.0a79/otpme/
+-rw-r--r--   0 root         (0) root         (0)     1555 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    12650 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/command.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.904490 otpme-0.3.0a79/otpme/lib/
+-rw-r--r--   0 root         (0) root         (0)    10420 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1970 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/arp.py
+-rw-r--r--   0 root         (0) root         (0)     3502 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/auth_script.py
+-rw-r--r--   0 root         (0) root         (0)    45393 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/backend.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.904490 otpme-0.3.0a79/otpme/lib/backends/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/backends/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.904490 otpme-0.3.0a79/otpme/lib/backends/file/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/backends/file/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    90398 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/backends/file/file.py
+-rw-r--r--   0 root         (0) root         (0)    12946 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/backends/file/index.py
+-rw-r--r--   0 root         (0) root         (0)     5831 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/backends/file/models.py
+-rw-r--r--   0 root         (0) root         (0)    67531 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/backends/file/transaction.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.904490 otpme-0.3.0a79/otpme/lib/cache/
+-rw-r--r--   0 root         (0) root         (0)    27567 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/cache/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3159 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/cache/dogpile.py
+-rw-r--r--   0 root         (0) root         (0)    19444 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/cache/funccache.py
+-rw-r--r--   0 root         (0) root         (0)     3448 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/cache/lru.py
+-rw-r--r--   0 root         (0) root         (0)    14349 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/cache/memcache.py
+-rw-r--r--   0 root         (0) root         (0)     6433 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/cache/memcached.py
+-rw-r--r--   0 root         (0) root         (0)     7277 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/cache/memcachedb.py
+-rw-r--r--   0 root         (0) root         (0)    27128 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/cache/redis.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.908491 otpme-0.3.0a79/otpme/lib/classes/
+-rw-r--r--   0 root         (0) root         (0)      890 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/classes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    86180 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/classes/accessgroup.py
+-rw-r--r--   0 root         (0) root         (0)    14859 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/classes/agent_conn.py
+-rw-r--r--   0 root         (0) root         (0)   129680 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/classes/auth_handler.py
+-rw-r--r--   0 root         (0) root         (0)    56607 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/classes/ca.py
+-rw-r--r--   0 root         (0) root         (0)    47860 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/classes/client.py
+-rw-r--r--   0 root         (0) root         (0)   228905 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/classes/command_handler.py
+-rw-r--r--   0 root         (0) root         (0)     8663 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/classes/conn_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.912490 otpme-0.3.0a79/otpme/lib/classes/data_objects/
+-rw-r--r--   0 root         (0) root         (0)      769 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/classes/data_objects/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2319 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/classes/data_objects/cert.py
+-rw-r--r--   0 root         (0) root         (0)     6798 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/classes/data_objects/data_revision.py
+-rw-r--r--   0 root         (0) root         (0)     6813 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/classes/data_objects/failed_pass.py
+-rw-r--r--   0 root         (0) root         (0)     8058 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/classes/data_objects/last_assigned_id.py
+-rw-r--r--   0 root         (0) root         (0)    10512 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/classes/data_objects/revoked_signature.py
+-rw-r--r--   0 root         (0) root         (0)     2503 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/classes/data_objects/rsa_key.py
+-rw-r--r--   0 root         (0) root         (0)     6953 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/classes/data_objects/skip_sync.py
+-rw-r--r--   0 root         (0) root         (0)     5744 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/classes/data_objects/token_counter.py
+-rw-r--r--   0 root         (0) root         (0)     5579 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/classes/data_objects/used_hash.py
+-rw-r--r--   0 root         (0) root         (0)     5922 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/classes/data_objects/used_otp.py
+-rw-r--r--   0 root         (0) root         (0)     5925 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/classes/data_objects/used_sotp.py
+-rw-r--r--   0 root         (0) root         (0)    28615 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/classes/dictionary.py
+-rw-r--r--   0 root         (0) root         (0)    39118 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/classes/group.py
+-rw-r--r--   0 root         (0) root         (0)    51998 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/classes/host.py
+-rw-r--r--   0 root         (0) root         (0)    12229 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/classes/login_handler.py
+-rw-r--r--   0 root         (0) root         (0)     5303 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/classes/mgmt_client.py
+-rw-r--r--   0 root         (0) root         (0)    38791 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/classes/node.py
+-rw-r--r--   0 root         (0) root         (0)    24374 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/classes/object_config.py
+-rw-r--r--   0 root         (0) root         (0)    76962 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/classes/otpme_agent.py
+-rw-r--r--   0 root         (0) root         (0)    49637 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/classes/otpme_host.py
+-rw-r--r--   0 root         (0) root         (0)   315740 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/classes/otpme_object.py
+-rw-r--r--   0 root         (0) root         (0)    23290 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/classes/policy.py
+-rw-r--r--   0 root         (0) root         (0)    62426 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/classes/realm.py
+-rw-r--r--   0 root         (0) root         (0)    74411 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/classes/resolver.py
+-rw-r--r--   0 root         (0) root         (0)    45000 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/classes/role.py
+-rw-r--r--   0 root         (0) root         (0)    34173 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/classes/script.py
+-rw-r--r--   0 root         (0) root         (0)    53490 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/classes/session.py
+-rw-r--r--   0 root         (0) root         (0)    31418 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/classes/signing.py
+-rw-r--r--   0 root         (0) root         (0)   116847 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/classes/site.py
+-rw-r--r--   0 root         (0) root         (0)     6987 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/classes/ssh_agent.py
+-rw-r--r--   0 root         (0) root         (0)   134938 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/classes/token.py
+-rw-r--r--   0 root         (0) root         (0)    49395 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/classes/unit.py
+-rw-r--r--   0 root         (0) root         (0)   185447 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/classes/user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.912490 otpme-0.3.0a79/otpme/lib/cli/
+-rw-r--r--   0 root         (0) root         (0)    64183 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12885 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/cli/accessgroup.py
+-rw-r--r--   0 root         (0) root         (0)     7119 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/cli/ca.py
+-rw-r--r--   0 root         (0) root         (0)    13242 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/cli/client.py
+-rw-r--r--   0 root         (0) root         (0)     5643 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/cli/dictionary.py
+-rw-r--r--   0 root         (0) root         (0)    12993 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/cli/group.py
+-rw-r--r--   0 root         (0) root         (0)    13057 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/cli/host.py
+-rw-r--r--   0 root         (0) root         (0)    10974 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/cli/node.py
+-rw-r--r--   0 root         (0) root         (0)     6165 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/cli/policy.py
+-rw-r--r--   0 root         (0) root         (0)     6174 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/cli/realm.py
+-rw-r--r--   0 root         (0) root         (0)     6600 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/cli/resolver.py
+-rw-r--r--   0 root         (0) root         (0)    20248 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/cli/role.py
+-rw-r--r--   0 root         (0) root         (0)     7383 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/cli/script.py
+-rw-r--r--   0 root         (0) root         (0)     7524 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/cli/site.py
+-rw-r--r--   0 root         (0) root         (0)    17354 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/cli/token.py
+-rw-r--r--   0 root         (0) root         (0)     5423 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/cli/unit.py
+-rw-r--r--   0 root         (0) root         (0)     7596 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/cli/user.py
+-rw-r--r--   0 root         (0) root         (0)    24867 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/compgen.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.912490 otpme-0.3.0a79/otpme/lib/compression/
+-rw-r--r--   0 root         (0) root         (0)      447 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/compression/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4082 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/compression/base.py
+-rw-r--r--   0 root         (0) root         (0)    14277 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/connections.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.916491 otpme-0.3.0a79/otpme/lib/daemon/
+-rw-r--r--   0 root         (0) root         (0)      652 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/daemon/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3785 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/daemon/authd.py
+-rw-r--r--   0 root         (0) root         (0)   111190 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/daemon/clusterd.py
+-rw-r--r--   0 root         (0) root         (0)    47741 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/daemon/controld.py
+-rw-r--r--   0 root         (0) root         (0)    76412 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/daemon/hostd.py
+-rw-r--r--   0 root         (0) root         (0)     6189 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/daemon/httpd.py
+-rw-r--r--   0 root         (0) root         (0)     3074 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/daemon/joind.py
+-rw-r--r--   0 root         (0) root         (0)     6713 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/daemon/ldapd.py
+-rw-r--r--   0 root         (0) root         (0)     3003 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/daemon/mgmtd.py
+-rw-r--r--   0 root         (0) root         (0)    15876 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/daemon/otpme_daemon.py
+-rw-r--r--   0 root         (0) root         (0)    11391 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/daemon/scriptd.py
+-rw-r--r--   0 root         (0) root         (0)     3017 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/daemon/syncd.py
+-rw-r--r--   0 root         (0) root         (0)     6941 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/daemon/unix_daemon.py
+-rw-r--r--   0 root         (0) root         (0)    19005 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/debug.py
+-rw-r--r--   0 root         (0) root         (0)     2090 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/doc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.916491 otpme-0.3.0a79/otpme/lib/encoding/
+-rw-r--r--   0 root         (0) root         (0)      429 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/encoding/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1779 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/encoding/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.916491 otpme-0.3.0a79/otpme/lib/encryption/
+-rw-r--r--   0 root         (0) root         (0)     3953 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/encryption/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3296 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/encryption/aes.py
+-rw-r--r--   0 root         (0) root         (0)     1479 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/encryption/aes_cfb.py
+-rw-r--r--   0 root         (0) root         (0)     7900 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/encryption/argon2.py
+-rw-r--r--   0 root         (0) root         (0)    10240 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/encryption/asymmetric_key_handler.py
+-rw-r--r--   0 root         (0) root         (0)     4251 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/encryption/ec.py
+-rw-r--r--   0 root         (0) root         (0)     2912 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/encryption/fernet.py
+-rw-r--r--   0 root         (0) root         (0)     3237 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/encryption/hkdf.py
+-rw-r--r--   0 root         (0) root         (0)     3727 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/encryption/pbkdf2.py
+-rw-r--r--   0 root         (0) root         (0)     7824 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/encryption/rsa.py
+-rw-r--r--   0 root         (0) root         (0)     4324 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.916491 otpme-0.3.0a79/otpme/lib/extensions/
+-rw-r--r--   0 root         (0) root         (0)      329 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/extensions/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.916491 otpme-0.3.0a79/otpme/lib/extensions/base/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/extensions/base/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12278 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/extensions/base/base.py
+-rw-r--r--   0 root         (0) root         (0)    40152 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/extensions/ldif_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.916491 otpme-0.3.0a79/otpme/lib/extensions/posix/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/extensions/posix/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14286 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/extensions/posix/posix.py
+-rw-r--r--   0 root         (0) root         (0)     3640 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/extensions/utils.py
+-rw-r--r--   0 root         (0) root         (0)    34585 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/filetools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.916491 otpme-0.3.0a79/otpme/lib/freeradius/
+-rw-r--r--   0 root         (0) root         (0)     9119 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/freeradius/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18685 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/freeradius/otpme.py
+-rw-r--r--   0 root         (0) root         (0)     1297 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/freeradius/radiusd.py
+-rw-r--r--   0 root         (0) root         (0)     1203 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/freeradius/radiusd_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.916491 otpme-0.3.0a79/otpme/lib/gpg/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/gpg/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    28498 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/gpg/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.920491 otpme-0.3.0a79/otpme/lib/help/
+-rwxr-xr-x   0 root         (0) root         (0)    26529 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/help/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22986 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/help/accessgroup.py
+-rw-r--r--   0 root         (0) root         (0)     5485 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/help/agent.py
+-rw-r--r--   0 root         (0) root         (0)     1857 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/help/auth.py
+-rw-r--r--   0 root         (0) root         (0)    15707 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/help/ca.py
+-rw-r--r--   0 root         (0) root         (0)    18323 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/help/client.py
+-rw-r--r--   0 root         (0) root         (0)     1568 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/help/cluster.py
+-rw-r--r--   0 root         (0) root         (0)     5785 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/help/controld.py
+-rw-r--r--   0 root         (0) root         (0)    11388 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/help/dictionary.py
+-rw-r--r--   0 root         (0) root         (0)      522 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/help/get_authorized_keys.py
+-rw-r--r--   0 root         (0) root         (0)    19872 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/help/group.py
+-rw-r--r--   0 root         (0) root         (0)    24436 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/help/host.py
+-rw-r--r--   0 root         (0) root         (0)    21309 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/help/node.py
+-rw-r--r--   0 root         (0) root         (0)      477 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/help/pinentry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.920491 otpme-0.3.0a79/otpme/lib/help/policy/
+-rw-r--r--   0 root         (0) root         (0)     8386 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/help/policy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3710 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/help/policy/authonaction.py
+-rw-r--r--   0 root         (0) root         (0)     1247 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/help/policy/autodisable.py
+-rw-r--r--   0 root         (0) root         (0)     1751 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/help/policy/defaultgroups.py
+-rw-r--r--   0 root         (0) root         (0)     1559 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/help/policy/defaultpolicies.py
+-rw-r--r--   0 root         (0) root         (0)     1421 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/help/policy/defaultroles.py
+-rw-r--r--   0 root         (0) root         (0)     1836 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/help/policy/defaultunits.py
+-rw-r--r--   0 root         (0) root         (0)     1492 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/help/policy/forcetoken.py
+-rw-r--r--   0 root         (0) root         (0)     2230 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/help/policy/idrange.py
+-rw-r--r--   0 root         (0) root         (0)     1831 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/help/policy/logintimes.py
+-rw-r--r--   0 root         (0) root         (0)     1098 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/help/policy/objecttemplates.py
+-rw-r--r--   0 root         (0) root         (0)     3463 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/help/policy/password.py
+-rw-r--r--   0 root         (0) root         (0)     2779 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/help/policy/tokenacls.py
+-rw-r--r--   0 root         (0) root         (0)    20037 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/help/realm.py
+-rw-r--r--   0 root         (0) root         (0)     1441 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/help/register.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.920491 otpme-0.3.0a79/otpme/lib/help/resolver/
+-rw-r--r--   0 root         (0) root         (0)    12522 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/help/resolver/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4465 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/help/resolver/ldap.py
+-rw-r--r--   0 root         (0) root         (0)    18198 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/help/role.py
+-rw-r--r--   0 root         (0) root         (0)    15111 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/help/script.py
+-rw-r--r--   0 root         (0) root         (0)     2844 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/help/session.py
+-rw-r--r--   0 root         (0) root         (0)    24542 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/help/site.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.920491 otpme-0.3.0a79/otpme/lib/help/token/
+-rw-r--r--   0 root         (0) root         (0)    20503 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/help/token/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1385 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/help/token/fido2.py
+-rw-r--r--   0 root         (0) root         (0)     5752 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/help/token/hotp.py
+-rw-r--r--   0 root         (0) root         (0)     6339 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/help/token/motp.py
+-rw-r--r--   0 root         (0) root         (0)     1991 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/help/token/otp_push.py
+-rw-r--r--   0 root         (0) root         (0)     4951 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/help/token/otpme.py
+-rw-r--r--   0 root         (0) root         (0)     4029 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/help/token/password.py
+-rw-r--r--   0 root         (0) root         (0)     7251 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/help/token/ssh.py
+-rw-r--r--   0 root         (0) root         (0)     5977 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/help/token/totp.py
+-rw-r--r--   0 root         (0) root         (0)     5803 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/help/token/yubikey_hmac.py
+-rw-r--r--   0 root         (0) root         (0)     1252 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/help/token/yubikey_hotp.py
+-rw-r--r--   0 root         (0) root         (0)    24935 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/help/tool.py
+-rw-r--r--   0 root         (0) root         (0)    15168 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/help/unit.py
+-rw-r--r--   0 root         (0) root         (0)    30280 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/help/user.py
+-rw-r--r--   0 root         (0) root         (0)    16341 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/host.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.920491 otpme-0.3.0a79/otpme/lib/humanize/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/humanize/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4191 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/humanize/units.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.924491 otpme-0.3.0a79/otpme/lib/index/
+-rw-r--r--   0 root         (0) root         (0)      382 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/index/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23948 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/index/mysql.py
+-rw-r--r--   0 root         (0) root         (0)    24542 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/index/postgres.py
+-rw-r--r--   0 root         (0) root         (0)     8336 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/index/sqlite3.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.924491 otpme-0.3.0a79/otpme/lib/job/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/job/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21189 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/job/callback.py
+-rw-r--r--   0 root         (0) root         (0)    12849 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/job/otpme_job.py
+-rw-r--r--   0 root         (0) root         (0)    37036 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/join.py
+-rw-r--r--   0 root         (0) root         (0)     4857 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/json.py
+-rw-r--r--   0 root         (0) root         (0)     1942 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/jwt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.924491 otpme-0.3.0a79/otpme/lib/ldap/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/ldap/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1354 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/ldap/client.py
+-rw-r--r--   0 root         (0) root         (0)    11062 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/ldap/schema.py
+-rw-r--r--   0 root         (0) root         (0)    50483 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/ldap/server.py
+-rw-r--r--   0 root         (0) root         (0)    19709 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/locking.py
+-rw-r--r--   0 root         (0) root         (0)     9430 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/log.py
+-rw-r--r--   0 root         (0) root         (0)     1529 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/messages.py
+-rw-r--r--   0 root         (0) root         (0)     5981 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/mschap.py
+-rw-r--r--   0 root         (0) root         (0)     2366 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/mschap_util.py
+-rw-r--r--   0 root         (0) root         (0)    35744 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/multiprocessing.py
+-rw-r--r--   0 root         (0) root         (0)    10250 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/net.py
+-rw-r--r--   0 root         (0) root         (0)    27144 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/nsscache.py
+-rw-r--r--   0 root         (0) root         (0)    63328 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/offline_token.py
+-rw-r--r--   0 root         (0) root         (0)    23778 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/oid.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.924491 otpme-0.3.0a79/otpme/lib/otp/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/otp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.924491 otpme-0.3.0a79/otpme/lib/otp/oath/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/otp/oath/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1727 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/otp/oath/hotp.py
+-rw-r--r--   0 root         (0) root         (0)     1581 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/otp/oath/totp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.924491 otpme-0.3.0a79/otpme/lib/otp/otpme/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/otp/otpme/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3087 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/otp/otpme/otpme.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.924491 otpme-0.3.0a79/otpme/lib/otp/yubico/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/otp/yubico/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3026 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/otp/yubico/yubiotp.py
+-rw-r--r--   0 root         (0) root         (0)    19883 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/otpme_acl.py
+-rw-r--r--   0 root         (0) root         (0)   115891 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/otpme_config.py
+-rw-r--r--   0 root         (0) root         (0)     3519 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/otpme_pass.py
+-rw-r--r--   0 root         (0) root         (0)    70359 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/pam.py
+-rw-r--r--   0 root         (0) root         (0)     1975 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/pickle.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.924491 otpme-0.3.0a79/otpme/lib/pinentry/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/pinentry/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27465 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/pinentry/pinentry.py
+-rwxr-xr-x   0 root         (0) root         (0)     7880 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/pinentry/wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.924491 otpme-0.3.0a79/otpme/lib/pki/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/pki/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9797 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/pki/cert.py
+-rw-r--r--   0 root         (0) root         (0)    23150 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/pki/utils.py
+-rw-r--r--   0 root         (0) root         (0)    16890 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/pki/utils_openssl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.924491 otpme-0.3.0a79/otpme/lib/policy/
+-rw-r--r--   0 root         (0) root         (0)     2099 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/policy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.924491 otpme-0.3.0a79/otpme/lib/policy/authonaction/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/policy/authonaction/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32675 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/policy/authonaction/authonaction.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.924491 otpme-0.3.0a79/otpme/lib/policy/autodisable/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/policy/autodisable/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15718 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/policy/autodisable/autodisable.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.924491 otpme-0.3.0a79/otpme/lib/policy/defaultgroups/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/policy/defaultgroups/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17570 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/policy/defaultgroups/defaultgroups.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.924491 otpme-0.3.0a79/otpme/lib/policy/defaultpolicies/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/policy/defaultpolicies/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14510 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/policy/defaultpolicies/defaultpolicies.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.924491 otpme-0.3.0a79/otpme/lib/policy/defaultroles/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/policy/defaultroles/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14217 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/policy/defaultroles/defaultroles.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.928491 otpme-0.3.0a79/otpme/lib/policy/defaultunits/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/policy/defaultunits/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15637 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/policy/defaultunits/defaultunits.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.928491 otpme-0.3.0a79/otpme/lib/policy/forcetoken/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/policy/forcetoken/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14202 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/policy/forcetoken/forcetoken.py
+-rw-r--r--   0 root         (0) root         (0)     1176 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/policy/get_class.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.928491 otpme-0.3.0a79/otpme/lib/policy/idrange/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/policy/idrange/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27362 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/policy/idrange/idrange.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.928491 otpme-0.3.0a79/otpme/lib/policy/logintimes/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/policy/logintimes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18083 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/policy/logintimes/logintimes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.928491 otpme-0.3.0a79/otpme/lib/policy/objecttemplates/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/policy/objecttemplates/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14954 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/policy/objecttemplates/objecttemplates.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.928491 otpme-0.3.0a79/otpme/lib/policy/password/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/policy/password/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29128 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/policy/password/password.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.928491 otpme-0.3.0a79/otpme/lib/policy/tokenacls/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/policy/tokenacls/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24897 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/policy/tokenacls/tokenacls.py
+-rw-r--r--   0 root         (0) root         (0)      491 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/policy/utils.py
+-rw-r--r--   0 root         (0) root         (0)     9315 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/preload.py
+-rw-r--r--   0 root         (0) root         (0)     2466 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/progress.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.928491 otpme-0.3.0a79/otpme/lib/protocols/
+-rw-r--r--   0 root         (0) root         (0)      304 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/protocols/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.928491 otpme-0.3.0a79/otpme/lib/protocols/client/
+-rw-r--r--   0 root         (0) root         (0)      655 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/protocols/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1887 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/protocols/client/agent1.py
+-rw-r--r--   0 root         (0) root         (0)      832 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/protocols/client/auth1.py
+-rw-r--r--   0 root         (0) root         (0)    14375 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/protocols/client/cluster1.py
+-rw-r--r--   0 root         (0) root         (0)     1046 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/protocols/client/get_class.py
+-rw-r--r--   0 root         (0) root         (0)     4645 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/protocols/client/host1.py
+-rw-r--r--   0 root         (0) root         (0)      832 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/protocols/client/join1.py
+-rwxr-xr-x   0 root         (0) root         (0)    11305 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/protocols/client/mgmt1.py
+-rw-r--r--   0 root         (0) root         (0)    67975 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/protocols/client/sync1.py
+-rw-r--r--   0 root         (0) root         (0)   160795 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/protocols/otpme_client.py
+-rw-r--r--   0 root         (0) root         (0)    81354 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/protocols/otpme_server.py
+-rw-r--r--   0 root         (0) root         (0)     1601 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/protocols/request.py
+-rw-r--r--   0 root         (0) root         (0)     1770 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/protocols/response.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.932491 otpme-0.3.0a79/otpme/lib/protocols/server/
+-rw-r--r--   0 root         (0) root         (0)      827 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/protocols/server/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    40314 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/protocols/server/agent1.py
+-rw-r--r--   0 root         (0) root         (0)    13084 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/protocols/server/auth1.py
+-rw-r--r--   0 root         (0) root         (0)    32506 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/protocols/server/cluster1.py
+-rw-r--r--   0 root         (0) root         (0)     1912 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/protocols/server/get_class.py
+-rw-r--r--   0 root         (0) root         (0)    26608 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/protocols/server/host1.py
+-rw-r--r--   0 root         (0) root         (0)    52562 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/protocols/server/join1.py
+-rw-r--r--   0 root         (0) root         (0)    70866 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/protocols/server/mgmt1.py
+-rw-r--r--   0 root         (0) root         (0)    45433 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/protocols/server/sync1.py
+-rw-r--r--   0 root         (0) root         (0)      527 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/protocols/status_codes.py
+-rw-r--r--   0 root         (0) root         (0)     6937 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/protocols/utils.py
+-rw-r--r--   0 root         (0) root         (0)     2157 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/push_script.py
+-rw-r--r--   0 root         (0) root         (0)     1139 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/qrcode.py
+-rw-r--r--   0 root         (0) root         (0)      478 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/re.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.932491 otpme-0.3.0a79/otpme/lib/register/
+-rw-r--r--   0 root         (0) root         (0)     9671 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/register/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.932491 otpme-0.3.0a79/otpme/lib/resolver/
+-rw-r--r--   0 root         (0) root         (0)      485 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/resolver/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1158 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/resolver/get_class.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.932491 otpme-0.3.0a79/otpme/lib/resolver/ldap/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/resolver/ldap/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39438 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/resolver/ldap/ldap.py
+-rw-r--r--   0 root         (0) root         (0)      451 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/resolver/utils.py
+-rw-r--r--   0 root         (0) root         (0)    10019 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/script.py
+-rw-r--r--   0 root         (0) root         (0)     3005 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/sign_key_cache.py
+-rw-r--r--   0 root         (0) root         (0)      537 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/slp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.932491 otpme-0.3.0a79/otpme/lib/smartcard/
+-rw-r--r--   0 root         (0) root         (0)      623 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/smartcard/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.932491 otpme-0.3.0a79/otpme/lib/smartcard/fido2/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/smartcard/fido2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10161 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/smartcard/fido2/fido2.py
+-rw-r--r--   0 root         (0) root         (0)      858 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/smartcard/get_class.py
+-rw-r--r--   0 root         (0) root         (0)     1666 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/smartcard/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.932491 otpme-0.3.0a79/otpme/lib/smartcard/yubikey/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/smartcard/yubikey/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11951 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/smartcard/yubikey/deploy.py
+-rw-r--r--   0 root         (0) root         (0)     1982 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/smartcard/yubikey/usb.py
+-rw-r--r--   0 root         (0) root         (0)     8075 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/smartcard/yubikey/yubikey.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.932491 otpme-0.3.0a79/otpme/lib/smartcard/yubikey_gpg/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/smartcard/yubikey_gpg/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6364 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/smartcard/yubikey_gpg/yubikey_gpg.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.932491 otpme-0.3.0a79/otpme/lib/smartcard/yubikey_hmac/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/smartcard/yubikey_hmac/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11955 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/smartcard/yubikey_hmac/yubikey_hmac.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.932491 otpme-0.3.0a79/otpme/lib/smartcard/yubikey_hotp/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/smartcard/yubikey_hotp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5032 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/smartcard/yubikey_hotp/yubikey_hotp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.932491 otpme-0.3.0a79/otpme/lib/socket/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/socket/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13587 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/socket/connect.py
+-rw-r--r--   0 root         (0) root         (0)     8450 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/socket/handler.py
+-rw-r--r--   0 root         (0) root         (0)    30962 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/socket/listen.py
+-rw-r--r--   0 root         (0) root         (0)     2830 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/socket/send_recv1.py
+-rw-r--r--   0 root         (0) root         (0)     4610 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/sotp.py
+-rwxr-xr-x   0 root         (0) root         (0)    37113 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/spsc.py
+-rw-r--r--   0 root         (0) root         (0)      544 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/srp.py
+-rw-r--r--   0 root         (0) root         (0)    23454 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/ssh.py
+-rw-r--r--   0 root         (0) root         (0)    63673 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/stuff.py
+-rw-r--r--   0 root         (0) root         (0)    12338 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/sync_cache.py
+-rw-r--r--   0 root         (0) root         (0)     4636 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/system_command.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.932491 otpme-0.3.0a79/otpme/lib/third_party/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/third_party/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.936491 otpme-0.3.0a79/otpme/lib/third_party/dogpile_caching/
+-rw-r--r--   0 root         (0) root         (0)     1981 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/third_party/dogpile_caching/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3021 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/third_party/dogpile_caching/advanced.py
+-rw-r--r--   0 root         (0) root         (0)     9859 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/third_party/dogpile_caching/caching_query.py
+-rw-r--r--   0 root         (0) root         (0)     2250 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/third_party/dogpile_caching/environment.py
+-rw-r--r--   0 root         (0) root         (0)     1764 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/third_party/dogpile_caching/fixture_data.py
+-rw-r--r--   0 root         (0) root         (0)     2248 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/third_party/dogpile_caching/helloworld.py
+-rw-r--r--   0 root         (0) root         (0)     3310 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/third_party/dogpile_caching/local_session_caching.py
+-rw-r--r--   0 root         (0) root         (0)     3033 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/third_party/dogpile_caching/model.py
+-rw-r--r--   0 root         (0) root         (0)     1040 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/third_party/dogpile_caching/relationship_caching.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.936491 otpme-0.3.0a79/otpme/lib/third_party/nss_cache/
+-rw-r--r--   0 root         (0) root         (0)     1140 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/third_party/nss_cache/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.936491 otpme-0.3.0a79/otpme/lib/third_party/nss_cache/caches/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/third_party/nss_cache/caches/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9083 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/third_party/nss_cache/caches/caches.py
+-rw-r--r--   0 root         (0) root         (0)    14341 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/third_party/nss_cache/caches/files.py
+-rw-r--r--   0 root         (0) root         (0)     1044 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/third_party/nss_cache/config.py
+-rw-r--r--   0 root         (0) root         (0)     1959 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/third_party/nss_cache/error.py
+-rw-r--r--   0 root         (0) root         (0)     7963 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/third_party/nss_cache/lock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.936491 otpme-0.3.0a79/otpme/lib/third_party/nss_cache/maps/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/third_party/nss_cache/maps/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2389 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/third_party/nss_cache/maps/group.py
+-rw-r--r--   0 root         (0) root         (0)    11745 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/third_party/nss_cache/maps/maps.py
+-rw-r--r--   0 root         (0) root         (0)     2554 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/third_party/nss_cache/maps/passwd.py
+-rw-r--r--   0 root         (0) root         (0)     2387 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/third_party/nss_cache/maps/shadow.py
+-rw-r--r--   0 root         (0) root         (0)     4140 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/third_party/nss_cache/nss.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.936491 otpme-0.3.0a79/otpme/lib/third_party/nss_cache/update/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/third_party/nss_cache/update/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5487 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/third_party/nss_cache/update/files_updater.py
+-rw-r--r--   0 root         (0) root         (0)     5826 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/third_party/nss_cache/update/map_updater.py
+-rw-r--r--   0 root         (0) root         (0)    10980 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/third_party/nss_cache/update/updater.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.936491 otpme-0.3.0a79/otpme/lib/third_party/nss_cache/util/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/third_party/nss_cache/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4117 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/third_party/nss_cache/util/file_formats.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.936491 otpme-0.3.0a79/otpme/lib/third_party/oath_toolkit/
+-rw-r--r--   0 root         (0) root         (0)        1 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/third_party/oath_toolkit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1592 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/third_party/oath_toolkit/_compat.py
+-rw-r--r--   0 root         (0) root         (0)     1772 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/third_party/oath_toolkit/uri.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.936491 otpme-0.3.0a79/otpme/lib/token/
+-rw-r--r--   0 root         (0) root         (0)      953 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/token/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.936491 otpme-0.3.0a79/otpme/lib/token/fido2/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/token/fido2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14939 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/token/fido2/fido2.py
+-rw-r--r--   0 root         (0) root         (0)     1056 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/token/get_class.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.936491 otpme-0.3.0a79/otpme/lib/token/hotp/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/token/hotp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39346 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/token/hotp/hotp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.936491 otpme-0.3.0a79/otpme/lib/token/link/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/token/link/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9656 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/token/link/link.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.936491 otpme-0.3.0a79/otpme/lib/token/motp/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/token/motp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27770 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/token/motp/motp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.936491 otpme-0.3.0a79/otpme/lib/token/oath/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/token/oath/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19667 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/token/oath/oath.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.936491 otpme-0.3.0a79/otpme/lib/token/otp_push/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/token/otp_push/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23393 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/token/otp_push/otp_push.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.936491 otpme-0.3.0a79/otpme/lib/token/otpme/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/token/otpme/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24704 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/token/otpme/otpme.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.940491 otpme-0.3.0a79/otpme/lib/token/password/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/token/password/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26906 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/token/password/password.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.940491 otpme-0.3.0a79/otpme/lib/token/script_otp/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/token/script_otp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9677 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/token/script_otp/script_otp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.940491 otpme-0.3.0a79/otpme/lib/token/script_static/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/token/script_static/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9677 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/token/script_static/script_static.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.940491 otpme-0.3.0a79/otpme/lib/token/ssh/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/token/ssh/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39547 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/token/ssh/ssh.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.940491 otpme-0.3.0a79/otpme/lib/token/totp/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/token/totp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35398 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/token/totp/totp.py
+-rw-r--r--   0 root         (0) root         (0)      480 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/token/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.940491 otpme-0.3.0a79/otpme/lib/token/yubikey_hmac/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/token/yubikey_hmac/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25111 2024-06-03 13:51:55.000000 otpme-0.3.0a79/otpme/lib/token/yubikey_hmac/yubikey_hmac.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:51:56.940491 otpme-0.3.0a79/otpme.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    44692 2024-06-03 13:51:56.000000 otpme-0.3.0a79/otpme.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    13467 2024-06-03 13:51:56.000000 otpme-0.3.0a79/otpme.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-06-03 13:51:56.000000 otpme-0.3.0a79/otpme.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1080 2024-06-03 13:51:56.000000 otpme-0.3.0a79/otpme.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-06-03 13:51:56.000000 otpme-0.3.0a79/otpme.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      988 2024-06-03 13:51:56.000000 otpme-0.3.0a79/otpme.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-06-03 13:51:56.000000 otpme-0.3.0a79/otpme.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2249 2024-06-03 13:51:55.000000 otpme-0.3.0a79/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1374 2024-06-03 13:51:55.000000 otpme-0.3.0a79/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-06-03 13:51:56.940491 otpme-0.3.0a79/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     9305 2024-06-03 13:51:55.000000 otpme-0.3.0a79/setup.py
```

### Comparing `otpme-0.3.0a78/LICENSE` & `otpme-0.3.0a79/LICENSE`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/MANIFEST.in` & `otpme-0.3.0a79/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/PKG-INFO` & `otpme-0.3.0a79/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otpme
-Version: 0.3.0a78
+Version: 0.3.0a79
 Summary: OTPme: A flexible One-Time-Password system
 Author-email: The2nd <the2nd@otpme.org>
 Maintainer-email: The2nd <the2nd@otpme.org>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
@@ -740,14 +740,18 @@
 Requires-Dist: pycryptodome>=3.4.3
 Requires-Dist: PyQRCode>=1.2.1
 Requires-Dist: pyre2>=0.3.6
 Requires-Dist: lz4>=4.3.2
 Requires-Dist: termcolor>=1.1.0
 Requires-Dist: radius-eap-mschapv2-client>=1.0.6
 Requires-Dist: pyrad>=2.4
+Requires-Dist: Flask>=3.0.3
+Requires-Dist: Flask-Login>=0.6.3
+Requires-Dist: Flask-WTF>=1.2.1
+Requires-Dist: gevent>=24.2.1
 
 # Installation instructions
 
 ## Install debian dependencies
 apt-get install python3.11-venv gobjc++ python3-pybind11 python3-dev build-essential cmake gcc dbus-x11 freeradius libacl1-dev libnss-cache liboath0 liboath-dev libpcsclite1 libpq-dev libre2-9 libre2-dev libsystemd-dev pkg-config postgresql postgresql-server-dev-all pwgen pyflakes3 redis redis-server redis-tools
 
 ### Disable installed services
```

### Comparing `otpme-0.3.0a78/README.md` & `otpme-0.3.0a79/README.md`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/bash_completion/otpme` & `otpme-0.3.0a79/bash_completion/otpme`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/deploy/dicts/abbreviations-it.gz` & `otpme-0.3.0a79/deploy/dicts/abbreviations-it.gz`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/deploy/dicts/at-surnames.gz` & `otpme-0.3.0a79/deploy/dicts/at-surnames.gz`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/deploy/dicts/common-passwords.gz` & `otpme-0.3.0a79/deploy/dicts/common-passwords.gz`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/deploy/dicts/convert_dict.sh` & `otpme-0.3.0a79/deploy/dicts/convert_dict.sh`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/deploy/dicts/de-female.gz` & `otpme-0.3.0a79/deploy/dicts/de-female.gz`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/deploy/dicts/de-male.gz` & `otpme-0.3.0a79/deploy/dicts/de-male.gz`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/deploy/dicts/de-surnames.gz` & `otpme-0.3.0a79/deploy/dicts/de-surnames.gz`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/deploy/dicts/de-top10000.gz` & `otpme-0.3.0a79/deploy/dicts/de-top10000.gz`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/deploy/dicts/en-top10000.gz` & `otpme-0.3.0a79/deploy/dicts/en-top10000.gz`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/deploy/dicts/english-guessing.gz` & `otpme-0.3.0a79/deploy/dicts/english-guessing.gz`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/deploy/dicts/english.gz` & `otpme-0.3.0a79/deploy/dicts/english.gz`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/deploy/dicts/german-guessing.gz` & `otpme-0.3.0a79/deploy/dicts/german-guessing.gz`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/deploy/dicts/german.gz` & `otpme-0.3.0a79/deploy/dicts/german.gz`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/deploy/dicts/us-female.gz` & `otpme-0.3.0a79/deploy/dicts/us-female.gz`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/deploy/dicts/us-male.gz` & `otpme-0.3.0a79/deploy/dicts/us-male.gz`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/deploy/dicts/us-surnames.gz` & `otpme-0.3.0a79/deploy/dicts/us-surnames.gz`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/deploy/otpme.conf.dist` & `otpme-0.3.0a79/deploy/otpme.conf.dist`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/deploy/pam/README` & `otpme-0.3.0a79/deploy/pam/README`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/deploy/pam/pam-python/README` & `otpme-0.3.0a79/deploy/pam/pam-python/README`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/deploy/pam/pam_otpme.py` & `otpme-0.3.0a79/deploy/pam/pam_otpme.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/deploy/radius/dictionary` & `otpme-0.3.0a79/deploy/radius/dictionary`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/deploy/radius/dictionary.freeradius` & `otpme-0.3.0a79/deploy/radius/dictionary.freeradius`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/deploy/schema/core.schema` & `otpme-0.3.0a79/deploy/schema/core.schema`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/deploy/schema/cosine.schema` & `otpme-0.3.0a79/deploy/schema/cosine.schema`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/deploy/schema/inetorgperson.schema` & `otpme-0.3.0a79/deploy/schema/inetorgperson.schema`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/deploy/schema/nis.schema` & `otpme-0.3.0a79/deploy/schema/nis.schema`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/deploy/scripts/agent_script.sh` & `otpme-0.3.0a79/deploy/scripts/agent_script.sh`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/deploy/scripts/key_script.sh` & `otpme-0.3.0a79/deploy/scripts/key_script.sh`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/__init__.py` & `otpme-0.3.0a79/otpme/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 #__project_url__ = "http://www.otpme.org"
 #__copyright__ = "Copyright 2014-2024 the2nd <the2nd@otpme.org>"
 #__project_description__ = "OTPme: A flexible One-Time-Password system."
 #__author__ = "the2nd"
 #__email__ = "the2nd@otpme.org"
 #__credits__ = []
 #__license__ = "GPLv2"
-__version__ = "0.3.0a78"
+__version__ = "0.3.0a79"
 #__status__ = "Development Status :: 3 - Alpha"
 ## In future versions :D
 ##__status__ = "Development Status :: 4 - Beta"
 ##__status__ = "Development Status :: 5 - Production/Stable"
 #__pkg_name__ = __project_name__
 #__maintainer__ = __author__
 #__author_email__  = __email__
```

### Comparing `otpme-0.3.0a78/otpme/command.py` & `otpme-0.3.0a79/otpme/command.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/__init__.py` & `otpme-0.3.0a79/otpme/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/arp.py` & `otpme-0.3.0a79/otpme/lib/arp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/auth_script.py` & `otpme-0.3.0a79/otpme/lib/auth_script.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/backend.py` & `otpme-0.3.0a79/otpme/lib/backend.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) 2014 the2nd <the2nd@otpme.org>
 import os
 import time
 import json
-import copy
 import pprint
 from functools import wraps
 
 try:
     if os.environ['OTPME_DEBUG_MODULE_LOADING'] == "True":
         print(_("Loading module: %s") % __name__)
 except:
@@ -240,100 +239,42 @@
         object_config.decrypt(config.master_key)
 
     return object_config
 
 @handle_daemon_shutdown()
 #@oid_lock(args_oid_pos=[0], write=True)
 def write_config(object_id, instance=None, object_config=None, cluster=False,
-    index_auto_update=True, full_index_update=False, full_data_update=None,
-    index_journal=[], index_journal_start_id=None,
+    full_index_update=False, full_data_update=None, index_journal=[],
     no_transaction=False, encrypt=True):
     """ Write object config to backend and update config cache. """
     # Get logger.
     logger = config.logger
     if not config.master_key:
         msg = "Missing AES master key. Unable to encrypt config data."
         logger.critical(msg)
         raise OTPmeException(msg)
-    if index_auto_update and index_journal:
-        msg = "You can use only one of <index_auto_update> or <index_journal>."
-        raise OTPmeException(msg)
-    if index_journal_start_id and index_journal:
-        msg = "You can use only one of <index_journal> or <index_journal_start_id>."
-        raise OTPmeException(msg)
-    if full_index_update and index_auto_update:
-        msg = "You can use only one of <full_index_update> or <index_auto_update>."
-        raise OTPmeException(msg)
     if full_index_update and index_journal:
         msg = "You can use only one of <full_index_update> or <index_journal>."
         raise OTPmeException(msg)
-    if full_index_update and index_journal_start_id:
-        msg = "You can use only one of <full_index_update> or <index_journal_start_id>."
-        raise OTPmeException(msg)
 
     # Replay any leftover transaction.
     replay_transactions()
 
     # Get config from instance.
     if instance is not None:
         object_config = instance.object_config
     else:
         object_config = ObjectConfig(object_id, object_config, encrypted=False)
 
-    if index_auto_update:
-        # By default do a full index update.
-        full_index_update = True
-        # The index journal ID of the object.
-        index_journal_start_id = None
-        # Read object config to get last journal ID.
-        try:
-            x_object_config = read(object_id, parameters=['INDEX_JOURNAL_ID'])
-        except Exception as e:
-            msg = "Failed to read index journal: %s: %s" % (object_id, e)
-            logger.critical(msg)
-        # Get journal ID.
-        try:
-            index_journal_start_id = x_object_config['INDEX_JOURNAL_ID']
-            full_index_update = False
-        except:
-            pass
-
     # Encrypt object config and update checksums.
     if encrypt:
         object_config = object_config.encrypt(config.master_key)
     else:
         object_config = object_config.copy()
 
-    if index_journal_start_id:
-        # Get object index journal archive.
-        try:
-            index_journal_archive = object_config['INDEX_JOURNAL_ARCHIVE']
-        except:
-            msg = "Invalid object config: %s: Missing index journal archive"
-            raise OTPmeException(msg)
-        # Get only index journal entries not already applied to this object.
-        index_journal = []
-        found_start_id = False
-        x_sort = lambda x: float(x)
-        for x in sorted(index_journal_archive, key=x_sort):
-            if float(x) < float(index_journal_start_id):
-                continue
-            if float(x) == float(index_journal_start_id):
-                found_start_id = True
-                continue
-            index_journal += copy.deepcopy(index_journal_archive[x]['data'])
-        # Fallback to full index update.
-        if not found_start_id:
-            # Log warning a index journal exists but cannot be used.
-            if index_journal_archive:
-                msg = ("Index journal out of sync, will do full index "
-                        "update: %s" % object_id)
-                logger.info(msg)
-            full_index_update = True
-
     # Write config file.
     write_status = write(object_id=object_id,
                     object_config=object_config,
                     index_journal=index_journal,
                     full_index_update=full_index_update,
                     full_data_update=full_data_update,
                     no_transaction=no_transaction,
@@ -448,15 +389,14 @@
         msg = "Object with UUID exists: %s" % x_object
         return callback.error(msg)
     try:
         write_config(object_id=object_id,
                     object_config=object_config,
                     full_index_update=True,
                     full_data_update=True,
-                    index_auto_update=False,
                     encrypt=False,
                     cluster=True)
     except Exception as e:
         msg = "Failed to restore object: %s: %s" % (object_id, e)
         return callback.error(msg)
     if object_id.object_type == "user":
         x_uuid = object_config['UUID']
@@ -800,15 +740,14 @@
                         "role",
                         "policy",
                         "resolver",
                         "script",
                         "dictionary",
                         "ca",
                         "used_otp",
-                        "used_slp",
                         "used_sotp",
                         "failed_pass",
                         "token_counter",
                         "revoked_signature",
                         ]
 
     if skip_users is None:
```

### Comparing `otpme-0.3.0a78/otpme/lib/backends/file/file.py` & `otpme-0.3.0a79/otpme/lib/backends/file/file.py`

 * *Files 0% similar despite different names*

```diff
@@ -595,15 +595,15 @@
         x_transaction.dismiss_object(object_id=x_old_oid)
         x_transaction.add_object(object_id=x_new_oid,
                                 object_config=x_object_config,
                                 full_index_update=True,
                                 cluster=cluster)
 
     if cluster:
-        write_transaction.cluster_write(uuid, object_id, object_config)
+        write_transaction.cluster_write(uuid, object_id, index_journal, object_config)
 
     # Commit and remove write transaction.
     if transaction_replay:
         write_transaction.replay()
     else:
         write_transaction.commit()
     # With an running object transaction the file transaction
@@ -1980,60 +1980,61 @@
     if index_object:
         q = session.query(IndexObjectACL)
         x = q.filter(IndexObjectACL.ioid == index_object.id)
         object_acls = x.all()
 
     # Handle index journal.
     attributes = []
-    for x_entry in index_journal:
-        x_entry_type = x_entry[0]
-        x_attribute = x_entry[1]
-        x_value = x_entry[2]
-
-        # Add attributes.
-        if x_entry_type == "add":
-            # Add attribute.
-            #if x_attribute == "ldif:memberUid":
-                #print("AAAA", x_attribute, x_value)
-            a = IndexObjectAttribute(realm=object_realm,
-                                    site=object_site,
-                                    object_type=object_type,
-                                    name=x_attribute, value=x_value)
-            # If the object already exists in the DB we just have to add the
-            # new/changed attribute.
-            if index_object:
-                # Reference attribute to existing index object.
-                a.ioid = index_object.id
-                session.add(a)
-                #local_object = session.merge(a)
-                #session.add(local_object)
-            else:
-                # Add attribute to list of attributes for the new index object.
-                attributes.append(a)
+    if index_journal:
+        for x_entry in index_journal:
+            x_entry_type = x_entry[0]
+            x_attribute = x_entry[1]
+            x_value = x_entry[2]
+
+            # Add attributes.
+            if x_entry_type == "add":
+                # Add attribute.
+                #if x_attribute == "ldif:memberUid":
+                    #print("AAAA", x_attribute, x_value)
+                a = IndexObjectAttribute(realm=object_realm,
+                                        site=object_site,
+                                        object_type=object_type,
+                                        name=x_attribute, value=x_value)
+                # If the object already exists in the DB we just have to add the
+                # new/changed attribute.
+                if index_object:
+                    # Reference attribute to existing index object.
+                    a.ioid = index_object.id
+                    session.add(a)
+                    #local_object = session.merge(a)
+                    #session.add(local_object)
+                else:
+                    # Add attribute to list of attributes for the new index object.
+                    attributes.append(a)
 
-        if x_entry_type == "del":
-            if not index_object:
-                continue
-            #if x_attribute == "ldif:memberUid":
-            #    print("dddd", x_attribute, x_value)
-            q = session.query(IndexObjectAttribute)
-            q = q.filter(IndexObjectAttribute.ioid == index_object.id)
-            q = q.filter(IndexObjectAttribute.name == x_attribute)
-            q = q.filter(IndexObjectAttribute.value == x_value)
-            result = q.all()
-            for a in result:
-                session.delete(a)
-                #local_object = session.merge(a)
-                #session.delete(local_object)
-                ## Make sure we commit attribute deletion.
-                #if autocommit:
-                #    try:
-                #        session.commit()
-                #    except ObjectDeletedError:
-                #        session.rollback()
+            if x_entry_type == "del":
+                if not index_object:
+                    continue
+                #if x_attribute == "ldif:memberUid":
+                #    print("dddd", x_attribute, x_value)
+                q = session.query(IndexObjectAttribute)
+                q = q.filter(IndexObjectAttribute.ioid == index_object.id)
+                q = q.filter(IndexObjectAttribute.name == x_attribute)
+                q = q.filter(IndexObjectAttribute.value == x_value)
+                result = q.all()
+                for a in result:
+                    session.delete(a)
+                    #local_object = session.merge(a)
+                    #session.delete(local_object)
+                    ## Make sure we commit attribute deletion.
+                    #if autocommit:
+                    #    try:
+                    #        session.commit()
+                    #    except ObjectDeletedError:
+                    #        session.rollback()
 
     # Make sure we remove orphan ACLs of an existing index object.
     clear_acl_cache = False
     if object_acls:
         for i in object_acls:
             del_acl = True
             for x in oacls:
```

### Comparing `otpme-0.3.0a78/otpme/lib/backends/file/index.py` & `otpme-0.3.0a79/otpme/lib/backends/file/index.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/backends/file/models.py` & `otpme-0.3.0a79/otpme/lib/backends/file/models.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/backends/file/transaction.py` & `otpme-0.3.0a79/otpme/lib/backends/file/transaction.py`

 * *Files 1% similar despite different names*

```diff
@@ -798,22 +798,23 @@
         try:
             self._write_journal()
         except EmptyTransaction:
             return
         # Call parent class write method to finalize write.
         return super(FileTransaction, self)._write()
 
-    def cluster_write(self, object_uuid, object_id, object_config):
+    def cluster_write(self, object_uuid, object_id, index_journal, object_config):
         """ Cluster write action. """
         action = "cluster_write"
         journal_file = self.get_journal_file(action)
         journal_entry = {
                         'action'        : action,
                         'object_uuid'   : object_uuid,
                         'object_id'     : object_id.full_oid,
+                        'index_journal' : index_journal,
                         'object_config' : object_config,
                         'journal_file'  : journal_file,
                         }
         self.journal.append(self.journal_counter)
         self.journal_entries[str(self.journal_counter)] = journal_entry
         self.journal_counter += 1
 
@@ -1051,30 +1052,34 @@
                 if not self.no_disk_writes:
                     object_id = journal_entry['object_id']
                     object_id = oid.get(object_id)
                     nsscache_action = journal_entry['nsscache_action']
                     self._update_nsscache(object_id, nsscache_action)
             elif action == "cluster_write":
                 if not self.no_disk_writes:
+                    object_config = journal_entry['object_config']
+                    index_journal = journal_entry['index_journal']
                     object_uuid = journal_entry['object_uuid']
                     object_id = journal_entry['object_id']
                     object_id = oid.get(object_id)
-                    object_config = journal_entry['object_config']
-                    # Decrypt object config.
+                    ## Get current object config.
+                    #object_config = read(object_id)
                     object_config = ObjectConfig(object_id, object_config)
+                    # Decrypt object config.
                     object_config = object_config.decrypt(config.master_key)
-                    checksum = object_config['CHECKSUM']
+                    object_checksum = object_config['CHECKSUM']
                     wait_for_write = True
                     if self._replay:
                         wait_for_write = False
                     cluster_event = cluster_sync_object(object_uuid=object_uuid,
                                                     object_id=object_id,
                                                     object_config=object_config,
                                                     action="write",
-                                                    checksum=checksum,
+                                                    checksum=object_checksum,
+                                                    index_journal=index_journal,
                                                     wait_for_write=wait_for_write)
                     if cluster_event:
                         cluster_events.append(cluster_event)
             elif action == "cluster_delete":
                 if not self.no_disk_writes:
                     object_uuid = journal_entry['object_uuid']
                     object_id = journal_entry['object_id']
```

### Comparing `otpme-0.3.0a78/otpme/lib/cache/__init__.py` & `otpme-0.3.0a79/otpme/lib/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/cache/dogpile.py` & `otpme-0.3.0a79/otpme/lib/cache/dogpile.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/cache/funccache.py` & `otpme-0.3.0a79/otpme/lib/cache/funccache.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/cache/lru.py` & `otpme-0.3.0a79/otpme/lib/cache/lru.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/cache/memcache.py` & `otpme-0.3.0a79/otpme/lib/cache/memcache.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/cache/memcached.py` & `otpme-0.3.0a79/otpme/lib/cache/memcached.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/cache/memcachedb.py` & `otpme-0.3.0a79/otpme/lib/cache/memcachedb.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/cache/redis.py` & `otpme-0.3.0a79/otpme/lib/cache/redis.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/classes/__init__.py` & `otpme-0.3.0a79/otpme/lib/classes/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/classes/accessgroup.py` & `otpme-0.3.0a79/otpme/lib/classes/accessgroup.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/classes/agent_conn.py` & `otpme-0.3.0a79/otpme/lib/classes/agent_conn.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,22 +194,23 @@
         """ Del session from otpme-agent. """
         status, status_code, reply = self.send("del_session")
         if status_code != status_codes.OK:
             msg = (_("Error removing login session from agent: %s") % reply)
             raise OTPmeException(msg)
         return reply
 
-    def add_rsp(self, realm, site, rsp, login_time, timeout, unused_timeout,
+    def add_rsp(self, realm, site, rsp, slp, login_time, timeout, unused_timeout,
         rsp_signature=None, session_key=None, offline=False):
         """ Add RSP to otpme-agent. """
         command_args = {
                         'realm'         : realm,
                         'site'          : site,
                         'rsp'           : rsp,
                         'rsp_signature' : rsp_signature,
+                        'slp'           : slp,
                         'session_key'   : session_key,
                         'offline'       : offline,
                         'login_time'    : login_time,
                         'timeout'       : timeout,
                         'unused_timeout': unused_timeout,
                     }
         status, status_code, reply = self.send("add_rsp", **command_args)
```

### Comparing `otpme-0.3.0a78/otpme/lib/classes/auth_handler.py` & `otpme-0.3.0a79/otpme/lib/classes/auth_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 try:
     if os.environ['OTPME_DEBUG_MODULE_LOADING'] == "True":
         print(_("Loading module: %s" % __name__))
 except:
     pass
 
 from otpme.lib import jwt
+from otpme.lib import slp
 from otpme.lib import sotp
 from otpme.lib import stuff
 from otpme.lib import config
 from otpme.lib import backend
 from otpme.lib import otpme_pass
 from otpme.lib.encryption.ec import ECKey
 from otpme.lib.encoding.base import decode
@@ -57,18 +58,14 @@
         if hash_params is None:
             if hash_type is None:
                 hash_type = self.auth_group.get_config_parameter('session_hash_type')
         # Generate NT hash.
         if not self.nt_hash:
             self.nt_hash = stuff.gen_nt_hash(self.password)
 
-        # If we already have a password hash there is nothing to do.
-        if self.password_hash:
-            return
-
         if self.auth_type == "mschap":
             self.password_hash = self.nt_hash
             return
 
         # Create password_hash for clear-text requests. Its at
         # least needed to count failed logins.
         hash_data = otpme_pass.gen_pass_hash(username=self.user.name,
@@ -97,15 +94,16 @@
         if request_type == "auth":
             self.logger.debug("Authentication parameters of request "
                             "matching session '%s'." % session.name)
             # If we found a session that matches this authentication request set
             # auth_session.
             self.auth_session = session
             # If we have a session no need to create a new one.
-            self.create_sessions = False
+            if self.auth_session.access_group == self.access_group:
+                self.create_sessions = False
             # Set password hash from matched session hash.
             self.password_hash = session.pass_hash
             if self.auth_type == "mschap":
                 # Set NT_KEY
                 self.nt_key = verify_reply['nt_key']
             return session_status
 
@@ -168,29 +166,29 @@
                 # Set NT_KEY
                 self.nt_key = verify_reply['nt_key']
                 # If we found an already used SOTP and this sessions is the
                 # REALM session, authentication is not done but also not failed
                 # because one of the child sessions may have been created by
                 # this SOTP.
                 if session.access_group == config.realm_access_group:
-                    if self.user.is_used(otype="sotp", hash=self.one_iter_hash):
+                    if self.user.is_used_sotp(hash=self.one_iter_hash):
                         return None
 
             if self.auth_type == "clear-text":
                 # For REALM session childs (SOTP reauth) we use a one iteration
                 # hash like we do for the REALM session itself.
                 self.password_hash = self.one_iter_hash
 
             msg = ("Found valid REALM session '%s' for this request (SOTP)."
                     % session.name)
             self.logger.debug(msg)
 
             self.found_sotp = True
             # Add SOTP to list of users used SOTPs.
-            self.user.add_used(otype="sotp", hash=self.one_iter_hash)
+            self.user.add_used_sotp(hash=self.one_iter_hash)
             # Set auth session if we found an SOTP.
             self.auth_session = session
             # Update session (e.g. last used timestamp).
             self.update_session(session)
             # No need to create a session on reauth via SOTP with REALM
             # accessgroup.
             if self.access_group == config.realm_access_group:
@@ -359,14 +357,18 @@
             # fail.
             self.auth_failed = True
             self.auth_message = "AUTH_TOKEN_UNKNOWN"
             return
 
         # Set auth token from session.
         self.auth_token = token
+        if self.found_sotp:
+            config.auth_type = "sotp"
+        else:
+            config.auth_type = "token"
 
         # On session logout we are done here.
         if self.session_logout:
             return
 
         # Verify auth token.
         if not self.auth_failed:
@@ -418,16 +420,14 @@
                 self.auth_message = "REALM_LOGOUT_OK"
             else:
                 self.logger.info("Logout request. Removing session '%s'"
                             % session.name)
                 self.auth_message = "SESSION_LOGOUT_OK"
             # Delete session if this is a logout request.
             session.delete(force=True, recursive=True, verify_acls=False)
-            # Add SLP hash to used SLPs list of the user.
-            self.user.add_used(otype="slp", hash=self.one_iter_hash)
             # On session logout authentication fails but the action was
             # successful. Thus loglevel INFO is sufficient.
             self.error_log_method = self.logger.info
             # Session update done.
             return
 
         if self.session_reneg:
@@ -457,117 +457,170 @@
             else:
                 self.auth_message = "AUTH_OK_SESSION"
                 # Update session login count which also updates the last used time.
                 self.auth_session.count_login()
 
     def verify_user_sessions(self):
         """ Verify user sessions. """
-        return_attributes = ['uuid', 'session_id']
+        return_attributes = ['uuid', 'session_id', 'accessgroup']
         # Get REALM sessions for this user.
         result = backend.search(object_type="accessgroup",
                                 attribute="name",
                                 value=config.realm_access_group,
                                 return_type="uuid")
         realm_access_group_uuid = result[0]
-        user_sessions = backend.get_sessions(user=self.user.uuid,
+        user_realm_sessions = backend.get_sessions(user=self.user.uuid,
                                     access_group=realm_access_group_uuid,
                                     return_attributes=return_attributes)
                                     # We have to check all sessions here because
                                     # e.g. a smartcard session will do SOTP auth
                                     # when connecting to mgmtd.
                                     #session_type=self.auth_type)
-        # Get realm session IDs.
+
+        # Get realm sessions that have the requested accessgroup as child.
+        verify_sessions = []
         realm_session_ids = []
-        for session_uuid in user_sessions:
-            session_id = user_sessions[session_uuid]['session_id'][0]
+        for session_uuid in user_realm_sessions:
+            # Get session instance.
+            session_id = user_realm_sessions[session_uuid]['session_id'][0]
+            session = backend.get_object(object_type="session",
+                                        uuid=session_uuid)
+            if not session:
+                continue
+            # Outdate expired session.
+            try:
+                if not session.exists(outdate=True):
+                    continue
+            except LockWaitAbort:
+                continue
             realm_session_ids.append(session_id)
+            session_ag_uuid = user_realm_sessions[session_uuid]['accessgroup'][0]
+            session_ag = backend.get_object(uuid=session_ag_uuid)
+            session_ag_childs = session_ag.childs(recursive=True)
+            if self.auth_group.uuid != session_ag.uuid:
+                if self.auth_group.name not in session_ag_childs:
+                    continue
+            verify_sessions.append(session)
+
+        # Get sessions for the session master.
+        session_master = self.auth_group.parents(recursive=True,
+                                                session_master=True,
+                                                return_type="instance")
+        session_master_session_ids = []
+        if session_master:
+            session_master_sessions = backend.get_sessions(user=self.user.uuid,
+                                                access_group=session_master.uuid,
+                                                return_attributes=return_attributes,
+                                                session_type=self.auth_type)
+            for session_uuid in session_master_sessions:
+                # Get session instance.
+                session_id = session_master_sessions[session_uuid]['session_id'][0]
+                session = backend.get_object(object_type="session",
+                                            uuid=session_uuid)
+                if not session:
+                    continue
+                # Outdate expired session.
+                try:
+                    if not session.exists(outdate=True):
+                        continue
+                except LockWaitAbort:
+                    continue
+                if session in verify_sessions:
+                    continue
+                verify_sessions.append(session)
+                session_master_session_ids.append(session_id)
 
         # Get sessions for this user/accessgroup.
         if self.auth_group.uuid != realm_access_group_uuid:
             group_session_ids = backend.get_sessions(user=self.user.uuid,
                                             access_group=self.auth_group.uuid,
                                             return_attributes=return_attributes,
                                             session_type=self.auth_type)
-            for x in group_session_ids:
-                if x in user_sessions:
+            for session_uuid in group_session_ids:
+                # Get session instance.
+                session_id = group_session_ids[session_uuid]['session_id'][0]
+                session = backend.get_object(object_type="session",
+                                            uuid=session_uuid)
+                if not session:
+                    continue
+                # Outdate expired session.
+                try:
+                    if not session.exists(outdate=True):
+                        continue
+                except LockWaitAbort:
                     continue
-                user_sessions[x] = group_session_ids[x]
+                if session in verify_sessions:
+                    continue
+                verify_sessions.append(session)
 
-        if not user_sessions:
+        if not verify_sessions:
             self.logger.debug("No session found for this request.")
 
         # Check users sessions.
         processed_sessions = []
-        for session_uuid in user_sessions:
-            if session_uuid in processed_sessions:
-                continue
-            processed_sessions.append(session_uuid)
-            # Get session instance.
-            session_id = user_sessions[session_uuid]['session_id'][0]
-            session = backend.get_object(object_type="session",
-                                        uuid=session_uuid)
-            if not session:
-                continue
-            # Outdate expired session.
-            try:
-                if not session.exists(outdate=True):
-                    continue
-            except LockWaitAbort:
+        for session in verify_sessions:
+            if session.uuid in processed_sessions:
                 continue
+            processed_sessions.append(session.uuid)
 
-            ## We can only verify sessions that match the requests auth type.
-            #if self.auth_type != session.session_type:
-            #    self.logger.debug("Ignoring %s session for %s request."
-            #                % (session.session_type, self.auth_type))
-            #    continue
+            check_for_used_sotp = False
+            if session.session_id in realm_session_ids:
+                check_for_used_sotp = True
+            if session.session_id in session_master_session_ids:
+                check_for_used_sotp = True
+
+            if check_for_used_sotp:
+                # For clear-text sessions we can check for an already used
+                # SOTP before verifying the session.
+                if self.auth_type == "clear-text":
+                    # We use just one iteration for SOTPs because of performance
+                    # reasons (e.g. login and session renegotiation). This should
+                    # not be a problem because everyone with access to the OTPme
+                    # server can still do bad stuff and the RSP itself changes on
+                    # each login or renegotiation.
+                    password_hash = self.one_iter_hash
+                    # If we found an already used SOTP there is no need to
+                    # check tis REALM session again. But we have to check if
+                    # the child session this OTP created still exists and
+                    # must be verified. We can NOT use self.check_used()
+                    # here because this will make this request fail.
+                    if self.user.is_used_sotp(hash=password_hash):
+                        continue
 
             self.logger.debug("Verifying session '%s'." % session.name)
 
             # FIXME: implement session reneg for non-REALM sessions???
-            if session_id in realm_session_ids:
+            if session.session_id in realm_session_ids:
                 # Add realm session childs to list.
                 realm_session_ids += session.child_sessions
-                # We use just one iteration for RSPs because of performance
-                # reasons (e.g. login and session renegotiation). This should
-                # not be a problem because everyone with access to the OTPme
-                # server can still do bad stuff and the RSP itself changes on
-                # each login or renegotiation.
-                password_hash = self.one_iter_hash
-
                 if session.access_group == config.realm_access_group:
-                    # For clear-text sessions we can check for an already used
-                    # SOTP before verifying the session.
-                    if self.auth_type == "clear-text":
-                        # If we found an already used SOTP there is no need to
-                        # check tis REALM session again. But we have to check if
-                        # the child session this OTP created still exists and
-                        # must be verified. We can NOT use self.check_used()
-                        # here because this will make this request fail.
-                        if self.user.is_used(otype="sotp", hash=password_hash):
-                            continue
                     check_auth = False
                     check_sotp = True
                     # No need to check for session renegotiation with MSCHAP
                     # requests.
                     if self.auth_type == "mschap":
                         do_reneg = False
                     else:
                         do_reneg = True
                 else:
                     check_auth = True
                     check_sotp = False
                     do_reneg = False
-
             else:
                 # Make sure we have a password hash.
                 self.gen_pass_hash(hash_params=session.pass_hash_params)
                 password_hash = self.password_hash
+                do_reneg = False
                 check_auth = True
                 check_sotp = False
-                do_reneg = False
+                if self.access_group == config.sso_access_group:
+                    check_sotp = True
+                if session_master:
+                    if session_master.name == config.sso_access_group:
+                        check_sotp = True
 
             if self.session_reneg is not None:
                 do_reneg = self.session_reneg
 
             kwargs = {
                 'do_reneg'          : do_reneg,
                 'reneg_salt'        : self.reneg_salt,
@@ -576,14 +629,17 @@
                 'check_sotp'        : check_sotp,
                 'password'          : self.password,
                 'password_hash'     : password_hash,
                 'challenge'         : self.challenge,
                 'response'          : self.response,
                 }
 
+            if self.access_group != config.realm_access_group:
+                kwargs['auth_ag'] = self.access_group
+
             # Try to verify session.
             if self.verify_session(session, **kwargs) is not None:
                 self.verify_session_token(session)
                 self.update_session(session)
                 self.request_cacheable = True
                 break
 
@@ -618,50 +674,46 @@
             session_status = verify_reply['status']
             if session_status is None:
                 continue
 
             request_type = verify_reply['type']
             # Found SLP.
             if request_type == "logout":
-                # Gen SLP hash.
-                slp_hash = self.get_one_iter_hash(slp, quiet=True)
-                # Add SLP hash to used SLPs list of the user.
-                self.user.add_used(otype="slp", hash=slp_hash)
                 # Delete session if it matches the given SLP.
                 session.delete(force=True, recursive=True, verify_acls=False)
                 self.logger.debug("Logged out old user session: %s" % session.name)
                 return session_status
 
-    def check_used(self, pass_type):
-        """ Verify request password against already used SLPs/SOTPs. """
+    def check_used(self):
+        """ Verify request password against already used SOTPs. """
         # Without password we cannot check.
         if not self.password:
             return
 
-        self.logger.debug("Checking for used %s..." % pass_type.upper())
+        self.logger.debug("Checking for used SOTP...")
         if not self.one_iter_hash:
             raise Exception("You have to set self.one_iter_hash first.")
 
         # Check if we checked this hash before (in this auth request). This is
         # to lower our load.
-        if self.one_iter_hash in self.checked_hashes[pass_type]:
+        if self.one_iter_hash in self.checked_hashes:
             return
 
         # Add hash to processed hashes.
-        self.checked_hashes[pass_type].append(self.one_iter_hash)
+        self.checked_hashes.append(self.one_iter_hash)
 
-        # This check is needed because we dont want to count recurring SLP/SOTP
+        # This check is needed because we dont want to count recurring SOTP
         # requests as failed logins.
-        if self.user.is_used(otype=pass_type, hash=self.one_iter_hash):
-            self.logger.warning("Request contains an already used %s. "
-                            "Authentication will fail." % pass_type.upper())
-            # If the password from this request is an already used SLP/SOTP
+        if self.user.is_used_sotp(hash=self.one_iter_hash):
+            self.logger.warning("Request contains an already used SOTP. "
+                                "Authentication will fail.")
+            # If the password from this request is an already used SOTP
             # authentication must fail.
             self.auth_failed = True
-            self.auth_message = "AUTH_ALREADY_USED_%s" % pass_type.upper()
+            self.auth_message = "AUTH_ALREADY_USED_SOTP"
 
     def get_client(self):
         """ Try to get client of this request. """
         # If we got a host set client infos from it.
         if self.host and not self.client:
             self.client = self.host
             if self.host_ip:
@@ -749,15 +801,15 @@
             # If client does not exist authentication is failed.
             self.auth_failed = True
             self.logger.error("Client '%s' does not exist." % self.client)
             self.auth_message = "AUTH_CLIENT_UNKNOWN"
             return
 
         # If client is not enabled authentication must fail.
-        if not self.auth_client.enabled:
+        if not self.auth_client.enabled and not self.user.allow_disabled_login:
             self.logger.debug("Client '%s' is disabled." % self.client)
             # If client is disabled auth must fail.
             self.auth_failed = True
             self.auth_message = "AUTH_CLIENT_DISABLED"
             return
 
         # Get accessgroup from client.
@@ -810,16 +862,16 @@
                             % self.access_group)
             # If group does not exist auth must fail.
             self.auth_failed = True
             self.auth_message = "AUTH_GROUP_UNKNOWN"
             return
 
         # If group is not enabled authentication must fail.
-        if not self.auth_group.enabled:
-            self.logger.debug("Access group '%s' is disabled." % self.access_group)
+        if not self.auth_group.enabled and not self.user.allow_disabled_login:
+            self.logger.warning("Access group '%s' is disabled." % self.access_group)
             # If group is disabled auth must fail.
             self.auth_failed = True
             self.auth_message = "AUTH_GROUP_DISABLED"
             return
 
         # Check if sessions are enabled for the accessgroup.
         if self.create_sessions:
@@ -838,39 +890,54 @@
     def check_user(self):
         """ Check user status. """
         # If auth is already failed no need to check user status.
         if self.auth_failed:
             return
 
         # Make sure authentication with users realm is not disabled.
-        if not self.user.is_admin() and not self.realm_logout:
+        if not self.user.is_admin() \
+        and not self.realm_logout \
+        and not self.user.allow_disabled_login:
             user_realm = backend.get_object(object_type="realm",
                                         uuid=self.user.realm_uuid)
             if not user_realm.auth_enabled:
-                self.logger.debug("Authentication with realm is disabled: %s"
+                self.logger.warning("Authentication with realm is disabled: %s"
                                     % (user_realm.name))
                 self.auth_failed = True
                 self.count_fails = False
-                self.auth_message = "AUTH_WITH_REALM_DISABLED"
+                self.auth_message = "AUTH_REALM_DISABLED"
                 return
 
             # Make sure authentication with users site is not disabled.
             user_site = backend.get_object(object_type="site",
                                     uuid=self.user.site_uuid)
             if not user_site.auth_enabled:
-                self.logger.debug("Authentication with site is disabled: %s/%s"
+                self.logger.warning("Authentication with site is disabled: %s/%s"
                                     % (user_site.realm, user_site.name))
                 self.auth_failed = True
                 self.count_fails = False
-                self.auth_message = "AUTH_WITH_SITE_DISABLED"
+                self.auth_message = "AUTH_SITE_DISABLED"
+                return
+
+        # Make sure users unit is not disabled.
+        if not self.user.is_admin() \
+        and not self.realm_logout \
+        and not self.user.allow_disabled_login:
+            users_unit = self.user.get_parent_object()
+            if not users_unit.enabled:
+                self.logger.warning("Users unit is disabled: %s"
+                                    % (users_unit.name))
+                self.auth_failed = True
+                self.count_fails = False
+                self.auth_message = "AUTH_UNIT_DISABLED"
                 return
 
         # If user is disabled or locked authentication is failed.
         if not self.user.enabled:
-            self.logger.debug("User '%s' is disabled." % self.user.name)
+            self.logger.warning("User '%s' is disabled." % self.user.name)
             self.auth_failed = True
             self.auth_message = "AUTH_USER_DISABLED"
             return
 
         if self.user.is_blocked(self.access_group,
                                 realm=config.realm,
                                 site=config.site):
@@ -1223,14 +1290,18 @@
             # If we got "None" as status token verification was not successful
             # but is also not failed and we can check next token.
             return None
 
         # If status is not None we found token of this request.
         self.auth_token = token
         self.verify_token = _verify_token
+        if self.found_sotp:
+            config.auth_type = "sotp"
+        else:
+            config.auth_type = "token"
 
         # Verify auth token.
         if not self.auth_failed:
             self.verify_auth_token()
         if self.auth_failed:
             return
 
@@ -1831,25 +1902,29 @@
 
         # If we found the session master and it has sessions enabled it must be
         # used as session_start_group.
         if session_master and session_master.sessions_enabled:
             self.logger.debug("Found a valid session master: '%s'."
                         % session_master)
             self.session_start_group = session_master.name
-
         else:
             # If there is no session master use accessgroup from request as
             # session start group.
             self.session_start_group = self.access_group
 
         if not self.auth_failed:
+            # Make sure we have a valid password hash.
+            if not self.realm_login:
+                self.gen_pass_hash()
             # Create parent session instance.
+            session_logout_pass = slp.gen(self.one_iter_hash)
             session = Session(self.auth_type, self.user.name,
                                 pass_hash=self.password_hash,
                                 pass_hash_params=self.pass_hash_params,
+                                slp=session_logout_pass,
                                 token=self.auth_token.uuid,
                                 uuid=self.new_session_uuid,
                                 access_group=self.session_start_group,
                                 client=self.client, client_ip=self.client_ip)
             # Invoke method to create child sessions which also creates
             # parent session so we need no session.add() here. Child
             # sessions are always created regardless if sessions are
@@ -2117,26 +2192,26 @@
         self.reneg_salt = reneg_salt
         # Will hold password hash.
         self.password_hash = None
         self.pass_hash_params = None
         # Will hold NT hash of the request password.
         self.nt_hash = None
         # Will hold a one iteration hash of the password which is used for
-        # REALM sessions and to check for already used SOTP/SLP.
+        # REALM sessions and to check for already used SOTP.
         self.one_iter_hash = None
         # Will hold NT Key (if this is an MSCHAP request)
         self.nt_key = None
         # Will hold the SOTP.
         self.auth_sotp = None
         # Will hold the SLP.
         self.auth_slp = None
         # Will hold the SRP.
         self.auth_srp = None
         # Will hold all checked password hashes. (e.g checked for already used SOTP)
-        self.checked_hashes = { 'sotp' : [], 'slp' : [] }
+        self.checked_hashes = []
         # Indicates if we should verify sessions.
         self.verify_sessions = True
         # Indicates if we should create sessions.
         self.create_sessions = True
         # Indicates if we should create sessions for static password tokens to
         # speedup recurring auth requests.
         self.cache_static_passwords = False
@@ -2298,27 +2373,23 @@
 
         # Do not create cache sessions for JOIN accessgroup.
         if self.access_group == config.join_access_group:
             self.cache_static_passwords = False
 
         if not self.auth_failed and self.auth_status is False:
             # Generate hash to be used for REALM sessions and to check for used
-            # SLP/SOTP.
+            # SOTP.
             if self.password and not self.one_iter_hash:
                 self.one_iter_hash = self.get_one_iter_hash(self.password)
 
             # Check if the request contains an already used SOTP.
             if not self.auth_failed and not self.auth_status:
                 if self.access_group == config.realm_access_group:
                     if not self.session_logout and not self.realm_logout:
-                        self.check_used(pass_type="sotp")
-
-            # Check if request contains an already used SLP.
-            if self.session_logout or self.realm_logout:
-                self.check_used(pass_type="slp")
+                        self.check_used()
 
         # Try to verify request against existing session if enabled.
         if not self.auth_failed and self.verify_sessions:
             # Verify sessions.
             self.verify_user_sessions()
 
         # Handle JWT (cross-site) authentication.
@@ -2512,19 +2583,14 @@
                 self.rsp = sotp.derive_rsp(secret=dh_secret,
                                         hash_type=self.rsp_hash_type,
                                         salt=ecdh_server_pub_pem)
                 rsp_hash = self.get_one_iter_hash(self.rsp)
                 # Set password hash to realm session password hash.
                 self.password_hash = rsp_hash
 
-            ## Handle non-realm logins.
-            #else:
-            #    # Make sure we have a password hash.
-            #    self.gen_pass_hash(self.pass_hash_params)
-
             # Build JWT.
             if self.gen_jwt:
                 reason = "REALM_AUTH"
                 if self.realm_login:
                     reason = "REALM_LOGIN"
                 if self.session_reneg:
                     reason = "SESSION_RENEG"
@@ -2642,16 +2708,20 @@
             ssh_private_key = None
             if self.verify_token.token_type == "ssh":
                 if self.verify_token._ssh_private_key:
                     self.logger.debug("Got SSH private key from token: %s"
                                 % self.verify_token.rel_path)
                     ssh_private_key = self.verify_token._ssh_private_key
             auth_reply['ssh_private_key'] = ssh_private_key
-
             auth_reply['request_cacheable'] = self.request_cacheable
+            if self.auth_session:
+                auth_reply['slp'] = self.auth_session.slp
+
+            if self.access_group == config.sso_access_group:
+                auth_reply['session_hash'] = self.auth_session.pass_hash
 
             # Update last used timestamps for user and token.
             self.user.update_last_used_time()
             self.auth_token.update_last_used_time()
 
             if self.realm_login:
                 self.logger.debug("Realm login successful with token '%s'."
```

### Comparing `otpme-0.3.0a78/otpme/lib/classes/ca.py` & `otpme-0.3.0a79/otpme/lib/classes/ca.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/classes/client.py` & `otpme-0.3.0a79/otpme/lib/classes/role.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,78 +6,62 @@
     if os.environ['OTPME_DEBUG_MODULE_LOADING'] == "True":
         print(_("Loading module: %s" % __name__))
 except:
     pass
 
 from otpme.lib import oid
 from otpme.lib import cli
-from otpme.lib import stuff
 from otpme.lib import config
 from otpme.lib import backend
-from otpme.lib import otpme_acl
 from otpme.lib.locking import object_lock
 from otpme.lib.otpme_acl import check_acls
+from otpme.lib.register import register_module
+from otpme.lib.cache import assigned_role_cache
+from otpme.lib.cache import assigned_token_cache
+from otpme.lib.classes.otpme_object import OTPmeObject
 from otpme.lib.protocols.utils import register_commands
-from otpme.lib.daemon.clusterd import cluster_radius_reload
-from otpme.lib.classes.otpme_object import OTPmeClientObject
 from otpme.lib.classes.otpme_object import run_pre_post_add_policies
 
 from otpme.lib.classes.otpme_object import \
     get_acls as _get_acls
 from otpme.lib.classes.otpme_object import \
     get_value_acls as _get_value_acls
 from otpme.lib.classes.otpme_object import \
     get_default_acls as _get_default_acls
 from otpme.lib.classes.otpme_object import \
     get_recursive_default_acls as _get_recursive_default_acls
 
 from otpme.lib.exceptions import *
 
+logger = config.logger
+
 default_callback = config.get_callback()
 
-read_acls =  []
+read_acls = []
+write_acls = []
 
-write_acls =  [
-                "limit_logins",
-                "unlimit_logins",
-            ]
-
-read_value_acls =    {
-                    "view"      : [
-                                "token",
-                                "group",
-                                "accessgroup",
-                                "secret",
-                                "address",
-                                ],
+read_value_acls = {
+                    "view"      : [ "user", "token", "accessgroup", "group", "policy", "role" ],
             }
 
 write_value_acls = {
-                    "add"       : [
-                                "address",
-                                ],
-                    "delete"    : [
-                                "address",
-                                ],
-                    "edit"      : [
-                                "accessgroup",
-                                "secret",
-                                ],
-                }
+                    "add"       : [ "user", "token", "role" ],
+                    "remove"    : [ "user", "token", "role" ],
+            }
 
 default_acls = []
+
 recursive_default_acls = []
 
 commands = {
     'add'   : {
             'OTPme-mgmt-1.0'    : {
                 'missing'    : {
                     'method'            : 'add',
-                    'args'              : [],
-                    'oargs'             : ['address', 'unit'],
+                    'oargs'             : ['unit'],
                     'job_type'          : 'process',
                     },
                 'exists'    : {
                     'method'            : 'add',
                     'job_type'          : 'process',
                     },
                 },
@@ -89,54 +73,58 @@
                     'job_type'          : 'process',
                     },
                 },
             },
     'show'   : {
             'OTPme-mgmt-1.0'    : {
                 'missing'    : {
-                    'method'            : cli.show_getter("client"),
+                    'method'            : cli.show_getter("role"),
                     'args'              : ['realm'],
                     'oargs'              : [
                                         'max_len',
                                         'show_all',
                                         'output_fields',
-                                        'max_policies',
                                         'search_regex',
                                         'sort_by',
                                         'reverse',
                                         'header',
                                         'csv',
                                         'csv_sep',
                                         'realm',
                                         'site',
+                                        'max_roles',
+                                        'max_tokens',
+                                        'max_ags',
+                                        'max_groups',
+                                        'max_policies',
                                         ],
                     'job_type'          : 'thread',
                     },
                 'exists'    : {
                     'method'            : 'show',
                     'args'              : ['realm'],
                     'job_type'          : 'thread',
                     },
                 },
             },
     'list'   : {
             'OTPme-mgmt-1.0'    : {
                 'missing'    : {
-                    'method'            : cli.list_getter("client"),
+                    'method'            : cli.list_getter("role"),
                     'oargs'              : [
                                         'reverse',
                                         'show_all',
                                         'attribute',
                                         'search_regex',
                                         'sort_by',
                                         ],
                     'job_type'          : None,
                     },
                 'exists'    : {
-                    'method'            : cli.list_getter("client"),
+                    'method'            : cli.list_getter("role"),
                     'oargs'              : [
                                         'reverse',
                                         'show_all',
                                         'attribute',
                                         'search_regex',
                                         'sort_by',
                                         ],
@@ -199,109 +187,106 @@
             'OTPme-mgmt-1.0'    : {
                 'exists'    : {
                     'method'            : 'disable_acl_inheritance',
                     'job_type'          : 'process',
                     },
                 },
             },
-    'secret'   : {
+    'add_token'   : {
             'OTPme-mgmt-1.0'    : {
                 'exists'    : {
-                    'method'            : 'change_secret',
-                    'oargs'             : ['auto_secret', 'secret'],
+                    'method'            : 'add_token',
+                    'args'              : ['token_path'],
+                    'oargs'             : ['token_options', 'login_interfaces', 'sign', 'tags'],
                     'job_type'          : 'process',
                     },
                 },
             },
-    'show_secret'   : {
+    'remove_token'   : {
             'OTPme-mgmt-1.0'    : {
                 'exists'    : {
-                    'method'            : 'show_secret',
+                    'method'            : 'remove_token',
+                    'args'              : ['token_path'],
+                    'oargs'             : ['keep_sign'],
                     'job_type'          : 'process',
                     },
                 },
             },
-    'access_group'   : {
+    'add_role'   : {
             'OTPme-mgmt-1.0'    : {
                 'exists'    : {
-                    'method'            : 'change_access_group',
-                    'args'              : ['access_group'],
+                    'method'            : 'add_role',
+                    'args'              : ['role_name'],
                     'job_type'          : 'process',
                     },
                 },
             },
-    'add_address'   : {
+    'remove_role'   : {
             'OTPme-mgmt-1.0'    : {
                 'exists'    : {
-                    'method'            : 'add_address',
-                    'args'              : ['address'],
+                    'method'            : 'remove_role',
+                    'args'              : ['role_name'],
                     'job_type'          : 'process',
                     },
                 },
             },
-    'del_address'   : {
+    'add_sync_user'   : {
             'OTPme-mgmt-1.0'    : {
                 'exists'    : {
-                    'method'            : 'del_address',
-                    'args'              : ['address'],
+                    'method'            : 'add_sync_user',
+                    'args'              : ['user_name'],
                     'job_type'          : 'process',
                     },
                 },
             },
-    'add_role'   : {
+    'remove_sync_user'   : {
             'OTPme-mgmt-1.0'    : {
                 'exists'    : {
-                    'method'            : 'add_role',
-                    'args'              : ['role_name'],
-                    'job_type'          : 'thread',
+                    'method'            : 'remove_sync_user',
+                    'args'              : ['user_name'],
+                    'job_type'          : 'process',
                     },
                 },
             },
-    'remove_role'   : {
+    'list_sync_users'   : {
             'OTPme-mgmt-1.0'    : {
                 'exists'    : {
-                    'method'            : 'remove_role',
-                    'args'              : ['role_name'],
+                    'method'            : 'get_sync_users',
+                    'oargs'             : ['return_type'],
+                    'dargs'             : {'return_type':'name'},
                     'job_type'          : 'thread',
                     },
                 },
             },
-    'add_token'   : {
+    'list_users'   : {
             'OTPme-mgmt-1.0'    : {
                 'exists'    : {
-                    'method'            : 'add_token',
-                    'args'              : ['token_path'],
-                    'oargs'             : ['token_options', 'login_interfaces', 'sign', 'tags'],
-                    'job_type'          : 'process',
+                    'method'            : 'get_token_users',
+                    'oargs'             : ['return_type'],
+                    'dargs'             : {'return_type':'name'},
+                    'job_type'          : 'thread',
                     },
                 },
             },
-    'remove_token'   : {
+    'list_tokens'   : {
             'OTPme-mgmt-1.0'    : {
                 'exists'    : {
-                    'method'            : 'remove_token',
-                    'args'              : ['token_path'],
-                    'oargs'             : ['keep_sign'],
+                    'method'            : 'get_tokens',
+                    'oargs'             : ['return_type', 'token_types'],
+                    'dargs'             : {'return_type':'rel_path', 'skip_disabled':False},
                     'job_type'          : 'process',
                     },
                 },
             },
-    'limit_logins'   : {
+    'list_roles'   : {
             'OTPme-mgmt-1.0'    : {
                 'exists'    : {
-                    'method'            : 'limit_logins',
-                    'job_type'          : 'thread',
-                    },
-                },
-            },
-    'unlimit_logins'   : {
-            'OTPme-mgmt-1.0'    : {
-                'exists'    : {
-                    'method'            : 'unlimit_logins',
-                    'job_type'          : 'thread',
+                    'method'            : 'get_roles',
+                    'oargs'             : ['recursive'],
+                    'job_type'          : 'process',
                     },
                 },
             },
     'list_policies'   : {
             'OTPme-mgmt-1.0'    : {
                 'exists'    : {
                     'method'            : 'get_policies',
@@ -466,14 +451,23 @@
             'OTPme-mgmt-1.0'    : {
                 'exists'    : {
                     'method'            : 'get_object_classes',
                     'job_type'          : 'thread',
                     },
                 },
             },
+    'show_ldif'   : {
+            'OTPme-mgmt-1.0'    : {
+                'exists'    : {
+                    'method'            : 'get_ldif',
+                    'args'              : ['attributes'],
+                    'job_type'          : 'thread',
+                    },
+                },
+            },
     'show_acls'   : {
             'OTPme-mgmt-1.0'    : {
                 'exists'    : {
                     'method'            : 'get_acls',
                     'job_type'          : 'thread',
                     },
                 },
@@ -523,168 +517,259 @@
 
 def get_default_acls(**kwargs):
     return _get_default_acls(default_acls, **kwargs)
 
 def get_recursive_default_acls(**kwargs):
     return _get_recursive_default_acls(recursive_default_acls, **kwargs)
 
-DEFAULT_UNIT = "clients"
+DEFAULT_UNIT = "roles"
+
 REGISTER_BEFORE = []
 REGISTER_AFTER = [
                 "otpme.lib.classes.unit",
-                "otpme.lib.classes.group",
                 ]
 
 def register():
+    register_dn()
     register_oid()
     register_hooks()
     register_backend()
     register_object_unit()
     register_sync_settings()
-    register_commands("client", commands)
-    # Register index attributes.
-    config.register_index_attribute("address")
+    register_commands("role", commands)
+    register_module("otpme.lib.classes.token")
+
+def register_dn():
+    """ Register DN attribute. """
+    config.register_dn_attribute("role", "cn")
 
 def register_hooks():
-    config.register_auth_on_action_hook("client", "add_token")
-    config.register_auth_on_action_hook("client", "remove_token")
-    config.register_auth_on_action_hook("client", "add_address")
-    config.register_auth_on_action_hook("client", "del_address")
-    config.register_auth_on_action_hook("client", "change_secret")
-    config.register_auth_on_action_hook("client", "change_access_group")
-    config.register_auth_on_action_hook("client", "show_secret")
-    config.register_auth_on_action_hook("client", "limit_logins")
-    config.register_auth_on_action_hook("client", "unlimit_logins")
+    config.register_auth_on_action_hook("role", "add")
+    config.register_auth_on_action_hook("role", "delete")
+    config.register_auth_on_action_hook("role", "add_role")
+    config.register_auth_on_action_hook("role", "remove_role")
+    config.register_auth_on_action_hook("role", "add_token")
+    config.register_auth_on_action_hook("role", "remove_token")
 
 def register_object_unit():
     """ Register default unit for this object type. """
-    config.register_default_unit("client", DEFAULT_UNIT)
+    config.register_default_unit("role", DEFAULT_UNIT)
     config.register_base_object("unit", DEFAULT_UNIT)
 
 def register_oid():
     full_oid_schema = [ 'realm', 'site', 'unit', 'name' ]
     read_oid_schema = [ 'realm', 'site', 'name' ]
     # OID regex stuff.
     unit_path_re = oid.object_regex['unit']['path']
-    client_name_re = '([0-9A-Za-z]([0-9A-Za-z_.-]*[0-9A-Za-z]){0,})'
-    client_path_re = '%s[/]%s' % (unit_path_re, client_name_re)
-    client_oid_re = 'client|%s' % client_path_re
-    oid.register_oid_schema(object_type="client",
+    role_name_re = '([0-9A-Za-z]([0-9A-Za-z_:.-]*[0-9A-Za-z]){0,})'
+    role_path_re = '%s[/]%s' % (unit_path_re, role_name_re)
+    role_oid_re = 'role|%s' % role_path_re
+    oid.register_oid_schema(object_type="role",
                             full_schema=full_oid_schema,
                             read_schema=read_oid_schema,
-                            name_regex=client_name_re,
-                            path_regex=client_path_re,
-                            oid_regex=client_oid_re)
+                            name_regex=role_name_re,
+                            path_regex=role_path_re,
+                            oid_regex=role_oid_re)
     rel_path_getter = lambda x: x[2:]
-    oid.register_rel_path_getter(object_type="client",
+    oid.register_rel_path_getter(object_type="role",
                                 getter=rel_path_getter)
 
 def register_backend():
     """ Register object for the file backend. """
-    client_dir_extension = "client"
-    def path_getter(client_oid):
-        return backend.config_path_getter(client_oid, client_dir_extension)
+    role_dir_extension = "role"
+    def path_getter(role_oid):
+        return backend.config_path_getter(role_oid, role_dir_extension)
     def index_rebuild(objects):
         after = [
                 'realm',
                 'site',
                 'unit',
                 'group',
                 'ca',
                 'node',
                 'host',
                 'user',
                 'token',
                 'accessgroup',
+                'client',
                 ]
-        return backend.rebuild_object_index("client", objects, after)
+        return backend.rebuild_object_index("role", objects, after)
     # Register object to config.
-    config.register_object_type(object_type="client",
+    config.register_object_type(object_type="role",
                             tree_object=True,
                             uniq_name=True,
-                            add_after=["host"],
-                            sync_after=["user", "token"],
+                            add_after=["token"],
+                            sync_before=["token", "user"],
                             object_cache=1024,
                             cache_region="tree_object",
                             backup_attributes=['realm', 'site', 'name'])
-    # Register index attributes.
-    config.register_index_attribute('accessgroup')
     # Register object to backend.
-    class_getter = lambda: Client
-    backend.register_object_type(object_type="client",
-                                dir_name_extension=client_dir_extension,
+    class_getter = lambda: Role
+    backend.register_object_type(object_type="role",
+                                dir_name_extension=role_dir_extension,
                                 class_getter=class_getter,
                                 index_rebuild_func=index_rebuild,
                                 path_getter=path_getter)
 
 def register_sync_settings():
     """ Register sync settings. """
-    config.register_object_sync(host_type="node", object_type="client")
+    config.register_object_sync(host_type="node", object_type="role")
+    config.register_object_sync(host_type="host", object_type="role")
 
-class Client(OTPmeClientObject):
-    """ Creates client object """
+def get_roles(role_uuid=None, skip_disabled=False, parent=False,
+    recursive=True, return_type="name", return_attributes=None):
+
+    def _get_roles(uuid, parent=False, return_attributes=None):
+        return_attrs = ['name', 'enabled', 'full_oid', 'site']
+        if return_attributes is not None:
+            return_attrs = list(set(return_attrs + return_attributes))
+        if parent:
+            result = backend.search(object_type="role",
+                                    attribute="role",
+                                    value=uuid,
+                                    return_attributes=return_attrs)
+        else:
+            child_roles = backend.search(object_type="role",
+                                        attribute="uuid",
+                                        value=uuid,
+                                        return_attributes=['role'])
+            result = []
+            if child_roles:
+                result = backend.search(object_type="role",
+                                        attribute="uuid",
+                                        values=child_roles,
+                                        return_attributes=return_attrs)
+        return result
+
+    result = []
+    processed_roles = []
+    # Get roles roles.
+    check_roles = _get_roles(uuid=role_uuid,
+                            parent=parent,
+                            return_attributes=return_attributes)
+    if not check_roles:
+        return result
+    oid_result = backend.search(object_type="role",
+                            attribute="uuid",
+                            value=role_uuid,
+                            return_type="oid")
+    role_oid = oid_result[0]
+    role_site = role_oid.site
+
+    loop_found = False
+    role_uuid_list = []
+    while True:
+        for uuid in list(check_roles):
+            x_role_data = check_roles.pop(uuid)
+            if uuid == role_uuid:
+                continue
+            # Get role data.
+            x_name = x_role_data['name']
+            x_site = x_role_data['site']
+            x_full_oid = x_role_data['full_oid']
+            x_enabled = x_role_data['enabled'][0]
+            if uuid in role_uuid_list:
+                continue
+            if skip_disabled:
+                if not x_enabled:
+                    continue
+            role_uuid_list.append(uuid)
+            if return_attributes:
+                result.append(x_role_data)
+            elif return_type == "instance":
+                role = backend.get_object(object_type="role", uuid=uuid)
+                result.append(role)
+            elif return_type == "uuid":
+                result.append(uuid)
+            elif return_type == "full_oid":
+                result.append(x_full_oid)
+            elif return_type == "name":
+                if x_site == role_site:
+                    role_name = x_name
+                else:
+                    role_name = "%s/%s" % (x_site, x_name)
+                result.append(role_name)
+            else:
+                msg = (_("Unknown return type: %s") % return_type)
+                raise OTPmeException(msg)
+            if uuid in processed_roles:
+                loop_found = True
+                continue
+            processed_roles.append(uuid)
+            # Gets role roles.
+            _result = _get_roles(uuid=uuid, parent=parent,
+                            return_attributes=return_attributes)
+            for x in _result:
+                check_roles[x] = _result[x]
+        if not recursive:
+            break
+        if not check_roles:
+            break
+        if loop_found:
+            break
+    if not return_attributes:
+        result = sorted(result)
+    return result
+
+class Role(OTPmeObject):
+    """ Role object """
     commands = commands
-    def __init__(self, object_id=None, name=None, realm=None,
-        unit=None, site=None, path=None, access_group=None, **kwargs):
-        # Set our type (used in parent class).
-        self.type = "client"
+    def __init__(self, object_id=None, path=None, name=None,
+        unit=None, site=None, realm=None, **kwargs):
+        # Set our type (used in parent class)
+        self.type = "role"
 
         # Call parent class init.
-        super(Client, self).__init__(object_id=object_id,
+        super(Role, self).__init__(object_id=object_id,
                                         realm=realm,
                                         site=site,
                                         unit=unit,
                                         name=name,
                                         path=path,
                                         **kwargs)
         self._acls = get_acls()
         self._value_acls = get_value_acls()
         self._default_acls = get_default_acls()
         self._recursive_default_acls = get_recursive_default_acls()
 
-        self.access_group = None
-        self.access_group_uuid = None
-        if access_group:
-            self.change_access_group(access_group=access_group,
-                                    verify_acls=False)
-
-        self.secret = None
-        self.secret_len = 32
-        # Clients should not inherit ACLs by default.
+        # Roles should not inherit ACLs by default.
         self.acl_inheritance_enabled = False
-        self.logins_limited = False
-        self.radius_reload = False
 
         self._sync_fields = {
+                    'host'  : {
+                        'trusted'  : [
+                            "EXTENSIONS",
+                            "OBJECT_CLASSES",
+                            "TOKENS",
+                            "ROLES",
+                            "SYNC_USERS",
+                            ]
+                        },
+
                     'node'  : {
                         'untrusted'  : [
                             "EXTENSIONS",
                             "OBJECT_CLASSES",
-                            "EXTENSION_ATTRIBUTES",
                             "TOKENS",
+                            "ROLES",
+                            "SYNC_USERS",
                             ]
                         },
                     }
 
     def _get_object_config(self):
         """ Get object config dict. """
         object_config = {
-                        'ADDRESSES'                 : {
-                                                        'var_name'  : 'addresses',
+                        'SYNC_USERS'                : {
+                                                        'var_name'  : 'sync_users',
                                                         'type'      : list,
                                                         'required'  : False,
                                                     },
 
-                        'ACCESS_GROUP'              : {
-                                                        'var_name'  : 'access_group_uuid',
-                                                        'type'      : 'uuid',
-                                                        'required'  : False,
-                                                    },
-
-                        'ROLES'                     : {
+                        'ROLES'                    : {
                                                         'var_name'  : 'roles',
                                                         'type'      : list,
                                                         'required'  : False,
                                                     },
 
                         'TOKENS'                    : {
                                                         'var_name'  : 'tokens',
@@ -693,171 +778,255 @@
                                                     },
 
                         'TOKEN_OPTIONS'             : {
                                                         'var_name'  : 'token_options',
                                                         'type'      : dict,
                                                         'required'  : False,
                                                     },
-
                         'TOKEN_LOGIN_INTERFACES'    : {
                                                         'var_name'  : 'token_login_interfaces',
                                                         'type'      : dict,
                                                         'required'  : False,
                                                     },
-                        'SECRET'    : {
-                                                        'var_name'  : 'secret',
-                                                        'type'      : str,
-                                                        'required'  : False,
-                                                        'encryption': config.disk_encryption,
-                                                    },
             }
 
-        return super(Client, self)._get_object_config(object_config=object_config)
+        return object_config
 
     def set_variables(self):
-        """ Set instance variables. """
-        if self.access_group_uuid:
-            ag = backend.get_object(object_type="accessgroup",
-                                    uuid=self.access_group_uuid,
-                                    realm=self.realm,
-                                    site=self.site)
-            if ag:
-                self.access_group = ag.name
+        """ Set instance variables """
         # Set OID.
         self.set_oid()
 
     def _set_name(self, name):
         """ Set object name. """
         # Make sure name is a string.
         name = str(name)
-        # Only base clients must have uppercase names.
-        base_clients = config.get_base_objects("client")
-        if name.upper() in base_clients:
+        # Only base roles must have uppercase names.
+        base_roles = config.get_base_objects("role")
+        if name.upper() in base_roles:
             self.name = name.upper()
         else:
             self.name = name.lower()
 
-    def _write(self, **kwargs):
-        """ Wrapper to make sure radius gets reloaded. """
-        result = super(Client, self)._write(**kwargs)
-        if not self.radius_reload:
+    @assigned_token_cache.cache_method()
+    def is_assigned_token(self, token_uuid, check_parent_roles=True,
+        skip_disabled_roles=True, processed_roles=[]):
+        if token_uuid in self.tokens:
+            return True
+        if not check_parent_roles:
+            return False
+        child_roles = self.get_roles(return_type="instance",
+                            skip_disabled=skip_disabled_roles,
+                            recursive=False)
+        for role in child_roles:
+            if skip_disabled_roles:
+                if not role.enabled:
+                    continue
+            if role.uuid in processed_roles:
+                continue
+            processed_roles.append(role.uuid)
+            if role.is_assigned_token(token_uuid):
+                return True
+        return False
+
+    @assigned_role_cache.cache_method()
+    def is_assigned_role(self, role_uuid, check_parent_roles=True,
+        skip_disabled_roles=True, processed_roles=[]):
+        if role_uuid in self.roles:
+            return True
+        if not check_parent_roles:
+            return False
+        parent_roles = self.get_roles(parent=True,
+                            return_type="instance",
+                            skip_disabled=skip_disabled_roles,
+                            recursive=False)
+        for role in parent_roles:
+            if skip_disabled_roles:
+                if not role.enabled:
+                    continue
+            if role.uuid in processed_roles:
+                continue
+            processed_roles.append(role.uuid)
+            if role.is_assigned_role(role_uuid, processed_roles=processed_roles):
+                return True
+        return False
+
+    @cli.check_rapi_opts()
+    def get_roles(self, return_type="name", parent=False,
+        skip_disabled=False, recursive=False, _caller="API",
+        callback=default_callback, **kwargs):
+        """ Get all roles of this role. """
+        result = get_roles(role_uuid=self.uuid,
+                            parent=parent,
+                            return_type=return_type,
+                            skip_disabled=skip_disabled,
+                            recursive=recursive)
+        if _caller == "API":
             return result
-        self.radius_reload = False
-        cluster_radius_reload()
-        return result
+        if _caller == "RAPI":
+            result = ",".join(result)
+        if _caller == "CLIENT":
+            result = "\n".join(result)
+        return callback.ok(result)
+
+    @cli.check_rapi_opts()
+    def get_access_groups(self, return_type="name", _caller="API",
+        callback=default_callback, **kwargs):
+        """ Return list with all access group names this role is in. """
+        result = backend.search(realm=self.realm,
+                            site=self.site,
+                            attribute="role",
+                            value=self.uuid,
+                            object_type="accessgroup",
+                            return_type=return_type)
+        if _caller == "RAPI":
+            result = ",".join(result)
+        if _caller == "CLIENT":
+            result = "\n".join(result)
+        return callback.ok(result)
+
+    @cli.check_rapi_opts()
+    def get_groups(self, return_type="uuid", _caller="API",
+        callback=default_callback, **kwargs):
+        """ Return list with all group names this role is in. """
+        result = backend.search(realm=self.realm,
+                            site=self.site,
+                            attribute="role",
+                            value=self.uuid,
+                            object_type="group",
+                            return_type=return_type)
+        if _caller == "RAPI":
+            result = ",".join(result)
+        if _caller == "CLIENT":
+            result = "\n".join(result)
+        return callback.ok(result)
 
-    # xxxxxxxxxxxxxxxxxxx
-    # FIXME: check if IP is valid!!!
-    @object_lock()
-    @check_acls(['add:address'])
-    def add_address(self, address, run_policies=True,
-        callback=default_callback, _caller="API", **kwargs):
-        """ Adds a address to this client. """
-        if address in self.addresses:
-            return callback.error(_("Address '%s' already added to this client.")
-                                    % address)
-        if run_policies:
-            try:
-                self.run_policies("modify",
-                                callback=callback,
-                                _caller=_caller)
-                self.run_policies("add_address",
-                                callback=callback,
-                                _caller=_caller)
-            except Exception as e:
-                return callback.error()
-        self.addresses.append(address)
-        # Update index.
-        self.add_index("address", address)
-        # Make sure radius gets reloaded
-        self.radius_reload = True
-        return self._cache(callback=callback)
+    @object_lock(full_lock=True)
+    @backend.transaction
+    def rename(self, new_name, callback=default_callback, _caller="API", **kwargs):
+        """ Rename role. """
+        base_roles = config.get_base_objects("role")
+        if self.name in base_roles:
+            return callback.error("Cannot rename base role.")
+        # Build new OID.
+        new_oid = oid.get(object_type="role",
+                        realm=self.realm,
+                        site=self.site,
+                        unit=self.unit,
+                        name=new_name)
+        return self._rename(new_oid, callback=callback, _caller=_caller, **kwargs)
 
-    @object_lock()
-    @check_acls(['delete:address'])
-    def del_address(self, address, run_policies=True,
-        callback=default_callback, _caller="API", **kwargs):
-        """ Deletes a address from this client. """
-        if not address in self.addresses:
-            return callback.error(_("Address '%s' is not an address of this client.")
-                                    % address)
-        if run_policies:
-            try:
-                self.run_policies("modify",
-                                callback=callback,
-                                _caller=_caller)
-                self.run_policies("del_address",
-                                callback=callback,
-                                _caller=_caller)
-            except Exception as e:
-                return callback.error()
-        self.addresses.remove(address)
-        # Update index.
-        self.del_index("address", address)
-        # Make sure radius gets reloaded
-        self.radius_reload = True
-        return self._cache(callback=callback)
+    @object_lock(full_lock=True)
+    @backend.transaction
+    @run_pre_post_add_policies()
+    def add(self, verbose_level=0, callback=default_callback, **kwargs):
+        """ Add a role. """
+        # Run parent class stuff e.g. verify ACLs.
+        result = self._prepare_add(callback=callback, **kwargs)
+        if result is False:
+            return callback.error()
+        # Add object using parent class.
+        return OTPmeObject.add(self, verbose_level=verbose_level,
+                                callback=callback, **kwargs)
+
+    @object_lock(full_lock=True)
+    @backend.transaction
+    def delete(self, force=False, run_policies=True,
+        verify_acls=True, verbose_level=0, _caller="API",
+        callback=default_callback, **kwargs):
+        """ Delete role. """
+        if not self.exists():
+            return callback.error("Role does not exist exists.")
+
+        base_roles = config.get_base_objects("role")
+        if self.name in base_roles:
+            return callback.error("Cannot delete base role.")
+
+        # Get parent object to check ACLs.
+        parent_object = self.get_parent_object()
+        if verify_acls:
+            if not self.verify_acl("delete:object"):
+                del_acl = "delete:%s" % self.type
+                if not parent_object.verify_acl(del_acl):
+                    msg = (_("Permission denied: %s") % self.name)
+                    return callback.error(msg, exception=PermissionDenied)
 
-    @object_lock()
-    @check_acls(['edit:accessgroup'])
-    def change_access_group(self, access_group=None,
-        run_policies=True, callback=default_callback,
-        _caller="API", **kwargs):
-        """ Change client access group. """
-        from otpme.lib.classes.accessgroup import AccessGroup
-        if access_group == self.access_group:
-            return callback.error(_("Group '%s' is already access group of "
-                                    "this client.") % access_group)
         if run_policies:
             try:
-                self.run_policies("modify",
-                                callback=callback,
-                                _caller=_caller)
-                self.run_policies("change_access_group",
-                                callback=callback,
-                                _caller=_caller)
+                self.run_policies("delete", callback=callback, _caller=_caller)
             except Exception as e:
                 return callback.error()
-        if access_group:
-            # Create access group instance.
-            g = AccessGroup(name=access_group,
-                            realm=self.realm,
-                            site=self.site)
-            if not g.exists():
-                return callback.error(_("Group '%s' does not exist.")
-                                        % self.access_group_uuid)
-            # Append access group UUID to access groups.
-            self.access_group_uuid = g.uuid
-            self.access_group = g.name
-            # Update Index.
-            self.update_index('accessgroup', self.access_group_uuid)
-        else:
-            self.access_group_uuid = None
-            self.access_group = None
-            # Update Index.
-            self.del_index('accessgroup')
 
-        return self._cache(callback=callback)
+        if not force:
+            exception = ""
+            # List that will hold all tokens that uses this role.
+            token_list = []
+            # Get all tokens from this role.
+            for t_uuid in self.tokens:
+                token = backend.get_object(object_type="token", uuid=t_uuid)
+                if token:
+                    token_list.append(token.rel_path)
+                else:
+                    token_list.append(t_uuid)
+
+            if token_list:
+                exception = (_("%sRole has member tokens: %s\n")
+                            % (exception, ", ".join(token_list)))
+
+            # List that will hold all groups that uses this role.
+            accessgroup_list = self.get_access_groups()
+
+            if accessgroup_list:
+                exception = (_("%sRole is member of this access groups: %s\n")
+                            % (exception, ", ".join(accessgroup_list)))
+
+            if exception != "":
+                if self.confirmation_policy != "force":
+                    if self.confirmation_policy == "paranoid":
+                        answer = callback.ask(_("%sPlease type '%s' to delete object: ")
+                                            % (exception, self.name))
+                        if answer != self.name:
+                            return callback.abort()
+                    else:
+                        answer = callback.ask(_("%sDelete role '%s'?: ")
+                                            % (exception, self.name))
+                        if answer.lower() != "y":
+                            return callback.abort()
+            else:
+                if self.confirmation_policy != "force":
+                    if self.confirmation_policy == "paranoid":
+                        answer = callback.ask(_("Please type '%s' to delete object: ") % self.name)
+                        if answer != self.name:
+                            return callback.abort()
+                    else:
+                        answer = callback.ask(_("Delete role '%s'?: ") % self.name)
+                        if answer.lower() != "y":
+                            return callback.abort()
+
+        # Delete object using parent class.
+        return OTPmeObject.delete(self, verbose_level=verbose_level,
+                                    force=force, callback=callback)
 
-    @object_lock()
     @check_acls(['remove:orphans'])
+    @object_lock()
     def remove_orphans(self, force=False, run_policies=True,
         verbose_level=0, callback=default_callback,
         _caller="API", **kwargs):
         """ Remove orphan UUIDs. """
         if run_policies:
             try:
                 self.run_policies("modify",
                                 callback=callback,
                                 _caller=_caller)
                 self.run_policies("remove_orphans",
                                 callback=callback,
                                 _caller=_caller)
             except Exception as e:
                 return callback.error()
+
         acl_list = self.get_orphan_acls()
         policy_list = self.get_orphan_policies()
 
         token_list = []
         token_uuids = set(self.tokens + list(self.token_options))
         for i in token_uuids:
             token_oid = backend.get_oid(object_type="token", uuid=i)
@@ -876,188 +1045,132 @@
                     msg = (_("%s%s|%s: Found the following orphan policies: %s\n")
                             % (msg, self.type, self.name, ",".join(policy_list)))
 
             if token_list:
                 msg = (_("%s%s|%s: Found the following orphan token UUIDs: %s\n")
                         % (msg, self.type, self.name, ",".join(token_list)))
 
+            if msg:
+                answer = callback.ask("%sRemove?: " % msg)
+                if answer.lower() != "y":
+                    return callback.abort()
+
         object_changed = False
         if acl_list:
             if self.remove_orphan_acls(force=True, verbose_level=verbose_level,
-                                                callback=callback, **kwargs):
+                                        callback=callback, **kwargs):
                 object_changed = True
 
         if policy_list:
             if self.remove_orphan_policies(force=True, verbose_level=verbose_level,
                                                 callback=callback, **kwargs):
                 object_changed = True
 
         for i in token_list:
             if verbose_level > 0:
-                callback.send(_("Removing orphan token UUID: %s" % i))
+                callback.send(_("Removing orphan token UUID: %s") % i)
             object_changed = True
-            if i in self.tokens:
+            try:
                 self.tokens.remove(i)
-            if i in self.token_options:
+            except KeyError:
+                pass
+            try:
                 self.token_options.pop(i)
+            except KeyError:
+                pass
+            try:
+                self.token_login_interfaces.pop(i)
+            except KeyError:
+                pass
 
         if not object_changed:
             msg = None
             if verbose_level > 0:
                 msg = (_("No orphan objects found for %s: %s")
                         % (self.type, self.name))
             return callback.ok(msg)
 
         return self._cache(callback=callback)
 
-    @object_lock(full_lock=True)
-    def rename(self, new_name, callback=default_callback, _caller="API", **kwargs):
-        """ Rename client. """
-        base_clients = config.get_base_objects("client")
-        if self.name in base_clients:
-            return callback.error("Cannot rename base client.")
-
-        # Build new OID.
-        new_oid = oid.get(object_type="client",
-                        realm=self.realm,
-                        site=self.site,
-                        unit=self.unit,
-                        name=new_name)
-        result = self._rename(new_oid, callback=callback, _caller=_caller, **kwargs)
-        # Make sure radius gets reloaded
-        self.radius_reload = True
-        return result
-
-    @object_lock(full_lock=True)
-    @run_pre_post_add_policies()
-    def add(self, address=None, verbose_level=0, callback=default_callback, **kwargs):
-        """ Add a client. """
-        if address:
-            result = backend.search(object_type="client",
-                                    attribute="address",
-                                    value=address,
-                                    return_type="name")
-            if result:
-                existing_client = result[0]
-                msg = "Client with this address already exists: %s" % existing_client
-                return callback.error(msg)
-
-        # Run parent class stuff e.g. verify ACLs.
-        result = self._prepare_add(callback=callback, **kwargs)
-        if result is False:
-            return callback.error()
-        self.secret = stuff.gen_secret(32)
-        # Add object using parent class.
-        add_result = super(Client, self).add(verbose_level=verbose_level,
-                                            callback=callback, **kwargs)
-        if not add_result:
-            msg = "Failed to add client."
-            return callback.error(msg)
-
-        if address:
-            self.add_address(address)
-            msg = "Radius secret: %s" % self.secret
-            callback.send(msg)
-        # Make sure radius gets reloaded
-        self.radius_reload = True
-        return callback.ok()
-
-    @object_lock(full_lock=True)
-    def delete(self, force=False, run_policies=True, verify_acls=True,
-        verbose_level=0, callback=default_callback, _caller="API", **kwargs):
-        """ Delete client. """
-        if not self.exists():
-            return callback.error("Client does not exist exists.")
-
-        base_clients = config.get_base_objects("client")
-        if self.name in base_clients:
-            return callback.error("Cannot delete base client.")
-
-        # Get parent object to check ACLs.
-        parent_object = self.get_parent_object()
-        if verify_acls:
-            if not self.verify_acl("delete:object"):
-                del_acl = "delete:%s" % self.type
-                if not parent_object.verify_acl(del_acl):
-                    msg = (_("Permission denied: %s") % self.name)
-                    return callback.error(msg, exception=PermissionDenied)
-
-        if run_policies:
-            try:
-                self.run_policies("delete", callback=callback, _caller=_caller)
-            except Exception as e:
-                return callback.error()
-
-        if not force:
-            if self.confirmation_policy == "paranoid":
-                msg = "Please type '%s' to delete object: " % self.name
-                answer = callback.ask(msg)
-                if answer != self.name:
-                    return callback.abort()
-            else:
-                answer = callback.ask(_("Delete client '%s'?: ") % self.name)
-                if answer.lower() != "y":
-                    return callback.abort()
-
-        # Delete object using parent class.
-        result = super(Client, self).delete(verbose_level=verbose_level,
-                                        force=force, callback=callback)
-        # Make sure radius gets reloaded.
-        cluster_radius_reload()
-        return result
-
     def show_config(self, callback=default_callback, **kwargs):
-        """ Show client config. """
+        """ Show role config. """
         if not self.verify_acl("view_public:object"):
             msg = ("Permission denied.")
             return callback.error(msg, exception=PermissionDenied)
 
+        token_list = []
+        if self.tokens:
+            if self.verify_acl("view:token."):
+                return_attrs = ['rel_path']
+                token_list = backend.search(object_type="token",
+                                            join_object_type="role",
+                                            join_search_attr="uuid",
+                                            join_search_val=self.uuid,
+                                            join_attribute="token",
+                                            attribute="uuid",
+                                            value="*",
+                                            return_attributes=return_attrs)
+            token_list.sort()
+
+        role_list = []
+        if self.roles:
+            if self.verify_acl("view:role."):
+                return_attrs = ['site', 'name']
+                roles_result = backend.search(object_type="role",
+                                            join_object_type="role",
+                                            join_search_attr="uuid",
+                                            join_search_val=self.uuid,
+                                            join_attribute="role",
+                                            attribute="uuid",
+                                            value="*",
+                                            return_attributes=return_attrs)
+                for x in roles_result:
+                    role_site = roles_result[x]['site']
+                    role_name = roles_result[x]['name']
+                    if role_site != config.site:
+                        role_name = "%s/%s" % (role_site, role_name)
+                    role_list.append(role_name)
+            role_list.sort()
+
         lines = []
 
-        if self.verify_acl("view:token") \
-        or self.verify_acl("add:token") \
-        or self.verify_acl("remove:token"):
-            token_list = []
-            for i in self.tokens:
-                token_oid = backend.get_oid(i, instance=True)
-                # Add UUIDs of orphan tokens.
-                if not token_oid:
-                    token_list.append(i)
-                    continue
-                if not otpme_acl.access_granted(object_id=token_oid,
-                                                acl="view_public:object"):
-                    continue
-                token_path = token_oid.rel_path
-                token_list.append(token_path)
-            token_list.sort()
+        if self.verify_acl("view:role"):
+            lines.append('ROLES="%s"' % ",".join(role_list))
         else:
-            token_list = [""]
+            lines.append('ROLES=""')
 
-        access_group = ""
-        if self.verify_acl("view:accessgroup") \
-        or self.verify_acl("edit:accessgroup"):
-            access_group = str(self.access_group)
-        lines.append('ACCESS_GROUP="%s"' % access_group)
-
-        addresses = ""
-        if self.verify_acl("view:address") \
-        or self.verify_acl("add:address") \
-        or self.verify_acl("remove:address"):
-            addresses = ",".join(self.addresses)
-        lines.append('ADDRESSES="%s"' % addresses)
-
-        secret = ""
-        if self.verify_acl("view_all:secret"):
-            secret = str(self.secret)
-        lines.append('SECRET="%s"' % secret)
 
-        lines.append('TOKENS="%s"' % token_list)
+        if self.verify_acl("view:accessgroup"):
+            lines.append('ACCESS_GROUPS="%s"' % ",".join(self.get_access_groups()))
+        else:
+            lines.append('ACCESS_GROUPS=""')
+
+        if self.verify_acl("view:group"):
+            lines.append('GROUPS="%s"' % ",".join(self.get_groups()))
+        else:
+            lines.append('GROUPS=""')
 
-        return super(Client, self).show_config(config_lines=lines,
-                                        callback=callback, **kwargs)
+        if self.verify_acl("view:token"):
+            lines.append('TOKENS="%s"' % ",".join(token_list))
+        else:
+            lines.append('TOKENS=""')
+
+        token_options = {}
+        for uuid in self.token_options:
+            if uuid in x_list:
+                token_path = x_list[uuid]['rel_path']
+            else:
+                token_path = uuid
+            token_options[token_path] = self.token_options[uuid]
+        lines.append('TOKEN_OPTIONS="%s"' % token_options)
+
+        return OTPmeObject.show_config(self,
+                                    config_lines=lines,
+                                    callback=callback,
+                                    **kwargs)
 
     def show(self, **kwargs):
-        """ Show client details. """
+        """ Show role details. """
         #if not self.verify_acl("view_public:object"):
         #    msg = ("Permission denied.")
         #    return callback.error(msg, exception=PermissionDenied)
         return self.show_config(**kwargs)
```

### Comparing `otpme-0.3.0a78/otpme/lib/classes/command_handler.py` & `otpme-0.3.0a79/otpme/lib/classes/command_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -880,15 +880,14 @@
                 print(msg)
                 x_oc = x_restore_order[x_oid]['object_config']
                 try:
                     backend.write_config(object_id=x_oid,
                                         object_config=x_oc,
                                         full_index_update=True,
                                         full_data_update=True,
-                                        index_auto_update=False,
                                         encrypt=False)
                 except Exception as e:
                     msg = "Failed to restore object: %s: %s" % (x_oid, e)
                     print(msg)
                     failed_restores.append(msg)
         msg = "Creating DB indexes..."
         print(msg)
```

### Comparing `otpme-0.3.0a78/otpme/lib/classes/conn_handler.py` & `otpme-0.3.0a79/otpme/lib/classes/conn_handler.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/classes/data_objects/__init__.py` & `otpme-0.3.0a79/otpme/lib/classes/data_objects/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 	'otpme.lib.classes.data_objects.failed_pass',
 	'otpme.lib.classes.data_objects.last_assigned_id',
 	'otpme.lib.classes.data_objects.revoked_signature',
 	'otpme.lib.classes.data_objects.token_counter',
 	'otpme.lib.classes.data_objects.data_revision',
 	'otpme.lib.classes.data_objects.used_hash',
 	'otpme.lib.classes.data_objects.used_otp',
-	'otpme.lib.classes.data_objects.used_slp',
 	'otpme.lib.classes.data_objects.used_sotp',
 	'otpme.lib.classes.data_objects.rsa_key',
 	'otpme.lib.classes.data_objects.cert',
     ]
 
 def register():
     """ Register object modules. """
```

### Comparing `otpme-0.3.0a78/otpme/lib/classes/data_objects/cert.py` & `otpme-0.3.0a79/otpme/lib/classes/data_objects/cert.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/classes/data_objects/data_revision.py` & `otpme-0.3.0a79/otpme/lib/classes/data_objects/data_revision.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/classes/data_objects/failed_pass.py` & `otpme-0.3.0a79/otpme/lib/classes/data_objects/failed_pass.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/classes/data_objects/last_assigned_id.py` & `otpme-0.3.0a79/otpme/lib/classes/data_objects/last_assigned_id.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/classes/data_objects/revoked_signature.py` & `otpme-0.3.0a79/otpme/lib/classes/data_objects/revoked_signature.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/classes/data_objects/rsa_key.py` & `otpme-0.3.0a79/otpme/lib/classes/data_objects/rsa_key.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/classes/data_objects/skip_sync.py` & `otpme-0.3.0a79/otpme/lib/classes/data_objects/skip_sync.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/classes/data_objects/token_counter.py` & `otpme-0.3.0a79/otpme/lib/classes/data_objects/token_counter.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/classes/data_objects/used_hash.py` & `otpme-0.3.0a79/otpme/lib/classes/data_objects/used_hash.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/classes/data_objects/used_otp.py` & `otpme-0.3.0a79/otpme/lib/classes/data_objects/used_otp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/classes/data_objects/used_sotp.py` & `otpme-0.3.0a79/otpme/lib/classes/data_objects/used_sotp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/classes/dictionary.py` & `otpme-0.3.0a79/otpme/lib/classes/dictionary.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/classes/group.py` & `otpme-0.3.0a79/otpme/lib/classes/group.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/classes/host.py` & `otpme-0.3.0a79/otpme/lib/classes/host.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/classes/login_handler.py` & `otpme-0.3.0a79/otpme/lib/classes/login_handler.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/classes/mgmt_client.py` & `otpme-0.3.0a79/otpme/lib/classes/mgmt_client.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/classes/node.py` & `otpme-0.3.0a79/otpme/lib/classes/node.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/classes/object_config.py` & `otpme-0.3.0a79/otpme/lib/classes/object_config.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/classes/otpme_agent.py` & `otpme-0.3.0a79/otpme/lib/classes/otpme_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -614,20 +614,17 @@
 
         if update_status:
             # Get new RSP from update message.
             new_rsp = auth_conn.new_rsp
             rsp_hash = otpme_pass.gen_one_iter_hash(login_user, new_rsp)
             # Gen SRP.
             new_srp = srp.gen(rsp_hash)
-            # Gen SLP.
-            new_slp = slp.gen(rsp_hash)
             # Update session auth data.
             session['rsp'] = new_rsp
             session['srp'] = new_srp
-            session['slp'] = new_slp
             # Update timestamps.
             session['next_reneg'] = None
             session['next_retry'] = None
             session['last_reneg'] = time.time()
             session['last_failed_reneg'] = None
             # If this session is from the current system user
             # we can try to update the login session file.
```

### Comparing `otpme-0.3.0a78/otpme/lib/classes/otpme_host.py` & `otpme-0.3.0a79/otpme/lib/classes/otpme_host.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/classes/otpme_object.py` & `otpme-0.3.0a79/otpme/lib/classes/otpme_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -787,25 +787,21 @@
         self.realm = None
         self.realm_uuid = None
         self.cert = None
         self._cert_oid = None
         self._cert_public_key_oid = None
         self.key = None
         self._key_oid = None
-        #self.private_key = None
         self._private_key_oid = None
         self.public_key = None
         self._public_key_oid = None
         self.pickable = True
         self.cache_expire = 30
         self.sub_type = None
-        #self.index = []
         self.index_journal = []
-        self.index_journal_id = None
-        #self.index_journal_archive = {}
         self.incremental_updates = []
         self.list_attributes = []
         self.dict_attributes = []
         self.template_name = None
         self.template_object = False
         self.handle_key_loading = False
         self.handle_cert_loading = False
@@ -1736,19 +1732,18 @@
                 msg = ("Object misses name: %s" % self.oid)
                 raise OTPmeException(msg)
 
         if update_last_modified:
             # Update last modified timestamp.
             self.update_last_modified()
 
-        # Add in index journal to archive.
+        # Process index journal.
         index_journal = []
         if self.index_journal:
             index_journal = copy.deepcopy(self.index_journal)
-            self.add_index_journal(self.index_journal)
         self.index_journal = []
 
         # Update object config from variables.
         self.update_object_config()
 
         # Add incremental update stuff.
         self.object_config['INDEX_JOURNAL'] = index_journal
@@ -1778,15 +1773,14 @@
             raise BackendUnavailable("Backend not available.")
 
         # Try to write object config to backend.
         try:
             write_method(object_id=self.oid,
                         instance=self,
                         cluster=cluster,
-                        index_auto_update=False,
                         no_transaction=self.no_transaction,
                         index_journal=index_journal)
         except Exception as e:
             config.raise_exception()
             msg = (_("Error writing config for %s '%s': %s")
                     % (self.type, self.oid, e))
             if config.daemon_mode:
@@ -1796,43 +1790,14 @@
                 logger.critical(msg)
                 return callback.error(msg, raise_exception=False)
             else:
                 return callback.error(msg)
 
         return callback.ok()
 
-    def add_index_journal(self, journal):
-        """ Add index journal and remove outdated entries. """
-        # Get current time.
-        now = time.time()
-        # Make sure we do not use the same timestamp for different entries.
-        if self.index_journal_id is not None:
-            if self.index_journal_id == str(now):
-                now += 1
-        # Gen ID for journal entry.
-        self.index_journal_id = str(now)
-        # Save journal entry.
-        journal_entry = {
-                        'time'  : now,
-                        'data'  : list(journal),
-                        }
-        self.index_journal_archive[self.index_journal_id] = journal_entry
-
-        # Remove outdated journal entries.
-        counter = 0
-        x_sort = lambda x: float(x)
-        for x in sorted(self.index_journal_archive, key=x_sort, reverse=True):
-            counter += 1
-            # Compare values as float() because json dict keys are always strings.
-            if float(x) >= float(self.index_journal_id):
-                continue
-            if counter < config.index_journal_max:
-                continue
-            self.index_journal_archive.pop(x)
-
     def update_index(self, key, value, **kwargs):
         """ Update attribute in object index. """
         self.del_index(key)
         self.add_index(key, value, **kwargs)
 
     def add_index(self, key, value):
         """ Add attribute to object index. """
@@ -1990,16 +1955,14 @@
                             "UUID",
                             "REALM",
                             "SITE",
                             "UNIT",
                             "NAME",
                             "TYPE",
                             "INDEX",
-                            "INDEX_JOURNAL_ID",
-                            "INDEX_JOURNAL_ARCHIVE",
                             "ENABLED",
                             "LDIF",
                             "LDIF_ATTRIBUTES",
                             "EXTENSION_ATTRIBUTES",
                             "POLICIES",
                             "POLICY_OPTIONS",
                             "CONFIG_PARAMS",
@@ -2021,16 +1984,14 @@
                             "REALM",
                             "SITE",
                             "UNIT",
                             "NAME",
                             "TYPE",
                             "CERT",
                             "INDEX",
-                            "INDEX_JOURNAL_ID",
-                            "INDEX_JOURNAL_ARCHIVE",
                             "TEMPLATE_INDEX",
                             "LDIF",
                             "LDIF_ATTRIBUTES",
                             "EXTENSION_ATTRIBUTES",
                             "ENABLED",
                             "UNUSED_DISABLE",
                             "AUTO_DISABLE",
@@ -2591,24 +2552,14 @@
                                             'required'      : True,
                                         },
             'INDEX'                     : {
                                             'var_name'      : 'index',
                                             'type'          : list,
                                             'required'      : False,
                                         },
-            'INDEX_JOURNAL_ID'          : {
-                                            'var_name'      : 'index_journal_id',
-                                            'type'          : str,
-                                            'required'      : False,
-                                        },
-            'INDEX_JOURNAL_ARCHIVE'     : {
-                                            'var_name'      : 'index_journal_archive',
-                                            'type'          : dict,
-                                            'required'      : False,
-                                        },
             'ORIGIN'                    : {
                                             'var_name'      : 'origin',
                                             'type'          : 'uuid',
                                             'required'      : False,
                                         },
             'ORIGIN_CACHE'              : {
                                             'var_name'      : 'origin_cache',
@@ -7958,32 +7909,28 @@
                     'node'  : {
                         'trusted'  : [
                             "UUID",
                             "REALM",
                             "SITE",
                             "TYPE",
                             "INDEX",
-                            "INDEX_JOURNAL_ID",
-                            "INDEX_JOURNAL_ARCHIVE",
                             "CHECKSUM",
                             "SYNC_CHECKSUM",
                             "SALT",
                             "CREATE_TIME",
                             "LAST_MODIFIED",
                             ],
                         },
                     'host'  : {
                         'trusted'  : [
                             "UUID",
                             "REALM",
                             "SITE",
                             "TYPE",
                             "INDEX",
-                            "INDEX_JOURNAL_ID",
-                            "INDEX_JOURNAL_ARCHIVE",
                             "CHECKSUM",
                             "SYNC_CHECKSUM",
                             "SALT",
                             "CREATE_TIME",
                             "LAST_MODIFIED",
                             ],
                         },
@@ -8106,24 +8053,14 @@
                                         },
 
             'INDEX'                     : {
                                             'var_name'      : 'index',
                                             'type'          : list,
                                             'required'      : False,
                                         },
-            'INDEX_JOURNAL_ID'          : {
-                                            'var_name'      : 'index_journal_id',
-                                            'type'          : str,
-                                            'required'      : False,
-                                        },
-            'INDEX_JOURNAL_ARCHIVE'     : {
-                                            'var_name'      : 'index_journal_archive',
-                                            'type'          : dict,
-                                            'required'      : False,
-                                        },
             'CREATE_TIME'               : {
                                             'var_name'      : 'create_time',
                                             'type'          : int,
                                             'required'      : True,
                                         },
 
             'LAST_MODIFIED'             : {
```

### Comparing `otpme-0.3.0a78/otpme/lib/classes/policy.py` & `otpme-0.3.0a79/otpme/lib/classes/policy.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/classes/realm.py` & `otpme-0.3.0a79/otpme/lib/classes/realm.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/classes/resolver.py` & `otpme-0.3.0a79/otpme/lib/classes/resolver.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/classes/role.py` & `otpme-0.3.0a79/otpme/lib/classes/client.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,62 +6,89 @@
     if os.environ['OTPME_DEBUG_MODULE_LOADING'] == "True":
         print(_("Loading module: %s" % __name__))
 except:
     pass
 
 from otpme.lib import oid
 from otpme.lib import cli
+from otpme.lib import stuff
 from otpme.lib import config
 from otpme.lib import backend
+from otpme.lib import otpme_acl
 from otpme.lib.locking import object_lock
 from otpme.lib.otpme_acl import check_acls
-from otpme.lib.register import register_module
-from otpme.lib.cache import assigned_role_cache
-from otpme.lib.cache import assigned_token_cache
-from otpme.lib.classes.otpme_object import OTPmeObject
 from otpme.lib.protocols.utils import register_commands
+from otpme.lib.daemon.clusterd import cluster_radius_reload
+from otpme.lib.classes.otpme_object import OTPmeClientObject
 from otpme.lib.classes.otpme_object import run_pre_post_add_policies
 
 from otpme.lib.classes.otpme_object import \
     get_acls as _get_acls
 from otpme.lib.classes.otpme_object import \
     get_value_acls as _get_value_acls
 from otpme.lib.classes.otpme_object import \
     get_default_acls as _get_default_acls
 from otpme.lib.classes.otpme_object import \
     get_recursive_default_acls as _get_recursive_default_acls
 
 from otpme.lib.exceptions import *
 
-logger = config.logger
-
 default_callback = config.get_callback()
 
-read_acls = []
-write_acls = []
+read_acls =  []
 
-read_value_acls = {
-                    "view"      : [ "user", "token", "accessgroup", "group", "policy", "role" ],
+write_acls =  [
+                "limit_logins",
+                "unlimit_logins",
+            ]
+
+read_value_acls =    {
+                    "view"      : [
+                                "token",
+                                "group",
+                                "accessgroup",
+                                "secret",
+                                "login_url",
+                                "sso_enabled",
+                                "helper_url",
+                                "address",
+                                ],
             }
 
 write_value_acls = {
-                    "add"       : [ "user", "token", "role" ],
-                    "remove"    : [ "user", "token", "role" ],
-            }
+                    "add"       : [
+                                "address",
+                                ],
+                    "delete"    : [
+                                "address",
+                                ],
+                    "enable"    : [
+                                "sso",
+                                ],
+                    "disable"   : [
+                                "sso",
+                                ],
+                    "edit"      : [
+                                "accessgroup",
+                                "secret",
+                                "login_url",
+                                "helper_url",
+                                ],
+                }
 
 default_acls = []
-
 recursive_default_acls = []
 
 commands = {
     'add'   : {
             'OTPme-mgmt-1.0'    : {
                 'missing'    : {
                     'method'            : 'add',
-                    'oargs'             : ['unit'],
+                    'args'              : [],
+                    'oargs'             : ['address', 'unit'],
                     'job_type'          : 'process',
                     },
                 'exists'    : {
                     'method'            : 'add',
                     'job_type'          : 'process',
                     },
                 },
@@ -73,58 +100,54 @@
                     'job_type'          : 'process',
                     },
                 },
             },
     'show'   : {
             'OTPme-mgmt-1.0'    : {
                 'missing'    : {
-                    'method'            : cli.show_getter("role"),
+                    'method'            : cli.show_getter("client"),
                     'args'              : ['realm'],
                     'oargs'              : [
                                         'max_len',
                                         'show_all',
                                         'output_fields',
+                                        'max_policies',
                                         'search_regex',
                                         'sort_by',
                                         'reverse',
                                         'header',
                                         'csv',
                                         'csv_sep',
                                         'realm',
                                         'site',
-                                        'max_roles',
-                                        'max_tokens',
-                                        'max_ags',
-                                        'max_groups',
-                                        'max_policies',
                                         ],
                     'job_type'          : 'thread',
                     },
                 'exists'    : {
                     'method'            : 'show',
                     'args'              : ['realm'],
                     'job_type'          : 'thread',
                     },
                 },
             },
     'list'   : {
             'OTPme-mgmt-1.0'    : {
                 'missing'    : {
-                    'method'            : cli.list_getter("role"),
+                    'method'            : cli.list_getter("client"),
                     'oargs'              : [
                                         'reverse',
                                         'show_all',
                                         'attribute',
                                         'search_regex',
                                         'sort_by',
                                         ],
                     'job_type'          : None,
                     },
                 'exists'    : {
-                    'method'            : cli.list_getter("role"),
+                    'method'            : cli.list_getter("client"),
                     'oargs'              : [
                                         'reverse',
                                         'show_all',
                                         'attribute',
                                         'search_regex',
                                         'sort_by',
                                         ],
@@ -187,109 +210,146 @@
             'OTPme-mgmt-1.0'    : {
                 'exists'    : {
                     'method'            : 'disable_acl_inheritance',
                     'job_type'          : 'process',
                     },
                 },
             },
-    'add_token'   : {
+    'secret'   : {
             'OTPme-mgmt-1.0'    : {
                 'exists'    : {
-                    'method'            : 'add_token',
-                    'args'              : ['token_path'],
-                    'oargs'             : ['token_options', 'login_interfaces', 'sign', 'tags'],
+                    'method'            : 'change_secret',
+                    'oargs'             : ['auto_secret', 'secret'],
                     'job_type'          : 'process',
                     },
                 },
             },
-    'remove_token'   : {
+    'show_secret'   : {
             'OTPme-mgmt-1.0'    : {
                 'exists'    : {
-                    'method'            : 'remove_token',
-                    'args'              : ['token_path'],
-                    'oargs'             : ['keep_sign'],
+                    'method'            : 'show_secret',
                     'job_type'          : 'process',
                     },
                 },
             },
-    'add_role'   : {
+    'enable_sso'   : {
             'OTPme-mgmt-1.0'    : {
                 'exists'    : {
-                    'method'            : 'add_role',
-                    'args'              : ['role_name'],
+                    'method'            : 'enable_sso',
+                    'job_type'          : 'thread',
+                    },
+                },
+            },
+    'disable_sso'   : {
+            'OTPme-mgmt-1.0'    : {
+                'exists'    : {
+                    'method'            : 'disable_sso',
+                    'job_type'          : 'thread',
+                    },
+                },
+            },
+    'login_url'   : {
+            'OTPme-mgmt-1.0'    : {
+                'exists'    : {
+                    'method'            : 'change_login_url',
+                    'oargs'             : ['login_url'],
                     'job_type'          : 'process',
                     },
                 },
             },
-    'remove_role'   : {
+    'helper_url'   : {
             'OTPme-mgmt-1.0'    : {
                 'exists'    : {
-                    'method'            : 'remove_role',
-                    'args'              : ['role_name'],
+                    'method'            : 'change_helper_url',
+                    'oargs'             : ['helper_url'],
                     'job_type'          : 'process',
                     },
                 },
             },
-    'add_sync_user'   : {
+    'access_group'   : {
             'OTPme-mgmt-1.0'    : {
                 'exists'    : {
-                    'method'            : 'add_sync_user',
-                    'args'              : ['user_name'],
+                    'method'            : 'change_access_group',
+                    'args'              : ['access_group'],
                     'job_type'          : 'process',
                     },
                 },
             },
-    'remove_sync_user'   : {
+    'add_address'   : {
             'OTPme-mgmt-1.0'    : {
                 'exists'    : {
-                    'method'            : 'remove_sync_user',
-                    'args'              : ['user_name'],
+                    'method'            : 'add_address',
+                    'args'              : ['address'],
                     'job_type'          : 'process',
                     },
                 },
             },
-    'list_sync_users'   : {
+    'del_address'   : {
             'OTPme-mgmt-1.0'    : {
                 'exists'    : {
-                    'method'            : 'get_sync_users',
-                    'oargs'             : ['return_type'],
-                    'dargs'             : {'return_type':'name'},
+                    'method'            : 'del_address',
+                    'args'              : ['address'],
+                    'job_type'          : 'process',
+                    },
+                },
+            },
+    'add_role'   : {
+            'OTPme-mgmt-1.0'    : {
+                'exists'    : {
+                    'method'            : 'add_role',
+                    'args'              : ['role_name'],
                     'job_type'          : 'thread',
                     },
                 },
             },
-    'list_users'   : {
+    'remove_role'   : {
             'OTPme-mgmt-1.0'    : {
                 'exists'    : {
-                    'method'            : 'get_token_users',
-                    'oargs'             : ['return_type'],
-                    'dargs'             : {'return_type':'name'},
+                    'method'            : 'remove_role',
+                    'args'              : ['role_name'],
                     'job_type'          : 'thread',
                     },
                 },
             },
-    'list_tokens'   : {
+    'add_token'   : {
             'OTPme-mgmt-1.0'    : {
                 'exists'    : {
-                    'method'            : 'get_tokens',
-                    'oargs'             : ['return_type', 'token_types'],
-                    'dargs'             : {'return_type':'rel_path', 'skip_disabled':False},
+                    'method'            : 'add_token',
+                    'args'              : ['token_path'],
+                    'oargs'             : ['token_options', 'login_interfaces', 'sign', 'tags'],
                     'job_type'          : 'process',
                     },
                 },
             },
-    'list_roles'   : {
+    'remove_token'   : {
             'OTPme-mgmt-1.0'    : {
                 'exists'    : {
-                    'method'            : 'get_roles',
-                    'oargs'             : ['recursive'],
+                    'method'            : 'remove_token',
+                    'args'              : ['token_path'],
+                    'oargs'             : ['keep_sign'],
                     'job_type'          : 'process',
                     },
                 },
             },
+    'limit_logins'   : {
+            'OTPme-mgmt-1.0'    : {
+                'exists'    : {
+                    'method'            : 'limit_logins',
+                    'job_type'          : 'thread',
+                    },
+                },
+            },
+    'unlimit_logins'   : {
+            'OTPme-mgmt-1.0'    : {
+                'exists'    : {
+                    'method'            : 'unlimit_logins',
+                    'job_type'          : 'thread',
+                    },
+                },
+            },
     'list_policies'   : {
             'OTPme-mgmt-1.0'    : {
                 'exists'    : {
                     'method'            : 'get_policies',
                     'job_type'          : 'process',
                     'oargs'             : ['return_type', 'policy_types'],
                     'dargs'             : {'return_type':'name', 'ignore_hooks':True},
@@ -451,23 +511,14 @@
             'OTPme-mgmt-1.0'    : {
                 'exists'    : {
                     'method'            : 'get_object_classes',
                     'job_type'          : 'thread',
                     },
                 },
             },
-    'show_ldif'   : {
-            'OTPme-mgmt-1.0'    : {
-                'exists'    : {
-                    'method'            : 'get_ldif',
-                    'args'              : ['attributes'],
-                    'job_type'          : 'thread',
-                    },
-                },
-            },
     'show_acls'   : {
             'OTPme-mgmt-1.0'    : {
                 'exists'    : {
                     'method'            : 'get_acls',
                     'job_type'          : 'thread',
                     },
                 },
@@ -517,259 +568,176 @@
 
 def get_default_acls(**kwargs):
     return _get_default_acls(default_acls, **kwargs)
 
 def get_recursive_default_acls(**kwargs):
     return _get_recursive_default_acls(recursive_default_acls, **kwargs)
 
-DEFAULT_UNIT = "roles"
-
+DEFAULT_UNIT = "clients"
 REGISTER_BEFORE = []
 REGISTER_AFTER = [
                 "otpme.lib.classes.unit",
+                "otpme.lib.classes.group",
                 ]
 
 def register():
-    register_dn()
     register_oid()
     register_hooks()
     register_backend()
     register_object_unit()
     register_sync_settings()
-    register_commands("role", commands)
-    register_module("otpme.lib.classes.token")
-
-def register_dn():
-    """ Register DN attribute. """
-    config.register_dn_attribute("role", "cn")
+    register_commands("client", commands)
+    # Register index attributes.
+    config.register_index_attribute("address")
+    config.register_index_attribute("sso_enabled")
 
 def register_hooks():
-    config.register_auth_on_action_hook("role", "add")
-    config.register_auth_on_action_hook("role", "delete")
-    config.register_auth_on_action_hook("role", "add_role")
-    config.register_auth_on_action_hook("role", "remove_role")
-    config.register_auth_on_action_hook("role", "add_token")
-    config.register_auth_on_action_hook("role", "remove_token")
+    config.register_auth_on_action_hook("client", "add_token")
+    config.register_auth_on_action_hook("client", "remove_token")
+    config.register_auth_on_action_hook("client", "add_address")
+    config.register_auth_on_action_hook("client", "del_address")
+    config.register_auth_on_action_hook("client", "change_secret")
+    config.register_auth_on_action_hook("client", "change_login_url")
+    config.register_auth_on_action_hook("client", "enable_sso")
+    config.register_auth_on_action_hook("client", "disable_sso")
+    config.register_auth_on_action_hook("client", "change_helper_url")
+    config.register_auth_on_action_hook("client", "change_access_group")
+    config.register_auth_on_action_hook("client", "show_secret")
+    config.register_auth_on_action_hook("client", "limit_logins")
+    config.register_auth_on_action_hook("client", "unlimit_logins")
 
 def register_object_unit():
     """ Register default unit for this object type. """
-    config.register_default_unit("role", DEFAULT_UNIT)
+    config.register_default_unit("client", DEFAULT_UNIT)
     config.register_base_object("unit", DEFAULT_UNIT)
 
 def register_oid():
     full_oid_schema = [ 'realm', 'site', 'unit', 'name' ]
     read_oid_schema = [ 'realm', 'site', 'name' ]
     # OID regex stuff.
     unit_path_re = oid.object_regex['unit']['path']
-    role_name_re = '([0-9A-Za-z]([0-9A-Za-z_:.-]*[0-9A-Za-z]){0,})'
-    role_path_re = '%s[/]%s' % (unit_path_re, role_name_re)
-    role_oid_re = 'role|%s' % role_path_re
-    oid.register_oid_schema(object_type="role",
+    client_name_re = '([0-9A-Za-z]([0-9A-Za-z_.-]*[0-9A-Za-z]){0,})'
+    client_path_re = '%s[/]%s' % (unit_path_re, client_name_re)
+    client_oid_re = 'client|%s' % client_path_re
+    oid.register_oid_schema(object_type="client",
                             full_schema=full_oid_schema,
                             read_schema=read_oid_schema,
-                            name_regex=role_name_re,
-                            path_regex=role_path_re,
-                            oid_regex=role_oid_re)
+                            name_regex=client_name_re,
+                            path_regex=client_path_re,
+                            oid_regex=client_oid_re)
     rel_path_getter = lambda x: x[2:]
-    oid.register_rel_path_getter(object_type="role",
+    oid.register_rel_path_getter(object_type="client",
                                 getter=rel_path_getter)
 
 def register_backend():
     """ Register object for the file backend. """
-    role_dir_extension = "role"
-    def path_getter(role_oid):
-        return backend.config_path_getter(role_oid, role_dir_extension)
+    client_dir_extension = "client"
+    def path_getter(client_oid):
+        return backend.config_path_getter(client_oid, client_dir_extension)
     def index_rebuild(objects):
         after = [
                 'realm',
                 'site',
                 'unit',
                 'group',
                 'ca',
                 'node',
                 'host',
                 'user',
                 'token',
                 'accessgroup',
-                'client',
                 ]
-        return backend.rebuild_object_index("role", objects, after)
+        return backend.rebuild_object_index("client", objects, after)
     # Register object to config.
-    config.register_object_type(object_type="role",
+    config.register_object_type(object_type="client",
                             tree_object=True,
                             uniq_name=True,
-                            add_after=["token"],
-                            sync_before=["token", "user"],
+                            add_after=["host"],
+                            sync_after=["user", "token"],
                             object_cache=1024,
                             cache_region="tree_object",
                             backup_attributes=['realm', 'site', 'name'])
+    # Register index attributes.
+    config.register_index_attribute('accessgroup')
     # Register object to backend.
-    class_getter = lambda: Role
-    backend.register_object_type(object_type="role",
-                                dir_name_extension=role_dir_extension,
+    class_getter = lambda: Client
+    backend.register_object_type(object_type="client",
+                                dir_name_extension=client_dir_extension,
                                 class_getter=class_getter,
                                 index_rebuild_func=index_rebuild,
                                 path_getter=path_getter)
 
 def register_sync_settings():
     """ Register sync settings. """
-    config.register_object_sync(host_type="node", object_type="role")
-    config.register_object_sync(host_type="host", object_type="role")
-
-def get_roles(role_uuid=None, skip_disabled=False, parent=False,
-    recursive=True, return_type="name", return_attributes=None):
-
-    def _get_roles(uuid, parent=False, return_attributes=None):
-        return_attrs = ['name', 'enabled', 'full_oid', 'site']
-        if return_attributes is not None:
-            return_attrs = list(set(return_attrs + return_attributes))
-        if parent:
-            result = backend.search(object_type="role",
-                                    attribute="role",
-                                    value=uuid,
-                                    return_attributes=return_attrs)
-        else:
-            child_roles = backend.search(object_type="role",
-                                        attribute="uuid",
-                                        value=uuid,
-                                        return_attributes=['role'])
-            result = []
-            if child_roles:
-                result = backend.search(object_type="role",
-                                        attribute="uuid",
-                                        values=child_roles,
-                                        return_attributes=return_attrs)
-        return result
-
-    result = []
-    processed_roles = []
-    # Get roles roles.
-    check_roles = _get_roles(uuid=role_uuid,
-                            parent=parent,
-                            return_attributes=return_attributes)
-    if not check_roles:
-        return result
-    oid_result = backend.search(object_type="role",
-                            attribute="uuid",
-                            value=role_uuid,
-                            return_type="oid")
-    role_oid = oid_result[0]
-    role_site = role_oid.site
-
-    loop_found = False
-    role_uuid_list = []
-    while True:
-        for uuid in list(check_roles):
-            x_role_data = check_roles.pop(uuid)
-            if uuid == role_uuid:
-                continue
-            # Get role data.
-            x_name = x_role_data['name']
-            x_site = x_role_data['site']
-            x_full_oid = x_role_data['full_oid']
-            x_enabled = x_role_data['enabled'][0]
-            if uuid in role_uuid_list:
-                continue
-            if skip_disabled:
-                if not x_enabled:
-                    continue
-            role_uuid_list.append(uuid)
-            if return_attributes:
-                result.append(x_role_data)
-            elif return_type == "instance":
-                role = backend.get_object(object_type="role", uuid=uuid)
-                result.append(role)
-            elif return_type == "uuid":
-                result.append(uuid)
-            elif return_type == "full_oid":
-                result.append(x_full_oid)
-            elif return_type == "name":
-                if x_site == role_site:
-                    role_name = x_name
-                else:
-                    role_name = "%s/%s" % (x_site, x_name)
-                result.append(role_name)
-            else:
-                msg = (_("Unknown return type: %s") % return_type)
-                raise OTPmeException(msg)
-            if uuid in processed_roles:
-                loop_found = True
-                continue
-            processed_roles.append(uuid)
-            # Gets role roles.
-            _result = _get_roles(uuid=uuid, parent=parent,
-                            return_attributes=return_attributes)
-            for x in _result:
-                check_roles[x] = _result[x]
-        if not recursive:
-            break
-        if not check_roles:
-            break
-        if loop_found:
-            break
-    if not return_attributes:
-        result = sorted(result)
-    return result
+    config.register_object_sync(host_type="node", object_type="client")
 
-class Role(OTPmeObject):
-    """ Role object """
+class Client(OTPmeClientObject):
+    """ Creates client object """
     commands = commands
-    def __init__(self, object_id=None, path=None, name=None,
-        unit=None, site=None, realm=None, **kwargs):
-        # Set our type (used in parent class)
-        self.type = "role"
+    def __init__(self, object_id=None, name=None, realm=None,
+        unit=None, site=None, path=None, access_group=None, **kwargs):
+        # Set our type (used in parent class).
+        self.type = "client"
 
         # Call parent class init.
-        super(Role, self).__init__(object_id=object_id,
+        super(Client, self).__init__(object_id=object_id,
                                         realm=realm,
                                         site=site,
                                         unit=unit,
                                         name=name,
                                         path=path,
                                         **kwargs)
         self._acls = get_acls()
         self._value_acls = get_value_acls()
         self._default_acls = get_default_acls()
         self._recursive_default_acls = get_recursive_default_acls()
 
-        # Roles should not inherit ACLs by default.
+        self.access_group = None
+        self.access_group_uuid = None
+        if access_group:
+            self.change_access_group(access_group=access_group,
+                                    verify_acls=False)
+
+        self.secret = None
+        self.secret_len = 32
+        # Clients should not inherit ACLs by default.
         self.acl_inheritance_enabled = False
+        self.logins_limited = False
+        self.radius_reload = False
+        self.sso_enabled = False
+        self.login_url = None
+        self.helper_url = None
 
         self._sync_fields = {
-                    'host'  : {
-                        'trusted'  : [
-                            "EXTENSIONS",
-                            "OBJECT_CLASSES",
-                            "TOKENS",
-                            "ROLES",
-                            "SYNC_USERS",
-                            ]
-                        },
-
                     'node'  : {
                         'untrusted'  : [
                             "EXTENSIONS",
                             "OBJECT_CLASSES",
+                            "EXTENSION_ATTRIBUTES",
                             "TOKENS",
-                            "ROLES",
-                            "SYNC_USERS",
                             ]
                         },
                     }
 
     def _get_object_config(self):
         """ Get object config dict. """
         object_config = {
-                        'SYNC_USERS'                : {
-                                                        'var_name'  : 'sync_users',
+                        'ADDRESSES'                 : {
+                                                        'var_name'  : 'addresses',
                                                         'type'      : list,
                                                         'required'  : False,
                                                     },
 
-                        'ROLES'                    : {
+                        'ACCESS_GROUP'              : {
+                                                        'var_name'  : 'access_group_uuid',
+                                                        'type'      : 'uuid',
+                                                        'required'  : False,
+                                                    },
+
+                        'ROLES'                     : {
                                                         'var_name'  : 'roles',
                                                         'type'      : list,
                                                         'required'  : False,
                                                     },
 
                         'TOKENS'                    : {
                                                         'var_name'  : 'tokens',
@@ -778,237 +746,271 @@
                                                     },
 
                         'TOKEN_OPTIONS'             : {
                                                         'var_name'  : 'token_options',
                                                         'type'      : dict,
                                                         'required'  : False,
                                                     },
+
                         'TOKEN_LOGIN_INTERFACES'    : {
                                                         'var_name'  : 'token_login_interfaces',
                                                         'type'      : dict,
                                                         'required'  : False,
                                                     },
+                        'SECRET'                    : {
+                                                        'var_name'  : 'secret',
+                                                        'type'      : str,
+                                                        'required'  : False,
+                                                        'encryption': config.disk_encryption,
+                                                    },
+                        'SSO_ENABLED'               : {
+                                                        'var_name'  : 'sso_enabled',
+                                                        'type'      : bool,
+                                                        'required'  : False,
+                                                    },
+                        'LOGIN_URL'                 : {
+                                                        'var_name'  : 'login_url',
+                                                        'type'      : str,
+                                                        'required'  : False,
+                                                    },
+                        'HELPER_URL'                : {
+                                                        'var_name'  : 'helper_url',
+                                                        'type'      : str,
+                                                        'required'  : False,
+                                                    },
             }
 
-        return object_config
+        return super(Client, self)._get_object_config(object_config=object_config)
 
     def set_variables(self):
-        """ Set instance variables """
+        """ Set instance variables. """
+        if self.access_group_uuid:
+            ag = backend.get_object(object_type="accessgroup",
+                                    uuid=self.access_group_uuid,
+                                    realm=self.realm,
+                                    site=self.site)
+            if ag:
+                self.access_group = ag.name
         # Set OID.
         self.set_oid()
 
     def _set_name(self, name):
         """ Set object name. """
         # Make sure name is a string.
         name = str(name)
-        # Only base roles must have uppercase names.
-        base_roles = config.get_base_objects("role")
-        if name.upper() in base_roles:
+        # Only base clients must have uppercase names.
+        base_clients = config.get_base_objects("client")
+        if name.upper() in base_clients:
             self.name = name.upper()
         else:
             self.name = name.lower()
 
-    @assigned_token_cache.cache_method()
-    def is_assigned_token(self, token_uuid, check_parent_roles=True,
-        skip_disabled_roles=True, processed_roles=[]):
-        if token_uuid in self.tokens:
-            return True
-        if not check_parent_roles:
-            return False
-        child_roles = self.get_roles(return_type="instance",
-                            skip_disabled=skip_disabled_roles,
-                            recursive=False)
-        for role in child_roles:
-            if skip_disabled_roles:
-                if not role.enabled:
-                    continue
-            if role.uuid in processed_roles:
-                continue
-            processed_roles.append(role.uuid)
-            if role.is_assigned_token(token_uuid):
-                return True
-        return False
-
-    @assigned_role_cache.cache_method()
-    def is_assigned_role(self, role_uuid, check_parent_roles=True,
-        skip_disabled_roles=True, processed_roles=[]):
-        if role_uuid in self.roles:
-            return True
-        if not check_parent_roles:
-            return False
-        parent_roles = self.get_roles(parent=True,
-                            return_type="instance",
-                            skip_disabled=skip_disabled_roles,
-                            recursive=False)
-        for role in parent_roles:
-            if skip_disabled_roles:
-                if not role.enabled:
-                    continue
-            if role.uuid in processed_roles:
-                continue
-            processed_roles.append(role.uuid)
-            if role.is_assigned_role(role_uuid, processed_roles=processed_roles):
-                return True
-        return False
-
-    @cli.check_rapi_opts()
-    def get_roles(self, return_type="name", parent=False,
-        skip_disabled=False, recursive=False, _caller="API",
-        callback=default_callback, **kwargs):
-        """ Get all roles of this role. """
-        result = get_roles(role_uuid=self.uuid,
-                            parent=parent,
-                            return_type=return_type,
-                            skip_disabled=skip_disabled,
-                            recursive=recursive)
-        if _caller == "API":
+    def _write(self, **kwargs):
+        """ Wrapper to make sure radius gets reloaded. """
+        result = super(Client, self)._write(**kwargs)
+        if not self.radius_reload:
             return result
-        if _caller == "RAPI":
-            result = ",".join(result)
-        if _caller == "CLIENT":
-            result = "\n".join(result)
-        return callback.ok(result)
+        self.radius_reload = False
+        cluster_radius_reload()
+        return result
 
-    @cli.check_rapi_opts()
-    def get_access_groups(self, return_type="name", _caller="API",
-        callback=default_callback, **kwargs):
-        """ Return list with all access group names this role is in. """
-        result = backend.search(realm=self.realm,
-                            site=self.site,
-                            attribute="role",
-                            value=self.uuid,
-                            object_type="accessgroup",
-                            return_type=return_type)
-        if _caller == "RAPI":
-            result = ",".join(result)
-        if _caller == "CLIENT":
-            result = "\n".join(result)
-        return callback.ok(result)
+    # xxxxxxxxxxxxxxxxxxx
+    # FIXME: check if IP is valid!!!
+    @object_lock()
+    @check_acls(['add:address'])
+    def add_address(self, address, run_policies=True,
+        callback=default_callback, _caller="API", **kwargs):
+        """ Adds a address to this client. """
+        if address in self.addresses:
+            return callback.error(_("Address '%s' already added to this client.")
+                                    % address)
+        if run_policies:
+            try:
+                self.run_policies("modify",
+                                callback=callback,
+                                _caller=_caller)
+                self.run_policies("add_address",
+                                callback=callback,
+                                _caller=_caller)
+            except Exception as e:
+                return callback.error()
+        self.addresses.append(address)
+        # Update index.
+        self.add_index("address", address)
+        # Make sure radius gets reloaded
+        self.radius_reload = True
+        return self._cache(callback=callback)
 
-    @cli.check_rapi_opts()
-    def get_groups(self, return_type="uuid", _caller="API",
-        callback=default_callback, **kwargs):
-        """ Return list with all group names this role is in. """
-        result = backend.search(realm=self.realm,
-                            site=self.site,
-                            attribute="role",
-                            value=self.uuid,
-                            object_type="group",
-                            return_type=return_type)
-        if _caller == "RAPI":
-            result = ",".join(result)
-        if _caller == "CLIENT":
-            result = "\n".join(result)
-        return callback.ok(result)
+    @object_lock()
+    @check_acls(['delete:address'])
+    def del_address(self, address, run_policies=True,
+        callback=default_callback, _caller="API", **kwargs):
+        """ Deletes a address from this client. """
+        if not address in self.addresses:
+            return callback.error(_("Address '%s' is not an address of this client.")
+                                    % address)
+        if run_policies:
+            try:
+                self.run_policies("modify",
+                                callback=callback,
+                                _caller=_caller)
+                self.run_policies("del_address",
+                                callback=callback,
+                                _caller=_caller)
+            except Exception as e:
+                return callback.error()
+        self.addresses.remove(address)
+        # Update index.
+        self.del_index("address", address)
+        # Make sure radius gets reloaded
+        self.radius_reload = True
+        return self._cache(callback=callback)
 
-    @object_lock(full_lock=True)
-    @backend.transaction
-    def rename(self, new_name, callback=default_callback, _caller="API", **kwargs):
-        """ Rename role. """
-        base_roles = config.get_base_objects("role")
-        if self.name in base_roles:
-            return callback.error("Cannot rename base role.")
-        # Build new OID.
-        new_oid = oid.get(object_type="role",
-                        realm=self.realm,
-                        site=self.site,
-                        unit=self.unit,
-                        name=new_name)
-        return self._rename(new_oid, callback=callback, _caller=_caller, **kwargs)
+    @object_lock()
+    @check_acls(['edit:accessgroup'])
+    def change_access_group(self, access_group=None,
+        run_policies=True, callback=default_callback,
+        _caller="API", **kwargs):
+        """ Change client access group. """
+        from otpme.lib.classes.accessgroup import AccessGroup
+        if access_group == self.access_group:
+            return callback.error(_("Group '%s' is already access group of "
+                                    "this client.") % access_group)
+        if run_policies:
+            try:
+                self.run_policies("modify",
+                                callback=callback,
+                                _caller=_caller)
+                self.run_policies("change_access_group",
+                                callback=callback,
+                                _caller=_caller)
+            except Exception as e:
+                return callback.error()
+        if access_group:
+            # Create access group instance.
+            g = AccessGroup(name=access_group,
+                            realm=self.realm,
+                            site=self.site)
+            if not g.exists():
+                return callback.error(_("Group '%s' does not exist.")
+                                        % self.access_group_uuid)
+            # Append access group UUID to access groups.
+            self.access_group_uuid = g.uuid
+            self.access_group = g.name
+            # Update Index.
+            self.update_index('accessgroup', self.access_group_uuid)
+        else:
+            self.access_group_uuid = None
+            self.access_group = None
+            # Update Index.
+            self.del_index('accessgroup')
 
-    @object_lock(full_lock=True)
-    @backend.transaction
-    @run_pre_post_add_policies()
-    def add(self, verbose_level=0, callback=default_callback, **kwargs):
-        """ Add a role. """
-        # Run parent class stuff e.g. verify ACLs.
-        result = self._prepare_add(callback=callback, **kwargs)
-        if result is False:
-            return callback.error()
-        # Add object using parent class.
-        return OTPmeObject.add(self, verbose_level=verbose_level,
-                                callback=callback, **kwargs)
+        return self._cache(callback=callback)
 
-    @object_lock(full_lock=True)
-    @backend.transaction
-    def delete(self, force=False, run_policies=True,
-        verify_acls=True, verbose_level=0, _caller="API",
+    @check_acls(['enable:sso'])
+    @object_lock()
+    def enable_sso(self, run_policies=True, _caller="API",
         callback=default_callback, **kwargs):
-        """ Delete role. """
-        if not self.exists():
-            return callback.error("Role does not exist exists.")
+        """ Enable SSO portal app. """
+        if self.sso_enabled:
+            msg = (_("SSO already enabled."))
+            return callback.error(msg)
+
+        if not self.login_url:
+            msg = "Login URL not configured."
+            return callback.error(msg)
+
+        if not self.helper_url:
+            msg = "Helper URL not configured."
+            return callback.error(msg)
 
-        base_roles = config.get_base_objects("role")
-        if self.name in base_roles:
-            return callback.error("Cannot delete base role.")
+        if run_policies:
+            try:
+                self.run_policies("modify",
+                                callback=callback,
+                                _caller=_caller)
+                self.run_policies("enable_sso",
+                                callback=callback,
+                                _caller=_caller)
+            except Exception as e:
+                return callback.error()
 
-        # Get parent object to check ACLs.
-        parent_object = self.get_parent_object()
-        if verify_acls:
-            if not self.verify_acl("delete:object"):
-                del_acl = "delete:%s" % self.type
-                if not parent_object.verify_acl(del_acl):
-                    msg = (_("Permission denied: %s") % self.name)
-                    return callback.error(msg, exception=PermissionDenied)
+        self.sso_enabled = True
+        self.update_index("sso_enabled", self.sso_enabled)
+
+        return self._write(callback=callback)
+
+    @check_acls(['disable:sso'])
+    @object_lock()
+    def disable_sso(self, run_policies=True, _caller="API",
+        callback=default_callback, **kwargs):
+        """ Disable SSO portal app. """
+        if self.sso_disabled:
+            msg = (_("SSO already disabled."))
+            return callback.error(msg)
 
         if run_policies:
             try:
-                self.run_policies("delete", callback=callback, _caller=_caller)
+                self.run_policies("modify",
+                                callback=callback,
+                                _caller=_caller)
+                self.run_policies("disable_sso",
+                                callback=callback,
+                                _caller=_caller)
             except Exception as e:
                 return callback.error()
 
-        if not force:
-            exception = ""
-            # List that will hold all tokens that uses this role.
-            token_list = []
-            # Get all tokens from this role.
-            for t_uuid in self.tokens:
-                token = backend.get_object(object_type="token", uuid=t_uuid)
-                if token:
-                    token_list.append(token.rel_path)
-                else:
-                    token_list.append(t_uuid)
+        self.sso_enabled = False
+        self.update_index("sso_enabled", self.sso_enabled)
 
-            if token_list:
-                exception = (_("%sRole has member tokens: %s\n")
-                            % (exception, ", ".join(token_list)))
+        return self._write(callback=callback)
 
-            # List that will hold all groups that uses this role.
-            accessgroup_list = self.get_access_groups()
+    @object_lock()
+    @check_acls(acls=['edit:login_url'])
+    def change_login_url(self, login_url=False, run_policies=True,
+        callback=default_callback, _caller="API", **kwargs):
+        """ Change object login_url """
+        if run_policies:
+            try:
+                self.run_policies("modify",
+                                callback=callback,
+                                _caller=_caller)
+                self.run_policies("change_login_url",
+                                callback=callback,
+                                _caller=_caller)
+            except Exception as e:
+                msg = str(e)
+                return callback.error(msg)
 
-            if accessgroup_list:
-                exception = (_("%sRole is member of this access groups: %s\n")
-                            % (exception, ", ".join(accessgroup_list)))
-
-            if exception != "":
-                if self.confirmation_policy != "force":
-                    if self.confirmation_policy == "paranoid":
-                        answer = callback.ask(_("%sPlease type '%s' to delete object: ")
-                                            % (exception, self.name))
-                        if answer != self.name:
-                            return callback.abort()
-                    else:
-                        answer = callback.ask(_("%sDelete role '%s'?: ")
-                                            % (exception, self.name))
-                        if answer.lower() != "y":
-                            return callback.abort()
-            else:
-                if self.confirmation_policy != "force":
-                    if self.confirmation_policy == "paranoid":
-                        answer = callback.ask(_("Please type '%s' to delete object: ") % self.name)
-                        if answer != self.name:
-                            return callback.abort()
-                    else:
-                        answer = callback.ask(_("Delete role '%s'?: ") % self.name)
-                        if answer.lower() != "y":
-                            return callback.abort()
+        # Set new login_url.
+        self.login_url = login_url
 
-        # Delete object using parent class.
-        return OTPmeObject.delete(self, verbose_level=verbose_level,
-                                    force=force, callback=callback)
+        return self._cache(callback=callback)
+
+    @object_lock()
+    @check_acls(acls=['edit:helper_url'])
+    def change_helper_url(self, helper_url=False, run_policies=True,
+        callback=default_callback, _caller="API", **kwargs):
+        """ Change object helper_url """
+        if run_policies:
+            try:
+                self.run_policies("modify",
+                                callback=callback,
+                                _caller=_caller)
+                self.run_policies("change_helper_url",
+                                callback=callback,
+                                _caller=_caller)
+            except Exception as e:
+                msg = str(e)
+                return callback.error(msg)
+
+        # Set new helper_url.
+        self.helper_url = helper_url
+
+        return self._cache(callback=callback)
 
     @check_acls(['remove:orphans'])
     @object_lock()
     def remove_orphans(self, force=False, run_policies=True,
         verbose_level=0, callback=default_callback,
         _caller="API", **kwargs):
         """ Remove orphan UUIDs. """
@@ -1018,15 +1020,14 @@
                                 callback=callback,
                                 _caller=_caller)
                 self.run_policies("remove_orphans",
                                 callback=callback,
                                 _caller=_caller)
             except Exception as e:
                 return callback.error()
-
         acl_list = self.get_orphan_acls()
         policy_list = self.get_orphan_policies()
 
         token_list = []
         token_uuids = set(self.tokens + list(self.token_options))
         for i in token_uuids:
             token_oid = backend.get_oid(object_type="token", uuid=i)
@@ -1045,132 +1046,203 @@
                     msg = (_("%s%s|%s: Found the following orphan policies: %s\n")
                             % (msg, self.type, self.name, ",".join(policy_list)))
 
             if token_list:
                 msg = (_("%s%s|%s: Found the following orphan token UUIDs: %s\n")
                         % (msg, self.type, self.name, ",".join(token_list)))
 
-            if msg:
-                answer = callback.ask("%sRemove?: " % msg)
-                if answer.lower() != "y":
-                    return callback.abort()
-
         object_changed = False
         if acl_list:
             if self.remove_orphan_acls(force=True, verbose_level=verbose_level,
-                                        callback=callback, **kwargs):
+                                                callback=callback, **kwargs):
                 object_changed = True
 
         if policy_list:
             if self.remove_orphan_policies(force=True, verbose_level=verbose_level,
                                                 callback=callback, **kwargs):
                 object_changed = True
 
         for i in token_list:
             if verbose_level > 0:
-                callback.send(_("Removing orphan token UUID: %s") % i)
+                callback.send(_("Removing orphan token UUID: %s" % i))
             object_changed = True
-            try:
+            if i in self.tokens:
                 self.tokens.remove(i)
-            except KeyError:
-                pass
-            try:
+            if i in self.token_options:
                 self.token_options.pop(i)
-            except KeyError:
-                pass
-            try:
-                self.token_login_interfaces.pop(i)
-            except KeyError:
-                pass
 
         if not object_changed:
             msg = None
             if verbose_level > 0:
                 msg = (_("No orphan objects found for %s: %s")
                         % (self.type, self.name))
             return callback.ok(msg)
 
         return self._cache(callback=callback)
 
-    def show_config(self, callback=default_callback, **kwargs):
-        """ Show role config. """
-        if not self.verify_acl("view_public:object"):
-            msg = ("Permission denied.")
-            return callback.error(msg, exception=PermissionDenied)
+    @object_lock(full_lock=True)
+    def rename(self, new_name, callback=default_callback, _caller="API", **kwargs):
+        """ Rename client. """
+        base_clients = config.get_base_objects("client")
+        if self.name in base_clients:
+            return callback.error("Cannot rename base client.")
 
-        token_list = []
-        if self.tokens:
-            if self.verify_acl("view:token."):
-                return_attrs = ['rel_path']
-                token_list = backend.search(object_type="token",
-                                            join_object_type="role",
-                                            join_search_attr="uuid",
-                                            join_search_val=self.uuid,
-                                            join_attribute="token",
-                                            attribute="uuid",
-                                            value="*",
-                                            return_attributes=return_attrs)
-            token_list.sort()
+        # Build new OID.
+        new_oid = oid.get(object_type="client",
+                        realm=self.realm,
+                        site=self.site,
+                        unit=self.unit,
+                        name=new_name)
+        result = self._rename(new_oid, callback=callback, _caller=_caller, **kwargs)
+        # Make sure radius gets reloaded
+        self.radius_reload = True
+        return result
 
-        role_list = []
-        if self.roles:
-            if self.verify_acl("view:role."):
-                return_attrs = ['site', 'name']
-                roles_result = backend.search(object_type="role",
-                                            join_object_type="role",
-                                            join_search_attr="uuid",
-                                            join_search_val=self.uuid,
-                                            join_attribute="role",
-                                            attribute="uuid",
-                                            value="*",
-                                            return_attributes=return_attrs)
-                for x in roles_result:
-                    role_site = roles_result[x]['site']
-                    role_name = roles_result[x]['name']
-                    if role_site != config.site:
-                        role_name = "%s/%s" % (role_site, role_name)
-                    role_list.append(role_name)
-            role_list.sort()
+    @object_lock(full_lock=True)
+    @run_pre_post_add_policies()
+    def add(self, address=None, verbose_level=0, callback=default_callback, **kwargs):
+        """ Add a client. """
+        if address:
+            result = backend.search(object_type="client",
+                                    attribute="address",
+                                    value=address,
+                                    return_type="name")
+            if result:
+                existing_client = result[0]
+                msg = "Client with this address already exists: %s" % existing_client
+                return callback.error(msg)
 
-        lines = []
+        # Run parent class stuff e.g. verify ACLs.
+        result = self._prepare_add(callback=callback, **kwargs)
+        if result is False:
+            return callback.error()
+        self.secret = stuff.gen_secret(32)
+        # Add object using parent class.
+        add_result = super(Client, self).add(verbose_level=verbose_level,
+                                            callback=callback, **kwargs)
+        if not add_result:
+            msg = "Failed to add client."
+            return callback.error(msg)
+
+        if address:
+            self.add_address(address)
+            msg = "Radius secret: %s" % self.secret
+            callback.send(msg)
+        # Make sure radius gets reloaded
+        self.radius_reload = True
+        return callback.ok()
 
-        if self.verify_acl("view:role"):
-            lines.append('ROLES="%s"' % ",".join(role_list))
-        else:
-            lines.append('ROLES=""')
+    @object_lock(full_lock=True)
+    def delete(self, force=False, run_policies=True, verify_acls=True,
+        verbose_level=0, callback=default_callback, _caller="API", **kwargs):
+        """ Delete client. """
+        if not self.exists():
+            return callback.error("Client does not exist exists.")
 
+        base_clients = config.get_base_objects("client")
+        if self.name in base_clients:
+            return callback.error("Cannot delete base client.")
 
-        if self.verify_acl("view:accessgroup"):
-            lines.append('ACCESS_GROUPS="%s"' % ",".join(self.get_access_groups()))
-        else:
-            lines.append('ACCESS_GROUPS=""')
+        # Get parent object to check ACLs.
+        parent_object = self.get_parent_object()
+        if verify_acls:
+            if not self.verify_acl("delete:object"):
+                del_acl = "delete:%s" % self.type
+                if not parent_object.verify_acl(del_acl):
+                    msg = (_("Permission denied: %s") % self.name)
+                    return callback.error(msg, exception=PermissionDenied)
 
-        if self.verify_acl("view:group"):
-            lines.append('GROUPS="%s"' % ",".join(self.get_groups()))
-        else:
-            lines.append('GROUPS=""')
+        if run_policies:
+            try:
+                self.run_policies("delete", callback=callback, _caller=_caller)
+            except Exception as e:
+                return callback.error()
 
-        if self.verify_acl("view:token"):
-            lines.append('TOKENS="%s"' % ",".join(token_list))
+        if not force:
+            if self.confirmation_policy == "paranoid":
+                msg = "Please type '%s' to delete object: " % self.name
+                answer = callback.ask(msg)
+                if answer != self.name:
+                    return callback.abort()
+            else:
+                answer = callback.ask(_("Delete client '%s'?: ") % self.name)
+                if answer.lower() != "y":
+                    return callback.abort()
+
+        # Delete object using parent class.
+        result = super(Client, self).delete(verbose_level=verbose_level,
+                                        force=force, callback=callback)
+        # Make sure radius gets reloaded.
+        cluster_radius_reload()
+        return result
+
+    def show_config(self, callback=default_callback, **kwargs):
+        """ Show client config. """
+        if not self.verify_acl("view_public:object"):
+            msg = ("Permission denied.")
+            return callback.error(msg, exception=PermissionDenied)
+
+        lines = []
+
+        if self.verify_acl("view:token") \
+        or self.verify_acl("add:token") \
+        or self.verify_acl("remove:token"):
+            token_list = []
+            for i in self.tokens:
+                token_oid = backend.get_oid(i, instance=True)
+                # Add UUIDs of orphan tokens.
+                if not token_oid:
+                    token_list.append(i)
+                    continue
+                if not otpme_acl.access_granted(object_id=token_oid,
+                                                acl="view_public:object"):
+                    continue
+                token_path = token_oid.rel_path
+                token_list.append(token_path)
+            token_list.sort()
         else:
-            lines.append('TOKENS=""')
+            token_list = [""]
 
-        token_options = {}
-        for uuid in self.token_options:
-            if uuid in x_list:
-                token_path = x_list[uuid]['rel_path']
-            else:
-                token_path = uuid
-            token_options[token_path] = self.token_options[uuid]
-        lines.append('TOKEN_OPTIONS="%s"' % token_options)
-
-        return OTPmeObject.show_config(self,
-                                    config_lines=lines,
-                                    callback=callback,
-                                    **kwargs)
+        access_group = ""
+        if self.verify_acl("view:accessgroup") \
+        or self.verify_acl("edit:accessgroup"):
+            access_group = str(self.access_group)
+        lines.append('ACCESS_GROUP="%s"' % access_group)
+
+        addresses = ""
+        if self.verify_acl("view:address") \
+        or self.verify_acl("add:address") \
+        or self.verify_acl("remove:address"):
+            addresses = ",".join(self.addresses)
+        lines.append('ADDRESSES="%s"' % addresses)
+
+        secret = ""
+        if self.verify_acl("view_all:secret"):
+            secret = str(self.secret)
+        lines.append('SECRET="%s"' % secret)
+
+        lines.append('TOKENS="%s"' % token_list)
+
+        sso_enabled = ""
+        if self.verify_acl("view:sso_enabled"):
+            sso_enabled = self.sso_enabled
+        lines.append('SSO_ENABLED="%s"' % sso_enabled)
+
+        login_url = ""
+        if self.verify_acl("view:login_url"):
+            login_url = self.login_url
+        lines.append('LOGIN_URL="%s"' % login_url)
+
+        helper_url = ""
+        if self.verify_acl("view:helper_url"):
+            helper_url = self.helper_url
+        lines.append('LOGIN_URL="%s"' % helper_url)
+
+        return super(Client, self).show_config(config_lines=lines,
+                                        callback=callback, **kwargs)
 
     def show(self, **kwargs):
-        """ Show role details. """
+        """ Show client details. """
         #if not self.verify_acl("view_public:object"):
         #    msg = ("Permission denied.")
         #    return callback.error(msg, exception=PermissionDenied)
         return self.show_config(**kwargs)
```

### Comparing `otpme-0.3.0a78/otpme/lib/classes/script.py` & `otpme-0.3.0a79/otpme/lib/classes/script.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/classes/session.py` & `otpme-0.3.0a79/otpme/lib/classes/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,14 @@
     if os.environ['OTPME_DEBUG_MODULE_LOADING'] == "True":
         print(_("Loading module: %s" % __name__))
 except:
     pass
 
 from otpme.lib import cli
 from otpme.lib import srp
-from otpme.lib import slp
 from otpme.lib import oid
 from otpme.lib import json
 from otpme.lib import sotp
 from otpme.lib import stuff
 from otpme.lib import config
 from otpme.lib import backend
 from otpme.lib import filetools
@@ -178,26 +177,27 @@
                                 path_getter=path_getter)
 
 class Session(OTPmeLockObject):
     """ OTPme session object. """
     def __init__(self, session_type=None, username=None, access_group=None,
         object_id=None, object_config=None, uuid=None, cache=False,
         pass_hash=None, pass_hash_params=None, session_id=None, token=None,
-        client=None, client_ip=None):
+        client=None, client_ip=None, slp=None):
         """ Init. """
         super(Session, self).__init__()
         self.realm = config.realm
         self.site = config.site
         #if pass_hash is not None:
         #    if pass_hash_params is None:
         #        msg = "Need <pass_hash_params>."
         #        raise OTPmeException(msg)
         # Set password hash.
         self.pass_hash = pass_hash
         self.pass_hash_params = pass_hash_params
+        self.slp = slp
         # Stuff for session renegotiation.
         self.reneg_started = False
         self.last_reneg = False
         self.reneg_hash = None
         # Some default values.
         self.last_login = None
         self.login_count = 0
@@ -510,14 +510,16 @@
         self.object_config = ObjectConfig(self.oid)
 
         self.last_modified = time.time()
 
         # Make sure password hashes etc. get encrypted.
         self.object_config.add(key='PASS_HASH', value=self.pass_hash,
                                     encryption=config.disk_encryption)
+        self.object_config.add(key='SLP', value=self.slp,
+                                    encryption=config.disk_encryption)
         if self.offline_data_key:
             self.object_config.add(key='OFFLINE_DATA_KEY',
                                     value=self.offline_data_key,
                                     encryption=config.disk_encryption)
         self.object_config['PASS_HASH_PARAMS'] = self.pass_hash_params
         self.object_config['REALM'] = self.realm
         self.object_config['SITE'] = self.site
@@ -549,15 +551,15 @@
         self.object_config['OLD_CHECKSUM'] = self.old_checksum
 
         # Write session config.
         try:
             backend.write_config(object_id=self.oid,
                                 instance=self,
                                 cluster=True,
-                                index_auto_update=True)
+                                full_index_update=True)
         except Exception as e:
             msg = "Failed to write session: %s: %s" % (self.oid, e)
             logger.warning(msg)
             config.raise_exception()
             return False
 
         return True
@@ -576,14 +578,15 @@
             self.child_sessions = self.get_config_parameter('CHILD_SESSIONS').split(',')
 
         self.realm = self.get_config_parameter('REALM')
         self.site = self.get_config_parameter('SITE')
         self.creation_time = self.get_config_parameter('CREATION_TIME')
         self.user_uuid = self.get_config_parameter('USER_UUID')
         self.pass_hash = self.get_config_parameter('PASS_HASH')
+        self.slp = self.get_config_parameter('SLP')
         self.pass_hash_params = self.get_config_parameter('PASS_HASH_PARAMS')
         self.session_type = self.get_config_parameter('SESSION_TYPE')
         self.access_group_uuid = self.get_config_parameter('ACCESS_GROUP_UUID')
         self.client = self.get_config_parameter('CLIENT')
         self.client_ip = self.get_config_parameter('CLIENT_IP')
         self.auth_token = self.get_config_parameter('AUTH_TOKEN')
         self.last_login = self.get_config_parameter('LAST_LOGIN')
@@ -642,16 +645,19 @@
         self.last_used = time.time()
 
         if not update_child_sessions:
             return
 
         # Update child sessions.
         for session_id in self.child_sessions:
-            session = backend.get_sessions(session_id=session_id,
-                                        return_type="instance")[0]
+            result = backend.get_sessions(session_id=session_id,
+                                        return_type="instance")
+            if not result:
+                continue
+            session = result[0]
             if not session:
                 continue
             # FIXME: Do we need this? disabled groups would be still denied
             #        in User().authenticate(). does this check have a big performance impact?
             # Create group instance for this session to check if it is enabled.
             session_group = backend.get_object(object_type="accessgroup",
                                                 name=session.access_group,
@@ -769,15 +775,15 @@
             verify_status = verify_reply['status']
             if verify_status is not None:
                 return verify_reply
         return verify_reply
 
     def _verify(self, auth_type, session_hash, password=None,
         password_hash=None, challenge=None, response=None, check_sotp=False,
-        do_reneg=False, reneg_salt=None, rsp_hash_type=None,
+        do_reneg=False, reneg_salt=None, rsp_hash_type=None, auth_ag=None,
         check_auth=True, check_slp=True, check_srp=True):
         """ Verify given session hash via password or MSCHAP challenge/response. """
         # default should be None -> session does not match request
         verify_reply = {'status' : None}
 
         if auth_type == "clear-text":
             logger.debug("Doing clear-text session verification.")
@@ -893,47 +899,44 @@
                                     'status'    : True,
                                     'nt_key'    : nt_key,
                                     }
                     return verify_reply
 
         # Check for SLP.
         if check_slp:
-            # Build logout pass from session hash.
-            _slp = slp.gen(session_hash)
-
             if auth_type == "clear-text":
                 # Check if given password matches logout password of this
                 # session.
-                if _slp == password:
+                if self.slp == password:
                     verify_reply = {
                                     'type'      : 'logout',
                                     'status'    : True,
-                                    'slp'       : _slp,
+                                    'slp'       : self.slp,
                                     }
                     return verify_reply
 
             if auth_type == "mschap":
                 # Generate password hash of logout password of this session.
-                _slp_hash = stuff.gen_nt_hash(_slp)
+                _slp_hash = stuff.gen_nt_hash(self.slp)
                 # Try to verify challenge/response with logout password hash for
                 # this session.
                 try:
                     verify_status, nt_key = mschap_util.verify(_slp_hash,
                                                                 challenge,
                                                                 response)
                 except Exception as e:
                     verify_status = None
-                    msg = ("bError verifying MSCHAP request (SLP): %s: %s"
+                    msg = ("Error verifying MSCHAP request (SLP): %s: %s"
                             % (self.session_id, e))
                     logger.critical(msg)
                 if verify_status:
                     verify_reply = {
                                     'type'      : 'logout',
                                     'status'    : True,
-                                    'slp'       : _slp,
+                                    'slp'       : self.slp,
                                     'slp_hash'  : _slp_hash,
                                     'nt_key'    : nt_key,
                                     }
                     return verify_reply
 
         # Check for SRP.
         if check_srp:
@@ -974,17 +977,30 @@
                                     'nt_key'    : nt_key,
                                     }
                     return verify_reply
 
         # Check for SOTP.
         if check_sotp:
             if auth_type == "clear-text":
+                auth_ag_uuid = None
+                if auth_ag:
+                    # Get sotp auth accessgroup.
+                    result = backend.search(object_type="accessgroup",
+                                            attribute="name",
+                                            value=auth_ag,
+                                            return_type="uuid")
+                    if not result:
+                        msg = "Unknown accessgroup: %s" % auth_ag
+                        logger.critical(msg)
+                        return verify_reply
+                    auth_ag_uuid = result[0]
                 # Check if given password matches an SOTP of this session.
                 sotp_verify_status = sotp.verify(password_hash=session_hash,
-                                                password=password)
+                                                password=password,
+                                                access_group=auth_ag_uuid)
                 if sotp_verify_status:
                     verify_reply = {
                                     'type'      : 'reauth',
                                     'status'    : True,
                                     'sotp'     : password,
                                     }
                     return verify_reply
@@ -995,15 +1011,15 @@
                     nt_key, \
                     _sotp, \
                     _sotp_hash = sotp.verify(password_hash=session_hash,
                                                 challenge=challenge,
                                                 response=response)
                 except Exception as e:
                     verify_status = None
-                    msg = ("dError verifying MSCHAP request (SOTP): %s: %s"
+                    msg = ("Error verifying MSCHAP request (SOTP): %s: %s"
                             % (self.session_id, e))
                     logger.critical(msg)
 
                 if sotp_verify_status:
                     verify_reply = {
                                     'type'      : 'reauth',
                                     'status'    : True,
@@ -1090,14 +1106,15 @@
             if not child_group.enabled:
                 continue
 
             # Create child session instance for each child group.
             child_session = Session(self.session_type,
                                     self.username,
                                     pass_hash=self.pass_hash,
+                                    pass_hash_params=self.pass_hash_params,
                                     token=self.auth_token,
                                     access_group=c,
                                     client=client,
                                     client_ip=client_ip)
             # Add child session if it does not exist.
             if not child_session.exists():
                 logger.debug("Adding child session '%s'." % child_session.name)
```

### Comparing `otpme-0.3.0a78/otpme/lib/classes/signing.py` & `otpme-0.3.0a79/otpme/lib/classes/signing.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/classes/site.py` & `otpme-0.3.0a79/otpme/lib/classes/site.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,14 +59,16 @@
                                 "sync",
                                 "ca",
                                 "cert",
                                 "cert_key",
                                 "admin_role",
                                 "user_role",
                                 "admin_token",
+                                "sso_secret",
+                                "sso_csrf_secret",
                                 ],
         }
 
 write_value_acls = {
                     "add"       : [
                                 "unit",
                                 "trust",
@@ -85,14 +87,18 @@
                                 ],
                     "edit"      : [
                                 "address",
                                 "auth_fqdn",
                                 "mgmt_fqdn",
                                 "radius_cert",
                                 "radius_key",
+                                "sso_cert",
+                                "sso_key",
+                                "sso_secret",
+                                "sso_csrf_secret",
                                 ],
                     "renew"     : [
                                 "cert",
                                 ],
                     "revoke"    : [
                                 "cert",
                                 ],
@@ -507,14 +513,66 @@
             'OTPme-mgmt-1.0'    : {
                 'exists'    : {
                     'method'            : 'del_radius_key',
                     'job_type'          : 'process',
                     },
                 },
             },
+    'sso_cert'   : {
+            'OTPme-mgmt-1.0'    : {
+                'exists'    : {
+                    'method'            : 'change_sso_cert',
+                    'args'              : ['sso_cert'],
+                    'job_type'          : 'process',
+                    },
+                },
+            },
+    'sso_key'   : {
+            'OTPme-mgmt-1.0'    : {
+                'exists'    : {
+                    'method'            : 'change_sso_key',
+                    'args'              : ['sso_key'],
+                    'job_type'          : 'process',
+                    },
+                },
+            },
+    'del_sso_cert'   : {
+            'OTPme-mgmt-1.0'    : {
+                'exists'    : {
+                    'method'            : 'del_sso_cert',
+                    'job_type'          : 'process',
+                    },
+                },
+            },
+    'del_sso_key'   : {
+            'OTPme-mgmt-1.0'    : {
+                'exists'    : {
+                    'method'            : 'del_sso_key',
+                    'job_type'          : 'process',
+                    },
+                },
+            },
+    'sso_secret'   : {
+            'OTPme-mgmt-1.0'    : {
+                'exists'    : {
+                    'method'            : 'change_sso_secret',
+                    'args'              : ['secret'],
+                    'job_type'          : 'thread',
+                    },
+                },
+            },
+    'sso_csrf_secret'   : {
+            'OTPme-mgmt-1.0'    : {
+                'exists'    : {
+                    'method'            : 'change_sso_csrf_secret',
+                    'args'              : ['secret'],
+                    'job_type'          : 'thread',
+                    },
+                },
+            },
     'add_trust'   : {
             'OTPme-mgmt-1.0'    : {
                 'exists'    : {
                     'method'            : 'add_trust',
                     'args'              : ['site_name'],
                     'job_type'          : 'process',
                     },
@@ -676,14 +734,17 @@
     return _get_recursive_default_acls(recursive_default_acls, **kwargs)
 
 REGISTER_BEFORE = []
 REGISTER_AFTER = [
                 "otpme.lib.classes.realm",
                 ]
 
+SSO_CLIENT_NAME = "SSO"
+SSO_ACCESSGROUP = "SSO"
+
 TEMPLATES_UNIT = "templates"
 
 def register():
     register_dn()
     register_oid()
     register_hooks()
     register_config()
@@ -706,14 +767,22 @@
     """ Register DN attribute. """
     config.register_dn_attribute("site", "ou")
 
 def register_config():
     """ Register config stuff. """
     config.register_config_var("default_site_validity", int, 5475)
     config.register_config_var("default_site_key_len", int, 2048)
+    # Register SSO base client and accessgroup.
+    config.register_config_var("sso_client_name", str, SSO_CLIENT_NAME)
+    config.register_config_var("sso_access_group", str, SSO_ACCESSGROUP)
+    config.register_base_object("accessgroup",  SSO_ACCESSGROUP)
+    client_attrs = {'access_group':SSO_ACCESSGROUP}
+    config.register_base_object(object_type="client",
+                            name=config.sso_client_name,
+                            attributes=client_attrs)
 
 def register_hooks():
     config.register_auth_on_action_hook("site", "add_unit")
     config.register_auth_on_action_hook("site", "change_address")
     config.register_auth_on_action_hook("site", "change_auth_fqdn")
     config.register_auth_on_action_hook("site", "change_mgmt_fqdn")
     config.register_auth_on_action_hook("site", "enable_auth")
@@ -809,14 +878,18 @@
         self.handle_cert_loading = True
         self.handle_key_loading = True
         #self.handle_public_key_loading = True
         #self.handle_private_key_loading = True
         self.radius_cert = None
         self.radius_key = None
         self.radius_reload = False
+        self.sso_cert = None
+        self.sso_key = None
+        self.sso_secret = None
+        self.sso_csrf_secret = None
 
         self._acls = get_acls()
         self._value_acls = get_value_acls()
         self._default_acls = get_default_acls()
         self._recursive_default_acls = get_recursive_default_acls()
 
         self._sync_fields = {
@@ -960,14 +1033,40 @@
             'RADIUS_KEY'                : {
                                             'var_name'  : 'radius_key',
                                             'type'      : str,
                                             'required'  : False,
                                             'encryption'    : config.disk_encryption,
                                         },
 
+            'SSO_CERT'                  : {
+                                            'var_name'  : 'sso_cert',
+                                            'type'      : str,
+                                            'required'  : False,
+                                            'encoding'  : 'BASE64',
+                                        },
+
+            'SSO_KEY'                   : {
+                                            'var_name'  : 'sso_key',
+                                            'type'      : str,
+                                            'required'  : False,
+                                            'encryption'    : config.disk_encryption,
+                                        },
+
+            'SSO_SECRET'                : {
+                                            'var_name'  : 'sso_secret',
+                                            'type'      : str,
+                                            'required'  : False,
+                                            'encryption'    : config.disk_encryption,
+                                        },
+            'SSO_CSRF_SECRET'           : {
+                                            'var_name'  : 'sso_csrf_secret',
+                                            'type'      : str,
+                                            'required'  : False,
+                                            'encryption'    : config.disk_encryption,
+                                        },
             }
 
         return object_config
 
     def _set_name(self, name):
         """ Set object name. """
         # Make sure name is a string and lowercase.
@@ -1203,14 +1302,128 @@
             except Exception as e:
                 return callback.error()
         self.radius_key = None
         # Make sure radius gets reloaded.
         self.radius_reload = True
         return self._cache(callback=callback)
 
+    @check_acls(['edit:sso_cert'])
+    @object_lock()
+    @backend.transaction
+    def change_sso_cert(self, sso_cert, run_policies=True,
+        callback=default_callback, _caller="API", **kwargs):
+        """ Change sso cert. """
+        if run_policies:
+            try:
+                self.run_policies("modify",
+                                callback=callback,
+                                _caller=_caller)
+                self.run_policies("change_sso_cert",
+                                callback=callback,
+                                _caller=_caller)
+            except Exception as e:
+                return callback.error()
+        self.sso_cert = sso_cert
+        return self._cache(callback=callback)
+
+    @check_acls(['edit:sso_cert'])
+    @object_lock()
+    @backend.transaction
+    def del_sso_cert(self, run_policies=True,
+        callback=default_callback, _caller="API", **kwargs):
+        """ Delete sso cert. """
+        if run_policies:
+            try:
+                self.run_policies("modify",
+                                callback=callback,
+                                _caller=_caller)
+                self.run_policies("del_sso_cert",
+                                callback=callback,
+                                _caller=_caller)
+            except Exception as e:
+                return callback.error()
+        self.sso_cert = None
+        return self._cache(callback=callback)
+
+    @check_acls(['edit:sso_key'])
+    @object_lock()
+    @backend.transaction
+    def change_sso_key(self, sso_key, run_policies=True,
+        callback=default_callback, _caller="API", **kwargs):
+        """ Change sso cert. """
+        if run_policies:
+            try:
+                self.run_policies("modify",
+                                callback=callback,
+                                _caller=_caller)
+                self.run_policies("change_sso_key",
+                                callback=callback,
+                                _caller=_caller)
+            except Exception as e:
+                return callback.error()
+        self.sso_key = sso_key
+        return self._cache(callback=callback)
+
+    @check_acls(['edit:sso_cert'])
+    @object_lock()
+    @backend.transaction
+    def del_sso_key(self, run_policies=True,
+        callback=default_callback, _caller="API", **kwargs):
+        """ Delete sso key. """
+        if run_policies:
+            try:
+                self.run_policies("modify",
+                                callback=callback,
+                                _caller=_caller)
+                self.run_policies("del_sso_key",
+                                callback=callback,
+                                _caller=_caller)
+            except Exception as e:
+                return callback.error()
+        self.sso_key = None
+        return self._cache(callback=callback)
+
+    @check_acls(['edit:sso_secret'])
+    @object_lock()
+    @backend.transaction
+    def change_sso_secret(self, secret, run_policies=True,
+        callback=default_callback, _caller="API", **kwargs):
+        """ Change sso secret. """
+        if run_policies:
+            try:
+                self.run_policies("modify",
+                                callback=callback,
+                                _caller=_caller)
+                self.run_policies("change_sso_secret",
+                                callback=callback,
+                                _caller=_caller)
+            except Exception as e:
+                return callback.error()
+        self.sso_secret = secret
+        return self._cache(callback=callback)
+
+    @check_acls(['edit:sso_csrf_secret'])
+    @object_lock()
+    @backend.transaction
+    def change_sso_csrf_secret(self, secret, run_policies=True,
+        callback=default_callback, _caller="API", **kwargs):
+        """ Change sso CSRF secret. """
+        if run_policies:
+            try:
+                self.run_policies("modify",
+                                callback=callback,
+                                _caller=_caller)
+                self.run_policies("change_sso_csrf_secret",
+                                callback=callback,
+                                _caller=_caller)
+            except Exception as e:
+                return callback.error()
+        self.sso_csrf_secret = secret
+        return self._cache(callback=callback)
+
     @check_acls(['enable:auth'])
     @object_lock()
     @backend.transaction
     def enable_auth(self, force=False, run_policies=True,
         callback=default_callback, _caller="API", **kwargs):
         """ Enable authentication with the site. """
         if self.auth_enabled:
@@ -1830,14 +2043,18 @@
         # Set site FQDN.
         self.auth_fqdn = site_fqdn
         self.mgmt_fqdn = site_fqdn
 
         # Set site address.
         self.address = site_address
 
+        # Set flask secrets.
+        self.sso_secret = stuff.gen_secret(len=64, encoding="hex")
+        self.sso_csrf_secret = stuff.gen_secret(len=64, encoding="hex")
+
         # Set config site.
         config.set_site(name=self.name,
                         uuid=self.uuid,
                         address=self.address,
                         auth_fqdn=self.auth_fqdn,
                         mgmt_fqdn=self.mgmt_fqdn)
 
@@ -2115,14 +2332,23 @@
                 group.change_max_sessions(verify_acls=False,
                                         max_sessions=3,
                                         callback=callback)
                 # Set relogin timeout for REALM group to 1 second.
                 group.change_relogin_timeout(verify_acls=False,
                                             relogin_timeout="1m",
                                             callback=callback)
+            if group.name == config.sso_access_group:
+                # Set max sessions for SSO portal group to 3.
+                group.change_max_sessions(verify_acls=False,
+                                        max_sessions=3,
+                                        callback=callback)
+                # Set relogin timeout for SSO portal to 1 second.
+                group.change_relogin_timeout(verify_acls=False,
+                                            relogin_timeout="1m",
+                                            callback=callback)
             if group.name == config.ldap_access_group:
                 # Set max sessions for ldap (ldaptor) group to 3.
                 group.change_max_sessions(verify_acls=False,
                                         max_sessions=3,
                                         callback=callback)
                 # Set relogin timeout for ldap group to 1 second.
                 group.change_relogin_timeout(verify_acls=False,
@@ -2707,16 +2933,27 @@
 
         if self.verify_acl("view:address") \
         or self.verify_acl("edit:address"):
             lines.append('ADDRESS="%s"' % self.address)
         else:
             lines.append('ADDRESS=""')
 
+        if self.verify_acl("view:sso_secret") \
+        or self.verify_acl("edit:sso_secret"):
+            lines.append('SSO_SECRET="%s"' % self.sso_secret)
+        else:
+            lines.append('SSO_SECRET=""')
+
+        if self.verify_acl("view:sso_csrf_secret") \
+        or self.verify_acl("edit:sso_csrf_secret"):
+            lines.append('SSO_CSRF_SECRET="%s"' % self.sso_csrf_secret)
+        else:
+            lines.append('SSO_CSRF_SECRET=""')
+
         lines.append('CA="%s"' % site_ca)
-        lines.append('MASTER="%s"' % master_node)
 
         lines.append('ADMIN_ROLE="%s"' % admin_role)
         lines.append('USER_ROLE="%s"' % user_role)
         lines.append('ADMIN_TOKEN="%s"' % admin_token)
 
         return OTPmeObject.show_config(self,
                                     config_lines=lines,
```

### Comparing `otpme-0.3.0a78/otpme/lib/classes/ssh_agent.py` & `otpme-0.3.0a79/otpme/lib/classes/ssh_agent.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/classes/token.py` & `otpme-0.3.0a79/otpme/lib/classes/token.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/classes/unit.py` & `otpme-0.3.0a79/otpme/lib/classes/unit.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/classes/user.py` & `otpme-0.3.0a79/otpme/lib/classes/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 from otpme.lib.encryption.rsa import RSAKey
 from otpme.lib.register import register_module
 from otpme.lib.encryption import hash_password
 from otpme.lib.policy import one_time_policy_run
 from otpme.lib.otpme_acl import check_special_user
 from otpme.lib.classes.otpme_object import OTPmeObject
 from otpme.lib.protocols.utils import register_commands
-from otpme.lib.classes.data_objects.used_slp import UsedSLP
 from otpme.lib.classes.data_objects.used_sotp import UsedSOTP
 from otpme.lib.classes.data_objects.failed_pass import FailedPass
 from otpme.lib.classes.otpme_object import run_pre_post_add_policies
 
 from otpme.lib.classes.otpme_object import \
     get_acls as _get_acls
 from otpme.lib.classes.otpme_object import \
@@ -107,20 +106,22 @@
                                 "key_script",
                                 "auth_script",
                                 "agent_script",
                                 "login_script",
                                 "auto_disable",
                                 ],
                     "enable"    : [
+                                "disabled_login",
                                 "autosign",
                                 "auth_script",
                                 "login_script",
                                 "token"
                                 ],
                     "disable"   : [
+                                "disabled_login",
                                 "autosign",
                                 "auth_script",
                                 "login_script",
                                 "token",
                                 ],
         }
 
@@ -281,14 +282,30 @@
                 'exists'    : {
                     'method'            : 'change_group',
                     'args'              : ['new_group'],
                     'job_type'          : 'process',
                     },
                 },
             },
+    'enable_disabled_login'   : {
+            'OTPme-mgmt-1.0'    : {
+                'exists'    : {
+                    'method'            : 'enable_disabled_login',
+                    'job_type'          : 'thread',
+                    },
+                },
+            },
+    'disable_disabled_login'   : {
+            'OTPme-mgmt-1.0'    : {
+                'exists'    : {
+                    'method'            : 'disable_disabled_login',
+                    'job_type'          : 'thread',
+                    },
+                },
+            },
     'enable_autosign'   : {
             'OTPme-mgmt-1.0'    : {
                 'exists'    : {
                     'method'            : 'enable_autosign',
                     'job_type'          : 'process',
                     },
                 },
@@ -855,15 +872,14 @@
     register_user_scripts()
     register_sync_settings()
     register_shared_objects()
     register_config_properties()
     register_config_parameters()
     register_commands("user", commands)
     register_module("otpme.lib.classes.session")
-    register_module("otpme.lib.classes.data_objects.used_slp")
     register_module("otpme.lib.classes.data_objects.used_sotp")
     register_module("otpme.lib.classes.data_objects.failed_pass")
     register_module("otpme.lib.classes.data_objects.last_assigned_id")
     register_module("otpme.lib.classes.data_objects.revoked_signature")
     multiprocessing.register_shared_dict("otp_hashes")
 
 def register_template():
@@ -1204,14 +1220,16 @@
         self._acls = get_acls()
         self._value_acls = get_value_acls()
         self._default_acls = get_default_acls()
         self._recursive_default_acls = get_recursive_default_acls()
 
         # Users primary group cache.
         self._group_uuid = None
+        # Indicates that the user is allowed to login even if realm/site/accessgroup/unit is disabled.
+        self.allow_disabled_login = False
         # Users keys can be handled by the key script on client side or by this
         # class.
         self.sign_mode = "client"
         # Will hold users RSA private key or stuff needed to get it
         # via self.key_script.
         #self.private_key = {}
         # Will hold users RSA public key.
@@ -1222,14 +1240,16 @@
         self.key_script = None
         # The OTPmeScript used to start/stop users gpg/ssh-agent.
         self.agent_script = None
         # The OTPmeScript used as users login script.
         self.login_script = None
         self.login_script_enabled = False
         self.used_pass_salt = None
+        # SSO session data.
+        self.sso_session_data = {}
         self.auth_script = None
         self.auth_script_enabled = False
         self.acl_inheritance_enabled = False
         self.track_last_used = True
 
         # Users default token.
         self.default_token = None
@@ -1239,14 +1259,15 @@
                         'trusted'  : [
                             "TOKENS",
                             "PUBLIC_KEY",
                             "DEFAULT_TOKEN",
                             "EXTENSIONS",
                             "EXTENSION_ATTRIBUTES",
                             "AUTOSIGN_ENABLED",
+                            "ALLOW_DISABLED_LOGIN",
                             "OBJECT_CLASSES",
                             "homeDirectory",
                             "loginShell",
                             "uidNumber",
                             "givenName",
                             "sn",
                             ]
@@ -1256,14 +1277,15 @@
                         'untrusted'  : [
                             "TOKENS",
                             "PUBLIC_KEY",
                             "DEFAULT_TOKEN",
                             "EXTENSIONS",
                             "EXTENSION_ATTRIBUTES",
                             "AUTOSIGN_ENABLED",
+                            "ALLOW_DISABLED_LOGIN",
                             "OBJECT_CLASSES",
                             "USED_PASS_SALT",
                             "ACLS",
                             "ACL_INHERITANCE_ENABLED",
                             "homeDirectory",
                             "loginShell",
                             "uidNumber",
@@ -1284,14 +1306,19 @@
 
                         'DEFAULT_TOKEN'             : {
                                                         'var_name'  : 'default_token',
                                                         'type'      : 'uuid',
                                                         'required'  : False,
                                                     },
 
+                        'ALLOW_DISABLED_LOGIN'      : {
+                                                        'var_name'  : 'allow_disabled_login',
+                                                        'type'      : bool,
+                                                        'required'  : False,
+                                                    },
 
                         'SIGN_MODE'                 : {
                                                         'var_name'  : 'sign_mode',
                                                         'type'      : str,
                                                         'required'  : False,
                                                     },
 
@@ -1378,14 +1405,20 @@
 
                         'USED_PASS_SALT'            : {
                                                         'var_name'  : 'used_pass_salt',
                                                         'type'      : str,
                                                         'required'  : False,
                                                         'encryption': config.disk_encryption,
                                                     },
+                        'SSO_SESSION_DATA'          : {
+                                                        'var_name'  : 'sso_session_data',
+                                                        'type'      : dict,
+                                                        'required'  : False,
+                                                        'encryption': config.disk_encryption,
+                                                    },
                         }
 
         return object_config
 
     def set_variables(self):
         """ Set instance variables. """
         # Try to get site name.
@@ -1407,14 +1440,27 @@
             name = name_upper
         else:
             if name != name.lower():
                 msg = (_("Username must be lowercase."))
                 raise OTPmeException(msg)
         self.name = name
 
+    def get_id(self):
+        return self.uuid
+
+    @property
+    def is_active(self):
+        return self.enabled
+
+    @property
+    def is_authenticated(self):
+        if config.auth_token:
+            return True
+        return False
+
     @property
     def group(self):
         if not self.group_uuid:
             return
         group_oid = backend.get_oid(self.group_uuid, instance=True)
         if not group_oid:
             return
@@ -2698,48 +2744,40 @@
         if not isinstance(string, str):
             raise OTPmeException("Need string")
 
         x_hash = stuff.gen_md5(string + self.used_pass_salt)
 
         return x_hash
 
-    def _get_used(self, otype):
+    def _get_used_sotp(self):
         """ Get users used SOTP/SLP hashes. """
-        if otype == "sotp":
-            object_type = "used_sotp"
-        elif otype == "slp":
-            object_type = "used_slp"
-        else:
-            raise OTPmeException("Unknown type: %s" % otype)
-
-        used_objects = backend.search(object_type=object_type,
+        used_objects = backend.search(object_type="used_sotp",
                                     attribute="user_uuid",
                                     value=self.uuid,
                                     return_attributes=['uuid', 'expiry'])
         return used_objects
 
-    def is_used(self, otype, hash, challenge=None, response=None):
+    def is_used_sotp(self, hash, challenge=None, response=None):
         """
-        Check if given SOTP/SLP hash is already used and remove outdated hashes
+        Check if given SOTP hash is already used and remove outdated hashes
         from cache.
         """
         from otpme.lib import mschap_util
         # Indicates if SOTP/SLP was already used.
         was_used = False
 
         # Generate hash.
         _hash = self._gen_used_hash(hash)
 
-        _used = self._get_used(otype)
+        _used = self._get_used_sotp()
         for uuid in _used:
             used_expiry = _used[uuid]['expiry'][0]
             # Check if object has expired.
             if time.time() > used_expiry:
-                msg = ("Removing expired used %s from backend: %s"
-                        % (otype.upper(), self.name))
+                msg = ("Removing expired used SOTP from backend: %s" % self.name)
                 logger.debug(msg)
                 used_object = backend.get_object(uuid=uuid)
                 if not used_object:
                     continue
                 try:
                     used_object.delete(force=True)
                 except UnknownObject:
@@ -2770,49 +2808,41 @@
             else:
                 # Stop processing if we found an already used hash.
                 if _hash == otp_hash:
                     was_used = True
                     break
         return was_used
 
-    # FIXME: add proto to cluster this list!
-    def add_used(self, otype, hash):
-        """ Add SOTP/SLP hash to list of already used hashes for this user. """
-        if otype == "sotp":
-            object_class = UsedSOTP
-        elif otype == "slp":
-            object_class = UsedSLP
-        else:
-            raise OTPmeException("Unknown type: %s" % otype)
-
+    def add_used_sotp(self, hash):
+        """ Add SOTP hash to list of already used hashes for this user. """
         # Generate hash
         _hash = self._gen_used_hash(hash)
 
         # We want to cache used hashes 1h. We cache SLPs to prevent server
         # load when doing authentication and SOTPs to prevent re-usage of them.
         # For both 1h should be enough.
         # FIXME: make this a config file option???
         cache_time = 3600
         # Get epoch time.
         expiry_timestamp = time.time() + cache_time
 
-        used_object = object_class(user_uuid=self.uuid,
+        used_object = UsedSOTP(user_uuid=self.uuid,
                                 object_hash=_hash,
                                 expiry=expiry_timestamp,
                                 realm=config.realm,
                                 site=config.site,
                                 no_transaction=True)
         try:
             used_object.add()
         except AlreadyExists:
             pass
         except LockWaitAbort:
             pass
         except OTPmeException as e:
-            msg = "Failed to add used %s" % otype
+            msg = "Failed to add used SOTP."
             logger.warning(msg)
 
     def remove_outdated_failed_pass_hashes(self, access_group):
         """ Remove outdated failed pass hashes of this user. """
         # Get max fail for accessgroup.
         result = backend.search(object_type="accessgroup",
                                     realm=config.realm,
@@ -3347,14 +3377,54 @@
         except ValueError:
             pass
         # Update index.
         self.del_index('token', token.uuid)
 
         return self._cache(callback=callback)
 
+    @check_acls(['enable:disabled_login'])
+    @object_lock()
+    def enable_disabled_login(self, run_policies=True,
+        callback=default_callback, _caller="API", **kwargs):
+        """ Enable user disabled login. """
+        if run_policies:
+            try:
+                self.run_policies("modify",
+                                callback=callback,
+                                _caller=_caller)
+                self.run_policies("enable_disabled_login",
+                                callback=callback,
+                                _caller=_caller)
+            except Exception as e:
+                return callback.error()
+
+        self.allow_disabled_login = True
+
+        return self._cache(callback=callback)
+
+    @check_acls(['disable:disabled_login'])
+    @object_lock()
+    def disable_disabled_login(self, run_policies=True,
+        callback=default_callback, _caller="API", **kwargs):
+        """ Disable user disabled login. """
+        if run_policies:
+            try:
+                self.run_policies("modify",
+                                callback=callback,
+                                _caller=_caller)
+                self.run_policies("disable_disabled_login",
+                                callback=callback,
+                                _caller=_caller)
+            except Exception as e:
+                return callback.error()
+
+        self.allow_disabled_login = False
+
+        return self._cache(callback=callback)
+
     @check_acls(['enable:autosign'])
     @object_lock()
     def enable_autosign(self, run_policies=True,
         callback=default_callback, _caller="API", **kwargs):
         """ Enable user auto-sign feature. """
         if run_policies:
             try:
@@ -4199,25 +4269,24 @@
                                         **kwargs)
             if not token_del_status:
                 msg = (_("Unable to remove token: %s") % token.name)
                 return callback.error(msg)
             self.tokens.remove(token.uuid)
 
         # Remove used SOTPs/SLPs.
-        for otype in ['sotp', 'slp']:
-            _used = self._get_used(otype)
-            for uuid in _used:
-                used_oid = backend.get_oid(uuid)
-                used_oid = oid.get(used_oid)
-                try:
-                    backend.delete_object(used_oid)
-                except Exception as e:
-                    msg = ("Error removing used %s '%s' from backend: %s"
-                            % (otype.upper(), used_object, e))
-                    logger.critical(msg)
+        _used = self._get_used()
+        for uuid in _used:
+            used_oid = backend.get_oid(uuid)
+            used_oid = oid.get(used_oid)
+            try:
+                backend.delete_object(used_oid)
+            except Exception as e:
+                msg = ("Error removing used SOTP '%s' from backend: %s"
+                        % (used_object, e))
+                logger.critical(msg)
 
         # Make sure to remove user from signers cache.
         sign_key_cache.del_cache(self.oid)
 
         # Delete object using parent class.
         del_status = super(User, self).delete(verbose_level=verbose_level,
                                             force=force, callback=callback)
@@ -4374,14 +4443,20 @@
 
         if view_acl or edit_acl:
             autosign = "Disabled"
             if self.autosign_enabled:
                 autosign = "Enabled"
             lines.append("\tauto-sign:\t\t%s\n" % autosign)
 
+        if view_acl or edit_acl:
+            allow_disabled_login = "Disabled"
+            if self.allow_disabled_login:
+                allow_disabled_login = "Enabled"
+            lines.append("\tallow-disabled-login:\t%s\n" % allow_disabled_login)
+
         if self.verify_acl("view:auth_script") \
         or self.verify_acl("enable:auth_script") \
         or self.verify_acl("disable:auth_script"):
             auth_script = "N/A"
             auth_script_status = "N/A"
             if self.auth_script:
                 if self.auth_script_enabled:
```

### Comparing `otpme-0.3.0a78/otpme/lib/cli/__init__.py` & `otpme-0.3.0a79/otpme/lib/cli/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1343,43 +1343,33 @@
     if reverse_sort:
         tree_level_multiplier = -1
     else:
         tree_level_multiplier = 1
 
 
     write_acls = [
-                "edit:session",
+                "delete:session",
                 ]
 
     read_acls = [
                 "view:session",
             ]
 
+    # Combine all ACLs to be checked.
+    verify_acls = write_acls + read_acls
+
     show_username = False
-    show_only_editable_objects = True
     if show_all:
         show_username = True
         if search_regex is None:
             search_regex = "*"
-        if config.auth_token:
-            if config.auth_token.is_admin():
-                show_only_editable_objects = False
 
     if search_regex is not None:
         show_username = True
 
-    # Combine all ACLs to be checked.
-    verify_acls = write_acls + read_acls
-
-    # If we will show only objects the user has edit permissions on
-    # we do not have to query for any "view-only" ACLs. This way the
-    # query is faster.
-    if show_only_editable_objects:
-        verify_acls = write_acls
-
     # Admin user does not need ACL check.
     if config.auth_token:
         if config.auth_token.is_admin():
             verify_acls = None
             if search_regex is None:
                 search_regex = config.auth_user.name
         else:
```

### Comparing `otpme-0.3.0a78/otpme/lib/cli/accessgroup.py` & `otpme-0.3.0a79/otpme/lib/cli/accessgroup.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/cli/ca.py` & `otpme-0.3.0a79/otpme/lib/cli/ca.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/cli/client.py` & `otpme-0.3.0a79/otpme/lib/cli/client.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/cli/dictionary.py` & `otpme-0.3.0a79/otpme/lib/cli/dictionary.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/cli/group.py` & `otpme-0.3.0a79/otpme/lib/cli/group.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/cli/host.py` & `otpme-0.3.0a79/otpme/lib/cli/host.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/cli/node.py` & `otpme-0.3.0a79/otpme/lib/cli/node.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/cli/policy.py` & `otpme-0.3.0a79/otpme/lib/cli/policy.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/cli/realm.py` & `otpme-0.3.0a79/otpme/lib/cli/realm.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/cli/resolver.py` & `otpme-0.3.0a79/otpme/lib/cli/resolver.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/cli/role.py` & `otpme-0.3.0a79/otpme/lib/cli/role.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/cli/script.py` & `otpme-0.3.0a79/otpme/lib/cli/script.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/cli/site.py` & `otpme-0.3.0a79/otpme/lib/cli/site.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/cli/token.py` & `otpme-0.3.0a79/otpme/lib/cli/token.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/cli/unit.py` & `otpme-0.3.0a79/otpme/lib/cli/unit.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/cli/user.py` & `otpme-0.3.0a79/otpme/lib/cli/user.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/compgen.py` & `otpme-0.3.0a79/otpme/lib/compgen.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/compression/base.py` & `otpme-0.3.0a79/otpme/lib/compression/base.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/connections.py` & `otpme-0.3.0a79/otpme/lib/connections.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/daemon/__init__.py` & `otpme-0.3.0a79/otpme/lib/daemon/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,15 @@
         'otpme.lib.daemon.syncd',
         'otpme.lib.daemon.authd',
         'otpme.lib.daemon.joind',
         'otpme.lib.daemon.scriptd',
         'otpme.lib.daemon.mgmtd',
         'otpme.lib.daemon.hostd',
         'otpme.lib.daemon.ldapd',
+        'otpme.lib.daemon.httpd',
         'otpme.lib.daemon.clusterd',
         ]
 
 def register():
     """ Register object modules. """
     from otpme.lib.register import _register_modules
     _register_modules(modules)
```

### Comparing `otpme-0.3.0a78/otpme/lib/daemon/authd.py` & `otpme-0.3.0a79/otpme/lib/daemon/authd.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/daemon/clusterd.py` & `otpme-0.3.0a79/otpme/lib/daemon/clusterd.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,15 +150,15 @@
     except ValueError:
         pass
     if not multiprocessing.cluster_out_event:
         return
     multiprocessing.cluster_out_event.set()
 
 def cluster_sync_object(object_uuid, object_id, action, object_config=None,
-    new_object_id=None, checksum=None, wait_for_write=True):
+    new_object_id=None, checksum=None, index_journal=None, wait_for_write=True):
     if not multiprocessing.cluster_out_event:
         return
     if config.one_node_setup:
         return
     if config.two_node_setup:
         if len(multiprocessing.online_nodes) == 0:
             if action != "delete":
@@ -169,14 +169,15 @@
     while True:
         try:
             cluster_journal_entry = ClusterJournalEntry(timestamp=time.time_ns(),
                                                     action=action,
                                                     object_uuid=object_uuid,
                                                     object_id=object_id,
                                                     checksum=checksum,
+                                                    index_journal=index_journal,
                                                     object_config=object_config,
                                                     new_object_id=new_object_id)
         except AlreadyExists:
             continue
         else:
             break
     if not wait_for_write:
@@ -394,32 +395,35 @@
         msg = ("Deleted cluster entry: %s" % object_id)
         self.logger.debug(msg)
 
 class ClusterJournalEntry(ClusterEntry):
     """ Cluster journal entry. """
     def __init__(self, timestamp, object_uuid=None, action=None,
         object_id=None, checksum=None, object_config=None,
-        new_object_id=None):
+        index_journal=None, new_object_id=None):
         journal_dir = config.cluster_out_journal_dir
         super(ClusterJournalEntry, self).__init__(journal_dir=journal_dir,
                                                     _lock_type=JOURNAL_LOCK_TYPE,
                                                     timestamp=timestamp,
                                                     action=action)
         self.object_id_file = os.path.join(self.entry_dir, "object_id")
         self.object_uuid_file = os.path.join(self.entry_dir, "object_uuid")
         self.new_object_id_file = os.path.join(self.entry_dir, "new_object_id")
         self.object_checksum_file = os.path.join(self.entry_dir, "object_checksum")
+        self.index_journal_file = os.path.join(self.entry_dir, "index_journal")
         if action is not None:
             self.action = action
         if object_id is not None:
             self.object_id = object_id
         if object_uuid is not None:
             self.object_uuid = object_uuid
         if object_config is not None:
             self.object_config = object_config
+        if index_journal is not None:
+            self.index_journal = index_journal
         if checksum is not None:
             self.object_checksum = checksum
         if new_object_id is not None:
             self.new_object_id = new_object_id
 
     def __str__(self):
         return self.timestamp
@@ -448,15 +452,15 @@
     def object_id(self):
         try:
             object_id = filetools.read_file(self.object_id_file)
         except FileNotFoundError:
             object_id = None
         except Exception as e:
             object_id = None
-            msg = ("Failed to read object ID from lock entry: %s: %s"
+            msg = ("Failed to read object ID from cluster entry: %s: %s"
                     % (self.timestamp, e))
             self.logger.critical(msg)
         return object_id
 
     @object_id.setter
     #@entry_lock(write=True)
     def object_id(self, object_id):
@@ -473,15 +477,15 @@
     def new_object_id(self):
         try:
             new_object_id = filetools.read_file(self.new_object_id_file)
         except FileNotFoundError:
             new_object_id = None
         except Exception as e:
             new_object_id = None
-            msg = ("Failed to read new object ID from lock entry: %s: %s"
+            msg = ("Failed to read new object ID from cluster entry: %s: %s"
                     % (self.timestamp, e))
             self.logger.critical(msg)
         return new_object_id
 
     @new_object_id.setter
     #@entry_lock(write=True)
     def new_object_id(self, new_object_id):
@@ -498,15 +502,15 @@
     def object_uuid(self):
         try:
             object_uuid = filetools.read_file(self.object_uuid_file)
         except FileNotFoundError:
             object_uuid = None
         except Exception as e:
             object_uuid = None
-            msg = ("Failed to read object UUID from lock entry: %s: %s"
+            msg = ("Failed to read object UUID from cluster entry: %s: %s"
                     % (self.timestamp, e))
             self.logger.critical(msg)
         return object_uuid
 
     @object_uuid.setter
     #@entry_lock(write=True)
     def object_uuid(self, object_uuid):
@@ -523,15 +527,15 @@
     def object_checksum(self):
         try:
             object_checksum = filetools.read_file(self.object_checksum_file)
         except FileNotFoundError:
             object_checksum = None
         except Exception as e:
             object_checksum = None
-            msg = ("Failed to read object checksum from lock entry: %s: %s"
+            msg = ("Failed to read object checksum from cluster entry: %s: %s"
                     % (self.timestamp, e))
             self.logger.critical(msg)
         return object_checksum
 
     @object_checksum.setter
     #@entry_lock(write=True)
     def object_checksum(self, object_checksum):
@@ -541,14 +545,41 @@
         except Exception as e:
             msg = ("Failed to add object checksum to cluster entry: %s: %s"
                     % (self.timestamp, e))
             self.logger.critical(msg)
 
     @property
     @entry_lock(write=False)
+    def index_journal(self):
+        try:
+            index_journal = filetools.read_file(self.index_journal_file)
+        except FileNotFoundError:
+            index_journal = None
+        except Exception as e:
+            index_journal = None
+            msg = ("Failed to read index journal from cluster entry: %s: %s"
+                    % (self.timestamp, e))
+            self.logger.critical(msg)
+        index_journal = ujson.loads(index_journal)
+        return index_journal
+
+    @index_journal.setter
+    #@entry_lock(write=True)
+    def index_journal(self, index_journal):
+        index_journal = ujson.dumps(index_journal)
+        try:
+            filetools.create_file(path=self.index_journal_file,
+                                    content=index_journal)
+        except Exception as e:
+            msg = ("Failed to add index journal to cluster entry: %s: %s"
+                    % (self.timestamp, e))
+            self.logger.critical(msg)
+
+    @property
+    @entry_lock(write=False)
     def object_config(self):
         try:
             object_config = multiprocessing.cluster_journal[self.timestamp]
         except KeyError:
             object_config = None
         return object_config
 
@@ -774,15 +805,15 @@
                 msg = "Data sync finished with node: %s" % node_name
                 self.logger.info(msg)
                 break
             except Exception as e:
                 msg = "Failed to sync with node: %s: %s" % (node_name, e)
                 self.logger.warning(msg)
                 time.sleep(1)
-                config.raise_exception()
+                #config.raise_exception()
 
     def start_interprocess_comm(self):
         """ Start cluster interprocess communication. """
         # Set proctitle.
         new_proctitle = "%s (Cluster IPC)" % self.full_name
         setproctitle.setproctitle(new_proctitle)
         def signal_handler(_signal, frame):
@@ -1068,14 +1099,16 @@
                             value="*",
                             realm=config.realm,
                             site=config.site,
                             return_type="instance")
         all_nodes = {}
         enabled_nodes = {}
         for node in result:
+            if node.uuid == config.uuid:
+                continue
             all_nodes[node.name] = node
             if not node.enabled:
                 continue
             enabled_nodes[node.name] = node
 
         try:
             own_node = all_nodes[self.host_name]
@@ -1215,15 +1248,15 @@
         while True:
             if config.daemon_shutdown:
                 os._exit(0)
             try:
                 clusterd_conn = self.get_clusterd_connection(master_node)
             except Exception as e:
                 self.node_disconnect(master_node)
-                msg = ("Failed to get cluster connection: %s: %s"
+                msg = ("Error getting cluster connection: %s: %s"
                         % (master_node, e))
                 self.logger.warning(msg)
                 current_try += 1
                 if current_try >= max_tries:
                     msg = ("Failed to get cluster connection after %s tries."
                             % max_tries)
                     self.logger.warning(msg)
@@ -1263,28 +1296,29 @@
             else:
                 return self.node_conn
 
         if self.node_conn is None:
             try:
                 self.node_conn = self.get_clusterd_connection(node_name)
             except Exception as e:
-                self.node_leave(node_name)
                 if not self.node_offline:
                     if not quiet:
                         msg = ("Failed to get cluster connection: %s: %s"
                                 % (node_name, e))
                         self.logger.warning(msg)
+                    self.node_leave(node_name)
                     self.node_offline = True
                 return None
             else:
                 multiprocessing.online_nodes[node_name] = True
-                self.node_offline = False
-                if not quiet:
-                    msg = "Node is online: %s" % node_name
-                    self.logger.info(msg)
+                if self.node_offline:
+                    if not quiet:
+                        msg = "Node is online: %s" % node_name
+                        self.logger.info(msg)
+                    self.node_offline = False
                 return self.node_conn
 
     def do_node_check(self, node_name):
         node_conn = self.get_node_connection(node_name)
         if not node_conn:
             return False
 
@@ -1365,15 +1399,15 @@
     def start_cluster_communication(self, **kwargs):
         """ Start cluster communication. """
         try:
             self._start_cluster_communication(**kwargs)
         except Exception as e:
             msg = "Error in cluster communication method: %s" % e
             self.logger.critical(msg)
-            config.raise_exception()
+            #config.raise_exception()
 
     def _start_cluster_communication(self, reload=False):
         """ Start cluster communication. """
         # Set proctitle.
         new_proctitle = "%s (Cluster communication)" % self.full_name
         setproctitle.setproctitle(new_proctitle)
         def signal_handler(_signal, frame):
@@ -1545,14 +1579,22 @@
                 current_master_node = multiprocessing.master_node['master']
             except KeyError:
                 current_master_node = None
             if current_master_node == new_master_node:
                 time.sleep(quorum_check_interval)
                 continue
 
+            while True:
+                cluster_journal_files = self.get_cluster_in_journal()
+                if not cluster_journal_files:
+                    break
+                msg = "Waiting for cluster in journal to be processed..."
+                self.logger.info(msg)
+                time.sleep(1)
+
             try:
                 self.switch_master_node(current_master_node, new_master_node)
             except Exception as e:
                 msg = "Failed to switch master node: %s" % e
                 self.logger.critical(msg)
 
             time.sleep(quorum_check_interval)
@@ -1654,42 +1696,32 @@
             action = object_data['action']
             if action == "write":
                 object_id = object_data['object_id']
                 object_id = oid.get(object_id)
                 last_used = object_data['last_used']
                 full_data_update = object_data['full_data_update']
                 full_index_update = object_data['full_index_update']
+                index_journal = object_data['index_journal']
                 object_config = object_data['object_config']
                 object_config = ObjectConfig(object_id, object_config)
                 object_config = object_config.decrypt(config.master_key)
                 object_uuid = object_config['UUID']
 
-                index_auto_update = False
-                if full_index_update:
-                    index_journal = []
-                else:
-                    try:
-                        index_journal = object_config['INDEX_JOURNAL']
-                    except KeyError:
-                        index_auto_update = True
-                        index_journal = []
-
                 x_object = backend.get_object(object_id)
                 if x_object:
                     x_object.acquire_lock(lock_caller="cluster")
                 try:
                     if last_used is not None:
                         backend.set_last_used(object_id.realm,
                                             object_id.site,
                                             object_id.object_type,
                                             object_uuid, last_used)
                     try:
                         backend.write_config(object_id=object_id,
                                             cluster=False,
-                                            index_auto_update=index_auto_update,
                                             full_data_update=full_data_update,
                                             full_index_update=full_index_update,
                                             index_journal=index_journal,
                                             object_config=object_config)
                     except Exception as e:
                         msg = "Failed to write object: %s: %s" % (object_id, e)
                         self.logger.warning(msg)
@@ -1792,15 +1824,15 @@
 
     def start_two_node_handler(self):
         try:
             self._start_two_node_handler()
         except Exception as e:
             msg = "Error in two node handler: %s" % e
             self.logger.critical(msg)
-            config.raise_exception()
+            #config.raise_exception()
 
     def _start_two_node_handler(self):
         """ Start two node handler. """
         # Set proctitle.
         new_proctitle = ("%s Cluster two node handler" % (self.full_name))
         setproctitle.setproctitle(new_proctitle)
 
@@ -1901,15 +1933,15 @@
 
     def start_node_write_connection(self, node_name):
         try:
             self._start_node_write_connection(node_name)
         except Exception as e:
             msg = "Error in node write connection: %s" % e
             self.logger.critical(msg)
-            config.raise_exception()
+            #config.raise_exception()
 
     def _start_node_write_connection(self, node_name):
         """ Start cluster write communication with node. """
         # Set proctitle.
         new_proctitle = ("%s Cluster sync (%s)"
                         % (self.full_name, node_name))
         setproctitle.setproctitle(new_proctitle)
@@ -1985,15 +2017,15 @@
             try:
                 written_entries = self.process_cluster_journal(node_name)
             except ProcessingFailed:
                 return True
             except Exception as e:
                 msg = "Error processing cluster journal: %s" % e
                 self.logger.critical(msg)
-                config.raise_exception()
+                #config.raise_exception()
                 return True
             if not self.member_candidate:
                 break
             if len(written_entries) <= 10:
                 break
         if self.member_candidate:
             multiprocessing.pause_writes.append(self.pid)
@@ -2001,15 +2033,15 @@
                 try:
                     self.process_cluster_journal(node_name)
                 except ProcessingFailed:
                     return True
                 except Exception as e:
                     msg = "Error processing cluster journal: %s" % e
                     self.logger.critical(msg)
-                    config.raise_exception()
+                    #config.raise_exception()
                     return True
                 # Update data revision on peer.
                 if config.master_node:
                     try:
                         remote_data_revision = self.node_conn.get_data_revision()
                     except Exception as e:
                         msg = "Failed to get data revision: %s: %s" % (node_name, e)
@@ -2076,15 +2108,15 @@
         for journal_dir in cluster_journal_dirs:
             entry_timestamp = os.path.basename(journal_dir)
             cluster_journal_entry = ClusterJournalEntry(timestamp=entry_timestamp)
             try:
                 if not cluster_journal_entry.committed:
                     break
                 if node_name in cluster_journal_entry.get_nodes():
-                    # Check if object was written to member nodes
+                    # Check if object was written to member nodes.
                     if self.check_member_nodes(cluster_journal_entry):
                         # Check if object was written to all online nodes.
                         self.check_online_nodes(cluster_journal_entry)
                     continue
                 entries_to_process.append(cluster_journal_entry)
             except ObjectDeleted:
                 pass
@@ -2119,14 +2151,15 @@
                 if config.master_node:
                     if object_id.object_type in config.tree_object_types:
                         if not unsync_status_set:
                             unsync_status_set = True
                             try:
                                 self.unset_node_sync(node_name)
                             except:
+                                self.check_member_nodes(cluster_journal_entry)
                                 raise ProcessingFailed()
                 # Write object to peer.
                 if action == "write":
                     object_config = cluster_journal_entry.object_config
                     # Remove outdated cluster journal entry.
                     if not object_config:
                         cluster_journal_entry.add_node(node_name)
@@ -2151,40 +2184,48 @@
                         if not oc:
                             oc = backend.read_config(object_id)
                         if oc:
                             full_data_update = True
                             full_index_update = True
                             full_object_update = True
                             object_config = oc.copy()
+                    index_journal = []
+                    if not full_index_update:
+                        index_journal = cluster_journal_entry.index_journal
                     try:
                         last_used = backend.get_last_used(object_id.realm,
                                                         object_id.site,
                                                         object_id.object_type,
                                                         object_uuid)
                     except Exception as e:
                         msg = "Failed to get last used time: %s" % object_id
                         self.logger.warning(msg)
                         continue
                     try:
                         write_status = node_conn.write(object_id.full_oid,
                                                         object_config,
                                                         last_used,
+                                                        index_journal=index_journal,
+                                                        #full_data_update=True,
                                                         full_data_update=full_data_update,
+                                                        #full_index_update=True)
                                                         full_index_update=full_index_update)
                     except (ConnectionTimeout, ConnectionError, ConnectionQuit) as e:
-                        self.node_disconnect(node_name)
+                        self.node_leave(node_name)
                         msg = ("Failed to send object: %s: %s: %s"
                                 % (node_name, object_id, e))
                         self.logger.warning(msg)
+                        self.check_member_nodes(cluster_journal_entry)
                         raise ProcessingFailed(msg)
                     except Exception as e:
-                        self.node_disconnect(node_name)
+                        self.node_leave(node_name)
                         msg = ("Error sending object: %s: %s: %s"
                                 % (node_name, object_id, e))
                         self.logger.warning(msg)
+                        self.check_member_nodes(cluster_journal_entry)
                         raise ProcessingFailed(msg)
                     if write_status != "done":
                         continue
                     msg = ("Written object to node: %s: %s (%s)"
                             % (node_name, object_id, object_checksum))
                     self.logger.debug(msg)
                     cluster_journal_entry.add_node(node_name)
@@ -2196,44 +2237,48 @@
                 if action == "rename":
                     new_object_id = cluster_journal_entry.new_object_id
                     new_object_id = oid.get(new_object_id)
                     try:
                         rename_status = node_conn.rename(object_id=object_id.full_oid,
                                                         new_object_id=new_object_id.full_oid)
                     except (ConnectionTimeout, ConnectionError, ConnectionQuit) as e:
-                        self.node_disconnect(node_name)
+                        self.node_leave(node_name)
                         msg = ("Failed to rename object: %s: %s: %s"
                                 % (node_name, object_id, e))
                         self.logger.warning(msg)
+                        self.check_member_nodes(cluster_journal_entry)
                         raise ProcessingFailed(msg)
                     except Exception as e:
-                        self.node_disconnect(node_name)
+                        self.node_leave(node_name)
                         msg = ("Failed to rename object: %s: %s: %s"
                                 % (node_name, object_id, e))
                         self.logger.warning(msg)
+                        self.check_member_nodes(cluster_journal_entry)
                         raise ProcessingFailed(msg)
                     if rename_status != "done":
                         continue
                     msg = ("Renamed object on node: %s: %s: %s"
                             % (node_name, object_id, new_object_id))
                     self.logger.debug(msg)
                     cluster_journal_entry.add_node(node_name)
                 # Delete object on peer.
                 if action == "delete":
                     try:
                         del_status = node_conn.delete(object_id.full_oid)
                     except (ConnectionTimeout, ConnectionError, ConnectionQuit) as e:
-                        self.node_disconnect(node_name)
+                        self.node_leave(node_name)
                         msg = "Failed to delete object: %s: %s" % (object_id, e)
                         self.logger.warning(msg)
+                        self.check_member_nodes(cluster_journal_entry)
                         raise ProcessingFailed(msg)
                     except Exception as e:
-                        self.node_disconnect(node_name)
+                        self.node_leave(node_name)
                         msg = "Failed to delete object: %s: %s" % (object_id, e)
                         self.logger.warning(msg)
+                        self.check_member_nodes(cluster_journal_entry)
                         raise ProcessingFailed(msg)
                     if del_status != "done":
                         continue
                     msg = ("Deleted object on node: %s: %s"
                             % (node_name, object_id))
                     self.logger.debug(msg)
                     try:
@@ -2276,21 +2321,21 @@
             self.logger.warning(msg)
             raise
 
     def unset_node_sync(self, node_name):
         try:
             self.node_conn.unset_node_sync()
         except (ConnectionTimeout, ConnectionError, ConnectionQuit) as e:
-            self.node_disconnect(node_name)
+            self.node_leave(node_name)
             msg = ("Failed to unset cluster sync state: %s: %s"
                     % (node_name, e))
             self.logger.warning(msg)
             raise
         except Exception as e:
-            self.node_disconnect(node_name)
+            self.node_leave(node_name)
             msg = ("Error unsetting cluster sync state: %s: %s"
                     % (node_name, e))
             self.logger.warning(msg)
             raise
 
     def check_online_nodes(self, cluster_journal_entry):
         entry_nodes = cluster_journal_entry.get_nodes()
@@ -2729,8 +2774,8 @@
                 if daemon_command == "ip_deconfigured":
                     config.master_failover = False
             except (KeyboardInterrupt, SystemExit):
                 pass
             except Exception as e:
                 msg = ("Unhandled error in clusterd: %s" % e)
                 self.logger.critical(msg, exc_info=True)
-                config.raise_exception()
+                #config.raise_exception()
```

### Comparing `otpme-0.3.0a78/otpme/lib/daemon/controld.py` & `otpme-0.3.0a79/otpme/lib/daemon/controld.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 from otpme.lib.register import register_modules
 
 from otpme.lib.daemon.authd import AuthDaemon
 from otpme.lib.daemon.mgmtd import MgmtDaemon
 from otpme.lib.daemon.syncd import SyncDaemon
 from otpme.lib.daemon.hostd import HostDaemon
 from otpme.lib.daemon.joind import JoinDaemon
+from otpme.lib.daemon.httpd import HttpDaemon
 from otpme.lib.daemon.scriptd import ScriptDaemon
 from otpme.lib.daemon.clusterd import ClusterDaemon
 from otpme.lib.daemon.unix_daemon import UnixDaemon
 #from otpme.lib.multiprocessing import handle_exit
 
 from otpme.lib.exceptions import *
 
@@ -464,21 +465,23 @@
                     'mgmtd',
                     'ldapd',
                     'joind',
                     'scriptd',
                     'syncd',
                     'authd',
                     'clusterd',
+                    'httpd',
                     ]
 
             # Set child daemons.
             child_daemons["authd"] = {}
             child_daemons["hostd"] = {}
             child_daemons["joind"] = {}
             child_daemons["ldapd"] = {}
+            child_daemons["httpd"] = {}
             child_daemons["mgmtd"] = {}
             child_daemons["syncd"] = {}
             child_daemons["scriptd"] = {}
             child_daemons["clusterd"] = {}
 
         if config.host_data['type'] == "host":
             # Daemons we have to handle and its start order.
@@ -933,14 +936,16 @@
 
         if daemon_name == "authd":
             daemon_class = AuthDaemon
         elif daemon_name == "hostd":
             daemon_class = HostDaemon
         elif daemon_name == "joind":
             daemon_class = JoinDaemon
+        elif daemon_name == "httpd":
+            daemon_class = HttpDaemon
         elif daemon_name == "ldapd":
             daemon_class = LdapDaemon
         elif daemon_name == "mgmtd":
             daemon_class = MgmtDaemon
         elif daemon_name == "syncd":
             daemon_class = SyncDaemon
         elif daemon_name == "scriptd":
```

### Comparing `otpme-0.3.0a78/otpme/lib/daemon/hostd.py` & `otpme-0.3.0a79/otpme/lib/daemon/hostd.py`

 * *Files 0% similar despite different names*

```diff
@@ -573,16 +573,14 @@
                         continue
                     # Realm/site objects need some special handling (e.g.
                     # preserve auth/sync settings.
                     if object_type == "realm" or object_type == "site":
                         # Preserve auth/sync settings.
                         o.auth_enabled = x_object.auth_enabled
                         o.sync_enabled = x_object.sync_enabled
-                        # Preserve journal ID to get sane index update.
-                        o.index_journal_id = x_object.index_journal_id
                         # Update object config.
                         o._set_variables()
                         o.set_variables()
                         o.update_object_config()
                         # Get object config of updated object.
                         object_config = o.object_config.copy()
                     updated_objects += 1
@@ -592,35 +590,33 @@
                     added_objects += 1
 
                 # Write object to backend. We cannot use o._write() because this
                 # triggers other things we do not want/need on sync.
                 try:
                     backend.write_config(object_id=x_oid,
                                     object_config=object_config,
-                                    index_auto_update=True)
+                                    full_index_update=True)
                 except Exception as e:
                     msg = "Failed to write object: %s: %s" % (x_oid, e)
                     self.logger.critical(msg)
                     config.raise_exception()
 
+        # Realm master nodes must not delete realms/sites.
+        if is_master_node:
+            if sync_status:
+                self.update_realm_data()
+            return True
+
         # Remove remote missing sites.
         local_sites = backend.search(object_type="site",
                                     attribute="uuid",
                                     value="*",
                                     return_type="instance")
         removed_objects = 0
         for site in local_sites:
-            # For realm master nodes we have to check if there was a problem
-            # getting the site object from its master node.
-            if is_master_node:
-                # If we were not able to get site from the master node (e.g. a
-                # connection problem) we must not remove it.
-                if site.oid not in reached_sites:
-                    continue
-
             # If the site is in the list of sites we received from master node
             # there is no need to remove it.
             if site.oid in sync_sites:
                 continue
 
             # We will not delete our own site. :)
             if site.uuid == config.site_uuid:
```

### Comparing `otpme-0.3.0a78/otpme/lib/daemon/joind.py` & `otpme-0.3.0a79/otpme/lib/daemon/joind.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/daemon/ldapd.py` & `otpme-0.3.0a79/otpme/lib/daemon/ldapd.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/daemon/mgmtd.py` & `otpme-0.3.0a79/otpme/lib/daemon/mgmtd.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/daemon/otpme_daemon.py` & `otpme-0.3.0a79/otpme/lib/daemon/otpme_daemon.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/daemon/scriptd.py` & `otpme-0.3.0a79/otpme/lib/daemon/scriptd.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/daemon/syncd.py` & `otpme-0.3.0a79/otpme/lib/daemon/syncd.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/daemon/unix_daemon.py` & `otpme-0.3.0a79/otpme/lib/daemon/unix_daemon.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/debug.py` & `otpme-0.3.0a79/otpme/lib/debug.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/doc.py` & `otpme-0.3.0a79/otpme/lib/doc.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/encoding/base.py` & `otpme-0.3.0a79/otpme/lib/encoding/base.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/encryption/__init__.py` & `otpme-0.3.0a79/otpme/lib/encryption/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/encryption/aes.py` & `otpme-0.3.0a79/otpme/lib/encryption/aes.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/encryption/aes_cfb.py` & `otpme-0.3.0a79/otpme/lib/encryption/aes_cfb.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/encryption/argon2.py` & `otpme-0.3.0a79/otpme/lib/encryption/argon2.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/encryption/asymmetric_key_handler.py` & `otpme-0.3.0a79/otpme/lib/encryption/asymmetric_key_handler.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/encryption/ec.py` & `otpme-0.3.0a79/otpme/lib/encryption/ec.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/encryption/fernet.py` & `otpme-0.3.0a79/otpme/lib/encryption/fernet.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/encryption/hkdf.py` & `otpme-0.3.0a79/otpme/lib/encryption/hkdf.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/encryption/pbkdf2.py` & `otpme-0.3.0a79/otpme/lib/encryption/pbkdf2.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/encryption/rsa.py` & `otpme-0.3.0a79/otpme/lib/encryption/rsa.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/exceptions.py` & `otpme-0.3.0a79/otpme/lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/extensions/base/base.py` & `otpme-0.3.0a79/otpme/lib/extensions/base/base.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/extensions/ldif_handler.py` & `otpme-0.3.0a79/otpme/lib/extensions/ldif_handler.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/extensions/posix/posix.py` & `otpme-0.3.0a79/otpme/lib/extensions/posix/posix.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/extensions/utils.py` & `otpme-0.3.0a79/otpme/lib/extensions/utils.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/filetools.py` & `otpme-0.3.0a79/otpme/lib/filetools.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import copy
 import time
 import ujson
 import fcntl
 import pprint
 import shutil
 from pathlib import Path
+from functools import wraps
 
 try:
     if os.environ['OTPME_DEBUG_MODULE_LOADING'] == "True":
         print(_("Loading module: %s") % __name__)
 except:
     pass
 
@@ -258,26 +259,14 @@
                 if not force:
                     self.release_lock()
                 return False
         # Remove file.
         self.fd.unlink()
         return True
 
-#def get_file_lock(path, write=True):
-#    from otpme.lib import locking
-#    real_path = os.path.realpath(path)
-#    lock_id = real_path.replace("/", ":")
-#    try:
-#        _lock = locking.acquire_lock(lock_type=FILE_LOCK_TYPE,
-#                                    lock_id=lock_id, write=write)
-#    except OTPmeException as e:
-#        msg = "Failed to acquire file lock: %s: %s" % (real_path, e)
-#        raise ObjectLocked(msg)
-#    return _lock
-
 def copy_file(src, dst):
     """ Copy file and perserving ownership and permissions. """
     try:
         shutil.copy2(src, dst)
         st = os.stat(src)
         os.chown(dst, st[stat.ST_UID], st[stat.ST_GID])
     except Exception as e:
@@ -688,14 +677,36 @@
     _file = JsonFile(filename)
     return _file.read(*args, **kwargs)
 
 def write_data_file(filename, *args, **kwargs):
     _file = JsonFile(filename)
     return _file.write(*args, **kwargs)
 
+def write_lock(write=True):
+    """ Decorator to handle write lock. """
+    def wrapper(f):
+        @wraps(f)
+        def wrapped(self, *f_args, **f_kwargs):
+            from otpme.lib import locking
+            lock_id = self.file_path.replace("/", ":")
+            try:
+                _lock = locking.acquire_lock(lock_type=FILE_LOCK_TYPE,
+                                            lock_id=lock_id, write=write)
+            except OTPmeException as e:
+                msg = "Failed to acquire file lock: %s: %s" % (self.file_path, e)
+                raise ObjectLocked(msg)
+            # Call given class method.
+            try:
+                result = f(self, *f_args, **f_kwargs)
+            finally:
+                _lock.release_lock()
+            return result
+        return wrapped
+    return wrapper
+
 class JsonFile(object):
     def __init__(self, file_path):
         from otpme.lib import config
         # Get file real path to ensure working locking (e.g. on symlink).
         file_real_path = os.path.realpath(file_path)
         self.file_path = file_real_path
         self.logger = config.logger
@@ -826,14 +837,15 @@
             for attr in dict(object_config):
                 if attr in parameters:
                     continue
                 object_config.pop(attr)
 
         return object_config
 
+    @write_lock(write=True)
     def write(self, object_config, full_data_update=None,
         user=None, group=True, mode=0o660, user_acls=[], group_acls=[]):
         """ Write dictionary to JSON config file. """
         from otpme.lib import stuff
         from otpme.lib import config
 
         if user is None:
@@ -907,14 +919,15 @@
                     increment_ids = current_oc["INCREMENT_IDS"]
                 except KeyError:
                     increment_ids = []
                 increment_ids = sorted(increment_ids)
                 for x in increment_ids:
                     incr_id = x[1]
                     if new_incr_id == incr_id:
+                        self.logger.warning("Duplicate write: %s" % self.file_path)
                         return
 
             if full_data_update is True:
                 self.write_file(object_config)
                 return
 
             _modified_attributes = modified_attributes.copy()
```

### Comparing `otpme-0.3.0a78/otpme/lib/freeradius/__init__.py` & `otpme-0.3.0a79/otpme/lib/freeradius/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/freeradius/otpme.py` & `otpme-0.3.0a79/otpme/lib/freeradius/otpme.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/freeradius/radiusd.py` & `otpme-0.3.0a79/otpme/lib/freeradius/radiusd.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/freeradius/radiusd_test.py` & `otpme-0.3.0a79/otpme/lib/freeradius/radiusd_test.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/gpg/utils.py` & `otpme-0.3.0a79/otpme/lib/gpg/utils.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/help/__init__.py` & `otpme-0.3.0a79/otpme/lib/help/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/help/accessgroup.py` & `otpme-0.3.0a79/otpme/lib/help/accessgroup.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/help/agent.py` & `otpme-0.3.0a79/otpme/lib/help/agent.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/help/auth.py` & `otpme-0.3.0a79/otpme/lib/help/auth.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/help/ca.py` & `otpme-0.3.0a79/otpme/lib/help/ca.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/help/client.py` & `otpme-0.3.0a79/otpme/lib/help/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -358,14 +358,45 @@
                     '_cmd_usage_help' : 'Usage: otpme-client show_secret {client}',
                     'cmd'   :   '<|object|>',
                     '_help' :   {
                                     'cmd'                   : 'show clients secret',
                                 },
                 },
 
+    'enable_sso'    : {
+                    '_cmd_usage_help' : 'Usage: otpme-client enable_sso {client}',
+                    'cmd'   :   '<|object|>',
+                    '_help' :   {
+                                    'cmd'                   : 'Enable SSO app for this client.',
+                                },
+                },
+
+    'disable_sso'    : {
+                    '_cmd_usage_help' : 'Usage: otpme-client disable_sso {client}',
+                    'cmd'   :   '<|object|>',
+                    '_help' :   {
+                                    'cmd'                   : 'Disable SSO app for this client.',
+                                },
+                },
+
+    'login_url'    : {
+                    '_cmd_usage_help' : 'Usage: otpme-client login_url {client} {login_url}',
+                    'cmd'   :   '<|object|> <login_url>',
+                    '_help' :   {
+                                    'cmd'                   : 'Change clients login URL.',
+                                },
+                },
+
+    'helper_url'    : {
+                    '_cmd_usage_help' : 'Usage: otpme-client helper_url {client} {helper_url}',
+                    'cmd'   :   '<|object|> <helper_url>',
+                    '_help' :   {
+                                    'cmd'                   : 'Change clients SSO helper URL.',
+                                },
+                },
 
     'add_address'   : {
                     '_cmd_usage_help' : 'Usage: otpme-client add_address {client} {address}',
                     'cmd'   :   '<|object|> <address>',
                     '_help' :   {
                                     'cmd'                   : 'add address to client',
                                 },
```

### Comparing `otpme-0.3.0a78/otpme/lib/help/cluster.py` & `otpme-0.3.0a79/otpme/lib/help/cluster.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/help/controld.py` & `otpme-0.3.0a79/otpme/lib/help/controld.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/help/dictionary.py` & `otpme-0.3.0a79/otpme/lib/help/dictionary.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/help/get_authorized_keys.py` & `otpme-0.3.0a79/otpme/lib/help/get_authorized_keys.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/help/group.py` & `otpme-0.3.0a79/otpme/lib/help/group.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/help/host.py` & `otpme-0.3.0a79/otpme/lib/help/host.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/help/node.py` & `otpme-0.3.0a79/otpme/lib/help/node.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/help/policy/__init__.py` & `otpme-0.3.0a79/otpme/lib/help/policy/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/help/policy/authonaction.py` & `otpme-0.3.0a79/otpme/lib/help/policy/authonaction.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/help/policy/autodisable.py` & `otpme-0.3.0a79/otpme/lib/help/policy/autodisable.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/help/policy/defaultgroups.py` & `otpme-0.3.0a79/otpme/lib/help/policy/defaultgroups.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/help/policy/defaultpolicies.py` & `otpme-0.3.0a79/otpme/lib/help/policy/defaultpolicies.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/help/policy/defaultroles.py` & `otpme-0.3.0a79/otpme/lib/help/policy/defaultroles.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/help/policy/defaultunits.py` & `otpme-0.3.0a79/otpme/lib/help/policy/defaultunits.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/help/policy/forcetoken.py` & `otpme-0.3.0a79/otpme/lib/help/policy/forcetoken.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/help/policy/idrange.py` & `otpme-0.3.0a79/otpme/lib/help/policy/idrange.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/help/policy/logintimes.py` & `otpme-0.3.0a79/otpme/lib/help/policy/logintimes.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/help/policy/objecttemplates.py` & `otpme-0.3.0a79/otpme/lib/help/policy/objecttemplates.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/help/policy/password.py` & `otpme-0.3.0a79/otpme/lib/help/policy/password.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/help/policy/tokenacls.py` & `otpme-0.3.0a79/otpme/lib/help/policy/tokenacls.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/help/realm.py` & `otpme-0.3.0a79/otpme/lib/help/realm.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/help/register.py` & `otpme-0.3.0a79/otpme/lib/help/register.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/help/resolver/__init__.py` & `otpme-0.3.0a79/otpme/lib/help/resolver/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/help/resolver/ldap.py` & `otpme-0.3.0a79/otpme/lib/help/resolver/ldap.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/help/role.py` & `otpme-0.3.0a79/otpme/lib/help/role.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/help/script.py` & `otpme-0.3.0a79/otpme/lib/help/script.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/help/session.py` & `otpme-0.3.0a79/otpme/lib/help/session.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/help/site.py` & `otpme-0.3.0a79/otpme/lib/help/site.py`

 * *Files 2% similar despite different names*

```diff
@@ -346,14 +346,62 @@
                     '_cmd_usage_help' : 'Usage: otpme-site del_radius_key {site}',
                     'cmd'   :   '<|object|>',
                     '_help' :   {
                                     'cmd'                   : 'Delete radius key.',
                                 },
                 },
 
+    'sso_cert'   : {
+                    '_cmd_usage_help' : 'Usage: otpme-site sso_cert {site} {sso_cert}',
+                    'cmd'   :   '<|object|> <file:sso_cert>',
+                    '_help' :   {
+                                    'cmd'                   : 'Change SSO certificate.',
+                                },
+                },
+
+    'sso_key'   : {
+                    '_cmd_usage_help' : 'Usage: otpme-site sso_key {site} {sso_key}',
+                    'cmd'   :   '<|object|> <file:sso_key>',
+                    '_help' :   {
+                                    'cmd'                   : 'Change SSO certificate key.',
+                                },
+                },
+
+    'del_sso_cert'   : {
+                    '_cmd_usage_help' : 'Usage: otpme-site del_sso_cert {site}',
+                    'cmd'   :   '<|object|>',
+                    '_help' :   {
+                                    'cmd'                   : 'Delete SSO certificate.',
+                                },
+                },
+
+    'del_sso_key'   : {
+                    '_cmd_usage_help' : 'Usage: otpme-site del_sso_key {site}',
+                    'cmd'   :   '<|object|>',
+                    '_help' :   {
+                                    'cmd'                   : 'Delete SSO key.',
+                                },
+                },
+
+    'sso_secret'   : {
+                    '_cmd_usage_help' : 'Usage: otpme-site sso_secret {site} {sso_secret}',
+                    'cmd'   :   '<|object|> <secret>',
+                    '_help' :   {
+                                    'cmd'                   : 'Change SSO secret.',
+                                },
+                },
+
+    'sso_csrf_secret'   : {
+                    '_cmd_usage_help' : 'Usage: otpme-site sso_csrf_secret {site} {sso_csrf_secret}',
+                    'cmd'   :   '<|object|> <secret>',
+                    '_help' :   {
+                                    'cmd'                   : 'Change SSO CSRF secret.',
+                                },
+                },
+
     'dump_ca_chain'   : {
                     '_cmd_usage_help' : 'Usage: otpme-site dump_ca_chain {site}',
                     'cmd'   :   '<|object|>',
                     '_help' :   {
                                     'cmd'                   : 'dump site certificate chain of site cert to stdout',
                                 },
                 },
```

### Comparing `otpme-0.3.0a78/otpme/lib/help/token/__init__.py` & `otpme-0.3.0a79/otpme/lib/help/token/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/help/token/fido2.py` & `otpme-0.3.0a79/otpme/lib/help/token/fido2.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/help/token/hotp.py` & `otpme-0.3.0a79/otpme/lib/help/token/hotp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/help/token/motp.py` & `otpme-0.3.0a79/otpme/lib/help/token/motp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/help/token/otp_push.py` & `otpme-0.3.0a79/otpme/lib/help/token/otp_push.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/help/token/otpme.py` & `otpme-0.3.0a79/otpme/lib/help/token/otpme.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/help/token/password.py` & `otpme-0.3.0a79/otpme/lib/help/token/password.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/help/token/ssh.py` & `otpme-0.3.0a79/otpme/lib/help/token/ssh.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/help/token/totp.py` & `otpme-0.3.0a79/otpme/lib/help/token/totp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/help/token/yubikey_hmac.py` & `otpme-0.3.0a79/otpme/lib/help/token/yubikey_hmac.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/help/token/yubikey_hotp.py` & `otpme-0.3.0a79/otpme/lib/help/token/yubikey_hotp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/help/tool.py` & `otpme-0.3.0a79/otpme/lib/help/tool.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/help/unit.py` & `otpme-0.3.0a79/otpme/lib/help/unit.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/help/user.py` & `otpme-0.3.0a79/otpme/lib/help/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -205,14 +205,30 @@
                     '_cmd_usage_help' : 'Usage: otpme-user touch {user}',
                     'cmd'   :   '<|object|>',
                     '_help' :   {
                                     'cmd'                   : 'Touch user (e.g. migrate).',
                                 },
                 },
 
+    'enable_disabled_login'    : {
+                    '_cmd_usage_help' : 'Usage: otpme-user _disabled_loginenable {user}',
+                    'cmd'   :   '<|object|>',
+                    '_help' :   {
+                                    'cmd'                   : 'Enable user to login even if e.g. accessgroup is disabled.',
+                                },
+                },
+
+    'disable_disabled_login'    : {
+                    '_cmd_usage_help' : 'Usage: otpme-user _disabled_logindisable {user}',
+                    'cmd'   :   '<|object|>',
+                    '_help' :   {
+                                    'cmd'                   : 'Disable user to login even if e.g. accessgroup is disabled.',
+                                },
+                },
+
     'enable'    : {
                     '_cmd_usage_help' : 'Usage: otpme-user enable {user}',
                     'cmd'   :   '<|object|>',
                     '_help' :   {
                                     'cmd'                   : 'enable user',
                                 },
                 },
```

### Comparing `otpme-0.3.0a78/otpme/lib/host.py` & `otpme-0.3.0a79/otpme/lib/host.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/humanize/units.py` & `otpme-0.3.0a79/otpme/lib/humanize/units.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/index/mysql.py` & `otpme-0.3.0a79/otpme/lib/index/mysql.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/index/postgres.py` & `otpme-0.3.0a79/otpme/lib/index/postgres.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/index/sqlite3.py` & `otpme-0.3.0a79/otpme/lib/index/sqlite3.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/job/callback.py` & `otpme-0.3.0a79/otpme/lib/job/callback.py`

 * *Files 7% similar despite different names*

```diff
@@ -401,22 +401,33 @@
             msg = (_("Unable to get public key of site "
                     "certificate: %s: %s") % (user.site, e))
             raise OTPmeException(msg)
         try:
             jwt_data = _jwt.decode(jwt=jwt,
                                    key=jwt_key,
                                    algorithm='RS256')
-        except Exception:
-            return False
-        jwt_token = jwt_data['login_token']
+        except Exception as e:
+            msg = "JWT decoding failed."
+            raise OTPmeException(msg)
+        # We do not allow SOTP generated JWTs. A login with a real
+        # token is required.
+        jwt_auth_type = jwt_data['auth_type']
+        if jwt_auth_type != "token":
+            msg = "Need token login, got: %s" % jwt_auth_type
+            raise OTPmeException(msg)
+        # Verify challenge.
         jwt_challenge = jwt_data['challenge']
-        if jwt_challenge == challenge:
-            if jwt_token == config.auth_token.uuid:
-                return jwt_data
-        return False
+        if jwt_challenge != challenge:
+            msg = "Wrong JWT challenge."
+            raise OTPmeException(msg)
+        # Verify JWT token.
+        jwt_token = jwt_data['login_token']
+        if jwt_token != config.auth_token.uuid:
+            msg = "Wrong login token: %s" % jwt_token
+            raise OTPmeException(msg)
 
     @handle_exception
     def dump(self, message,  timeout=1):
         """ Dump some data on client site. """
         return self.send(message, timeout=timeout, ignore_escaping=True)
 
     @handle_exception
```

### Comparing `otpme-0.3.0a78/otpme/lib/job/otpme_job.py` & `otpme-0.3.0a79/otpme/lib/job/otpme_job.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/join.py` & `otpme-0.3.0a79/otpme/lib/join.py`

 * *Files 1% similar despite different names*

```diff
@@ -417,16 +417,15 @@
                     current_checksum = current_object_config['CHECKSUM']
                     if current_checksum == new_checksum:
                         continue
                 logger.debug("Adding object: %s" % object_id)
                 # Write object to backend.
                 try:
                     backend.write_config(object_id=object_id,
-                                    index_auto_update=True,
-                                    #full_index_update=True,
+                                    full_index_update=True,
                                     object_config=object_config)
                 except Exception as e:
                     config.raise_exception()
                     msg = (_("Joining %s failed: Error adding object %s: %s")
                             % (self.host_type, object_id, e))
                     raise OTPmeException(msg)
                 # Update signers cache.
```

### Comparing `otpme-0.3.0a78/otpme/lib/json.py` & `otpme-0.3.0a79/otpme/lib/json.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/jwt.py` & `otpme-0.3.0a79/otpme/lib/jwt.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/ldap/client.py` & `otpme-0.3.0a79/otpme/lib/ldap/client.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/ldap/schema.py` & `otpme-0.3.0a79/otpme/lib/ldap/schema.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/ldap/server.py` & `otpme-0.3.0a79/otpme/lib/ldap/server.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/locking.py` & `otpme-0.3.0a79/otpme/lib/locking.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/log.py` & `otpme-0.3.0a79/otpme/lib/log.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/messages.py` & `otpme-0.3.0a79/otpme/lib/messages.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/mschap.py` & `otpme-0.3.0a79/otpme/lib/mschap.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/mschap_util.py` & `otpme-0.3.0a79/otpme/lib/mschap_util.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/multiprocessing.py` & `otpme-0.3.0a79/otpme/lib/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/net.py` & `otpme-0.3.0a79/otpme/lib/net.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/nsscache.py` & `otpme-0.3.0a79/otpme/lib/nsscache.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/offline_token.py` & `otpme-0.3.0a79/otpme/lib/offline_token.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/oid.py` & `otpme-0.3.0a79/otpme/lib/oid.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/otp/oath/hotp.py` & `otpme-0.3.0a79/otpme/lib/otp/oath/hotp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/otp/oath/totp.py` & `otpme-0.3.0a79/otpme/lib/otp/oath/totp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/otp/otpme/otpme.py` & `otpme-0.3.0a79/otpme/lib/otp/otpme/otpme.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/otp/yubico/yubiotp.py` & `otpme-0.3.0a79/otpme/lib/otp/yubico/yubiotp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/otpme_acl.py` & `otpme-0.3.0a79/otpme/lib/otpme_acl.py`

 * *Files 1% similar despite different names*

```diff
@@ -497,20 +497,20 @@
         # Add the "all" ACL.
         acl_list.append("all")
 
         # Add complete ACL to check for.
         acl_list.append(acl)
 
         # Add "edit" ACL.
-        if acl_name == "edit":
+        if acl_name == "edit" and acl_value  is None:
             acl_list.append("edit")
             acl_list.append("edit:attribute")
 
         # Add "view" ACL.
-        if acl_name == "view":
+        if acl_name == "view" and acl_value  is None:
             acl_list.append("view")
             acl_list.append("view_all")
             acl_list.append("view:attribute")
             acl_list.append("view_all:attribute")
 
         # Add value ACLs.
         if acl_name == "view":
```

### Comparing `otpme-0.3.0a78/otpme/lib/otpme_config.py` & `otpme-0.3.0a79/otpme/lib/otpme_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -318,14 +318,16 @@
         # OTPme username that was/will be used to login
         self.register_config_var("login_user", str, None)
         # Users (instance) of the authenticated user.
         self.register_config_var("auth_user", None, None)
         # Users token (instance) that was used to authenticate the user of the current
         # connection.
         self.register_config_var("auth_token", None, None)
+        # Which auth type the user authenticated (e.g. sotp)
+        self.register_config_var("auth_type", None, None)
         # Token with realm admin rights.
         self.register_config_var("admin_token_uuid", str, None)
         # OTPme site admin role UUID.
         self.register_config_var("admin_role_uuid", str, None)
         # Run root scripts as this user.
         self.register_config_var("root_script_user", str, "nobody",
                             config_file_parameter="ROOT_SCRIPT_USER")
```

### Comparing `otpme-0.3.0a78/otpme/lib/otpme_pass.py` & `otpme-0.3.0a79/otpme/lib/otpme_pass.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/pam.py` & `otpme-0.3.0a79/otpme/lib/pam.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/pickle.py` & `otpme-0.3.0a79/otpme/lib/pickle.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/pinentry/pinentry.py` & `otpme-0.3.0a79/otpme/lib/pinentry/pinentry.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/pinentry/wrapper.py` & `otpme-0.3.0a79/otpme/lib/pinentry/wrapper.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/pki/cert.py` & `otpme-0.3.0a79/otpme/lib/pki/cert.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/pki/utils.py` & `otpme-0.3.0a79/otpme/lib/pki/utils.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/pki/utils_openssl.py` & `otpme-0.3.0a79/otpme/lib/pki/utils_openssl.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/policy/__init__.py` & `otpme-0.3.0a79/otpme/lib/policy/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/policy/authonaction/authonaction.py` & `otpme-0.3.0a79/otpme/lib/policy/authonaction/authonaction.py`

 * *Files 1% similar despite different names*

```diff
@@ -416,19 +416,20 @@
         # read from config.
         Policy.set_variables(self)
 
     def test(self, force=False, verbose_level=0,
         _caller="API", callback=default_callback):
         """ Test the policy. """
         challenge = stuff.gen_secret(32)
-        status = callback.auth_jwt(reason="authonaction",
-                                    challenge=challenge)
-        if status:
-            return callback.ok("JWT auth succeeded.")
-        return callback.error("JWT auth failed.")
+        try:
+            callback.auth_jwt(reason="authonaction",
+                            challenge=challenge)
+        except OTPmeException as e:
+            return callback.error("JWT auth failed.")
+        return callback.ok("JWT auth succeeded.")
 
     def handle_hook(self, hook_object, hook_name,
         callback=default_callback, **kwargs):
         """ Handle policy hooks. """
         if "interactive" in config.ignore_policy_tags:
             if config.debug_level() > 3:
                 msg = ("AuthonactionPolicy disabled by "
@@ -511,17 +512,18 @@
             do_reauth = False
 
         if do_reauth:
             msg = "You need to re-authenticate for this action."
             callback.send(msg)
             # Verify auth token.
             challenge = stuff.gen_secret(32)
-            verify_status = callback.auth_jwt(reason="authonaction",
-                                                challenge=challenge)
-            if not verify_status:
+            try:
+                callback.auth_jwt(reason="authonaction",
+                                challenge=challenge)
+            except OTPmeException as e:
                 if config.auth_token.uuid in config.first_reauth:
                     config.first_reauth.pop(config.auth_token.uuid)
                 if config.auth_token.uuid in config.last_reauth:
                     config.last_reauth.pop(config.auth_token.uuid)
                 raise self.policy_exception("Authentication failed.")
 
         # Set first re-auth time.
```

### Comparing `otpme-0.3.0a78/otpme/lib/policy/autodisable/autodisable.py` & `otpme-0.3.0a79/otpme/lib/policy/autodisable/autodisable.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/policy/defaultgroups/defaultgroups.py` & `otpme-0.3.0a79/otpme/lib/policy/defaultgroups/defaultgroups.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/policy/defaultpolicies/defaultpolicies.py` & `otpme-0.3.0a79/otpme/lib/policy/defaultpolicies/defaultpolicies.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/policy/defaultroles/defaultroles.py` & `otpme-0.3.0a79/otpme/lib/policy/defaultroles/defaultroles.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/policy/defaultunits/defaultunits.py` & `otpme-0.3.0a79/otpme/lib/policy/defaultunits/defaultunits.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/policy/forcetoken/forcetoken.py` & `otpme-0.3.0a79/otpme/lib/policy/forcetoken/forcetoken.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/policy/get_class.py` & `otpme-0.3.0a79/otpme/lib/policy/get_class.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/policy/idrange/idrange.py` & `otpme-0.3.0a79/otpme/lib/policy/idrange/idrange.py`

 * *Files 1% similar despite different names*

```diff
@@ -375,14 +375,17 @@
                 # Make sure start ID is within ID range.
                 if start_id >= range_start and start_id <= range_end:
                     # If we do not start at range_start we have to restart the
                     # search if no free ID was found between start_id and
                     # range_end.
                     restart_on_end = True
                     new_id = start_id
+                else:
+                    start_id = range_start
+                    new_id = range_start
             if self.verify_new_id or random_range:
                 try:
                     ldif_attribute = "ldif:%s" % attribute
                     msg = ("Searching free ID for attribute: %s" % attribute)
                     logger.debug(msg)
                     new_id = self.find_free_number(object_type=object_type,
                                                     attribute=ldif_attribute,
```

### Comparing `otpme-0.3.0a78/otpme/lib/policy/logintimes/logintimes.py` & `otpme-0.3.0a79/otpme/lib/policy/logintimes/logintimes.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/policy/objecttemplates/objecttemplates.py` & `otpme-0.3.0a79/otpme/lib/policy/objecttemplates/objecttemplates.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/policy/password/password.py` & `otpme-0.3.0a79/otpme/lib/policy/password/password.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/policy/tokenacls/tokenacls.py` & `otpme-0.3.0a79/otpme/lib/policy/tokenacls/tokenacls.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/preload.py` & `otpme-0.3.0a79/otpme/lib/preload.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) 2014 the2nd <the2nd@otpme.org>
 
-# NOTE: This file was auto generated by update_preload.sh at 23.05.2024 18:00:22.
+# NOTE: This file was auto generated by update_preload.sh at 02.06.2024 16:16:18.
 
 from otpme.lib import config
 
 preload_modules = [
     'otpme.lib.arp',
     'otpme.lib.auth_script',
     'otpme.lib.backend',
@@ -33,15 +33,14 @@
     'otpme.lib.classes.data_objects.last_assigned_id',
     'otpme.lib.classes.data_objects.revoked_signature',
     'otpme.lib.classes.data_objects.rsa_key',
     'otpme.lib.classes.data_objects.skip_sync',
     'otpme.lib.classes.data_objects.token_counter',
     'otpme.lib.classes.data_objects.used_hash',
     'otpme.lib.classes.data_objects.used_otp',
-    'otpme.lib.classes.data_objects.used_slp',
     'otpme.lib.classes.data_objects.used_sotp',
     'otpme.lib.classes.dictionary',
     'otpme.lib.classes.group',
     'otpme.lib.classes.host',
     'otpme.lib.classes.login_handler',
     'otpme.lib.classes.mgmt_client',
     'otpme.lib.classes.node',
@@ -80,14 +79,15 @@
     'otpme.lib.compgen',
     'otpme.lib.compression.base',
     'otpme.lib.connections',
     'otpme.lib.daemon.authd',
     'otpme.lib.daemon.clusterd',
     'otpme.lib.daemon.controld',
     'otpme.lib.daemon.hostd',
+    'otpme.lib.daemon.httpd',
     'otpme.lib.daemon.joind',
     'otpme.lib.daemon.mgmtd',
     'otpme.lib.daemon.otpme_daemon',
     'otpme.lib.daemon.scriptd',
     'otpme.lib.daemon.syncd',
     'otpme.lib.debug',
     'otpme.lib.doc',
```

### Comparing `otpme-0.3.0a78/otpme/lib/progress.py` & `otpme-0.3.0a79/otpme/lib/progress.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/protocols/client/__init__.py` & `otpme-0.3.0a79/otpme/lib/protocols/client/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/protocols/client/agent1.py` & `otpme-0.3.0a79/otpme/lib/protocols/client/agent1.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/protocols/client/auth1.py` & `otpme-0.3.0a79/otpme/lib/protocols/client/auth1.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/protocols/client/cluster1.py` & `otpme-0.3.0a79/otpme/lib/protocols/client/cluster1.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,22 +37,23 @@
         command = "ping"
         command_args = {}
         status, \
         status_code, \
         reply = self.connection.send(command, command_args)
         return reply
 
-    def write(self, object_id, object_config,
-        last_used=None, full_data_update=False,
+    def write(self, object_id, object_config, last_used=None,
+        index_journal=None, full_data_update=False,
         full_index_update=False):
         """ Send object to peer. """
         command = "write"
         command_args = {}
         command_args['object_id'] = object_id
         command_args['object_config'] = object_config
+        command_args['index_journal'] = index_journal
         command_args['last_used'] = last_used
         command_args['full_data_update'] = full_data_update
         command_args['full_index_update'] = full_index_update
         status, \
         status_code, \
         reply = self.connection.send(command, command_args)
         if not status:
```

### Comparing `otpme-0.3.0a78/otpme/lib/protocols/client/get_class.py` & `otpme-0.3.0a79/otpme/lib/protocols/client/get_class.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/protocols/client/host1.py` & `otpme-0.3.0a79/otpme/lib/protocols/client/host1.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/protocols/client/join1.py` & `otpme-0.3.0a79/otpme/lib/protocols/client/join1.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/protocols/client/mgmt1.py` & `otpme-0.3.0a79/otpme/lib/protocols/client/mgmt1.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/protocols/client/sync1.py` & `otpme-0.3.0a79/otpme/lib/protocols/client/sync1.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/protocols/otpme_client.py` & `otpme-0.3.0a79/otpme/lib/protocols/otpme_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -3318,16 +3318,18 @@
                 offline_tokens = self.auth_reply['offline_tokens']
                 if offline_tokens:
                     # Get offline session key (e.g. to be forwarded on login redirect).
                     self._offline_token.gen_session_key()
                     #self.offline_session_key = self._offline_token.session_key_public
                     self.offline_session_key = self._offline_token.session_key_private
 
+                # Get SLP for this session.
+                slp = self.auth_reply['slp']
                 # Add login session to agent, handle offline tokens etc.
-                self._add_login_session()
+                self._add_login_session(slp)
 
             elif self.reneg:
                 if reply_message == "AUTH_SESSION_RENEG_START":
                     # Send second auth request with new RSP to finish
                     # renegotiation.
                     command_args['password'] = self.new_rsp
                     status, \
@@ -3513,15 +3515,15 @@
         response = (_("%s response verification successful: %s")
                                 % (peer_type, self.peer.fqdn))
         if config.debug_level(DEBUG_SLOT) > 3:
             self.logger.debug(response)
 
         return response
 
-    def _add_login_session(self):
+    def _add_login_session(self, slp):
         """ Create login session file and add RSP to otpme-agent. """
         # Indicates if we have to cache offline tokens.
         cache_offline_tokens = False
 
         # Set login token to otpme-agent.
         login_token = self.auth_reply['login_token']
         login_pass_type = self.auth_reply['login_pass_type']
@@ -3592,22 +3594,23 @@
         rsp_signature = key.sign(self.rsp, encoding="hex")
 
         # Add RSP to otpme-agent.
         agent_conn = connections.get("agent",
                         user=self.otpme_agent_user)
         try:
             agent_conn.add_rsp(realm=self.realm,
-                                site=self.site,
-                                rsp=self.rsp,
-                                rsp_signature=rsp_signature,
-                                session_key=self.offline_session_key,
-                                login_time=login_time,
-                                timeout=session_timeout,
-                                unused_timeout=session_unused_timeout,
-                                offline=keep_offline_session)
+                            site=self.site,
+                            rsp=self.rsp,
+                            slp=slp,
+                            rsp_signature=rsp_signature,
+                            session_key=self.offline_session_key,
+                            login_time=login_time,
+                            timeout=session_timeout,
+                            unused_timeout=session_unused_timeout,
+                            offline=keep_offline_session)
         except Exception as e:
             msg = ("Error adding RSP to otpme-agent: %s" % e)
             self.logger.critical(msg)
 
         # Create offline session file.
         if keep_offline_session and (cache_offline_tokens or self.offline_session_key):
             # Save RSP to disk. This will be used to add a session to
```

### Comparing `otpme-0.3.0a78/otpme/lib/protocols/otpme_server.py` & `otpme-0.3.0a79/otpme/lib/protocols/otpme_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -1472,17 +1472,14 @@
     #        token = _token
     #        break
 
     #    return token, verify_token
 
     def authenticate_host(self, command, command_args):
         """ Authenticate host/node. """
-        # FIXME: xxx remove!!!
-        self.authenticated = True
-
         if self.peer_challenge:
             try:
                 peer_response = command_args['client_response']
             except:
                 msg = ("Invalid auth command: Missing peer challenge")
                 self.logger.warning(msg)
                 raise OTPmeException("AUTH_INVALID_REQUEST")
```

### Comparing `otpme-0.3.0a78/otpme/lib/protocols/request.py` & `otpme-0.3.0a79/otpme/lib/protocols/request.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/protocols/response.py` & `otpme-0.3.0a79/otpme/lib/protocols/response.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/protocols/server/__init__.py` & `otpme-0.3.0a79/otpme/lib/protocols/server/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/protocols/server/agent1.py` & `otpme-0.3.0a79/otpme/lib/protocols/server/agent1.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 try:
     if os.environ['OTPME_DEBUG_MODULE_LOADING'] == "True":
         print(_("Loading module: %s") % __name__)
 except:
     pass
 
 from otpme.lib import re
-from otpme.lib import slp
 from otpme.lib import srp
 from otpme.lib import json
 from otpme.lib import stuff
 from otpme.lib import config
 from otpme.lib import otpme_pass
 from otpme.lib import multiprocessing
 #from otpme.lib.encoding.base import encode
@@ -684,14 +683,19 @@
                 status = False
             try:
                 rsp = command_args['rsp']
             except:
                 message = "AGENT_INCOMPLETE_COMMAND"
                 status = False
             try:
+                slp = command_args['slp']
+            except:
+                message = "AGENT_INCOMPLETE_COMMAND"
+                status = False
+            try:
                 login_time = float(command_args['login_time'])
             except:
                 message = "AGENT_INCOMPLETE_COMMAND"
                 status = False
             try:
                 session_timeout = int(command_args['timeout'])
             except:
@@ -756,16 +760,15 @@
                 # Add RSP.
                 session['rsp'] = rsp
                 # Gen SRP.
                 rsp_hash = otpme_pass.gen_one_iter_hash(self.login_user, rsp)
                 _srp = srp.gen(rsp_hash)
                 session['srp'] = _srp
                 # Gen SLP.
-                _slp = slp.gen(rsp_hash)
-                session['slp'] = _slp
+                session['slp'] = slp
                 # Add session public key.
                 session['session_key'] = session_key
                 # Add login time.
                 session['login_time'] = login_time
                 # For sessions with offline flag set no logout command
                 # will be sent to the server on agent shutdown etc. to
                 # allow re-use of the session after a reboot.
```

### Comparing `otpme-0.3.0a78/otpme/lib/protocols/server/auth1.py` & `otpme-0.3.0a79/otpme/lib/protocols/server/auth1.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,14 +95,19 @@
 
             if not self.authenticated:
                 message = "Not logged in."
                 status = status_codes.NEED_USER_AUTH
                 self.require_auth = "user"
                 return self.build_response(status, message)
 
+            if config.auth_type != "token":
+                message = "Need token login."
+                status = False
+                return self.build_response(status, message)
+
             # Set proctitle to contain username.
             self.set_proctitle(self.username)
 
             try:
                 jwt_reason = command_args['jwt_reason']
             except:
                 status = False
@@ -144,14 +149,15 @@
                     'realm'             : config.realm,
                     'site'              : config.site,
                     'reason'            : jwt_reason,
                     'message'           : "JWT signed by authd.",
                     'challenge'         : jwt_challenge,
                     'login_time'        : time.time(),
                     'login_token'       : config.auth_token.uuid,
+                    'auth_type'         : config.auth_type,
                     'accessgroup'       : jwt_accessgroup,
                     }
 
             _jwt = jwt.encode(payload=jwt_data, key=sign_key, algorithm='RS256')
 
             msg = ("Sigend JWT: user=%s token=%s access_group=%s, reason=%s"
                     % (self.username, config.auth_token.name,
```

### Comparing `otpme-0.3.0a78/otpme/lib/protocols/server/cluster1.py` & `otpme-0.3.0a79/otpme/lib/protocols/server/cluster1.py`

 * *Files 2% similar despite different names*

```diff
@@ -360,14 +360,19 @@
                 status = False
             try:
                 object_config = command_args['object_config']
             except:
                 message = "Missing object config."
                 status = False
             try:
+                index_journal = command_args['index_journal']
+            except:
+                message = "Missing index journal."
+                status = False
+            try:
                 last_used = command_args['last_used']
             except:
                 last_used = None
             try:
                 full_data_update = command_args['full_data_update']
             except:
                 full_data_update = False
@@ -376,16 +381,15 @@
             except:
                 full_index_update = False
             if config.daemon_shutdown:
                 message = "Daemon shutdown."
                 status = False
             if status:
                 object_checksum = object_config['CHECKSUM']
-                msg = ("Writing object (node:%s): %s (%s)"
-                    % (self.peer.name, object_id, object_checksum))
+                msg = ("Writing object: %s (%s)" % (object_id, object_checksum))
                 logger.debug(msg)
                 message = "done"
                 while True:
                     entry_time = str(time.time_ns())
                     cluster_journal_file = os.path.join(config.cluster_in_journal_dir, entry_time)
                     if os.path.exists(cluster_journal_file):
                         continue
@@ -394,14 +398,15 @@
                 object_config = object_config.encrypt(config.master_key,
                                                     update_checksums=False)
                 object_data = {
                                 'action'            : 'write',
                                 'object_id'         : object_id,
                                 'last_used'         : last_used,
                                 'object_config'     : object_config,
+                                'index_journal'     : index_journal,
                                 'full_data_update'  : full_data_update,
                                 'full_index_update' : full_index_update,
                             }
                 file_content = ujson.dumps(object_data)
                 try:
                     filetools.create_file(path=cluster_journal_file,
                                             content=file_content,
```

### Comparing `otpme-0.3.0a78/otpme/lib/protocols/server/get_class.py` & `otpme-0.3.0a79/otpme/lib/protocols/server/get_class.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/protocols/server/host1.py` & `otpme-0.3.0a79/otpme/lib/protocols/server/host1.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/protocols/server/join1.py` & `otpme-0.3.0a79/otpme/lib/protocols/server/join1.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/protocols/server/mgmt1.py` & `otpme-0.3.0a79/otpme/lib/protocols/server/mgmt1.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/protocols/server/sync1.py` & `otpme-0.3.0a79/otpme/lib/protocols/server/sync1.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/protocols/status_codes.py` & `otpme-0.3.0a79/otpme/lib/protocols/status_codes.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/protocols/utils.py` & `otpme-0.3.0a79/otpme/lib/protocols/utils.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/push_script.py` & `otpme-0.3.0a79/otpme/lib/push_script.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/qrcode.py` & `otpme-0.3.0a79/otpme/lib/qrcode.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/register/__init__.py` & `otpme-0.3.0a79/otpme/lib/register/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 modules = [
 	#'otpme.lib.classes.data_objects.failed_pass',
 	#'otpme.lib.classes.data_objects.last_assigned_id',
 	#'otpme.lib.classes.data_objects.revoked_signature',
 	#'otpme.lib.classes.data_objects.token_counter',
 	#'otpme.lib.classes.data_objects.used_hash',
 	#'otpme.lib.classes.data_objects.used_otp',
-	#'otpme.lib.classes.data_objects.used_slp',
 	#'otpme.lib.classes.data_objects.used_sotp',
 	#'otpme.lib.classes.data_objects.rsa_key',
 	#'otpme.lib.classes.data_objects.cert',
 	#'otpme.lib.classes.accessgroup',
 	#'otpme.lib.classes.ca',
 	#'otpme.lib.classes.client',
 	#'otpme.lib.classes.dictionary',
```

### Comparing `otpme-0.3.0a78/otpme/lib/resolver/get_class.py` & `otpme-0.3.0a79/otpme/lib/resolver/get_class.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/resolver/ldap/ldap.py` & `otpme-0.3.0a79/otpme/lib/resolver/ldap/ldap.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/script.py` & `otpme-0.3.0a79/otpme/lib/script.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/sign_key_cache.py` & `otpme-0.3.0a79/otpme/lib/sign_key_cache.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/slp.py` & `otpme-0.3.0a79/otpme/lib/slp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/smartcard/__init__.py` & `otpme-0.3.0a79/otpme/lib/smartcard/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/smartcard/fido2/fido2.py` & `otpme-0.3.0a79/otpme/lib/smartcard/fido2/fido2.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/smartcard/get_class.py` & `otpme-0.3.0a79/otpme/lib/smartcard/get_class.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/smartcard/utils.py` & `otpme-0.3.0a79/otpme/lib/smartcard/utils.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/smartcard/yubikey/deploy.py` & `otpme-0.3.0a79/otpme/lib/smartcard/yubikey/deploy.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/smartcard/yubikey/usb.py` & `otpme-0.3.0a79/otpme/lib/smartcard/yubikey/usb.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/smartcard/yubikey/yubikey.py` & `otpme-0.3.0a79/otpme/lib/smartcard/yubikey/yubikey.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/smartcard/yubikey_gpg/yubikey_gpg.py` & `otpme-0.3.0a79/otpme/lib/smartcard/yubikey_gpg/yubikey_gpg.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/smartcard/yubikey_hmac/yubikey_hmac.py` & `otpme-0.3.0a79/otpme/lib/smartcard/yubikey_hmac/yubikey_hmac.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/smartcard/yubikey_hotp/yubikey_hotp.py` & `otpme-0.3.0a79/otpme/lib/smartcard/yubikey_hotp/yubikey_hotp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/socket/connect.py` & `otpme-0.3.0a79/otpme/lib/socket/connect.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) 2014 the2nd <the2nd@otpme.org>
 import os
 import ssl
+import signal
 import socket
+import threading
 
 try:
     if os.environ['OTPME_DEBUG_MODULE_LOADING'] == "True":
         print(_("Loading module: %s") % __name__)
 except:
     pass
 
@@ -33,14 +35,19 @@
         self.key_file = None
         self.key_pass = None
         self.cert_file = None
         self.ca_data_file = None
         self.connected = False
         self.logger = config.logger
 
+        is_main_thread = isinstance(threading.current_thread(), threading._MainThread)
+        if is_main_thread:
+            signal.signal(signal.SIGTERM, self.signal_handler)
+            signal.signal(signal.SIGINT, self.signal_handler)
+
         # Handle unix sockets.
         if self.socket_uri.startswith("socket://"):
             # Get protocol.
             self.protocol = re.sub('^([^:]*):.*$', r'\1', self.socket_uri)
             # Get unix socket path.
             self.socket = re.sub('^socket://(.*)', r'\1', self.socket_uri)
 
@@ -166,14 +173,20 @@
         else:
             self.socket_handler = socket_handler("client", self._socket)
 
     def __getattr__(self, name):
         """ Map to original methods. """
         return getattr(self._socket, name)
 
+    def signal_handler(self, _signal, frame):
+        """ Handle signals """
+        if _signal != 15:
+            return
+        self.remove_cert_files()
+
     def connect(self, timeout=15, connect_timeout=3, quiet=False, **kwargs):
         """ Connect to remote socket and read first packet. """
         if self.connected:
             msg = "Already connected: %s" % self.socket_uri
             raise AlreadyConnected(msg)
         if timeout is None:
             timeout_msg = "None"
@@ -310,17 +323,18 @@
             msg = (_("Error receiving data: %s") % e)
             config.raise_exception()
             raise ConnectionError(msg)
         return data
 
     def remove_cert_files(self):
         """ Remove temporary SSL cert/key files. """
-        if self.cert_file and self.key_file:
+        if self.cert_file:
             if os.path.exists(self.cert_file):
                 os.remove(self.cert_file)
+        if self.key_file:
             if os.path.exists(self.key_file):
                 os.remove(self.key_file)
         if self.ca_data_file:
             if os.path.exists(self.ca_data_file):
                 os.remove(self.ca_data_file)
 
     def close(self):
```

### Comparing `otpme-0.3.0a78/otpme/lib/socket/handler.py` & `otpme-0.3.0a79/otpme/lib/socket/handler.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/socket/listen.py` & `otpme-0.3.0a79/otpme/lib/socket/listen.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/socket/send_recv1.py` & `otpme-0.3.0a79/otpme/lib/socket/send_recv1.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/sotp.py` & `otpme-0.3.0a79/otpme/lib/sotp.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,15 +43,16 @@
                             salt=salt,
                             iterations=1,
                             quiet=True)
     rsp = result['hash'][0:rsp_len]
     return rsp
 
 def verify(password_hash, epoch_time=None, validity_range=None, reneg=False,
-    password=None, challenge=None, response=None, sotp_len=None):
+    password=None, challenge=None, response=None,
+    sotp_len=None, access_group=None):
     """ Verify session OTP. """
     if sotp_len is None:
         sotp_len = config.sotp_len
 
     if not epoch_time:
         # Get epoch time (10 second timestep).
         epoch_time = int(str(int(time.time()))[:-1])
@@ -65,14 +66,16 @@
         # Get epoch time that honors timedrift values.
         epoch_time = validity_times[0]
         validity_range = validity_times[1]
 
     # Check for renegotiation OTP if needed
     if reneg:
         secret = "RENEG:%s" % password_hash
+    elif access_group:
+        secret = "%s:%s" % (access_group, password_hash)
     else:
         secret = password_hash
 
     # If we got a password from a clear-text request we have to verify it
     # against all possible SOTPs for the given validity range.
     if password:
         for o in otpme.generate(epoch_time=epoch_time, secret=secret,
@@ -89,16 +92,16 @@
             mschap_verify_status, nt_key = mschap_util.verify(o_hash,
                                                             challenge,
                                                             response)
             if mschap_verify_status:
                 return mschap_verify_status, nt_key, o, o_hash
         return False, None, None, None
 
-def gen(epoch_time=None, password_hash=None,
-    sotp_len=None, reneg=False, rsp_hash_type=None):
+def gen(epoch_time=None, password_hash=None, sotp_len=None,
+    reneg=False, rsp_hash_type=None, access_group=None):
     """ Generate session OTP. """
     if not epoch_time:
         # get epoch time (10 second timestep)
         epoch_time = int(str(int(time.time()))[:-1])
 
     if sotp_len is None:
         sotp_len = config.sotp_len
@@ -106,14 +109,16 @@
     # Generate renegotiation OTP if needed.
     if reneg:
         if not rsp_hash_type:
             msg = "Need <rsp_hash_type>."
             raise OTPmeException(msg)
         secret = "RENEG:%s" % password_hash
         reneg_salt = stuff.gen_secret(32)
+    elif access_group:
+        secret = "%s:%s" % (access_group, password_hash)
     else:
         secret = password_hash
 
     # Generate OTP.
     otp = otpme.generate(epoch_time=epoch_time, secret=secret,
                             otp_count=1, otp_len=sotp_len)
     if reneg:
```

### Comparing `otpme-0.3.0a78/otpme/lib/spsc.py` & `otpme-0.3.0a79/otpme/lib/spsc.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/srp.py` & `otpme-0.3.0a79/otpme/lib/srp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/ssh.py` & `otpme-0.3.0a79/otpme/lib/ssh.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/stuff.py` & `otpme-0.3.0a79/otpme/lib/stuff.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/sync_cache.py` & `otpme-0.3.0a79/otpme/lib/sync_cache.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/system_command.py` & `otpme-0.3.0a79/otpme/lib/system_command.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/third_party/dogpile_caching/__init__.py` & `otpme-0.3.0a79/otpme/lib/third_party/dogpile_caching/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/third_party/dogpile_caching/advanced.py` & `otpme-0.3.0a79/otpme/lib/third_party/dogpile_caching/advanced.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/third_party/dogpile_caching/caching_query.py` & `otpme-0.3.0a79/otpme/lib/third_party/dogpile_caching/caching_query.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/third_party/dogpile_caching/environment.py` & `otpme-0.3.0a79/otpme/lib/third_party/dogpile_caching/environment.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/third_party/dogpile_caching/fixture_data.py` & `otpme-0.3.0a79/otpme/lib/third_party/dogpile_caching/fixture_data.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/third_party/dogpile_caching/helloworld.py` & `otpme-0.3.0a79/otpme/lib/third_party/dogpile_caching/helloworld.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/third_party/dogpile_caching/local_session_caching.py` & `otpme-0.3.0a79/otpme/lib/third_party/dogpile_caching/local_session_caching.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/third_party/dogpile_caching/model.py` & `otpme-0.3.0a79/otpme/lib/third_party/dogpile_caching/model.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/third_party/dogpile_caching/relationship_caching.py` & `otpme-0.3.0a79/otpme/lib/third_party/dogpile_caching/relationship_caching.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/third_party/nss_cache/__init__.py` & `otpme-0.3.0a79/otpme/lib/third_party/nss_cache/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/third_party/nss_cache/caches/caches.py` & `otpme-0.3.0a79/otpme/lib/third_party/nss_cache/caches/caches.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/third_party/nss_cache/caches/files.py` & `otpme-0.3.0a79/otpme/lib/third_party/nss_cache/caches/files.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/third_party/nss_cache/config.py` & `otpme-0.3.0a79/otpme/lib/third_party/nss_cache/config.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/third_party/nss_cache/error.py` & `otpme-0.3.0a79/otpme/lib/third_party/nss_cache/error.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/third_party/nss_cache/lock.py` & `otpme-0.3.0a79/otpme/lib/third_party/nss_cache/lock.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/third_party/nss_cache/maps/group.py` & `otpme-0.3.0a79/otpme/lib/third_party/nss_cache/maps/group.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/third_party/nss_cache/maps/maps.py` & `otpme-0.3.0a79/otpme/lib/third_party/nss_cache/maps/maps.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/third_party/nss_cache/maps/passwd.py` & `otpme-0.3.0a79/otpme/lib/third_party/nss_cache/maps/passwd.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/third_party/nss_cache/maps/shadow.py` & `otpme-0.3.0a79/otpme/lib/third_party/nss_cache/maps/shadow.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/third_party/nss_cache/nss.py` & `otpme-0.3.0a79/otpme/lib/third_party/nss_cache/nss.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/third_party/nss_cache/update/files_updater.py` & `otpme-0.3.0a79/otpme/lib/third_party/nss_cache/update/files_updater.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/third_party/nss_cache/update/map_updater.py` & `otpme-0.3.0a79/otpme/lib/third_party/nss_cache/update/map_updater.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/third_party/nss_cache/update/updater.py` & `otpme-0.3.0a79/otpme/lib/third_party/nss_cache/update/updater.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/third_party/nss_cache/util/file_formats.py` & `otpme-0.3.0a79/otpme/lib/third_party/nss_cache/util/file_formats.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/third_party/oath_toolkit/_compat.py` & `otpme-0.3.0a79/otpme/lib/third_party/oath_toolkit/_compat.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/third_party/oath_toolkit/uri.py` & `otpme-0.3.0a79/otpme/lib/third_party/oath_toolkit/uri.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/token/__init__.py` & `otpme-0.3.0a79/otpme/lib/token/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/token/fido2/fido2.py` & `otpme-0.3.0a79/otpme/lib/token/fido2/fido2.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/token/get_class.py` & `otpme-0.3.0a79/otpme/lib/token/get_class.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/token/hotp/hotp.py` & `otpme-0.3.0a79/otpme/lib/token/hotp/hotp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/token/link/link.py` & `otpme-0.3.0a79/otpme/lib/token/link/link.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/token/motp/motp.py` & `otpme-0.3.0a79/otpme/lib/token/motp/motp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/token/oath/oath.py` & `otpme-0.3.0a79/otpme/lib/token/oath/oath.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/token/otp_push/otp_push.py` & `otpme-0.3.0a79/otpme/lib/token/otp_push/otp_push.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/token/otpme/otpme.py` & `otpme-0.3.0a79/otpme/lib/token/otpme/otpme.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/token/password/password.py` & `otpme-0.3.0a79/otpme/lib/token/password/password.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/token/script_otp/script_otp.py` & `otpme-0.3.0a79/otpme/lib/token/script_otp/script_otp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/token/script_static/script_static.py` & `otpme-0.3.0a79/otpme/lib/token/script_static/script_static.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/token/ssh/ssh.py` & `otpme-0.3.0a79/otpme/lib/token/ssh/ssh.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/token/totp/totp.py` & `otpme-0.3.0a79/otpme/lib/token/totp/totp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme/lib/token/yubikey_hmac/yubikey_hmac.py` & `otpme-0.3.0a79/otpme/lib/token/yubikey_hmac/yubikey_hmac.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme.egg-info/PKG-INFO` & `otpme-0.3.0a79/otpme.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otpme
-Version: 0.3.0a78
+Version: 0.3.0a79
 Summary: OTPme: A flexible One-Time-Password system
 Author-email: The2nd <the2nd@otpme.org>
 Maintainer-email: The2nd <the2nd@otpme.org>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
@@ -740,14 +740,18 @@
 Requires-Dist: pycryptodome>=3.4.3
 Requires-Dist: PyQRCode>=1.2.1
 Requires-Dist: pyre2>=0.3.6
 Requires-Dist: lz4>=4.3.2
 Requires-Dist: termcolor>=1.1.0
 Requires-Dist: radius-eap-mschapv2-client>=1.0.6
 Requires-Dist: pyrad>=2.4
+Requires-Dist: Flask>=3.0.3
+Requires-Dist: Flask-Login>=0.6.3
+Requires-Dist: Flask-WTF>=1.2.1
+Requires-Dist: gevent>=24.2.1
 
 # Installation instructions
 
 ## Install debian dependencies
 apt-get install python3.11-venv gobjc++ python3-pybind11 python3-dev build-essential cmake gcc dbus-x11 freeradius libacl1-dev libnss-cache liboath0 liboath-dev libpcsclite1 libpq-dev libre2-9 libre2-dev libsystemd-dev pkg-config postgresql postgresql-server-dev-all pwgen pyflakes3 redis redis-server redis-tools
 
 ### Disable installed services
```

### Comparing `otpme-0.3.0a78/otpme.egg-info/SOURCES.txt` & `otpme-0.3.0a79/otpme.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -144,15 +144,14 @@
 otpme/lib/classes/data_objects/last_assigned_id.py
 otpme/lib/classes/data_objects/revoked_signature.py
 otpme/lib/classes/data_objects/rsa_key.py
 otpme/lib/classes/data_objects/skip_sync.py
 otpme/lib/classes/data_objects/token_counter.py
 otpme/lib/classes/data_objects/used_hash.py
 otpme/lib/classes/data_objects/used_otp.py
-otpme/lib/classes/data_objects/used_slp.py
 otpme/lib/classes/data_objects/used_sotp.py
 otpme/lib/cli/__init__.py
 otpme/lib/cli/accessgroup.py
 otpme/lib/cli/ca.py
 otpme/lib/cli/client.py
 otpme/lib/cli/dictionary.py
 otpme/lib/cli/group.py
@@ -170,14 +169,15 @@
 otpme/lib/compression/__init__.py
 otpme/lib/compression/base.py
 otpme/lib/daemon/__init__.py
 otpme/lib/daemon/authd.py
 otpme/lib/daemon/clusterd.py
 otpme/lib/daemon/controld.py
 otpme/lib/daemon/hostd.py
+otpme/lib/daemon/httpd.py
 otpme/lib/daemon/joind.py
 otpme/lib/daemon/ldapd.py
 otpme/lib/daemon/mgmtd.py
 otpme/lib/daemon/otpme_daemon.py
 otpme/lib/daemon/scriptd.py
 otpme/lib/daemon/syncd.py
 otpme/lib/daemon/unix_daemon.py
```

### Comparing `otpme-0.3.0a78/otpme.egg-info/entry_points.txt` & `otpme-0.3.0a79/otpme.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/otpme.egg-info/requires.txt` & `otpme-0.3.0a79/otpme.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -51,7 +51,11 @@
 pycryptodome>=3.4.3
 PyQRCode>=1.2.1
 pyre2>=0.3.6
 lz4>=4.3.2
 termcolor>=1.1.0
 radius-eap-mschapv2-client>=1.0.6
 pyrad>=2.4
+Flask>=3.0.3
+Flask-Login>=0.6.3
+Flask-WTF>=1.2.1
+gevent>=24.2.1
```

### Comparing `otpme-0.3.0a78/pyproject.toml` & `otpme-0.3.0a79/pyproject.toml`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a78/requirements.txt` & `otpme-0.3.0a79/requirements.txt`

 * *Files 8% similar despite different names*

```diff
@@ -63,12 +63,16 @@
 pyre2>=0.3.6
 lz4>=4.3.2
 #re2>=0.2.22
 #systemd>=0.16.1
 termcolor>=1.1.0
 radius-eap-mschapv2-client>=1.0.6
 pyrad>=2.4
+Flask>=3.0.3
+Flask-Login>=0.6.3
+Flask-WTF>=1.2.1
+gevent>=24.2.1
 #py-radius>=2.0.2.post1
 # apt-get install libffi-dev libssl-dev
 # For use with U2F token (client site only).
 #hidapi>=0.7.99.post8
 #python-u2flib-host>=3.0.0
```

### Comparing `otpme-0.3.0a78/setup.py` & `otpme-0.3.0a79/setup.py`

 * *Files identical despite different names*

