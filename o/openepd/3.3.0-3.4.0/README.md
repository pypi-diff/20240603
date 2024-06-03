# Comparing `tmp/openepd-3.3.0.tar.gz` & `tmp/openepd-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openepd-3.3.0.tar", max compression
+gzip compressed data, was "openepd-3.4.0.tar", max compression
```

## Comparing `openepd-3.3.0.tar` & `openepd-3.4.0.tar`

### file list

```diff
@@ -1,93 +1,93 @@
--rw-r--r--   0        0        0    11357 2024-05-30 11:02:26.077691 openepd-3.3.0/LICENSE
--rw-r--r--   0        0        0     6786 2024-05-30 11:02:26.077691 openepd-3.3.0/README.md
--rw-r--r--   0        0        0     3147 2024-05-30 11:02:26.077691 openepd-3.3.0/pyproject.toml
--rw-r--r--   0        0        0      837 2024-05-30 11:02:26.077691 openepd-3.3.0/src/openepd/__init__.py
--rw-r--r--   0        0        0      855 2024-05-30 11:02:26.077691 openepd-3.3.0/src/openepd/__version__.py
--rw-r--r--   0        0        0      837 2024-05-30 11:02:26.077691 openepd-3.3.0/src/openepd/api/__init__.py
--rw-r--r--   0        0        0    21142 2024-05-30 11:02:26.077691 openepd-3.3.0/src/openepd/api/base_sync_client.py
--rw-r--r--   0        0        0      837 2024-05-30 11:02:26.077691 openepd-3.3.0/src/openepd/api/category/__init__.py
--rw-r--r--   0        0        0     1067 2024-05-30 11:02:26.077691 openepd-3.3.0/src/openepd/api/category/dto.py
--rw-r--r--   0        0        0     1588 2024-05-30 11:02:26.077691 openepd-3.3.0/src/openepd/api/category/sync_api.py
--rw-r--r--   0        0        0     8681 2024-05-30 11:02:26.077691 openepd-3.3.0/src/openepd/api/common.py
--rw-r--r--   0        0        0      837 2024-05-30 11:02:26.077691 openepd-3.3.0/src/openepd/api/dto/__init__.py
--rw-r--r--   0        0        0     1250 2024-05-30 11:02:26.077691 openepd-3.3.0/src/openepd/api/dto/base.py
--rw-r--r--   0        0        0     4705 2024-05-30 11:02:26.077691 openepd-3.3.0/src/openepd/api/dto/common.py
--rw-r--r--   0        0        0     2377 2024-05-30 11:02:26.077691 openepd-3.3.0/src/openepd/api/dto/meta.py
--rw-r--r--   0        0        0     2211 2024-05-30 11:02:26.077691 openepd-3.3.0/src/openepd/api/dto/mf.py
--rw-r--r--   0        0        0      837 2024-05-30 11:02:26.077691 openepd-3.3.0/src/openepd/api/dto/params.py
--rw-r--r--   0        0        0      837 2024-05-30 11:02:26.077691 openepd-3.3.0/src/openepd/api/epd/__init__.py
--rw-r--r--   0        0        0     5091 2024-05-30 11:02:26.077691 openepd-3.3.0/src/openepd/api/epd/dto.py
--rw-r--r--   0        0        0     4391 2024-05-30 11:02:26.077691 openepd-3.3.0/src/openepd/api/epd/sync_api.py
--rw-r--r--   0        0        0     2376 2024-05-30 11:02:26.077691 openepd-3.3.0/src/openepd/api/errors.py
--rw-r--r--   0        0        0      837 2024-05-30 11:02:26.077691 openepd-3.3.0/src/openepd/api/pcr/__init__.py
--rw-r--r--   0        0        0     1649 2024-05-30 11:02:26.077691 openepd-3.3.0/src/openepd/api/pcr/dto.py
--rw-r--r--   0        0        0     1805 2024-05-30 11:02:26.077691 openepd-3.3.0/src/openepd/api/pcr/sync_api.py
--rw-r--r--   0        0        0     2504 2024-05-30 11:02:26.077691 openepd-3.3.0/src/openepd/api/sync_client.py
--rw-r--r--   0        0        0      837 2024-05-30 11:02:26.077691 openepd-3.3.0/src/openepd/api/test/__init__.py
--rw-r--r--   0        0        0      837 2024-05-30 11:02:26.077691 openepd-3.3.0/src/openepd/bundle/__init__.py
--rw-r--r--   0        0        0     7086 2024-05-30 11:02:26.077691 openepd-3.3.0/src/openepd/bundle/base.py
--rw-r--r--   0        0        0     2663 2024-05-30 11:02:26.077691 openepd-3.3.0/src/openepd/bundle/model.py
--rw-r--r--   0        0        0     6904 2024-05-30 11:02:26.077691 openepd-3.3.0/src/openepd/bundle/reader.py
--rw-r--r--   0        0        0     8353 2024-05-30 11:02:26.081692 openepd-3.3.0/src/openepd/bundle/writer.py
--rw-r--r--   0        0        0      837 2024-05-30 11:02:26.081692 openepd-3.3.0/src/openepd/compat/__init__.py
--rw-r--r--   0        0        0     1051 2024-05-30 11:02:26.081692 openepd-3.3.0/src/openepd/compat/compat_functional_validators.py
--rw-r--r--   0        0        0     1363 2024-05-30 11:02:26.081692 openepd-3.3.0/src/openepd/compat/pydantic.py
--rw-r--r--   0        0        0      837 2024-05-30 11:02:26.081692 openepd-3.3.0/src/openepd/model/__init__.py
--rw-r--r--   0        0        0     9154 2024-05-30 11:02:26.081692 openepd-3.3.0/src/openepd/model/base.py
--rw-r--r--   0        0        0     1856 2024-05-30 11:02:26.081692 openepd-3.3.0/src/openepd/model/category.py
--rw-r--r--   0        0        0     5659 2024-05-30 11:02:26.081692 openepd-3.3.0/src/openepd/model/common.py
--rw-r--r--   0        0        0    14299 2024-05-30 11:02:26.081692 openepd-3.3.0/src/openepd/model/epd.py
--rw-r--r--   0        0        0     1918 2024-05-30 11:02:26.081692 openepd-3.3.0/src/openepd/model/factory.py
--rw-r--r--   0        0        0    17165 2024-05-30 11:02:26.081692 openepd-3.3.0/src/openepd/model/lcia.py
--rw-r--r--   0        0        0     4013 2024-05-30 11:02:26.081692 openepd-3.3.0/src/openepd/model/org.py
--rw-r--r--   0        0        0     4620 2024-05-30 11:02:26.081692 openepd-3.3.0/src/openepd/model/pcr.py
--rw-r--r--   0        0        0      862 2024-05-30 11:02:26.081692 openepd-3.3.0/src/openepd/model/specs/README.md
--rw-r--r--   0        0        0     5176 2024-05-30 11:02:26.081692 openepd-3.3.0/src/openepd/model/specs/__init__.py
--rw-r--r--   0        0        0     3549 2024-05-30 11:02:26.081692 openepd-3.3.0/src/openepd/model/specs/asphalt.py
--rw-r--r--   0        0        0     2697 2024-05-30 11:02:26.081692 openepd-3.3.0/src/openepd/model/specs/base.py
--rw-r--r--   0        0        0     9810 2024-05-30 11:02:26.081692 openepd-3.3.0/src/openepd/model/specs/concrete.py
--rw-r--r--   0        0        0      837 2024-05-30 11:02:26.081692 openepd-3.3.0/src/openepd/model/specs/generated/__init__.py
--rw-r--r--   0        0        0     2230 2024-05-30 11:02:26.081692 openepd-3.3.0/src/openepd/model/specs/generated/accessories.py
--rw-r--r--   0        0        0     3161 2024-05-30 11:02:26.081692 openepd-3.3.0/src/openepd/model/specs/generated/aggregates.py
--rw-r--r--   0        0        0     2630 2024-05-30 11:02:26.081692 openepd-3.3.0/src/openepd/model/specs/generated/aluminium.py
--rw-r--r--   0        0        0     3369 2024-05-30 11:02:26.081692 openepd-3.3.0/src/openepd/model/specs/generated/asphalt.py
--rw-r--r--   0        0        0     1092 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/specs/generated/bulk_materials.py
--rw-r--r--   0        0        0     1172 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/specs/generated/cast_decks_and_underlayment.py
--rw-r--r--   0        0        0     6779 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/specs/generated/cladding.py
--rw-r--r--   0        0        0     2011 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/specs/generated/cmu.py
--rw-r--r--   0        0        0     1117 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/specs/generated/common.py
--rw-r--r--   0        0        0     7204 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/specs/generated/concrete.py
--rw-r--r--   0        0        0     2034 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/specs/generated/conveying_equipment.py
--rw-r--r--   0        0        0    10972 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/specs/generated/electrical.py
--rw-r--r--   0        0        0     2195 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/specs/generated/electrical_transmission_and_distribution_equipment.py
--rw-r--r--   0        0        0     1040 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/specs/generated/electricity.py
--rw-r--r--   0        0        0    58546 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/specs/generated/enums.py
--rw-r--r--   0        0        0    21338 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/specs/generated/finishes.py
--rw-r--r--   0        0        0     3285 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/specs/generated/fire_and_smoke_protection.py
--rw-r--r--   0        0        0     2798 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/specs/generated/furnishings.py
--rw-r--r--   0        0        0     1151 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/specs/generated/grouting.py
--rw-r--r--   0        0        0     5320 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/specs/generated/manufacturing_inputs.py
--rw-r--r--   0        0        0     3286 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/specs/generated/masonry.py
--rw-r--r--   0        0        0     1491 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/specs/generated/material_handling.py
--rw-r--r--   0        0        0     9494 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/specs/generated/mechanical.py
--rw-r--r--   0        0        0     1834 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/specs/generated/mechanical_insulation.py
--rw-r--r--   0        0        0     8374 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/specs/generated/network_infrastructure.py
--rw-r--r--   0        0        0    19035 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/specs/generated/openings.py
--rw-r--r--   0        0        0     1031 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/specs/generated/other_electrical_equipment.py
--rw-r--r--   0        0        0     3715 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/specs/generated/other_materials.py
--rw-r--r--   0        0        0     4795 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/specs/generated/plumbing.py
--rw-r--r--   0        0        0     7544 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/specs/generated/precast_concrete.py
--rw-r--r--   0        0        0     3853 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/specs/generated/sheathing.py
--rw-r--r--   0        0        0    10118 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/specs/generated/steel.py
--rw-r--r--   0        0        0     8422 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/specs/generated/thermal_moisture_protection.py
--rw-r--r--   0        0        0     2710 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/specs/generated/utility_piping.py
--rw-r--r--   0        0        0     6756 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/specs/generated/wood.py
--rw-r--r--   0        0        0     2079 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/specs/generated/wood_joists.py
--rw-r--r--   0        0        0     1535 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/standard.py
--rw-r--r--   0        0        0      837 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/validation/__init__.py
--rw-r--r--   0        0        0     2652 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/validation/common.py
--rw-r--r--   0        0        0     1105 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/validation/numbers.py
--rw-r--r--   0        0        0     7402 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/validation/quantity.py
--rw-r--r--   0        0        0     4690 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/versioning.py
--rw-r--r--   0        0        0        0 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/py.typed
--rw-r--r--   0        0        0     7790 1970-01-01 00:00:00.000000 openepd-3.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-06-03 15:02:47.203205 openepd-3.4.0/LICENSE
+-rw-r--r--   0        0        0     6786 2024-06-03 15:02:47.203205 openepd-3.4.0/README.md
+-rw-r--r--   0        0        0     3147 2024-06-03 15:02:47.203205 openepd-3.4.0/pyproject.toml
+-rw-r--r--   0        0        0      837 2024-06-03 15:02:47.203205 openepd-3.4.0/src/openepd/__init__.py
+-rw-r--r--   0        0        0      855 2024-06-03 15:02:47.203205 openepd-3.4.0/src/openepd/__version__.py
+-rw-r--r--   0        0        0      837 2024-06-03 15:02:47.203205 openepd-3.4.0/src/openepd/api/__init__.py
+-rw-r--r--   0        0        0    21142 2024-06-03 15:02:47.203205 openepd-3.4.0/src/openepd/api/base_sync_client.py
+-rw-r--r--   0        0        0      837 2024-06-03 15:02:47.203205 openepd-3.4.0/src/openepd/api/category/__init__.py
+-rw-r--r--   0        0        0     1067 2024-06-03 15:02:47.203205 openepd-3.4.0/src/openepd/api/category/dto.py
+-rw-r--r--   0        0        0     1588 2024-06-03 15:02:47.203205 openepd-3.4.0/src/openepd/api/category/sync_api.py
+-rw-r--r--   0        0        0     8681 2024-06-03 15:02:47.203205 openepd-3.4.0/src/openepd/api/common.py
+-rw-r--r--   0        0        0      837 2024-06-03 15:02:47.203205 openepd-3.4.0/src/openepd/api/dto/__init__.py
+-rw-r--r--   0        0        0     1250 2024-06-03 15:02:47.203205 openepd-3.4.0/src/openepd/api/dto/base.py
+-rw-r--r--   0        0        0     4705 2024-06-03 15:02:47.203205 openepd-3.4.0/src/openepd/api/dto/common.py
+-rw-r--r--   0        0        0     2377 2024-06-03 15:02:47.203205 openepd-3.4.0/src/openepd/api/dto/meta.py
+-rw-r--r--   0        0        0     2211 2024-06-03 15:02:47.203205 openepd-3.4.0/src/openepd/api/dto/mf.py
+-rw-r--r--   0        0        0      837 2024-06-03 15:02:47.203205 openepd-3.4.0/src/openepd/api/dto/params.py
+-rw-r--r--   0        0        0      837 2024-06-03 15:02:47.203205 openepd-3.4.0/src/openepd/api/epd/__init__.py
+-rw-r--r--   0        0        0     5091 2024-06-03 15:02:47.203205 openepd-3.4.0/src/openepd/api/epd/dto.py
+-rw-r--r--   0        0        0     4391 2024-06-03 15:02:47.203205 openepd-3.4.0/src/openepd/api/epd/sync_api.py
+-rw-r--r--   0        0        0     2376 2024-06-03 15:02:47.203205 openepd-3.4.0/src/openepd/api/errors.py
+-rw-r--r--   0        0        0      837 2024-06-03 15:02:47.203205 openepd-3.4.0/src/openepd/api/pcr/__init__.py
+-rw-r--r--   0        0        0     1649 2024-06-03 15:02:47.203205 openepd-3.4.0/src/openepd/api/pcr/dto.py
+-rw-r--r--   0        0        0     1805 2024-06-03 15:02:47.203205 openepd-3.4.0/src/openepd/api/pcr/sync_api.py
+-rw-r--r--   0        0        0     2504 2024-06-03 15:02:47.203205 openepd-3.4.0/src/openepd/api/sync_client.py
+-rw-r--r--   0        0        0      837 2024-06-03 15:02:47.207205 openepd-3.4.0/src/openepd/api/test/__init__.py
+-rw-r--r--   0        0        0      837 2024-06-03 15:02:47.207205 openepd-3.4.0/src/openepd/bundle/__init__.py
+-rw-r--r--   0        0        0     7086 2024-06-03 15:02:47.207205 openepd-3.4.0/src/openepd/bundle/base.py
+-rw-r--r--   0        0        0     2663 2024-06-03 15:02:47.207205 openepd-3.4.0/src/openepd/bundle/model.py
+-rw-r--r--   0        0        0     6904 2024-06-03 15:02:47.207205 openepd-3.4.0/src/openepd/bundle/reader.py
+-rw-r--r--   0        0        0     8353 2024-06-03 15:02:47.207205 openepd-3.4.0/src/openepd/bundle/writer.py
+-rw-r--r--   0        0        0      837 2024-06-03 15:02:47.207205 openepd-3.4.0/src/openepd/compat/__init__.py
+-rw-r--r--   0        0        0     1051 2024-06-03 15:02:47.207205 openepd-3.4.0/src/openepd/compat/compat_functional_validators.py
+-rw-r--r--   0        0        0     1363 2024-06-03 15:02:47.207205 openepd-3.4.0/src/openepd/compat/pydantic.py
+-rw-r--r--   0        0        0      837 2024-06-03 15:02:47.207205 openepd-3.4.0/src/openepd/model/__init__.py
+-rw-r--r--   0        0        0     9154 2024-06-03 15:02:47.207205 openepd-3.4.0/src/openepd/model/base.py
+-rw-r--r--   0        0        0     1856 2024-06-03 15:02:47.207205 openepd-3.4.0/src/openepd/model/category.py
+-rw-r--r--   0        0        0     5677 2024-06-03 15:02:47.207205 openepd-3.4.0/src/openepd/model/common.py
+-rw-r--r--   0        0        0    14299 2024-06-03 15:02:47.207205 openepd-3.4.0/src/openepd/model/epd.py
+-rw-r--r--   0        0        0     1918 2024-06-03 15:02:47.207205 openepd-3.4.0/src/openepd/model/factory.py
+-rw-r--r--   0        0        0    17165 2024-06-03 15:02:47.211205 openepd-3.4.0/src/openepd/model/lcia.py
+-rw-r--r--   0        0        0     4013 2024-06-03 15:02:47.211205 openepd-3.4.0/src/openepd/model/org.py
+-rw-r--r--   0        0        0     4620 2024-06-03 15:02:47.211205 openepd-3.4.0/src/openepd/model/pcr.py
+-rw-r--r--   0        0        0      862 2024-06-03 15:02:47.211205 openepd-3.4.0/src/openepd/model/specs/README.md
+-rw-r--r--   0        0        0     5176 2024-06-03 15:02:47.211205 openepd-3.4.0/src/openepd/model/specs/__init__.py
+-rw-r--r--   0        0        0     3549 2024-06-03 15:02:47.211205 openepd-3.4.0/src/openepd/model/specs/asphalt.py
+-rw-r--r--   0        0        0     2697 2024-06-03 15:02:47.211205 openepd-3.4.0/src/openepd/model/specs/base.py
+-rw-r--r--   0        0        0     9810 2024-06-03 15:02:47.211205 openepd-3.4.0/src/openepd/model/specs/concrete.py
+-rw-r--r--   0        0        0      837 2024-06-03 15:02:47.211205 openepd-3.4.0/src/openepd/model/specs/generated/__init__.py
+-rw-r--r--   0        0        0     2230 2024-06-03 15:02:47.211205 openepd-3.4.0/src/openepd/model/specs/generated/accessories.py
+-rw-r--r--   0        0        0     3161 2024-06-03 15:02:47.211205 openepd-3.4.0/src/openepd/model/specs/generated/aggregates.py
+-rw-r--r--   0        0        0     2630 2024-06-03 15:02:47.211205 openepd-3.4.0/src/openepd/model/specs/generated/aluminium.py
+-rw-r--r--   0        0        0     3369 2024-06-03 15:02:47.211205 openepd-3.4.0/src/openepd/model/specs/generated/asphalt.py
+-rw-r--r--   0        0        0     1092 2024-06-03 15:02:47.211205 openepd-3.4.0/src/openepd/model/specs/generated/bulk_materials.py
+-rw-r--r--   0        0        0     1172 2024-06-03 15:02:47.211205 openepd-3.4.0/src/openepd/model/specs/generated/cast_decks_and_underlayment.py
+-rw-r--r--   0        0        0     6779 2024-06-03 15:02:47.211205 openepd-3.4.0/src/openepd/model/specs/generated/cladding.py
+-rw-r--r--   0        0        0     2011 2024-06-03 15:02:47.211205 openepd-3.4.0/src/openepd/model/specs/generated/cmu.py
+-rw-r--r--   0        0        0     1117 2024-06-03 15:02:47.211205 openepd-3.4.0/src/openepd/model/specs/generated/common.py
+-rw-r--r--   0        0        0     7204 2024-06-03 15:02:47.211205 openepd-3.4.0/src/openepd/model/specs/generated/concrete.py
+-rw-r--r--   0        0        0     3269 2024-06-03 15:02:47.211205 openepd-3.4.0/src/openepd/model/specs/generated/conveying_equipment.py
+-rw-r--r--   0        0        0    10972 2024-06-03 15:02:47.211205 openepd-3.4.0/src/openepd/model/specs/generated/electrical.py
+-rw-r--r--   0        0        0     2195 2024-06-03 15:02:47.211205 openepd-3.4.0/src/openepd/model/specs/generated/electrical_transmission_and_distribution_equipment.py
+-rw-r--r--   0        0        0     1040 2024-06-03 15:02:47.211205 openepd-3.4.0/src/openepd/model/specs/generated/electricity.py
+-rw-r--r--   0        0        0    58546 2024-06-03 15:02:47.211205 openepd-3.4.0/src/openepd/model/specs/generated/enums.py
+-rw-r--r--   0        0        0    21338 2024-06-03 15:02:47.211205 openepd-3.4.0/src/openepd/model/specs/generated/finishes.py
+-rw-r--r--   0        0        0     3285 2024-06-03 15:02:47.211205 openepd-3.4.0/src/openepd/model/specs/generated/fire_and_smoke_protection.py
+-rw-r--r--   0        0        0     2798 2024-06-03 15:02:47.211205 openepd-3.4.0/src/openepd/model/specs/generated/furnishings.py
+-rw-r--r--   0        0        0     1151 2024-06-03 15:02:47.211205 openepd-3.4.0/src/openepd/model/specs/generated/grouting.py
+-rw-r--r--   0        0        0     5320 2024-06-03 15:02:47.211205 openepd-3.4.0/src/openepd/model/specs/generated/manufacturing_inputs.py
+-rw-r--r--   0        0        0     3286 2024-06-03 15:02:47.211205 openepd-3.4.0/src/openepd/model/specs/generated/masonry.py
+-rw-r--r--   0        0        0     1491 2024-06-03 15:02:47.211205 openepd-3.4.0/src/openepd/model/specs/generated/material_handling.py
+-rw-r--r--   0        0        0     9494 2024-06-03 15:02:47.211205 openepd-3.4.0/src/openepd/model/specs/generated/mechanical.py
+-rw-r--r--   0        0        0     1834 2024-06-03 15:02:47.211205 openepd-3.4.0/src/openepd/model/specs/generated/mechanical_insulation.py
+-rw-r--r--   0        0        0     8374 2024-06-03 15:02:47.211205 openepd-3.4.0/src/openepd/model/specs/generated/network_infrastructure.py
+-rw-r--r--   0        0        0    19035 2024-06-03 15:02:47.211205 openepd-3.4.0/src/openepd/model/specs/generated/openings.py
+-rw-r--r--   0        0        0     1031 2024-06-03 15:02:47.211205 openepd-3.4.0/src/openepd/model/specs/generated/other_electrical_equipment.py
+-rw-r--r--   0        0        0     3715 2024-06-03 15:02:47.211205 openepd-3.4.0/src/openepd/model/specs/generated/other_materials.py
+-rw-r--r--   0        0        0     4795 2024-06-03 15:02:47.211205 openepd-3.4.0/src/openepd/model/specs/generated/plumbing.py
+-rw-r--r--   0        0        0     7544 2024-06-03 15:02:47.211205 openepd-3.4.0/src/openepd/model/specs/generated/precast_concrete.py
+-rw-r--r--   0        0        0     3853 2024-06-03 15:02:47.211205 openepd-3.4.0/src/openepd/model/specs/generated/sheathing.py
+-rw-r--r--   0        0        0    10118 2024-06-03 15:02:47.211205 openepd-3.4.0/src/openepd/model/specs/generated/steel.py
+-rw-r--r--   0        0        0     8422 2024-06-03 15:02:47.211205 openepd-3.4.0/src/openepd/model/specs/generated/thermal_moisture_protection.py
+-rw-r--r--   0        0        0     2710 2024-06-03 15:02:47.211205 openepd-3.4.0/src/openepd/model/specs/generated/utility_piping.py
+-rw-r--r--   0        0        0     6756 2024-06-03 15:02:47.211205 openepd-3.4.0/src/openepd/model/specs/generated/wood.py
+-rw-r--r--   0        0        0     2079 2024-06-03 15:02:47.211205 openepd-3.4.0/src/openepd/model/specs/generated/wood_joists.py
+-rw-r--r--   0        0        0     1535 2024-06-03 15:02:47.211205 openepd-3.4.0/src/openepd/model/standard.py
+-rw-r--r--   0        0        0      837 2024-06-03 15:02:47.211205 openepd-3.4.0/src/openepd/model/validation/__init__.py
+-rw-r--r--   0        0        0     2652 2024-06-03 15:02:47.211205 openepd-3.4.0/src/openepd/model/validation/common.py
+-rw-r--r--   0        0        0     1105 2024-06-03 15:02:47.211205 openepd-3.4.0/src/openepd/model/validation/numbers.py
+-rw-r--r--   0        0        0     7523 2024-06-03 15:02:47.211205 openepd-3.4.0/src/openepd/model/validation/quantity.py
+-rw-r--r--   0        0        0     4690 2024-06-03 15:02:47.211205 openepd-3.4.0/src/openepd/model/versioning.py
+-rw-r--r--   0        0        0        0 2024-06-03 15:02:47.211205 openepd-3.4.0/src/openepd/py.typed
+-rw-r--r--   0        0        0     7790 1970-01-01 00:00:00.000000 openepd-3.4.0/PKG-INFO
```

### Comparing `openepd-3.3.0/LICENSE` & `openepd-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/README.md` & `openepd-3.4.0/README.md`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/pyproject.toml` & `openepd-3.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openepd"
-version = "3.3.0"
+version = "3.4.0"
 license = "Apache-2.0"
 description = "Python library to work with OpenEPD format"
 authors = ["C-Change Labs <support@c-change-labs.com>"]
 maintainers = ["C-Change Labs <open-source@c-change-labs.com>"]
 repository = "https://github.com/cchangelabs/openepd"
 keywords = []
 classifiers = [
```

