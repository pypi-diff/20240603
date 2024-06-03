# Comparing `tmp/pypgstac-0.8.6.tar.gz` & `tmp/pypgstac-0.9.0.tar.gz`

## Comparing `pypgstac-0.8.6.tar` & `pypgstac-0.9.0.tar`

### file list

```diff
@@ -1,139 +1,139 @@
--rw-r--r--   0        0        0      344 1970-01-01 00:00:00.000000 pypgstac-0.8.6/Cargo.toml
--rw-r--r--   0     1001      127       49 2024-06-03 14:22:31.000000 pypgstac-0.8.6/README.md
--rw-r--r--   0     1001      127       92 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/__init__.py
--rw-r--r--   0     1001      127     9695 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/db.py
--rw-r--r--   0     1001      127     5601 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/hydration.py
--rw-r--r--   0     1001      127    26025 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/load.py
--rw-r--r--   0     1001      127     5453 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrate.py
--rw-r--r--   0     1001      127       86 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.1.9-0.2.3.sql
--rw-r--r--   0     1001      127    35445 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.1.9.sql
--rw-r--r--   0     1001      127       86 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.2.3-0.2.4.sql
--rw-r--r--   0     1001      127    35445 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.2.3.sql
--rw-r--r--   0     1001      127     7132 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.2.4-0.2.5.sql
--rw-r--r--   0     1001      127     8816 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.2.4-0.2.7.sql
--rw-r--r--   0     1001      127    35445 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.2.4.sql
--rw-r--r--   0     1001      127     1783 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.2.5-0.2.7.sql
--rw-r--r--   0     1001      127    35570 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.2.5.sql
--rw-r--r--   0     1001      127      103 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.2.7-0.2.8.sql
--rw-r--r--   0     1001      127    35570 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.2.7.sql
--rw-r--r--   0     1001      127       86 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.2.8-0.2.9.sql
--rw-r--r--   0     1001      127    30676 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.2.8.sql
--rw-r--r--   0     1001      127    48852 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.2.9-0.3.0.sql
--rw-r--r--   0     1001      127    30676 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.2.9.sql
--rw-r--r--   0     1001      127      732 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.3.0-0.3.1.sql
--rw-r--r--   0     1001      127    48316 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.3.0.sql
--rw-r--r--   0     1001      127     1692 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.3.1-0.3.2.sql
--rw-r--r--   0     1001      127    48318 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.3.1.sql
--rw-r--r--   0     1001      127    10974 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.3.2-0.3.3.sql
--rw-r--r--   0     1001      127    48321 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.3.2.sql
--rw-r--r--   0     1001      127     6266 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.3.3-0.3.4.sql
--rw-r--r--   0     1001      127    49082 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.3.3.sql
--rw-r--r--   0     1001      127    28806 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.3.4-0.3.5.sql
--rw-r--r--   0     1001      127    55504 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.3.4.sql
--rw-r--r--   0     1001      127    14273 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.3.5-0.3.6.sql
--rw-r--r--   0     1001      127    66800 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.3.5.sql
--rw-r--r--   0     1001      127    28561 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.3.6-0.4.0.sql
--rw-r--r--   0     1001      127    68520 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.3.6.sql
--rw-r--r--   0     1001      127     5517 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.4.0-0.4.1.sql
--rw-r--r--   0     1001      127    75093 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.4.0.sql
--rw-r--r--   0     1001      127     5773 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.4.1-0.4.2.sql
--rw-r--r--   0     1001      127    75572 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.4.1.sql
--rw-r--r--   0     1001      127     4725 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.4.2-0.4.3.sql
--rw-r--r--   0     1001      127    75821 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.4.2.sql
--rw-r--r--   0     1001      127    16274 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.4.3-0.4.4.sql
--rw-r--r--   0     1001      127    75829 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.4.3.sql
--rw-r--r--   0     1001      127     8986 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.4.4-0.4.5.sql
--rw-r--r--   0     1001      127    77866 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.4.4.sql
--rw-r--r--   0     1001      127    87157 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.4.5-0.5.0.sql
--rw-r--r--   0     1001      127    77907 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.4.5.sql
--rw-r--r--   0     1001      127     6474 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.5.0-0.5.1.sql
--rw-r--r--   0     1001      127    86941 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.5.0.sql
--rw-r--r--   0     1001      127    23595 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.5.1-0.6.0.sql
--rw-r--r--   0     1001      127    88071 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.5.1.sql
--rw-r--r--   0     1001      127      314 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.6.0-0.6.1.sql
--rw-r--r--   0     1001      127    91221 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.6.0.sql
--rw-r--r--   0     1001      127       64 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.6.1-0.6.2.sql
--rw-r--r--   0     1001      127    91293 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.6.1.sql
--rw-r--r--   0     1001      127     2395 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.6.10-0.6.11.sql
--rw-r--r--   0     1001      127    97746 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.6.10.sql
--rw-r--r--   0     1001      127    23983 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.6.11-0.6.12.sql
--rw-r--r--   0     1001      127    97746 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.6.11.sql
--rw-r--r--   0     1001      127     6177 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.6.12-0.6.13.sql
--rw-r--r--   0     1001      127   109293 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.6.12.sql
--rw-r--r--   0     1001      127    62266 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.6.13-0.7.0.sql
--rw-r--r--   0     1001      127    71093 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.6.13-0.7.3.sql
--rw-r--r--   0     1001      127   109390 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.6.13.sql
--rw-r--r--   0     1001      127      512 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.6.2-0.6.3.sql
--rw-r--r--   0     1001      127    91293 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.6.2.sql
--rw-r--r--   0     1001      127     5310 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.6.3-0.6.4.sql
--rw-r--r--   0     1001      127    91293 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.6.3.sql
--rw-r--r--   0     1001      127     4869 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.6.4-0.6.5.sql
--rw-r--r--   0     1001      127    92207 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.6.4.sql
--rw-r--r--   0     1001      127     6513 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.6.5-0.6.6.sql
--rw-r--r--   0     1001      127    92729 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.6.5.sql
--rw-r--r--   0     1001      127     5879 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.6.6-0.6.7.sql
--rw-r--r--   0     1001      127    93392 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.6.6.sql
--rw-r--r--   0     1001      127    10806 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.6.7-0.6.8.sql
--rw-r--r--   0     1001      127    93421 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.6.7.sql
--rw-r--r--   0     1001      127     6043 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.6.8-0.6.9.sql
--rw-r--r--   0     1001      127    97125 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.6.8.sql
--rw-r--r--   0     1001      127     1323 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.6.9-0.6.10.sql
--rw-r--r--   0     1001      127    97247 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.6.9.sql
--rw-r--r--   0     1001      127    25596 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.7.0-0.7.1.sql
--rw-r--r--   0     1001      127   124336 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.7.0.sql
--rw-r--r--   0     1001      127    12904 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.7.1-0.7.2.sql
--rw-r--r--   0     1001      127   128215 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.7.1.sql
--rw-r--r--   0     1001      127    15709 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.7.10-0.8.0.sql
--rw-r--r--   0     1001      127   136758 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.7.10.sql
--rw-r--r--   0     1001      127    14951 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.7.2-0.7.3.sql
--rw-r--r--   0     1001      127   129127 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.7.2.sql
--rw-r--r--   0     1001      127    25457 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.7.3-0.7.4.sql
--rw-r--r--   0     1001      127   128574 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.7.3.sql
--rw-r--r--   0     1001      127    35126 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.7.4-0.7.5.sql
--rw-r--r--   0     1001      127   132836 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.7.4.sql
--rw-r--r--   0     1001      127     9377 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.7.5-0.7.6.sql
--rw-r--r--   0     1001      127   135013 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.7.5.sql
--rw-r--r--   0     1001      127    14610 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.7.6-0.7.7.sql
--rw-r--r--   0     1001      127   135026 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.7.6.sql
--rw-r--r--   0     1001      127     8604 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.7.7-0.7.8.sql
--rw-r--r--   0     1001      127   136049 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.7.7.sql
--rw-r--r--   0     1001      127     6841 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.7.8-0.7.9.sql
--rw-r--r--   0     1001      127   136073 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.7.8.sql
--rw-r--r--   0     1001      127     8132 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.7.9-0.7.10.sql
--rw-r--r--   0     1001      127   136073 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.7.9.sql
--rw-r--r--   0     1001      127     7760 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.8.0-0.8.1.sql
--rw-r--r--   0     1001      127   137625 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.8.0.sql
--rw-r--r--   0     1001      127    46866 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.8.1-0.8.2.sql
--rw-r--r--   0     1001      127   137625 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.8.1.sql
--rw-r--r--   0     1001      127    12488 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.8.2-0.8.3.sql
--rw-r--r--   0     1001      127   146813 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.8.2.sql
--rw-r--r--   0     1001      127     9716 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.8.3-0.8.4.sql
--rw-r--r--   0     1001      127   147162 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.8.3.sql
--rw-r--r--   0     1001      127    15676 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.8.4-0.8.5.sql
--rw-r--r--   0     1001      127   147162 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.8.4.sql
--rw-r--r--   0     1001      127     9716 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.8.5-0.8.6.sql
--rw-r--r--   0     1001      127   147174 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.8.5.sql
--rw-r--r--   0     1001      127   147174 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.8.6.sql
--rw-r--r--   0     1001      127        0 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/py.typed
--rw-r--r--   0     1001      127     3588 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/pypgstac.py
--rw-r--r--   0     1001      127       37 2024-06-03 14:22:31.000000 pypgstac-0.8.6/python/pypgstac/version.py
--rw-r--r--   0     1001      127     2437 2024-06-03 14:22:31.000000 pypgstac-0.8.6/src/lib.rs
--rw-r--r--   0     1001      127        0 2024-06-03 14:22:31.000000 pypgstac-0.8.6/tests/__init__.py
--rw-r--r--   0     1001      127     2173 2024-06-03 14:22:31.000000 pypgstac-0.8.6/tests/conftest.py
--rw-r--r--   0     1001      127     6737 2024-06-03 14:22:31.000000 pypgstac-0.8.6/tests/data-files/hydration/collections/chloris-biomass.json
--rw-r--r--   0     1001      127     9009 2024-06-03 14:22:31.000000 pypgstac-0.8.6/tests/data-files/hydration/collections/landsat-c2-l1.json
--rw-r--r--   0     1001      127    12629 2024-06-03 14:22:31.000000 pypgstac-0.8.6/tests/data-files/hydration/collections/sentinel-1-grd.json
--rw-r--r--   0     1001      127    11473 2024-06-03 14:22:31.000000 pypgstac-0.8.6/tests/data-files/hydration/dehydrated-items/landsat-c2-l1/LM04_L1GS_001001_19830527_02_T2.json
--rw-r--r--   0     1001      127    14310 2024-06-03 14:22:31.000000 pypgstac-0.8.6/tests/data-files/hydration/raw-items/landsat-c2-l1/LM04_L1GS_001001_19830527_02_T2.json
--rw-r--r--   0     1001      127    10925 2024-06-03 14:22:31.000000 pypgstac-0.8.6/tests/data-files/hydration/raw-items/sentinel-1-grd/S1A_IW_GRDH_1SDV_20220428T034417_20220428T034442_042968_05213C.json
--rw-r--r--   0     1001      127     4992 2024-06-03 14:22:31.000000 pypgstac-0.8.6/tests/data-files/load/dehydrated.txt
--rw-r--r--   0     1001      127        0 2024-06-03 14:22:31.000000 pypgstac-0.8.6/tests/hydration/__init__.py
--rw-r--r--   0     1001      127      893 2024-06-03 14:22:31.000000 pypgstac-0.8.6/tests/hydration/test_base_item.py
--rw-r--r--   0     1001      127     9044 2024-06-03 14:22:31.000000 pypgstac-0.8.6/tests/hydration/test_dehydrate.py
--rw-r--r--   0     1001      127     1241 2024-06-03 14:22:31.000000 pypgstac-0.8.6/tests/hydration/test_dehydrate_pg.py
--rw-r--r--   0     1001      127     7687 2024-06-03 14:22:31.000000 pypgstac-0.8.6/tests/hydration/test_hydrate.py
--rw-r--r--   0     1001      127     1258 2024-06-03 14:22:31.000000 pypgstac-0.8.6/tests/hydration/test_hydrate_pg.py
--rw-r--r--   0     1001      127    11887 2024-06-03 14:22:31.000000 pypgstac-0.8.6/tests/test_load.py
--rw-r--r--   0     1001      127     7636 2024-06-03 14:22:31.000000 pypgstac-0.8.6/Cargo.lock
--rw-r--r--   0     1001      127     3051 2024-06-03 14:22:31.000000 pypgstac-0.8.6/pyproject.toml
--rw-r--r--   0        0        0     2332 1970-01-01 00:00:00.000000 pypgstac-0.8.6/PKG-INFO
+-rw-r--r--   0        0        0      357 1970-01-01 00:00:00.000000 pypgstac-0.9.0/Cargo.toml
+-rw-r--r--   0     1001      127       49 2024-04-30 19:01:24.000000 pypgstac-0.9.0/README.md
+-rw-r--r--   0     1001      127       92 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/__init__.py
+-rw-r--r--   0     1001      127     9695 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/db.py
+-rw-r--r--   0     1001      127     5601 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/hydration.py
+-rw-r--r--   0     1001      127    26025 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/load.py
+-rw-r--r--   0     1001      127     5453 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrate.py
+-rw-r--r--   0     1001      127       86 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.1.9-0.2.3.sql
+-rw-r--r--   0     1001      127    35445 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.1.9.sql
+-rw-r--r--   0     1001      127       86 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.2.3-0.2.4.sql
+-rw-r--r--   0     1001      127    35445 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.2.3.sql
+-rw-r--r--   0     1001      127     7132 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.2.4-0.2.5.sql
+-rw-r--r--   0     1001      127     8816 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.2.4-0.2.7.sql
+-rw-r--r--   0     1001      127    35445 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.2.4.sql
+-rw-r--r--   0     1001      127     1783 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.2.5-0.2.7.sql
+-rw-r--r--   0     1001      127    35570 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.2.5.sql
+-rw-r--r--   0     1001      127      103 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.2.7-0.2.8.sql
+-rw-r--r--   0     1001      127    35570 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.2.7.sql
+-rw-r--r--   0     1001      127       86 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.2.8-0.2.9.sql
+-rw-r--r--   0     1001      127    30676 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.2.8.sql
+-rw-r--r--   0     1001      127    48852 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.2.9-0.3.0.sql
+-rw-r--r--   0     1001      127    30676 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.2.9.sql
+-rw-r--r--   0     1001      127      732 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.3.0-0.3.1.sql
+-rw-r--r--   0     1001      127    48316 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.3.0.sql
+-rw-r--r--   0     1001      127     1692 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.3.1-0.3.2.sql
+-rw-r--r--   0     1001      127    48318 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.3.1.sql
+-rw-r--r--   0     1001      127    10974 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.3.2-0.3.3.sql
+-rw-r--r--   0     1001      127    48321 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.3.2.sql
+-rw-r--r--   0     1001      127     6266 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.3.3-0.3.4.sql
+-rw-r--r--   0     1001      127    49082 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.3.3.sql
+-rw-r--r--   0     1001      127    28806 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.3.4-0.3.5.sql
+-rw-r--r--   0     1001      127    55504 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.3.4.sql
+-rw-r--r--   0     1001      127    14273 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.3.5-0.3.6.sql
+-rw-r--r--   0     1001      127    66800 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.3.5.sql
+-rw-r--r--   0     1001      127    28561 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.3.6-0.4.0.sql
+-rw-r--r--   0     1001      127    68520 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.3.6.sql
+-rw-r--r--   0     1001      127     5517 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.4.0-0.4.1.sql
+-rw-r--r--   0     1001      127    75093 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.4.0.sql
+-rw-r--r--   0     1001      127     5773 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.4.1-0.4.2.sql
+-rw-r--r--   0     1001      127    75572 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.4.1.sql
+-rw-r--r--   0     1001      127     4725 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.4.2-0.4.3.sql
+-rw-r--r--   0     1001      127    75821 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.4.2.sql
+-rw-r--r--   0     1001      127    16274 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.4.3-0.4.4.sql
+-rw-r--r--   0     1001      127    75829 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.4.3.sql
+-rw-r--r--   0     1001      127     8986 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.4.4-0.4.5.sql
+-rw-r--r--   0     1001      127    77866 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.4.4.sql
+-rw-r--r--   0     1001      127    87157 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.4.5-0.5.0.sql
+-rw-r--r--   0     1001      127    77907 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.4.5.sql
+-rw-r--r--   0     1001      127     6474 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.5.0-0.5.1.sql
+-rw-r--r--   0     1001      127    86941 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.5.0.sql
+-rw-r--r--   0     1001      127    23595 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.5.1-0.6.0.sql
+-rw-r--r--   0     1001      127    88071 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.5.1.sql
+-rw-r--r--   0     1001      127      314 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.6.0-0.6.1.sql
+-rw-r--r--   0     1001      127    91221 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.6.0.sql
+-rw-r--r--   0     1001      127       64 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.6.1-0.6.2.sql
+-rw-r--r--   0     1001      127    91293 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.6.1.sql
+-rw-r--r--   0     1001      127     2395 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.6.10-0.6.11.sql
+-rw-r--r--   0     1001      127    97746 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.6.10.sql
+-rw-r--r--   0     1001      127    23983 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.6.11-0.6.12.sql
+-rw-r--r--   0     1001      127    97746 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.6.11.sql
+-rw-r--r--   0     1001      127     6177 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.6.12-0.6.13.sql
+-rw-r--r--   0     1001      127   109293 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.6.12.sql
+-rw-r--r--   0     1001      127    62266 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.6.13-0.7.0.sql
+-rw-r--r--   0     1001      127    71093 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.6.13-0.7.3.sql
+-rw-r--r--   0     1001      127   109390 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.6.13.sql
+-rw-r--r--   0     1001      127      512 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.6.2-0.6.3.sql
+-rw-r--r--   0     1001      127    91293 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.6.2.sql
+-rw-r--r--   0     1001      127     5310 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.6.3-0.6.4.sql
+-rw-r--r--   0     1001      127    91293 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.6.3.sql
+-rw-r--r--   0     1001      127     4869 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.6.4-0.6.5.sql
+-rw-r--r--   0     1001      127    92207 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.6.4.sql
+-rw-r--r--   0     1001      127     6513 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.6.5-0.6.6.sql
+-rw-r--r--   0     1001      127    92729 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.6.5.sql
+-rw-r--r--   0     1001      127     5879 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.6.6-0.6.7.sql
+-rw-r--r--   0     1001      127    93392 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.6.6.sql
+-rw-r--r--   0     1001      127    10806 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.6.7-0.6.8.sql
+-rw-r--r--   0     1001      127    93421 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.6.7.sql
+-rw-r--r--   0     1001      127     6043 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.6.8-0.6.9.sql
+-rw-r--r--   0     1001      127    97125 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.6.8.sql
+-rw-r--r--   0     1001      127     1323 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.6.9-0.6.10.sql
+-rw-r--r--   0     1001      127    97247 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.6.9.sql
+-rw-r--r--   0     1001      127    25596 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.7.0-0.7.1.sql
+-rw-r--r--   0     1001      127   124336 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.7.0.sql
+-rw-r--r--   0     1001      127    12904 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.7.1-0.7.2.sql
+-rw-r--r--   0     1001      127   128215 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.7.1.sql
+-rw-r--r--   0     1001      127    15709 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.7.10-0.8.0.sql
+-rw-r--r--   0     1001      127   136758 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.7.10.sql
+-rw-r--r--   0     1001      127    14951 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.7.2-0.7.3.sql
+-rw-r--r--   0     1001      127   129127 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.7.2.sql
+-rw-r--r--   0     1001      127    25457 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.7.3-0.7.4.sql
+-rw-r--r--   0     1001      127   128574 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.7.3.sql
+-rw-r--r--   0     1001      127    35126 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.7.4-0.7.5.sql
+-rw-r--r--   0     1001      127   132836 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.7.4.sql
+-rw-r--r--   0     1001      127     9377 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.7.5-0.7.6.sql
+-rw-r--r--   0     1001      127   135013 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.7.5.sql
+-rw-r--r--   0     1001      127    14610 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.7.6-0.7.7.sql
+-rw-r--r--   0     1001      127   135026 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.7.6.sql
+-rw-r--r--   0     1001      127     8604 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.7.7-0.7.8.sql
+-rw-r--r--   0     1001      127   136049 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.7.7.sql
+-rw-r--r--   0     1001      127     6841 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.7.8-0.7.9.sql
+-rw-r--r--   0     1001      127   136073 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.7.8.sql
+-rw-r--r--   0     1001      127     8132 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.7.9-0.7.10.sql
+-rw-r--r--   0     1001      127   136073 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.7.9.sql
+-rw-r--r--   0     1001      127     7760 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.8.0-0.8.1.sql
+-rw-r--r--   0     1001      127   137625 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.8.0.sql
+-rw-r--r--   0     1001      127    46866 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.8.1-0.8.2.sql
+-rw-r--r--   0     1001      127   137625 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.8.1.sql
+-rw-r--r--   0     1001      127    12488 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.8.2-0.8.3.sql
+-rw-r--r--   0     1001      127   146813 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.8.2.sql
+-rw-r--r--   0     1001      127     9716 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.8.3-0.8.4.sql
+-rw-r--r--   0     1001      127   147162 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.8.3.sql
+-rw-r--r--   0     1001      127    15676 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.8.4-0.8.5.sql
+-rw-r--r--   0     1001      127   147162 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.8.4.sql
+-rw-r--r--   0     1001      127    40203 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.8.5-0.9.0.sql
+-rw-r--r--   0     1001      127   147174 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.8.5.sql
+-rw-r--r--   0     1001      127   150864 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.9.0.sql
+-rw-r--r--   0     1001      127        0 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/py.typed
+-rw-r--r--   0     1001      127     3588 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/pypgstac.py
+-rw-r--r--   0     1001      127       37 2024-04-30 19:01:24.000000 pypgstac-0.9.0/python/pypgstac/version.py
+-rw-r--r--   0     1001      127     2788 2024-04-30 19:01:24.000000 pypgstac-0.9.0/src/lib.rs
+-rw-r--r--   0     1001      127        0 2024-04-30 19:01:24.000000 pypgstac-0.9.0/tests/__init__.py
+-rw-r--r--   0     1001      127     2173 2024-04-30 19:01:24.000000 pypgstac-0.9.0/tests/conftest.py
+-rw-r--r--   0     1001      127     6737 2024-04-30 19:01:24.000000 pypgstac-0.9.0/tests/data-files/hydration/collections/chloris-biomass.json
+-rw-r--r--   0     1001      127     9009 2024-04-30 19:01:24.000000 pypgstac-0.9.0/tests/data-files/hydration/collections/landsat-c2-l1.json
+-rw-r--r--   0     1001      127    12629 2024-04-30 19:01:24.000000 pypgstac-0.9.0/tests/data-files/hydration/collections/sentinel-1-grd.json
+-rw-r--r--   0     1001      127    11473 2024-04-30 19:01:24.000000 pypgstac-0.9.0/tests/data-files/hydration/dehydrated-items/landsat-c2-l1/LM04_L1GS_001001_19830527_02_T2.json
+-rw-r--r--   0     1001      127    14310 2024-04-30 19:01:24.000000 pypgstac-0.9.0/tests/data-files/hydration/raw-items/landsat-c2-l1/LM04_L1GS_001001_19830527_02_T2.json
+-rw-r--r--   0     1001      127    10925 2024-04-30 19:01:24.000000 pypgstac-0.9.0/tests/data-files/hydration/raw-items/sentinel-1-grd/S1A_IW_GRDH_1SDV_20220428T034417_20220428T034442_042968_05213C.json
+-rw-r--r--   0     1001      127     4992 2024-04-30 19:01:24.000000 pypgstac-0.9.0/tests/data-files/load/dehydrated.txt
+-rw-r--r--   0     1001      127        0 2024-04-30 19:01:24.000000 pypgstac-0.9.0/tests/hydration/__init__.py
+-rw-r--r--   0     1001      127      893 2024-04-30 19:01:24.000000 pypgstac-0.9.0/tests/hydration/test_base_item.py
+-rw-r--r--   0     1001      127     9044 2024-04-30 19:01:24.000000 pypgstac-0.9.0/tests/hydration/test_dehydrate.py
+-rw-r--r--   0     1001      127     1241 2024-04-30 19:01:24.000000 pypgstac-0.9.0/tests/hydration/test_dehydrate_pg.py
+-rw-r--r--   0     1001      127     7926 2024-04-30 19:01:24.000000 pypgstac-0.9.0/tests/hydration/test_hydrate.py
+-rw-r--r--   0     1001      127     1258 2024-04-30 19:01:24.000000 pypgstac-0.9.0/tests/hydration/test_hydrate_pg.py
+-rw-r--r--   0     1001      127    11887 2024-04-30 19:01:24.000000 pypgstac-0.9.0/tests/test_load.py
+-rw-r--r--   0     1001      127     8072 2024-04-30 19:01:24.000000 pypgstac-0.9.0/Cargo.lock
+-rw-r--r--   0     1001      127     3053 2024-04-30 19:01:24.000000 pypgstac-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     2334 1970-01-01 00:00:00.000000 pypgstac-0.9.0/PKG-INFO
```

