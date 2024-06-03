# Comparing `tmp/django-tmmis-0.3.6.tar.gz` & `tmp/django_tmmis-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-tmmis-0.3.6.tar", last modified: Wed Nov  8 12:21:17 2023, max compression
+gzip compressed data, was "django_tmmis-0.3.9.tar", last modified: Mon Jun  3 06:28:15 2024, max compression
```

## Comparing `django-tmmis-0.3.6.tar` & `django_tmmis-0.3.9.tar`

### file list

```diff
@@ -1,116 +1,118 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-08 12:21:17.323343 django-tmmis-0.3.6/
--rw-rw-rw-   0 root         (0) root         (0)       45 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2079 2023-11-08 12:21:17.323343 django-tmmis-0.3.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1104 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-08 12:21:17.283343 django-tmmis-0.3.6/django_tmmis.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2079 2023-11-08 12:21:17.000000 django-tmmis-0.3.6/django_tmmis.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3594 2023-11-08 12:21:17.000000 django-tmmis-0.3.6/django_tmmis.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-11-08 12:21:17.000000 django-tmmis-0.3.6/django_tmmis.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-11-08 12:21:17.000000 django-tmmis-0.3.6/django_tmmis.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-11-08 12:21:17.000000 django-tmmis-0.3.6/django_tmmis.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      920 2023-11-08 12:21:17.323343 django-tmmis-0.3.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      113 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-08 12:21:17.287343 django-tmmis-0.3.6/tmmis/
--rw-rw-rw-   0 root         (0) root         (0)      138 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/admin.py
--rw-rw-rw-   0 root         (0) root         (0)       85 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     1168 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/handlers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-08 12:21:17.319343 django-tmmis-0.3.6/tmmis/models/
--rw-rw-rw-   0 root         (0) root         (0)     4433 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      994 2023-02-06 03:36:56.000000 django-tmmis-0.3.6/tmmis/models/atf_file_attachment.py
--rw-rw-rw-   0 root         (0) root         (0)     1817 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/atf_file_info.py
--rw-rw-rw-   0 root         (0) root         (0)      801 2023-02-06 03:36:56.000000 django-tmmis-0.3.6/tmmis/models/atf_file_type.py
--rw-rw-rw-   0 root         (0) root         (0)      506 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/base_model.py
--rw-rw-rw-   0 root         (0) root         (0)     1485 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/models/hlt_blank_template.py
--rw-rw-rw-   0 root         (0) root         (0)     3734 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/models/hlt_call_doctor.py
--rw-rw-rw-   0 root         (0) root         (0)      408 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/models/hlt_call_doctor_status.py
--rw-rw-rw-   0 root         (0) root         (0)      598 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/hlt_citizen.py
--rw-rw-rw-   0 root         (0) root         (0)     1682 2023-11-08 12:20:29.000000 django-tmmis-0.3.6/tmmis/models/hlt_disp_result_type.py
--rw-rw-rw-   0 root         (0) root         (0)     1354 2023-11-08 12:20:29.000000 django-tmmis-0.3.6/tmmis/models/hlt_disp_result_type_value.py
--rw-rw-rw-   0 root         (0) root         (0)     1826 2023-11-08 12:20:29.000000 django-tmmis-0.3.6/tmmis/models/hlt_disp_result_value.py
--rw-rw-rw-   0 root         (0) root         (0)     2078 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/models/hlt_doc_prvd.py
--rw-rw-rw-   0 root         (0) root         (0)     1440 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/models/hlt_doctor_time_table.py
--rw-rw-rw-   0 root         (0) root         (0)     2730 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/models/hlt_doctor_visit_table.py
--rw-rw-rw-   0 root         (0) root         (0)     1525 2023-02-06 03:36:56.000000 django-tmmis-0.3.6/tmmis/models/hlt_lpu_doctor.py
--rw-rw-rw-   0 root         (0) root         (0)     2667 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/hlt_med_record.py
--rw-rw-rw-   0 root         (0) root         (0)     7644 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/hlt_mkab.py
--rw-rw-rw-   0 root         (0) root         (0)     1933 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/hlt_mkb_tap.py
--rw-rw-rw-   0 root         (0) root         (0)     1089 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/hlt_polis_mkab.py
--rw-rw-rw-   0 root         (0) root         (0)      607 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/models/hlt_reason_care.py
--rw-rw-rw-   0 root         (0) root         (0)     3473 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/models/hlt_representative_mkab.py
--rw-rw-rw-   0 root         (0) root         (0)     3724 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/hlt_smtap.py
--rw-rw-rw-   0 root         (0) root         (0)     6309 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/hlt_tap.py
--rw-rw-rw-   0 root         (0) root         (0)      579 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/models/hlt_type_call_doctor.py
--rw-rw-rw-   0 root         (0) root         (0)     1018 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/models/hlt_uchastok.py
--rw-rw-rw-   0 root         (0) root         (0)     1306 2023-02-06 03:36:56.000000 django-tmmis-0.3.6/tmmis/models/hlt_visit_history.py
--rw-rw-rw-   0 root         (0) root         (0)     1076 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/models/kla_address.py
--rw-rw-rw-   0 root         (0) root         (0)      675 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/models/kla_house.py
--rw-rw-rw-   0 root         (0) root         (0)     1094 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/models/kla_kladr.py
--rw-rw-rw-   0 root         (0) root         (0)      984 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/models/kla_street.py
--rw-rw-rw-   0 root         (0) root         (0)      721 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/lbr_complex_research_type.py
--rw-rw-rw-   0 root         (0) root         (0)      742 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/lbr_histological_block.py
--rw-rw-rw-   0 root         (0) root         (0)      524 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/lbr_lab_direction_type.py
--rw-rw-rw-   0 root         (0) root         (0)      652 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/lbr_lab_research_cause.py
--rw-rw-rw-   0 root         (0) root         (0)      651 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/lbr_lab_research_target.py
--rw-rw-rw-   0 root         (0) root         (0)      877 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/lbr_laboratory.py
--rw-rw-rw-   0 root         (0) root         (0)      626 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/lbr_laboratory_kind.py
--rw-rw-rw-   0 root         (0) root         (0)     4525 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/lbr_laboratory_research.py
--rw-rw-rw-   0 root         (0) root         (0)     1112 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/lbr_laboratory_research_in_pack.py
--rw-rw-rw-   0 root         (0) root         (0)      636 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/lbr_laboratory_research_pack.py
--rw-rw-rw-   0 root         (0) root         (0)      695 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/lbr_laboratory_research_type.py
--rw-rw-rw-   0 root         (0) root         (0)      715 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/lbr_laboratory_type.py
--rw-rw-rw-   0 root         (0) root         (0)      752 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/lbr_option.py
--rw-rw-rw-   0 root         (0) root         (0)      586 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/lbr_option_enum_values.py
--rw-rw-rw-   0 root         (0) root         (0)      591 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/lbr_option_value.py
--rw-rw-rw-   0 root         (0) root         (0)      592 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/lbr_option_value_type.py
--rw-rw-rw-   0 root         (0) root         (0)     3930 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/lbr_research.py
--rw-rw-rw-   0 root         (0) root         (0)      917 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/lbr_research_journal.py
--rw-rw-rw-   0 root         (0) root         (0)      472 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/lbr_research_param_value_type.py
--rw-rw-rw-   0 root         (0) root         (0)      780 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/lbr_research_param_values.py
--rw-rw-rw-   0 root         (0) root         (0)     1874 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/lbr_research_result.py
--rw-rw-rw-   0 root         (0) root         (0)      990 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/lbr_research_sample.py
--rw-rw-rw-   0 root         (0) root         (0)      636 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/lbr_research_service.py
--rw-rw-rw-   0 root         (0) root         (0)      411 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/lbr_research_state.py
--rw-rw-rw-   0 root         (0) root         (0)     1410 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/lbr_research_type.py
--rw-rw-rw-   0 root         (0) root         (0)      725 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/lbr_research_type_in_pack.py
--rw-rw-rw-   0 root         (0) root         (0)      838 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/lbr_research_type_kind.py
--rw-rw-rw-   0 root         (0) root         (0)      595 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/lbr_research_type_kind_doc_prvd.py
--rw-rw-rw-   0 root         (0) root         (0)     2027 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/lbr_research_type_param.py
--rw-rw-rw-   0 root         (0) root         (0)      764 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/lbr_research_type_param_in_pack.py
--rw-rw-rw-   0 root         (0) root         (0)      840 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/lbr_research_type_param_to_research_type.py
--rw-rw-rw-   0 root         (0) root         (0)      632 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/lbr_research_type_to_lpu.py
--rw-rw-rw-   0 root         (0) root         (0)      576 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/lbr_research_type_to_profile.py
--rw-rw-rw-   0 root         (0) root         (0)     1638 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/models/oms_department.py
--rw-rw-rw-   0 root         (0) root         (0)      523 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/models/oms_kl_age_group.py
--rw-rw-rw-   0 root         (0) root         (0)      443 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/models/oms_kl_dd_service.py
--rw-rw-rw-   0 root         (0) root         (0)      467 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/models/oms_kl_department_profile.py
--rw-rw-rw-   0 root         (0) root         (0)      458 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/models/oms_kl_department_type.py
--rw-rw-rw-   0 root         (0) root         (0)      831 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/oms_kl_diagnos_type.py
--rw-rw-rw-   0 root         (0) root         (0)      449 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/models/oms_kl_disease_type.py
--rw-rw-rw-   0 root         (0) root         (0)      449 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/models/oms_kl_health_group.py
--rw-rw-rw-   0 root         (0) root         (0)      449 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/models/oms_kl_med_care_type.py
--rw-rw-rw-   0 root         (0) root         (0)      747 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/oms_kl_met_issl.py
--rw-rw-rw-   0 root         (0) root         (0)      524 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/models/oms_kl_profit_type.py
--rw-rw-rw-   0 root         (0) root         (0)      552 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/models/oms_kl_reason_type.py
--rw-rw-rw-   0 root         (0) root         (0)      544 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/models/oms_kl_soc_status.py
--rw-rw-rw-   0 root         (0) root         (0)      799 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/models/oms_kl_stat_cure_result.py
--rw-rw-rw-   0 root         (0) root         (0)      593 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/models/oms_kl_tip_oms.py
--rw-rw-rw-   0 root         (0) root         (0)      446 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/models/oms_kl_visit_place.py
--rw-rw-rw-   0 root         (0) root         (0)      952 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/models/oms_kl_visit_result.py
--rw-rw-rw-   0 root         (0) root         (0)     4240 2023-02-06 03:36:56.000000 django-tmmis-0.3.6/tmmis/models/oms_lpu.py
--rw-rw-rw-   0 root         (0) root         (0)      592 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/models/oms_mkb.py
--rw-rw-rw-   0 root         (0) root         (0)      778 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/models/oms_okato.py
--rw-rw-rw-   0 root         (0) root         (0)      689 2023-02-06 03:36:56.000000 django-tmmis-0.3.6/tmmis/models/oms_okved.py
--rw-rw-rw-   0 root         (0) root         (0)     2351 2023-02-06 03:36:56.000000 django-tmmis-0.3.6/tmmis/models/oms_organisation.py
--rw-rw-rw-   0 root         (0) root         (0)      644 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/models/oms_prvd.py
--rw-rw-rw-   0 root         (0) root         (0)     1047 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/models/oms_prvs.py
--rw-rw-rw-   0 root         (0) root         (0)     2625 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/models/oms_service_medical.py
--rw-rw-rw-   0 root         (0) root         (0)     2337 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/models/oms_smo.py
--rw-rw-rw-   0 root         (0) root         (0)      798 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/models/oms_type_doc.py
--rw-rw-rw-   0 root         (0) root         (0)     1780 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/x_doc_elem_def.py
--rw-rw-rw-   0 root         (0) root         (0)      983 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/x_doc_type_def.py
--rw-rw-rw-   0 root         (0) root         (0)      707 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/models/x_user.py
--rw-rw-rw-   0 root         (0) root         (0)      286 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/router.py
--rw-rw-rw-   0 root         (0) root         (0)       60 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/tests.py
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 06:28:15.326889 django_tmmis-0.3.9/
+-rw-rw-rw-   0 root         (0) root         (0)       45 2023-01-27 09:33:43.000000 django_tmmis-0.3.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2068 2024-06-03 06:28:15.326889 django_tmmis-0.3.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1104 2023-02-21 15:15:18.000000 django_tmmis-0.3.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 06:28:15.326889 django_tmmis-0.3.9/django_tmmis.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2068 2024-06-03 06:28:15.000000 django_tmmis-0.3.9/django_tmmis.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3684 2024-06-03 06:28:15.000000 django_tmmis-0.3.9/django_tmmis.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-06-03 06:28:15.000000 django_tmmis-0.3.9/django_tmmis.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-06-03 06:28:15.000000 django_tmmis-0.3.9/django_tmmis.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-06-03 06:28:15.000000 django_tmmis-0.3.9/django_tmmis.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1764 2024-06-02 19:22:19.000000 django_tmmis-0.3.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-06-03 06:28:15.326889 django_tmmis-0.3.9/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 06:28:15.294888 django_tmmis-0.3.9/tmmis/
+-rw-rw-rw-   0 root         (0) root         (0)      138 2024-06-02 19:06:02.000000 django_tmmis-0.3.9/tmmis/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-01-27 09:33:43.000000 django_tmmis-0.3.9/tmmis/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)       85 2023-02-06 03:09:08.000000 django_tmmis-0.3.9/tmmis/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)     1168 2024-06-02 19:06:02.000000 django_tmmis-0.3.9/tmmis/handlers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 06:28:15.326889 django_tmmis-0.3.9/tmmis/models/
+-rw-rw-rw-   0 root         (0) root         (0)     4583 2024-06-03 06:27:16.000000 django_tmmis-0.3.9/tmmis/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      994 2023-02-06 04:01:43.000000 django_tmmis-0.3.9/tmmis/models/atf_file_attachment.py
+-rw-rw-rw-   0 root         (0) root         (0)     1817 2024-06-02 19:06:02.000000 django_tmmis-0.3.9/tmmis/models/atf_file_info.py
+-rw-rw-rw-   0 root         (0) root         (0)      801 2023-02-06 04:01:43.000000 django_tmmis-0.3.9/tmmis/models/atf_file_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      506 2024-06-02 19:06:02.000000 django_tmmis-0.3.9/tmmis/models/base_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1485 2023-02-06 03:09:08.000000 django_tmmis-0.3.9/tmmis/models/hlt_blank_template.py
+-rw-rw-rw-   0 root         (0) root         (0)     3734 2023-02-06 03:09:08.000000 django_tmmis-0.3.9/tmmis/models/hlt_call_doctor.py
+-rw-rw-rw-   0 root         (0) root         (0)      408 2023-02-06 03:09:08.000000 django_tmmis-0.3.9/tmmis/models/hlt_call_doctor_status.py
+-rw-rw-rw-   0 root         (0) root         (0)      598 2024-06-02 19:06:02.000000 django_tmmis-0.3.9/tmmis/models/hlt_citizen.py
+-rw-rw-rw-   0 root         (0) root         (0)     1682 2024-06-02 19:06:02.000000 django_tmmis-0.3.9/tmmis/models/hlt_disp_result_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     1354 2024-06-02 19:06:02.000000 django_tmmis-0.3.9/tmmis/models/hlt_disp_result_type_value.py
+-rw-rw-rw-   0 root         (0) root         (0)     1826 2024-06-02 19:06:02.000000 django_tmmis-0.3.9/tmmis/models/hlt_disp_result_value.py
+-rw-rw-rw-   0 root         (0) root         (0)     2078 2023-02-06 03:09:08.000000 django_tmmis-0.3.9/tmmis/models/hlt_doc_prvd.py
+-rw-rw-rw-   0 root         (0) root         (0)     1440 2023-02-06 03:09:08.000000 django_tmmis-0.3.9/tmmis/models/hlt_doctor_time_table.py
+-rw-rw-rw-   0 root         (0) root         (0)     2730 2023-02-06 03:09:08.000000 django_tmmis-0.3.9/tmmis/models/hlt_doctor_visit_table.py
+-rw-rw-rw-   0 root         (0) root         (0)     1525 2023-02-06 04:01:43.000000 django_tmmis-0.3.9/tmmis/models/hlt_lpu_doctor.py
+-rw-rw-rw-   0 root         (0) root         (0)     2667 2023-02-21 15:15:18.000000 django_tmmis-0.3.9/tmmis/models/hlt_med_record.py
+-rw-rw-rw-   0 root         (0) root         (0)     7644 2024-06-02 19:06:02.000000 django_tmmis-0.3.9/tmmis/models/hlt_mkab.py
+-rw-rw-rw-   0 root         (0) root         (0)     1933 2024-06-02 19:06:02.000000 django_tmmis-0.3.9/tmmis/models/hlt_mkb_tap.py
+-rw-rw-rw-   0 root         (0) root         (0)     1089 2023-02-07 13:45:07.000000 django_tmmis-0.3.9/tmmis/models/hlt_polis_mkab.py
+-rw-rw-rw-   0 root         (0) root         (0)      607 2023-02-06 03:09:08.000000 django_tmmis-0.3.9/tmmis/models/hlt_reason_care.py
+-rw-rw-rw-   0 root         (0) root         (0)     3473 2023-02-06 03:09:08.000000 django_tmmis-0.3.9/tmmis/models/hlt_representative_mkab.py
+-rw-rw-rw-   0 root         (0) root         (0)     3724 2023-02-07 13:45:07.000000 django_tmmis-0.3.9/tmmis/models/hlt_smtap.py
+-rw-rw-rw-   0 root         (0) root         (0)     6309 2023-02-21 15:15:18.000000 django_tmmis-0.3.9/tmmis/models/hlt_tap.py
+-rw-rw-rw-   0 root         (0) root         (0)      579 2023-02-06 03:09:08.000000 django_tmmis-0.3.9/tmmis/models/hlt_type_call_doctor.py
+-rw-rw-rw-   0 root         (0) root         (0)     1018 2023-02-06 03:09:08.000000 django_tmmis-0.3.9/tmmis/models/hlt_uchastok.py
+-rw-rw-rw-   0 root         (0) root         (0)     1306 2023-02-06 04:01:43.000000 django_tmmis-0.3.9/tmmis/models/hlt_visit_history.py
+-rw-rw-rw-   0 root         (0) root         (0)     1076 2023-02-06 03:09:08.000000 django_tmmis-0.3.9/tmmis/models/kla_address.py
+-rw-rw-rw-   0 root         (0) root         (0)      675 2023-02-06 03:09:08.000000 django_tmmis-0.3.9/tmmis/models/kla_house.py
+-rw-rw-rw-   0 root         (0) root         (0)     1094 2023-02-06 03:09:08.000000 django_tmmis-0.3.9/tmmis/models/kla_kladr.py
+-rw-rw-rw-   0 root         (0) root         (0)      984 2023-02-06 03:09:08.000000 django_tmmis-0.3.9/tmmis/models/kla_street.py
+-rw-rw-rw-   0 root         (0) root         (0)      721 2024-06-02 19:06:02.000000 django_tmmis-0.3.9/tmmis/models/lbr_complex_research_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      742 2024-06-02 19:06:02.000000 django_tmmis-0.3.9/tmmis/models/lbr_histological_block.py
+-rw-rw-rw-   0 root         (0) root         (0)      524 2024-06-02 19:06:02.000000 django_tmmis-0.3.9/tmmis/models/lbr_lab_direction_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      652 2024-06-02 19:06:02.000000 django_tmmis-0.3.9/tmmis/models/lbr_lab_research_cause.py
+-rw-rw-rw-   0 root         (0) root         (0)      651 2024-06-02 19:06:02.000000 django_tmmis-0.3.9/tmmis/models/lbr_lab_research_target.py
+-rw-rw-rw-   0 root         (0) root         (0)      877 2024-06-02 19:06:02.000000 django_tmmis-0.3.9/tmmis/models/lbr_laboratory.py
+-rw-rw-rw-   0 root         (0) root         (0)      626 2024-06-02 19:06:02.000000 django_tmmis-0.3.9/tmmis/models/lbr_laboratory_kind.py
+-rw-rw-rw-   0 root         (0) root         (0)     4525 2024-06-02 19:06:02.000000 django_tmmis-0.3.9/tmmis/models/lbr_laboratory_research.py
+-rw-rw-rw-   0 root         (0) root         (0)     1112 2024-06-02 19:06:02.000000 django_tmmis-0.3.9/tmmis/models/lbr_laboratory_research_in_pack.py
+-rw-rw-rw-   0 root         (0) root         (0)      636 2024-06-02 19:06:02.000000 django_tmmis-0.3.9/tmmis/models/lbr_laboratory_research_pack.py
+-rw-rw-rw-   0 root         (0) root         (0)      695 2024-06-02 19:06:02.000000 django_tmmis-0.3.9/tmmis/models/lbr_laboratory_research_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      715 2024-06-02 19:06:02.000000 django_tmmis-0.3.9/tmmis/models/lbr_laboratory_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      752 2024-06-02 19:06:02.000000 django_tmmis-0.3.9/tmmis/models/lbr_option.py
+-rw-rw-rw-   0 root         (0) root         (0)      586 2024-06-02 19:06:02.000000 django_tmmis-0.3.9/tmmis/models/lbr_option_enum_values.py
+-rw-rw-rw-   0 root         (0) root         (0)      591 2024-06-02 19:06:02.000000 django_tmmis-0.3.9/tmmis/models/lbr_option_value.py
+-rw-rw-rw-   0 root         (0) root         (0)      592 2024-06-02 19:06:02.000000 django_tmmis-0.3.9/tmmis/models/lbr_option_value_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     5351 2024-06-02 19:06:02.000000 django_tmmis-0.3.9/tmmis/models/lbr_research.py
+-rw-rw-rw-   0 root         (0) root         (0)      917 2024-06-02 19:06:02.000000 django_tmmis-0.3.9/tmmis/models/lbr_research_journal.py
+-rw-rw-rw-   0 root         (0) root         (0)      472 2024-06-02 19:06:02.000000 django_tmmis-0.3.9/tmmis/models/lbr_research_param_value_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      780 2024-06-02 19:06:02.000000 django_tmmis-0.3.9/tmmis/models/lbr_research_param_values.py
+-rw-rw-rw-   0 root         (0) root         (0)     1874 2024-06-02 19:06:02.000000 django_tmmis-0.3.9/tmmis/models/lbr_research_result.py
+-rw-rw-rw-   0 root         (0) root         (0)      990 2024-06-02 19:06:02.000000 django_tmmis-0.3.9/tmmis/models/lbr_research_sample.py
+-rw-rw-rw-   0 root         (0) root         (0)      636 2024-06-02 19:06:02.000000 django_tmmis-0.3.9/tmmis/models/lbr_research_service.py
+-rw-rw-rw-   0 root         (0) root         (0)      411 2024-06-02 19:06:02.000000 django_tmmis-0.3.9/tmmis/models/lbr_research_state.py
+-rw-rw-rw-   0 root         (0) root         (0)     1780 2024-06-02 19:06:02.000000 django_tmmis-0.3.9/tmmis/models/lbr_research_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      725 2024-06-02 19:06:02.000000 django_tmmis-0.3.9/tmmis/models/lbr_research_type_in_pack.py
+-rw-rw-rw-   0 root         (0) root         (0)      838 2024-06-02 19:06:02.000000 django_tmmis-0.3.9/tmmis/models/lbr_research_type_kind.py
+-rw-rw-rw-   0 root         (0) root         (0)      595 2024-06-02 19:06:02.000000 django_tmmis-0.3.9/tmmis/models/lbr_research_type_kind_doc_prvd.py
+-rw-rw-rw-   0 root         (0) root         (0)     2027 2024-06-02 19:06:02.000000 django_tmmis-0.3.9/tmmis/models/lbr_research_type_param.py
+-rw-rw-rw-   0 root         (0) root         (0)      764 2024-06-02 19:06:02.000000 django_tmmis-0.3.9/tmmis/models/lbr_research_type_param_in_pack.py
+-rw-rw-rw-   0 root         (0) root         (0)      840 2024-06-02 19:06:02.000000 django_tmmis-0.3.9/tmmis/models/lbr_research_type_param_to_research_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      632 2024-06-02 19:06:02.000000 django_tmmis-0.3.9/tmmis/models/lbr_research_type_to_lpu.py
+-rw-rw-rw-   0 root         (0) root         (0)      576 2024-06-02 19:06:02.000000 django_tmmis-0.3.9/tmmis/models/lbr_research_type_to_profile.py
+-rw-rw-rw-   0 root         (0) root         (0)     1638 2023-02-06 03:09:08.000000 django_tmmis-0.3.9/tmmis/models/oms_department.py
+-rw-rw-rw-   0 root         (0) root         (0)      523 2023-02-06 03:09:08.000000 django_tmmis-0.3.9/tmmis/models/oms_kl_age_group.py
+-rw-rw-rw-   0 root         (0) root         (0)      443 2023-02-06 03:09:08.000000 django_tmmis-0.3.9/tmmis/models/oms_kl_dd_service.py
+-rw-rw-rw-   0 root         (0) root         (0)      467 2023-02-06 03:09:08.000000 django_tmmis-0.3.9/tmmis/models/oms_kl_department_profile.py
+-rw-rw-rw-   0 root         (0) root         (0)      458 2023-02-06 03:09:08.000000 django_tmmis-0.3.9/tmmis/models/oms_kl_department_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      831 2023-02-07 18:55:59.000000 django_tmmis-0.3.9/tmmis/models/oms_kl_diagnos_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      449 2023-02-06 03:09:08.000000 django_tmmis-0.3.9/tmmis/models/oms_kl_disease_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      449 2023-02-06 03:09:08.000000 django_tmmis-0.3.9/tmmis/models/oms_kl_health_group.py
+-rw-rw-rw-   0 root         (0) root         (0)      449 2023-02-06 03:09:08.000000 django_tmmis-0.3.9/tmmis/models/oms_kl_med_care_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      747 2024-06-02 19:06:02.000000 django_tmmis-0.3.9/tmmis/models/oms_kl_met_issl.py
+-rw-rw-rw-   0 root         (0) root         (0)      434 2024-06-02 19:06:02.000000 django_tmmis-0.3.9/tmmis/models/oms_kl_nom_lpu.py
+-rw-rw-rw-   0 root         (0) root         (0)      446 2024-06-02 19:06:02.000000 django_tmmis-0.3.9/tmmis/models/oms_kl_nom_service.py
+-rw-rw-rw-   0 root         (0) root         (0)      880 2024-06-02 19:06:02.000000 django_tmmis-0.3.9/tmmis/models/oms_kl_nom_service_mkb_mse.py
+-rw-rw-rw-   0 root         (0) root         (0)      524 2023-02-06 03:09:08.000000 django_tmmis-0.3.9/tmmis/models/oms_kl_profit_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      552 2023-02-06 03:09:08.000000 django_tmmis-0.3.9/tmmis/models/oms_kl_reason_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      544 2023-02-06 03:09:08.000000 django_tmmis-0.3.9/tmmis/models/oms_kl_soc_status.py
+-rw-rw-rw-   0 root         (0) root         (0)      799 2023-02-06 03:09:08.000000 django_tmmis-0.3.9/tmmis/models/oms_kl_stat_cure_result.py
+-rw-rw-rw-   0 root         (0) root         (0)      593 2023-02-06 03:09:08.000000 django_tmmis-0.3.9/tmmis/models/oms_kl_tip_oms.py
+-rw-rw-rw-   0 root         (0) root         (0)      446 2023-02-06 03:09:08.000000 django_tmmis-0.3.9/tmmis/models/oms_kl_visit_place.py
+-rw-rw-rw-   0 root         (0) root         (0)      952 2023-02-06 03:09:08.000000 django_tmmis-0.3.9/tmmis/models/oms_kl_visit_result.py
+-rw-rw-rw-   0 root         (0) root         (0)     4240 2023-02-06 04:01:43.000000 django_tmmis-0.3.9/tmmis/models/oms_lpu.py
+-rw-rw-rw-   0 root         (0) root         (0)      592 2023-02-06 03:09:08.000000 django_tmmis-0.3.9/tmmis/models/oms_mkb.py
+-rw-rw-rw-   0 root         (0) root         (0)      778 2023-02-06 03:09:08.000000 django_tmmis-0.3.9/tmmis/models/oms_okato.py
+-rw-rw-rw-   0 root         (0) root         (0)      689 2023-02-06 04:01:43.000000 django_tmmis-0.3.9/tmmis/models/oms_okved.py
+-rw-rw-rw-   0 root         (0) root         (0)     2351 2023-02-06 04:01:43.000000 django_tmmis-0.3.9/tmmis/models/oms_organisation.py
+-rw-rw-rw-   0 root         (0) root         (0)      644 2023-02-06 03:09:08.000000 django_tmmis-0.3.9/tmmis/models/oms_prvd.py
+-rw-rw-rw-   0 root         (0) root         (0)     1047 2023-02-06 03:09:08.000000 django_tmmis-0.3.9/tmmis/models/oms_prvs.py
+-rw-rw-rw-   0 root         (0) root         (0)     2625 2023-02-06 03:09:08.000000 django_tmmis-0.3.9/tmmis/models/oms_service_medical.py
+-rw-rw-rw-   0 root         (0) root         (0)     2337 2023-02-06 03:09:08.000000 django_tmmis-0.3.9/tmmis/models/oms_smo.py
+-rw-rw-rw-   0 root         (0) root         (0)      798 2023-02-06 03:09:08.000000 django_tmmis-0.3.9/tmmis/models/oms_type_doc.py
+-rw-rw-rw-   0 root         (0) root         (0)     1780 2023-02-21 15:15:18.000000 django_tmmis-0.3.9/tmmis/models/x_doc_elem_def.py
+-rw-rw-rw-   0 root         (0) root         (0)      983 2023-02-21 15:15:18.000000 django_tmmis-0.3.9/tmmis/models/x_doc_type_def.py
+-rw-rw-rw-   0 root         (0) root         (0)      707 2023-02-06 03:09:08.000000 django_tmmis-0.3.9/tmmis/models/x_user.py
+-rw-rw-rw-   0 root         (0) root         (0)      286 2023-02-06 03:09:08.000000 django_tmmis-0.3.9/tmmis/router.py
+-rw-rw-rw-   0 root         (0) root         (0)       60 2023-01-27 09:33:43.000000 django_tmmis-0.3.9/tmmis/tests.py
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-01-27 09:33:43.000000 django_tmmis-0.3.9/tmmis/views.py
```

### Comparing `django-tmmis-0.3.6/PKG-INFO` & `django_tmmis-0.3.9/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 Metadata-Version: 2.1
 Name: django-tmmis