### Comparing `openepd-3.3.0/src/openepd/__init__.py` & `openepd-3.4.0/src/openepd/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/__version__.py` & `openepd-3.4.0/src/openepd/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
-VERSION = "3.3.0"
+VERSION = "3.4.0"
```

### Comparing `openepd-3.3.0/src/openepd/api/__init__.py` & `openepd-3.4.0/src/openepd/api/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/api/base_sync_client.py` & `openepd-3.4.0/src/openepd/api/base_sync_client.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/api/category/__init__.py` & `openepd-3.4.0/src/openepd/api/category/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/api/category/dto.py` & `openepd-3.4.0/src/openepd/api/category/dto.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/api/category/sync_api.py` & `openepd-3.4.0/src/openepd/api/category/sync_api.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/api/common.py` & `openepd-3.4.0/src/openepd/api/common.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/api/dto/__init__.py` & `openepd-3.4.0/src/openepd/api/dto/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/api/dto/base.py` & `openepd-3.4.0/src/openepd/api/dto/base.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/api/dto/common.py` & `openepd-3.4.0/src/openepd/api/dto/common.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/api/dto/meta.py` & `openepd-3.4.0/src/openepd/api/dto/meta.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/api/dto/mf.py` & `openepd-3.4.0/src/openepd/api/dto/mf.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/api/dto/params.py` & `openepd-3.4.0/src/openepd/api/dto/params.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/api/epd/__init__.py` & `openepd-3.4.0/src/openepd/api/epd/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/api/epd/dto.py` & `openepd-3.4.0/src/openepd/api/epd/dto.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/api/epd/sync_api.py` & `openepd-3.4.0/src/openepd/api/epd/sync_api.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/api/errors.py` & `openepd-3.4.0/src/openepd/api/errors.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/api/pcr/__init__.py` & `openepd-3.4.0/src/openepd/api/pcr/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/api/pcr/dto.py` & `openepd-3.4.0/src/openepd/api/pcr/dto.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/api/pcr/sync_api.py` & `openepd-3.4.0/src/openepd/api/pcr/sync_api.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/api/sync_client.py` & `openepd-3.4.0/src/openepd/api/sync_client.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/api/test/__init__.py` & `openepd-3.4.0/src/openepd/api/test/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/bundle/__init__.py` & `openepd-3.4.0/src/openepd/bundle/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/bundle/base.py` & `openepd-3.4.0/src/openepd/bundle/base.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/bundle/model.py` & `openepd-3.4.0/src/openepd/bundle/model.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/bundle/reader.py` & `openepd-3.4.0/src/openepd/bundle/reader.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/bundle/writer.py` & `openepd-3.4.0/src/openepd/bundle/writer.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/compat/__init__.py` & `openepd-3.4.0/src/openepd/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/compat/compat_functional_validators.py` & `openepd-3.4.0/src/openepd/compat/compat_functional_validators.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/compat/pydantic.py` & `openepd-3.4.0/src/openepd/compat/pydantic.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/model/__init__.py` & `openepd-3.4.0/src/openepd/model/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/model/base.py` & `openepd-3.4.0/src/openepd/model/base.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/model/category.py` & `openepd-3.4.0/src/openepd/model/category.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/model/common.py` & `openepd-3.4.0/src/openepd/model/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,7 +149,8 @@
     t_km = "t * km"
     MPa = "MPa"
     item = "item"
     W = "W"
     use = "use"
     degree_c = "°C"
     kg_co2 = "kgCO2e"