### Comparing `pypgstac-0.8.6/python/pypgstac/db.py` & `pypgstac-0.9.0/python/pypgstac/db.py`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/hydration.py` & `pypgstac-0.9.0/python/pypgstac/hydration.py`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/load.py` & `pypgstac-0.9.0/python/pypgstac/load.py`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrate.py` & `pypgstac-0.9.0/python/pypgstac/migrate.py`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.1.9.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.1.9.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.2.3.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.2.3.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.2.4-0.2.5.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.2.4-0.2.5.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.2.4-0.2.7.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.2.4-0.2.7.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.2.4.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.2.4.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.2.5-0.2.7.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.2.5-0.2.7.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.2.5.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.2.5.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.2.7.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.2.7.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.2.8.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.2.8.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.2.9-0.3.0.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.2.9-0.3.0.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.2.9.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.2.9.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.3.0-0.3.1.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.3.0-0.3.1.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.3.0.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.3.0.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.3.1-0.3.2.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.3.1-0.3.2.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.3.1.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.3.1.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.3.2-0.3.3.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.3.2-0.3.3.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.3.2.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.3.2.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.3.3-0.3.4.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.3.3-0.3.4.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.3.3.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.3.3.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.3.4-0.3.5.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.3.4-0.3.5.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.3.4.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.3.4.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.3.5-0.3.6.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.3.5-0.3.6.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.3.5.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.3.5.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.3.6-0.4.0.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.3.6-0.4.0.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.3.6.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.3.6.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.4.0-0.4.1.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.4.0-0.4.1.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.4.0.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.4.0.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.4.1-0.4.2.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.4.1-0.4.2.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.4.1.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.4.1.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.4.2-0.4.3.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.4.2-0.4.3.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.4.2.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.4.2.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.4.3-0.4.4.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.4.3-0.4.4.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.4.3.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.4.3.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.4.4-0.4.5.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.4.4-0.4.5.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.4.4.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.4.4.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.4.5-0.5.0.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.4.5-0.5.0.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.4.5.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.4.5.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.5.0-0.5.1.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.5.0-0.5.1.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.5.0.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.5.0.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.5.1-0.6.0.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.5.1-0.6.0.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.5.1.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.5.1.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.6.0.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.6.0.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.6.1.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.6.1.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.6.10-0.6.11.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.6.10-0.6.11.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.6.10.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.6.10.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.6.11-0.6.12.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.6.11-0.6.12.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.6.11.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.6.11.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.6.12-0.6.13.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.6.12-0.6.13.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.6.12.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.6.12.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.6.13-0.7.0.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.6.13-0.7.0.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.6.13-0.7.3.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.6.13-0.7.3.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.6.13.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.6.13.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.6.2-0.6.3.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.6.2-0.6.3.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.6.2.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.6.2.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.6.3-0.6.4.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.6.3-0.6.4.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.6.3.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.6.3.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.6.4-0.6.5.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.6.4-0.6.5.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.6.4.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.6.4.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.6.5-0.6.6.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.6.5-0.6.6.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.6.5.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.6.5.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.6.6-0.6.7.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.6.6-0.6.7.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.6.6.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.6.6.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.6.7-0.6.8.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.6.7-0.6.8.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.6.7.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.6.7.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.6.8-0.6.9.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.6.8-0.6.9.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.6.8.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.6.8.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.6.9-0.6.10.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.6.9-0.6.10.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.6.9.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.6.9.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.7.0-0.7.1.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.7.0-0.7.1.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.7.0.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.7.0.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.7.1-0.7.2.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.7.1-0.7.2.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.7.1.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.7.1.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.7.10-0.8.0.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.7.10-0.8.0.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.7.10.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.7.10.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.7.2-0.7.3.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.7.2-0.7.3.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.7.2.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.7.2.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.7.3-0.7.4.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.7.3-0.7.4.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.7.3.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.7.3.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.7.4-0.7.5.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.7.4-0.7.5.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.7.4.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.7.4.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.7.5-0.7.6.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.7.5-0.7.6.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.7.5.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.7.5.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.7.6-0.7.7.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.7.6-0.7.7.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.7.6.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.7.6.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.7.7-0.7.8.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.7.7-0.7.8.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.7.7.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.7.7.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.7.8-0.7.9.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.7.8-0.7.9.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.7.8.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.7.8.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.7.9-0.7.10.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.7.9-0.7.10.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.7.9.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.7.9.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.8.0-0.8.1.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.8.0-0.8.1.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.8.0.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.8.0.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.8.1-0.8.2.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.8.1-0.8.2.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.8.1.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.8.1.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.8.2-0.8.3.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.8.2-0.8.3.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.8.2.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.8.2.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.8.3-0.8.4.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.8.3-0.8.4.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.8.3.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.8.3.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.8.4-0.8.5.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.8.4-0.8.5.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.8.4.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.8.4.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.8.5.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.8.5.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/python/pypgstac/migrations/pgstac.0.8.6.sql` & `pypgstac-0.9.0/python/pypgstac/migrations/pgstac.0.9.0.sql`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 BEGIN
   IF NOT EXISTS (SELECT 1 FROM pg_extension WHERE extname='postgis') THEN
     CREATE EXTENSION IF NOT EXISTS postgis;
   END IF;
   IF NOT EXISTS (SELECT 1 FROM pg_extension WHERE extname='btree_gist') THEN
     CREATE EXTENSION IF NOT EXISTS btree_gist;
   END IF;
