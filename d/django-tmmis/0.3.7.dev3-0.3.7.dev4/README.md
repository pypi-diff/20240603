# Comparing `tmp/django_tmmis-0.3.7.dev3.tar.gz` & `tmp/django_tmmis-0.3.7.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_tmmis-0.3.7.dev3.tar", last modified: Sun Jun  2 22:22:09 2024, max compression
+gzip compressed data, was "django_tmmis-0.3.7.dev4.tar", last modified: Sun Jun  2 22:28:42 2024, max compression
```

## Comparing `django_tmmis-0.3.7.dev3.tar` & `django_tmmis-0.3.7.dev4.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 22:22:09.462828 django_tmmis-0.3.7.dev3/
--rw-rw-rw-   0 root         (0) root         (0)       45 2023-01-26 18:08:54.000000 django_tmmis-0.3.7.dev3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2073 2024-06-02 22:22:09.462828 django_tmmis-0.3.7.dev3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1104 2023-02-07 19:50:12.000000 django_tmmis-0.3.7.dev3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 22:22:09.462828 django_tmmis-0.3.7.dev3/django_tmmis.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2073 2024-06-02 22:22:09.000000 django_tmmis-0.3.7.dev3/django_tmmis.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3684 2024-06-02 22:22:09.000000 django_tmmis-0.3.7.dev3/django_tmmis.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-06-02 22:22:09.000000 django_tmmis-0.3.7.dev3/django_tmmis.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-06-02 22:22:09.000000 django_tmmis-0.3.7.dev3/django_tmmis.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-06-02 22:22:09.000000 django_tmmis-0.3.7.dev3/django_tmmis.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1764 2024-06-02 19:19:49.000000 django_tmmis-0.3.7.dev3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-06-02 22:22:09.462828 django_tmmis-0.3.7.dev3/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 22:22:09.426828 django_tmmis-0.3.7.dev3/tmmis/
--rw-rw-rw-   0 root         (0) root         (0)      138 2023-03-07 07:01:36.000000 django_tmmis-0.3.7.dev3/tmmis/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-01-26 18:08:54.000000 django_tmmis-0.3.7.dev3/tmmis/admin.py
--rw-rw-rw-   0 root         (0) root         (0)       85 2023-02-06 02:22:49.000000 django_tmmis-0.3.7.dev3/tmmis/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     1168 2023-03-07 07:01:36.000000 django_tmmis-0.3.7.dev3/tmmis/handlers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 22:22:09.462828 django_tmmis-0.3.7.dev3/tmmis/models/
--rw-rw-rw-   0 root         (0) root         (0)     4728 2024-05-31 20:51:59.000000 django_tmmis-0.3.7.dev3/tmmis/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      994 2023-02-06 04:39:16.000000 django_tmmis-0.3.7.dev3/tmmis/models/atf_file_attachment.py
--rw-rw-rw-   0 root         (0) root         (0)     1817 2023-03-07 07:01:36.000000 django_tmmis-0.3.7.dev3/tmmis/models/atf_file_info.py
--rw-rw-rw-   0 root         (0) root         (0)      801 2023-02-06 04:39:16.000000 django_tmmis-0.3.7.dev3/tmmis/models/atf_file_type.py
--rw-rw-rw-   0 root         (0) root         (0)      506 2023-03-07 07:01:36.000000 django_tmmis-0.3.7.dev3/tmmis/models/base_model.py
--rw-rw-rw-   0 root         (0) root         (0)     1485 2023-02-06 02:22:49.000000 django_tmmis-0.3.7.dev3/tmmis/models/hlt_blank_template.py
--rw-rw-rw-   0 root         (0) root         (0)     3734 2023-02-06 02:22:49.000000 django_tmmis-0.3.7.dev3/tmmis/models/hlt_call_doctor.py
--rw-rw-rw-   0 root         (0) root         (0)      408 2023-02-06 02:22:49.000000 django_tmmis-0.3.7.dev3/tmmis/models/hlt_call_doctor_status.py
--rw-rw-rw-   0 root         (0) root         (0)      598 2023-03-07 07:01:36.000000 django_tmmis-0.3.7.dev3/tmmis/models/hlt_citizen.py
--rw-rw-rw-   0 root         (0) root         (0)     1682 2024-05-31 20:51:59.000000 django_tmmis-0.3.7.dev3/tmmis/models/hlt_disp_result_type.py
--rw-rw-rw-   0 root         (0) root         (0)     1354 2024-05-31 20:51:59.000000 django_tmmis-0.3.7.dev3/tmmis/models/hlt_disp_result_type_value.py
--rw-rw-rw-   0 root         (0) root         (0)     1826 2024-05-31 20:51:59.000000 django_tmmis-0.3.7.dev3/tmmis/models/hlt_disp_result_value.py
--rw-rw-rw-   0 root         (0) root         (0)     2078 2023-02-06 02:22:49.000000 django_tmmis-0.3.7.dev3/tmmis/models/hlt_doc_prvd.py
--rw-rw-rw-   0 root         (0) root         (0)     1440 2023-02-06 02:22:49.000000 django_tmmis-0.3.7.dev3/tmmis/models/hlt_doctor_time_table.py
--rw-rw-rw-   0 root         (0) root         (0)     2730 2023-02-06 02:22:49.000000 django_tmmis-0.3.7.dev3/tmmis/models/hlt_doctor_visit_table.py
--rw-rw-rw-   0 root         (0) root         (0)     1525 2023-02-06 04:39:16.000000 django_tmmis-0.3.7.dev3/tmmis/models/hlt_lpu_doctor.py
--rw-rw-rw-   0 root         (0) root         (0)     2667 2023-02-09 13:55:41.000000 django_tmmis-0.3.7.dev3/tmmis/models/hlt_med_record.py
--rw-rw-rw-   0 root         (0) root         (0)     7644 2023-03-07 07:01:36.000000 django_tmmis-0.3.7.dev3/tmmis/models/hlt_mkab.py
--rw-rw-rw-   0 root         (0) root         (0)     1933 2024-05-31 20:51:59.000000 django_tmmis-0.3.7.dev3/tmmis/models/hlt_mkb_tap.py
--rw-rw-rw-   0 root         (0) root         (0)     1089 2023-02-07 16:28:45.000000 django_tmmis-0.3.7.dev3/tmmis/models/hlt_polis_mkab.py
--rw-rw-rw-   0 root         (0) root         (0)      607 2023-02-06 02:22:49.000000 django_tmmis-0.3.7.dev3/tmmis/models/hlt_reason_care.py
--rw-rw-rw-   0 root         (0) root         (0)     3473 2023-02-06 02:22:49.000000 django_tmmis-0.3.7.dev3/tmmis/models/hlt_representative_mkab.py
--rw-rw-rw-   0 root         (0) root         (0)     3724 2023-02-07 13:16:56.000000 django_tmmis-0.3.7.dev3/tmmis/models/hlt_smtap.py
--rw-rw-rw-   0 root         (0) root         (0)     6309 2023-02-07 21:58:23.000000 django_tmmis-0.3.7.dev3/tmmis/models/hlt_tap.py
--rw-rw-rw-   0 root         (0) root         (0)      579 2023-02-06 02:22:49.000000 django_tmmis-0.3.7.dev3/tmmis/models/hlt_type_call_doctor.py
--rw-rw-rw-   0 root         (0) root         (0)     1018 2023-02-06 02:22:49.000000 django_tmmis-0.3.7.dev3/tmmis/models/hlt_uchastok.py
--rw-rw-rw-   0 root         (0) root         (0)     1306 2023-02-06 04:39:16.000000 django_tmmis-0.3.7.dev3/tmmis/models/hlt_visit_history.py
--rw-rw-rw-   0 root         (0) root         (0)     1076 2023-02-06 02:22:49.000000 django_tmmis-0.3.7.dev3/tmmis/models/kla_address.py
--rw-rw-rw-   0 root         (0) root         (0)      675 2023-02-06 02:22:49.000000 django_tmmis-0.3.7.dev3/tmmis/models/kla_house.py
--rw-rw-rw-   0 root         (0) root         (0)     1094 2023-02-06 02:22:49.000000 django_tmmis-0.3.7.dev3/tmmis/models/kla_kladr.py
--rw-rw-rw-   0 root         (0) root         (0)      984 2023-02-06 02:22:49.000000 django_tmmis-0.3.7.dev3/tmmis/models/kla_street.py
--rw-rw-rw-   0 root         (0) root         (0)      721 2023-03-07 07:01:36.000000 django_tmmis-0.3.7.dev3/tmmis/models/lbr_complex_research_type.py
--rw-rw-rw-   0 root         (0) root         (0)      742 2023-03-07 07:01:36.000000 django_tmmis-0.3.7.dev3/tmmis/models/lbr_histological_block.py
--rw-rw-rw-   0 root         (0) root         (0)      524 2023-03-07 07:01:36.000000 django_tmmis-0.3.7.dev3/tmmis/models/lbr_lab_direction_type.py
--rw-rw-rw-   0 root         (0) root         (0)      652 2023-03-07 07:01:36.000000 django_tmmis-0.3.7.dev3/tmmis/models/lbr_lab_research_cause.py
--rw-rw-rw-   0 root         (0) root         (0)      651 2023-03-07 07:01:36.000000 django_tmmis-0.3.7.dev3/tmmis/models/lbr_lab_research_target.py
--rw-rw-rw-   0 root         (0) root         (0)      877 2023-03-07 07:01:36.000000 django_tmmis-0.3.7.dev3/tmmis/models/lbr_laboratory.py
--rw-rw-rw-   0 root         (0) root         (0)      626 2023-03-07 07:01:36.000000 django_tmmis-0.3.7.dev3/tmmis/models/lbr_laboratory_kind.py
--rw-rw-rw-   0 root         (0) root         (0)     4525 2023-03-07 07:01:36.000000 django_tmmis-0.3.7.dev3/tmmis/models/lbr_laboratory_research.py
--rw-rw-rw-   0 root         (0) root         (0)     1112 2023-03-07 07:01:36.000000 django_tmmis-0.3.7.dev3/tmmis/models/lbr_laboratory_research_in_pack.py
--rw-rw-rw-   0 root         (0) root         (0)      636 2023-03-07 07:01:36.000000 django_tmmis-0.3.7.dev3/tmmis/models/lbr_laboratory_research_pack.py
--rw-rw-rw-   0 root         (0) root         (0)      695 2023-03-07 07:01:36.000000 django_tmmis-0.3.7.dev3/tmmis/models/lbr_laboratory_research_type.py
--rw-rw-rw-   0 root         (0) root         (0)      715 2023-03-07 07:01:36.000000 django_tmmis-0.3.7.dev3/tmmis/models/lbr_laboratory_type.py
--rw-rw-rw-   0 root         (0) root         (0)      752 2023-03-07 07:01:36.000000 django_tmmis-0.3.7.dev3/tmmis/models/lbr_option.py
--rw-rw-rw-   0 root         (0) root         (0)      586 2023-03-07 07:01:36.000000 django_tmmis-0.3.7.dev3/tmmis/models/lbr_option_enum_values.py
--rw-rw-rw-   0 root         (0) root         (0)      591 2023-03-07 07:01:36.000000 django_tmmis-0.3.7.dev3/tmmis/models/lbr_option_value.py
--rw-rw-rw-   0 root         (0) root         (0)      592 2023-03-07 07:01:36.000000 django_tmmis-0.3.7.dev3/tmmis/models/lbr_option_value_type.py
--rw-rw-rw-   0 root         (0) root         (0)     5351 2024-06-02 15:21:39.000000 django_tmmis-0.3.7.dev3/tmmis/models/lbr_research.py
--rw-rw-rw-   0 root         (0) root         (0)      917 2023-03-07 07:01:36.000000 django_tmmis-0.3.7.dev3/tmmis/models/lbr_research_journal.py
--rw-rw-rw-   0 root         (0) root         (0)      472 2023-03-07 07:01:36.000000 django_tmmis-0.3.7.dev3/tmmis/models/lbr_research_param_value_type.py
--rw-rw-rw-   0 root         (0) root         (0)      780 2023-03-07 07:01:36.000000 django_tmmis-0.3.7.dev3/tmmis/models/lbr_research_param_values.py
--rw-rw-rw-   0 root         (0) root         (0)     1874 2023-03-07 07:01:36.000000 django_tmmis-0.3.7.dev3/tmmis/models/lbr_research_result.py
--rw-rw-rw-   0 root         (0) root         (0)      990 2023-03-07 07:01:36.000000 django_tmmis-0.3.7.dev3/tmmis/models/lbr_research_sample.py
--rw-rw-rw-   0 root         (0) root         (0)      636 2023-03-07 07:01:36.000000 django_tmmis-0.3.7.dev3/tmmis/models/lbr_research_service.py
--rw-rw-rw-   0 root         (0) root         (0)      411 2023-03-07 07:01:36.000000 django_tmmis-0.3.7.dev3/tmmis/models/lbr_research_state.py
--rw-rw-rw-   0 root         (0) root         (0)     1780 2024-06-02 15:21:39.000000 django_tmmis-0.3.7.dev3/tmmis/models/lbr_research_type.py
--rw-rw-rw-   0 root         (0) root         (0)      725 2023-03-07 07:01:36.000000 django_tmmis-0.3.7.dev3/tmmis/models/lbr_research_type_in_pack.py
--rw-rw-rw-   0 root         (0) root         (0)      838 2023-03-07 07:01:36.000000 django_tmmis-0.3.7.dev3/tmmis/models/lbr_research_type_kind.py
--rw-rw-rw-   0 root         (0) root         (0)      595 2023-03-07 07:01:36.000000 django_tmmis-0.3.7.dev3/tmmis/models/lbr_research_type_kind_doc_prvd.py
--rw-rw-rw-   0 root         (0) root         (0)     2027 2023-03-07 07:01:36.000000 django_tmmis-0.3.7.dev3/tmmis/models/lbr_research_type_param.py
--rw-rw-rw-   0 root         (0) root         (0)      764 2023-03-07 07:01:36.000000 django_tmmis-0.3.7.dev3/tmmis/models/lbr_research_type_param_in_pack.py
--rw-rw-rw-   0 root         (0) root         (0)      840 2023-03-07 07:01:36.000000 django_tmmis-0.3.7.dev3/tmmis/models/lbr_research_type_param_to_research_type.py
--rw-rw-rw-   0 root         (0) root         (0)      632 2023-03-07 07:01:36.000000 django_tmmis-0.3.7.dev3/tmmis/models/lbr_research_type_to_lpu.py
--rw-rw-rw-   0 root         (0) root         (0)      576 2023-03-07 07:01:36.000000 django_tmmis-0.3.7.dev3/tmmis/models/lbr_research_type_to_profile.py
--rw-rw-rw-   0 root         (0) root         (0)     1638 2023-02-06 02:22:49.000000 django_tmmis-0.3.7.dev3/tmmis/models/oms_department.py
--rw-rw-rw-   0 root         (0) root         (0)      523 2023-02-06 02:22:49.000000 django_tmmis-0.3.7.dev3/tmmis/models/oms_kl_age_group.py
--rw-rw-rw-   0 root         (0) root         (0)      443 2023-02-06 02:22:49.000000 django_tmmis-0.3.7.dev3/tmmis/models/oms_kl_dd_service.py
--rw-rw-rw-   0 root         (0) root         (0)      467 2023-02-06 02:22:49.000000 django_tmmis-0.3.7.dev3/tmmis/models/oms_kl_department_profile.py
--rw-rw-rw-   0 root         (0) root         (0)      458 2023-02-06 02:22:49.000000 django_tmmis-0.3.7.dev3/tmmis/models/oms_kl_department_type.py
--rw-rw-rw-   0 root         (0) root         (0)      831 2023-02-07 16:51:22.000000 django_tmmis-0.3.7.dev3/tmmis/models/oms_kl_diagnos_type.py
--rw-rw-rw-   0 root         (0) root         (0)      449 2023-02-06 02:22:49.000000 django_tmmis-0.3.7.dev3/tmmis/models/oms_kl_disease_type.py
--rw-rw-rw-   0 root         (0) root         (0)      449 2023-02-06 02:22:49.000000 django_tmmis-0.3.7.dev3/tmmis/models/oms_kl_health_group.py
--rw-rw-rw-   0 root         (0) root         (0)      449 2023-02-06 02:22:49.000000 django_tmmis-0.3.7.dev3/tmmis/models/oms_kl_med_care_type.py
--rw-rw-rw-   0 root         (0) root         (0)      747 2024-05-31 20:51:59.000000 django_tmmis-0.3.7.dev3/tmmis/models/oms_kl_met_issl.py
--rw-rw-rw-   0 root         (0) root         (0)      434 2024-05-31 20:51:59.000000 django_tmmis-0.3.7.dev3/tmmis/models/oms_kl_nom_lpu.py
--rw-rw-rw-   0 root         (0) root         (0)      446 2024-05-31 20:51:59.000000 django_tmmis-0.3.7.dev3/tmmis/models/oms_kl_nom_service.py
--rw-rw-rw-   0 root         (0) root         (0)      880 2024-05-31 20:51:59.000000 django_tmmis-0.3.7.dev3/tmmis/models/oms_kl_nom_service_mkb_mse.py
--rw-rw-rw-   0 root         (0) root         (0)      524 2023-02-06 02:22:49.000000 django_tmmis-0.3.7.dev3/tmmis/models/oms_kl_profit_type.py
--rw-rw-rw-   0 root         (0) root         (0)      552 2023-02-06 02:22:49.000000 django_tmmis-0.3.7.dev3/tmmis/models/oms_kl_reason_type.py
--rw-rw-rw-   0 root         (0) root         (0)      544 2023-02-06 02:22:49.000000 django_tmmis-0.3.7.dev3/tmmis/models/oms_kl_soc_status.py
--rw-rw-rw-   0 root         (0) root         (0)      799 2023-02-06 02:22:49.000000 django_tmmis-0.3.7.dev3/tmmis/models/oms_kl_stat_cure_result.py
--rw-rw-rw-   0 root         (0) root         (0)      593 2023-02-06 02:22:49.000000 django_tmmis-0.3.7.dev3/tmmis/models/oms_kl_tip_oms.py
--rw-rw-rw-   0 root         (0) root         (0)      446 2023-02-06 02:22:49.000000 django_tmmis-0.3.7.dev3/tmmis/models/oms_kl_visit_place.py
--rw-rw-rw-   0 root         (0) root         (0)      952 2023-02-06 02:22:49.000000 django_tmmis-0.3.7.dev3/tmmis/models/oms_kl_visit_result.py
--rw-rw-rw-   0 root         (0) root         (0)     4240 2023-02-06 04:39:16.000000 django_tmmis-0.3.7.dev3/tmmis/models/oms_lpu.py
--rw-rw-rw-   0 root         (0) root         (0)      592 2023-02-06 02:22:49.000000 django_tmmis-0.3.7.dev3/tmmis/models/oms_mkb.py
--rw-rw-rw-   0 root         (0) root         (0)      778 2023-02-06 02:22:49.000000 django_tmmis-0.3.7.dev3/tmmis/models/oms_okato.py
--rw-rw-rw-   0 root         (0) root         (0)      689 2023-02-06 04:39:16.000000 django_tmmis-0.3.7.dev3/tmmis/models/oms_okved.py
--rw-rw-rw-   0 root         (0) root         (0)     2351 2023-02-06 04:39:16.000000 django_tmmis-0.3.7.dev3/tmmis/models/oms_organisation.py
--rw-rw-rw-   0 root         (0) root         (0)      644 2023-02-06 02:22:49.000000 django_tmmis-0.3.7.dev3/tmmis/models/oms_prvd.py
--rw-rw-rw-   0 root         (0) root         (0)     1047 2023-02-06 02:22:49.000000 django_tmmis-0.3.7.dev3/tmmis/models/oms_prvs.py
--rw-rw-rw-   0 root         (0) root         (0)     2625 2023-02-06 02:22:49.000000 django_tmmis-0.3.7.dev3/tmmis/models/oms_service_medical.py
--rw-rw-rw-   0 root         (0) root         (0)     2337 2023-02-06 02:22:49.000000 django_tmmis-0.3.7.dev3/tmmis/models/oms_smo.py
--rw-rw-rw-   0 root         (0) root         (0)      798 2023-02-06 02:22:49.000000 django_tmmis-0.3.7.dev3/tmmis/models/oms_type_doc.py
--rw-rw-rw-   0 root         (0) root         (0)     1780 2023-02-15 13:28:46.000000 django_tmmis-0.3.7.dev3/tmmis/models/x_doc_elem_def.py
--rw-rw-rw-   0 root         (0) root         (0)      983 2023-02-15 13:28:46.000000 django_tmmis-0.3.7.dev3/tmmis/models/x_doc_type_def.py
--rw-rw-rw-   0 root         (0) root         (0)      707 2023-02-06 02:22:49.000000 django_tmmis-0.3.7.dev3/tmmis/models/x_user.py
--rw-rw-rw-   0 root         (0) root         (0)      286 2023-02-06 02:22:49.000000 django_tmmis-0.3.7.dev3/tmmis/router.py
--rw-rw-rw-   0 root         (0) root         (0)       60 2023-01-26 18:08:54.000000 django_tmmis-0.3.7.dev3/tmmis/tests.py
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-01-26 18:08:54.000000 django_tmmis-0.3.7.dev3/tmmis/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 22:28:42.475242 django_tmmis-0.3.7.dev4/
+-rw-rw-rw-   0 root         (0) root         (0)       45 2023-01-27 12:40:20.000000 django_tmmis-0.3.7.dev4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2073 2024-06-02 22:28:42.475242 django_tmmis-0.3.7.dev4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1104 2023-02-07 21:01:04.000000 django_tmmis-0.3.7.dev4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 22:28:42.475242 django_tmmis-0.3.7.dev4/django_tmmis.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2073 2024-06-02 22:28:42.000000 django_tmmis-0.3.7.dev4/django_tmmis.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3684 2024-06-02 22:28:42.000000 django_tmmis-0.3.7.dev4/django_tmmis.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-06-02 22:28:42.000000 django_tmmis-0.3.7.dev4/django_tmmis.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-06-02 22:28:42.000000 django_tmmis-0.3.7.dev4/django_tmmis.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-06-02 22:28:42.000000 django_tmmis-0.3.7.dev4/django_tmmis.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1764 2024-06-02 19:31:11.000000 django_tmmis-0.3.7.dev4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-06-02 22:28:42.475242 django_tmmis-0.3.7.dev4/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 22:28:42.447242 django_tmmis-0.3.7.dev4/tmmis/
+-rw-rw-rw-   0 root         (0) root         (0)      138 2023-03-22 12:17:27.000000 django_tmmis-0.3.7.dev4/tmmis/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-01-27 12:40:20.000000 django_tmmis-0.3.7.dev4/tmmis/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)       85 2023-02-06 03:15:44.000000 django_tmmis-0.3.7.dev4/tmmis/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)     1168 2023-03-22 12:17:27.000000 django_tmmis-0.3.7.dev4/tmmis/handlers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 22:28:42.475242 django_tmmis-0.3.7.dev4/tmmis/models/
+-rw-rw-rw-   0 root         (0) root         (0)     4728 2024-05-31 20:29:16.000000 django_tmmis-0.3.7.dev4/tmmis/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      994 2023-02-06 04:20:19.000000 django_tmmis-0.3.7.dev4/tmmis/models/atf_file_attachment.py
+-rw-rw-rw-   0 root         (0) root         (0)     1817 2023-03-02 16:53:57.000000 django_tmmis-0.3.7.dev4/tmmis/models/atf_file_info.py
+-rw-rw-rw-   0 root         (0) root         (0)      801 2023-02-06 04:20:19.000000 django_tmmis-0.3.7.dev4/tmmis/models/atf_file_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      506 2023-03-02 16:53:57.000000 django_tmmis-0.3.7.dev4/tmmis/models/base_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1485 2023-02-06 03:15:44.000000 django_tmmis-0.3.7.dev4/tmmis/models/hlt_blank_template.py
+-rw-rw-rw-   0 root         (0) root         (0)     3734 2023-02-06 03:15:44.000000 django_tmmis-0.3.7.dev4/tmmis/models/hlt_call_doctor.py
+-rw-rw-rw-   0 root         (0) root         (0)      408 2023-02-06 03:15:44.000000 django_tmmis-0.3.7.dev4/tmmis/models/hlt_call_doctor_status.py
+-rw-rw-rw-   0 root         (0) root         (0)      598 2023-03-22 12:17:27.000000 django_tmmis-0.3.7.dev4/tmmis/models/hlt_citizen.py
+-rw-rw-rw-   0 root         (0) root         (0)     1682 2023-11-08 12:21:56.000000 django_tmmis-0.3.7.dev4/tmmis/models/hlt_disp_result_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     1354 2023-11-08 12:21:56.000000 django_tmmis-0.3.7.dev4/tmmis/models/hlt_disp_result_type_value.py
+-rw-rw-rw-   0 root         (0) root         (0)     1826 2023-11-08 12:21:56.000000 django_tmmis-0.3.7.dev4/tmmis/models/hlt_disp_result_value.py
+-rw-rw-rw-   0 root         (0) root         (0)     2078 2023-02-06 03:15:44.000000 django_tmmis-0.3.7.dev4/tmmis/models/hlt_doc_prvd.py
+-rw-rw-rw-   0 root         (0) root         (0)     1440 2023-02-06 03:15:44.000000 django_tmmis-0.3.7.dev4/tmmis/models/hlt_doctor_time_table.py
+-rw-rw-rw-   0 root         (0) root         (0)     2730 2023-02-06 03:15:44.000000 django_tmmis-0.3.7.dev4/tmmis/models/hlt_doctor_visit_table.py
+-rw-rw-rw-   0 root         (0) root         (0)     1525 2023-02-06 04:20:19.000000 django_tmmis-0.3.7.dev4/tmmis/models/hlt_lpu_doctor.py
+-rw-rw-rw-   0 root         (0) root         (0)     2667 2023-02-15 13:29:54.000000 django_tmmis-0.3.7.dev4/tmmis/models/hlt_med_record.py
+-rw-rw-rw-   0 root         (0) root         (0)     7644 2023-03-22 12:17:27.000000 django_tmmis-0.3.7.dev4/tmmis/models/hlt_mkab.py
+-rw-rw-rw-   0 root         (0) root         (0)     1933 2023-03-22 12:17:27.000000 django_tmmis-0.3.7.dev4/tmmis/models/hlt_mkb_tap.py
+-rw-rw-rw-   0 root         (0) root         (0)     1089 2023-02-07 13:46:24.000000 django_tmmis-0.3.7.dev4/tmmis/models/hlt_polis_mkab.py
+-rw-rw-rw-   0 root         (0) root         (0)      607 2023-02-06 03:15:44.000000 django_tmmis-0.3.7.dev4/tmmis/models/hlt_reason_care.py
+-rw-rw-rw-   0 root         (0) root         (0)     3473 2023-02-06 03:15:44.000000 django_tmmis-0.3.7.dev4/tmmis/models/hlt_representative_mkab.py
+-rw-rw-rw-   0 root         (0) root         (0)     3724 2023-02-06 11:21:28.000000 django_tmmis-0.3.7.dev4/tmmis/models/hlt_smtap.py
+-rw-rw-rw-   0 root         (0) root         (0)     6309 2023-02-07 21:57:19.000000 django_tmmis-0.3.7.dev4/tmmis/models/hlt_tap.py
+-rw-rw-rw-   0 root         (0) root         (0)      579 2023-02-06 03:15:44.000000 django_tmmis-0.3.7.dev4/tmmis/models/hlt_type_call_doctor.py
+-rw-rw-rw-   0 root         (0) root         (0)     1018 2023-02-06 03:15:44.000000 django_tmmis-0.3.7.dev4/tmmis/models/hlt_uchastok.py
+-rw-rw-rw-   0 root         (0) root         (0)     1306 2023-02-06 04:20:19.000000 django_tmmis-0.3.7.dev4/tmmis/models/hlt_visit_history.py
+-rw-rw-rw-   0 root         (0) root         (0)     1076 2023-02-06 03:15:44.000000 django_tmmis-0.3.7.dev4/tmmis/models/kla_address.py
+-rw-rw-rw-   0 root         (0) root         (0)      675 2023-02-06 03:15:44.000000 django_tmmis-0.3.7.dev4/tmmis/models/kla_house.py
+-rw-rw-rw-   0 root         (0) root         (0)     1094 2023-02-06 03:15:44.000000 django_tmmis-0.3.7.dev4/tmmis/models/kla_kladr.py
+-rw-rw-rw-   0 root         (0) root         (0)      984 2023-02-06 03:15:44.000000 django_tmmis-0.3.7.dev4/tmmis/models/kla_street.py
+-rw-rw-rw-   0 root         (0) root         (0)      721 2023-03-02 17:03:13.000000 django_tmmis-0.3.7.dev4/tmmis/models/lbr_complex_research_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      742 2023-03-02 16:53:57.000000 django_tmmis-0.3.7.dev4/tmmis/models/lbr_histological_block.py
+-rw-rw-rw-   0 root         (0) root         (0)      524 2023-03-02 17:03:13.000000 django_tmmis-0.3.7.dev4/tmmis/models/lbr_lab_direction_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      652 2023-03-02 16:53:57.000000 django_tmmis-0.3.7.dev4/tmmis/models/lbr_lab_research_cause.py
+-rw-rw-rw-   0 root         (0) root         (0)      651 2023-03-02 16:53:57.000000 django_tmmis-0.3.7.dev4/tmmis/models/lbr_lab_research_target.py
+-rw-rw-rw-   0 root         (0) root         (0)      877 2023-03-02 17:03:13.000000 django_tmmis-0.3.7.dev4/tmmis/models/lbr_laboratory.py
+-rw-rw-rw-   0 root         (0) root         (0)      626 2023-03-02 17:03:13.000000 django_tmmis-0.3.7.dev4/tmmis/models/lbr_laboratory_kind.py
+-rw-rw-rw-   0 root         (0) root         (0)     4525 2023-03-02 17:03:13.000000 django_tmmis-0.3.7.dev4/tmmis/models/lbr_laboratory_research.py
+-rw-rw-rw-   0 root         (0) root         (0)     1112 2023-03-02 17:03:13.000000 django_tmmis-0.3.7.dev4/tmmis/models/lbr_laboratory_research_in_pack.py
+-rw-rw-rw-   0 root         (0) root         (0)      636 2023-03-02 17:03:13.000000 django_tmmis-0.3.7.dev4/tmmis/models/lbr_laboratory_research_pack.py
+-rw-rw-rw-   0 root         (0) root         (0)      695 2023-03-02 17:03:13.000000 django_tmmis-0.3.7.dev4/tmmis/models/lbr_laboratory_research_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      715 2023-03-02 17:03:13.000000 django_tmmis-0.3.7.dev4/tmmis/models/lbr_laboratory_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      752 2023-03-02 16:53:57.000000 django_tmmis-0.3.7.dev4/tmmis/models/lbr_option.py
+-rw-rw-rw-   0 root         (0) root         (0)      586 2023-03-02 16:53:57.000000 django_tmmis-0.3.7.dev4/tmmis/models/lbr_option_enum_values.py
+-rw-rw-rw-   0 root         (0) root         (0)      591 2023-03-02 16:53:57.000000 django_tmmis-0.3.7.dev4/tmmis/models/lbr_option_value.py
+-rw-rw-rw-   0 root         (0) root         (0)      592 2023-03-02 16:53:57.000000 django_tmmis-0.3.7.dev4/tmmis/models/lbr_option_value_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     5351 2024-06-02 15:23:21.000000 django_tmmis-0.3.7.dev4/tmmis/models/lbr_research.py
+-rw-rw-rw-   0 root         (0) root         (0)      917 2023-03-02 16:53:57.000000 django_tmmis-0.3.7.dev4/tmmis/models/lbr_research_journal.py
+-rw-rw-rw-   0 root         (0) root         (0)      472 2023-03-02 16:53:57.000000 django_tmmis-0.3.7.dev4/tmmis/models/lbr_research_param_value_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      780 2023-03-02 17:03:13.000000 django_tmmis-0.3.7.dev4/tmmis/models/lbr_research_param_values.py
+-rw-rw-rw-   0 root         (0) root         (0)     1874 2023-03-02 17:03:13.000000 django_tmmis-0.3.7.dev4/tmmis/models/lbr_research_result.py
+-rw-rw-rw-   0 root         (0) root         (0)      990 2023-03-02 17:03:13.000000 django_tmmis-0.3.7.dev4/tmmis/models/lbr_research_sample.py
+-rw-rw-rw-   0 root         (0) root         (0)      636 2023-03-02 16:53:57.000000 django_tmmis-0.3.7.dev4/tmmis/models/lbr_research_service.py
+-rw-rw-rw-   0 root         (0) root         (0)      411 2023-03-02 16:53:57.000000 django_tmmis-0.3.7.dev4/tmmis/models/lbr_research_state.py
+-rw-rw-rw-   0 root         (0) root         (0)     1780 2024-06-02 15:23:21.000000 django_tmmis-0.3.7.dev4/tmmis/models/lbr_research_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      725 2023-03-02 17:03:13.000000 django_tmmis-0.3.7.dev4/tmmis/models/lbr_research_type_in_pack.py
+-rw-rw-rw-   0 root         (0) root         (0)      838 2023-03-02 17:03:13.000000 django_tmmis-0.3.7.dev4/tmmis/models/lbr_research_type_kind.py
+-rw-rw-rw-   0 root         (0) root         (0)      595 2023-03-02 17:03:13.000000 django_tmmis-0.3.7.dev4/tmmis/models/lbr_research_type_kind_doc_prvd.py
+-rw-rw-rw-   0 root         (0) root         (0)     2027 2023-03-02 17:03:13.000000 django_tmmis-0.3.7.dev4/tmmis/models/lbr_research_type_param.py
+-rw-rw-rw-   0 root         (0) root         (0)      764 2023-03-02 17:03:13.000000 django_tmmis-0.3.7.dev4/tmmis/models/lbr_research_type_param_in_pack.py
+-rw-rw-rw-   0 root         (0) root         (0)      840 2023-03-02 17:03:13.000000 django_tmmis-0.3.7.dev4/tmmis/models/lbr_research_type_param_to_research_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      632 2023-03-02 16:53:57.000000 django_tmmis-0.3.7.dev4/tmmis/models/lbr_research_type_to_lpu.py
+-rw-rw-rw-   0 root         (0) root         (0)      576 2023-03-02 17:03:13.000000 django_tmmis-0.3.7.dev4/tmmis/models/lbr_research_type_to_profile.py
+-rw-rw-rw-   0 root         (0) root         (0)     1638 2023-02-06 03:15:44.000000 django_tmmis-0.3.7.dev4/tmmis/models/oms_department.py
+-rw-rw-rw-   0 root         (0) root         (0)      523 2023-02-06 03:15:44.000000 django_tmmis-0.3.7.dev4/tmmis/models/oms_kl_age_group.py
+-rw-rw-rw-   0 root         (0) root         (0)      443 2023-02-06 03:15:44.000000 django_tmmis-0.3.7.dev4/tmmis/models/oms_kl_dd_service.py
+-rw-rw-rw-   0 root         (0) root         (0)      467 2023-02-06 03:15:44.000000 django_tmmis-0.3.7.dev4/tmmis/models/oms_kl_department_profile.py
+-rw-rw-rw-   0 root         (0) root         (0)      458 2023-02-06 03:15:44.000000 django_tmmis-0.3.7.dev4/tmmis/models/oms_kl_department_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      831 2023-02-07 17:01:22.000000 django_tmmis-0.3.7.dev4/tmmis/models/oms_kl_diagnos_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      449 2023-02-06 03:15:44.000000 django_tmmis-0.3.7.dev4/tmmis/models/oms_kl_disease_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      449 2023-02-06 03:15:44.000000 django_tmmis-0.3.7.dev4/tmmis/models/oms_kl_health_group.py
+-rw-rw-rw-   0 root         (0) root         (0)      449 2023-02-06 03:15:44.000000 django_tmmis-0.3.7.dev4/tmmis/models/oms_kl_med_care_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      747 2024-05-31 20:29:16.000000 django_tmmis-0.3.7.dev4/tmmis/models/oms_kl_met_issl.py
+-rw-rw-rw-   0 root         (0) root         (0)      434 2024-05-31 20:29:16.000000 django_tmmis-0.3.7.dev4/tmmis/models/oms_kl_nom_lpu.py
+-rw-rw-rw-   0 root         (0) root         (0)      446 2024-05-31 20:29:16.000000 django_tmmis-0.3.7.dev4/tmmis/models/oms_kl_nom_service.py
+-rw-rw-rw-   0 root         (0) root         (0)      880 2024-05-31 20:29:16.000000 django_tmmis-0.3.7.dev4/tmmis/models/oms_kl_nom_service_mkb_mse.py
+-rw-rw-rw-   0 root         (0) root         (0)      524 2023-02-06 03:15:44.000000 django_tmmis-0.3.7.dev4/tmmis/models/oms_kl_profit_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      552 2023-02-06 03:15:44.000000 django_tmmis-0.3.7.dev4/tmmis/models/oms_kl_reason_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      544 2023-02-06 03:15:44.000000 django_tmmis-0.3.7.dev4/tmmis/models/oms_kl_soc_status.py
+-rw-rw-rw-   0 root         (0) root         (0)      799 2023-02-06 03:15:44.000000 django_tmmis-0.3.7.dev4/tmmis/models/oms_kl_stat_cure_result.py
+-rw-rw-rw-   0 root         (0) root         (0)      593 2023-02-06 03:15:44.000000 django_tmmis-0.3.7.dev4/tmmis/models/oms_kl_tip_oms.py
+-rw-rw-rw-   0 root         (0) root         (0)      446 2023-02-06 03:15:44.000000 django_tmmis-0.3.7.dev4/tmmis/models/oms_kl_visit_place.py
+-rw-rw-rw-   0 root         (0) root         (0)      952 2023-02-06 03:15:44.000000 django_tmmis-0.3.7.dev4/tmmis/models/oms_kl_visit_result.py
+-rw-rw-rw-   0 root         (0) root         (0)     4240 2023-02-06 04:20:19.000000 django_tmmis-0.3.7.dev4/tmmis/models/oms_lpu.py
+-rw-rw-rw-   0 root         (0) root         (0)      592 2023-02-06 03:15:44.000000 django_tmmis-0.3.7.dev4/tmmis/models/oms_mkb.py
+-rw-rw-rw-   0 root         (0) root         (0)      778 2023-02-06 03:15:44.000000 django_tmmis-0.3.7.dev4/tmmis/models/oms_okato.py
+-rw-rw-rw-   0 root         (0) root         (0)      689 2023-02-06 04:20:19.000000 django_tmmis-0.3.7.dev4/tmmis/models/oms_okved.py
+-rw-rw-rw-   0 root         (0) root         (0)     2351 2023-02-06 04:20:19.000000 django_tmmis-0.3.7.dev4/tmmis/models/oms_organisation.py
+-rw-rw-rw-   0 root         (0) root         (0)      644 2023-02-06 03:15:44.000000 django_tmmis-0.3.7.dev4/tmmis/models/oms_prvd.py
+-rw-rw-rw-   0 root         (0) root         (0)     1047 2023-02-06 03:15:44.000000 django_tmmis-0.3.7.dev4/tmmis/models/oms_prvs.py
+-rw-rw-rw-   0 root         (0) root         (0)     2625 2023-02-06 03:15:44.000000 django_tmmis-0.3.7.dev4/tmmis/models/oms_service_medical.py
+-rw-rw-rw-   0 root         (0) root         (0)     2337 2023-02-06 03:15:44.000000 django_tmmis-0.3.7.dev4/tmmis/models/oms_smo.py
+-rw-rw-rw-   0 root         (0) root         (0)      798 2023-02-06 03:15:44.000000 django_tmmis-0.3.7.dev4/tmmis/models/oms_type_doc.py
+-rw-rw-rw-   0 root         (0) root         (0)     1780 2023-02-15 13:29:54.000000 django_tmmis-0.3.7.dev4/tmmis/models/x_doc_elem_def.py
+-rw-rw-rw-   0 root         (0) root         (0)      983 2023-02-15 13:29:54.000000 django_tmmis-0.3.7.dev4/tmmis/models/x_doc_type_def.py
+-rw-rw-rw-   0 root         (0) root         (0)      707 2023-02-06 03:15:44.000000 django_tmmis-0.3.7.dev4/tmmis/models/x_user.py
+-rw-rw-rw-   0 root         (0) root         (0)      286 2023-02-06 03:15:44.000000 django_tmmis-0.3.7.dev4/tmmis/router.py
+-rw-rw-rw-   0 root         (0) root         (0)       60 2023-01-27 12:40:20.000000 django_tmmis-0.3.7.dev4/tmmis/tests.py
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-01-27 12:40:20.000000 django_tmmis-0.3.7.dev4/tmmis/views.py
```

### Comparing `django_tmmis-0.3.7.dev3/PKG-INFO` & `django_tmmis-0.3.7.dev4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-tmmis
-Version: 0.3.7.dev3
+Version: 0.3.7.dev4
 Summary: A Django app provided ORM to TrustMed medical information system
 Author-email: Chmelyuk Vladislav <neimp@yandex.ru>
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
```

### Comparing `django_tmmis-0.3.7.dev3/README.md` & `django_tmmis-0.3.7.dev4/README.md`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/django_tmmis.egg-info/PKG-INFO` & `django_tmmis-0.3.7.dev4/django_tmmis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-tmmis
-Version: 0.3.7.dev3
+Version: 0.3.7.dev4
 Summary: A Django app provided ORM to TrustMed medical information system
 Author-email: Chmelyuk Vladislav <neimp@yandex.ru>
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
```