+    hour = "hour"
```

### Comparing `openepd-3.3.0/src/openepd/model/epd.py` & `openepd-3.4.0/src/openepd/model/epd.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/model/factory.py` & `openepd-3.4.0/src/openepd/model/factory.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/model/lcia.py` & `openepd-3.4.0/src/openepd/model/lcia.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/model/org.py` & `openepd-3.4.0/src/openepd/model/org.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/model/pcr.py` & `openepd-3.4.0/src/openepd/model/pcr.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/model/specs/README.md` & `openepd-3.4.0/src/openepd/model/specs/README.md`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/model/specs/__init__.py` & `openepd-3.4.0/src/openepd/model/specs/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/model/specs/asphalt.py` & `openepd-3.4.0/src/openepd/model/specs/asphalt.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/model/specs/base.py` & `openepd-3.4.0/src/openepd/model/specs/base.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/model/specs/concrete.py` & `openepd-3.4.0/src/openepd/model/specs/concrete.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/model/specs/generated/__init__.py` & `openepd-3.4.0/src/openepd/model/specs/generated/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/model/specs/generated/accessories.py` & `openepd-3.4.0/src/openepd/model/specs/generated/accessories.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/model/specs/generated/aggregates.py` & `openepd-3.4.0/src/openepd/model/specs/generated/aggregates.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/model/specs/generated/aluminium.py` & `openepd-3.4.0/src/openepd/model/specs/generated/aluminium.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/model/specs/generated/asphalt.py` & `openepd-3.4.0/src/openepd/model/specs/generated/asphalt.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/model/specs/generated/bulk_materials.py` & `openepd-3.4.0/src/openepd/model/specs/generated/bulk_materials.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/model/specs/generated/cast_decks_and_underlayment.py` & `openepd-3.4.0/src/openepd/model/specs/generated/cast_decks_and_underlayment.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/model/specs/generated/cladding.py` & `openepd-3.4.0/src/openepd/model/specs/generated/cladding.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/model/specs/generated/cmu.py` & `openepd-3.4.0/src/openepd/model/specs/generated/cmu.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/model/specs/generated/common.py` & `openepd-3.4.0/src/openepd/model/specs/generated/common.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/model/specs/generated/concrete.py` & `openepd-3.4.0/src/openepd/model/specs/generated/concrete.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/model/specs/generated/conveying_equipment.py` & `openepd-3.4.0/src/openepd/model/specs/generated/utility_piping.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,33 +15,53 @@
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
 from openepd.compat.pydantic import pyd
 from openepd.model.specs.base import BaseOpenEpdHierarchicalSpec
-from openepd.model.specs.generated.enums import ElevatorsBuildingRise, ElevatorsUsageIntensity
-from openepd.model.validation.quantity import LengthMStr, MassKgStr, SpeedStr
+from openepd.model.specs.generated.enums import BuriedPipingType, PipingAnsiSchedule, UtilityPipingMaterial
+from openepd.model.validation.quantity import LengthMmStr, MassPerLengthStr
 
 
-class ElevatorsV1(BaseOpenEpdHierarchicalSpec):
-    """Car that moves in a vertical shaft to carry passengers or freight between the levels of a multistory building."""
+class BuildingHeatingPipingV1(BaseOpenEpdHierarchicalSpec):
+    """
+    Heating piping.
+
+    System of pipes used to supply heated fluids (liquids or steam) for purposes of controlling temperature inside a
+    home, business, or other building facility.
+    """
+
+    _EXT_VERSION = "1.0"
+
+
+class BuriedPipingV1(BaseOpenEpdHierarchicalSpec):
+    """System of pipes used to provide or transport fluids (liquids and gases) underground."""
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
-    usage_intensity: list[ElevatorsUsageIntensity] | None = pyd.Field(
-        default=None, description="", example=["Very low"]
+    buried_piping_type: list[BuriedPipingType] | None = pyd.Field(
+        default=None, description="", example=["Water Utilities"]
     )
-    travel_length: LengthMStr | None = pyd.Field(default=None, description="", example="1 m")
-    rated_load: MassKgStr | None = pyd.Field(default=None, description="", example="1 kg")
-    rated_speed: SpeedStr | None = pyd.Field(default=None, description="", example="1 m / s")
-    building_rise: ElevatorsBuildingRise | None = pyd.Field(default=None, description="", example="Low-rise")
 
 
-class ConveyingEquipmentV1(BaseOpenEpdHierarchicalSpec):
-    """Conveying Equipment."""
+class UtilityPipingV1(BaseOpenEpdHierarchicalSpec):
+    """
+    Utility piping.
+
+    System of pipes used to convey fluids (liquids and gases) from one location to another. Piping can be metal,
+    plastic, concrete, fiberglass, or other materials.
+    """
 
     _EXT_VERSION = "1.0"
 
+    # Own fields:
+    thickness: LengthMmStr | None = pyd.Field(default=None, description="", example="6 m")
+    piping_diameter: LengthMmStr | None = pyd.Field(default=None, description="", example="200 mm")
+    mass_per_unit_length: MassPerLengthStr | None = pyd.Field(default=None, description="", example="1 kg / m")
+    piping_ansi_schedule: PipingAnsiSchedule | None = pyd.Field(default=None, description="", example="5")
+    utility_piping_material: UtilityPipingMaterial | None = pyd.Field(default=None, description="", example="PVC")
+
     # Nested specs:
-    Elevators: ElevatorsV1 | None = None
+    BuildingHeatingPiping: BuildingHeatingPipingV1 | None = None
+    BuriedPiping: BuriedPipingV1 | None = None
```