+  IF NOT EXISTS (SELECT 1 FROM pg_extension WHERE extname='unaccent') THEN
+    CREATE EXTENSION IF NOT EXISTS unaccent;
+  END IF;
 END;
 $$ LANGUAGE PLPGSQL;
 
 DO $$
   BEGIN
     CREATE ROLE pgstac_admin;
   EXCEPTION WHEN duplicate_object THEN
@@ -1743,15 +1746,17 @@
     ('-', '%s - %s', NULL),
     ('*', '%s * %s', NULL),
     ('/', '%s / %s', NULL),
     ('not', 'NOT (%s)', NULL),
     ('between', '%s BETWEEN %s AND %s', NULL),
     ('isnull', '%s IS NULL', NULL),
     ('upper', 'upper(%s)', NULL),
-    ('lower', 'lower(%s)', NULL)
+    ('lower', 'lower(%s)', NULL),
+    ('casei', 'upper(%s)', NULL),
+    ('accenti', 'unaccent(%s)', NULL)
 ON CONFLICT (op) DO UPDATE
     SET
         template = EXCLUDED.template
 ;
 
 
 CREATE OR REPLACE FUNCTION cql2_query(j jsonb, wrapper text DEFAULT NULL) RETURNS text AS $$
@@ -1845,16 +1850,16 @@
     END IF;
 
 
 
     IF op = 'between' THEN
         args = jsonb_build_array(
             args->0,
-            args->1->0,
-            args->1->1
+            args->1,
+            args->2
         );
     END IF;
 
     -- Make sure that args is an array and run cql2_query on
     -- each element of the array
     RAISE NOTICE 'ARGS PRE: %', args;
     IF j ? 'args' THEN