### Comparing `django_tmmis-0.3.7.dev3/django_tmmis.egg-info/SOURCES.txt` & `django_tmmis-0.3.7.dev4/django_tmmis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/pyproject.toml` & `django_tmmis-0.3.7.dev4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/handlers.py` & `django_tmmis-0.3.7.dev4/tmmis/handlers.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/__init__.py` & `django_tmmis-0.3.7.dev4/tmmis/models/__init__.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/atf_file_attachment.py` & `django_tmmis-0.3.7.dev4/tmmis/models/atf_file_attachment.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/atf_file_info.py` & `django_tmmis-0.3.7.dev4/tmmis/models/atf_file_info.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/atf_file_type.py` & `django_tmmis-0.3.7.dev4/tmmis/models/atf_file_type.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/hlt_blank_template.py` & `django_tmmis-0.3.7.dev4/tmmis/models/hlt_blank_template.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/hlt_call_doctor.py` & `django_tmmis-0.3.7.dev4/tmmis/models/hlt_call_doctor.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/hlt_citizen.py` & `django_tmmis-0.3.7.dev4/tmmis/models/hlt_citizen.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/hlt_disp_result_type.py` & `django_tmmis-0.3.7.dev4/tmmis/models/hlt_disp_result_type.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/hlt_disp_result_type_value.py` & `django_tmmis-0.3.7.dev4/tmmis/models/hlt_disp_result_type_value.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/hlt_disp_result_value.py` & `django_tmmis-0.3.7.dev4/tmmis/models/hlt_disp_result_value.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/hlt_doc_prvd.py` & `django_tmmis-0.3.7.dev4/tmmis/models/hlt_doc_prvd.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/hlt_doctor_time_table.py` & `django_tmmis-0.3.7.dev4/tmmis/models/hlt_doctor_time_table.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/hlt_doctor_visit_table.py` & `django_tmmis-0.3.7.dev4/tmmis/models/hlt_doctor_visit_table.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/hlt_lpu_doctor.py` & `django_tmmis-0.3.7.dev4/tmmis/models/hlt_lpu_doctor.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/hlt_med_record.py` & `django_tmmis-0.3.7.dev4/tmmis/models/hlt_med_record.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/hlt_mkab.py` & `django_tmmis-0.3.7.dev4/tmmis/models/hlt_mkab.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/hlt_mkb_tap.py` & `django_tmmis-0.3.7.dev4/tmmis/models/hlt_mkb_tap.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/hlt_polis_mkab.py` & `django_tmmis-0.3.7.dev4/tmmis/models/hlt_polis_mkab.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/hlt_reason_care.py` & `django_tmmis-0.3.7.dev4/tmmis/models/hlt_reason_care.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/hlt_representative_mkab.py` & `django_tmmis-0.3.7.dev4/tmmis/models/hlt_representative_mkab.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/hlt_smtap.py` & `django_tmmis-0.3.7.dev4/tmmis/models/hlt_smtap.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/hlt_tap.py` & `django_tmmis-0.3.7.dev4/tmmis/models/hlt_tap.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/hlt_type_call_doctor.py` & `django_tmmis-0.3.7.dev4/tmmis/models/hlt_type_call_doctor.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/hlt_uchastok.py` & `django_tmmis-0.3.7.dev4/tmmis/models/hlt_uchastok.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/hlt_visit_history.py` & `django_tmmis-0.3.7.dev4/tmmis/models/hlt_visit_history.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/kla_address.py` & `django_tmmis-0.3.7.dev4/tmmis/models/kla_address.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/kla_house.py` & `django_tmmis-0.3.7.dev4/tmmis/models/kla_house.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/kla_kladr.py` & `django_tmmis-0.3.7.dev4/tmmis/models/kla_kladr.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/kla_street.py` & `django_tmmis-0.3.7.dev4/tmmis/models/kla_street.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/lbr_complex_research_type.py` & `django_tmmis-0.3.7.dev4/tmmis/models/lbr_complex_research_type.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/lbr_histological_block.py` & `django_tmmis-0.3.7.dev4/tmmis/models/lbr_histological_block.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/lbr_lab_direction_type.py` & `django_tmmis-0.3.7.dev4/tmmis/models/lbr_lab_direction_type.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/lbr_lab_research_cause.py` & `django_tmmis-0.3.7.dev4/tmmis/models/lbr_lab_research_cause.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/lbr_lab_research_target.py` & `django_tmmis-0.3.7.dev4/tmmis/models/lbr_lab_research_target.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/lbr_laboratory.py` & `django_tmmis-0.3.7.dev4/tmmis/models/lbr_laboratory.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/lbr_laboratory_kind.py` & `django_tmmis-0.3.7.dev4/tmmis/models/lbr_laboratory_kind.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/lbr_laboratory_research.py` & `django_tmmis-0.3.7.dev4/tmmis/models/lbr_laboratory_research.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/lbr_laboratory_research_in_pack.py` & `django_tmmis-0.3.7.dev4/tmmis/models/lbr_laboratory_research_in_pack.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/lbr_laboratory_research_pack.py` & `django_tmmis-0.3.7.dev4/tmmis/models/lbr_laboratory_research_pack.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/lbr_laboratory_research_type.py` & `django_tmmis-0.3.7.dev4/tmmis/models/lbr_laboratory_research_type.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/lbr_laboratory_type.py` & `django_tmmis-0.3.7.dev4/tmmis/models/lbr_laboratory_type.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/lbr_option.py` & `django_tmmis-0.3.7.dev4/tmmis/models/lbr_option.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/lbr_option_enum_values.py` & `django_tmmis-0.3.7.dev4/tmmis/models/lbr_option_enum_values.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/lbr_option_value.py` & `django_tmmis-0.3.7.dev4/tmmis/models/lbr_option_value.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/lbr_option_value_type.py` & `django_tmmis-0.3.7.dev4/tmmis/models/lbr_option_value_type.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/lbr_research.py` & `django_tmmis-0.3.7.dev4/tmmis/models/lbr_research.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/lbr_research_journal.py` & `django_tmmis-0.3.7.dev4/tmmis/models/lbr_research_journal.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/lbr_research_param_values.py` & `django_tmmis-0.3.7.dev4/tmmis/models/lbr_research_param_values.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/lbr_research_result.py` & `django_tmmis-0.3.7.dev4/tmmis/models/lbr_research_result.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/lbr_research_sample.py` & `django_tmmis-0.3.7.dev4/tmmis/models/lbr_research_sample.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/lbr_research_service.py` & `django_tmmis-0.3.7.dev4/tmmis/models/lbr_research_service.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/lbr_research_type.py` & `django_tmmis-0.3.7.dev4/tmmis/models/lbr_research_type.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/lbr_research_type_in_pack.py` & `django_tmmis-0.3.7.dev4/tmmis/models/lbr_research_type_in_pack.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/lbr_research_type_kind.py` & `django_tmmis-0.3.7.dev4/tmmis/models/lbr_research_type_kind.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/lbr_research_type_kind_doc_prvd.py` & `django_tmmis-0.3.7.dev4/tmmis/models/lbr_research_type_kind_doc_prvd.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/lbr_research_type_param.py` & `django_tmmis-0.3.7.dev4/tmmis/models/lbr_research_type_param.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/lbr_research_type_param_in_pack.py` & `django_tmmis-0.3.7.dev4/tmmis/models/lbr_research_type_param_in_pack.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/lbr_research_type_param_to_research_type.py` & `django_tmmis-0.3.7.dev4/tmmis/models/lbr_research_type_param_to_research_type.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/lbr_research_type_to_lpu.py` & `django_tmmis-0.3.7.dev4/tmmis/models/lbr_research_type_to_lpu.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/lbr_research_type_to_profile.py` & `django_tmmis-0.3.7.dev4/tmmis/models/lbr_research_type_to_profile.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/oms_department.py` & `django_tmmis-0.3.7.dev4/tmmis/models/oms_department.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/oms_kl_age_group.py` & `django_tmmis-0.3.7.dev4/tmmis/models/oms_kl_age_group.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/oms_kl_diagnos_type.py` & `django_tmmis-0.3.7.dev4/tmmis/models/oms_kl_diagnos_type.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/oms_kl_met_issl.py` & `django_tmmis-0.3.7.dev4/tmmis/models/oms_kl_met_issl.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/oms_kl_nom_service_mkb_mse.py` & `django_tmmis-0.3.7.dev4/tmmis/models/oms_kl_nom_service_mkb_mse.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/oms_kl_profit_type.py` & `django_tmmis-0.3.7.dev4/tmmis/models/oms_kl_profit_type.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/oms_kl_reason_type.py` & `django_tmmis-0.3.7.dev4/tmmis/models/oms_kl_reason_type.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/oms_kl_soc_status.py` & `django_tmmis-0.3.7.dev4/tmmis/models/oms_kl_soc_status.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/oms_kl_stat_cure_result.py` & `django_tmmis-0.3.7.dev4/tmmis/models/oms_kl_stat_cure_result.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/oms_kl_tip_oms.py` & `django_tmmis-0.3.7.dev4/tmmis/models/oms_kl_tip_oms.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/oms_kl_visit_result.py` & `django_tmmis-0.3.7.dev4/tmmis/models/oms_kl_visit_result.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/oms_lpu.py` & `django_tmmis-0.3.7.dev4/tmmis/models/oms_lpu.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/oms_mkb.py` & `django_tmmis-0.3.7.dev4/tmmis/models/oms_mkb.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/oms_okato.py` & `django_tmmis-0.3.7.dev4/tmmis/models/oms_okato.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/oms_okved.py` & `django_tmmis-0.3.7.dev4/tmmis/models/oms_okved.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/oms_organisation.py` & `django_tmmis-0.3.7.dev4/tmmis/models/oms_organisation.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/oms_prvd.py` & `django_tmmis-0.3.7.dev4/tmmis/models/oms_prvd.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/oms_prvs.py` & `django_tmmis-0.3.7.dev4/tmmis/models/oms_prvs.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/oms_service_medical.py` & `django_tmmis-0.3.7.dev4/tmmis/models/oms_service_medical.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/oms_smo.py` & `django_tmmis-0.3.7.dev4/tmmis/models/oms_smo.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/oms_type_doc.py` & `django_tmmis-0.3.7.dev4/tmmis/models/oms_type_doc.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/x_doc_elem_def.py` & `django_tmmis-0.3.7.dev4/tmmis/models/x_doc_elem_def.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/x_doc_type_def.py` & `django_tmmis-0.3.7.dev4/tmmis/models/x_doc_type_def.py`

 * *Files identical despite different names*

### Comparing `django_tmmis-0.3.7.dev3/tmmis/models/x_user.py` & `django_tmmis-0.3.7.dev4/tmmis/models/x_user.py`

 * *Files identical despite different names*