### Comparing `openepd-3.3.0/src/openepd/model/specs/generated/electrical.py` & `openepd-3.4.0/src/openepd/model/specs/generated/electrical.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/model/specs/generated/electrical_transmission_and_distribution_equipment.py` & `openepd-3.4.0/src/openepd/model/specs/generated/electrical_transmission_and_distribution_equipment.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/model/specs/generated/electricity.py` & `openepd-3.4.0/src/openepd/model/specs/generated/electricity.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/model/specs/generated/enums.py` & `openepd-3.4.0/src/openepd/model/specs/generated/enums.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/model/specs/generated/finishes.py` & `openepd-3.4.0/src/openepd/model/specs/generated/finishes.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/model/specs/generated/fire_and_smoke_protection.py` & `openepd-3.4.0/src/openepd/model/specs/generated/fire_and_smoke_protection.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/model/specs/generated/furnishings.py` & `openepd-3.4.0/src/openepd/model/specs/generated/furnishings.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/model/specs/generated/grouting.py` & `openepd-3.4.0/src/openepd/model/specs/generated/grouting.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/model/specs/generated/manufacturing_inputs.py` & `openepd-3.4.0/src/openepd/model/specs/generated/manufacturing_inputs.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/model/specs/generated/masonry.py` & `openepd-3.4.0/src/openepd/model/specs/generated/masonry.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/model/specs/generated/material_handling.py` & `openepd-3.4.0/src/openepd/model/specs/generated/material_handling.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/model/specs/generated/mechanical.py` & `openepd-3.4.0/src/openepd/model/specs/generated/mechanical.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/model/specs/generated/mechanical_insulation.py` & `openepd-3.4.0/src/openepd/model/specs/generated/mechanical_insulation.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/model/specs/generated/network_infrastructure.py` & `openepd-3.4.0/src/openepd/model/specs/generated/network_infrastructure.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/model/specs/generated/openings.py` & `openepd-3.4.0/src/openepd/model/specs/generated/openings.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/model/specs/generated/other_electrical_equipment.py` & `openepd-3.4.0/src/openepd/model/specs/generated/other_electrical_equipment.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/model/specs/generated/other_materials.py` & `openepd-3.4.0/src/openepd/model/specs/generated/other_materials.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/model/specs/generated/plumbing.py` & `openepd-3.4.0/src/openepd/model/specs/generated/plumbing.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/model/specs/generated/precast_concrete.py` & `openepd-3.4.0/src/openepd/model/specs/generated/precast_concrete.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/model/specs/generated/sheathing.py` & `openepd-3.4.0/src/openepd/model/specs/generated/sheathing.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/model/specs/generated/steel.py` & `openepd-3.4.0/src/openepd/model/specs/generated/steel.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/model/specs/generated/thermal_moisture_protection.py` & `openepd-3.4.0/src/openepd/model/specs/generated/thermal_moisture_protection.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/model/specs/generated/utility_piping.py` & `openepd-3.4.0/src/openepd/model/specs/generated/wood_joists.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,54 +14,30 @@
 #  limitations under the License.
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
 from openepd.compat.pydantic import pyd