@@ -3352,202 +3357,247 @@
     time_to_count float,
     partitions text[]
 );
 
 CREATE INDEX IF NOT EXISTS search_wheres_partitions ON search_wheres USING GIN (partitions);
 CREATE UNIQUE INDEX IF NOT EXISTS search_wheres_where ON search_wheres ((md5(_where)));
 
-CREATE OR REPLACE FUNCTION where_stats(inwhere text, updatestats boolean default false, conf jsonb default null) RETURNS search_wheres AS $$
+CREATE OR REPLACE FUNCTION where_stats(
+    inwhere text,
+    updatestats boolean default false,
+    conf jsonb default null
+) RETURNS search_wheres AS $$
 DECLARE
     t timestamptz;
     i interval;
     explain_json jsonb;
     partitions text[];
     sw search_wheres%ROWTYPE;
     inwhere_hash text := md5(inwhere);
     _context text := lower(context(conf));
     _stats_ttl interval := context_stats_ttl(conf);
-    _estimated_cost float := context_estimated_cost(conf);
-    _estimated_count int := context_estimated_count(conf);
+    _estimated_cost_threshold float := context_estimated_cost(conf);
+    _estimated_count_threshold int := context_estimated_count(conf);
     ro bool := pgstac.readonly(conf);
 BEGIN
-    IF ro THEN
-        updatestats := FALSE;
+    -- If updatestats is true then set ttl to 0
+    IF updatestats THEN
+        RAISE DEBUG 'Updatestats set to TRUE, setting TTL to 0';
+        _stats_ttl := '0'::interval;
     END IF;
 
+    -- If we don't need to calculate context, just return
     IF _context = 'off' THEN
-        sw._where := inwhere;
-        return sw;
+        sw._where = inwhere;
+        RETURN sw;
     END IF;
 
+    -- Get any stats that we have. If there is a lock where another process is
+    -- updating the stats, wait so that we don't end up calculating a bunch of times.
     SELECT * INTO sw FROM search_wheres WHERE md5(_where)=inwhere_hash FOR UPDATE;
 
-    -- Update statistics if explicitly set, if statistics do not exist, or statistics ttl has expired
-    IF NOT updatestats THEN
-        RAISE NOTICE 'Checking if update is needed for: % .', inwhere;
-        RAISE NOTICE 'Stats Last Updated: %', sw.statslastupdated;
-        RAISE NOTICE 'TTL: %, Age: %', _stats_ttl, now() - sw.statslastupdated;
-        RAISE NOTICE 'Context: %, Existing Total: %', _context, sw.total_count;
-        IF
-            (
-                sw.statslastupdated IS NULL
-                OR (now() - sw.statslastupdated) > _stats_ttl
-                OR (context(conf) != 'off' AND sw.total_count IS NULL)
-            ) AND NOT ro
-        THEN
-            updatestats := TRUE;
+    -- If there is a cached row, figure out if we need to update
+    IF
+        sw IS NOT NULL
+        AND sw.statslastupdated IS NOT NULL
+        AND sw.total_count IS NOT NULL
+        AND now() - sw.statslastupdated <= _stats_ttl
+    THEN
+        -- we have a cached row with data that is within our ttl
+        RAISE DEBUG 'Stats present in table and lastupdated within ttl: %', sw;
+        IF NOT ro THEN
+            RAISE DEBUG 'Updating search_wheres only bumping lastused and usecount';
+            UPDATE search_wheres SET
+                lastused = now(),
+                usecount = search_wheres.usecount + 1
+            WHERE md5(_where) = inwhere_hash
+            RETURNING * INTO sw;
         END IF;
-    END IF;
-
-    sw._where := inwhere;
-    sw.lastused := now();
-    sw.usecount := coalesce(sw.usecount,0) + 1;
-
-    IF NOT updatestats THEN
-        UPDATE search_wheres SET
-            lastused = sw.lastused,
-            usecount = sw.usecount
-        WHERE md5(_where) = inwhere_hash
-        RETURNING * INTO sw
-        ;
+        RAISE DEBUG 'Returning cached counts. %', sw;
         RETURN sw;
     END IF;
 