-Version: 0.3.6
+Version: 0.3.9
 Summary: A Django app provided ORM to TrustMed medical information system
-Home-page: UNKNOWN
-Author: Chmelyuk Vladislav
-Author-email: neimp@yandex.ru
-License: UNKNOWN
-Platform: UNKNOWN
+Author-email: Chmelyuk Vladislav <neimp@yandex.ru>
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -18,15 +14,17 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Requires-Dist: mssql-django
 
 ![Pypi version](https://img.shields.io/pypi/v/django-tmmis.svg)
 ![Python versions](https://img.shields.io/pypi/pyversions/django-tmmis)
 ![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)
 
 ### Настройка
 
@@ -62,9 +60,7 @@
 python config/manage.py inspectdb --database=tmmis {table_name} > tmmis/models/{table_name}.py
 ```
 
 Windows:
 ```shell script
 py .\config\manage.py inspectdb --database=tmmis {table_name} > .\tmmis\models\{table_name}.py
 ```
-
-
```

### Comparing `django-tmmis-0.3.6/README.md` & `django_tmmis-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/django_tmmis.egg-info/PKG-INFO` & `django_tmmis-0.3.9/django_tmmis.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 Metadata-Version: 2.1
 Name: django-tmmis
-Version: 0.3.6
+Version: 0.3.9
 Summary: A Django app provided ORM to TrustMed medical information system
-Home-page: UNKNOWN
-Author: Chmelyuk Vladislav
-Author-email: neimp@yandex.ru
-License: UNKNOWN
-Platform: UNKNOWN
+Author-email: Chmelyuk Vladislav <neimp@yandex.ru>
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -18,15 +14,17 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Requires-Dist: mssql-django
 
 ![Pypi version](https://img.shields.io/pypi/v/django-tmmis.svg)
 ![Python versions](https://img.shields.io/pypi/pyversions/django-tmmis)
 ![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)
 
 ### Настройка
 
@@ -62,9 +60,7 @@
 python config/manage.py inspectdb --database=tmmis {table_name} > tmmis/models/{table_name}.py
 ```
 
 Windows:
 ```shell script
 py .\config\manage.py inspectdb --database=tmmis {table_name} > .\tmmis\models\{table_name}.py
 ```
-
-
```

### Comparing `django-tmmis-0.3.6/django_tmmis.egg-info/SOURCES.txt` & `django_tmmis-0.3.9/django_tmmis.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 MANIFEST.in
 README.md
 pyproject.toml
-setup.cfg
-setup.py
 django_tmmis.egg-info/PKG-INFO
 django_tmmis.egg-info/SOURCES.txt
 django_tmmis.egg-info/dependency_links.txt
 django_tmmis.egg-info/requires.txt
 django_tmmis.egg-info/top_level.txt
 tmmis/__init__.py
 tmmis/admin.py
@@ -85,14 +83,17 @@
 tmmis/models/oms_kl_department_profile.py
 tmmis/models/oms_kl_department_type.py
 tmmis/models/oms_kl_diagnos_type.py
 tmmis/models/oms_kl_disease_type.py
 tmmis/models/oms_kl_health_group.py
 tmmis/models/oms_kl_med_care_type.py
 tmmis/models/oms_kl_met_issl.py
+tmmis/models/oms_kl_nom_lpu.py
+tmmis/models/oms_kl_nom_service.py
+tmmis/models/oms_kl_nom_service_mkb_mse.py
 tmmis/models/oms_kl_profit_type.py
 tmmis/models/oms_kl_reason_type.py
 tmmis/models/oms_kl_soc_status.py
 tmmis/models/oms_kl_stat_cure_result.py
 tmmis/models/oms_kl_tip_oms.py
 tmmis/models/oms_kl_visit_place.py
 tmmis/models/oms_kl_visit_result.py
```

### Comparing `django-tmmis-0.3.6/tmmis/handlers.py` & `django_tmmis-0.3.9/tmmis/handlers.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/__init__.py` & `django_tmmis-0.3.9/tmmis/models/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,14 +66,17 @@
 from .oms_kl_department_profile import OmsKlDepartmentProfile
 from .oms_kl_department_type import OmsKlDepartmentType
 from .oms_kl_diagnos_type import OmsKlDiagnosType
 from .oms_kl_disease_type import OmsKlDiseaseType
 from .oms_kl_health_group import OmsKlHealthGroup
 from .oms_kl_med_care_type import OmsKlMedCareType
 from .oms_kl_met_issl import OmsKlMetIssl
+from .oms_kl_nom_lpu import OmsKlNomLPU
+from .oms_kl_nom_service import OmsKlNomService
+from .oms_kl_nom_service_mkb_mse import OmsKlNomServiceMkbMse
 from .oms_kl_profit_type import OmsKlProfitType
 from .oms_kl_reason_type import OmsKlReasonType
 from .oms_kl_soc_status import OmsKlSocStatus
 from .oms_kl_stat_cure_result import OmsKlStatCureResult
 from .oms_kl_tip_oms import OmsKlTipOms
 from .oms_kl_visit_place import OmsKlVisitPlace
 from .oms_kl_visit_result import OmsKlVisitResult
```

### Comparing `django-tmmis-0.3.6/tmmis/models/atf_file_attachment.py` & `django_tmmis-0.3.9/tmmis/models/atf_file_attachment.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/atf_file_info.py` & `django_tmmis-0.3.9/tmmis/models/atf_file_info.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/atf_file_type.py` & `django_tmmis-0.3.9/tmmis/models/atf_file_type.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/hlt_blank_template.py` & `django_tmmis-0.3.9/tmmis/models/hlt_blank_template.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/hlt_call_doctor.py` & `django_tmmis-0.3.9/tmmis/models/hlt_call_doctor.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/hlt_citizen.py` & `django_tmmis-0.3.9/tmmis/models/hlt_citizen.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/hlt_disp_result_type.py` & `django_tmmis-0.3.9/tmmis/models/hlt_disp_result_type.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/hlt_disp_result_type_value.py` & `django_tmmis-0.3.9/tmmis/models/hlt_disp_result_type_value.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/hlt_disp_result_value.py` & `django_tmmis-0.3.9/tmmis/models/hlt_disp_result_value.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/hlt_doc_prvd.py` & `django_tmmis-0.3.9/tmmis/models/hlt_doc_prvd.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/hlt_doctor_time_table.py` & `django_tmmis-0.3.9/tmmis/models/hlt_doctor_time_table.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/hlt_doctor_visit_table.py` & `django_tmmis-0.3.9/tmmis/models/hlt_doctor_visit_table.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/hlt_lpu_doctor.py` & `django_tmmis-0.3.9/tmmis/models/hlt_lpu_doctor.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/hlt_med_record.py` & `django_tmmis-0.3.9/tmmis/models/hlt_med_record.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/hlt_mkab.py` & `django_tmmis-0.3.9/tmmis/models/hlt_mkab.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/hlt_mkb_tap.py` & `django_tmmis-0.3.9/tmmis/models/hlt_mkb_tap.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/hlt_polis_mkab.py` & `django_tmmis-0.3.9/tmmis/models/hlt_polis_mkab.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/hlt_reason_care.py` & `django_tmmis-0.3.9/tmmis/models/hlt_reason_care.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/hlt_representative_mkab.py` & `django_tmmis-0.3.9/tmmis/models/hlt_representative_mkab.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/hlt_smtap.py` & `django_tmmis-0.3.9/tmmis/models/hlt_smtap.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/hlt_tap.py` & `django_tmmis-0.3.9/tmmis/models/hlt_tap.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/hlt_type_call_doctor.py` & `django_tmmis-0.3.9/tmmis/models/hlt_type_call_doctor.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/hlt_uchastok.py` & `django_tmmis-0.3.9/tmmis/models/hlt_uchastok.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/hlt_visit_history.py` & `django_tmmis-0.3.9/tmmis/models/hlt_visit_history.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/kla_address.py` & `django_tmmis-0.3.9/tmmis/models/kla_address.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/kla_house.py` & `django_tmmis-0.3.9/tmmis/models/kla_house.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/kla_kladr.py` & `django_tmmis-0.3.9/tmmis/models/kla_kladr.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/kla_street.py` & `django_tmmis-0.3.9/tmmis/models/kla_street.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/lbr_complex_research_type.py` & `django_tmmis-0.3.9/tmmis/models/lbr_complex_research_type.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/lbr_histological_block.py` & `django_tmmis-0.3.9/tmmis/models/lbr_histological_block.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/lbr_lab_direction_type.py` & `django_tmmis-0.3.9/tmmis/models/lbr_lab_direction_type.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/lbr_lab_research_cause.py` & `django_tmmis-0.3.9/tmmis/models/lbr_lab_research_cause.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/lbr_lab_research_target.py` & `django_tmmis-0.3.9/tmmis/models/lbr_lab_research_target.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/lbr_laboratory.py` & `django_tmmis-0.3.9/tmmis/models/lbr_laboratory.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/lbr_laboratory_kind.py` & `django_tmmis-0.3.9/tmmis/models/lbr_laboratory_kind.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/lbr_laboratory_research.py` & `django_tmmis-0.3.9/tmmis/models/lbr_laboratory_research.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/lbr_laboratory_research_in_pack.py` & `django_tmmis-0.3.9/tmmis/models/lbr_laboratory_research_in_pack.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/lbr_laboratory_research_pack.py` & `django_tmmis-0.3.9/tmmis/models/lbr_laboratory_research_pack.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/lbr_laboratory_research_type.py` & `django_tmmis-0.3.9/tmmis/models/lbr_laboratory_research_type.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/lbr_laboratory_type.py` & `django_tmmis-0.3.9/tmmis/models/lbr_laboratory_type.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/lbr_option.py` & `django_tmmis-0.3.9/tmmis/models/lbr_option.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/lbr_option_enum_values.py` & `django_tmmis-0.3.9/tmmis/models/lbr_option_enum_values.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/lbr_option_value.py` & `django_tmmis-0.3.9/tmmis/models/lbr_option_value.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/lbr_option_value_type.py` & `django_tmmis-0.3.9/tmmis/models/lbr_option_value_type.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/lbr_research_journal.py` & `django_tmmis-0.3.9/tmmis/models/lbr_research_journal.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/lbr_research_param_values.py` & `django_tmmis-0.3.9/tmmis/models/lbr_research_param_values.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/lbr_research_result.py` & `django_tmmis-0.3.9/tmmis/models/lbr_research_result.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/lbr_research_sample.py` & `django_tmmis-0.3.9/tmmis/models/lbr_research_sample.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/lbr_research_service.py` & `django_tmmis-0.3.9/tmmis/models/lbr_research_service.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/lbr_research_type.py` & `django_tmmis-0.3.9/tmmis/models/lbr_research_type.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,22 +8,26 @@
 
     id = models.AutoField(db_column="ResearchTypeID", primary_key=True)
     uguid = models.CharField(db_column="UGUID", max_length=36, unique=True)
     code = models.CharField(db_column="Code", max_length=50)
     period = models.IntegerField(db_column="Period")
     report = models.TextField(db_column="Report")
     name = models.CharField(db_column="ResearchName", max_length=8000)
-    bio_m_id = models.IntegerField(db_column="rf_BioMID")
+    bio_mid = models.IntegerField(db_column="rf_BioMID")
     type = models.ForeignKey("LbrLaboratoryType", db_column="rf_LaboratoryTypeID", **FK_DEFAULT)
     research_type_kind = models.ForeignKey("LbrResearchTypeKind", db_column="rf_ResearchTypeKindID", **FK_DEFAULT)
     service_medical = models.ForeignKey("OmsServiceMedical", db_column="rf_ServiceMedicalID", **FK_DEFAULT)
     flags = models.IntegerField(db_column="Flags")
     date_begin = models.DateTimeField(db_column="DateBegin")
     date_end = models.DateTimeField(db_column="DateEnd")
-    nom_service_id = models.IntegerField(db_column="rf_kl_NomServiceID")
+    nom_service = models.ForeignKey("OmsKlNomService", db_column="rf_kl_NomServiceID", **FK_DEFAULT)
     is_complex = models.BooleanField(db_column="IsComplex")
     norm_duration = models.IntegerField(db_column="NormDuration")
-    met_issl_id = models.IntegerField(db_column="rf_kl_MetIsslID")
+    met_issl = models.ForeignKey("OmsKlMetIssl", db_column="rf_kl_MetIsslID", **FK_DEFAULT)
+    component = models.CharField(db_column="Component", max_length=500)
+    localization = models.CharField(db_column="Localization", max_length=500)
+    body_area = models.CharField(db_column="BodyArea", max_length=500)
+    rf_diagnostic_type_guid = models.CharField(db_column="rf_DiagnosticTypeGUID", max_length=36)
 
     class Meta:
         managed = False
         db_table = "lbr_ResearchType"
```

### Comparing `django-tmmis-0.3.6/tmmis/models/lbr_research_type_in_pack.py` & `django_tmmis-0.3.9/tmmis/models/lbr_research_type_in_pack.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/lbr_research_type_kind.py` & `django_tmmis-0.3.9/tmmis/models/lbr_research_type_kind.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/lbr_research_type_kind_doc_prvd.py` & `django_tmmis-0.3.9/tmmis/models/lbr_research_type_kind_doc_prvd.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/lbr_research_type_param.py` & `django_tmmis-0.3.9/tmmis/models/lbr_research_type_param.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/lbr_research_type_param_in_pack.py` & `django_tmmis-0.3.9/tmmis/models/lbr_research_type_param_in_pack.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/lbr_research_type_param_to_research_type.py` & `django_tmmis-0.3.9/tmmis/models/lbr_research_type_param_to_research_type.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/lbr_research_type_to_lpu.py` & `django_tmmis-0.3.9/tmmis/models/lbr_research_type_to_lpu.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/lbr_research_type_to_profile.py` & `django_tmmis-0.3.9/tmmis/models/lbr_research_type_to_profile.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/oms_department.py` & `django_tmmis-0.3.9/tmmis/models/oms_department.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/oms_kl_age_group.py` & `django_tmmis-0.3.9/tmmis/models/oms_kl_age_group.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/oms_kl_diagnos_type.py` & `django_tmmis-0.3.9/tmmis/models/oms_kl_diagnos_type.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/oms_kl_met_issl.py` & `django_tmmis-0.3.9/tmmis/models/oms_kl_met_issl.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 
 class OmsKlMetIssl(BaseModel):
     """
     Классификатор методов диагностического исследования (V029)
     """
 
-    id = models.AutoField(db_column='kl_MetIsslID', primary_key=True)
-    code = models.CharField(db_column='Code', max_length=10)
-    name = models.CharField(db_column='Name', max_length=200)
-    date_begin = models.DateTimeField(db_column='DateBegin')
-    date_end = models.DateTimeField(db_column='DateEnd')
-    description = models.TextField(db_column='Description')
-    flags = models.IntegerField(db_column='Flags')
-    guid = models.CharField(db_column='Guid', max_length=36)
+    id = models.AutoField(db_column="kl_MetIsslID", primary_key=True)
+    code = models.CharField(db_column="Code", max_length=10)
+    name = models.CharField(db_column="Name", max_length=200)
+    date_begin = models.DateTimeField(db_column="DateBegin")
+    date_end = models.DateTimeField(db_column="DateEnd")
+    description = models.TextField(db_column="Description")
+    flags = models.IntegerField(db_column="Flags")
+    guid = models.CharField(db_column="Guid", max_length=36)
 
     class Meta:
         managed = False
-        db_table = 'oms_kl_MetIssl'
+        db_table = "oms_kl_MetIssl"
```

### Comparing `django-tmmis-0.3.6/tmmis/models/oms_kl_profit_type.py` & `django_tmmis-0.3.9/tmmis/models/oms_kl_profit_type.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/oms_kl_reason_type.py` & `django_tmmis-0.3.9/tmmis/models/oms_kl_reason_type.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/oms_kl_soc_status.py` & `django_tmmis-0.3.9/tmmis/models/oms_kl_soc_status.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/oms_kl_stat_cure_result.py` & `django_tmmis-0.3.9/tmmis/models/oms_kl_stat_cure_result.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/oms_kl_tip_oms.py` & `django_tmmis-0.3.9/tmmis/models/oms_kl_tip_oms.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/oms_kl_visit_result.py` & `django_tmmis-0.3.9/tmmis/models/oms_kl_visit_result.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/oms_lpu.py` & `django_tmmis-0.3.9/tmmis/models/oms_lpu.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/oms_mkb.py` & `django_tmmis-0.3.9/tmmis/models/oms_mkb.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/oms_okato.py` & `django_tmmis-0.3.9/tmmis/models/oms_okato.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/oms_okved.py` & `django_tmmis-0.3.9/tmmis/models/oms_okved.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/oms_organisation.py` & `django_tmmis-0.3.9/tmmis/models/oms_organisation.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/oms_prvd.py` & `django_tmmis-0.3.9/tmmis/models/oms_prvd.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/oms_prvs.py` & `django_tmmis-0.3.9/tmmis/models/oms_prvs.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/oms_service_medical.py` & `django_tmmis-0.3.9/tmmis/models/oms_service_medical.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/oms_smo.py` & `django_tmmis-0.3.9/tmmis/models/oms_smo.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/oms_type_doc.py` & `django_tmmis-0.3.9/tmmis/models/oms_type_doc.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/x_doc_elem_def.py` & `django_tmmis-0.3.9/tmmis/models/x_doc_elem_def.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/x_doc_type_def.py` & `django_tmmis-0.3.9/tmmis/models/x_doc_type_def.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.6/tmmis/models/x_user.py` & `django_tmmis-0.3.9/tmmis/models/x_user.py`

 * *Files identical despite different names*