+from openepd.model.org import OrgRef
 from openepd.model.specs.base import BaseOpenEpdHierarchicalSpec
-from openepd.model.specs.generated.enums import BuriedPipingType, PipingAnsiSchedule, UtilityPipingMaterial
-from openepd.model.validation.quantity import LengthMmStr, MassPerLengthStr
+from openepd.model.specs.generated.common import HasForestPracticesCertifiers
+from openepd.model.specs.generated.enums import AllFabrication, AllTimberSpecies
 
 
-class BuildingHeatingPipingV1(BaseOpenEpdHierarchicalSpec):
+class WoodJoistsV1(BaseOpenEpdHierarchicalSpec, HasForestPracticesCertifiers):
     """
-    Heating piping.
+    Wood joists.
 
-    System of pipes used to supply heated fluids (liquids or steam) for purposes of controlling temperature inside a
-    home, business, or other building facility.
-    """
-
-    _EXT_VERSION = "1.0"
-
-
-class BuriedPipingV1(BaseOpenEpdHierarchicalSpec):
-    """System of pipes used to provide or transport fluids (liquids and gases) underground."""
-
-    _EXT_VERSION = "1.0"
-
-    # Own fields:
-    buried_piping_type: list[BuriedPipingType] | None = pyd.Field(
-        default=None, description="", example=["Water Utilities"]
-    )
-
-
-class UtilityPipingV1(BaseOpenEpdHierarchicalSpec):
-    """
-    Utility piping.
-
-    System of pipes used to convey fluids (liquids and gases) from one location to another. Piping can be metal,
-    plastic, concrete, fiberglass, or other materials.
+    Prefabricated I-shaped engineered wood structural members made primarily from one or more types of wood. Includes
+    products made with metallic webbing. Excludes products where the wood is merely decorative.
     """
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
-    thickness: LengthMmStr | None = pyd.Field(default=None, description="", example="6 m")
-    piping_diameter: LengthMmStr | None = pyd.Field(default=None, description="", example="200 mm")
-    mass_per_unit_length: MassPerLengthStr | None = pyd.Field(default=None, description="", example="1 kg / m")
-    piping_ansi_schedule: PipingAnsiSchedule | None = pyd.Field(default=None, description="", example="5")
-    utility_piping_material: UtilityPipingMaterial | None = pyd.Field(default=None, description="", example="PVC")
-
-    # Nested specs:
-    BuildingHeatingPiping: BuildingHeatingPipingV1 | None = None
-    BuriedPiping: BuriedPipingV1 | None = None
+    timber_species: AllTimberSpecies | None = pyd.Field(default=None, description="", example="Alaska Cedar")
+    fabrication: AllFabrication | None = pyd.Field(default=None, description="", example="LVL")
+    forest_practices_certifiers: list[OrgRef] | None = pyd.Field(default=None, description="")
+    weather_exposed: bool | None = pyd.Field(default=None, description="", example=True)
+    fire_retardant: bool | None = pyd.Field(default=None, description="", example=True)
+    decay_resistant: bool | None = pyd.Field(default=None, description="", example=True)
```

### Comparing `openepd-3.3.0/src/openepd/model/specs/generated/wood.py` & `openepd-3.4.0/src/openepd/model/specs/generated/wood.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/model/specs/generated/wood_joists.py` & `openepd-3.4.0/src/openepd/model/standard.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,30 +14,20 @@
 #  limitations under the License.
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
 from openepd.compat.pydantic import pyd