-    -- Use explain to get estimated count/cost and a list of the partitions that would be hit by the query
-    t := clock_timestamp();
-    EXECUTE format('EXPLAIN (format json) SELECT 1 FROM items WHERE %s', inwhere)
-    INTO explain_json;
-    RAISE NOTICE 'Time for just the explain: %', clock_timestamp() - t;
-    i := clock_timestamp() - t;
+    -- Calculate estimated cost and rows
+    -- Use explain to get estimated count/cost
+    IF sw.estimated_count IS NULL OR sw.estimated_cost IS NULL THEN
+        RAISE DEBUG 'Calculating estimated stats';
+        t := clock_timestamp();
+        EXECUTE format('EXPLAIN (format json) SELECT 1 FROM items WHERE %s', inwhere)
+            INTO explain_json;
+        RAISE DEBUG 'Time for just the explain: %', clock_timestamp() - t;
+        i := clock_timestamp() - t;
 
-    sw.statslastupdated := now();
-    sw.estimated_count := explain_json->0->'Plan'->'Plan Rows';
-    sw.estimated_cost := explain_json->0->'Plan'->'Total Cost';
-    sw.time_to_estimate := extract(epoch from i);
+        sw.estimated_count := explain_json->0->'Plan'->'Plan Rows';
+        sw.estimated_cost := explain_json->0->'Plan'->'Total Cost';
+        sw.time_to_estimate := extract(epoch from i);
+    END IF;
 
-    RAISE NOTICE 'ESTIMATED_COUNT: % < %', sw.estimated_count, _estimated_count;
-    RAISE NOTICE 'ESTIMATED_COST: % < %', sw.estimated_cost, _estimated_cost;
+    RAISE DEBUG 'ESTIMATED_COUNT: %, THRESHOLD %', sw.estimated_count, _estimated_count_threshold;
+    RAISE DEBUG 'ESTIMATED_COST: %, THRESHOLD %', sw.estimated_cost, _estimated_cost_threshold;
 
-    -- Do a full count of rows if context is set to on or if auto is set and estimates are low enough
+    -- If context is set to auto and the costs are within the threshold return the estimated costs
     IF
-        _context = 'on'
-        OR
-        ( _context = 'auto' AND
-            (
-                sw.estimated_count < _estimated_count
-                AND
-                sw.estimated_cost < _estimated_cost
-            )
-        )
+        _context = 'auto'
+        AND sw.estimated_count >= _estimated_count_threshold
+        AND sw.estimated_cost >= _estimated_cost_threshold
     THEN
-        t := clock_timestamp();
-        RAISE NOTICE 'Calculating actual count...';
-        EXECUTE format(
-            'SELECT count(*) FROM items WHERE %s',
-            inwhere
-        ) INTO sw.total_count;
-        i := clock_timestamp() - t;
-        RAISE NOTICE 'Actual Count: % -- %', sw.total_count, i;
-        sw.time_to_count := extract(epoch FROM i);
-    ELSE
-        sw.total_count := NULL;
-        sw.time_to_count := NULL;
+        IF NOT ro THEN
+            INSERT INTO search_wheres (
+                _where,
+                lastused,
+                usecount,
+                statslastupdated,
+                estimated_count,
+                estimated_cost,
+                time_to_estimate,
+                total_count,
+                time_to_count
+            ) VALUES (
+                inwhere,
+                now(),
+                1,
+                now(),
+                sw.estimated_count,
+                sw.estimated_cost,
+                sw.time_to_estimate,
+                null,
+                null
+            ) ON CONFLICT ((md5(_where)))
+            DO UPDATE SET
+                lastused = EXCLUDED.lastused,
+                usecount = search_wheres.usecount + 1,
+                statslastupdated = EXCLUDED.statslastupdated,
+                estimated_count = EXCLUDED.estimated_count,
+                estimated_cost = EXCLUDED.estimated_cost,
+                time_to_estimate = EXCLUDED.time_to_estimate,
+                total_count = EXCLUDED.total_count,
+                time_to_count = EXCLUDED.time_to_count
+            RETURNING * INTO sw;
+        END IF;
+        RAISE DEBUG 'Estimates are within thresholds, returning estimates. %', sw;
+        RETURN sw;
     END IF;
 
+    -- Calculate Actual Count
+    t := clock_timestamp();
+    RAISE NOTICE 'Calculating actual count...';
+    EXECUTE format(
+        'SELECT count(*) FROM items WHERE %s',
+        inwhere
+    ) INTO sw.total_count;
+    i := clock_timestamp() - t;
+    RAISE NOTICE 'Actual Count: % -- %', sw.total_count, i;
+    sw.time_to_count := extract(epoch FROM i);
+
     IF NOT ro THEN
-        INSERT INTO search_wheres
-            (_where, lastused, usecount, statslastupdated, estimated_count, estimated_cost, time_to_estimate, partitions, total_count, time_to_count)
-        SELECT sw._where, sw.lastused, sw.usecount, sw.statslastupdated, sw.estimated_count, sw.estimated_cost, sw.time_to_estimate, sw.partitions, sw.total_count, sw.time_to_count
-        ON CONFLICT ((md5(_where)))
-        DO UPDATE
-            SET
-                lastused = sw.lastused,
-                usecount = sw.usecount,
-                statslastupdated = sw.statslastupdated,
-                estimated_count = sw.estimated_count,
-                estimated_cost = sw.estimated_cost,
-                time_to_estimate = sw.time_to_estimate,
-                total_count = sw.total_count,
-                time_to_count = sw.time_to_count
-        ;
+        INSERT INTO search_wheres (
+            _where,
+            lastused,
+            usecount,
+            statslastupdated,
+            estimated_count,
+            estimated_cost,
+            time_to_estimate,
+            total_count,
+            time_to_count
+        ) VALUES (
+            inwhere,
+            now(),
+            1,
+            now(),
+            sw.estimated_count,
+            sw.estimated_cost,
+            sw.time_to_estimate,
+            sw.total_count,
+            sw.time_to_count
+        ) ON CONFLICT ((md5(_where)))
+        DO UPDATE SET
+            lastused = EXCLUDED.lastused,
+            usecount = search_wheres.usecount + 1,
+            statslastupdated = EXCLUDED.statslastupdated,
+            estimated_count = EXCLUDED.estimated_count,
+            estimated_cost = EXCLUDED.estimated_cost,
+            time_to_estimate = EXCLUDED.time_to_estimate,
+            total_count = EXCLUDED.total_count,
+            time_to_count = EXCLUDED.time_to_count
+        RETURNING * INTO sw;
     END IF;
+    RAISE DEBUG 'Returning with actual count. %', sw;
     RETURN sw;
 END;
 $$ LANGUAGE PLPGSQL SECURITY DEFINER;
 
 
 CREATE OR REPLACE FUNCTION search_query(
     _search jsonb = '{}'::jsonb,
     updatestats boolean = false,
     _metadata jsonb = '{}'::jsonb
 ) RETURNS searches AS $$
 DECLARE
     search searches%ROWTYPE;
+    cached_search searches%ROWTYPE;
     pexplain jsonb;
     t timestamptz;
     i interval;
-    _hash text := search_hash(_search, _metadata);
     doupdate boolean := FALSE;
     insertfound boolean := FALSE;
     ro boolean := pgstac.readonly();
+    found_search text;
 BEGIN
+    RAISE NOTICE 'SEARCH: %', _search;
+    -- Calculate hash, where clause, and order by statement
+    search.search := _search;
+    search.metadata := _metadata;
+    search.hash := search_hash(_search, _metadata);
+    search._where := stac_search_to_where(_search);
+    search.orderby := sort_sqlorderby(_search);
+    search.lastused := now();
+    search.usecount := 1;
+
+    -- If we are in read only mode, directly return search
     IF ro THEN
-        updatestats := FALSE;
+        RETURN search;
     END IF;
 
-    SELECT * INTO search FROM searches
-    WHERE hash=_hash;
-
-    search.hash := _hash;
+    RAISE NOTICE 'Updating Statistics for search: %s', search;
+    -- Update statistics for times used and and when last used
+    -- If the entry is locked, rather than waiting, skip updating the stats
+    INSERT INTO searches (search, lastused, usecount, metadata)
+        VALUES (search.search, now(), 1, search.metadata)
+        ON CONFLICT DO NOTHING
+        RETURNING * INTO cached_search
+    ;
 
-    -- Calculate the where clause if not already calculated
-    IF search._where IS NULL THEN
-        search._where := stac_search_to_where(_search);
-    ELSE
-        doupdate := TRUE;
+    IF NOT FOUND OR cached_search IS NULL THEN
+        UPDATE searches SET
+            lastused = now(),
+            usecount = searches.usecount + 1
+        WHERE hash = (
+            SELECT hash FROM searches WHERE hash=search.hash FOR UPDATE SKIP LOCKED
+        )
+        RETURNING * INTO cached_search
+        ;
     END IF;
 
-    -- Calculate the order by clause if not already calculated
-    IF search.orderby IS NULL THEN
-        search.orderby := sort_sqlorderby(_search);
-    ELSE
-        doupdate := TRUE;
+    IF cached_search IS NOT NULL THEN
+        cached_search._where = search._where;
+        cached_search.orderby = search.orderby;
+        RETURN cached_search;
     END IF;
-
-    PERFORM where_stats(search._where, updatestats, _search->'conf');
-
-    IF NOT ro THEN
-        IF NOT doupdate THEN
-            INSERT INTO searches (search, _where, orderby, lastused, usecount, metadata)
-            VALUES (_search, search._where, search.orderby, clock_timestamp(), 1, _metadata)
-            ON CONFLICT (hash) DO NOTHING RETURNING * INTO search;
-            IF FOUND THEN
-                RETURN search;
-            END IF;
-        END IF;
-
-        UPDATE searches
-            SET
-                lastused=clock_timestamp(),
-                usecount=usecount+1
-        WHERE hash=(
-            SELECT hash FROM searches
-            WHERE hash=_hash
-            FOR UPDATE SKIP LOCKED
-        );
-        IF NOT FOUND THEN
-            RAISE NOTICE 'Did not update stats for % due to lock. (This is generally OK)', _search;
-        END IF;
-    END IF;
-
     RETURN search;
 
 END;
 $$ LANGUAGE PLPGSQL SECURITY DEFINER;
 
+CREATE OR REPLACE FUNCTION search_fromhash(
+    _hash text
+) RETURNS searches AS $$
+    SELECT * FROM search_query((SELECT search FROM searches WHERE hash=_hash LIMIT 1));
+$$ LANGUAGE SQL STRICT;
+
 CREATE OR REPLACE FUNCTION search_rows(
     IN _where text DEFAULT 'TRUE',
     IN _orderby text DEFAULT 'datetime DESC, id DESC',
     IN partitions text[] DEFAULT NULL,
     IN _limit int DEFAULT 10
 ) RETURNS SETOF items AS $$
 DECLARE
@@ -3581,15 +3631,15 @@
             base_query,
             sdate,
             edate,
             _where,
             _orderby,
             records_left
         );
-        RAISE LOG 'QUERY: %', query;
+        RAISE DEBUG 'QUERY: %', query;
         timer := clock_timestamp();
         RETURN QUERY EXECUTE query;
 
         GET DIAGNOSTICS n = ROW_COUNT;
         records_left := records_left - n;
         RAISE NOTICE 'Returned %/% Rows From % to %. % to go. Time: %ms', n, _limit, sdate, edate, records_left, age_ms(timer);
         timer := clock_timestamp();
@@ -3605,15 +3655,15 @@
             base_query,
             sdate,
             edate,
             _where,
             _orderby,
             records_left
         );
-        RAISE LOG 'QUERY: %', query;
+        RAISE DEBUG 'QUERY: %', query;
         timer := clock_timestamp();
         RETURN QUERY EXECUTE query;
 
         GET DIAGNOSTICS n = ROW_COUNT;
         records_left := records_left - n;
         RAISE NOTICE 'Returned %/% Rows From % to %. % to go. Time: %ms', n, _limit, sdate, edate, records_left, age_ms(timer);
         timer := clock_timestamp();
@@ -3626,15 +3676,15 @@
     query := format($q$
         SELECT * FROM items
         WHERE %s
         ORDER BY %s
         LIMIT %L
     $q$, _where, _orderby, _limit
     );
-    RAISE LOG 'QUERY: %', query;
+    RAISE DEBUG 'QUERY: %', query;
     timer := clock_timestamp();
     RETURN QUERY EXECUTE query;
     RAISE NOTICE 'FULL QUERY TOOK %ms', age_ms(timer);
 END IF;
 RAISE NOTICE 'SEARCH_ROWS TOOK %ms', age_ms(full_timer);
 RETURN;
 END;
@@ -3707,40 +3757,42 @@
     out_records jsonb;
     out_len int;
     _limit int := coalesce((_search->>'limit')::int, 10);
     _querylimit int;
     _fields jsonb := coalesce(_search->'fields', '{}'::jsonb);
     has_prev boolean := FALSE;
     has_next boolean := FALSE;
+    links jsonb := '[]'::jsonb;
+    base_url text:= concat(rtrim(base_url(_search->'conf'),'/'));
 BEGIN
     searches := search_query(_search);
     _where := searches._where;
     orderby := searches.orderby;
     search_where := where_stats(_where);
     total_count := coalesce(search_where.total_count, search_where.estimated_count);
     RAISE NOTICE 'SEARCH:TOKEN: %', _search->>'token';
     token := get_token_record(_search->>'token');
     RAISE NOTICE '***TOKEN: %', token;
     _querylimit := _limit + 1;
     IF token IS NOT NULL THEN
         token_prev := token.prev;
         token_item := token.item;
         token_where := get_token_filter(_search->'sortby', token_item, token_prev, FALSE);
-        RAISE LOG 'TOKEN_WHERE: % (%ms from search start)', token_where, age_ms(timer);
+        RAISE DEBUG 'TOKEN_WHERE: % (%ms from search start)', token_where, age_ms(timer);
         IF token_prev THEN -- if we are using a prev token, we know has_next is true
-            RAISE LOG 'There is a previous token, so automatically setting has_next to true';
+            RAISE DEBUG 'There is a previous token, so automatically setting has_next to true';
             has_next := TRUE;
             orderby := sort_sqlorderby(_search, TRUE);
         ELSE
-            RAISE LOG 'There is a next token, so automatically setting has_prev to true';
+            RAISE DEBUG 'There is a next token, so automatically setting has_prev to true';
             has_prev := TRUE;
 
         END IF;
     ELSE -- if there was no token, we know there is no prev
-        RAISE LOG 'There is no token, so we know there is no prev. setting has_prev to false';
+        RAISE DEBUG 'There is no token, so we know there is no prev. setting has_prev to false';
         has_prev := FALSE;
     END IF;
 
     full_where := concat_ws(' AND ', _where, token_where);
     RAISE NOTICE 'FULL WHERE CLAUSE: %', full_where;
     RAISE NOTICE 'Time to get counts and build query %', age_ms(timer);
     timer := clock_timestamp();
@@ -3766,17 +3818,17 @@
 
 
     IF token_prev THEN
         out_records := flip_jsonb_array(out_records);
     END IF;
 
     RAISE NOTICE 'Query returned % records.', jsonb_array_length(out_records);
-    RAISE LOG 'TOKEN:   % %', token_item.id, token_item.collection;
-    RAISE LOG 'RECORD_1: % %', out_records->0->>'id', out_records->0->>'collection';
-    RAISE LOG 'RECORD-1: % %', out_records->-1->>'id', out_records->-1->>'collection';
+    RAISE DEBUG 'TOKEN:   % %', token_item.id, token_item.collection;
+    RAISE DEBUG 'RECORD_1: % %', out_records->0->>'id', out_records->0->>'collection';
+    RAISE DEBUG 'RECORD-1: % %', out_records->-1->>'id', out_records->-1->>'collection';
 
     -- REMOVE records that were from our token
     IF out_records->0->>'id' = token_item.id AND out_records->0->>'collection' = token_item.collection THEN
         out_records := out_records - 0;
     ELSIF out_records->-1->>'id' = token_item.id AND out_records->-1->>'collection' = token_item.collection THEN
         out_records := out_records - -1;
     END IF;
@@ -3789,57 +3841,79 @@
             out_records := out_records - 0;
         ELSE
             has_next := TRUE;
             out_records := out_records - -1;
         END IF;
     END IF;
 
+
+    links := links || jsonb_build_object(
+        'rel', 'root',
+        'type', 'application/json',
+        'href', base_url
+    ) || jsonb_build_object(
+        'rel', 'self',
+        'type', 'application/json',
+        'href', concat(base_url, '/search')
+    );
+
     IF has_next THEN
         next := concat(out_records->-1->>'collection', ':', out_records->-1->>'id');
         RAISE NOTICE 'HAS NEXT | %', next;
+        links := links || jsonb_build_object(
+            'rel', 'next',
+            'type', 'application/geo+json',
+            'method', 'GET',
+            'href', concat(base_url, '/search?token=next:', next)
+        );
     END IF;
 
     IF has_prev THEN
         prev := concat(out_records->0->>'collection', ':', out_records->0->>'id');
         RAISE NOTICE 'HAS PREV | %', prev;
+        links := links || jsonb_build_object(
+            'rel', 'prev',
+            'type', 'application/geo+json',
+            'method', 'GET',
+            'href', concat(base_url, '/search?token=prev:', prev)
+        );
     END IF;
 
     RAISE NOTICE 'Time to get prev/next %', age_ms(timer);
     timer := clock_timestamp();
 
-    IF context(_search->'conf') != 'off' THEN
-        context := jsonb_strip_nulls(jsonb_build_object(
-            'limit', _limit,
-            'matched', total_count,
-            'returned', coalesce(jsonb_array_length(out_records), 0)
-        ));
-    ELSE
-        context := jsonb_strip_nulls(jsonb_build_object(
-            'limit', _limit,
-            'returned', coalesce(jsonb_array_length(out_records), 0)
-        ));
-    END IF;
 
     collection := jsonb_build_object(
         'type', 'FeatureCollection',
         'features', coalesce(out_records, '[]'::jsonb),
-        'next', next,
-        'prev', prev,
-        'context', context
+        'links', links
     );
 