-from openepd.model.org import OrgRef
-from openepd.model.specs.base import BaseOpenEpdHierarchicalSpec
-from openepd.model.specs.generated.common import HasForestPracticesCertifiers
-from openepd.model.specs.generated.enums import AllFabrication, AllTimberSpecies
+from openepd.model.base import BaseOpenEpdSchema
+from openepd.model.org import Org
 
 
-class WoodJoistsV1(BaseOpenEpdHierarchicalSpec, HasForestPracticesCertifiers):
-    """
-    Wood joists.
+class Standard(BaseOpenEpdSchema):
+    """A standard, such as EN 15804, ISO 14044, ISO 14024:2018, etc."""
 
-    Prefabricated I-shaped engineered wood structural members made primarily from one or more types of wood. Includes
-    products made with metallic webbing. Excludes products where the wood is merely decorative.
-    """
-
-    _EXT_VERSION = "1.0"
-
-    # Own fields:
-    timber_species: AllTimberSpecies | None = pyd.Field(default=None, description="", example="Alaska Cedar")
-    fabrication: AllFabrication | None = pyd.Field(default=None, description="", example="LVL")
-    forest_practices_certifiers: list[OrgRef] | None = pyd.Field(default=None, description="")
-    weather_exposed: bool | None = pyd.Field(default=None, description="", example=True)
-    fire_retardant: bool | None = pyd.Field(default=None, description="", example=True)
-    decay_resistant: bool | None = pyd.Field(default=None, description="", example=True)
+    short_name: str = pyd.Field(description="Short-form of name of standard.  Must be unique. Case-insensitive")
+    name: str | None = pyd.Field(description="Full document name.  Must be unique. Case-insensitive", default=None)
+    link: pyd.AnyUrl | None = pyd.Field(
+        description="Link to the exact standard (including version) referred to", default=None
+    )
+    issuer: Org | None = pyd.Field(description="Org that issued this standard", default=None)
```

### Comparing `openepd-3.3.0/src/openepd/model/validation/__init__.py` & `openepd-3.4.0/src/openepd/model/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/model/validation/common.py` & `openepd-3.4.0/src/openepd/model/validation/common.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/model/validation/numbers.py` & `openepd-3.4.0/src/openepd/model/validation/numbers.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/src/openepd/model/validation/quantity.py` & `openepd-3.4.0/src/openepd/model/validation/quantity.py`

 * *Files 2% similar despite different names*

```diff
@@ -210,14 +210,20 @@
 
 class GwpKgCo2eStr(QuantityStr):
     """GWP intensity quantity type."""
 
     unit = OpenEPDUnit.kg_co2
 
 