+
+
+    IF context(_search->'conf') != 'off' THEN
+        collection := collection || jsonb_strip_nulls(jsonb_build_object(
+            'numberMatched', total_count,
+            'numberReturned', coalesce(jsonb_array_length(out_records), 0)
+        ));
+    ELSE
+        collection := collection || jsonb_strip_nulls(jsonb_build_object(
+            'numberReturned', coalesce(jsonb_array_length(out_records), 0)
+        ));
+    END IF;
+
     IF get_setting_bool('timing', _search->'conf') THEN
         collection = collection || jsonb_build_object('timing', age_ms(init_ts));
     END IF;
 
     RAISE NOTICE 'Time to build final json %', age_ms(timer);
     timer := clock_timestamp();
 
     RAISE NOTICE 'Total Time: %', age_ms(current_timestamp);
-    RAISE NOTICE 'RETURNING % records. NEXT: %. PREV: %', collection->'context'->>'returned', collection->>'next', collection->>'prev';
+    RAISE NOTICE 'RETURNING % records. NEXT: %. PREV: %', collection->>'numberReturned', collection->>'next', collection->>'prev';
     RETURN collection;
 END;
 $$ LANGUAGE PLPGSQL;
 
 
 CREATE OR REPLACE FUNCTION search_cursor(_search jsonb = '{}'::jsonb) RETURNS refcursor AS $$
 DECLARE
@@ -4014,19 +4088,16 @@
                 )
             );
         END IF;
     END IF;
 
     ret := jsonb_build_object(
         'collections', out_records,
-        'context', jsonb_build_object(
-            'limit', _limit,
-            'matched', number_matched,
-            'returned', number_returned
-        ),
+        'numberMatched', number_matched,
+        'numberReturned', number_returned,
         'links', links
     );
     RETURN ret;
 
 END;
 $$ LANGUAGE PLPGSQL STABLE PARALLEL SAFE;
 SET SEARCH_PATH TO pgstac, public;
@@ -4095,17 +4166,17 @@
     END IF;
 
     -- If skipcovered is true then you will always want to exit when the passed in geometry is full
     IF skipcovered THEN
         exitwhenfull := TRUE;
     END IF;
 
-    SELECT * INTO search FROM searches WHERE hash=queryhash;
+    search := search_fromhash(queryhash);
 
-    IF NOT FOUND THEN
+    IF search IS NULL THEN
         RAISE EXCEPTION 'Search with Query Hash % Not Found', queryhash;
     END IF;
 
     tilearea := st_area(geom);
     _where := format('%s AND st_intersects(geometry, %L::geometry)', search._where, geom);
 
 
@@ -4343,14 +4414,51 @@
   ('queue_timeout', '10 minutes'),
   ('update_collection_extent', 'false'),
   ('format_cache', 'false'),
   ('readonly', 'false')
 ON CONFLICT DO NOTHING
 ;
 
+
+INSERT INTO cql2_ops (op, template, types) VALUES
+    ('eq', '%s = %s', NULL),
+    ('neq', '%s != %s', NULL),
+    ('ne', '%s != %s', NULL),
+    ('!=', '%s != %s', NULL),
+    ('<>', '%s != %s', NULL),
+    ('lt', '%s < %s', NULL),
+    ('lte', '%s <= %s', NULL),
+    ('gt', '%s > %s', NULL),
+    ('gte', '%s >= %s', NULL),
+    ('le', '%s <= %s', NULL),
+    ('ge', '%s >= %s', NULL),
+    ('=', '%s = %s', NULL),
+    ('<', '%s < %s', NULL),
+    ('<=', '%s <= %s', NULL),
+    ('>', '%s > %s', NULL),
+    ('>=', '%s >= %s', NULL),
+    ('like', '%s LIKE %s', NULL),
+    ('ilike', '%s ILIKE %s', NULL),
+    ('+', '%s + %s', NULL),
+    ('-', '%s - %s', NULL),
+    ('*', '%s * %s', NULL),
+    ('/', '%s / %s', NULL),
+    ('not', 'NOT (%s)', NULL),
+    ('between', '%s BETWEEN %s AND %s', NULL),
+    ('isnull', '%s IS NULL', NULL),
+    ('upper', 'upper(%s)', NULL),
+    ('lower', 'lower(%s)', NULL),
+    ('casei', 'upper(%s)', NULL),
+    ('accenti', 'unaccent(%s)', NULL)
+ON CONFLICT (op) DO UPDATE
+    SET
+        template = EXCLUDED.template
+;
+
+
 ALTER FUNCTION to_text COST 5000;
 ALTER FUNCTION to_float COST 5000;
 ALTER FUNCTION to_int COST 5000;
 ALTER FUNCTION to_tstz COST 5000;
 ALTER FUNCTION to_text_array COST 5000;
 
 ALTER FUNCTION update_partition_stats SECURITY DEFINER;
@@ -4386,8 +4494,8 @@
 REVOKE ALL PRIVILEGES ON FUNCTION run_queued_queries_intransaction FROM public;
 GRANT ALL ON FUNCTION run_queued_queries_intransaction TO pgstac_admin;
 
 RESET ROLE;
 
 SET ROLE pgstac_ingest;
 SELECT update_partition_stats_q(partition) FROM partitions_view;
-SELECT set_version('0.8.6');
+SELECT set_version('0.9.0');
```

### Comparing `pypgstac-0.8.6/python/pypgstac/pypgstac.py` & `pypgstac-0.9.0/python/pypgstac/pypgstac.py`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/src/lib.rs` & `pypgstac-0.9.0/src/lib.rs`

 * *Files 22% similar despite different names*

```diff
@@ -18,74 +18,90 @@
     unused_import_braces,
     unused_lifetimes,
     unused_qualifications,
     unused_results
 )]
 
 use anyhow::anyhow;
+use pyo3::pybacked::PyBackedStr;
 use pyo3::{
     prelude::*,
-    types::{PyDict, PyList, PyString},
+    types::{PyDict, PyList},
 };
 
 const MAGIC_MARKER: &str = "𒍟※";
 
 #[pyfunction]
-fn hydrate<'a>(base: &PyAny, item: &'a PyAny) -> PyResult<&'a PyAny> {
+fn hydrate<'py>(
+    base: &'py Bound<'py, PyAny>,
+    item: &'py Bound<'py, PyAny>,
+) -> PyResult<&'py Bound<'py, PyAny>> {
     hydrate_any(base, item)
 }
 
-fn hydrate_any<'a>(base: &PyAny, item: &'a PyAny) -> PyResult<&'a PyAny> {
+fn hydrate_any<'py>(
+    base: &'py Bound<'py, PyAny>,
+    item: &'py Bound<'py, PyAny>,
+) -> PyResult<&'py Bound<'py, PyAny>> {
     if let Ok(item) = item.downcast::<PyDict>() {
         if let Ok(base) = base.downcast::<PyDict>() {
-            hydrate_dict(base, item).map(|item| item.into())
+            Ok(hydrate_dict(base, item)?.as_any())
+        } else if base.is_none() {
+            Ok(item)
         } else {
             Err(anyhow!("type mismatch").into())
         }
     } else if let Ok(item) = item.downcast::<PyList>() {
         if let Ok(base) = base.downcast::<PyList>() {
-            hydrate_list(base, item).map(|item| item.into())
+            Ok(hydrate_list(base, item)?.as_any())
+        } else if base.is_none() {
+            Ok(item)
         } else {
             Err(anyhow!("type mismatch").into())
         }
     } else {
         Ok(item)
     }
 }
 
-fn hydrate_list<'a>(base: &PyList, item: &'a PyList) -> PyResult<&'a PyList> {
+fn hydrate_list<'py>(
+    base: &'py Bound<'py, PyList>,
+    item: &'py Bound<'py, PyList>,
+) -> PyResult<&'py Bound<'py, PyList>> {
     for i in 0..item.len() {
         if i >= base.len() {
             return Ok(item);
         } else {
-            item.set_item(i, hydrate(&base[i], &item[i])?)?;
+            item.set_item(i, hydrate(&base.get_item(i)?, &item.get_item(i)?)?)?;
         }
     }
     Ok(item)
 }
 
-fn hydrate_dict<'a>(base: &PyDict, item: &'a PyDict) -> PyResult<&'a PyDict> {
+fn hydrate_dict<'py>(
+    base: &'py Bound<'py, PyDict>,
+    item: &'py Bound<'py, PyDict>,
+) -> PyResult<&'py Bound<'py, PyDict>> {
     for (key, base_value) in base {
-        if let Some(item_value) = item.get_item(key) {
+        if let Some(item_value) = item.get_item(&key)? {
             if item_value
-                .downcast::<PyString>()
+                .extract::<PyBackedStr>()
                 .ok()
-                .and_then(|value| value.to_str().ok())
-                .map(|s| s == MAGIC_MARKER)
+                .map(|s| <PyBackedStr as AsRef<str>>::as_ref(&s) == MAGIC_MARKER)
                 .unwrap_or(false)
             {
-                item.del_item(&key)?;
+                item.del_item(key)?;
             } else {
-                item.set_item(key, hydrate(base_value, item_value)?)?;
+                item.set_item(&key, hydrate(&base_value, &item_value)?)?;
             }
         } else {
             item.set_item(key, base_value)?;
         }
     }
     Ok(item)
 }
 
 #[pymodule]
-fn pgstacrs(_py: Python<'_>, m: &PyModule) -> PyResult<()> {
+fn pgstacrs(_py: Python<'_>, m: &Bound<'_, PyModule>) -> PyResult<()> {
     m.add_function(wrap_pyfunction!(crate::hydrate, m)?)?;
     Ok(())
 }
```

### Comparing `pypgstac-0.8.6/tests/conftest.py` & `pypgstac-0.9.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/tests/data-files/hydration/collections/chloris-biomass.json` & `pypgstac-0.9.0/tests/data-files/hydration/collections/chloris-biomass.json`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/tests/data-files/hydration/collections/landsat-c2-l1.json` & `pypgstac-0.9.0/tests/data-files/hydration/collections/landsat-c2-l1.json`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/tests/data-files/hydration/collections/sentinel-1-grd.json` & `pypgstac-0.9.0/tests/data-files/hydration/collections/sentinel-1-grd.json`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/tests/data-files/hydration/dehydrated-items/landsat-c2-l1/LM04_L1GS_001001_19830527_02_T2.json` & `pypgstac-0.9.0/tests/data-files/hydration/dehydrated-items/landsat-c2-l1/LM04_L1GS_001001_19830527_02_T2.json`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/tests/data-files/hydration/raw-items/landsat-c2-l1/LM04_L1GS_001001_19830527_02_T2.json` & `pypgstac-0.9.0/tests/data-files/hydration/raw-items/landsat-c2-l1/LM04_L1GS_001001_19830527_02_T2.json`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/tests/data-files/hydration/raw-items/sentinel-1-grd/S1A_IW_GRDH_1SDV_20220428T034417_20220428T034442_042968_05213C.json` & `pypgstac-0.9.0/tests/data-files/hydration/raw-items/sentinel-1-grd/S1A_IW_GRDH_1SDV_20220428T034417_20220428T034442_042968_05213C.json`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/tests/data-files/load/dehydrated.txt` & `pypgstac-0.9.0/tests/data-files/load/dehydrated.txt`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/tests/hydration/test_base_item.py` & `pypgstac-0.9.0/tests/hydration/test_base_item.py`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/tests/hydration/test_dehydrate.py` & `pypgstac-0.9.0/tests/hydration/test_dehydrate.py`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/tests/hydration/test_dehydrate_pg.py` & `pypgstac-0.9.0/tests/hydration/test_dehydrate_pg.py`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/tests/hydration/test_hydrate.py` & `pypgstac-0.9.0/tests/hydration/test_hydrate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Test Hydration."""
+
 import json
 from copy import deepcopy
 from pathlib import Path
 from typing import Any, Dict, cast
 
 from pypgstac import hydration
 from pypgstac.hydration import DO_NOT_MERGE_MARKER
@@ -31,15 +32,17 @@
     / "landsat-c2-l1"
     / "LM04_L1GS_001001_19830527_02_T2.json"
 )
 
 
 class TestHydrate:
     def hydrate(
-        self, base_item: Dict[str, Any], item: Dict[str, Any],
+        self,
+        base_item: Dict[str, Any],
+        item: Dict[str, Any],
     ) -> Dict[str, Any]:
         hpy = hydration.hydrate_py(deepcopy(base_item), deepcopy(item))
         hrs = hydration.hydrate(deepcopy(base_item), deepcopy(item))
         assert hpy == hrs
         return hrs
 
     def test_landsat_c2_l1(self, loader: Loader) -> None:
@@ -230,7 +233,13 @@
             "triple": DO_NOT_MERGE_MARKER,
             "unique": "value",
         }
 
         hydrated = self.hydrate(base_item, dehydrated)
 
         assert hydrated == {"included": "value", "unique": "value"}
+
+    def test_base_none(self) -> None:
+        base_item = {"value": None}
+        dehydrated = {"value": {"a": "b"}}
+        hydrated = self.hydrate(base_item, dehydrated)
+        assert hydrated == {"value": {"a": "b"}}
```

### Comparing `pypgstac-0.8.6/tests/hydration/test_hydrate_pg.py` & `pypgstac-0.9.0/tests/hydration/test_hydrate_pg.py`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/tests/test_load.py` & `pypgstac-0.9.0/tests/test_load.py`

 * *Files identical despite different names*

### Comparing `pypgstac-0.8.6/Cargo.lock` & `pypgstac-0.9.0/Cargo.lock`

 * *Files 10% similar despite different names*

```diff
@@ -23,18 +23,24 @@
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
+name = "heck"
+version = "0.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
+
+[[package]]
 name = "indoc"
-version = "1.0.9"
+version = "2.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
+checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
 
 [[package]]
 name = "libc"
 version = "0.2.148"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9cdc71e17332e86d2e1d38c1f99edcb6288ee11b815fb1a4b049eaa2114d369b"
 
@@ -91,79 +97,88 @@
 version = "0.0.0"
 dependencies = [
  "anyhow",
  "pyo3",
 ]
 
 [[package]]
+name = "portable-atomic"
+version = "1.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
+
+[[package]]
 name = "proc-macro2"
 version = "1.0.67"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3d433d9f1a3e8c1263d9456598b16fec66f4acc9a74dacffd35c7bb09b3a1328"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.19.2"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e681a6cfdc4adcc93b4d3cf993749a4552018ee0a9b65fc0ccfad74352c72a38"
+checksum = "a5e00b96a521718e08e03b1a622f01c8a8deb50719335de3f60b3b3950f069d8"
 dependencies = [
  "anyhow",
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
+ "portable-atomic",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.19.2"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "076c73d0bc438f7a4ef6fdd0c3bb4732149136abd952b110ac93e4edb13a6ba5"
+checksum = "7883df5835fafdad87c0d888b266c8ec0f4c9ca48a5bed6bbb592e8dedee1b50"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.19.2"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e53cee42e77ebe256066ba8aa77eff722b3bb91f3419177cf4cd0f304d3284d9"
+checksum = "01be5843dc60b916ab4dad1dca6d20b9b4e6ddc8e15f50c47fe6d85f1fb97403"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.19.2"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dfeb4c99597e136528c6dd7d5e3de5434d1ceaf487436a3f03b2d56b6fc9efd1"
+checksum = "77b34069fc0682e11b31dbd10321cbf94808394c56fd996796ce45217dfac53c"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.19.2"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "947dc12175c254889edc0c02e399476c2f652b4b9ebd123aa655c224de259536"
+checksum = "08260721f32db5e1a5beae69a55553f56b99bd0e1c3e6e0a5e8851a9d0f5a85c"
 dependencies = [
+ "heck",
  "proc-macro2",
+ "pyo3-build-config",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "quote"
 version = "1.0.33"
@@ -192,17 +207,17 @@
 name = "smallvec"
 version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "62bb4feee49fdd9f707ef802e22365a35de4b7b299de4763d44bfea899442ff9"
 
 [[package]]
 name = "syn"
-version = "1.0.109"
+version = "2.0.43"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
+checksum = "ee659fb5f3d355364e1f3e5bc10fb82068efbf824a1e9d1c9504244a6469ad53"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -215,17 +230,17 @@
 name = "unicode-ident"
 version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3354b9ac3fae1ff6755cb6db53683adb661634f67557942dea4facebec0fee4b"
 
 [[package]]
 name = "unindent"
-version = "0.1.11"
+version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
+checksum = "c7de7d73e1754487cb58364ee906a499937a0dfabd86bcb980fa99ec8c8fa2ce"
 
 [[package]]
 name = "windows-targets"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
 dependencies = [
```

### Comparing `pypgstac-0.8.6/pyproject.toml` & `pypgstac-0.9.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pypgstac"
-version = "0.8.6"
+version = "0.9.0"
 description = "Schema, functions and a python library for storing and accessing STAC collections and items in PostgreSQL"
 readme = "README.md"
 requires-python = ">=3.8"
 license = "MIT"
 authors = [
     {name = "David Bitner", email = "bitner@dbspatial.com"},
 ]
@@ -16,15 +16,15 @@
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
-    "smart-open>=4.2",
+    "smart-open==6.3.*",
     "orjson>=3.5.2",
     "python-dateutil==2.8.*",
     "fire==0.4.*",
     "plpygis==0.2.*",
     "pydantic>=1.7",
     "tenacity==8.1.*",
     "cachetools==5.3.*",
```

### Comparing `pypgstac-0.8.6/PKG-INFO` & `pypgstac-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.3
 Name: pypgstac
-Version: 0.8.6
+Version: 0.9.0
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: smart-open >=4.2
+Requires-Dist: smart-open ==6.3.*
 Requires-Dist: orjson >=3.5.2
 Requires-Dist: python-dateutil ==2.8.*
 Requires-Dist: fire ==0.4.*
 Requires-Dist: plpygis ==0.2.*
 Requires-Dist: pydantic >=1.7
 Requires-Dist: tenacity ==8.1.*
 Requires-Dist: cachetools ==5.3.*
```