+class CapacityPerHourStr(QuantityStr):
+    """Capacity per-hour quantity type."""
+
+    unit = f"{OpenEPDUnit.hour}^-1"
+
+
 class RValueStr(QuantityStr):
     """R-Value quantity type."""
 
     unit = "K * m2 / W"
 
 
 class SpeedStr(QuantityStr):
```

### Comparing `openepd-3.3.0/src/openepd/model/versioning.py` & `openepd-3.4.0/src/openepd/model/versioning.py`

 * *Files identical despite different names*

### Comparing `openepd-3.3.0/PKG-INFO` & `openepd-3.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openepd
-Version: 3.3.0
+Version: 3.4.0
 Summary: Python library to work with OpenEPD format
 Home-page: https://github.com/cchangelabs/openepd
 License: Apache-2.0
 Author: C-Change Labs
 Author-email: support@c-change-labs.com
 Maintainer: C-Change Labs
 Maintainer-email: open-source@c-change-labs.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: openepd Version: 3.3.0 Summary: Python library to
+Metadata-Version: 2.1 Name: openepd Version: 3.4.0 Summary: Python library to
 work with OpenEPD format Home-page: https://github.com/cchangelabs/openepd
 License: Apache-2.0 Author: C-Change Labs Author-email: support@c-change-
 labs.com Maintainer: C-Change Labs Maintainer-email: open-source@c-change-
 labs.com Requires-Python: >=3.11,<4.0 Classifier: Development Status :: 3 -
 Alpha Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Classifier:
```

