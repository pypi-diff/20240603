# Comparing `tmp/cg-60.9.1.tar.gz` & `tmp/cg-60.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cg-60.9.1.tar", max compression
+gzip compressed data, was "cg-60.9.3.tar", max compression
```

## Comparing `cg-60.9.1.tar` & `cg-60.9.3.tar`

### file list

```diff
@@ -1,1357 +1,1357 @@
--rw-r--r--   0        0        0     2686 2024-05-30 12:47:24.899939 cg-60.9.1/README.md
--rw-r--r--   0        0        0       40 2024-05-30 12:47:24.903939 cg-60.9.1/cg/__init__.py
--rw-r--r--   0        0        0      315 2024-05-30 12:47:24.903939 cg-60.9.1/cg/apps/__init__.py
--rw-r--r--   0        0        0       27 2024-05-30 12:47:24.903939 cg-60.9.1/cg/apps/coverage/__init__.py
--rw-r--r--   0        0        0     2940 2024-05-30 12:47:24.903939 cg-60.9.1/cg/apps/coverage/api.py
--rw-r--r--   0        0        0       56 2024-05-30 12:47:24.903939 cg-60.9.1/cg/apps/crunchy/__init__.py
--rw-r--r--   0        0        0    12783 2024-05-30 12:47:24.903939 cg-60.9.1/cg/apps/crunchy/crunchy.py
--rw-r--r--   0        0        0     4502 2024-05-30 12:47:24.903939 cg-60.9.1/cg/apps/crunchy/files.py
--rw-r--r--   0        0        0      430 2024-05-30 12:47:24.903939 cg-60.9.1/cg/apps/crunchy/models.py
--rw-r--r--   0        0        0      910 2024-05-30 12:47:24.903939 cg-60.9.1/cg/apps/crunchy/sbatch.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.903939 cg-60.9.1/cg/apps/demultiplex/__init__.py
--rw-r--r--   0        0        0    11299 2024-05-30 12:47:24.903939 cg-60.9.1/cg/apps/demultiplex/demultiplex_api.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.907940 cg-60.9.1/cg/apps/demultiplex/sample_sheet/__init__.py
--rw-r--r--   0        0        0    11227 2024-05-30 12:47:24.907940 cg-60.9.1/cg/apps/demultiplex/sample_sheet/api.py
--rw-r--r--   0        0        0     2183 2024-05-30 12:47:24.907940 cg-60.9.1/cg/apps/demultiplex/sample_sheet/index.py
--rw-r--r--   0        0        0     7341 2024-05-30 12:47:24.907940 cg-60.9.1/cg/apps/demultiplex/sample_sheet/override_cycles_validator.py
--rw-r--r--   0        0        0     3188 2024-05-30 12:47:24.907940 cg-60.9.1/cg/apps/demultiplex/sample_sheet/read_sample_sheet.py
--rw-r--r--   0        0        0     7071 2024-05-30 12:47:24.907940 cg-60.9.1/cg/apps/demultiplex/sample_sheet/sample_models.py
--rw-r--r--   0        0        0     6076 2024-05-30 12:47:24.907940 cg-60.9.1/cg/apps/demultiplex/sample_sheet/sample_sheet_creator.py
--rw-r--r--   0        0        0     1372 2024-05-30 12:47:24.907940 cg-60.9.1/cg/apps/demultiplex/sample_sheet/sample_sheet_models.py
--rw-r--r--   0        0        0     8092 2024-05-30 12:47:24.907940 cg-60.9.1/cg/apps/demultiplex/sample_sheet/sample_sheet_validator.py
--rw-r--r--   0        0        0      824 2024-05-30 12:47:24.907940 cg-60.9.1/cg/apps/demultiplex/sample_sheet/validators.py
--rw-r--r--   0        0        0      677 2024-05-30 12:47:24.907940 cg-60.9.1/cg/apps/demultiplex/sbatch.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.907940 cg-60.9.1/cg/apps/downsample/__init__.py
--rw-r--r--   0        0        0     6340 2024-05-30 12:47:24.907940 cg-60.9.1/cg/apps/downsample/downsample.py
--rw-r--r--   0        0        0     2125 2024-05-30 12:47:24.907940 cg-60.9.1/cg/apps/downsample/utils.py
--rw-r--r--   0        0        0      298 2024-05-30 12:47:24.907940 cg-60.9.1/cg/apps/environ.py
--rw-r--r--   0        0        0     1741 2024-05-30 12:47:24.907940 cg-60.9.1/cg/apps/gens.py
--rw-r--r--   0        0        0     3419 2024-05-30 12:47:24.907940 cg-60.9.1/cg/apps/gt.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.907940 cg-60.9.1/cg/apps/hermes/__init__.py
--rw-r--r--   0        0        0     2249 2024-05-30 12:47:24.907940 cg-60.9.1/cg/apps/hermes/hermes_api.py
--rw-r--r--   0        0        0     1298 2024-05-30 12:47:24.907940 cg-60.9.1/cg/apps/hermes/models.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.907940 cg-60.9.1/cg/apps/housekeeper/__init__.py
--rw-r--r--   0        0        0    30395 2024-05-30 12:47:24.907940 cg-60.9.1/cg/apps/housekeeper/hk.py
--rw-r--r--   0        0        0      326 2024-05-30 12:47:24.907940 cg-60.9.1/cg/apps/housekeeper/models.py
--rw-r--r--   0        0        0       32 2024-05-30 12:47:24.907940 cg-60.9.1/cg/apps/invoice/__init__.py
--rw-r--r--   0        0        0     4804 2024-05-30 12:47:24.907940 cg-60.9.1/cg/apps/invoice/render.py
--rw-r--r--   0        0        0   113467 2024-05-30 12:47:24.907940 cg-60.9.1/cg/apps/invoice/templates/KI_pool_invoice.xlsx
--rw-r--r--   0        0        0    75562 2024-05-30 12:47:24.907940 cg-60.9.1/cg/apps/invoice/templates/KI_sample_invoice.xlsx
--rw-r--r--   0        0        0   113512 2024-05-30 12:47:24.907940 cg-60.9.1/cg/apps/invoice/templates/KTH_pool_invoice.xlsx
--rw-r--r--   0        0        0    75459 2024-05-30 12:47:24.907940 cg-60.9.1/cg/apps/invoice/templates/KTH_sample_invoice.xlsx
--rw-r--r--   0        0        0       25 2024-05-30 12:47:24.907940 cg-60.9.1/cg/apps/lims/__init__.py
--rw-r--r--   0        0        0    18873 2024-05-30 12:47:24.907940 cg-60.9.1/cg/apps/lims/api.py
--rw-r--r--   0        0        0     2652 2024-05-30 12:47:24.907940 cg-60.9.1/cg/apps/lims/batch.py
--rw-r--r--   0        0        0     8129 2024-05-30 12:47:24.907940 cg-60.9.1/cg/apps/lims/order.py
--rw-r--r--   0        0        0     3118 2024-05-30 12:47:24.907940 cg-60.9.1/cg/apps/lims/sample_sheet.py
--rw-r--r--   0        0        0     4866 2024-05-30 12:47:24.907940 cg-60.9.1/cg/apps/loqus.py
--rw-r--r--   0        0        0       35 2024-05-30 12:47:24.907940 cg-60.9.1/cg/apps/madeline/__init__.py
--rw-r--r--   0        0        0     3213 2024-05-30 12:47:24.907940 cg-60.9.1/cg/apps/madeline/api.py
--rw-r--r--   0        0        0       23 2024-05-30 12:47:24.907940 cg-60.9.1/cg/apps/mip/__init__.py
--rw-r--r--   0        0        0     3564 2024-05-30 12:47:24.907940 cg-60.9.1/cg/apps/mip/confighandler.py
--rw-r--r--   0        0        0     2207 2024-05-30 12:47:24.907940 cg-60.9.1/cg/apps/mutacc_auto.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.907940 cg-60.9.1/cg/apps/orderform/__init__.py
--rw-r--r--   0        0        0     9498 2024-05-30 12:47:24.907940 cg-60.9.1/cg/apps/orderform/excel_orderform_parser.py
--rw-r--r--   0        0        0     3051 2024-05-30 12:47:24.907940 cg-60.9.1/cg/apps/orderform/json_orderform_parser.py
--rw-r--r--   0        0        0     6419 2024-05-30 12:47:24.907940 cg-60.9.1/cg/apps/orderform/orderform_parser.py
--rw-r--r--   0        0        0      252 2024-05-30 12:47:24.907940 cg-60.9.1/cg/apps/orderform/utils.py
--rw-r--r--   0        0        0     2537 2024-05-30 12:47:24.907940 cg-60.9.1/cg/apps/osticket.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.907940 cg-60.9.1/cg/apps/scout/__init__.py
--rw-r--r--   0        0        0     3177 2024-05-30 12:47:24.907940 cg-60.9.1/cg/apps/scout/scout_export.py
--rw-r--r--   0        0        0    11108 2024-05-30 12:47:24.907940 cg-60.9.1/cg/apps/scout/scoutapi.py
--rw-r--r--   0        0        0      444 2024-05-30 12:47:24.907940 cg-60.9.1/cg/apps/scout/validators.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.907940 cg-60.9.1/cg/apps/slurm/__init__.py
--rw-r--r--   0        0        0     1277 2024-05-30 12:47:24.907940 cg-60.9.1/cg/apps/slurm/sbatch.py
--rw-r--r--   0        0        0     3559 2024-05-30 12:47:24.911939 cg-60.9.1/cg/apps/slurm/slurm_api.py
--rw-r--r--   0        0        0       32 2024-05-30 12:47:24.911939 cg-60.9.1/cg/apps/tb/__init__.py
--rw-r--r--   0        0        0     8025 2024-05-30 12:47:24.911939 cg-60.9.1/cg/apps/tb/api.py
--rw-r--r--   0        0        0      152 2024-05-30 12:47:24.911939 cg-60.9.1/cg/apps/tb/dto/create_job_request.py
--rw-r--r--   0        0        0      250 2024-05-30 12:47:24.911939 cg-60.9.1/cg/apps/tb/dto/summary_response.py
--rw-r--r--   0        0        0     1305 2024-05-30 12:47:24.911939 cg-60.9.1/cg/apps/tb/models.py
--rw-r--r--   0        0        0      305 2024-05-30 12:47:24.911939 cg-60.9.1/cg/apps/tb/validators.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/__init__.py
--rw-r--r--   0        0        0    11714 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/add.py
--rw-r--r--   0        0        0     4308 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/archive.py
--rw-r--r--   0        0        0    10118 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/backup.py
--rw-r--r--   0        0        0     3916 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/base.py
--rw-r--r--   0        0        0    10506 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/clean.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/compress/__init__.py
--rw-r--r--   0        0        0     2135 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/compress/base.py
--rw-r--r--   0        0        0     6706 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/compress/fastq.py
--rw-r--r--   0        0        0     8163 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/compress/helpers.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/delete/__init__.py
--rw-r--r--   0        0        0      564 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/delete/base.py
--rw-r--r--   0        0        0     4603 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/delete/case.py
--rw-r--r--   0        0        0     1896 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/delete/cases.py
--rw-r--r--   0        0        0     2470 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/delete/observations.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/deliver/__init__.py
--rw-r--r--   0        0        0     6068 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/deliver/base.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/demultiplex/__init__.py
--rw-r--r--   0        0        0      829 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/demultiplex/base.py
--rw-r--r--   0        0        0     4905 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/demultiplex/copy_novaseqx_demultiplex_data.py
--rw-r--r--   0        0        0     7717 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/demultiplex/demux.py
--rw-r--r--   0        0        0     1473 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/demultiplex/finish.py
--rw-r--r--   0        0        0     3119 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/demultiplex/sample_sheet.py
--rw-r--r--   0        0        0     3316 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/downsample.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/generate/__init__.py
--rw-r--r--   0        0        0      356 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/generate/base.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/generate/report/__init__.py
--rw-r--r--   0        0        0     4645 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/generate/report/base.py
--rw-r--r--   0        0        0      685 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/generate/report/options.py
--rw-r--r--   0        0        0     5615 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/generate/report/utils.py
--rw-r--r--   0        0        0     8327 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/get.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/set/__init__.py
--rw-r--r--   0        0        0     9856 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/set/base.py
--rw-r--r--   0        0        0     4384 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/set/case.py
--rw-r--r--   0        0        0     2595 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/set/cases.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/store/__init__.py
--rw-r--r--   0        0        0     1093 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/store/base.py
--rw-r--r--   0        0        0     6191 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/store/store.py
--rw-r--r--   0        0        0     1761 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/transfer.py
--rw-r--r--   0        0        0        1 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/upload/__init__.py
--rw-r--r--   0        0        0     5706 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/upload/base.py
--rw-r--r--   0        0        0     5548 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/upload/clinical_delivery.py
--rw-r--r--   0        0        0     1175 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/upload/coverage.py
--rw-r--r--   0        0        0     1465 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/upload/delivery_report.py
--rw-r--r--   0        0        0     3910 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/upload/fohm.py
--rw-r--r--   0        0        0     1463 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/upload/genotype.py
--rw-r--r--   0        0        0     1913 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/upload/gens.py
--rw-r--r--   0        0        0      584 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/upload/gisaid.py
--rw-r--r--   0        0        0     2615 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/upload/mutacc.py
--rw-r--r--   0        0        0       23 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/upload/nipt/__init__.py
--rw-r--r--   0        0        0     2985 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/upload/nipt/base.py
--rw-r--r--   0        0        0     2254 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/upload/nipt/ftp.py
--rw-r--r--   0        0        0     1607 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/upload/nipt/statina.py
--rw-r--r--   0        0        0      112 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/upload/observations/__init__.py
--rw-r--r--   0        0        0     2563 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/upload/observations/observations.py
--rw-r--r--   0        0        0     1968 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/upload/observations/utils.py
--rw-r--r--   0        0        0     9970 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/upload/scout.py
--rw-r--r--   0        0        0      650 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/upload/utils.py
--rw-r--r--   0        0        0     1667 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/upload/validate.py
--rw-r--r--   0        0        0      363 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/utils.py
--rw-r--r--   0        0        0      599 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/validate.py
--rw-r--r--   0        0        0       18 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/workflow/__init__.py
--rw-r--r--   0        0        0       22 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/workflow/balsamic/__init__.py
--rw-r--r--   0        0        0     8925 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/workflow/balsamic/base.py
--rw-r--r--   0        0        0     1980 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/workflow/balsamic/options.py
--rw-r--r--   0        0        0      881 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/workflow/balsamic/pon.py
--rw-r--r--   0        0        0     1162 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/workflow/balsamic/qc.py
--rw-r--r--   0        0        0     1177 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/workflow/balsamic/umi.py
--rw-r--r--   0        0        0     1342 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/workflow/base.py
--rw-r--r--   0        0        0    12264 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/workflow/commands.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/workflow/fastq/__init__.py
--rw-r--r--   0        0        0     1483 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/workflow/fastq/base.py
--rw-r--r--   0        0        0     1787 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/workflow/fastq/fastq_service.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/workflow/fluffy/__init__.py
--rw-r--r--   0        0        0     4081 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/workflow/fluffy/base.py
--rw-r--r--   0        0        0       22 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/workflow/jasen/__init__.py
--rw-r--r--   0        0        0      535 2024-05-30 12:47:24.911939 cg-60.9.1/cg/cli/workflow/jasen/base.py
--rw-r--r--   0        0        0       22 2024-05-30 12:47:24.915939 cg-60.9.1/cg/cli/workflow/microsalt/__init__.py
--rw-r--r--   0        0        0     7651 2024-05-30 12:47:24.915939 cg-60.9.1/cg/cli/workflow/microsalt/base.py
--rw-r--r--   0        0        0       22 2024-05-30 12:47:24.915939 cg-60.9.1/cg/cli/workflow/mip/__init__.py
--rw-r--r--   0        0        0     6605 2024-05-30 12:47:24.915939 cg-60.9.1/cg/cli/workflow/mip/base.py
--rw-r--r--   0        0        0     1125 2024-05-30 12:47:24.915939 cg-60.9.1/cg/cli/workflow/mip/options.py
--rw-r--r--   0        0        0       22 2024-05-30 12:47:24.915939 cg-60.9.1/cg/cli/workflow/mip_dna/__init__.py
--rw-r--r--   0        0        0     1013 2024-05-30 12:47:24.915939 cg-60.9.1/cg/cli/workflow/mip_dna/base.py
--rw-r--r--   0        0        0       22 2024-05-30 12:47:24.915939 cg-60.9.1/cg/cli/workflow/mip_rna/__init__.py
--rw-r--r--   0        0        0      916 2024-05-30 12:47:24.915939 cg-60.9.1/cg/cli/workflow/mip_rna/base.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.915939 cg-60.9.1/cg/cli/workflow/mutant/__init__.py
--rw-r--r--   0        0        0     3428 2024-05-30 12:47:24.915939 cg-60.9.1/cg/cli/workflow/mutant/base.py
--rw-r--r--   0        0        0     8980 2024-05-30 12:47:24.915939 cg-60.9.1/cg/cli/workflow/nf_analysis.py
--rw-r--r--   0        0        0       22 2024-05-30 12:47:24.915939 cg-60.9.1/cg/cli/workflow/raredisease/__init__.py
--rw-r--r--   0        0        0     2201 2024-05-30 12:47:24.915939 cg-60.9.1/cg/cli/workflow/raredisease/base.py
--rw-r--r--   0        0        0       22 2024-05-30 12:47:24.915939 cg-60.9.1/cg/cli/workflow/rnafusion/__init__.py
--rw-r--r--   0        0        0     1179 2024-05-30 12:47:24.915939 cg-60.9.1/cg/cli/workflow/rnafusion/base.py
--rw-r--r--   0        0        0       22 2024-05-30 12:47:24.915939 cg-60.9.1/cg/cli/workflow/taxprofiler/__init__.py
--rw-r--r--   0        0        0     1211 2024-05-30 12:47:24.915939 cg-60.9.1/cg/cli/workflow/taxprofiler/base.py
--rw-r--r--   0        0        0     1111 2024-05-30 12:47:24.915939 cg-60.9.1/cg/cli/workflow/tomte/base.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.915939 cg-60.9.1/cg/clients/__init__.py
--rw-r--r--   0        0        0     1363 2024-05-30 12:47:24.915939 cg-60.9.1/cg/clients/arnold/api.py
--rw-r--r--   0        0        0      160 2024-05-30 12:47:24.915939 cg-60.9.1/cg/clients/arnold/dto/create_case_request.py
--rw-r--r--   0        0        0      384 2024-05-30 12:47:24.915939 cg-60.9.1/cg/clients/arnold/exceptions.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.915939 cg-60.9.1/cg/clients/janus/__init__.py
--rw-r--r--   0        0        0     1246 2024-05-30 12:47:24.915939 cg-60.9.1/cg/clients/janus/api.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.915939 cg-60.9.1/cg/clients/janus/dto/__init__.py
--rw-r--r--   0        0        0      503 2024-05-30 12:47:24.915939 cg-60.9.1/cg/clients/janus/dto/create_qc_metrics_request.py
--rw-r--r--   0        0        0      420 2024-05-30 12:47:24.915939 cg-60.9.1/cg/clients/janus/exceptions.py
--rw-r--r--   0        0        0      937 2024-05-30 12:47:24.915939 cg-60.9.1/cg/constants/__init__.py
--rw-r--r--   0        0        0      253 2024-05-30 12:47:24.915939 cg-60.9.1/cg/constants/archiving.py
--rw-r--r--   0        0        0       35 2024-05-30 12:47:24.915939 cg-60.9.1/cg/constants/backup.py
--rw-r--r--   0        0        0      769 2024-05-30 12:47:24.915939 cg-60.9.1/cg/constants/bcl_convert_metrics.py
--rw-r--r--   0        0        0      469 2024-05-30 12:47:24.915939 cg-60.9.1/cg/constants/compression.py
--rw-r--r--   0        0        0     7086 2024-05-30 12:47:24.915939 cg-60.9.1/cg/constants/constants.py
--rw-r--r--   0        0        0     6055 2024-05-30 12:47:24.915939 cg-60.9.1/cg/constants/delivery.py
--rw-r--r--   0        0        0     7690 2024-05-30 12:47:24.915939 cg-60.9.1/cg/constants/demultiplexing.py
--rw-r--r--   0        0        0      172 2024-05-30 12:47:24.915939 cg-60.9.1/cg/constants/devices.py
--rw-r--r--   0        0        0     1422 2024-05-30 12:47:24.915939 cg-60.9.1/cg/constants/encryption.py
--rw-r--r--   0        0        0      372 2024-05-30 12:47:24.915939 cg-60.9.1/cg/constants/extraction.py
--rw-r--r--   0        0        0      134 2024-05-30 12:47:24.915939 cg-60.9.1/cg/constants/file_transfer_service.py
--rw-r--r--   0        0        0     2137 2024-05-30 12:47:24.915939 cg-60.9.1/cg/constants/gene_panel.py
--rw-r--r--   0        0        0     6747 2024-05-30 12:47:24.915939 cg-60.9.1/cg/constants/housekeeper_tags.py
--rw-r--r--   0        0        0       95 2024-05-30 12:47:24.915939 cg-60.9.1/cg/constants/invoice.py
--rw-r--r--   0        0        0     5815 2024-05-30 12:47:24.915939 cg-60.9.1/cg/constants/lims.py
--rw-r--r--   0        0        0      847 2024-05-30 12:47:24.915939 cg-60.9.1/cg/constants/metrics.py
--rw-r--r--   0        0        0      231 2024-05-30 12:47:24.915939 cg-60.9.1/cg/constants/nanopore_files.py
--rw-r--r--   0        0        0      650 2024-05-30 12:47:24.915939 cg-60.9.1/cg/constants/nextflow.py
--rw-r--r--   0        0        0     1595 2024-05-30 12:47:24.915939 cg-60.9.1/cg/constants/nf_analysis.py
--rw-r--r--   0        0        0       19 2024-05-30 12:47:24.915939 cg-60.9.1/cg/constants/nipt.py
--rw-r--r--   0        0        0     2178 2024-05-30 12:47:24.915939 cg-60.9.1/cg/constants/observations.py
--rw-r--r--   0        0        0     1216 2024-05-30 12:47:24.915939 cg-60.9.1/cg/constants/orderforms.py
--rw-r--r--   0        0        0       96 2024-05-30 12:47:24.915939 cg-60.9.1/cg/constants/paths.py
--rw-r--r--   0        0        0      266 2024-05-30 12:47:24.915939 cg-60.9.1/cg/constants/pdc.py
--rw-r--r--   0        0        0      160 2024-05-30 12:47:24.915939 cg-60.9.1/cg/constants/pedigree.py
--rw-r--r--   0        0        0     1044 2024-05-30 12:47:24.915939 cg-60.9.1/cg/constants/priority.py
--rw-r--r--   0        0        0       79 2024-05-30 12:47:24.915939 cg-60.9.1/cg/constants/process.py
--rw-r--r--   0        0        0     5885 2024-05-30 12:47:24.915939 cg-60.9.1/cg/constants/report.py
--rw-r--r--   0        0        0     1118 2024-05-30 12:47:24.915939 cg-60.9.1/cg/constants/sample_sources.py
--rw-r--r--   0        0        0     3111 2024-05-30 12:47:24.915939 cg-60.9.1/cg/constants/scout.py
--rw-r--r--   0        0        0     1669 2024-05-30 12:47:24.915939 cg-60.9.1/cg/constants/sequencing.py
--rw-r--r--   0        0        0      313 2024-05-30 12:47:24.915939 cg-60.9.1/cg/constants/slurm.py
--rw-r--r--   0        0        0      529 2024-05-30 12:47:24.915939 cg-60.9.1/cg/constants/subject.py
--rw-r--r--   0        0        0       55 2024-05-30 12:47:24.915939 cg-60.9.1/cg/constants/symbols.py
--rw-r--r--   0        0        0      435 2024-05-30 12:47:24.915939 cg-60.9.1/cg/constants/tb.py
--rw-r--r--   0        0        0      161 2024-05-30 12:47:24.915939 cg-60.9.1/cg/constants/time.py
--rw-r--r--   0        0        0     6639 2024-05-30 12:47:24.915939 cg-60.9.1/cg/exc.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.915939 cg-60.9.1/cg/io/__init__.py
--rw-r--r--   0        0        0     1037 2024-05-30 12:47:24.915939 cg-60.9.1/cg/io/api.py
--rw-r--r--   0        0        0      621 2024-05-30 12:47:24.915939 cg-60.9.1/cg/io/config.py
--rw-r--r--   0        0        0     2978 2024-05-30 12:47:24.915939 cg-60.9.1/cg/io/controller.py
--rw-r--r--   0        0        0     1763 2024-05-30 12:47:24.915939 cg-60.9.1/cg/io/csv.py
--rw-r--r--   0        0        0      210 2024-05-30 12:47:24.915939 cg-60.9.1/cg/io/gzip.py
--rw-r--r--   0        0        0      662 2024-05-30 12:47:24.915939 cg-60.9.1/cg/io/json.py
--rw-r--r--   0        0        0      525 2024-05-30 12:47:24.915939 cg-60.9.1/cg/io/png.py
--rw-r--r--   0        0        0     1094 2024-05-30 12:47:24.915939 cg-60.9.1/cg/io/txt.py
--rw-r--r--   0        0        0      552 2024-05-30 12:47:24.915939 cg-60.9.1/cg/io/validate_path.py
--rw-r--r--   0        0        0     1289 2024-05-30 12:47:24.915939 cg-60.9.1/cg/io/xml.py
--rw-r--r--   0        0        0     1153 2024-05-30 12:47:24.915939 cg-60.9.1/cg/io/yaml.py
--rw-r--r--   0        0        0      281 2024-05-30 12:47:24.915939 cg-60.9.1/cg/meta/__init__.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.915939 cg-60.9.1/cg/meta/archive/__init__.py
--rw-r--r--   0        0        0    16317 2024-05-30 12:47:24.915939 cg-60.9.1/cg/meta/archive/archive.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.915939 cg-60.9.1/cg/meta/archive/ddn/__init__.py
--rw-r--r--   0        0        0     1727 2024-05-30 12:47:24.915939 cg-60.9.1/cg/meta/archive/ddn/constants.py
--rw-r--r--   0        0        0    10852 2024-05-30 12:47:24.915939 cg-60.9.1/cg/meta/archive/ddn/ddn_data_flow_client.py
--rw-r--r--   0        0        0     3704 2024-05-30 12:47:24.915939 cg-60.9.1/cg/meta/archive/ddn/models.py
--rw-r--r--   0        0        0     1250 2024-05-30 12:47:24.915939 cg-60.9.1/cg/meta/archive/ddn/utils.py
--rw-r--r--   0        0        0     2024 2024-05-30 12:47:24.915939 cg-60.9.1/cg/meta/archive/models.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.915939 cg-60.9.1/cg/meta/backup/__init__.py
--rw-r--r--   0        0        0    17426 2024-05-30 12:47:24.919940 cg-60.9.1/cg/meta/backup/backup.py
--rw-r--r--   0        0        0     5397 2024-05-30 12:47:24.919940 cg-60.9.1/cg/meta/backup/pdc.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.919940 cg-60.9.1/cg/meta/clean/__init__.py
--rw-r--r--   0        0        0     3901 2024-05-30 12:47:24.919940 cg-60.9.1/cg/meta/clean/api.py
--rw-r--r--   0        0        0     7738 2024-05-30 12:47:24.919940 cg-60.9.1/cg/meta/clean/clean_flow_cells.py
--rw-r--r--   0        0        0     1841 2024-05-30 12:47:24.919940 cg-60.9.1/cg/meta/clean/clean_retrieved_spring_files.py
--rw-r--r--   0        0        0       34 2024-05-30 12:47:24.919940 cg-60.9.1/cg/meta/compress/__init__.py
--rw-r--r--   0        0        0    14557 2024-05-30 12:47:24.919940 cg-60.9.1/cg/meta/compress/compress.py
--rw-r--r--   0        0        0     4947 2024-05-30 12:47:24.919940 cg-60.9.1/cg/meta/compress/files.py
--rw-r--r--   0        0        0       77 2024-05-30 12:47:24.919940 cg-60.9.1/cg/meta/deliver/__init__.py
--rw-r--r--   0        0        0    14956 2024-05-30 12:47:24.919940 cg-60.9.1/cg/meta/deliver/deliver.py
--rw-r--r--   0        0        0     4565 2024-05-30 12:47:24.919940 cg-60.9.1/cg/meta/deliver/deliver_ticket.py
--rw-r--r--   0        0        0      904 2024-05-30 12:47:24.919940 cg-60.9.1/cg/meta/deliver/fastq_path_generator.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.919940 cg-60.9.1/cg/meta/delivery/__init__.py
--rw-r--r--   0        0        0     8518 2024-05-30 12:47:24.919940 cg-60.9.1/cg/meta/delivery/delivery.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.919940 cg-60.9.1/cg/meta/demultiplex/__init__.py
--rw-r--r--   0        0        0     2592 2024-05-30 12:47:24.919940 cg-60.9.1/cg/meta/demultiplex/combine_sequencing_metrics.py
--rw-r--r--   0        0        0     5817 2024-05-30 12:47:24.919940 cg-60.9.1/cg/meta/demultiplex/demux_post_processing.py
--rw-r--r--   0        0        0     8655 2024-05-30 12:47:24.919940 cg-60.9.1/cg/meta/demultiplex/housekeeper_storage_functions.py
--rw-r--r--   0        0        0     6198 2024-05-30 12:47:24.919940 cg-60.9.1/cg/meta/demultiplex/status_db_storage_functions.py
--rw-r--r--   0        0        0    10690 2024-05-30 12:47:24.919940 cg-60.9.1/cg/meta/demultiplex/utils.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.919940 cg-60.9.1/cg/meta/encryption/__init__.py
--rw-r--r--   0        0        0    20271 2024-05-30 12:47:24.919940 cg-60.9.1/cg/meta/encryption/encryption.py
--rw-r--r--   0        0        0      537 2024-05-30 12:47:24.919940 cg-60.9.1/cg/meta/encryption/sbatch.py
--rw-r--r--   0        0        0    10922 2024-05-30 12:47:24.919940 cg-60.9.1/cg/meta/invoice.py
--rw-r--r--   0        0        0     2360 2024-05-30 12:47:24.919940 cg-60.9.1/cg/meta/meta.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.919940 cg-60.9.1/cg/meta/observations/__init__.py
--rw-r--r--   0        0        0     7052 2024-05-30 12:47:24.919940 cg-60.9.1/cg/meta/observations/balsamic_observations_api.py
--rw-r--r--   0        0        0     6396 2024-05-30 12:47:24.919940 cg-60.9.1/cg/meta/observations/mip_dna_observations_api.py
--rw-r--r--   0        0        0     6932 2024-05-30 12:47:24.919940 cg-60.9.1/cg/meta/observations/observations_api.py
--rw-r--r--   0        0        0       27 2024-05-30 12:47:24.919940 cg-60.9.1/cg/meta/orders/__init__.py
--rw-r--r--   0        0        0     3736 2024-05-30 12:47:24.919940 cg-60.9.1/cg/meta/orders/api.py
--rw-r--r--   0        0        0      121 2024-05-30 12:47:24.919940 cg-60.9.1/cg/meta/orders/balsamic_qc_submitter.py
--rw-r--r--   0        0        0      107 2024-05-30 12:47:24.919940 cg-60.9.1/cg/meta/orders/balsamic_submitter.py
--rw-r--r--   0        0        0      122 2024-05-30 12:47:24.919940 cg-60.9.1/cg/meta/orders/balsamic_umi_submitter.py
--rw-r--r--   0        0        0    15145 2024-05-30 12:47:24.919940 cg-60.9.1/cg/meta/orders/case_submitter.py
--rw-r--r--   0        0        0     5991 2024-05-30 12:47:24.919940 cg-60.9.1/cg/meta/orders/fastq_submitter.py
--rw-r--r--   0        0        0      105 2024-05-30 12:47:24.919940 cg-60.9.1/cg/meta/orders/fluffy_submitter.py
--rw-r--r--   0        0        0     1254 2024-05-30 12:47:24.919940 cg-60.9.1/cg/meta/orders/lims.py
--rw-r--r--   0        0        0     5782 2024-05-30 12:47:24.919940 cg-60.9.1/cg/meta/orders/metagenome_submitter.py
--rw-r--r--   0        0        0     6337 2024-05-30 12:47:24.919940 cg-60.9.1/cg/meta/orders/microbial_submitter.py
--rw-r--r--   0        0        0      123 2024-05-30 12:47:24.919940 cg-60.9.1/cg/meta/orders/microsalt_submitter.py
--rw-r--r--   0        0        0      105 2024-05-30 12:47:24.919940 cg-60.9.1/cg/meta/orders/mip_dna_submitter.py
--rw-r--r--   0        0        0      105 2024-05-30 12:47:24.919940 cg-60.9.1/cg/meta/orders/mip_rna_submitter.py
--rw-r--r--   0        0        0     7622 2024-05-30 12:47:24.919940 cg-60.9.1/cg/meta/orders/pool_submitter.py
--rw-r--r--   0        0        0      102 2024-05-30 12:47:24.919940 cg-60.9.1/cg/meta/orders/rml_submitter.py
--rw-r--r--   0        0        0      718 2024-05-30 12:47:24.919940 cg-60.9.1/cg/meta/orders/rnafusion_submitter.py
--rw-r--r--   0        0        0     1268 2024-05-30 12:47:24.919940 cg-60.9.1/cg/meta/orders/sars_cov_2_submitter.py
--rw-r--r--   0        0        0     1754 2024-05-30 12:47:24.919940 cg-60.9.1/cg/meta/orders/submitter.py
--rw-r--r--   0        0        0     7880 2024-05-30 12:47:24.919940 cg-60.9.1/cg/meta/orders/ticket_handler.py
--rw-r--r--   0        0        0      104 2024-05-30 12:47:24.919940 cg-60.9.1/cg/meta/orders/tomte_submitter.py
--rw-r--r--   0        0        0     4105 2024-05-30 12:47:24.919940 cg-60.9.1/cg/meta/qc_metrics/collect_qc_metrics.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.919940 cg-60.9.1/cg/meta/report/__init__.py
--rw-r--r--   0        0        0     8168 2024-05-30 12:47:24.919940 cg-60.9.1/cg/meta/report/balsamic.py
--rw-r--r--   0        0        0      562 2024-05-30 12:47:24.919940 cg-60.9.1/cg/meta/report/balsamic_qc.py
--rw-r--r--   0        0        0      717 2024-05-30 12:47:24.919940 cg-60.9.1/cg/meta/report/balsamic_umi.py
--rw-r--r--   0        0        0     4171 2024-05-30 12:47:24.919940 cg-60.9.1/cg/meta/report/field_validators.py
--rw-r--r--   0        0        0     6620 2024-05-30 12:47:24.919940 cg-60.9.1/cg/meta/report/mip_dna.py
--rw-r--r--   0        0        0    18543 2024-05-30 12:47:24.919940 cg-60.9.1/cg/meta/report/report_api.py
--rw-r--r--   0        0        0     5625 2024-05-30 12:47:24.919940 cg-60.9.1/cg/meta/report/rnafusion.py
--rw-r--r--   0        0        0     2822 2024-05-30 12:47:24.919940 cg-60.9.1/cg/meta/report/taxprofiler.py
--rw-r--r--   0        0        0     1911 2024-05-30 12:47:24.919940 cg-60.9.1/cg/meta/report/templates/delivery-report.html
--rw-r--r--   0        0        0     4460 2024-05-30 12:47:24.919940 cg-60.9.1/cg/meta/report/templates/macros/data_analysis/data_analysis.html
--rw-r--r--   0        0        0     1049 2024-05-30 12:47:24.919940 cg-60.9.1/cg/meta/report/templates/macros/data_analysis/limitations.html
--rw-r--r--   0        0        0     3351 2024-05-30 12:47:24.919940 cg-60.9.1/cg/meta/report/templates/macros/data_analysis/qc_metrics/balsamic_qc_metrics.html
--rw-r--r--   0        0        0     1364 2024-05-30 12:47:24.919940 cg-60.9.1/cg/meta/report/templates/macros/data_analysis/qc_metrics/mip_dna_qc_metrics.html
--rw-r--r--   0        0        0      807 2024-05-30 12:47:24.919940 cg-60.9.1/cg/meta/report/templates/macros/data_analysis/qc_metrics/qc_metrics.html
--rw-r--r--   0        0        0     3284 2024-05-30 12:47:24.919940 cg-60.9.1/cg/meta/report/templates/macros/data_analysis/qc_metrics/rnafusion_qc_metrics.html
--rw-r--r--   0        0        0     3670 2024-05-30 12:47:24.919940 cg-60.9.1/cg/meta/report/templates/macros/data_analysis/qc_metrics/tomte_qc_metrics.html
--rw-r--r--   0        0        0     2332 2024-05-30 12:47:24.919940 cg-60.9.1/cg/meta/report/templates/macros/header.html
--rw-r--r--   0        0        0     2178 2024-05-30 12:47:24.923940 cg-60.9.1/cg/meta/report/templates/macros/order.html
--rw-r--r--   0        0        0     2243 2024-05-30 12:47:24.923940 cg-60.9.1/cg/meta/report/templates/macros/sample_prep.html
--rw-r--r--   0        0        0      472 2024-05-30 12:47:24.923940 cg-60.9.1/cg/meta/report/templates/macros/ticket_system.html
--rw-r--r--   0        0        0     1165 2024-05-30 12:47:24.923940 cg-60.9.1/cg/meta/report/templates/macros/uploaded_files/balsamic_uploaded_files.html
--rw-r--r--   0        0        0     1538 2024-05-30 12:47:24.923940 cg-60.9.1/cg/meta/report/templates/macros/uploaded_files/mip_dna_uploaded_files.html
--rw-r--r--   0        0        0      428 2024-05-30 12:47:24.923940 cg-60.9.1/cg/meta/report/templates/macros/uploaded_files/rnafusion_uploaded_files.html
--rw-r--r--   0        0        0     4266 2024-05-30 12:47:24.923940 cg-60.9.1/cg/meta/report/templates/macros/uploaded_files/uploaded_files.html
--rw-r--r--   0        0        0       80 2024-05-30 12:47:24.923940 cg-60.9.1/cg/meta/report/templates/partials/footer.html
--rw-r--r--   0        0        0      172 2024-05-30 12:47:24.923940 cg-60.9.1/cg/meta/report/templates/partials/signature.html
--rw-r--r--   0        0        0   232803 2024-05-30 12:47:24.923940 cg-60.9.1/cg/meta/report/templates/static/css/bootstrap.min.css
--rw-r--r--   0        0        0       33 2024-05-30 12:47:24.923940 cg-60.9.1/cg/meta/report/templates/static/css/custom.css
--rw-r--r--   0        0        0    30068 2024-05-30 12:47:24.923940 cg-60.9.1/cg/meta/report/templates/static/images/SWEDAC_logo.png
--rw-r--r--   0        0        0     3913 2024-05-30 12:47:24.923940 cg-60.9.1/cg/meta/report/tomte.py
--rw-r--r--   0        0        0       32 2024-05-30 12:47:24.923940 cg-60.9.1/cg/meta/rsync/__init__.py
--rw-r--r--   0        0        0    12291 2024-05-30 12:47:24.923940 cg-60.9.1/cg/meta/rsync/rsync_api.py
--rw-r--r--   0        0        0      387 2024-05-30 12:47:24.923940 cg-60.9.1/cg/meta/rsync/sbatch.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.923940 cg-60.9.1/cg/meta/tar/__init__.py
--rw-r--r--   0        0        0     1694 2024-05-30 12:47:24.923940 cg-60.9.1/cg/meta/tar/tar.py
--rw-r--r--   0        0        0       71 2024-05-30 12:47:24.923940 cg-60.9.1/cg/meta/transfer/__init__.py
--rw-r--r--   0        0        0    10242 2024-05-30 12:47:24.923940 cg-60.9.1/cg/meta/transfer/external_data.py
--rw-r--r--   0        0        0     5814 2024-05-30 12:47:24.923940 cg-60.9.1/cg/meta/transfer/lims.py
--rw-r--r--   0        0        0      503 2024-05-30 12:47:24.923940 cg-60.9.1/cg/meta/transfer/utils.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.923940 cg-60.9.1/cg/meta/upload/__init__.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.923940 cg-60.9.1/cg/meta/upload/balsamic/__init__.py
--rw-r--r--   0        0        0     3107 2024-05-30 12:47:24.923940 cg-60.9.1/cg/meta/upload/balsamic/balsamic.py
--rw-r--r--   0        0        0     2224 2024-05-30 12:47:24.923940 cg-60.9.1/cg/meta/upload/coverage.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.923940 cg-60.9.1/cg/meta/upload/fohm/__init__.py
--rw-r--r--   0        0        0    12102 2024-05-30 12:47:24.923940 cg-60.9.1/cg/meta/upload/fohm/fohm.py
--rw-r--r--   0        0        0       30 2024-05-30 12:47:24.923940 cg-60.9.1/cg/meta/upload/gisaid/__init__.py
--rw-r--r--   0        0        0      928 2024-05-30 12:47:24.923940 cg-60.9.1/cg/meta/upload/gisaid/constants.py
--rw-r--r--   0        0        0    13521 2024-05-30 12:47:24.923940 cg-60.9.1/cg/meta/upload/gisaid/gisaid.py
--rw-r--r--   0        0        0     3312 2024-05-30 12:47:24.923940 cg-60.9.1/cg/meta/upload/gisaid/models.py
--rw-r--r--   0        0        0     5310 2024-05-30 12:47:24.923940 cg-60.9.1/cg/meta/upload/gt.py
--rw-r--r--   0        0        0      898 2024-05-30 12:47:24.923940 cg-60.9.1/cg/meta/upload/microsalt/microsalt_upload_api.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.923940 cg-60.9.1/cg/meta/upload/mip/__init__.py
--rw-r--r--   0        0        0     2546 2024-05-30 12:47:24.923940 cg-60.9.1/cg/meta/upload/mip/mip_dna.py
--rw-r--r--   0        0        0     1400 2024-05-30 12:47:24.923940 cg-60.9.1/cg/meta/upload/mip/mip_rna.py
--rw-r--r--   0        0        0     7294 2024-05-30 12:47:24.923940 cg-60.9.1/cg/meta/upload/mutacc.py
--rw-r--r--   0        0        0     1853 2024-05-30 12:47:24.923940 cg-60.9.1/cg/meta/upload/nf_analysis.py
--rw-r--r--   0        0        0       32 2024-05-30 12:47:24.923940 cg-60.9.1/cg/meta/upload/nipt/__init__.py
--rw-r--r--   0        0        0      696 2024-05-30 12:47:24.923940 cg-60.9.1/cg/meta/upload/nipt/models.py
--rw-r--r--   0        0        0     8106 2024-05-30 12:47:24.923940 cg-60.9.1/cg/meta/upload/nipt/nipt.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.923940 cg-60.9.1/cg/meta/upload/scout/__init__.py
--rw-r--r--   0        0        0     4009 2024-05-30 12:47:24.923940 cg-60.9.1/cg/meta/upload/scout/balsamic_config_builder.py
--rw-r--r--   0        0        0     1491 2024-05-30 12:47:24.923940 cg-60.9.1/cg/meta/upload/scout/balsamic_umi_config_builder.py
--rw-r--r--   0        0        0     3322 2024-05-30 12:47:24.923940 cg-60.9.1/cg/meta/upload/scout/hk_tags.py
--rw-r--r--   0        0        0     9103 2024-05-30 12:47:24.923940 cg-60.9.1/cg/meta/upload/scout/mip_config_builder.py
--rw-r--r--   0        0        0     3495 2024-05-30 12:47:24.923940 cg-60.9.1/cg/meta/upload/scout/rnafusion_config_builder.py
--rw-r--r--   0        0        0     7231 2024-05-30 12:47:24.923940 cg-60.9.1/cg/meta/upload/scout/scout_config_builder.py
--rw-r--r--   0        0        0    23146 2024-05-30 12:47:24.923940 cg-60.9.1/cg/meta/upload/scout/uploadscoutapi.py
--rw-r--r--   0        0        0     3197 2024-05-30 12:47:24.923940 cg-60.9.1/cg/meta/upload/upload_api.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.923940 cg-60.9.1/cg/meta/workflow/__init__.py
--rw-r--r--   0        0        0    31742 2024-05-30 12:47:24.927940 cg-60.9.1/cg/meta/workflow/analysis.py
--rw-r--r--   0        0        0    28062 2024-05-30 12:47:24.927940 cg-60.9.1/cg/meta/workflow/balsamic.py
--rw-r--r--   0        0        0     2700 2024-05-30 12:47:24.927940 cg-60.9.1/cg/meta/workflow/balsamic_pon.py
--rw-r--r--   0        0        0      553 2024-05-30 12:47:24.927940 cg-60.9.1/cg/meta/workflow/balsamic_qc.py
--rw-r--r--   0        0        0      556 2024-05-30 12:47:24.927940 cg-60.9.1/cg/meta/workflow/balsamic_umi.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.927940 cg-60.9.1/cg/meta/workflow/downsample/__init__.py
--rw-r--r--   0        0        0     3991 2024-05-30 12:47:24.927940 cg-60.9.1/cg/meta/workflow/downsample/downsample.py
--rw-r--r--   0        0        0      711 2024-05-30 12:47:24.927940 cg-60.9.1/cg/meta/workflow/downsample/sbatch.py
--rw-r--r--   0        0        0     8913 2024-05-30 12:47:24.927940 cg-60.9.1/cg/meta/workflow/fastq.py
--rw-r--r--   0        0        0    10603 2024-05-30 12:47:24.927940 cg-60.9.1/cg/meta/workflow/fluffy.py
--rw-r--r--   0        0        0      521 2024-05-30 12:47:24.927940 cg-60.9.1/cg/meta/workflow/jasen.py
--rw-r--r--   0        0        0       70 2024-05-30 12:47:24.927940 cg-60.9.1/cg/meta/workflow/microsalt/__init__.py
--rw-r--r--   0        0        0      116 2024-05-30 12:47:24.927940 cg-60.9.1/cg/meta/workflow/microsalt/constants.py
--rw-r--r--   0        0        0      174 2024-05-30 12:47:24.927940 cg-60.9.1/cg/meta/workflow/microsalt/metrics_parser/__init__.py
--rw-r--r--   0        0        0      366 2024-05-30 12:47:24.927940 cg-60.9.1/cg/meta/workflow/microsalt/metrics_parser/metrics_parser.py
--rw-r--r--   0        0        0      903 2024-05-30 12:47:24.927940 cg-60.9.1/cg/meta/workflow/microsalt/metrics_parser/models.py
--rw-r--r--   0        0        0    13257 2024-05-30 12:47:24.927940 cg-60.9.1/cg/meta/workflow/microsalt/microsalt.py
--rw-r--r--   0        0        0      113 2024-05-30 12:47:24.927940 cg-60.9.1/cg/meta/workflow/microsalt/quality_controller/__init__.py
--rw-r--r--   0        0        0      712 2024-05-30 12:47:24.927940 cg-60.9.1/cg/meta/workflow/microsalt/quality_controller/models.py
--rw-r--r--   0        0        0     5697 2024-05-30 12:47:24.927940 cg-60.9.1/cg/meta/workflow/microsalt/quality_controller/quality_controller.py
--rw-r--r--   0        0        0     1217 2024-05-30 12:47:24.927940 cg-60.9.1/cg/meta/workflow/microsalt/quality_controller/report_generator.py
--rw-r--r--   0        0        0     2373 2024-05-30 12:47:24.927940 cg-60.9.1/cg/meta/workflow/microsalt/quality_controller/result_logger.py
--rw-r--r--   0        0        0     5641 2024-05-30 12:47:24.927940 cg-60.9.1/cg/meta/workflow/microsalt/quality_controller/utils.py
--rw-r--r--   0        0        0     1220 2024-05-30 12:47:24.927940 cg-60.9.1/cg/meta/workflow/microsalt/utils.py
--rw-r--r--   0        0        0    12611 2024-05-30 12:47:24.927940 cg-60.9.1/cg/meta/workflow/mip.py
--rw-r--r--   0        0        0     2948 2024-05-30 12:47:24.927940 cg-60.9.1/cg/meta/workflow/mip_dna.py
--rw-r--r--   0        0        0     2124 2024-05-30 12:47:24.927940 cg-60.9.1/cg/meta/workflow/mip_rna.py
--rw-r--r--   0        0        0    10957 2024-05-30 12:47:24.927940 cg-60.9.1/cg/meta/workflow/mutant.py
--rw-r--r--   0        0        0    37498 2024-05-30 12:47:24.927940 cg-60.9.1/cg/meta/workflow/nf_analysis.py
--rw-r--r--   0        0        0     6161 2024-05-30 12:47:24.927940 cg-60.9.1/cg/meta/workflow/nf_handlers.py
--rw-r--r--   0        0        0     6357 2024-05-30 12:47:24.927940 cg-60.9.1/cg/meta/workflow/prepare_fastq.py
--rw-r--r--   0        0        0     6028 2024-05-30 12:47:24.927940 cg-60.9.1/cg/meta/workflow/raredisease.py
--rw-r--r--   0        0        0     5419 2024-05-30 12:47:24.927940 cg-60.9.1/cg/meta/workflow/rnafusion.py
--rw-r--r--   0        0        0     4658 2024-05-30 12:47:24.927940 cg-60.9.1/cg/meta/workflow/taxprofiler.py
--rw-r--r--   0        0        0     3592 2024-05-30 12:47:24.927940 cg-60.9.1/cg/meta/workflow/tomte.py
--rw-r--r--   0        0        0      113 2024-05-30 12:47:24.927940 cg-60.9.1/cg/models/__init__.py
--rw-r--r--   0        0        0      457 2024-05-30 12:47:24.927940 cg-60.9.1/cg/models/analysis.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.927940 cg-60.9.1/cg/models/balsamic/__init__.py
--rw-r--r--   0        0        0      459 2024-05-30 12:47:24.927940 cg-60.9.1/cg/models/balsamic/analysis.py
--rw-r--r--   0        0        0     4550 2024-05-30 12:47:24.927940 cg-60.9.1/cg/models/balsamic/config.py
--rw-r--r--   0        0        0     1986 2024-05-30 12:47:24.927940 cg-60.9.1/cg/models/balsamic/metrics.py
--rw-r--r--   0        0        0    18130 2024-05-30 12:47:24.927940 cg-60.9.1/cg/models/cg_config.py
--rw-r--r--   0        0        0     4302 2024-05-30 12:47:24.927940 cg-60.9.1/cg/models/compression_data.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.927940 cg-60.9.1/cg/models/deliverables/__init__.py
--rw-r--r--   0        0        0     5219 2024-05-30 12:47:24.927940 cg-60.9.1/cg/models/deliverables/metric_deliverables.py
--rw-r--r--   0        0        0      243 2024-05-30 12:47:24.927940 cg-60.9.1/cg/models/delivery/delivery.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.927940 cg-60.9.1/cg/models/demultiplex/__init__.py
--rw-r--r--   0        0        0    13100 2024-05-30 12:47:24.927940 cg-60.9.1/cg/models/demultiplex/run_parameters.py
--rw-r--r--   0        0        0      539 2024-05-30 12:47:24.927940 cg-60.9.1/cg/models/demultiplex/sbatch.py
--rw-r--r--   0        0        0     7006 2024-05-30 12:47:24.927940 cg-60.9.1/cg/models/downsample/downsample_data.py
--rw-r--r--   0        0        0      255 2024-05-30 12:47:24.927940 cg-60.9.1/cg/models/email.py
--rw-r--r--   0        0        0     1046 2024-05-30 12:47:24.927940 cg-60.9.1/cg/models/fastq.py
--rw-r--r--   0        0        0     2157 2024-05-30 12:47:24.927940 cg-60.9.1/cg/models/file_data.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.927940 cg-60.9.1/cg/models/flow_cell/__init__.py
--rw-r--r--   0        0        0    13761 2024-05-30 12:47:24.927940 cg-60.9.1/cg/models/flow_cell/flow_cell.py
--rw-r--r--   0        0        0      317 2024-05-30 12:47:24.927940 cg-60.9.1/cg/models/flow_cell/utils.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.927940 cg-60.9.1/cg/models/invoice/__init__.py
--rw-r--r--   0        0        0     1254 2024-05-30 12:47:24.927940 cg-60.9.1/cg/models/invoice/invoice.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.927940 cg-60.9.1/cg/models/lims/__init__.py
--rw-r--r--   0        0        0     2019 2024-05-30 12:47:24.927940 cg-60.9.1/cg/models/lims/sample.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.927940 cg-60.9.1/cg/models/mip/__init__.py
--rw-r--r--   0        0        0      337 2024-05-30 12:47:24.927940 cg-60.9.1/cg/models/mip/mip_analysis.py
--rw-r--r--   0        0        0     1564 2024-05-30 12:47:24.927940 cg-60.9.1/cg/models/mip/mip_config.py
--rw-r--r--   0        0        0     4696 2024-05-30 12:47:24.927940 cg-60.9.1/cg/models/mip/mip_metrics_deliverables.py
--rw-r--r--   0        0        0     2550 2024-05-30 12:47:24.927940 cg-60.9.1/cg/models/mip/mip_sample_info.py
--rw-r--r--   0        0        0     2472 2024-05-30 12:47:24.927940 cg-60.9.1/cg/models/nf_analysis.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.927940 cg-60.9.1/cg/models/observations/__init__.py
--rw-r--r--   0        0        0      688 2024-05-30 12:47:24.927940 cg-60.9.1/cg/models/observations/input_files.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.927940 cg-60.9.1/cg/models/orders/__init__.py
--rw-r--r--   0        0        0     2691 2024-05-30 12:47:24.927940 cg-60.9.1/cg/models/orders/constants.py
--rw-r--r--   0        0        0     5604 2024-05-30 12:47:24.927940 cg-60.9.1/cg/models/orders/excel_sample.py
--rw-r--r--   0        0        0      898 2024-05-30 12:47:24.927940 cg-60.9.1/cg/models/orders/json_sample.py
--rw-r--r--   0        0        0     1449 2024-05-30 12:47:24.927940 cg-60.9.1/cg/models/orders/order.py
--rw-r--r--   0        0        0      811 2024-05-30 12:47:24.927940 cg-60.9.1/cg/models/orders/orderform_schema.py
--rw-r--r--   0        0        0     4212 2024-05-30 12:47:24.927940 cg-60.9.1/cg/models/orders/sample_base.py
--rw-r--r--   0        0        0     9786 2024-05-30 12:47:24.927940 cg-60.9.1/cg/models/orders/samples.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.931940 cg-60.9.1/cg/models/orders/validators/__init__.py
--rw-r--r--   0        0        0     2328 2024-05-30 12:47:24.931940 cg-60.9.1/cg/models/orders/validators/excel_sample_validators.py
--rw-r--r--   0        0        0      576 2024-05-30 12:47:24.931940 cg-60.9.1/cg/models/orders/validators/json_sample_validators.py
--rw-r--r--   0        0        0       71 2024-05-30 12:47:24.931940 cg-60.9.1/cg/models/orders/validators/sample_base_validators.py
--rw-r--r--   0        0        0      101 2024-05-30 12:47:24.931940 cg-60.9.1/cg/models/qc_metrics.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.931940 cg-60.9.1/cg/models/raredisease/__init__.py
--rw-r--r--   0        0        0     2034 2024-05-30 12:47:24.931940 cg-60.9.1/cg/models/raredisease/raredisease.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.931940 cg-60.9.1/cg/models/report/__init__.py
--rw-r--r--   0        0        0     8872 2024-05-30 12:47:24.931940 cg-60.9.1/cg/models/report/metadata.py
--rw-r--r--   0        0        0     6180 2024-05-30 12:47:24.931940 cg-60.9.1/cg/models/report/report.py
--rw-r--r--   0        0        0     5298 2024-05-30 12:47:24.931940 cg-60.9.1/cg/models/report/sample.py
--rw-r--r--   0        0        0     3267 2024-05-30 12:47:24.931940 cg-60.9.1/cg/models/report/validators.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.931940 cg-60.9.1/cg/models/rnafusion/__init__.py
--rw-r--r--   0        0        0     1865 2024-05-30 12:47:24.931940 cg-60.9.1/cg/models/rnafusion/rnafusion.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.931940 cg-60.9.1/cg/models/scout/__init__.py
--rw-r--r--   0        0        0     4783 2024-05-30 12:47:24.931940 cg-60.9.1/cg/models/scout/scout_load_config.py
--rw-r--r--   0        0        0      116 2024-05-30 12:47:24.931940 cg-60.9.1/cg/models/scout/validators.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.931940 cg-60.9.1/cg/models/slurm/__init__.py
--rw-r--r--   0        0        0      617 2024-05-30 12:47:24.931940 cg-60.9.1/cg/models/slurm/sbatch.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.931940 cg-60.9.1/cg/models/taxprofiler/__init__.py
--rw-r--r--   0        0        0     2597 2024-05-30 12:47:24.931940 cg-60.9.1/cg/models/taxprofiler/taxprofiler.py
--rw-r--r--   0        0        0     2588 2024-05-30 12:47:24.931940 cg-60.9.1/cg/models/tomte/tomte.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.931940 cg-60.9.1/cg/models/workflow/__init__.py
--rw-r--r--   0        0        0      685 2024-05-30 12:47:24.931940 cg-60.9.1/cg/models/workflow/mutant.py
--rw-r--r--   0        0        0       70 2024-05-30 12:47:24.931940 cg-60.9.1/cg/models/workflow/validators.py
--rw-r--r--   0        0        0      842 2024-05-30 12:47:24.931940 cg-60.9.1/cg/resources/__init__.py
--rw-r--r--   0        0        0     3493 2024-05-30 12:47:24.931940 cg-60.9.1/cg/resources/rnafusion_bundle_filenames.yaml
--rw-r--r--   0        0        0     2434 2024-05-30 12:47:24.931940 cg-60.9.1/cg/resources/taxprofiler_bundle_filenames.yaml
--rw-r--r--   0        0        0     4568 2024-05-30 12:47:24.931940 cg-60.9.1/cg/resources/tomte_bundle_filenames.yaml
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.931940 cg-60.9.1/cg/server/__init__.py
--rw-r--r--   0        0        0    21909 2024-05-30 12:47:24.931940 cg-60.9.1/cg/server/admin.py
--rw-r--r--   0        0        0    22743 2024-05-30 12:47:24.931940 cg-60.9.1/cg/server/api.py
--rw-r--r--   0        0        0     4969 2024-05-30 12:47:24.931940 cg-60.9.1/cg/server/app.py
--rw-r--r--   0        0        0       48 2024-05-30 12:47:24.931940 cg-60.9.1/cg/server/auto.py
--rw-r--r--   0        0        0     1184 2024-05-30 12:47:24.931940 cg-60.9.1/cg/server/config.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.931940 cg-60.9.1/cg/server/dto/__init__.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.931940 cg-60.9.1/cg/server/dto/delivery_message/__init__.py
--rw-r--r--   0        0        0      300 2024-05-30 12:47:24.931940 cg-60.9.1/cg/server/dto/delivery_message/delivery_message_request.py
--rw-r--r--   0        0        0      183 2024-05-30 12:47:24.931940 cg-60.9.1/cg/server/dto/delivery_message/delivery_message_response.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.931940 cg-60.9.1/cg/server/dto/orders/__init__.py
--rw-r--r--   0        0        0      165 2024-05-30 12:47:24.931940 cg-60.9.1/cg/server/dto/orders/order_delivery_update_request.py
--rw-r--r--   0        0        0       91 2024-05-30 12:47:24.931940 cg-60.9.1/cg/server/dto/orders/order_patch_request.py
--rw-r--r--   0        0        0      662 2024-05-30 12:47:24.931940 cg-60.9.1/cg/server/dto/orders/orders_request.py
--rw-r--r--   0        0        0      414 2024-05-30 12:47:24.931940 cg-60.9.1/cg/server/dto/orders/orders_response.py
--rw-r--r--   0        0        0     2599 2024-05-30 12:47:24.931940 cg-60.9.1/cg/server/ext.py
--rw-r--r--   0        0        0       29 2024-05-30 12:47:24.931940 cg-60.9.1/cg/server/invoices/__init__.py
--rw-r--r--   0        0        0     4793 2024-05-30 12:47:24.931940 cg-60.9.1/cg/server/invoices/templates/invoices/index.html
--rw-r--r--   0        0        0     8171 2024-05-30 12:47:24.931940 cg-60.9.1/cg/server/invoices/templates/invoices/invoice.html
--rw-r--r--   0        0        0     2838 2024-05-30 12:47:24.931940 cg-60.9.1/cg/server/invoices/templates/invoices/layout.html
--rw-r--r--   0        0        0     4956 2024-05-30 12:47:24.931940 cg-60.9.1/cg/server/invoices/templates/invoices/new.html
--rw-r--r--   0        0        0     7708 2024-05-30 12:47:24.931940 cg-60.9.1/cg/server/invoices/views.py
--rw-r--r--   0        0        0      354 2024-05-30 12:47:24.931940 cg-60.9.1/cg/server/templates/admin/index.html
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.931940 cg-60.9.1/cg/services/__init__.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.931940 cg-60.9.1/cg/services/analysis_service/__init__.py
--rw-r--r--   0        0        0      482 2024-05-30 12:47:24.931940 cg-60.9.1/cg/services/analysis_service/analysis_service.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.931940 cg-60.9.1/cg/services/delivery_message/__init__.py
--rw-r--r--   0        0        0     2531 2024-05-30 12:47:24.931940 cg-60.9.1/cg/services/delivery_message/delivery_message_service.py
--rw-r--r--   0        0        0      792 2024-05-30 12:47:24.931940 cg-60.9.1/cg/services/delivery_message/messages/__init__.py
--rw-r--r--   0        0        0     1366 2024-05-30 12:47:24.931940 cg-60.9.1/cg/services/delivery_message/messages/analysis_scout_message.py
--rw-r--r--   0        0        0      791 2024-05-30 12:47:24.931940 cg-60.9.1/cg/services/delivery_message/messages/covid_message.py
--rw-r--r--   0        0        0      189 2024-05-30 12:47:24.931940 cg-60.9.1/cg/services/delivery_message/messages/delivery_message.py
--rw-r--r--   0        0        0     1391 2024-05-30 12:47:24.931940 cg-60.9.1/cg/services/delivery_message/messages/fastq_analysis_scout_message.py
--rw-r--r--   0        0        0      535 2024-05-30 12:47:24.931940 cg-60.9.1/cg/services/delivery_message/messages/fastq_message.py
--rw-r--r--   0        0        0     1358 2024-05-30 12:47:24.931940 cg-60.9.1/cg/services/delivery_message/messages/fastq_scout_message.py
--rw-r--r--   0        0        0      604 2024-05-30 12:47:24.931940 cg-60.9.1/cg/services/delivery_message/messages/microsalt_mwr_message.py
--rw-r--r--   0        0        0      592 2024-05-30 12:47:24.931940 cg-60.9.1/cg/services/delivery_message/messages/microsalt_mwx_message.py
--rw-r--r--   0        0        0      903 2024-05-30 12:47:24.931940 cg-60.9.1/cg/services/delivery_message/messages/scout_message.py
--rw-r--r--   0        0        0      512 2024-05-30 12:47:24.931940 cg-60.9.1/cg/services/delivery_message/messages/statina_message.py
--rw-r--r--   0        0        0      779 2024-05-30 12:47:24.931940 cg-60.9.1/cg/services/delivery_message/messages/utils.py
--rw-r--r--   0        0        0     3300 2024-05-30 12:47:24.931940 cg-60.9.1/cg/services/delivery_message/utils.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.931940 cg-60.9.1/cg/services/fastq_concatenation_service/__init__.py
--rw-r--r--   0        0        0      101 2024-05-30 12:47:24.931940 cg-60.9.1/cg/services/fastq_concatenation_service/exceptions.py
--rw-r--r--   0        0        0     1110 2024-05-30 12:47:24.931940 cg-60.9.1/cg/services/fastq_concatenation_service/fastq_concatenation_service.py
--rw-r--r--   0        0        0     3000 2024-05-30 12:47:24.931940 cg-60.9.1/cg/services/fastq_concatenation_service/utils.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.931940 cg-60.9.1/cg/services/illumina_services/__init__.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.931940 cg-60.9.1/cg/services/illumina_services/illumina_metrics_service/__init__.py
--rw-r--r--   0        0        0    10867 2024-05-30 12:47:24.931940 cg-60.9.1/cg/services/illumina_services/illumina_metrics_service/bcl_convert_metrics_parser.py
--rw-r--r--   0        0        0     1121 2024-05-30 12:47:24.931940 cg-60.9.1/cg/services/illumina_services/illumina_metrics_service/illumina_demux_version_service.py
--rw-r--r--   0        0        0     9558 2024-05-30 12:47:24.931940 cg-60.9.1/cg/services/illumina_services/illumina_metrics_service/illumina_metrics_service.py
--rw-r--r--   0        0        0     2826 2024-05-30 12:47:24.931940 cg-60.9.1/cg/services/illumina_services/illumina_metrics_service/models.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.931940 cg-60.9.1/cg/services/illumina_services/illumina_post_processing_service/__init__.py
--rw-r--r--   0        0        0     5658 2024-05-30 12:47:24.931940 cg-60.9.1/cg/services/illumina_services/illumina_post_processing_service/illumina_post_processing_service.py
--rw-r--r--   0        0        0      473 2024-05-30 12:47:24.931940 cg-60.9.1/cg/services/illumina_services/illumina_post_processing_service/utils.py
--rw-r--r--   0        0        0     2892 2024-05-30 12:47:24.931940 cg-60.9.1/cg/services/illumina_services/illumina_post_processing_service/validation.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.931940 cg-60.9.1/cg/services/orders/__init__.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.931940 cg-60.9.1/cg/services/orders/order_service/__init__.py
--rw-r--r--   0        0        0     2717 2024-05-30 12:47:24.935940 cg-60.9.1/cg/services/orders/order_service/order_service.py
--rw-r--r--   0        0        0     1214 2024-05-30 12:47:24.935940 cg-60.9.1/cg/services/orders/order_service/utils.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.935940 cg-60.9.1/cg/services/orders/order_summary_service/__init__.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.935940 cg-60.9.1/cg/services/orders/order_summary_service/dto/__init__.py
--rw-r--r--   0        0        0      236 2024-05-30 12:47:24.935940 cg-60.9.1/cg/services/orders/order_summary_service/dto/case_summary.py
--rw-r--r--   0        0        0      319 2024-05-30 12:47:24.935940 cg-60.9.1/cg/services/orders/order_summary_service/dto/order_summary.py
--rw-r--r--   0        0        0     2029 2024-05-30 12:47:24.935940 cg-60.9.1/cg/services/orders/order_summary_service/order_summary_service.py
--rw-r--r--   0        0        0     2208 2024-05-30 12:47:24.935940 cg-60.9.1/cg/services/orders/order_summary_service/utils.py
--rw-r--r--   0        0        0     1175 2024-05-30 12:47:24.935940 cg-60.9.1/cg/services/parse_run_completion_status_service/parse_run_completion_status_service.py
--rw-r--r--   0        0        0       88 2024-05-30 12:47:24.935940 cg-60.9.1/cg/services/sequencing_qc_service/__init__.py
--rw-r--r--   0        0        0     1822 2024-05-30 12:47:24.935940 cg-60.9.1/cg/services/sequencing_qc_service/quality_checks/checks.py
--rw-r--r--   0        0        0     4987 2024-05-30 12:47:24.935940 cg-60.9.1/cg/services/sequencing_qc_service/quality_checks/utils.py
--rw-r--r--   0        0        0      930 2024-05-30 12:47:24.935940 cg-60.9.1/cg/services/sequencing_qc_service/sequencing_qc_service.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.935940 cg-60.9.1/cg/services/slurm_service/__init__.py
--rw-r--r--   0        0        0      703 2024-05-30 12:47:24.935940 cg-60.9.1/cg/services/slurm_service/slurm_cli_service.py
--rw-r--r--   0        0        0      242 2024-05-30 12:47:24.935940 cg-60.9.1/cg/services/slurm_service/slurm_service.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.935940 cg-60.9.1/cg/services/slurm_upload_service/__init__.py
--rw-r--r--   0        0        0      175 2024-05-30 12:47:24.935940 cg-60.9.1/cg/services/slurm_upload_service/slurm_upload_config.py
--rw-r--r--   0        0        0     2074 2024-05-30 12:47:24.935940 cg-60.9.1/cg/services/slurm_upload_service/slurm_upload_service.py
--rw-r--r--   0        0        0      203 2024-05-30 12:47:24.935940 cg-60.9.1/cg/services/slurm_upload_service/utils.py
--rw-r--r--   0        0        0     2904 2024-05-30 12:47:24.935940 cg-60.9.1/cg/services/validate_file_transfer_service/validate_file_transfer_service.py
--rw-r--r--   0        0        0     4161 2024-05-30 12:47:24.935940 cg-60.9.1/cg/services/validate_file_transfer_service/validate_pacbio_file_transfer_service.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.935940 cg-60.9.1/cg/store/__init__.py
--rw-r--r--   0        0        0     4650 2024-05-30 12:47:24.935940 cg-60.9.1/cg/store/base.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.935940 cg-60.9.1/cg/store/crud/__init__.py
--rw-r--r--   0        0        0    16830 2024-05-30 12:47:24.935940 cg-60.9.1/cg/store/crud/create.py
--rw-r--r--   0        0        0     2144 2024-05-30 12:47:24.935940 cg-60.9.1/cg/store/crud/delete.py
--rw-r--r--   0        0        0    60570 2024-05-30 12:47:24.935940 cg-60.9.1/cg/store/crud/read.py
--rw-r--r--   0        0        0     1121 2024-05-30 12:47:24.935940 cg-60.9.1/cg/store/crud/update.py
--rw-r--r--   0        0        0     1662 2024-05-30 12:47:24.935940 cg-60.9.1/cg/store/database.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.935940 cg-60.9.1/cg/store/filters/__init__.py
--rw-r--r--   0        0        0     5371 2024-05-30 12:47:24.935940 cg-60.9.1/cg/store/filters/status_analysis_filters.py
--rw-r--r--   0        0        0     1712 2024-05-30 12:47:24.935940 cg-60.9.1/cg/store/filters/status_application_filters.py
--rw-r--r--   0        0        0     1440 2024-05-30 12:47:24.935940 cg-60.9.1/cg/store/filters/status_application_limitations_filters.py
--rw-r--r--   0        0        0     2523 2024-05-30 12:47:24.935940 cg-60.9.1/cg/store/filters/status_application_version_filters.py
--rw-r--r--   0        0        0     1390 2024-05-30 12:47:24.935940 cg-60.9.1/cg/store/filters/status_bed_filters.py
--rw-r--r--   0        0        0     1317 2024-05-30 12:47:24.935940 cg-60.9.1/cg/store/filters/status_bed_version_filters.py
--rw-r--r--   0        0        0    10801 2024-05-30 12:47:24.935940 cg-60.9.1/cg/store/filters/status_case_filters.py
--rw-r--r--   0        0        0     3272 2024-05-30 12:47:24.935940 cg-60.9.1/cg/store/filters/status_case_sample_filters.py
--rw-r--r--   0        0        0      903 2024-05-30 12:47:24.935940 cg-60.9.1/cg/store/filters/status_collaboration_filters.py
--rw-r--r--   0        0        0     1412 2024-05-30 12:47:24.935940 cg-60.9.1/cg/store/filters/status_customer_filters.py
--rw-r--r--   0        0        0     1880 2024-05-30 12:47:24.935940 cg-60.9.1/cg/store/filters/status_flow_cell_filters.py
--rw-r--r--   0        0        0      896 2024-05-30 12:47:24.935940 cg-60.9.1/cg/store/filters/status_illumina_flow_cell_filters.py
--rw-r--r--   0        0        0     1255 2024-05-30 12:47:24.935940 cg-60.9.1/cg/store/filters/status_invoice_filters.py
--rw-r--r--   0        0        0     2792 2024-05-30 12:47:24.935940 cg-60.9.1/cg/store/filters/status_metrics_filters.py
--rw-r--r--   0        0        0     3225 2024-05-30 12:47:24.935940 cg-60.9.1/cg/store/filters/status_order_filters.py
--rw-r--r--   0        0        0      851 2024-05-30 12:47:24.935940 cg-60.9.1/cg/store/filters/status_organism_filters.py
--rw-r--r--   0        0        0      783 2024-05-30 12:47:24.935940 cg-60.9.1/cg/store/filters/status_panel_filters.py
--rw-r--r--   0        0        0     3923 2024-05-30 12:47:24.935940 cg-60.9.1/cg/store/filters/status_pool_filters.py
--rw-r--r--   0        0        0     8660 2024-05-30 12:47:24.935940 cg-60.9.1/cg/store/filters/status_sample_filters.py
--rw-r--r--   0        0        0      731 2024-05-30 12:47:24.935940 cg-60.9.1/cg/store/filters/status_user_filters.py
--rw-r--r--   0        0        0    41622 2024-05-30 12:47:24.935940 cg-60.9.1/cg/store/models.py
--rw-r--r--   0        0        0      706 2024-05-30 12:47:24.935940 cg-60.9.1/cg/store/store.py
--rw-r--r--   0        0        0       30 2024-05-30 12:47:24.935940 cg-60.9.1/cg/utils/__init__.py
--rw-r--r--   0        0        0      187 2024-05-30 12:47:24.935940 cg-60.9.1/cg/utils/calculations.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.935940 cg-60.9.1/cg/utils/checksum/__init__.py
--rw-r--r--   0        0        0     1992 2024-05-30 12:47:24.935940 cg-60.9.1/cg/utils/checksum/checksum.py
--rw-r--r--   0        0        0     1655 2024-05-30 12:47:24.935940 cg-60.9.1/cg/utils/click/EnumChoice.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.935940 cg-60.9.1/cg/utils/click/__init__.py
--rw-r--r--   0        0        0     4910 2024-05-30 12:47:24.935940 cg-60.9.1/cg/utils/commands.py
--rw-r--r--   0        0        0     1811 2024-05-30 12:47:24.935940 cg-60.9.1/cg/utils/date.py
--rw-r--r--   0        0        0      635 2024-05-30 12:47:24.935940 cg-60.9.1/cg/utils/dict.py
--rw-r--r--   0        0        0     2111 2024-05-30 12:47:24.935940 cg-60.9.1/cg/utils/dispatcher.py
--rw-r--r--   0        0        0     1251 2024-05-30 12:47:24.935940 cg-60.9.1/cg/utils/email.py
--rw-r--r--   0        0        0      134 2024-05-30 12:47:24.935940 cg-60.9.1/cg/utils/enums.py
--rw-r--r--   0        0        0     3727 2024-05-30 12:47:24.935940 cg-60.9.1/cg/utils/files.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.935940 cg-60.9.1/cg/utils/flask/__init__.py
--rw-r--r--   0        0        0     1052 2024-05-30 12:47:24.935940 cg-60.9.1/cg/utils/flask/enum.py
--rw-r--r--   0        0        0      233 2024-05-30 12:47:24.935940 cg-60.9.1/cg/utils/flow_cell.py
--rw-r--r--   0        0        0     1552 2024-05-30 12:47:24.935940 cg-60.9.1/cg/utils/time.py
--rw-r--r--   0        0        0     1410 2024-05-30 12:47:24.935940 cg-60.9.1/cg/utils/utils.py
--rw-r--r--   0        0        0     1697 2024-05-30 12:47:24.939940 cg-60.9.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.939940 cg-60.9.1/tests/__init__.py
--rw-r--r--   0        0        0     1158 2024-05-30 12:47:24.939940 cg-60.9.1/tests/apps/conftest.py
--rw-r--r--   0        0        0      231 2024-05-30 12:47:24.939940 cg-60.9.1/tests/apps/coverage/conftest.py
--rw-r--r--   0        0        0     6188 2024-05-30 12:47:24.939940 cg-60.9.1/tests/apps/coverage/test_coverage.py
--rw-r--r--   0        0        0     1693 2024-05-30 12:47:24.939940 cg-60.9.1/tests/apps/crunchy/conftest.py
--rw-r--r--   0        0        0     5438 2024-05-30 12:47:24.939940 cg-60.9.1/tests/apps/crunchy/test_compress_fastq.py
--rw-r--r--   0        0        0     2283 2024-05-30 12:47:24.939940 cg-60.9.1/tests/apps/crunchy/test_config.py
--rw-r--r--   0        0        0    14032 2024-05-30 12:47:24.939940 cg-60.9.1/tests/apps/crunchy/test_crunchy.py
--rw-r--r--   0        0        0     9109 2024-05-30 12:47:24.939940 cg-60.9.1/tests/apps/crunchy/test_spring_decompression.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.939940 cg-60.9.1/tests/apps/demultiplex/__init__.py
--rw-r--r--   0        0        0     4994 2024-05-30 12:47:24.939940 cg-60.9.1/tests/apps/demultiplex/conftest.py
--rw-r--r--   0        0        0     4010 2024-05-30 12:47:24.939940 cg-60.9.1/tests/apps/demultiplex/test_create_sample_sheet.py
--rw-r--r--   0        0        0     7986 2024-05-30 12:47:24.939940 cg-60.9.1/tests/apps/demultiplex/test_demultiplex_api.py
--rw-r--r--   0        0        0     4782 2024-05-30 12:47:24.939940 cg-60.9.1/tests/apps/demultiplex/test_index.py
--rw-r--r--   0        0        0     9468 2024-05-30 12:47:24.939940 cg-60.9.1/tests/apps/demultiplex/test_override_cycles_validator.py
--rw-r--r--   0        0        0     4042 2024-05-30 12:47:24.939940 cg-60.9.1/tests/apps/demultiplex/test_read_sample_sheet.py
--rw-r--r--   0        0        0    12389 2024-05-30 12:47:24.939940 cg-60.9.1/tests/apps/demultiplex/test_sample_models.py
--rw-r--r--   0        0        0      951 2024-05-30 12:47:24.939940 cg-60.9.1/tests/apps/demultiplex/test_sample_sheet_creator.py
--rw-r--r--   0        0        0     3175 2024-05-30 12:47:24.939940 cg-60.9.1/tests/apps/demultiplex/test_sample_sheet_models.py
--rw-r--r--   0        0        0    10932 2024-05-30 12:47:24.939940 cg-60.9.1/tests/apps/demultiplex/test_sample_sheet_validator.py
--rw-r--r--   0        0        0     4896 2024-05-30 12:47:24.939940 cg-60.9.1/tests/apps/demultiplex/test_translate_sample_sheet.py
--rw-r--r--   0        0        0     1450 2024-05-30 12:47:24.939940 cg-60.9.1/tests/apps/demultiplex/test_validate.py
--rw-r--r--   0        0        0     5105 2024-05-30 12:47:24.939940 cg-60.9.1/tests/apps/downsample/test_downsample.py
--rw-r--r--   0        0        0     1419 2024-05-30 12:47:24.939940 cg-60.9.1/tests/apps/downsample/test_downsample_utils.py
--rw-r--r--   0        0        0     1716 2024-05-30 12:47:24.939940 cg-60.9.1/tests/apps/gens/test_gens_api.py
--rw-r--r--   0        0        0     1950 2024-05-30 12:47:24.939940 cg-60.9.1/tests/apps/gt/conftest.py
--rw-r--r--   0        0        0     4276 2024-05-30 12:47:24.939940 cg-60.9.1/tests/apps/gt/test_gt_api.py
--rw-r--r--   0        0        0     1453 2024-05-30 12:47:24.939940 cg-60.9.1/tests/apps/hk/conftest.py
--rw-r--r--   0        0        0      684 2024-05-30 12:47:24.939940 cg-60.9.1/tests/apps/hk/test__getattr__.py
--rw-r--r--   0        0        0     1593 2024-05-30 12:47:24.939940 cg-60.9.1/tests/apps/hk/test_add_file.py
--rw-r--r--   0        0        0     3523 2024-05-30 12:47:24.939940 cg-60.9.1/tests/apps/hk/test_bundles.py
--rw-r--r--   0        0        0      871 2024-05-30 12:47:24.939940 cg-60.9.1/tests/apps/hk/test_core.py
--rw-r--r--   0        0        0    31172 2024-05-30 12:47:24.939940 cg-60.9.1/tests/apps/hk/test_file.py
--rw-r--r--   0        0        0     5080 2024-05-30 12:47:24.939940 cg-60.9.1/tests/apps/hk/test_version.py
--rw-r--r--   0        0        0     1840 2024-05-30 12:47:24.939940 cg-60.9.1/tests/apps/lims/conftest.py
--rw-r--r--   0        0        0     3197 2024-05-30 12:47:24.939940 cg-60.9.1/tests/apps/lims/test_api.py
--rw-r--r--   0        0        0     1451 2024-05-30 12:47:24.939940 cg-60.9.1/tests/apps/lims/test_sample_sheet.py
--rw-r--r--   0        0        0     9146 2024-05-30 12:47:24.939940 cg-60.9.1/tests/apps/loqus/test_loqusdb_api.py
--rw-r--r--   0        0        0     2439 2024-05-30 12:47:24.943940 cg-60.9.1/tests/apps/madeline/conftest.py
--rw-r--r--   0        0        0     4653 2024-05-30 12:47:24.943940 cg-60.9.1/tests/apps/madeline/test_madeline.py
--rw-r--r--   0        0        0     3328 2024-05-30 12:47:24.943940 cg-60.9.1/tests/apps/mip/conftest.py
--rw-r--r--   0        0        0     2487 2024-05-30 12:47:24.943940 cg-60.9.1/tests/apps/mip/test_config_mip.py
--rw-r--r--   0        0        0      883 2024-05-30 12:47:24.943940 cg-60.9.1/tests/apps/mutacc_auto/conftest.py
--rw-r--r--   0        0        0     2473 2024-05-30 12:47:24.943940 cg-60.9.1/tests/apps/mutacc_auto/test_mutacc_auto.py
--rw-r--r--   0        0        0    12196 2024-05-30 12:47:24.943940 cg-60.9.1/tests/apps/orderform/conftest.py
--rw-r--r--   0        0        0     9484 2024-05-30 12:47:24.943940 cg-60.9.1/tests/apps/orderform/test_excel_orderform_parser.py
--rw-r--r--   0        0        0     4351 2024-05-30 12:47:24.943940 cg-60.9.1/tests/apps/orderform/test_excel_sample_schema.py
--rw-r--r--   0        0        0     1032 2024-05-30 12:47:24.943940 cg-60.9.1/tests/apps/orderform/test_json_orderform_parser.py
--rw-r--r--   0        0        0     2474 2024-05-30 12:47:24.943940 cg-60.9.1/tests/apps/orderform/test_orderform_parser.py
--rw-r--r--   0        0        0    16002 2024-05-30 12:47:24.943940 cg-60.9.1/tests/apps/orderform/validators/test_excel_sample_validators.py
--rw-r--r--   0        0        0     3670 2024-05-30 12:47:24.943940 cg-60.9.1/tests/apps/scout/conftest.py
--rw-r--r--   0        0        0     2269 2024-05-30 12:47:24.943940 cg-60.9.1/tests/apps/scout/test_get_causative_variants.py
--rw-r--r--   0        0        0     1376 2024-05-30 12:47:24.943940 cg-60.9.1/tests/apps/scout/test_get_scout_cases.py
--rw-r--r--   0        0        0     1840 2024-05-30 12:47:24.943940 cg-60.9.1/tests/apps/scout/test_scout_load_config.py
--rw-r--r--   0        0        0     7047 2024-05-30 12:47:24.943940 cg-60.9.1/tests/apps/scout/test_scout_models.py
--rw-r--r--   0        0        0     1131 2024-05-30 12:47:24.943940 cg-60.9.1/tests/apps/slurm/conftest.py
--rw-r--r--   0        0        0     4412 2024-05-30 12:47:24.943940 cg-60.9.1/tests/apps/slurm/test_slurm_api.py
--rw-r--r--   0        0        0      831 2024-05-30 12:47:24.943940 cg-60.9.1/tests/apps/test_apps_environ.py
--rw-r--r--   0        0        0      957 2024-05-30 12:47:24.943940 cg-60.9.1/tests/apps/test_osticket.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.943940 cg-60.9.1/tests/cli/__init__.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.943940 cg-60.9.1/tests/cli/add/__init__.py
--rw-r--r--   0        0        0     1174 2024-05-30 12:47:24.943940 cg-60.9.1/tests/cli/add/test_cli_add.py
--rw-r--r--   0        0        0     2471 2024-05-30 12:47:24.943940 cg-60.9.1/tests/cli/add/test_cli_add_customer.py
--rw-r--r--   0        0        0     6841 2024-05-30 12:47:24.943940 cg-60.9.1/tests/cli/add/test_cli_add_family.py
--rw-r--r--   0        0        0     7588 2024-05-30 12:47:24.943940 cg-60.9.1/tests/cli/add/test_cli_add_relationship.py
--rw-r--r--   0        0        0     8382 2024-05-30 12:47:24.943940 cg-60.9.1/tests/cli/add/test_cli_add_sample.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.943940 cg-60.9.1/tests/cli/backup/__init__.py
--rw-r--r--   0        0        0      705 2024-05-30 12:47:24.943940 cg-60.9.1/tests/cli/backup/conftest.py
--rw-r--r--   0        0        0    11101 2024-05-30 12:47:24.943940 cg-60.9.1/tests/cli/backup/test_backup_command.py
--rw-r--r--   0        0        0     6819 2024-05-30 12:47:24.943940 cg-60.9.1/tests/cli/clean/conftest.py
--rw-r--r--   0        0        0     5564 2024-05-30 12:47:24.943940 cg-60.9.1/tests/cli/clean/test_balsamic_clean.py
--rw-r--r--   0        0        0     2564 2024-05-30 12:47:24.943940 cg-60.9.1/tests/cli/clean/test_clean_flow_cell.py
--rw-r--r--   0        0        0     1830 2024-05-30 12:47:24.943940 cg-60.9.1/tests/cli/clean/test_clean_hk_bundle_files.py
--rw-r--r--   0        0        0     2098 2024-05-30 12:47:24.943940 cg-60.9.1/tests/cli/clean/test_hk_bundle_files.py
--rw-r--r--   0        0        0     4610 2024-05-30 12:47:24.943940 cg-60.9.1/tests/cli/clean/test_hk_case_bundle_files.py
--rw-r--r--   0        0        0     3592 2024-05-30 12:47:24.943940 cg-60.9.1/tests/cli/clean/test_microbial_clean.py
--rw-r--r--   0        0        0     1888 2024-05-30 12:47:24.943940 cg-60.9.1/tests/cli/clean/test_rsync_past_run_dirs.py
--rw-r--r--   0        0        0     9707 2024-05-30 12:47:24.943940 cg-60.9.1/tests/cli/compress/conftest.py
--rw-r--r--   0        0        0     7709 2024-05-30 12:47:24.943940 cg-60.9.1/tests/cli/compress/test_cli_compress_fastq.py
--rw-r--r--   0        0        0     1416 2024-05-30 12:47:24.943940 cg-60.9.1/tests/cli/compress/test_cli_decompress_spring.py
--rw-r--r--   0        0        0     5205 2024-05-30 12:47:24.943940 cg-60.9.1/tests/cli/compress/test_compress_helpers.py
--rw-r--r--   0        0        0     1239 2024-05-30 12:47:24.943940 cg-60.9.1/tests/cli/compress/test_store_fastq.py
--rw-r--r--   0        0        0     7558 2024-05-30 12:47:24.943940 cg-60.9.1/tests/cli/conftest.py
--rw-r--r--   0        0        0    12747 2024-05-30 12:47:24.943940 cg-60.9.1/tests/cli/delete/test_cli_delete_case.py
--rw-r--r--   0        0        0     1873 2024-05-30 12:47:24.943940 cg-60.9.1/tests/cli/delete/test_cli_delete_cases.py
--rw-r--r--   0        0        0     3794 2024-05-30 12:47:24.943940 cg-60.9.1/tests/cli/deliver/conftest.py
--rw-r--r--   0        0        0     4428 2024-05-30 12:47:24.943940 cg-60.9.1/tests/cli/deliver/test_deliver_base.py
--rw-r--r--   0        0        0     1166 2024-05-30 12:47:24.943940 cg-60.9.1/tests/cli/deliver/test_rsync_base.py
--rw-r--r--   0        0        0     8569 2024-05-30 12:47:24.943940 cg-60.9.1/tests/cli/deliver/test_run_deliver_cmd.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.943940 cg-60.9.1/tests/cli/demultiplex/__init__.py
--rw-r--r--   0        0        0     5109 2024-05-30 12:47:24.943940 cg-60.9.1/tests/cli/demultiplex/test_create_sample_sheet.py
--rw-r--r--   0        0        0     5411 2024-05-30 12:47:24.943940 cg-60.9.1/tests/cli/demultiplex/test_demultiplex_flowcell.py
--rw-r--r--   0        0        0     1639 2024-05-30 12:47:24.943940 cg-60.9.1/tests/cli/demultiplex/test_finish_demux.py
--rw-r--r--   0        0        0     3015 2024-05-30 12:47:24.943940 cg-60.9.1/tests/cli/demultiplex/test_validate_sample_sheet.py
--rw-r--r--   0        0        0     4291 2024-05-30 12:47:24.943940 cg-60.9.1/tests/cli/demultiplex/test_verify_syncing.py
--rw-r--r--   0        0        0     1585 2024-05-30 12:47:24.943940 cg-60.9.1/tests/cli/downsample/test_cli_downsample.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.943940 cg-60.9.1/tests/cli/generate/__init__.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.943940 cg-60.9.1/tests/cli/generate/report/__init__.py
--rw-r--r--   0        0        0     1622 2024-05-30 12:47:24.943940 cg-60.9.1/tests/cli/generate/report/conftest.py
--rw-r--r--   0        0        0     2477 2024-05-30 12:47:24.943940 cg-60.9.1/tests/cli/generate/report/test_cli_delivery_report.py
--rw-r--r--   0        0        0     2760 2024-05-30 12:47:24.943940 cg-60.9.1/tests/cli/generate/report/test_utils.py
--rw-r--r--   0        0        0      563 2024-05-30 12:47:24.943940 cg-60.9.1/tests/cli/generate/test_cli_base.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.943940 cg-60.9.1/tests/cli/get/__init__.py
--rw-r--r--   0        0        0      863 2024-05-30 12:47:24.943940 cg-60.9.1/tests/cli/get/test_cli_get.py
--rw-r--r--   0        0        0     1526 2024-05-30 12:47:24.943940 cg-60.9.1/tests/cli/get/test_cli_get_analysis.py
--rw-r--r--   0        0        0     1242 2024-05-30 12:47:24.943940 cg-60.9.1/tests/cli/get/test_cli_get_case.py
--rw-r--r--   0        0        0     6208 2024-05-30 12:47:24.943940 cg-60.9.1/tests/cli/get/test_cli_get_flow_cell.py
--rw-r--r--   0        0        0     8835 2024-05-30 12:47:24.943940 cg-60.9.1/tests/cli/get/test_cli_get_sample.py
--rw-r--r--   0        0        0     1364 2024-05-30 12:47:24.943940 cg-60.9.1/tests/cli/set/conftest.py
--rw-r--r--   0        0        0     7311 2024-05-30 12:47:24.943940 cg-60.9.1/tests/cli/set/test_cli_set_case.py
--rw-r--r--   0        0        0     1460 2024-05-30 12:47:24.943940 cg-60.9.1/tests/cli/set/test_cli_set_cases.py
--rw-r--r--   0        0        0     2016 2024-05-30 12:47:24.943940 cg-60.9.1/tests/cli/set/test_cli_set_flowcell.py
--rw-r--r--   0        0        0     1685 2024-05-30 12:47:24.943940 cg-60.9.1/tests/cli/set/test_cli_set_list_keys.py
--rw-r--r--   0        0        0    12450 2024-05-30 12:47:24.943940 cg-60.9.1/tests/cli/set/test_cli_set_sample.py
--rw-r--r--   0        0        0     6124 2024-05-30 12:47:24.943940 cg-60.9.1/tests/cli/set/test_cli_set_samples.py
--rw-r--r--   0        0        0     7015 2024-05-30 12:47:24.947940 cg-60.9.1/tests/cli/store/test_store.py
--rw-r--r--   0        0        0     2332 2024-05-30 12:47:24.947940 cg-60.9.1/tests/cli/test_base.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.947940 cg-60.9.1/tests/cli/upload/__init__.py
--rw-r--r--   0        0        0    10102 2024-05-30 12:47:24.947940 cg-60.9.1/tests/cli/upload/conftest.py
--rw-r--r--   0        0        0     2295 2024-05-30 12:47:24.947940 cg-60.9.1/tests/cli/upload/test_cli_scout.py
--rw-r--r--   0        0        0     1789 2024-05-30 12:47:24.947940 cg-60.9.1/tests/cli/upload/test_cli_upload.py
--rw-r--r--   0        0        0      971 2024-05-30 12:47:24.947940 cg-60.9.1/tests/cli/upload/test_cli_upload_auto.py
--rw-r--r--   0        0        0     1669 2024-05-30 12:47:24.947940 cg-60.9.1/tests/cli/upload/test_cli_upload_delivery_report.py
--rw-r--r--   0        0        0      895 2024-05-30 12:47:24.947940 cg-60.9.1/tests/cli/upload/test_cli_upload_fastq.py
--rw-r--r--   0        0        0     1199 2024-05-30 12:47:24.947940 cg-60.9.1/tests/cli/upload/test_cli_upload_genotype.py
--rw-r--r--   0        0        0      694 2024-05-30 12:47:24.947940 cg-60.9.1/tests/cli/upload/test_cli_upload_gens.py
--rw-r--r--   0        0        0     9965 2024-05-30 12:47:24.947940 cg-60.9.1/tests/cli/upload/test_cli_upload_nipt.py
--rw-r--r--   0        0        0     4684 2024-05-30 12:47:24.947940 cg-60.9.1/tests/cli/upload/test_cli_upload_nipt_ftp.py
--rw-r--r--   0        0        0     1839 2024-05-30 12:47:24.947940 cg-60.9.1/tests/cli/upload/test_cli_upload_nipt_statina.py
--rw-r--r--   0        0        0     4193 2024-05-30 12:47:24.947940 cg-60.9.1/tests/cli/upload/test_cli_upload_observations.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.947940 cg-60.9.1/tests/cli/workflow/__init__.py
--rw-r--r--   0        0        0    31369 2024-05-30 12:47:24.947940 cg-60.9.1/tests/cli/workflow/balsamic/conftest.py
--rw-r--r--   0        0        0    13938 2024-05-30 12:47:24.947940 cg-60.9.1/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py
--rw-r--r--   0        0        0     7950 2024-05-30 12:47:24.947940 cg-60.9.1/tests/cli/workflow/balsamic/test_compound_commands.py
--rw-r--r--   0        0        0     2336 2024-05-30 12:47:24.947940 cg-60.9.1/tests/cli/workflow/balsamic/test_link.py
--rw-r--r--   0        0        0     3554 2024-05-30 12:47:24.947940 cg-60.9.1/tests/cli/workflow/balsamic/test_report_deliver.py
--rw-r--r--   0        0        0     6209 2024-05-30 12:47:24.947940 cg-60.9.1/tests/cli/workflow/balsamic/test_run.py
--rw-r--r--   0        0        0     7014 2024-05-30 12:47:24.947940 cg-60.9.1/tests/cli/workflow/balsamic/test_store_housekeeper.py
--rw-r--r--   0        0        0     8171 2024-05-30 12:47:24.947940 cg-60.9.1/tests/cli/workflow/conftest.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.947940 cg-60.9.1/tests/cli/workflow/fastq/__init__.py
--rw-r--r--   0        0        0     2332 2024-05-30 12:47:24.947940 cg-60.9.1/tests/cli/workflow/fastq/test_fastq_base.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.947940 cg-60.9.1/tests/cli/workflow/fluffy/__init__.py
--rw-r--r--   0        0        0     5237 2024-05-30 12:47:24.947940 cg-60.9.1/tests/cli/workflow/fluffy/conftest.py
--rw-r--r--   0        0        0     5687 2024-05-30 12:47:24.947940 cg-60.9.1/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py
--rw-r--r--   0        0        0     3302 2024-05-30 12:47:24.947940 cg-60.9.1/tests/cli/workflow/fluffy/test_cli_link.py
--rw-r--r--   0        0        0     1896 2024-05-30 12:47:24.947940 cg-60.9.1/tests/cli/workflow/fluffy/test_cli_run.py
--rw-r--r--   0        0        0     2968 2024-05-30 12:47:24.947940 cg-60.9.1/tests/cli/workflow/fluffy/test_cli_start.py
--rw-r--r--   0        0        0     7815 2024-05-30 12:47:24.947940 cg-60.9.1/tests/cli/workflow/fluffy/test_cli_store.py
--rw-r--r--   0        0        0     2775 2024-05-30 12:47:24.947940 cg-60.9.1/tests/cli/workflow/microsalt/conftest.py
--rw-r--r--   0        0        0     7059 2024-05-30 12:47:24.947940 cg-60.9.1/tests/cli/workflow/microsalt/test_microsalt_case_config.py
--rw-r--r--   0        0        0     1007 2024-05-30 12:47:24.947940 cg-60.9.1/tests/cli/workflow/microsalt/test_microsalt_run.py
--rw-r--r--   0        0        0     6544 2024-05-30 12:47:24.947940 cg-60.9.1/tests/cli/workflow/mip/conftest.py
--rw-r--r--   0        0        0     7011 2024-05-30 12:47:24.947940 cg-60.9.1/tests/cli/workflow/mip/test_cli_mip_base.py
--rw-r--r--   0        0        0     1542 2024-05-30 12:47:24.947940 cg-60.9.1/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py
--rw-r--r--   0        0        0      431 2024-05-30 12:47:24.947940 cg-60.9.1/tests/cli/workflow/mip/test_cli_mip_dna_link.py
--rw-r--r--   0        0        0     2108 2024-05-30 12:47:24.947940 cg-60.9.1/tests/cli/workflow/mip/test_cli_mip_dna_manged_variants.py
--rw-r--r--   0        0        0     1273 2024-05-30 12:47:24.947940 cg-60.9.1/tests/cli/workflow/mip/test_cli_mip_dna_panel.py
--rw-r--r--   0        0        0     3595 2024-05-30 12:47:24.947940 cg-60.9.1/tests/cli/workflow/mip/test_cli_mip_dna_run.py
--rw-r--r--   0        0        0     3884 2024-05-30 12:47:24.947940 cg-60.9.1/tests/cli/workflow/mip/test_cli_mip_dna_start.py
--rw-r--r--   0        0        0     1004 2024-05-30 12:47:24.947940 cg-60.9.1/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py
--rw-r--r--   0        0        0      527 2024-05-30 12:47:24.947940 cg-60.9.1/tests/cli/workflow/mip/test_cli_mip_rna_link.py
--rw-r--r--   0        0        0      716 2024-05-30 12:47:24.947940 cg-60.9.1/tests/cli/workflow/mip/test_cli_mip_rna_run.py
--rw-r--r--   0        0        0     8559 2024-05-30 12:47:24.947940 cg-60.9.1/tests/cli/workflow/mip/test_cli_mip_store.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.947940 cg-60.9.1/tests/cli/workflow/nf_analysis/__init__.py
--rw-r--r--   0        0        0     8504 2024-05-30 12:47:24.947940 cg-60.9.1/tests/cli/workflow/nf_analysis/test_cli_config_case.py
--rw-r--r--   0        0        0     3831 2024-05-30 12:47:24.947940 cg-60.9.1/tests/cli/workflow/nf_analysis/test_cli_metrics_deliver.py
--rw-r--r--   0        0        0     5087 2024-05-30 12:47:24.947940 cg-60.9.1/tests/cli/workflow/nf_analysis/test_cli_report_deliver.py
--rw-r--r--   0        0        0     9211 2024-05-30 12:47:24.947940 cg-60.9.1/tests/cli/workflow/nf_analysis/test_cli_run.py
--rw-r--r--   0        0        0     3331 2024-05-30 12:47:24.947940 cg-60.9.1/tests/cli/workflow/nf_analysis/test_cli_start.py
--rw-r--r--   0        0        0     9877 2024-05-30 12:47:24.947940 cg-60.9.1/tests/cli/workflow/nf_analysis/test_cli_store.py
--rw-r--r--   0        0        0    10453 2024-05-30 12:47:24.947940 cg-60.9.1/tests/cli/workflow/nf_analysis/test_cli_store_housekeeper.py
--rw-r--r--   0        0        0      978 2024-05-30 12:47:24.947940 cg-60.9.1/tests/cli/workflow/nf_analysis/test_cli_workflow_base.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.947940 cg-60.9.1/tests/cli/workflow/raredisease/__init__.py
--rw-r--r--   0        0        0     3940 2024-05-30 12:47:24.947940 cg-60.9.1/tests/cli/workflow/raredisease/test_cli_raredisease_compound_commands.py
--rw-r--r--   0        0        0      921 2024-05-30 12:47:24.947940 cg-60.9.1/tests/cli/workflow/test_cli_workflow.py
--rw-r--r--   0        0        0     4310 2024-05-30 12:47:24.947940 cg-60.9.1/tests/cli/workflow/test_cli_workflow_clean.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.947940 cg-60.9.1/tests/clients/__init__.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.947940 cg-60.9.1/tests/clients/arnold/__init__.py
--rw-r--r--   0        0        0     1080 2024-05-30 12:47:24.947940 cg-60.9.1/tests/clients/arnold/conftest.py
--rw-r--r--   0        0        0     1503 2024-05-30 12:47:24.947940 cg-60.9.1/tests/clients/arnold/test_arnold_api_client.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.947940 cg-60.9.1/tests/clients/janus/__init__.py
--rw-r--r--   0        0        0     2381 2024-05-30 12:47:24.947940 cg-60.9.1/tests/clients/janus/conftest.py
--rw-r--r--   0        0        0     1716 2024-05-30 12:47:24.947940 cg-60.9.1/tests/clients/janus/test_janus_api_client.py
--rw-r--r--   0        0        0   128095 2024-05-30 12:47:24.947940 cg-60.9.1/tests/conftest.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.947940 cg-60.9.1/tests/fixture_plugins/__init__.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.947940 cg-60.9.1/tests/fixture_plugins/delivery_fixtures/__init__.py
--rw-r--r--   0        0        0     2653 2024-05-30 12:47:24.947940 cg-60.9.1/tests/fixture_plugins/delivery_fixtures/bundle_fixtures.py
--rw-r--r--   0        0        0     4972 2024-05-30 12:47:24.947940 cg-60.9.1/tests/fixture_plugins/delivery_fixtures/context_fixtures.py
--rw-r--r--   0        0        0     1494 2024-05-30 12:47:24.947940 cg-60.9.1/tests/fixture_plugins/delivery_fixtures/path_fixtures.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixture_plugins/demultiplex_fixtures/__init__.py
--rw-r--r--   0        0        0     5098 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixture_plugins/demultiplex_fixtures/flow_cell_fixtures.py
--rw-r--r--   0        0        0     3413 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixture_plugins/demultiplex_fixtures/name_fixtures.py
--rw-r--r--   0        0        0    21023 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixture_plugins/demultiplex_fixtures/path_fixtures.py
--rw-r--r--   0        0        0     3419 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixture_plugins/demultiplex_fixtures/run_parameters_fixtures.py
--rw-r--r--   0        0        0     5988 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixture_plugins/demultiplex_fixtures/sample_fixtures.py
--rw-r--r--   0        0        0     8960 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixture_plugins/demultiplex_fixtures/sample_sheet_fixtures.py
--rw-r--r--   0        0        0     1768 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixture_plugins/loqusdb_fixtures/loqusdb_api_fixtures.py
--rw-r--r--   0        0        0     6190 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixture_plugins/loqusdb_fixtures/loqusdb_output_fixtures.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixture_plugins/observations_fixtures/__init__.py
--rw-r--r--   0        0        0     2953 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixture_plugins/observations_fixtures/observations_api_fixtures.py
--rw-r--r--   0        0        0     1512 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixture_plugins/observations_fixtures/observations_input_files_fixtures.py
--rw-r--r--   0        0        0     3174 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixture_plugins/quality_controller_fixtures/sequencing_qc_check_scenario.py
--rw-r--r--   0        0        0     4801 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixture_plugins/quality_controller_fixtures/sequencing_qc_fixtures.py
--rw-r--r--   0        0        0     1304 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixture_plugins/timestamp_fixtures.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixtures/analysis/balsamic/tn_wgs/adm1.cram
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixtures/analysis/balsamic/tn_wgs/ascat.output.pdf
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixtures/analysis/balsamic/tn_wgs/snv.vcf
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixtures/analysis/balsamic/tn_wgs/sv.vcf
--rw-r--r--   0        0        0    14644 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json
--rw-r--r--   0        0        0    15921 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixtures/analysis/mip/dna/ADM1.baf.bed.gz
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixtures/analysis/mip/dna/ADM1.cov.bed.gz
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixtures/analysis/mip/dna/ADM2.cram
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixtures/analysis/mip/dna/ADM3.cram
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixtures/analysis/mip/dna/adm1.cram
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixtures/analysis/mip/dna/adm1.mt.bam
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixtures/analysis/mip/dna/multiqc.html
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixtures/analysis/mip/dna/report.pdf
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixtures/analysis/mip/dna/smn.vcf
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixtures/analysis/mip/dna/snv.vcf
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixtures/analysis/mip/dna/snv_research.vcf
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixtures/analysis/mip/dna/str.vcf
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixtures/analysis/mip/dna/sv.vcf
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixtures/analysis/mip/dna/sv_research.vcf
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixtures/analysis/mip/dna/vcf2cytosure.txt
--rw-r--r--   0        0        0       70 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixtures/analysis/nf-analysis/pipeline_params.config
--rw-r--r--   0        0        0      195 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixtures/analysis/nf-analysis/pipeline_resource_optimisation.config
--rw-r--r--   0        0        0      195 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixtures/analysis/nf-analysis/platform.config
--rw-r--r--   0        0        0     8177 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixtures/analysis/raredisease/multiqc_data.json
--rw-r--r--   0        0        0    20039 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixtures/analysis/raredisease/raredisease_case_enough_reads_metrics_deliverables.yaml
--rw-r--r--   0        0        0     5497 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixtures/analysis/rnafusion/multiqc_data.json
--rw-r--r--   0        0        0    12499 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixtures/analysis/rnafusion/rnafusion_case_enough_reads_metrics_deliverables.yaml
--rw-r--r--   0        0        0     2873 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixtures/analysis/sample_coverage.bed
--rw-r--r--   0        0        0     6506 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixtures/analysis/taxprofiler/multiqc_data.json
--rw-r--r--   0        0        0    10513 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixtures/analysis/taxprofiler/taxprofiler_case_metrics_deliverables.yaml
--rw-r--r--   0        0        0     5771 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixtures/analysis/tomte/multiqc_data.json
--rw-r--r--   0        0        0    14859 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixtures/analysis/tomte/tomte_case_enough_reads_metrics_deliverables.yaml
--rw-r--r--   0        0        0    10961 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixtures/apps/balsamic/case/config.json
--rw-r--r--   0        0        0     3465 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixtures/apps/balsamic/case/metadata.yml
--rw-r--r--   0        0        0       63 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixtures/apps/balsamic/case/metadata_directory.yml
--rw-r--r--   0        0        0      165 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixtures/apps/balsamic/case/metadata_file_tags.yml
--rw-r--r--   0        0        0     2705 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml
--rw-r--r--   0        0        0      692 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixtures/apps/crunchy/spring_metadata.json
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/ACC2655A1_S2_L002_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/ACC2655A1_S2_L002_R2_001.fastq.gz
--rw-r--r--   0        0        0      412 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/Reports/Adapter_Metrics.csv
--rw-r--r--   0        0        0      484 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/Reports/Demultiplex_Stats.csv
--rw-r--r--   0        0        0      658 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/Reports/Quality_Metrics.csv
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/SVE2648A1_S1_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/SVE2648A1_S1_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/Undetermined_S0_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/Undetermined_S0_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/demuxcomplete.txt
--rw-r--r--   0        0        0     1757 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
--rw-r--r--   0        0        0        7 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0     6034 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
--rw-r--r--   0        0        0     1172 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
--rw-r--r--   0        0        0        7 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/fastq_1.fastq.gz
--rw-r--r--   0        0        0        7 2024-05-30 12:47:24.955940 cg-60.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/fastq_2.fastq.gz
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.955940 cg-60.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/BCLConvert/fastq/ACC13169A1_S1_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.955940 cg-60.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/BCLConvert/fastq/ACC13169A1_S1_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.955940 cg-60.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/BCLConvert/fastq/ACC13170A6_S2_L002_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.955940 cg-60.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/BCLConvert/fastq/ACC13170A6_S2_L002_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.955940 cg-60.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/BCLConvert/fastq/Undetermined_S0_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.955940 cg-60.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/BCLConvert/fastq/Undetermined_S0_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0      288 2024-05-30 12:47:24.955940 cg-60.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/Reports/Adapter_Metrics.csv
--rw-r--r--   0        0        0      361 2024-05-30 12:47:24.955940 cg-60.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/Reports/Demultiplex_Stats.csv
--rw-r--r--   0        0        0      414 2024-05-30 12:47:24.955940 cg-60.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/Reports/Quality_Metrics.csv
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.955940 cg-60.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/demuxcomplete.txt
--rw-r--r--   0        0        0    47757 2024-05-30 12:47:24.955940 cg-60.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/dragen-replay.json
--rw-r--r--   0        0        0      315 2024-05-30 12:47:24.955940 cg-60.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRZZ/Unaligned/Reports/Adapter_Metrics.csv
--rw-r--r--   0        0        0      434 2024-05-30 12:47:24.955940 cg-60.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRZZ/Unaligned/Reports/Quality_Metrics.csv
--rw-r--r--   0        0        0     8624 2024-05-30 12:47:24.955940 cg-60.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRZZ/Unaligned/Reports/RunInfo.xml
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.955940 cg-60.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/ACC12642A4_S2_L002_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.955940 cg-60.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/ACC12642A4_S2_L002_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.955940 cg-60.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/ACC12642A7_S1_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.955940 cg-60.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/ACC12642A7_S1_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0      303 2024-05-30 12:47:24.955940 cg-60.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/Reports/Adapter_Metrics.csv
--rw-r--r--   0        0        0      364 2024-05-30 12:47:24.955940 cg-60.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/Reports/Demultiplex_Stats.csv
--rw-r--r--   0        0        0      427 2024-05-30 12:47:24.955940 cg-60.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/Reports/Quality_Metrics.csv
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.955940 cg-60.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/Undetermined_S0_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.955940 cg-60.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/Undetermined_S0_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.955940 cg-60.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/demuxcomplete.txt
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0     4439 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
--rw-r--r--   0        0        0     1172 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R2_001.fastq.gz
--rw-r--r--   0        0        0     5127 2024-05-30 12:47:24.951940 cg-60.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/230912_A00187_1009_AHK33MDRX3/SampleSheet.csv
--rw-r--r--   0        0        0       43 2024-05-30 12:47:24.955940 cg-60.9.1/tests/fixtures/apps/demultiplexing/fastq/dummy_run_R1_001.fastq.gz
--rw-r--r--   0        0        0       67 2024-05-30 12:47:24.955940 cg-60.9.1/tests/fixtures/apps/demultiplexing/fastq/dummy_run_R1_001.fastq.gz.md5
--rw-r--r--   0        0        0   338370 2024-05-30 12:47:24.955940 cg-60.9.1/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R1_001.fastq.gz
--rw-r--r--   0        0        0       67 2024-05-30 12:47:24.955940 cg-60.9.1/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R1_001.fastq.gz.md5
--rw-r--r--   0        0        0   338349 2024-05-30 12:47:24.955940 cg-60.9.1/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.955940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/CopyComplete.txt
--rw-r--r--   0        0        0     2126 2024-05-30 12:47:24.955940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/HJCFFALXX_bcl2fastq_raw.json
--rw-r--r--   0        0        0     1827 2024-05-30 12:47:24.955940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/HJCFFALXX_bcl_convert_raw.json
--rw-r--r--   0        0        0       78 2024-05-30 12:47:24.955940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/README.txt
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.955940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTAComplete.txt
--rw-r--r--   0        0        0     6895 2024-05-30 12:47:24.955940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTAConfiguration.xml
--rw-r--r--   0        0        0       37 2024-05-30 12:47:24.955940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTARead1Complete.txt
--rw-r--r--   0        0        0       36 2024-05-30 12:47:24.955940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTARead2Complete.txt
--rw-r--r--   0        0        0       36 2024-05-30 12:47:24.955940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTARead3Complete.txt
--rw-r--r--   0        0        0    24755 2024-05-30 12:47:24.955940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RunInfo.xml
--rw-r--r--   0        0        0      692 2024-05-30 12:47:24.955940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet.csv
--rw-r--r--   0        0        0      724 2024-05-30 12:47:24.955940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet_bcl2fastq.csv
--rw-r--r--   0        0        0       61 2024-05-30 12:47:24.955940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SequencingComplete.txt
--rw-r--r--   0        0        0     5775 2024-05-30 12:47:24.955940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/runParameters.xml
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.955940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/CopyComplete.txt
--rw-r--r--   0        0        0     2282 2024-05-30 12:47:24.955940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/HL32LCCXY_bcl2fastq_raw.json
--rw-r--r--   0        0        0     1632 2024-05-30 12:47:24.955940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/HL32LCCXY_bcl_convert_raw.json
--rw-r--r--   0        0        0       76 2024-05-30 12:47:24.955940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/README.txt
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.955940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTAComplete.txt
--rw-r--r--   0        0        0     6912 2024-05-30 12:47:24.955940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTAConfiguration.xml
--rw-r--r--   0        0        0       36 2024-05-30 12:47:24.955940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTARead1Complete.txt
--rw-r--r--   0        0        0       36 2024-05-30 12:47:24.955940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTARead2Complete.txt
--rw-r--r--   0        0        0       36 2024-05-30 12:47:24.955940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTARead3Complete.txt
--rw-r--r--   0        0        0       36 2024-05-30 12:47:24.955940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTARead4Complete.txt
--rw-r--r--   0        0        0    24814 2024-05-30 12:47:24.955940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RunInfo.xml
--rw-r--r--   0        0        0      814 2024-05-30 12:47:24.955940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SampleSheet.csv
--rw-r--r--   0        0        0      660 2024-05-30 12:47:24.955940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SampleSheet_bcl2fastq.csv
--rw-r--r--   0        0        0       61 2024-05-30 12:47:24.955940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SequencingComplete.txt
--rw-r--r--   0        0        0     5853 2024-05-30 12:47:24.959940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/runParameters.xml
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.959940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/CopyComplete.txt
--rw-r--r--   0        0        0    21848 2024-05-30 12:47:24.959940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/HGYFNBCX2_bcl2fastq_raw.json
--rw-r--r--   0        0        0    15512 2024-05-30 12:47:24.959940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/HGYFNBCX2_bcl_convert_raw.json
--rw-r--r--   0        0        0       79 2024-05-30 12:47:24.959940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/README.txt
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.959940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/RTAComplete.txt
--rw-r--r--   0        0        0      756 2024-05-30 12:47:24.959940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/RunInfo.xml
--rw-r--r--   0        0        0     4118 2024-05-30 12:47:24.959940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/SampleSheet.csv
--rw-r--r--   0        0        0     1408 2024-05-30 12:47:24.959940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/SampleSheet_bcl2fastq.csv
--rw-r--r--   0        0        0     5326 2024-05-30 12:47:24.959940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/runParameters.xml
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.959940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/CopyComplete.txt
--rw-r--r--   0        0        0    15041 2024-05-30 12:47:24.959940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/HM2LNBCX2_bcl2fastq_raw.json
--rw-r--r--   0        0        0    10649 2024-05-30 12:47:24.959940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/HM2LNBCX2_bcl_convert_raw.json
--rw-r--r--   0        0        0       81 2024-05-30 12:47:24.959940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/README.txt
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.959940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/RTAComplete.txt
--rw-r--r--   0        0        0      755 2024-05-30 12:47:24.959940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/RunInfo.xml
--rw-r--r--   0        0        0     2878 2024-05-30 12:47:24.959940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/SampleSheet.csv
--rw-r--r--   0        0        0      928 2024-05-30 12:47:24.959940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/SampleSheet_bcl2fastq.csv
--rw-r--r--   0        0        0     5359 2024-05-30 12:47:24.959940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/runParameters.xml
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.959940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/CopyComplete.txt
--rw-r--r--   0        0        0    27887 2024-05-30 12:47:24.959940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/CorrectSampleSheet.csv
--rw-r--r--   0        0        0   141870 2024-05-30 12:47:24.959940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/HLYWYDSXX_bcl2fastq_raw.json
--rwxr-xr-x   0        0        0   122682 2024-05-30 12:47:24.959940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/HLYWYDSXX_bcl_convert_raw.json
--rw-r--r--   0        0        0      243 2024-05-30 12:47:24.959940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/README.txt
--rw-r--r--   0        0        0    28230 2024-05-30 12:47:24.959940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RTA3.cfg
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.959940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RTAComplete.txt
--rw-r--r--   0        0        0    94426 2024-05-30 12:47:24.959940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RunInfo.xml
--rw-r--r--   0        0        0     5819 2024-05-30 12:47:24.959940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RunParameters.xml
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.959940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/SequenceComplete.txt
--rw-r--r--   0        0        0     1757 2024-05-30 12:47:24.959940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
--rw-r--r--   0        0        0     1757 2024-05-30 12:47:24.959940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stdout
--rw-r--r--   0        0        0    47522 2024-05-30 12:47:24.959940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_raw.json
--rw-r--r--   0        0        0       12 2024-05-30 12:47:24.959940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/README.txt
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.959940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/RTAComplete.txt
--rw-r--r--   0        0        0     6666 2024-05-30 12:47:24.959940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/RunParameters.xml
--rw-r--r--   0        0        0      254 2024-05-30 12:47:24.959940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.959940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/copycomplete.txt
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.959940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/delivery.txt
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.959940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/demuxstarted.txt
--rwxr-xr-x   0        0        0    47434 2024-05-30 12:47:24.959940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/22F52TLT3_raw.json
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.959940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/CopyComplete.txt
--rw-r--r--   0        0        0    10950 2024-05-30 12:47:24.959940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/CorrectSampleSheet.csv
--rw-r--r--   0        0        0      225 2024-05-30 12:47:24.959940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/Manifest.tsv
--rw-r--r--   0        0        0       55 2024-05-30 12:47:24.959940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/README.txt
--rwxr-xr-x   0        0        0     2493 2024-05-30 12:47:24.959940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RTA.cfg
--rwxr-xr-x   0        0        0        1 2024-05-30 12:47:24.959940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RTAComplete.txt
--rwxr-xr-x   0        0        0        2 2024-05-30 12:47:24.959940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RTAExited.txt
--rwxr-xr-x   0        0        0      730 2024-05-30 12:47:24.959940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunCompletionStatus.xml
--rwxr-xr-x   0        0        0    79277 2024-05-30 12:47:24.959940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunInfo.xml
--rwxr-xr-x   0        0        0     2694 2024-05-30 12:47:24.959940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunParameters.xml
--rw-r--r--   0        0        0    10950 2024-05-30 12:47:24.959940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.959940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/CopyComplete.txt
--rw-r--r--   0        0        0      509 2024-05-30 12:47:24.959940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stderr
--rw-r--r--   0        0        0     2229 2024-05-30 12:47:24.959940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stdout
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.959940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/RTAComplete.txt
--rw-r--r--   0        0        0     6665 2024-05-30 12:47:24.959940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/RunParameters.xml
--rw-r--r--   0        0        0      619 2024-05-30 12:47:24.959940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.959940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/CopyComplete.txt
--rw-r--r--   0        0        0     4941 2024-05-30 12:47:24.959940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/CorrectSampleSheet.csv
--rwxr-xr-x   0        0        0    20050 2024-05-30 12:47:24.959940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/HK33MDRX3_bcl_convert_raw.json
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.959940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/HK33MDRX3_demultiplex.stderr
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.959940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/HK33MDRX3_demultiplex.stdout
--rw-r--r--   0        0        0      244 2024-05-30 12:47:24.959940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/README.txt
--rw-r--r--   0        0        0     6391 2024-05-30 12:47:24.959940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RTA3.cfg
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.959940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RTAComplete.txt
--rw-r--r--   0        0        0    16428 2024-05-30 12:47:24.959940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RunInfo.xml
--rw-r--r--   0        0        0     6728 2024-05-30 12:47:24.959940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RunParameters.xml
--rw-r--r--   0        0        0     5127 2024-05-30 12:47:24.959940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.963940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/SequenceComplete.txt
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.963940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/demuxstarted.txt
--rw-r--r--   0        0        0      133 2024-05-30 12:47:24.963940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/170517_ST-E00266_0210_BHJCFFALXX/README.txt
--rw-r--r--   0        0        0      724 2024-05-30 12:47:24.963940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet.csv
--rw-r--r--   0        0        0     5775 2024-05-30 12:47:24.963940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/170517_ST-E00266_0210_BHJCFFALXX/runParameters.xml
--rw-r--r--   0        0        0      124 2024-05-30 12:47:24.963940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/180509_D00450_0598_BHGYFNBCX2/README.txt
--rw-r--r--   0        0        0      310 2024-05-30 12:47:24.963940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/190927_A00689_0069_BHLYWYDSXX/README.txt
--rw-r--r--   0        0        0     5819 2024-05-30 12:47:24.963940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/190927_A00689_0069_BHLYWYDSXX/RunParameters.xml
--rw-r--r--   0        0        0      122 2024-05-30 12:47:24.963940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/20231108_LH00188_0028_B22F52TLT3/README.txt
--rwxr-xr-x   0        0        0     2694 2024-05-30 12:47:24.963940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/20231108_LH00188_0028_B22F52TLT3/RunParameters.xml
--rw-r--r--   0        0        0      311 2024-05-30 12:47:24.963940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/230912_A00187_1009_AHK33MDRX3/README.txt
--rw-r--r--   0        0        0     6728 2024-05-30 12:47:24.963940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/230912_A00187_1009_AHK33MDRX3/RunParameters.xml
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.963940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/CopyComplete.txt
--rw-r--r--   0        0        0      509 2024-05-30 12:47:24.963940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stderr
--rw-r--r--   0        0        0     2229 2024-05-30 12:47:24.963940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.963940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/RTAComplete.txt
--rw-r--r--   0        0        0     6665 2024-05-30 12:47:24.963940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml
--rw-r--r--   0        0        0      399 2024-05-30 12:47:24.963940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.963940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/CopyComplete.txt
--rw-r--r--   0        0        0      509 2024-05-30 12:47:24.963940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stderr
--rw-r--r--   0        0        0     2229 2024-05-30 12:47:24.963940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stdout
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.963940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/RTAComplete.txt
--rw-r--r--   0        0        0     6665 2024-05-30 12:47:24.963940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/RunParameters.xml
--rw-r--r--   0        0        0      399 2024-05-30 12:47:24.963940 cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.963940 cg-60.9.1/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/fastq_pass/PAS86456_pass_72d9fceb_8a4fd683_0.fastq.gz
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.963940 cg-60.9.1/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/fastq_pass/PAS86456_pass_72d9fceb_8a4fd683_1.fastq.gz
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.963940 cg-60.9.1/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/final_summary_PAS86456_72d9fceb_8a4fd683.txt
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.963940 cg-60.9.1/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/pod5_pass/PAS86456_pass_72d9fceb_8a4fd683_0.pod5
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.963940 cg-60.9.1/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/pod5_pass/PAS86456_pass_72d9fceb_8a4fd683_1.pod5
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.963940 cg-60.9.1/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/fastq_pass/PAS97781_pass_595b5663_efc7f02e_0.fastq.gz
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.963940 cg-60.9.1/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/fastq_pass/PAS97781_pass_595b5663_efc7f02e_1.fastq.gz
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.963940 cg-60.9.1/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/final_summary_PAS97781_595b5663_efc7f02e.txt
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.963940 cg-60.9.1/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/pod5_pass/PAS97781_pass_595b5663_efc7f02e_0.pod5
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.963940 cg-60.9.1/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/pod5_pass/PAS97781_pass_595b5663_efc7f02e_1.pod5
--rw-r--r--   0        0        0     5319 2024-05-30 12:47:24.963940 cg-60.9.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_hiseq_2500_different_index_cycles.xml
--rw-r--r--   0        0        0     5944 2024-05-30 12:47:24.963940 cg-60.9.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_6000_different_index_cycles.xml
--rwxr-xr-x   0        0        0     2603 2024-05-30 12:47:24.963940 cg-60.9.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_different_index_cycles.xml
--rwxr-xr-x   0        0        0     2597 2024-05-30 12:47:24.963940 cg-60.9.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_wrong_instrument.xml
--rw-r--r--   0        0        0     5899 2024-05-30 12:47:24.963940 cg-60.9.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_no_software_nor_reagent_version.xml
--rw-r--r--   0        0        0     4941 2024-05-30 12:47:24.963940 cg-60.9.1/tests/fixtures/apps/demultiplexing/sample_sheets/novaseq_6000_sample_sheet_with_reversed_cycles.csv
--rw-r--r--   0        0        0    10950 2024-05-30 12:47:24.963940 cg-60.9.1/tests/fixtures/apps/demultiplexing/sample_sheets/novaseq_x_sample_sheet_with_forward_cycles.csv
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.963940 cg-60.9.1/tests/fixtures/apps/demultiplexing/spring/dummy_run_001.spring
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.963940 cg-60.9.1/tests/fixtures/apps/demultiplexing/spring/dummy_run_002.spring
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.963940 cg-60.9.1/tests/fixtures/apps/demultiplexing/spring/dummy_spring_meta_data.json
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.963940 cg-60.9.1/tests/fixtures/apps/fluffy/2020-23219-05/2020-23219-05.WCXpredict_aberrations.filt.bed
--rw-r--r--   0        0        0     5554 2024-05-30 12:47:24.963940 cg-60.9.1/tests/fixtures/apps/fluffy/SampleSheet.csv
--rw-r--r--   0        0        0      901 2024-05-30 12:47:24.963940 cg-60.9.1/tests/fixtures/apps/fluffy/deliverables.yaml
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.963940 cg-60.9.1/tests/fixtures/apps/fluffy/fluffy_fastq.fastq.gz
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.963940 cg-60.9.1/tests/fixtures/apps/fluffy/multiqc_report.html
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.963940 cg-60.9.1/tests/fixtures/apps/fluffy/summary.csv
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.963940 cg-60.9.1/tests/fixtures/apps/gt/yellowhog.bcf
--rw-r--r--   0        0        0     5114 2024-05-30 12:47:24.963940 cg-60.9.1/tests/fixtures/apps/madeline/madeline.xml
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.963940 cg-60.9.1/tests/fixtures/apps/mip/case_file.txt
--rw-r--r--   0        0        0     3241 2024-05-30 12:47:24.963940 cg-60.9.1/tests/fixtures/apps/mip/case_metrics_deliverables.yaml
--rw-r--r--   0        0        0    21811 2024-05-30 12:47:24.963940 cg-60.9.1/tests/fixtures/apps/mip/dna/store/case_config.yaml
--rw-r--r--   0        0        0    23364 2024-05-30 12:47:24.963940 cg-60.9.1/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml
--rw-r--r--   0        0        0    37367 2024-05-30 12:47:24.963940 cg-60.9.1/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml
--rw-r--r--   0        0        0       16 2024-05-30 12:47:24.963940 cg-60.9.1/tests/fixtures/apps/mip/dna/store/empty_case_config.yaml
--rw-r--r--   0        0        0       16 2024-05-30 12:47:24.963940 cg-60.9.1/tests/fixtures/apps/mip/dna/store/empty_case_metrics_deliverables.yaml
--rw-r--r--   0        0        0       16 2024-05-30 12:47:24.963940 cg-60.9.1/tests/fixtures/apps/mip/dna/store/empty_case_qc_sample_info.yaml
--rw-r--r--   0        0        0      123 2024-05-30 12:47:24.963940 cg-60.9.1/tests/fixtures/apps/mip/dna/store/empty_delivery_report.html
--rw-r--r--   0        0        0    62741 2024-05-30 12:47:24.963940 cg-60.9.1/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf
--rw-r--r--   0        0        0    11242 2024-05-30 12:47:24.963940 cg-60.9.1/tests/fixtures/apps/mip/rna/case_config.yaml
--rw-r--r--   0        0        0    12164 2024-05-30 12:47:24.963940 cg-60.9.1/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml
--rw-r--r--   0        0        0     5231 2024-05-30 12:47:24.963940 cg-60.9.1/tests/fixtures/apps/mip/rna/store/bundle_data.yaml
--rw-r--r--   0        0        0     9774 2024-05-30 12:47:24.963940 cg-60.9.1/tests/fixtures/apps/mip/rna/store/case_config.yaml
--rw-r--r--   0        0        0     4624 2024-05-30 12:47:24.963940 cg-60.9.1/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml
--rw-r--r--   0        0        0    13666 2024-05-30 12:47:24.963940 cg-60.9.1/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.963940 cg-60.9.1/tests/fixtures/apps/mip/sample_file.txt
--rw-r--r--   0        0        0     1885 2024-05-30 12:47:24.963940 cg-60.9.1/tests/fixtures/apps/scout/643594.config.yaml
--rw-r--r--   0        0        0     6027 2024-05-30 12:47:24.963940 cg-60.9.1/tests/fixtures/apps/scout/case_export.json
--rw-r--r--   0        0        0     9349 2024-05-30 12:47:24.967940 cg-60.9.1/tests/fixtures/apps/scout/export_causatives.json
--rw-r--r--   0        0        0     1315 2024-05-30 12:47:24.967940 cg-60.9.1/tests/fixtures/apps/scout/none_case_export.json
--rw-r--r--   0        0        0     3518 2024-05-30 12:47:24.967940 cg-60.9.1/tests/fixtures/apps/scout/other_sex_case.json
--rw-r--r--   0        0        0     8874 2024-05-30 12:47:24.967940 cg-60.9.1/tests/fixtures/apps/scout/panel_export.bed
--rw-r--r--   0        0        0     4169 2024-05-30 12:47:24.967940 cg-60.9.1/tests/fixtures/apps/scout/panel_export.csv
--rw-r--r--   0        0        0       42 2024-05-30 12:47:24.967940 cg-60.9.1/tests/fixtures/apps/shipping/scout-deploy.yaml
--rw-r--r--   0        0        0     1036 2024-05-30 12:47:24.967940 cg-60.9.1/tests/fixtures/cgweb_orders/balsamic.json
--rw-r--r--   0        0        0     1104 2024-05-30 12:47:24.967940 cg-60.9.1/tests/fixtures/cgweb_orders/fastq.json
--rw-r--r--   0        0        0     1313 2024-05-30 12:47:24.967940 cg-60.9.1/tests/fixtures/cgweb_orders/metagenome.json
--rw-r--r--   0        0        0     3038 2024-05-30 12:47:24.967940 cg-60.9.1/tests/fixtures/cgweb_orders/microsalt.json
--rw-r--r--   0        0        0     3705 2024-05-30 12:47:24.967940 cg-60.9.1/tests/fixtures/cgweb_orders/mip.json
--rw-r--r--   0        0        0     1364 2024-05-30 12:47:24.967940 cg-60.9.1/tests/fixtures/cgweb_orders/mip_rna.json
--rw-r--r--   0        0        0     2125 2024-05-30 12:47:24.967940 cg-60.9.1/tests/fixtures/cgweb_orders/rml.json
--rw-r--r--   0        0        0     1368 2024-05-30 12:47:24.967940 cg-60.9.1/tests/fixtures/cgweb_orders/rnafusion.json
--rw-r--r--   0        0        0     4684 2024-05-30 12:47:24.967940 cg-60.9.1/tests/fixtures/cgweb_orders/sarscov2.json
--rw-r--r--   0        0        0     3811 2024-05-30 12:47:24.967940 cg-60.9.1/tests/fixtures/cgweb_orders/tomte.json
--rw-r--r--   0        0        0     5609 2024-05-30 12:47:24.967940 cg-60.9.1/tests/fixtures/data/SampleSheet.csv
--rw-r--r--   0        0        0      511 2024-05-30 12:47:24.967940 cg-60.9.1/tests/fixtures/data/bcl_convert_sample_sheet.csv
--rw-r--r--   0        0        0   258048 2024-05-30 12:47:24.967940 cg-60.9.1/tests/fixtures/data/cgfixture.db
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.967940 cg-60.9.1/tests/fixtures/data/fastq.fastq.gz
--rw-r--r--   0        0        0    49152 2024-05-30 12:47:24.967940 cg-60.9.1/tests/fixtures/data/hkstore.db
--rw-r--r--   0        0        0       73 2024-05-30 12:47:24.967940 cg-60.9.1/tests/fixtures/data/yellowhog/pedigree.yaml
--rw-r--r--   0        0        0       76 2024-05-30 12:47:24.967940 cg-60.9.1/tests/fixtures/io/casava_five_parts.fastq.gz
--rw-r--r--   0        0        0       90 2024-05-30 12:47:24.967940 cg-60.9.1/tests/fixtures/io/casava_seven_parts.fastq.gz
--rw-r--r--   0        0        0       96 2024-05-30 12:47:24.967940 cg-60.9.1/tests/fixtures/io/casava_ten_parts.fastq.gz
--rw-r--r--   0        0        0      153 2024-05-30 12:47:24.967940 cg-60.9.1/tests/fixtures/io/example.csv
--rw-r--r--   0        0        0       46 2024-05-30 12:47:24.967940 cg-60.9.1/tests/fixtures/io/example.gz
--rw-r--r--   0        0        0      147 2024-05-30 12:47:24.967940 cg-60.9.1/tests/fixtures/io/example.tsv
--rw-r--r--   0        0        0       20 2024-05-30 12:47:24.967940 cg-60.9.1/tests/fixtures/io/example.txt
--rw-r--r--   0        0        0       20 2024-05-30 12:47:24.967940 cg-60.9.1/tests/fixtures/io/example2.txt
--rw-r--r--   0        0        0      582 2024-05-30 12:47:24.967940 cg-60.9.1/tests/fixtures/io/example_json.json
--rw-r--r--   0        0        0      103 2024-05-30 12:47:24.967940 cg-60.9.1/tests/fixtures/io/example_xml.xml
--rw-r--r--   0        0        0       20 2024-05-30 12:47:24.967940 cg-60.9.1/tests/fixtures/meta/qc_metrics/file_with_right_tags.json
--rw-r--r--   0        0        0       20 2024-05-30 12:47:24.967940 cg-60.9.1/tests/fixtures/meta/qc_metrics/file_without_right_tags.json
--rw-r--r--   0        0        0   258670 2024-05-30 12:47:24.971940 cg-60.9.1/tests/fixtures/orderforms/1508.31.balsamic.xlsx
--rw-r--r--   0        0        0   258572 2024-05-30 12:47:24.971940 cg-60.9.1/tests/fixtures/orderforms/1508.31.balsamic_qc.xlsx
--rw-r--r--   0        0        0   258081 2024-05-30 12:47:24.971940 cg-60.9.1/tests/fixtures/orderforms/1508.31.balsamic_umi.xlsx
--rw-r--r--   0        0        0   258109 2024-05-30 12:47:24.971940 cg-60.9.1/tests/fixtures/orderforms/1508.31.fastq.xlsx
--rw-r--r--   0        0        0   256330 2024-05-30 12:47:24.971940 cg-60.9.1/tests/fixtures/orderforms/1508.31.metagenome.xlsx
--rw-r--r--   0        0        0   258966 2024-05-30 12:47:24.975940 cg-60.9.1/tests/fixtures/orderforms/1508.31.mip.xlsx
--rw-r--r--   0        0        0   258987 2024-05-30 12:47:24.975940 cg-60.9.1/tests/fixtures/orderforms/1508.31.mip_rna.xlsx
--rw-r--r--   0        0        0   258708 2024-05-30 12:47:24.975940 cg-60.9.1/tests/fixtures/orderforms/1508.31.rnafusion.xlsx
--rw-r--r--   0        0        0   258603 2024-05-30 12:47:24.975940 cg-60.9.1/tests/fixtures/orderforms/1508.31.tomte.xlsx
--rw-r--r--   0        0        0    82677 2024-05-30 12:47:24.975940 cg-60.9.1/tests/fixtures/orderforms/1603.11.microbial.xlsx
--rw-r--r--   0        0        0   149394 2024-05-30 12:47:24.975940 cg-60.9.1/tests/fixtures/orderforms/1604.17.rml.xlsx
--rw-r--r--   0        0        0   223184 2024-05-30 12:47:24.979940 cg-60.9.1/tests/fixtures/orderforms/2184.9.sarscov2.xlsx
--rw-r--r--   0        0        0    18639 2024-05-30 12:47:24.979940 cg-60.9.1/tests/fixtures/orderforms/NIPT-json.json
--rw-r--r--   0        0        0     6052 2024-05-30 12:47:24.979940 cg-60.9.1/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json
--rw-r--r--   0        0        0     6611 2024-05-30 12:47:24.979940 cg-60.9.1/tests/fixtures/orderforms/mip_uploaded_json_orderform.json
--rw-r--r--   0        0        0     1417 2024-05-30 12:47:24.979940 cg-60.9.1/tests/fixtures/report/case_data.json
--rw-r--r--   0        0        0     1109 2024-05-30 12:47:24.979940 cg-60.9.1/tests/fixtures/report/lims_exported_samples.json
--rw-r--r--   0        0        0     1562 2024-05-30 12:47:24.979940 cg-60.9.1/tests/fixtures/report/lims_family.json
--rw-r--r--   0        0        0      619 2024-05-30 12:47:24.979940 cg-60.9.1/tests/fixtures/services/illumina_metrics_service/230622_A00621_0864_AHY7FFDRX2/SampleSheet.csv
--rw-r--r--   0        0        0     2554 2024-05-30 12:47:24.979940 cg-60.9.1/tests/fixtures/services/illumina_metrics_service/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Adapter_Metrics.csv
--rw-r--r--   0        0        0     2016 2024-05-30 12:47:24.979940 cg-60.9.1/tests/fixtures/services/illumina_metrics_service/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Demultiplex_Stats.csv
--rw-r--r--   0        0        0     3607 2024-05-30 12:47:24.979940 cg-60.9.1/tests/fixtures/services/illumina_metrics_service/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Quality_Metrics.csv
--rw-r--r--   0        0        0      248 2024-05-30 12:47:24.979940 cg-60.9.1/tests/fixtures/services/validate_file_transfer_service/pacbio_transfer_done
--rw-r--r--   0        0        0      279 2024-05-30 12:47:24.979940 cg-60.9.1/tests/fixtures/services/validate_file_transfer_service/pacbio_transfer_done_fail
--rw-r--r--   0        0        0     3296 2024-05-30 12:47:24.979940 cg-60.9.1/tests/io/conftest.py
--rw-r--r--   0        0        0      431 2024-05-30 12:47:24.979940 cg-60.9.1/tests/io/test_io_config.py
--rw-r--r--   0        0        0     8639 2024-05-30 12:47:24.979940 cg-60.9.1/tests/io/test_io_controller.py
--rw-r--r--   0        0        0     3877 2024-05-30 12:47:24.979940 cg-60.9.1/tests/io/test_io_csv.py
--rw-r--r--   0        0        0      482 2024-05-30 12:47:24.979940 cg-60.9.1/tests/io/test_io_gzip.py
--rw-r--r--   0        0        0     1779 2024-05-30 12:47:24.979940 cg-60.9.1/tests/io/test_io_json.py
--rw-r--r--   0        0        0     2914 2024-05-30 12:47:24.979940 cg-60.9.1/tests/io/test_io_txt.py
--rw-r--r--   0        0        0     1027 2024-05-30 12:47:24.979940 cg-60.9.1/tests/io/test_io_xml.py
--rw-r--r--   0        0        0     2131 2024-05-30 12:47:24.979940 cg-60.9.1/tests/io/test_io_yaml.py
--rw-r--r--   0        0        0     1233 2024-05-30 12:47:24.979940 cg-60.9.1/tests/io/test_validate_path.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.979940 cg-60.9.1/tests/meta/__init__.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.979940 cg-60.9.1/tests/meta/archive/__init__.py
--rw-r--r--   0        0        0    13482 2024-05-30 12:47:24.979940 cg-60.9.1/tests/meta/archive/conftest.py
--rw-r--r--   0        0        0    20911 2024-05-30 12:47:24.979940 cg-60.9.1/tests/meta/archive/test_archive_api.py
--rw-r--r--   0        0        0    10246 2024-05-30 12:47:24.979940 cg-60.9.1/tests/meta/archive/test_archive_cli.py
--rw-r--r--   0        0        0    15766 2024-05-30 12:47:24.979940 cg-60.9.1/tests/meta/archive/test_archiving.py
--rw-r--r--   0        0        0     3807 2024-05-30 12:47:24.979940 cg-60.9.1/tests/meta/backup/conftest.py
--rw-r--r--   0        0        0    26368 2024-05-30 12:47:24.979940 cg-60.9.1/tests/meta/backup/test_meta_backup.py
--rw-r--r--   0        0        0    10055 2024-05-30 12:47:24.979940 cg-60.9.1/tests/meta/backup/test_meta_pdc.py
--rw-r--r--   0        0        0    12570 2024-05-30 12:47:24.979940 cg-60.9.1/tests/meta/clean/conftest.py
--rw-r--r--   0        0        0    16944 2024-05-30 12:47:24.979940 cg-60.9.1/tests/meta/clean/test_clean_flow_cells_api.py
--rw-r--r--   0        0        0     2286 2024-05-30 12:47:24.979940 cg-60.9.1/tests/meta/clean/test_clean_retrieved_spring_files.py
--rw-r--r--   0        0        0     7691 2024-05-30 12:47:24.979940 cg-60.9.1/tests/meta/compress/conftest.py
--rw-r--r--   0        0        0     7961 2024-05-30 12:47:24.979940 cg-60.9.1/tests/meta/compress/test_clean_fastq.py
--rw-r--r--   0        0        0     1778 2024-05-30 12:47:24.979940 cg-60.9.1/tests/meta/compress/test_compress_files.py
--rw-r--r--   0        0        0     3644 2024-05-30 12:47:24.979940 cg-60.9.1/tests/meta/compress/test_compress_meta_fastq.py
--rw-r--r--   0        0        0     1180 2024-05-30 12:47:24.979940 cg-60.9.1/tests/meta/compress/test_decompress_spring_meta.py
--rw-r--r--   0        0        0     7045 2024-05-30 12:47:24.979940 cg-60.9.1/tests/meta/compress/test_meta_compress_update_hk.py
--rw-r--r--   0        0        0     8269 2024-05-30 12:47:24.979940 cg-60.9.1/tests/meta/conftest.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.979940 cg-60.9.1/tests/meta/deliver/__init__.py
--rw-r--r--   0        0        0     3525 2024-05-30 12:47:24.979940 cg-60.9.1/tests/meta/deliver/conftest.py
--rw-r--r--   0        0        0     5533 2024-05-30 12:47:24.979940 cg-60.9.1/tests/meta/deliver/test_deliver_ticket.py
--rw-r--r--   0        0        0    10331 2024-05-30 12:47:24.979940 cg-60.9.1/tests/meta/deliver/test_delivery_api.py
--rw-r--r--   0        0        0     1057 2024-05-30 12:47:24.979940 cg-60.9.1/tests/meta/deliver/test_fastq_path_generator.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.979940 cg-60.9.1/tests/meta/delivery/__init__.py
--rw-r--r--   0        0        0    16660 2024-05-30 12:47:24.979940 cg-60.9.1/tests/meta/delivery/test_delivery_api.py
--rw-r--r--   0        0        0     8066 2024-05-30 12:47:24.979940 cg-60.9.1/tests/meta/demultiplex/conftest.py
--rw-r--r--   0        0        0     5382 2024-05-30 12:47:24.979940 cg-60.9.1/tests/meta/demultiplex/test_combine_sequencing_metrics.py
--rw-r--r--   0        0        0     8659 2024-05-30 12:47:24.979940 cg-60.9.1/tests/meta/demultiplex/test_demux_post_processing.py
--rw-r--r--   0        0        0    13740 2024-05-30 12:47:24.979940 cg-60.9.1/tests/meta/demultiplex/test_housekeeper_storage_functions.py
--rw-r--r--   0        0        0     4392 2024-05-30 12:47:24.979940 cg-60.9.1/tests/meta/demultiplex/test_status_db_storage_functions.py
--rw-r--r--   0        0        0    22787 2024-05-30 12:47:24.979940 cg-60.9.1/tests/meta/demultiplex/test_utils.py
--rw-r--r--   0        0        0     6301 2024-05-30 12:47:24.979940 cg-60.9.1/tests/meta/demultiplex/test_validation.py
--rw-r--r--   0        0        0     4943 2024-05-30 12:47:24.979940 cg-60.9.1/tests/meta/encryption/conftest.py
--rw-r--r--   0        0        0    18133 2024-05-30 12:47:24.979940 cg-60.9.1/tests/meta/encryption/test_encryption.py
--rw-r--r--   0        0        0     7289 2024-05-30 12:47:24.983940 cg-60.9.1/tests/meta/observations/test_balsamic_observations_api.py
--rw-r--r--   0        0        0     6177 2024-05-30 12:47:24.983940 cg-60.9.1/tests/meta/observations/test_mip_dna_observations_api.py
--rw-r--r--   0        0        0    18356 2024-05-30 12:47:24.983940 cg-60.9.1/tests/meta/observations/test_observations_api.py
--rw-r--r--   0        0        0     5345 2024-05-30 12:47:24.983940 cg-60.9.1/tests/meta/orders/conftest.py
--rw-r--r--   0        0        0     1749 2024-05-30 12:47:24.983940 cg-60.9.1/tests/meta/orders/test_PoolSubmitter_validate_order.py
--rw-r--r--   0        0        0     1470 2024-05-30 12:47:24.983940 cg-60.9.1/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py
--rw-r--r--   0        0        0     1768 2024-05-30 12:47:24.983940 cg-60.9.1/tests/meta/orders/test_SarsCov2Submitter_store_order.py
--rw-r--r--   0        0        0     2032 2024-05-30 12:47:24.983940 cg-60.9.1/tests/meta/orders/test_SarsCov2Submitter_validate_order.py
--rw-r--r--   0        0        0    19783 2024-05-30 12:47:24.983940 cg-60.9.1/tests/meta/orders/test_meta_orders_api.py
--rw-r--r--   0        0        0     7086 2024-05-30 12:47:24.983940 cg-60.9.1/tests/meta/orders/test_meta_orders_lims.py
--rw-r--r--   0        0        0    28893 2024-05-30 12:47:24.983940 cg-60.9.1/tests/meta/orders/test_meta_orders_status.py
--rw-r--r--   0        0        0     1677 2024-05-30 12:47:24.983940 cg-60.9.1/tests/meta/orders/test_rnafusion_submitter.py
--rw-r--r--   0        0        0     1068 2024-05-30 12:47:24.983940 cg-60.9.1/tests/meta/orders/test_ticket_handler.py
--rw-r--r--   0        0        0     4336 2024-05-30 12:47:24.983940 cg-60.9.1/tests/meta/qc_metrics/conftest.py
--rw-r--r--   0        0        0     1972 2024-05-30 12:47:24.983940 cg-60.9.1/tests/meta/qc_metrics/test_collect_qc_metrics.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.983940 cg-60.9.1/tests/meta/report/__init__.py
--rw-r--r--   0        0        0     6512 2024-05-30 12:47:24.983940 cg-60.9.1/tests/meta/report/conftest.py
--rw-r--r--   0        0        0      434 2024-05-30 12:47:24.983940 cg-60.9.1/tests/meta/report/helper.py
--rw-r--r--   0        0        0     2604 2024-05-30 12:47:24.983940 cg-60.9.1/tests/meta/report/test_balsamic_api.py
--rw-r--r--   0        0        0     4056 2024-05-30 12:47:24.983940 cg-60.9.1/tests/meta/report/test_field_validators.py
--rw-r--r--   0        0        0     2858 2024-05-30 12:47:24.983940 cg-60.9.1/tests/meta/report/test_mip_dna_api.py
--rw-r--r--   0        0        0    16042 2024-05-30 12:47:24.983940 cg-60.9.1/tests/meta/report/test_report_api.py
--rw-r--r--   0        0        0     3123 2024-05-30 12:47:24.983940 cg-60.9.1/tests/meta/report/test_rnafusion_api.py
--rw-r--r--   0        0        0     1250 2024-05-30 12:47:24.983940 cg-60.9.1/tests/meta/report/test_tomte_api.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.983940 cg-60.9.1/tests/meta/rsync/__init__.py
--rw-r--r--   0        0        0      916 2024-05-30 12:47:24.983940 cg-60.9.1/tests/meta/rsync/conftest.py
--rw-r--r--   0        0        0     9442 2024-05-30 12:47:24.983940 cg-60.9.1/tests/meta/rsync/test_rsync.py
--rw-r--r--   0        0        0     3147 2024-05-30 12:47:24.983940 cg-60.9.1/tests/meta/test_invoice.py
--rw-r--r--   0        0        0     1220 2024-05-30 12:47:24.983940 cg-60.9.1/tests/meta/transfer/conftest.py
--rw-r--r--   0        0        0    10552 2024-05-30 12:47:24.983940 cg-60.9.1/tests/meta/transfer/test_external_data.py
--rw-r--r--   0        0        0     4395 2024-05-30 12:47:24.983940 cg-60.9.1/tests/meta/transfer/test_meta_transfer_lims.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.983940 cg-60.9.1/tests/meta/upload/__init__.py
--rw-r--r--   0        0        0     2210 2024-05-30 12:47:24.983940 cg-60.9.1/tests/meta/upload/balsamic/test_balsamic.py
--rw-r--r--   0        0        0     4002 2024-05-30 12:47:24.983940 cg-60.9.1/tests/meta/upload/conftest.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.983940 cg-60.9.1/tests/meta/upload/gisaid/__init__.py
--rw-r--r--   0        0        0     2557 2024-05-30 12:47:24.983940 cg-60.9.1/tests/meta/upload/gisaid/fixtures/four_samples.csv
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.983940 cg-60.9.1/tests/meta/upload/gisaid/fixtures/invalid_housekeeper.fasta
--rw-r--r--   0        0        0      211 2024-05-30 12:47:24.983940 cg-60.9.1/tests/meta/upload/gisaid/fixtures/valid_gisaid.fasta
--rw-r--r--   0        0        0      371 2024-05-30 12:47:24.983940 cg-60.9.1/tests/meta/upload/gisaid/fixtures/valid_housekeeper.fasta
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.983940 cg-60.9.1/tests/meta/upload/mutacc/__init__.py
--rw-r--r--   0        0        0     3684 2024-05-30 12:47:24.983940 cg-60.9.1/tests/meta/upload/mutacc/conftest.py
--rw-r--r--   0        0        0     4188 2024-05-30 12:47:24.983940 cg-60.9.1/tests/meta/upload/mutacc/test_meta_upload_mutacc.py
--rw-r--r--   0        0        0     1149 2024-05-30 12:47:24.983940 cg-60.9.1/tests/meta/upload/nipt/conftest.py
--rw-r--r--   0        0        0     1683 2024-05-30 12:47:24.983940 cg-60.9.1/tests/meta/upload/nipt/test_models.py
--rw-r--r--   0        0        0     1242 2024-05-30 12:47:24.983940 cg-60.9.1/tests/meta/upload/nipt/test_nipt_upload_api.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.983940 cg-60.9.1/tests/meta/upload/scout/__init__.py
--rw-r--r--   0        0        0    23954 2024-05-30 12:47:24.983940 cg-60.9.1/tests/meta/upload/scout/conftest.py
--rw-r--r--   0        0        0     4734 2024-05-30 12:47:24.983940 cg-60.9.1/tests/meta/upload/scout/test_generate_load_config.py
--rw-r--r--   0        0        0     4182 2024-05-30 12:47:24.983940 cg-60.9.1/tests/meta/upload/scout/test_meta_upload_scoutapi.py
--rw-r--r--   0        0        0    33260 2024-05-30 12:47:24.983940 cg-60.9.1/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py
--rw-r--r--   0        0        0     7372 2024-05-30 12:47:24.983940 cg-60.9.1/tests/meta/upload/scout/test_scout_config_builder.py
--rw-r--r--   0        0        0     2511 2024-05-30 12:47:24.983940 cg-60.9.1/tests/meta/upload/test_meta_upload_coverage.py
--rw-r--r--   0        0        0     1473 2024-05-30 12:47:24.983940 cg-60.9.1/tests/meta/upload/test_upload_api.py
--rw-r--r--   0        0        0     2547 2024-05-30 12:47:24.983940 cg-60.9.1/tests/meta/upload/test_upload_genotypes_api.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.983940 cg-60.9.1/tests/meta/workflow/__init__.py
--rw-r--r--   0        0        0    10262 2024-05-30 12:47:24.983940 cg-60.9.1/tests/meta/workflow/conftest.py
--rw-r--r--   0        0        0     3679 2024-05-30 12:47:24.983940 cg-60.9.1/tests/meta/workflow/microsalt/conftest.py
--rw-r--r--   0        0        0      318 2024-05-30 12:47:24.983940 cg-60.9.1/tests/meta/workflow/microsalt/test_parsing_metrics.py
--rw-r--r--   0        0        0     3759 2024-05-30 12:47:24.983940 cg-60.9.1/tests/meta/workflow/microsalt/test_quality_controller.py
--rw-r--r--   0        0        0    14367 2024-05-30 12:47:24.983940 cg-60.9.1/tests/meta/workflow/microsalt/test_quality_controller_utils.py
--rw-r--r--   0        0        0      825 2024-05-30 12:47:24.983940 cg-60.9.1/tests/meta/workflow/microsalt/test_report_generation.py
--rw-r--r--   0        0        0    20894 2024-05-30 12:47:24.983940 cg-60.9.1/tests/meta/workflow/test_analysis.py
--rw-r--r--   0        0        0     7934 2024-05-30 12:47:24.983940 cg-60.9.1/tests/meta/workflow/test_balsamic.py
--rw-r--r--   0        0        0     3034 2024-05-30 12:47:24.983940 cg-60.9.1/tests/meta/workflow/test_fastq.py
--rw-r--r--   0        0        0     1532 2024-05-30 12:47:24.983940 cg-60.9.1/tests/meta/workflow/test_microsalt.py
--rw-r--r--   0        0        0     2721 2024-05-30 12:47:24.983940 cg-60.9.1/tests/meta/workflow/test_nf_analysis.py
--rw-r--r--   0        0        0     7741 2024-05-30 12:47:24.983940 cg-60.9.1/tests/meta/workflow/test_prepare_fastq_api.py
--rw-r--r--   0        0        0     2095 2024-05-30 12:47:24.983940 cg-60.9.1/tests/meta/workflow/test_raredisease.py
--rw-r--r--   0        0        0     1674 2024-05-30 12:47:24.983940 cg-60.9.1/tests/meta/workflow/test_rnafusion.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.983940 cg-60.9.1/tests/mocks/__init__.py
--rw-r--r--   0        0        0     1168 2024-05-30 12:47:24.983940 cg-60.9.1/tests/mocks/balsamic_analysis_mock.py
--rw-r--r--   0        0        0     3500 2024-05-30 12:47:24.987940 cg-60.9.1/tests/mocks/crunchy.py
--rw-r--r--   0        0        0    21787 2024-05-30 12:47:24.987940 cg-60.9.1/tests/mocks/hk_mock.py
--rw-r--r--   0        0        0     4215 2024-05-30 12:47:24.987940 cg-60.9.1/tests/mocks/limsmock.py
--rw-r--r--   0        0        0      572 2024-05-30 12:47:24.987940 cg-60.9.1/tests/mocks/madeline.py
--rw-r--r--   0        0        0     1297 2024-05-30 12:47:24.987940 cg-60.9.1/tests/mocks/mip_analysis_mock.py
--rw-r--r--   0        0        0     1525 2024-05-30 12:47:24.987940 cg-60.9.1/tests/mocks/osticket.py
--rw-r--r--   0        0        0     3239 2024-05-30 12:47:24.987940 cg-60.9.1/tests/mocks/process_mock.py
--rw-r--r--   0        0        0     4713 2024-05-30 12:47:24.987940 cg-60.9.1/tests/mocks/report.py
--rw-r--r--   0        0        0     3915 2024-05-30 12:47:24.987940 cg-60.9.1/tests/mocks/scout.py
--rw-r--r--   0        0        0      750 2024-05-30 12:47:24.987940 cg-60.9.1/tests/mocks/store_model.py
--rw-r--r--   0        0        0     1620 2024-05-30 12:47:24.987940 cg-60.9.1/tests/mocks/tb_mock.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.987940 cg-60.9.1/tests/models/__init__.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.987940 cg-60.9.1/tests/models/balsamic/__init__.py
--rw-r--r--   0        0        0     1194 2024-05-30 12:47:24.987940 cg-60.9.1/tests/models/balsamic/conftest.py
--rw-r--r--   0        0        0     1030 2024-05-30 12:47:24.987940 cg-60.9.1/tests/models/balsamic/test_balsamic_analysis.py
--rw-r--r--   0        0        0     1050 2024-05-30 12:47:24.987940 cg-60.9.1/tests/models/conftest.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.987940 cg-60.9.1/tests/models/demultiplexing/__init__.py
--rw-r--r--   0        0        0    12651 2024-05-30 12:47:24.987940 cg-60.9.1/tests/models/demultiplexing/test_run_parameters.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.987940 cg-60.9.1/tests/models/downsample/__init__.py
--rw-r--r--   0        0        0     2096 2024-05-30 12:47:24.987940 cg-60.9.1/tests/models/downsample/test_down_sample_meta_data.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.987940 cg-60.9.1/tests/models/flow_cell/__init__.py
--rw-r--r--   0        0        0     7778 2024-05-30 12:47:24.987940 cg-60.9.1/tests/models/flow_cell/test_flowcell_model.py
--rw-r--r--   0        0        0     6637 2024-05-30 12:47:24.987940 cg-60.9.1/tests/models/mip/conftest.py
--rw-r--r--   0        0        0     1239 2024-05-30 12:47:24.987940 cg-60.9.1/tests/models/mip/test_mip_analysis.py
--rw-r--r--   0        0        0     2348 2024-05-30 12:47:24.987940 cg-60.9.1/tests/models/mip/test_mip_config.py
--rw-r--r--   0        0        0     6392 2024-05-30 12:47:24.987940 cg-60.9.1/tests/models/mip/test_mip_metrics_deliverables.py
--rw-r--r--   0        0        0     3959 2024-05-30 12:47:24.987940 cg-60.9.1/tests/models/mip/test_mip_sample_info.py
--rw-r--r--   0        0        0     3314 2024-05-30 12:47:24.987940 cg-60.9.1/tests/models/nextflow/test_nextflow_deliver.py
--rw-r--r--   0        0        0     2663 2024-05-30 12:47:24.987940 cg-60.9.1/tests/models/observations/test_observations_input_files.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.987940 cg-60.9.1/tests/models/report/__init__.py
--rw-r--r--   0        0        0     7879 2024-05-30 12:47:24.987940 cg-60.9.1/tests/models/report/test_validators.py
--rw-r--r--   0        0        0     3855 2024-05-30 12:47:24.987940 cg-60.9.1/tests/models/rnafusion/test_rnafusion_sample.py
--rw-r--r--   0        0        0     1374 2024-05-30 12:47:24.987940 cg-60.9.1/tests/models/test_cg_models.py
--rw-r--r--   0        0        0      990 2024-05-30 12:47:24.987940 cg-60.9.1/tests/models/test_compression_data.py
--rw-r--r--   0        0        0      729 2024-05-30 12:47:24.987940 cg-60.9.1/tests/models/test_fastq.py
--rw-r--r--   0        0        0     2860 2024-05-30 12:47:24.987940 cg-60.9.1/tests/models/test_file_data.py
--rw-r--r--   0        0        0     5094 2024-05-30 12:47:24.987940 cg-60.9.1/tests/server/conftest.py
--rw-r--r--   0        0        0     3135 2024-05-30 12:47:24.987940 cg-60.9.1/tests/server/endpoints/test_delivery_message_endpoint.py
--rw-r--r--   0        0        0     3239 2024-05-30 12:47:24.987940 cg-60.9.1/tests/server/endpoints/test_orders_endpoint.py
--rw-r--r--   0        0        0      271 2024-05-30 12:47:24.987940 cg-60.9.1/tests/server/test_server_auto.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.987940 cg-60.9.1/tests/services/__init__.py
--rw-r--r--   0        0        0     1092 2024-05-30 12:47:24.987940 cg-60.9.1/tests/services/fastq_file_service/conftest.py
--rw-r--r--   0        0        0     3712 2024-05-30 12:47:24.987940 cg-60.9.1/tests/services/fastq_file_service/test_fastq_file_service.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.987940 cg-60.9.1/tests/services/illumina_services/__init__.py
--rw-r--r--   0        0        0      738 2024-05-30 12:47:24.987940 cg-60.9.1/tests/services/illumina_services/illumina_demux_version_service/conftest.py
--rw-r--r--   0        0        0     1344 2024-05-30 12:47:24.987940 cg-60.9.1/tests/services/illumina_services/illumina_demux_version_service/test_illumina_demux_version_service.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.987940 cg-60.9.1/tests/services/illumina_services/illumina_metrics_service/__init__.py
--rw-r--r--   0        0        0     4020 2024-05-30 12:47:24.987940 cg-60.9.1/tests/services/illumina_services/illumina_metrics_service/conftest.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.987940 cg-60.9.1/tests/services/illumina_services/illumina_metrics_service/parsers/__init__.py
--rw-r--r--   0        0        0    10501 2024-05-30 12:47:24.987940 cg-60.9.1/tests/services/illumina_services/illumina_metrics_service/parsers/test_bclconvert_metrics_parser.py
--rw-r--r--   0        0        0     3262 2024-05-30 12:47:24.987940 cg-60.9.1/tests/services/illumina_services/illumina_metrics_service/parsers/test_illumina_metrics_service.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.987940 cg-60.9.1/tests/services/illumina_services/illumina_post_processing_service/__init__.py
--rw-r--r--   0        0        0     1431 2024-05-30 12:47:24.987940 cg-60.9.1/tests/services/illumina_services/illumina_post_processing_service/conftest.py
--rw-r--r--   0        0        0     4441 2024-05-30 12:47:24.987940 cg-60.9.1/tests/services/illumina_services/illumina_post_processing_service/test_illumina_post_processing_service.py
--rw-r--r--   0        0        0     4862 2024-05-30 12:47:24.987940 cg-60.9.1/tests/services/orders/order_status_service/conftest.py
--rw-r--r--   0        0        0     2876 2024-05-30 12:47:24.987940 cg-60.9.1/tests/services/orders/order_status_service/test_order_summary_service.py
--rw-r--r--   0        0        0      748 2024-05-30 12:47:24.987940 cg-60.9.1/tests/services/parse_completion_status_service/conftest.py
--rw-r--r--   0        0        0     1249 2024-05-30 12:47:24.987940 cg-60.9.1/tests/services/parse_completion_status_service/test_parse_completion_status_service.py
--rw-r--r--   0        0        0     9598 2024-05-30 12:47:24.987940 cg-60.9.1/tests/services/sequencing_qc_service/test_sequencing_quality_checks_utils.py
--rw-r--r--   0        0        0     3427 2024-05-30 12:47:24.987940 cg-60.9.1/tests/services/validate_file_transfer_service/conftest.py
--rw-r--r--   0        0        0     4258 2024-05-30 12:47:24.987940 cg-60.9.1/tests/services/validate_file_transfer_service/test_validate_file_transfer_service.py
--rw-r--r--   0        0        0     2952 2024-05-30 12:47:24.987940 cg-60.9.1/tests/services/validate_file_transfer_service/test_validate_pacbio_file_transfer_service.py
--rw-r--r--   0        0        0      318 2024-05-30 12:47:24.987940 cg-60.9.1/tests/small_helpers.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.987940 cg-60.9.1/tests/store/__init__.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.987940 cg-60.9.1/tests/store/api/__init__.py
--rw-r--r--   0        0        0     3032 2024-05-30 12:47:24.987940 cg-60.9.1/tests/store/api/conftest.py
--rw-r--r--   0        0        0     1557 2024-05-30 12:47:24.987940 cg-60.9.1/tests/store/api/test_base.py
--rw-r--r--   0        0        0    21033 2024-05-30 12:47:24.987940 cg-60.9.1/tests/store/conftest.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.987940 cg-60.9.1/tests/store/crud/__init__.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.987940 cg-60.9.1/tests/store/crud/add/__init__.py
--rw-r--r--   0        0        0     1497 2024-05-30 12:47:24.987940 cg-60.9.1/tests/store/crud/add/test_store_add_application_version.py
--rw-r--r--   0        0        0     5254 2024-05-30 12:47:24.987940 cg-60.9.1/tests/store/crud/add/test_store_add_base.py
--rw-r--r--   0        0        0     2502 2024-05-30 12:47:24.987940 cg-60.9.1/tests/store/crud/add/test_store_add_customer.py
--rw-r--r--   0        0        0     1704 2024-05-30 12:47:24.987940 cg-60.9.1/tests/store/crud/add/test_store_add_flow_celll.py
--rw-r--r--   0        0        0    12288 2024-05-30 12:47:24.991940 cg-60.9.1/tests/store/crud/conftest.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.991940 cg-60.9.1/tests/store/crud/delete/__init__.py
--rw-r--r--   0        0        0     5611 2024-05-30 12:47:24.991940 cg-60.9.1/tests/store/crud/delete/test_delete.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.991940 cg-60.9.1/tests/store/crud/read/__init__.py
--rw-r--r--   0        0        0    56073 2024-05-30 12:47:24.991940 cg-60.9.1/tests/store/crud/read/test_read.py
--rw-r--r--   0        0        0     5461 2024-05-30 12:47:24.991940 cg-60.9.1/tests/store/crud/read/test_read_analyses_to_clean.py
--rw-r--r--   0        0        0     3553 2024-05-30 12:47:24.991940 cg-60.9.1/tests/store/crud/read/test_read_analyses_to_delivery_report.py
--rw-r--r--   0        0        0    17328 2024-05-30 12:47:24.991940 cg-60.9.1/tests/store/crud/read/test_read_analysis.py
--rw-r--r--   0        0        0     2743 2024-05-30 12:47:24.991940 cg-60.9.1/tests/store/crud/read/test_read_application_version.py
--rw-r--r--   0        0        0     1105 2024-05-30 12:47:24.991940 cg-60.9.1/tests/store/crud/read/test_read_customer.py
--rw-r--r--   0        0        0      732 2024-05-30 12:47:24.991940 cg-60.9.1/tests/store/crud/read/test_read_illumina_flow_cell.py
--rw-r--r--   0        0        0     1530 2024-05-30 12:47:24.991940 cg-60.9.1/tests/store/crud/read/test_read_pool.py
--rw-r--r--   0        0        0    21503 2024-05-30 12:47:24.991940 cg-60.9.1/tests/store/crud/read/test_read_sample.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.991940 cg-60.9.1/tests/store/crud/update/__init__.py
--rw-r--r--   0        0        0      737 2024-05-30 12:47:24.991940 cg-60.9.1/tests/store/crud/update/test_update.py
--rw-r--r--   0        0        0    11693 2024-05-30 12:47:24.991940 cg-60.9.1/tests/store/filters/test_status_analyses_filters.py
--rw-r--r--   0        0        0     3397 2024-05-30 12:47:24.991940 cg-60.9.1/tests/store/filters/test_status_application_filters.py
--rw-r--r--   0        0        0     2073 2024-05-30 12:47:24.991940 cg-60.9.1/tests/store/filters/test_status_application_limitations_filters.py
--rw-r--r--   0        0        0    10452 2024-05-30 12:47:24.991940 cg-60.9.1/tests/store/filters/test_status_application_version_filters.py
--rw-r--r--   0        0        0     2804 2024-05-30 12:47:24.991940 cg-60.9.1/tests/store/filters/test_status_bed_filters.py
--rw-r--r--   0        0        0     2362 2024-05-30 12:47:24.991940 cg-60.9.1/tests/store/filters/test_status_bed_version_filters.py
--rw-r--r--   0        0        0     3495 2024-05-30 12:47:24.991940 cg-60.9.1/tests/store/filters/test_status_case_sample_filters.py
--rw-r--r--   0        0        0    39100 2024-05-30 12:47:24.991940 cg-60.9.1/tests/store/filters/test_status_cases_filters.py
--rw-r--r--   0        0        0     1345 2024-05-30 12:47:24.991940 cg-60.9.1/tests/store/filters/test_status_collaboration_filters.py
--rw-r--r--   0        0        0     2482 2024-05-30 12:47:24.991940 cg-60.9.1/tests/store/filters/test_status_customer_filters.py
--rw-r--r--   0        0        0     5153 2024-05-30 12:47:24.991940 cg-60.9.1/tests/store/filters/test_status_flow_cell_filters.py
--rw-r--r--   0        0        0     1095 2024-05-30 12:47:24.991940 cg-60.9.1/tests/store/filters/test_status_illumina_flow_cell_filters.py
--rw-r--r--   0        0        0     2226 2024-05-30 12:47:24.991940 cg-60.9.1/tests/store/filters/test_status_invoice_filters.py
--rw-r--r--   0        0        0     5871 2024-05-30 12:47:24.991940 cg-60.9.1/tests/store/filters/test_status_metrics_filters.py
--rw-r--r--   0        0        0     2404 2024-05-30 12:47:24.991940 cg-60.9.1/tests/store/filters/test_status_organism_filters.py
--rw-r--r--   0        0        0     1804 2024-05-30 12:47:24.991940 cg-60.9.1/tests/store/filters/test_status_panel_filters.py
--rw-r--r--   0        0        0     8720 2024-05-30 12:47:24.991940 cg-60.9.1/tests/store/filters/test_status_pool_filters.py
--rw-r--r--   0        0        0    22875 2024-05-30 12:47:24.991940 cg-60.9.1/tests/store/filters/test_status_samples_filters.py
--rw-r--r--   0        0        0     1576 2024-05-30 12:47:24.991940 cg-60.9.1/tests/store/filters/test_status_user_filters.py
--rw-r--r--   0        0        0     2147 2024-05-30 12:47:24.991940 cg-60.9.1/tests/store/test_delivery.py
--rw-r--r--   0        0        0     4127 2024-05-30 12:47:24.991940 cg-60.9.1/tests/store/test_store_models.py
--rw-r--r--   0        0        0    37125 2024-05-30 12:47:24.991940 cg-60.9.1/tests/store_helpers.py
--rw-r--r--   0        0        0     4988 2024-05-30 12:47:24.991940 cg-60.9.1/tests/test_copy_novaseqx_flow_cell.py
--rw-r--r--   0        0        0      911 2024-05-30 12:47:24.991940 cg-60.9.1/tests/test_store_helpers.py
--rw-r--r--   0        0        0        0 2024-05-30 12:47:24.991940 cg-60.9.1/tests/utils/__init__.py
--rw-r--r--   0        0        0     1749 2024-05-30 12:47:24.991940 cg-60.9.1/tests/utils/conftest.py
--rw-r--r--   0        0        0      371 2024-05-30 12:47:24.991940 cg-60.9.1/tests/utils/test_calculations.py
--rw-r--r--   0        0        0     1906 2024-05-30 12:47:24.991940 cg-60.9.1/tests/utils/test_checksum.py
--rw-r--r--   0        0        0     2920 2024-05-30 12:47:24.991940 cg-60.9.1/tests/utils/test_commands.py
--rw-r--r--   0        0        0      953 2024-05-30 12:47:24.991940 cg-60.9.1/tests/utils/test_date.py
--rw-r--r--   0        0        0     1508 2024-05-30 12:47:24.991940 cg-60.9.1/tests/utils/test_dict.py
--rw-r--r--   0        0        0     7154 2024-05-30 12:47:24.991940 cg-60.9.1/tests/utils/test_dispatcher.py
--rw-r--r--   0        0        0     5204 2024-05-30 12:47:24.991940 cg-60.9.1/tests/utils/test_files.py
--rw-r--r--   0        0        0     2052 2024-05-30 12:47:24.991940 cg-60.9.1/tests/utils/test_time.py
--rw-r--r--   0        0        0     2752 2024-05-30 12:47:24.991940 cg-60.9.1/tests/utils/test_utils.py
--rw-r--r--   0        0        0     4369 1970-01-01 00:00:00.000000 cg-60.9.1/PKG-INFO
+-rw-r--r--   0        0        0     2686 2024-06-03 12:38:31.266665 cg-60.9.3/README.md
+-rw-r--r--   0        0        0       40 2024-06-03 12:38:31.270666 cg-60.9.3/cg/__init__.py
+-rw-r--r--   0        0        0      315 2024-06-03 12:38:31.270666 cg-60.9.3/cg/apps/__init__.py
+-rw-r--r--   0        0        0       27 2024-06-03 12:38:31.270666 cg-60.9.3/cg/apps/coverage/__init__.py
+-rw-r--r--   0        0        0     2940 2024-06-03 12:38:31.270666 cg-60.9.3/cg/apps/coverage/api.py
+-rw-r--r--   0        0        0       56 2024-06-03 12:38:31.270666 cg-60.9.3/cg/apps/crunchy/__init__.py
+-rw-r--r--   0        0        0    12783 2024-06-03 12:38:31.270666 cg-60.9.3/cg/apps/crunchy/crunchy.py
+-rw-r--r--   0        0        0     4502 2024-06-03 12:38:31.270666 cg-60.9.3/cg/apps/crunchy/files.py
+-rw-r--r--   0        0        0      430 2024-06-03 12:38:31.270666 cg-60.9.3/cg/apps/crunchy/models.py
+-rw-r--r--   0        0        0      910 2024-06-03 12:38:31.270666 cg-60.9.3/cg/apps/crunchy/sbatch.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.270666 cg-60.9.3/cg/apps/demultiplex/__init__.py
+-rw-r--r--   0        0        0    11369 2024-06-03 12:38:31.270666 cg-60.9.3/cg/apps/demultiplex/demultiplex_api.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.270666 cg-60.9.3/cg/apps/demultiplex/sample_sheet/__init__.py
+-rw-r--r--   0        0        0    11277 2024-06-03 12:38:31.270666 cg-60.9.3/cg/apps/demultiplex/sample_sheet/api.py
+-rw-r--r--   0        0        0     2183 2024-06-03 12:38:31.270666 cg-60.9.3/cg/apps/demultiplex/sample_sheet/index.py
+-rw-r--r--   0        0        0     7341 2024-06-03 12:38:31.270666 cg-60.9.3/cg/apps/demultiplex/sample_sheet/override_cycles_validator.py
+-rw-r--r--   0        0        0     3188 2024-06-03 12:38:31.270666 cg-60.9.3/cg/apps/demultiplex/sample_sheet/read_sample_sheet.py
+-rw-r--r--   0        0        0     7071 2024-06-03 12:38:31.270666 cg-60.9.3/cg/apps/demultiplex/sample_sheet/sample_models.py
+-rw-r--r--   0        0        0     6105 2024-06-03 12:38:31.270666 cg-60.9.3/cg/apps/demultiplex/sample_sheet/sample_sheet_creator.py
+-rw-r--r--   0        0        0     1372 2024-06-03 12:38:31.270666 cg-60.9.3/cg/apps/demultiplex/sample_sheet/sample_sheet_models.py
+-rw-r--r--   0        0        0     8092 2024-06-03 12:38:31.270666 cg-60.9.3/cg/apps/demultiplex/sample_sheet/sample_sheet_validator.py
+-rw-r--r--   0        0        0      824 2024-06-03 12:38:31.270666 cg-60.9.3/cg/apps/demultiplex/sample_sheet/validators.py
+-rw-r--r--   0        0        0      677 2024-06-03 12:38:31.270666 cg-60.9.3/cg/apps/demultiplex/sbatch.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.270666 cg-60.9.3/cg/apps/downsample/__init__.py
+-rw-r--r--   0        0        0     6340 2024-06-03 12:38:31.270666 cg-60.9.3/cg/apps/downsample/downsample.py
+-rw-r--r--   0        0        0     2125 2024-06-03 12:38:31.270666 cg-60.9.3/cg/apps/downsample/utils.py
+-rw-r--r--   0        0        0      298 2024-06-03 12:38:31.270666 cg-60.9.3/cg/apps/environ.py
+-rw-r--r--   0        0        0     1741 2024-06-03 12:38:31.270666 cg-60.9.3/cg/apps/gens.py
+-rw-r--r--   0        0        0     3419 2024-06-03 12:38:31.270666 cg-60.9.3/cg/apps/gt.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.270666 cg-60.9.3/cg/apps/hermes/__init__.py
+-rw-r--r--   0        0        0     2249 2024-06-03 12:38:31.270666 cg-60.9.3/cg/apps/hermes/hermes_api.py
+-rw-r--r--   0        0        0     1298 2024-06-03 12:38:31.270666 cg-60.9.3/cg/apps/hermes/models.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.270666 cg-60.9.3/cg/apps/housekeeper/__init__.py
+-rw-r--r--   0        0        0    30395 2024-06-03 12:38:31.270666 cg-60.9.3/cg/apps/housekeeper/hk.py
+-rw-r--r--   0        0        0      326 2024-06-03 12:38:31.270666 cg-60.9.3/cg/apps/housekeeper/models.py
+-rw-r--r--   0        0        0       32 2024-06-03 12:38:31.270666 cg-60.9.3/cg/apps/invoice/__init__.py
+-rw-r--r--   0        0        0     4804 2024-06-03 12:38:31.270666 cg-60.9.3/cg/apps/invoice/render.py
+-rw-r--r--   0        0        0   113467 2024-06-03 12:38:31.270666 cg-60.9.3/cg/apps/invoice/templates/KI_pool_invoice.xlsx
+-rw-r--r--   0        0        0    75562 2024-06-03 12:38:31.274665 cg-60.9.3/cg/apps/invoice/templates/KI_sample_invoice.xlsx
+-rw-r--r--   0        0        0   113512 2024-06-03 12:38:31.274665 cg-60.9.3/cg/apps/invoice/templates/KTH_pool_invoice.xlsx
+-rw-r--r--   0        0        0    75459 2024-06-03 12:38:31.274665 cg-60.9.3/cg/apps/invoice/templates/KTH_sample_invoice.xlsx
+-rw-r--r--   0        0        0       25 2024-06-03 12:38:31.274665 cg-60.9.3/cg/apps/lims/__init__.py
+-rw-r--r--   0        0        0    18873 2024-06-03 12:38:31.274665 cg-60.9.3/cg/apps/lims/api.py
+-rw-r--r--   0        0        0     2652 2024-06-03 12:38:31.274665 cg-60.9.3/cg/apps/lims/batch.py
+-rw-r--r--   0        0        0     8129 2024-06-03 12:38:31.274665 cg-60.9.3/cg/apps/lims/order.py
+-rw-r--r--   0        0        0     3118 2024-06-03 12:38:31.274665 cg-60.9.3/cg/apps/lims/sample_sheet.py
+-rw-r--r--   0        0        0     4866 2024-06-03 12:38:31.274665 cg-60.9.3/cg/apps/loqus.py
+-rw-r--r--   0        0        0       35 2024-06-03 12:38:31.274665 cg-60.9.3/cg/apps/madeline/__init__.py
+-rw-r--r--   0        0        0     3213 2024-06-03 12:38:31.274665 cg-60.9.3/cg/apps/madeline/api.py
+-rw-r--r--   0        0        0       23 2024-06-03 12:38:31.274665 cg-60.9.3/cg/apps/mip/__init__.py
+-rw-r--r--   0        0        0     3564 2024-06-03 12:38:31.274665 cg-60.9.3/cg/apps/mip/confighandler.py
+-rw-r--r--   0        0        0     2207 2024-06-03 12:38:31.274665 cg-60.9.3/cg/apps/mutacc_auto.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.274665 cg-60.9.3/cg/apps/orderform/__init__.py
+-rw-r--r--   0        0        0     9498 2024-06-03 12:38:31.274665 cg-60.9.3/cg/apps/orderform/excel_orderform_parser.py
+-rw-r--r--   0        0        0     3051 2024-06-03 12:38:31.274665 cg-60.9.3/cg/apps/orderform/json_orderform_parser.py
+-rw-r--r--   0        0        0     6419 2024-06-03 12:38:31.274665 cg-60.9.3/cg/apps/orderform/orderform_parser.py
+-rw-r--r--   0        0        0      252 2024-06-03 12:38:31.274665 cg-60.9.3/cg/apps/orderform/utils.py
+-rw-r--r--   0        0        0     2537 2024-06-03 12:38:31.274665 cg-60.9.3/cg/apps/osticket.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.274665 cg-60.9.3/cg/apps/scout/__init__.py
+-rw-r--r--   0        0        0     3177 2024-06-03 12:38:31.274665 cg-60.9.3/cg/apps/scout/scout_export.py
+-rw-r--r--   0        0        0    11108 2024-06-03 12:38:31.274665 cg-60.9.3/cg/apps/scout/scoutapi.py
+-rw-r--r--   0        0        0      444 2024-06-03 12:38:31.274665 cg-60.9.3/cg/apps/scout/validators.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.274665 cg-60.9.3/cg/apps/slurm/__init__.py
+-rw-r--r--   0        0        0     1277 2024-06-03 12:38:31.274665 cg-60.9.3/cg/apps/slurm/sbatch.py
+-rw-r--r--   0        0        0     3559 2024-06-03 12:38:31.274665 cg-60.9.3/cg/apps/slurm/slurm_api.py
+-rw-r--r--   0        0        0       32 2024-06-03 12:38:31.274665 cg-60.9.3/cg/apps/tb/__init__.py
+-rw-r--r--   0        0        0     8025 2024-06-03 12:38:31.274665 cg-60.9.3/cg/apps/tb/api.py
+-rw-r--r--   0        0        0      152 2024-06-03 12:38:31.274665 cg-60.9.3/cg/apps/tb/dto/create_job_request.py
+-rw-r--r--   0        0        0      250 2024-06-03 12:38:31.274665 cg-60.9.3/cg/apps/tb/dto/summary_response.py
+-rw-r--r--   0        0        0     1305 2024-06-03 12:38:31.274665 cg-60.9.3/cg/apps/tb/models.py
+-rw-r--r--   0        0        0      305 2024-06-03 12:38:31.274665 cg-60.9.3/cg/apps/tb/validators.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.274665 cg-60.9.3/cg/cli/__init__.py
+-rw-r--r--   0        0        0    11714 2024-06-03 12:38:31.274665 cg-60.9.3/cg/cli/add.py
+-rw-r--r--   0        0        0     4308 2024-06-03 12:38:31.274665 cg-60.9.3/cg/cli/archive.py
+-rw-r--r--   0        0        0    10172 2024-06-03 12:38:31.274665 cg-60.9.3/cg/cli/backup.py
+-rw-r--r--   0        0        0     3916 2024-06-03 12:38:31.274665 cg-60.9.3/cg/cli/base.py
+-rw-r--r--   0        0        0    10506 2024-06-03 12:38:31.274665 cg-60.9.3/cg/cli/clean.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.274665 cg-60.9.3/cg/cli/compress/__init__.py
+-rw-r--r--   0        0        0     2135 2024-06-03 12:38:31.274665 cg-60.9.3/cg/cli/compress/base.py
+-rw-r--r--   0        0        0     6706 2024-06-03 12:38:31.274665 cg-60.9.3/cg/cli/compress/fastq.py
+-rw-r--r--   0        0        0     8163 2024-06-03 12:38:31.274665 cg-60.9.3/cg/cli/compress/helpers.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.274665 cg-60.9.3/cg/cli/delete/__init__.py
+-rw-r--r--   0        0        0      564 2024-06-03 12:38:31.274665 cg-60.9.3/cg/cli/delete/base.py
+-rw-r--r--   0        0        0     4603 2024-06-03 12:38:31.274665 cg-60.9.3/cg/cli/delete/case.py
+-rw-r--r--   0        0        0     1896 2024-06-03 12:38:31.274665 cg-60.9.3/cg/cli/delete/cases.py
+-rw-r--r--   0        0        0     2470 2024-06-03 12:38:31.274665 cg-60.9.3/cg/cli/delete/observations.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.274665 cg-60.9.3/cg/cli/deliver/__init__.py
+-rw-r--r--   0        0        0     6068 2024-06-03 12:38:31.274665 cg-60.9.3/cg/cli/deliver/base.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.274665 cg-60.9.3/cg/cli/demultiplex/__init__.py
+-rw-r--r--   0        0        0      829 2024-06-03 12:38:31.274665 cg-60.9.3/cg/cli/demultiplex/base.py
+-rw-r--r--   0        0        0     4905 2024-06-03 12:38:31.274665 cg-60.9.3/cg/cli/demultiplex/copy_novaseqx_demultiplex_data.py
+-rw-r--r--   0        0        0     7751 2024-06-03 12:38:31.274665 cg-60.9.3/cg/cli/demultiplex/demux.py
+-rw-r--r--   0        0        0     1473 2024-06-03 12:38:31.274665 cg-60.9.3/cg/cli/demultiplex/finish.py
+-rw-r--r--   0        0        0     3119 2024-06-03 12:38:31.274665 cg-60.9.3/cg/cli/demultiplex/sample_sheet.py
+-rw-r--r--   0        0        0     3316 2024-06-03 12:38:31.274665 cg-60.9.3/cg/cli/downsample.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.274665 cg-60.9.3/cg/cli/generate/__init__.py
+-rw-r--r--   0        0        0      356 2024-06-03 12:38:31.274665 cg-60.9.3/cg/cli/generate/base.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.274665 cg-60.9.3/cg/cli/generate/report/__init__.py
+-rw-r--r--   0        0        0     4645 2024-06-03 12:38:31.274665 cg-60.9.3/cg/cli/generate/report/base.py
+-rw-r--r--   0        0        0      685 2024-06-03 12:38:31.274665 cg-60.9.3/cg/cli/generate/report/options.py
+-rw-r--r--   0        0        0     5615 2024-06-03 12:38:31.274665 cg-60.9.3/cg/cli/generate/report/utils.py
+-rw-r--r--   0        0        0     8327 2024-06-03 12:38:31.274665 cg-60.9.3/cg/cli/get.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.274665 cg-60.9.3/cg/cli/set/__init__.py
+-rw-r--r--   0        0        0     9856 2024-06-03 12:38:31.274665 cg-60.9.3/cg/cli/set/base.py
+-rw-r--r--   0        0        0     4384 2024-06-03 12:38:31.274665 cg-60.9.3/cg/cli/set/case.py
+-rw-r--r--   0        0        0     2595 2024-06-03 12:38:31.274665 cg-60.9.3/cg/cli/set/cases.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.274665 cg-60.9.3/cg/cli/store/__init__.py
+-rw-r--r--   0        0        0     1093 2024-06-03 12:38:31.274665 cg-60.9.3/cg/cli/store/base.py
+-rw-r--r--   0        0        0     6191 2024-06-03 12:38:31.278665 cg-60.9.3/cg/cli/store/store.py
+-rw-r--r--   0        0        0     1761 2024-06-03 12:38:31.278665 cg-60.9.3/cg/cli/transfer.py
+-rw-r--r--   0        0        0        1 2024-06-03 12:38:31.278665 cg-60.9.3/cg/cli/upload/__init__.py
+-rw-r--r--   0        0        0     5706 2024-06-03 12:38:31.278665 cg-60.9.3/cg/cli/upload/base.py
+-rw-r--r--   0        0        0     5548 2024-06-03 12:38:31.278665 cg-60.9.3/cg/cli/upload/clinical_delivery.py
+-rw-r--r--   0        0        0     1175 2024-06-03 12:38:31.278665 cg-60.9.3/cg/cli/upload/coverage.py
+-rw-r--r--   0        0        0     1465 2024-06-03 12:38:31.278665 cg-60.9.3/cg/cli/upload/delivery_report.py
+-rw-r--r--   0        0        0     3910 2024-06-03 12:38:31.278665 cg-60.9.3/cg/cli/upload/fohm.py
+-rw-r--r--   0        0        0     1463 2024-06-03 12:38:31.278665 cg-60.9.3/cg/cli/upload/genotype.py
+-rw-r--r--   0        0        0     1913 2024-06-03 12:38:31.278665 cg-60.9.3/cg/cli/upload/gens.py
+-rw-r--r--   0        0        0      584 2024-06-03 12:38:31.278665 cg-60.9.3/cg/cli/upload/gisaid.py
+-rw-r--r--   0        0        0     2615 2024-06-03 12:38:31.278665 cg-60.9.3/cg/cli/upload/mutacc.py
+-rw-r--r--   0        0        0       23 2024-06-03 12:38:31.278665 cg-60.9.3/cg/cli/upload/nipt/__init__.py
+-rw-r--r--   0        0        0     2985 2024-06-03 12:38:31.278665 cg-60.9.3/cg/cli/upload/nipt/base.py
+-rw-r--r--   0        0        0     2254 2024-06-03 12:38:31.278665 cg-60.9.3/cg/cli/upload/nipt/ftp.py
+-rw-r--r--   0        0        0     1607 2024-06-03 12:38:31.278665 cg-60.9.3/cg/cli/upload/nipt/statina.py
+-rw-r--r--   0        0        0      112 2024-06-03 12:38:31.278665 cg-60.9.3/cg/cli/upload/observations/__init__.py
+-rw-r--r--   0        0        0     2563 2024-06-03 12:38:31.278665 cg-60.9.3/cg/cli/upload/observations/observations.py
+-rw-r--r--   0        0        0     1968 2024-06-03 12:38:31.278665 cg-60.9.3/cg/cli/upload/observations/utils.py
+-rw-r--r--   0        0        0     9970 2024-06-03 12:38:31.278665 cg-60.9.3/cg/cli/upload/scout.py
+-rw-r--r--   0        0        0      650 2024-06-03 12:38:31.278665 cg-60.9.3/cg/cli/upload/utils.py
+-rw-r--r--   0        0        0     1667 2024-06-03 12:38:31.278665 cg-60.9.3/cg/cli/upload/validate.py
+-rw-r--r--   0        0        0      363 2024-06-03 12:38:31.278665 cg-60.9.3/cg/cli/utils.py
+-rw-r--r--   0        0        0      599 2024-06-03 12:38:31.278665 cg-60.9.3/cg/cli/validate.py
+-rw-r--r--   0        0        0       18 2024-06-03 12:38:31.278665 cg-60.9.3/cg/cli/workflow/__init__.py
+-rw-r--r--   0        0        0       22 2024-06-03 12:38:31.278665 cg-60.9.3/cg/cli/workflow/balsamic/__init__.py
+-rw-r--r--   0        0        0     8925 2024-06-03 12:38:31.278665 cg-60.9.3/cg/cli/workflow/balsamic/base.py
+-rw-r--r--   0        0        0     1980 2024-06-03 12:38:31.278665 cg-60.9.3/cg/cli/workflow/balsamic/options.py
+-rw-r--r--   0        0        0      881 2024-06-03 12:38:31.278665 cg-60.9.3/cg/cli/workflow/balsamic/pon.py
+-rw-r--r--   0        0        0     1162 2024-06-03 12:38:31.278665 cg-60.9.3/cg/cli/workflow/balsamic/qc.py
+-rw-r--r--   0        0        0     1177 2024-06-03 12:38:31.278665 cg-60.9.3/cg/cli/workflow/balsamic/umi.py
+-rw-r--r--   0        0        0     1342 2024-06-03 12:38:31.278665 cg-60.9.3/cg/cli/workflow/base.py
+-rw-r--r--   0        0        0    12264 2024-06-03 12:38:31.278665 cg-60.9.3/cg/cli/workflow/commands.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.278665 cg-60.9.3/cg/cli/workflow/fastq/__init__.py
+-rw-r--r--   0        0        0     1483 2024-06-03 12:38:31.278665 cg-60.9.3/cg/cli/workflow/fastq/base.py
+-rw-r--r--   0        0        0     1787 2024-06-03 12:38:31.278665 cg-60.9.3/cg/cli/workflow/fastq/fastq_service.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.278665 cg-60.9.3/cg/cli/workflow/fluffy/__init__.py
+-rw-r--r--   0        0        0     4081 2024-06-03 12:38:31.278665 cg-60.9.3/cg/cli/workflow/fluffy/base.py
+-rw-r--r--   0        0        0       22 2024-06-03 12:38:31.278665 cg-60.9.3/cg/cli/workflow/jasen/__init__.py
+-rw-r--r--   0        0        0      535 2024-06-03 12:38:31.278665 cg-60.9.3/cg/cli/workflow/jasen/base.py
+-rw-r--r--   0        0        0       22 2024-06-03 12:38:31.278665 cg-60.9.3/cg/cli/workflow/microsalt/__init__.py
+-rw-r--r--   0        0        0     7651 2024-06-03 12:38:31.278665 cg-60.9.3/cg/cli/workflow/microsalt/base.py
+-rw-r--r--   0        0        0       22 2024-06-03 12:38:31.278665 cg-60.9.3/cg/cli/workflow/mip/__init__.py
+-rw-r--r--   0        0        0     6605 2024-06-03 12:38:31.278665 cg-60.9.3/cg/cli/workflow/mip/base.py
+-rw-r--r--   0        0        0     1125 2024-06-03 12:38:31.278665 cg-60.9.3/cg/cli/workflow/mip/options.py
+-rw-r--r--   0        0        0       22 2024-06-03 12:38:31.278665 cg-60.9.3/cg/cli/workflow/mip_dna/__init__.py
+-rw-r--r--   0        0        0     1013 2024-06-03 12:38:31.278665 cg-60.9.3/cg/cli/workflow/mip_dna/base.py
+-rw-r--r--   0        0        0       22 2024-06-03 12:38:31.278665 cg-60.9.3/cg/cli/workflow/mip_rna/__init__.py
+-rw-r--r--   0        0        0      916 2024-06-03 12:38:31.278665 cg-60.9.3/cg/cli/workflow/mip_rna/base.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.278665 cg-60.9.3/cg/cli/workflow/mutant/__init__.py
+-rw-r--r--   0        0        0     3428 2024-06-03 12:38:31.278665 cg-60.9.3/cg/cli/workflow/mutant/base.py
+-rw-r--r--   0        0        0     8980 2024-06-03 12:38:31.278665 cg-60.9.3/cg/cli/workflow/nf_analysis.py
+-rw-r--r--   0        0        0       22 2024-06-03 12:38:31.278665 cg-60.9.3/cg/cli/workflow/raredisease/__init__.py
+-rw-r--r--   0        0        0     2201 2024-06-03 12:38:31.278665 cg-60.9.3/cg/cli/workflow/raredisease/base.py
+-rw-r--r--   0        0        0       22 2024-06-03 12:38:31.278665 cg-60.9.3/cg/cli/workflow/rnafusion/__init__.py
+-rw-r--r--   0        0        0     1179 2024-06-03 12:38:31.278665 cg-60.9.3/cg/cli/workflow/rnafusion/base.py
+-rw-r--r--   0        0        0       22 2024-06-03 12:38:31.278665 cg-60.9.3/cg/cli/workflow/taxprofiler/__init__.py
+-rw-r--r--   0        0        0     1211 2024-06-03 12:38:31.278665 cg-60.9.3/cg/cli/workflow/taxprofiler/base.py
+-rw-r--r--   0        0        0     1111 2024-06-03 12:38:31.278665 cg-60.9.3/cg/cli/workflow/tomte/base.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.278665 cg-60.9.3/cg/clients/__init__.py
+-rw-r--r--   0        0        0     1363 2024-06-03 12:38:31.278665 cg-60.9.3/cg/clients/arnold/api.py
+-rw-r--r--   0        0        0      160 2024-06-03 12:38:31.278665 cg-60.9.3/cg/clients/arnold/dto/create_case_request.py
+-rw-r--r--   0        0        0      384 2024-06-03 12:38:31.278665 cg-60.9.3/cg/clients/arnold/exceptions.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.278665 cg-60.9.3/cg/clients/janus/__init__.py
+-rw-r--r--   0        0        0     1246 2024-06-03 12:38:31.278665 cg-60.9.3/cg/clients/janus/api.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.278665 cg-60.9.3/cg/clients/janus/dto/__init__.py
+-rw-r--r--   0        0        0      503 2024-06-03 12:38:31.278665 cg-60.9.3/cg/clients/janus/dto/create_qc_metrics_request.py
+-rw-r--r--   0        0        0      420 2024-06-03 12:38:31.278665 cg-60.9.3/cg/clients/janus/exceptions.py
+-rw-r--r--   0        0        0      937 2024-06-03 12:38:31.278665 cg-60.9.3/cg/constants/__init__.py
+-rw-r--r--   0        0        0      253 2024-06-03 12:38:31.278665 cg-60.9.3/cg/constants/archiving.py
+-rw-r--r--   0        0        0       35 2024-06-03 12:38:31.278665 cg-60.9.3/cg/constants/backup.py
+-rw-r--r--   0        0        0      769 2024-06-03 12:38:31.278665 cg-60.9.3/cg/constants/bcl_convert_metrics.py
+-rw-r--r--   0        0        0      469 2024-06-03 12:38:31.278665 cg-60.9.3/cg/constants/compression.py
+-rw-r--r--   0        0        0     7086 2024-06-03 12:38:31.278665 cg-60.9.3/cg/constants/constants.py
+-rw-r--r--   0        0        0     6055 2024-06-03 12:38:31.278665 cg-60.9.3/cg/constants/delivery.py
+-rw-r--r--   0        0        0     7690 2024-06-03 12:38:31.278665 cg-60.9.3/cg/constants/demultiplexing.py
+-rw-r--r--   0        0        0      176 2024-06-03 12:38:31.278665 cg-60.9.3/cg/constants/devices.py
+-rw-r--r--   0        0        0     1422 2024-06-03 12:38:31.278665 cg-60.9.3/cg/constants/encryption.py
+-rw-r--r--   0        0        0      372 2024-06-03 12:38:31.278665 cg-60.9.3/cg/constants/extraction.py
+-rw-r--r--   0        0        0      134 2024-06-03 12:38:31.278665 cg-60.9.3/cg/constants/file_transfer_service.py
+-rw-r--r--   0        0        0     2137 2024-06-03 12:38:31.278665 cg-60.9.3/cg/constants/gene_panel.py
+-rw-r--r--   0        0        0     6747 2024-06-03 12:38:31.278665 cg-60.9.3/cg/constants/housekeeper_tags.py
+-rw-r--r--   0        0        0       95 2024-06-03 12:38:31.278665 cg-60.9.3/cg/constants/invoice.py
+-rw-r--r--   0        0        0     5815 2024-06-03 12:38:31.278665 cg-60.9.3/cg/constants/lims.py
+-rw-r--r--   0        0        0      847 2024-06-03 12:38:31.278665 cg-60.9.3/cg/constants/metrics.py
+-rw-r--r--   0        0        0      231 2024-06-03 12:38:31.278665 cg-60.9.3/cg/constants/nanopore_files.py
+-rw-r--r--   0        0        0      650 2024-06-03 12:38:31.278665 cg-60.9.3/cg/constants/nextflow.py
+-rw-r--r--   0        0        0     1595 2024-06-03 12:38:31.278665 cg-60.9.3/cg/constants/nf_analysis.py
+-rw-r--r--   0        0        0       19 2024-06-03 12:38:31.282665 cg-60.9.3/cg/constants/nipt.py
+-rw-r--r--   0        0        0     2178 2024-06-03 12:38:31.282665 cg-60.9.3/cg/constants/observations.py
+-rw-r--r--   0        0        0     1216 2024-06-03 12:38:31.282665 cg-60.9.3/cg/constants/orderforms.py
+-rw-r--r--   0        0        0       96 2024-06-03 12:38:31.282665 cg-60.9.3/cg/constants/paths.py
+-rw-r--r--   0        0        0      266 2024-06-03 12:38:31.282665 cg-60.9.3/cg/constants/pdc.py
+-rw-r--r--   0        0        0      160 2024-06-03 12:38:31.282665 cg-60.9.3/cg/constants/pedigree.py
+-rw-r--r--   0        0        0     1044 2024-06-03 12:38:31.282665 cg-60.9.3/cg/constants/priority.py
+-rw-r--r--   0        0        0       79 2024-06-03 12:38:31.282665 cg-60.9.3/cg/constants/process.py
+-rw-r--r--   0        0        0     5885 2024-06-03 12:38:31.282665 cg-60.9.3/cg/constants/report.py
+-rw-r--r--   0        0        0     1118 2024-06-03 12:38:31.282665 cg-60.9.3/cg/constants/sample_sources.py
+-rw-r--r--   0        0        0     3111 2024-06-03 12:38:31.282665 cg-60.9.3/cg/constants/scout.py
+-rw-r--r--   0        0        0     1669 2024-06-03 12:38:31.282665 cg-60.9.3/cg/constants/sequencing.py
+-rw-r--r--   0        0        0      313 2024-06-03 12:38:31.282665 cg-60.9.3/cg/constants/slurm.py
+-rw-r--r--   0        0        0      529 2024-06-03 12:38:31.282665 cg-60.9.3/cg/constants/subject.py
+-rw-r--r--   0        0        0       55 2024-06-03 12:38:31.282665 cg-60.9.3/cg/constants/symbols.py
+-rw-r--r--   0        0        0      435 2024-06-03 12:38:31.282665 cg-60.9.3/cg/constants/tb.py
+-rw-r--r--   0        0        0      161 2024-06-03 12:38:31.282665 cg-60.9.3/cg/constants/time.py
+-rw-r--r--   0        0        0     6639 2024-06-03 12:38:31.282665 cg-60.9.3/cg/exc.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.282665 cg-60.9.3/cg/io/__init__.py
+-rw-r--r--   0        0        0     1037 2024-06-03 12:38:31.282665 cg-60.9.3/cg/io/api.py
+-rw-r--r--   0        0        0      621 2024-06-03 12:38:31.282665 cg-60.9.3/cg/io/config.py
+-rw-r--r--   0        0        0     2978 2024-06-03 12:38:31.282665 cg-60.9.3/cg/io/controller.py
+-rw-r--r--   0        0        0     1763 2024-06-03 12:38:31.282665 cg-60.9.3/cg/io/csv.py
+-rw-r--r--   0        0        0      210 2024-06-03 12:38:31.282665 cg-60.9.3/cg/io/gzip.py
+-rw-r--r--   0        0        0      662 2024-06-03 12:38:31.282665 cg-60.9.3/cg/io/json.py
+-rw-r--r--   0        0        0      525 2024-06-03 12:38:31.282665 cg-60.9.3/cg/io/png.py
+-rw-r--r--   0        0        0     1094 2024-06-03 12:38:31.282665 cg-60.9.3/cg/io/txt.py
+-rw-r--r--   0        0        0      552 2024-06-03 12:38:31.282665 cg-60.9.3/cg/io/validate_path.py
+-rw-r--r--   0        0        0     1289 2024-06-03 12:38:31.282665 cg-60.9.3/cg/io/xml.py
+-rw-r--r--   0        0        0     1153 2024-06-03 12:38:31.282665 cg-60.9.3/cg/io/yaml.py
+-rw-r--r--   0        0        0      281 2024-06-03 12:38:31.282665 cg-60.9.3/cg/meta/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.282665 cg-60.9.3/cg/meta/archive/__init__.py
+-rw-r--r--   0        0        0    16317 2024-06-03 12:38:31.282665 cg-60.9.3/cg/meta/archive/archive.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.282665 cg-60.9.3/cg/meta/archive/ddn/__init__.py
+-rw-r--r--   0        0        0     1727 2024-06-03 12:38:31.282665 cg-60.9.3/cg/meta/archive/ddn/constants.py
+-rw-r--r--   0        0        0    10852 2024-06-03 12:38:31.282665 cg-60.9.3/cg/meta/archive/ddn/ddn_data_flow_client.py
+-rw-r--r--   0        0        0     3704 2024-06-03 12:38:31.282665 cg-60.9.3/cg/meta/archive/ddn/models.py
+-rw-r--r--   0        0        0     1250 2024-06-03 12:38:31.282665 cg-60.9.3/cg/meta/archive/ddn/utils.py
+-rw-r--r--   0        0        0     2024 2024-06-03 12:38:31.282665 cg-60.9.3/cg/meta/archive/models.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.282665 cg-60.9.3/cg/meta/backup/__init__.py
+-rw-r--r--   0        0        0    17426 2024-06-03 12:38:31.282665 cg-60.9.3/cg/meta/backup/backup.py
+-rw-r--r--   0        0        0     5397 2024-06-03 12:38:31.282665 cg-60.9.3/cg/meta/backup/pdc.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.282665 cg-60.9.3/cg/meta/clean/__init__.py
+-rw-r--r--   0        0        0     3901 2024-06-03 12:38:31.282665 cg-60.9.3/cg/meta/clean/api.py
+-rw-r--r--   0        0        0     7769 2024-06-03 12:38:31.282665 cg-60.9.3/cg/meta/clean/clean_flow_cells.py
+-rw-r--r--   0        0        0     1841 2024-06-03 12:38:31.282665 cg-60.9.3/cg/meta/clean/clean_retrieved_spring_files.py
+-rw-r--r--   0        0        0       34 2024-06-03 12:38:31.282665 cg-60.9.3/cg/meta/compress/__init__.py
+-rw-r--r--   0        0        0    14557 2024-06-03 12:38:31.282665 cg-60.9.3/cg/meta/compress/compress.py
+-rw-r--r--   0        0        0     4947 2024-06-03 12:38:31.282665 cg-60.9.3/cg/meta/compress/files.py
+-rw-r--r--   0        0        0       77 2024-06-03 12:38:31.282665 cg-60.9.3/cg/meta/deliver/__init__.py
+-rw-r--r--   0        0        0    14956 2024-06-03 12:38:31.282665 cg-60.9.3/cg/meta/deliver/deliver.py
+-rw-r--r--   0        0        0     4565 2024-06-03 12:38:31.282665 cg-60.9.3/cg/meta/deliver/deliver_ticket.py
+-rw-r--r--   0        0        0      904 2024-06-03 12:38:31.282665 cg-60.9.3/cg/meta/deliver/fastq_path_generator.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.282665 cg-60.9.3/cg/meta/delivery/__init__.py
+-rw-r--r--   0        0        0     8518 2024-06-03 12:38:31.282665 cg-60.9.3/cg/meta/delivery/delivery.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.282665 cg-60.9.3/cg/meta/demultiplex/__init__.py
+-rw-r--r--   0        0        0     2592 2024-06-03 12:38:31.282665 cg-60.9.3/cg/meta/demultiplex/combine_sequencing_metrics.py
+-rw-r--r--   0        0        0     5846 2024-06-03 12:38:31.282665 cg-60.9.3/cg/meta/demultiplex/demux_post_processing.py
+-rw-r--r--   0        0        0     8693 2024-06-03 12:38:31.282665 cg-60.9.3/cg/meta/demultiplex/housekeeper_storage_functions.py
+-rw-r--r--   0        0        0     6236 2024-06-03 12:38:31.282665 cg-60.9.3/cg/meta/demultiplex/status_db_storage_functions.py
+-rw-r--r--   0        0        0    10690 2024-06-03 12:38:31.282665 cg-60.9.3/cg/meta/demultiplex/utils.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.282665 cg-60.9.3/cg/meta/encryption/__init__.py
+-rw-r--r--   0        0        0    20305 2024-06-03 12:38:31.282665 cg-60.9.3/cg/meta/encryption/encryption.py
+-rw-r--r--   0        0        0      537 2024-06-03 12:38:31.282665 cg-60.9.3/cg/meta/encryption/sbatch.py
+-rw-r--r--   0        0        0    10922 2024-06-03 12:38:31.282665 cg-60.9.3/cg/meta/invoice.py
+-rw-r--r--   0        0        0     2360 2024-06-03 12:38:31.282665 cg-60.9.3/cg/meta/meta.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.282665 cg-60.9.3/cg/meta/observations/__init__.py
+-rw-r--r--   0        0        0     7052 2024-06-03 12:38:31.282665 cg-60.9.3/cg/meta/observations/balsamic_observations_api.py
+-rw-r--r--   0        0        0     6396 2024-06-03 12:38:31.282665 cg-60.9.3/cg/meta/observations/mip_dna_observations_api.py
+-rw-r--r--   0        0        0     6932 2024-06-03 12:38:31.282665 cg-60.9.3/cg/meta/observations/observations_api.py
+-rw-r--r--   0        0        0       27 2024-06-03 12:38:31.282665 cg-60.9.3/cg/meta/orders/__init__.py
+-rw-r--r--   0        0        0     3736 2024-06-03 12:38:31.282665 cg-60.9.3/cg/meta/orders/api.py
+-rw-r--r--   0        0        0      121 2024-06-03 12:38:31.282665 cg-60.9.3/cg/meta/orders/balsamic_qc_submitter.py
+-rw-r--r--   0        0        0      107 2024-06-03 12:38:31.282665 cg-60.9.3/cg/meta/orders/balsamic_submitter.py
+-rw-r--r--   0        0        0      122 2024-06-03 12:38:31.282665 cg-60.9.3/cg/meta/orders/balsamic_umi_submitter.py
+-rw-r--r--   0        0        0    15145 2024-06-03 12:38:31.282665 cg-60.9.3/cg/meta/orders/case_submitter.py
+-rw-r--r--   0        0        0     5991 2024-06-03 12:38:31.282665 cg-60.9.3/cg/meta/orders/fastq_submitter.py
+-rw-r--r--   0        0        0      105 2024-06-03 12:38:31.282665 cg-60.9.3/cg/meta/orders/fluffy_submitter.py
+-rw-r--r--   0        0        0     1254 2024-06-03 12:38:31.282665 cg-60.9.3/cg/meta/orders/lims.py
+-rw-r--r--   0        0        0     5782 2024-06-03 12:38:31.282665 cg-60.9.3/cg/meta/orders/metagenome_submitter.py
+-rw-r--r--   0        0        0     6337 2024-06-03 12:38:31.282665 cg-60.9.3/cg/meta/orders/microbial_submitter.py
+-rw-r--r--   0        0        0      123 2024-06-03 12:38:31.282665 cg-60.9.3/cg/meta/orders/microsalt_submitter.py
+-rw-r--r--   0        0        0      105 2024-06-03 12:38:31.282665 cg-60.9.3/cg/meta/orders/mip_dna_submitter.py
+-rw-r--r--   0        0        0      105 2024-06-03 12:38:31.282665 cg-60.9.3/cg/meta/orders/mip_rna_submitter.py
+-rw-r--r--   0        0        0     7622 2024-06-03 12:38:31.286666 cg-60.9.3/cg/meta/orders/pool_submitter.py
+-rw-r--r--   0        0        0      102 2024-06-03 12:38:31.286666 cg-60.9.3/cg/meta/orders/rml_submitter.py
+-rw-r--r--   0        0        0      718 2024-06-03 12:38:31.286666 cg-60.9.3/cg/meta/orders/rnafusion_submitter.py
+-rw-r--r--   0        0        0     1268 2024-06-03 12:38:31.286666 cg-60.9.3/cg/meta/orders/sars_cov_2_submitter.py
+-rw-r--r--   0        0        0     1754 2024-06-03 12:38:31.286666 cg-60.9.3/cg/meta/orders/submitter.py
+-rw-r--r--   0        0        0     7880 2024-06-03 12:38:31.286666 cg-60.9.3/cg/meta/orders/ticket_handler.py
+-rw-r--r--   0        0        0      104 2024-06-03 12:38:31.286666 cg-60.9.3/cg/meta/orders/tomte_submitter.py
+-rw-r--r--   0        0        0     4105 2024-06-03 12:38:31.286666 cg-60.9.3/cg/meta/qc_metrics/collect_qc_metrics.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.286666 cg-60.9.3/cg/meta/report/__init__.py
+-rw-r--r--   0        0        0     8168 2024-06-03 12:38:31.286666 cg-60.9.3/cg/meta/report/balsamic.py
+-rw-r--r--   0        0        0      562 2024-06-03 12:38:31.286666 cg-60.9.3/cg/meta/report/balsamic_qc.py
+-rw-r--r--   0        0        0      717 2024-06-03 12:38:31.286666 cg-60.9.3/cg/meta/report/balsamic_umi.py
+-rw-r--r--   0        0        0     4171 2024-06-03 12:38:31.286666 cg-60.9.3/cg/meta/report/field_validators.py
+-rw-r--r--   0        0        0     6620 2024-06-03 12:38:31.286666 cg-60.9.3/cg/meta/report/mip_dna.py
+-rw-r--r--   0        0        0    18543 2024-06-03 12:38:31.286666 cg-60.9.3/cg/meta/report/report_api.py
+-rw-r--r--   0        0        0     5625 2024-06-03 12:38:31.286666 cg-60.9.3/cg/meta/report/rnafusion.py
+-rw-r--r--   0        0        0     2822 2024-06-03 12:38:31.286666 cg-60.9.3/cg/meta/report/taxprofiler.py
+-rw-r--r--   0        0        0     1911 2024-06-03 12:38:31.286666 cg-60.9.3/cg/meta/report/templates/delivery-report.html
+-rw-r--r--   0        0        0     4460 2024-06-03 12:38:31.286666 cg-60.9.3/cg/meta/report/templates/macros/data_analysis/data_analysis.html
+-rw-r--r--   0        0        0     1049 2024-06-03 12:38:31.286666 cg-60.9.3/cg/meta/report/templates/macros/data_analysis/limitations.html
+-rw-r--r--   0        0        0     3351 2024-06-03 12:38:31.286666 cg-60.9.3/cg/meta/report/templates/macros/data_analysis/qc_metrics/balsamic_qc_metrics.html
+-rw-r--r--   0        0        0     1364 2024-06-03 12:38:31.286666 cg-60.9.3/cg/meta/report/templates/macros/data_analysis/qc_metrics/mip_dna_qc_metrics.html
+-rw-r--r--   0        0        0      807 2024-06-03 12:38:31.286666 cg-60.9.3/cg/meta/report/templates/macros/data_analysis/qc_metrics/qc_metrics.html
+-rw-r--r--   0        0        0     3284 2024-06-03 12:38:31.286666 cg-60.9.3/cg/meta/report/templates/macros/data_analysis/qc_metrics/rnafusion_qc_metrics.html
+-rw-r--r--   0        0        0     3670 2024-06-03 12:38:31.286666 cg-60.9.3/cg/meta/report/templates/macros/data_analysis/qc_metrics/tomte_qc_metrics.html
+-rw-r--r--   0        0        0     2332 2024-06-03 12:38:31.286666 cg-60.9.3/cg/meta/report/templates/macros/header.html
+-rw-r--r--   0        0        0     2178 2024-06-03 12:38:31.286666 cg-60.9.3/cg/meta/report/templates/macros/order.html
+-rw-r--r--   0        0        0     2243 2024-06-03 12:38:31.286666 cg-60.9.3/cg/meta/report/templates/macros/sample_prep.html
+-rw-r--r--   0        0        0      472 2024-06-03 12:38:31.286666 cg-60.9.3/cg/meta/report/templates/macros/ticket_system.html
+-rw-r--r--   0        0        0     1165 2024-06-03 12:38:31.286666 cg-60.9.3/cg/meta/report/templates/macros/uploaded_files/balsamic_uploaded_files.html
+-rw-r--r--   0        0        0     1538 2024-06-03 12:38:31.286666 cg-60.9.3/cg/meta/report/templates/macros/uploaded_files/mip_dna_uploaded_files.html
+-rw-r--r--   0        0        0      428 2024-06-03 12:38:31.286666 cg-60.9.3/cg/meta/report/templates/macros/uploaded_files/rnafusion_uploaded_files.html
+-rw-r--r--   0        0        0     4266 2024-06-03 12:38:31.286666 cg-60.9.3/cg/meta/report/templates/macros/uploaded_files/uploaded_files.html
+-rw-r--r--   0        0        0       80 2024-06-03 12:38:31.286666 cg-60.9.3/cg/meta/report/templates/partials/footer.html
+-rw-r--r--   0        0        0      172 2024-06-03 12:38:31.286666 cg-60.9.3/cg/meta/report/templates/partials/signature.html
+-rw-r--r--   0        0        0   232803 2024-06-03 12:38:31.286666 cg-60.9.3/cg/meta/report/templates/static/css/bootstrap.min.css
+-rw-r--r--   0        0        0       33 2024-06-03 12:38:31.286666 cg-60.9.3/cg/meta/report/templates/static/css/custom.css
+-rw-r--r--   0        0        0    30068 2024-06-03 12:38:31.286666 cg-60.9.3/cg/meta/report/templates/static/images/SWEDAC_logo.png
+-rw-r--r--   0        0        0     3913 2024-06-03 12:38:31.286666 cg-60.9.3/cg/meta/report/tomte.py
+-rw-r--r--   0        0        0       32 2024-06-03 12:38:31.286666 cg-60.9.3/cg/meta/rsync/__init__.py
+-rw-r--r--   0        0        0    12291 2024-06-03 12:38:31.286666 cg-60.9.3/cg/meta/rsync/rsync_api.py
+-rw-r--r--   0        0        0      387 2024-06-03 12:38:31.286666 cg-60.9.3/cg/meta/rsync/sbatch.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.286666 cg-60.9.3/cg/meta/tar/__init__.py
+-rw-r--r--   0        0        0     1694 2024-06-03 12:38:31.286666 cg-60.9.3/cg/meta/tar/tar.py
+-rw-r--r--   0        0        0       71 2024-06-03 12:38:31.286666 cg-60.9.3/cg/meta/transfer/__init__.py
+-rw-r--r--   0        0        0    10242 2024-06-03 12:38:31.286666 cg-60.9.3/cg/meta/transfer/external_data.py
+-rw-r--r--   0        0        0     5814 2024-06-03 12:38:31.286666 cg-60.9.3/cg/meta/transfer/lims.py
+-rw-r--r--   0        0        0      503 2024-06-03 12:38:31.286666 cg-60.9.3/cg/meta/transfer/utils.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.286666 cg-60.9.3/cg/meta/upload/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.286666 cg-60.9.3/cg/meta/upload/balsamic/__init__.py
+-rw-r--r--   0        0        0     3107 2024-06-03 12:38:31.286666 cg-60.9.3/cg/meta/upload/balsamic/balsamic.py
+-rw-r--r--   0        0        0     2224 2024-06-03 12:38:31.286666 cg-60.9.3/cg/meta/upload/coverage.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.286666 cg-60.9.3/cg/meta/upload/fohm/__init__.py
+-rw-r--r--   0        0        0    12102 2024-06-03 12:38:31.286666 cg-60.9.3/cg/meta/upload/fohm/fohm.py
+-rw-r--r--   0        0        0       30 2024-06-03 12:38:31.286666 cg-60.9.3/cg/meta/upload/gisaid/__init__.py
+-rw-r--r--   0        0        0      928 2024-06-03 12:38:31.286666 cg-60.9.3/cg/meta/upload/gisaid/constants.py
+-rw-r--r--   0        0        0    13521 2024-06-03 12:38:31.286666 cg-60.9.3/cg/meta/upload/gisaid/gisaid.py
+-rw-r--r--   0        0        0     3312 2024-06-03 12:38:31.286666 cg-60.9.3/cg/meta/upload/gisaid/models.py
+-rw-r--r--   0        0        0     5310 2024-06-03 12:38:31.286666 cg-60.9.3/cg/meta/upload/gt.py
+-rw-r--r--   0        0        0      898 2024-06-03 12:38:31.286666 cg-60.9.3/cg/meta/upload/microsalt/microsalt_upload_api.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.290665 cg-60.9.3/cg/meta/upload/mip/__init__.py
+-rw-r--r--   0        0        0     2546 2024-06-03 12:38:31.290665 cg-60.9.3/cg/meta/upload/mip/mip_dna.py
+-rw-r--r--   0        0        0     1400 2024-06-03 12:38:31.290665 cg-60.9.3/cg/meta/upload/mip/mip_rna.py
+-rw-r--r--   0        0        0     7294 2024-06-03 12:38:31.290665 cg-60.9.3/cg/meta/upload/mutacc.py
+-rw-r--r--   0        0        0     1853 2024-06-03 12:38:31.290665 cg-60.9.3/cg/meta/upload/nf_analysis.py
+-rw-r--r--   0        0        0       32 2024-06-03 12:38:31.290665 cg-60.9.3/cg/meta/upload/nipt/__init__.py
+-rw-r--r--   0        0        0      696 2024-06-03 12:38:31.290665 cg-60.9.3/cg/meta/upload/nipt/models.py
+-rw-r--r--   0        0        0     8106 2024-06-03 12:38:31.290665 cg-60.9.3/cg/meta/upload/nipt/nipt.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.290665 cg-60.9.3/cg/meta/upload/scout/__init__.py
+-rw-r--r--   0        0        0     4009 2024-06-03 12:38:31.290665 cg-60.9.3/cg/meta/upload/scout/balsamic_config_builder.py
+-rw-r--r--   0        0        0     1491 2024-06-03 12:38:31.290665 cg-60.9.3/cg/meta/upload/scout/balsamic_umi_config_builder.py
+-rw-r--r--   0        0        0     3322 2024-06-03 12:38:31.290665 cg-60.9.3/cg/meta/upload/scout/hk_tags.py
+-rw-r--r--   0        0        0     9103 2024-06-03 12:38:31.290665 cg-60.9.3/cg/meta/upload/scout/mip_config_builder.py
+-rw-r--r--   0        0        0     3495 2024-06-03 12:38:31.290665 cg-60.9.3/cg/meta/upload/scout/rnafusion_config_builder.py
+-rw-r--r--   0        0        0     7231 2024-06-03 12:38:31.290665 cg-60.9.3/cg/meta/upload/scout/scout_config_builder.py
+-rw-r--r--   0        0        0    23146 2024-06-03 12:38:31.290665 cg-60.9.3/cg/meta/upload/scout/uploadscoutapi.py
+-rw-r--r--   0        0        0     3197 2024-06-03 12:38:31.290665 cg-60.9.3/cg/meta/upload/upload_api.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.290665 cg-60.9.3/cg/meta/workflow/__init__.py
+-rw-r--r--   0        0        0    31742 2024-06-03 12:38:31.290665 cg-60.9.3/cg/meta/workflow/analysis.py
+-rw-r--r--   0        0        0    28062 2024-06-03 12:38:31.290665 cg-60.9.3/cg/meta/workflow/balsamic.py
+-rw-r--r--   0        0        0     2700 2024-06-03 12:38:31.290665 cg-60.9.3/cg/meta/workflow/balsamic_pon.py
+-rw-r--r--   0        0        0      553 2024-06-03 12:38:31.290665 cg-60.9.3/cg/meta/workflow/balsamic_qc.py
+-rw-r--r--   0        0        0      556 2024-06-03 12:38:31.290665 cg-60.9.3/cg/meta/workflow/balsamic_umi.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.290665 cg-60.9.3/cg/meta/workflow/downsample/__init__.py
+-rw-r--r--   0        0        0     3991 2024-06-03 12:38:31.290665 cg-60.9.3/cg/meta/workflow/downsample/downsample.py
+-rw-r--r--   0        0        0      711 2024-06-03 12:38:31.290665 cg-60.9.3/cg/meta/workflow/downsample/sbatch.py
+-rw-r--r--   0        0        0     8913 2024-06-03 12:38:31.290665 cg-60.9.3/cg/meta/workflow/fastq.py
+-rw-r--r--   0        0        0    10603 2024-06-03 12:38:31.290665 cg-60.9.3/cg/meta/workflow/fluffy.py
+-rw-r--r--   0        0        0      521 2024-06-03 12:38:31.290665 cg-60.9.3/cg/meta/workflow/jasen.py
+-rw-r--r--   0        0        0       70 2024-06-03 12:38:31.290665 cg-60.9.3/cg/meta/workflow/microsalt/__init__.py
+-rw-r--r--   0        0        0      116 2024-06-03 12:38:31.290665 cg-60.9.3/cg/meta/workflow/microsalt/constants.py
+-rw-r--r--   0        0        0      174 2024-06-03 12:38:31.290665 cg-60.9.3/cg/meta/workflow/microsalt/metrics_parser/__init__.py
+-rw-r--r--   0        0        0      366 2024-06-03 12:38:31.290665 cg-60.9.3/cg/meta/workflow/microsalt/metrics_parser/metrics_parser.py
+-rw-r--r--   0        0        0      903 2024-06-03 12:38:31.290665 cg-60.9.3/cg/meta/workflow/microsalt/metrics_parser/models.py
+-rw-r--r--   0        0        0    13257 2024-06-03 12:38:31.290665 cg-60.9.3/cg/meta/workflow/microsalt/microsalt.py
+-rw-r--r--   0        0        0      113 2024-06-03 12:38:31.290665 cg-60.9.3/cg/meta/workflow/microsalt/quality_controller/__init__.py
+-rw-r--r--   0        0        0      712 2024-06-03 12:38:31.290665 cg-60.9.3/cg/meta/workflow/microsalt/quality_controller/models.py
+-rw-r--r--   0        0        0     5697 2024-06-03 12:38:31.290665 cg-60.9.3/cg/meta/workflow/microsalt/quality_controller/quality_controller.py
+-rw-r--r--   0        0        0     1217 2024-06-03 12:38:31.290665 cg-60.9.3/cg/meta/workflow/microsalt/quality_controller/report_generator.py
+-rw-r--r--   0        0        0     2373 2024-06-03 12:38:31.290665 cg-60.9.3/cg/meta/workflow/microsalt/quality_controller/result_logger.py
+-rw-r--r--   0        0        0     5641 2024-06-03 12:38:31.290665 cg-60.9.3/cg/meta/workflow/microsalt/quality_controller/utils.py
+-rw-r--r--   0        0        0     1220 2024-06-03 12:38:31.290665 cg-60.9.3/cg/meta/workflow/microsalt/utils.py
+-rw-r--r--   0        0        0    12611 2024-06-03 12:38:31.290665 cg-60.9.3/cg/meta/workflow/mip.py
+-rw-r--r--   0        0        0     2948 2024-06-03 12:38:31.290665 cg-60.9.3/cg/meta/workflow/mip_dna.py
+-rw-r--r--   0        0        0     2124 2024-06-03 12:38:31.290665 cg-60.9.3/cg/meta/workflow/mip_rna.py
+-rw-r--r--   0        0        0    10957 2024-06-03 12:38:31.290665 cg-60.9.3/cg/meta/workflow/mutant.py
+-rw-r--r--   0        0        0    37498 2024-06-03 12:38:31.290665 cg-60.9.3/cg/meta/workflow/nf_analysis.py
+-rw-r--r--   0        0        0     6161 2024-06-03 12:38:31.290665 cg-60.9.3/cg/meta/workflow/nf_handlers.py
+-rw-r--r--   0        0        0     6357 2024-06-03 12:38:31.290665 cg-60.9.3/cg/meta/workflow/prepare_fastq.py
+-rw-r--r--   0        0        0     6028 2024-06-03 12:38:31.290665 cg-60.9.3/cg/meta/workflow/raredisease.py
+-rw-r--r--   0        0        0     5419 2024-06-03 12:38:31.290665 cg-60.9.3/cg/meta/workflow/rnafusion.py
+-rw-r--r--   0        0        0     4658 2024-06-03 12:38:31.290665 cg-60.9.3/cg/meta/workflow/taxprofiler.py
+-rw-r--r--   0        0        0     3592 2024-06-03 12:38:31.290665 cg-60.9.3/cg/meta/workflow/tomte.py
+-rw-r--r--   0        0        0      113 2024-06-03 12:38:31.290665 cg-60.9.3/cg/models/__init__.py
+-rw-r--r--   0        0        0      457 2024-06-03 12:38:31.290665 cg-60.9.3/cg/models/analysis.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.290665 cg-60.9.3/cg/models/balsamic/__init__.py
+-rw-r--r--   0        0        0      459 2024-06-03 12:38:31.290665 cg-60.9.3/cg/models/balsamic/analysis.py
+-rw-r--r--   0        0        0     4550 2024-06-03 12:38:31.290665 cg-60.9.3/cg/models/balsamic/config.py
+-rw-r--r--   0        0        0     1986 2024-06-03 12:38:31.290665 cg-60.9.3/cg/models/balsamic/metrics.py
+-rw-r--r--   0        0        0    18130 2024-06-03 12:38:31.290665 cg-60.9.3/cg/models/cg_config.py
+-rw-r--r--   0        0        0     4302 2024-06-03 12:38:31.290665 cg-60.9.3/cg/models/compression_data.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.290665 cg-60.9.3/cg/models/deliverables/__init__.py
+-rw-r--r--   0        0        0     5219 2024-06-03 12:38:31.290665 cg-60.9.3/cg/models/deliverables/metric_deliverables.py
+-rw-r--r--   0        0        0      243 2024-06-03 12:38:31.290665 cg-60.9.3/cg/models/delivery/delivery.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.290665 cg-60.9.3/cg/models/demultiplex/__init__.py
+-rw-r--r--   0        0        0    13100 2024-06-03 12:38:31.290665 cg-60.9.3/cg/models/demultiplex/run_parameters.py
+-rw-r--r--   0        0        0      539 2024-06-03 12:38:31.290665 cg-60.9.3/cg/models/demultiplex/sbatch.py
+-rw-r--r--   0        0        0     7006 2024-06-03 12:38:31.290665 cg-60.9.3/cg/models/downsample/downsample_data.py
+-rw-r--r--   0        0        0      255 2024-06-03 12:38:31.290665 cg-60.9.3/cg/models/email.py
+-rw-r--r--   0        0        0     1046 2024-06-03 12:38:31.290665 cg-60.9.3/cg/models/fastq.py
+-rw-r--r--   0        0        0     2157 2024-06-03 12:38:31.290665 cg-60.9.3/cg/models/file_data.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.290665 cg-60.9.3/cg/models/invoice/__init__.py
+-rw-r--r--   0        0        0     1254 2024-06-03 12:38:31.294665 cg-60.9.3/cg/models/invoice/invoice.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.294665 cg-60.9.3/cg/models/lims/__init__.py
+-rw-r--r--   0        0        0     2019 2024-06-03 12:38:31.294665 cg-60.9.3/cg/models/lims/sample.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.294665 cg-60.9.3/cg/models/mip/__init__.py
+-rw-r--r--   0        0        0      337 2024-06-03 12:38:31.294665 cg-60.9.3/cg/models/mip/mip_analysis.py
+-rw-r--r--   0        0        0     1564 2024-06-03 12:38:31.294665 cg-60.9.3/cg/models/mip/mip_config.py
+-rw-r--r--   0        0        0     4696 2024-06-03 12:38:31.294665 cg-60.9.3/cg/models/mip/mip_metrics_deliverables.py
+-rw-r--r--   0        0        0     2550 2024-06-03 12:38:31.294665 cg-60.9.3/cg/models/mip/mip_sample_info.py
+-rw-r--r--   0        0        0     2472 2024-06-03 12:38:31.294665 cg-60.9.3/cg/models/nf_analysis.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.294665 cg-60.9.3/cg/models/observations/__init__.py
+-rw-r--r--   0        0        0      688 2024-06-03 12:38:31.294665 cg-60.9.3/cg/models/observations/input_files.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.294665 cg-60.9.3/cg/models/orders/__init__.py
+-rw-r--r--   0        0        0     2691 2024-06-03 12:38:31.294665 cg-60.9.3/cg/models/orders/constants.py
+-rw-r--r--   0        0        0     5604 2024-06-03 12:38:31.294665 cg-60.9.3/cg/models/orders/excel_sample.py
+-rw-r--r--   0        0        0      898 2024-06-03 12:38:31.294665 cg-60.9.3/cg/models/orders/json_sample.py
+-rw-r--r--   0        0        0     1449 2024-06-03 12:38:31.294665 cg-60.9.3/cg/models/orders/order.py
+-rw-r--r--   0        0        0      811 2024-06-03 12:38:31.294665 cg-60.9.3/cg/models/orders/orderform_schema.py
+-rw-r--r--   0        0        0     4212 2024-06-03 12:38:31.294665 cg-60.9.3/cg/models/orders/sample_base.py
+-rw-r--r--   0        0        0     9786 2024-06-03 12:38:31.294665 cg-60.9.3/cg/models/orders/samples.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.294665 cg-60.9.3/cg/models/orders/validators/__init__.py
+-rw-r--r--   0        0        0     2328 2024-06-03 12:38:31.294665 cg-60.9.3/cg/models/orders/validators/excel_sample_validators.py
+-rw-r--r--   0        0        0      576 2024-06-03 12:38:31.294665 cg-60.9.3/cg/models/orders/validators/json_sample_validators.py
+-rw-r--r--   0        0        0       71 2024-06-03 12:38:31.294665 cg-60.9.3/cg/models/orders/validators/sample_base_validators.py
+-rw-r--r--   0        0        0      101 2024-06-03 12:38:31.294665 cg-60.9.3/cg/models/qc_metrics.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.294665 cg-60.9.3/cg/models/raredisease/__init__.py
+-rw-r--r--   0        0        0     2034 2024-06-03 12:38:31.294665 cg-60.9.3/cg/models/raredisease/raredisease.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.294665 cg-60.9.3/cg/models/report/__init__.py
+-rw-r--r--   0        0        0     8872 2024-06-03 12:38:31.294665 cg-60.9.3/cg/models/report/metadata.py
+-rw-r--r--   0        0        0     6180 2024-06-03 12:38:31.294665 cg-60.9.3/cg/models/report/report.py
+-rw-r--r--   0        0        0     5298 2024-06-03 12:38:31.294665 cg-60.9.3/cg/models/report/sample.py
+-rw-r--r--   0        0        0     3267 2024-06-03 12:38:31.294665 cg-60.9.3/cg/models/report/validators.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.294665 cg-60.9.3/cg/models/rnafusion/__init__.py
+-rw-r--r--   0        0        0     1865 2024-06-03 12:38:31.294665 cg-60.9.3/cg/models/rnafusion/rnafusion.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.294665 cg-60.9.3/cg/models/run_devices/__init__.py
+-rw-r--r--   0        0        0    14038 2024-06-03 12:38:31.294665 cg-60.9.3/cg/models/run_devices/illumina_run_directory_data.py
+-rw-r--r--   0        0        0      317 2024-06-03 12:38:31.294665 cg-60.9.3/cg/models/run_devices/utils.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.294665 cg-60.9.3/cg/models/scout/__init__.py
+-rw-r--r--   0        0        0     4783 2024-06-03 12:38:31.294665 cg-60.9.3/cg/models/scout/scout_load_config.py
+-rw-r--r--   0        0        0      116 2024-06-03 12:38:31.294665 cg-60.9.3/cg/models/scout/validators.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.294665 cg-60.9.3/cg/models/slurm/__init__.py
+-rw-r--r--   0        0        0      617 2024-06-03 12:38:31.294665 cg-60.9.3/cg/models/slurm/sbatch.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.294665 cg-60.9.3/cg/models/taxprofiler/__init__.py
+-rw-r--r--   0        0        0     2597 2024-06-03 12:38:31.294665 cg-60.9.3/cg/models/taxprofiler/taxprofiler.py
+-rw-r--r--   0        0        0     2588 2024-06-03 12:38:31.294665 cg-60.9.3/cg/models/tomte/tomte.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.294665 cg-60.9.3/cg/models/workflow/__init__.py
+-rw-r--r--   0        0        0      685 2024-06-03 12:38:31.294665 cg-60.9.3/cg/models/workflow/mutant.py
+-rw-r--r--   0        0        0       70 2024-06-03 12:38:31.294665 cg-60.9.3/cg/models/workflow/validators.py
+-rw-r--r--   0        0        0      842 2024-06-03 12:38:31.294665 cg-60.9.3/cg/resources/__init__.py
+-rw-r--r--   0        0        0     3493 2024-06-03 12:38:31.294665 cg-60.9.3/cg/resources/rnafusion_bundle_filenames.yaml
+-rw-r--r--   0        0        0     2434 2024-06-03 12:38:31.294665 cg-60.9.3/cg/resources/taxprofiler_bundle_filenames.yaml
+-rw-r--r--   0        0        0     4568 2024-06-03 12:38:31.294665 cg-60.9.3/cg/resources/tomte_bundle_filenames.yaml
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.294665 cg-60.9.3/cg/server/__init__.py
+-rw-r--r--   0        0        0    20348 2024-06-03 12:38:31.294665 cg-60.9.3/cg/server/admin.py
+-rw-r--r--   0        0        0    22743 2024-06-03 12:38:31.294665 cg-60.9.3/cg/server/api.py
+-rw-r--r--   0        0        0     4804 2024-06-03 12:38:31.294665 cg-60.9.3/cg/server/app.py
+-rw-r--r--   0        0        0       48 2024-06-03 12:38:31.294665 cg-60.9.3/cg/server/auto.py
+-rw-r--r--   0        0        0     1184 2024-06-03 12:38:31.294665 cg-60.9.3/cg/server/config.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.294665 cg-60.9.3/cg/server/dto/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.294665 cg-60.9.3/cg/server/dto/delivery_message/__init__.py
+-rw-r--r--   0        0        0      300 2024-06-03 12:38:31.294665 cg-60.9.3/cg/server/dto/delivery_message/delivery_message_request.py
+-rw-r--r--   0        0        0      183 2024-06-03 12:38:31.294665 cg-60.9.3/cg/server/dto/delivery_message/delivery_message_response.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.294665 cg-60.9.3/cg/server/dto/orders/__init__.py
+-rw-r--r--   0        0        0      165 2024-06-03 12:38:31.294665 cg-60.9.3/cg/server/dto/orders/order_delivery_update_request.py
+-rw-r--r--   0        0        0       91 2024-06-03 12:38:31.294665 cg-60.9.3/cg/server/dto/orders/order_patch_request.py
+-rw-r--r--   0        0        0      662 2024-06-03 12:38:31.294665 cg-60.9.3/cg/server/dto/orders/orders_request.py
+-rw-r--r--   0        0        0      414 2024-06-03 12:38:31.294665 cg-60.9.3/cg/server/dto/orders/orders_response.py
+-rw-r--r--   0        0        0     2599 2024-06-03 12:38:31.294665 cg-60.9.3/cg/server/ext.py
+-rw-r--r--   0        0        0       29 2024-06-03 12:38:31.294665 cg-60.9.3/cg/server/invoices/__init__.py
+-rw-r--r--   0        0        0     4793 2024-06-03 12:38:31.294665 cg-60.9.3/cg/server/invoices/templates/invoices/index.html
+-rw-r--r--   0        0        0     8171 2024-06-03 12:38:31.294665 cg-60.9.3/cg/server/invoices/templates/invoices/invoice.html
+-rw-r--r--   0        0        0     2838 2024-06-03 12:38:31.294665 cg-60.9.3/cg/server/invoices/templates/invoices/layout.html
+-rw-r--r--   0        0        0     4956 2024-06-03 12:38:31.294665 cg-60.9.3/cg/server/invoices/templates/invoices/new.html
+-rw-r--r--   0        0        0     7708 2024-06-03 12:38:31.294665 cg-60.9.3/cg/server/invoices/views.py
+-rw-r--r--   0        0        0      354 2024-06-03 12:38:31.294665 cg-60.9.3/cg/server/templates/admin/index.html
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.294665 cg-60.9.3/cg/services/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.294665 cg-60.9.3/cg/services/analysis_service/__init__.py
+-rw-r--r--   0        0        0      482 2024-06-03 12:38:31.294665 cg-60.9.3/cg/services/analysis_service/analysis_service.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.294665 cg-60.9.3/cg/services/delivery_message/__init__.py
+-rw-r--r--   0        0        0     2531 2024-06-03 12:38:31.294665 cg-60.9.3/cg/services/delivery_message/delivery_message_service.py
+-rw-r--r--   0        0        0      792 2024-06-03 12:38:31.294665 cg-60.9.3/cg/services/delivery_message/messages/__init__.py
+-rw-r--r--   0        0        0     1366 2024-06-03 12:38:31.294665 cg-60.9.3/cg/services/delivery_message/messages/analysis_scout_message.py
+-rw-r--r--   0        0        0      791 2024-06-03 12:38:31.294665 cg-60.9.3/cg/services/delivery_message/messages/covid_message.py
+-rw-r--r--   0        0        0      189 2024-06-03 12:38:31.294665 cg-60.9.3/cg/services/delivery_message/messages/delivery_message.py
+-rw-r--r--   0        0        0     1391 2024-06-03 12:38:31.298665 cg-60.9.3/cg/services/delivery_message/messages/fastq_analysis_scout_message.py
+-rw-r--r--   0        0        0      535 2024-06-03 12:38:31.298665 cg-60.9.3/cg/services/delivery_message/messages/fastq_message.py
+-rw-r--r--   0        0        0     1358 2024-06-03 12:38:31.298665 cg-60.9.3/cg/services/delivery_message/messages/fastq_scout_message.py
+-rw-r--r--   0        0        0      604 2024-06-03 12:38:31.298665 cg-60.9.3/cg/services/delivery_message/messages/microsalt_mwr_message.py
+-rw-r--r--   0        0        0      592 2024-06-03 12:38:31.298665 cg-60.9.3/cg/services/delivery_message/messages/microsalt_mwx_message.py
+-rw-r--r--   0        0        0      903 2024-06-03 12:38:31.298665 cg-60.9.3/cg/services/delivery_message/messages/scout_message.py
+-rw-r--r--   0        0        0      512 2024-06-03 12:38:31.298665 cg-60.9.3/cg/services/delivery_message/messages/statina_message.py
+-rw-r--r--   0        0        0      779 2024-06-03 12:38:31.298665 cg-60.9.3/cg/services/delivery_message/messages/utils.py
+-rw-r--r--   0        0        0     3300 2024-06-03 12:38:31.298665 cg-60.9.3/cg/services/delivery_message/utils.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.298665 cg-60.9.3/cg/services/fastq_concatenation_service/__init__.py
+-rw-r--r--   0        0        0      101 2024-06-03 12:38:31.298665 cg-60.9.3/cg/services/fastq_concatenation_service/exceptions.py
+-rw-r--r--   0        0        0     1110 2024-06-03 12:38:31.298665 cg-60.9.3/cg/services/fastq_concatenation_service/fastq_concatenation_service.py
+-rw-r--r--   0        0        0     3000 2024-06-03 12:38:31.298665 cg-60.9.3/cg/services/fastq_concatenation_service/utils.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.298665 cg-60.9.3/cg/services/illumina_services/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.298665 cg-60.9.3/cg/services/illumina_services/illumina_metrics_service/__init__.py
+-rw-r--r--   0        0        0    10867 2024-06-03 12:38:31.298665 cg-60.9.3/cg/services/illumina_services/illumina_metrics_service/bcl_convert_metrics_parser.py
+-rw-r--r--   0        0        0     1121 2024-06-03 12:38:31.298665 cg-60.9.3/cg/services/illumina_services/illumina_metrics_service/illumina_demux_version_service.py
+-rw-r--r--   0        0        0     9620 2024-06-03 12:38:31.298665 cg-60.9.3/cg/services/illumina_services/illumina_metrics_service/illumina_metrics_service.py
+-rw-r--r--   0        0        0     2826 2024-06-03 12:38:31.298665 cg-60.9.3/cg/services/illumina_services/illumina_metrics_service/models.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.298665 cg-60.9.3/cg/services/illumina_services/illumina_post_processing_service/__init__.py
+-rw-r--r--   0        0        0     5696 2024-06-03 12:38:31.298665 cg-60.9.3/cg/services/illumina_services/illumina_post_processing_service/illumina_post_processing_service.py
+-rw-r--r--   0        0        0      473 2024-06-03 12:38:31.298665 cg-60.9.3/cg/services/illumina_services/illumina_post_processing_service/utils.py
+-rw-r--r--   0        0        0     2924 2024-06-03 12:38:31.298665 cg-60.9.3/cg/services/illumina_services/illumina_post_processing_service/validation.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.298665 cg-60.9.3/cg/services/orders/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.298665 cg-60.9.3/cg/services/orders/order_service/__init__.py
+-rw-r--r--   0        0        0     2717 2024-06-03 12:38:31.298665 cg-60.9.3/cg/services/orders/order_service/order_service.py
+-rw-r--r--   0        0        0     1214 2024-06-03 12:38:31.298665 cg-60.9.3/cg/services/orders/order_service/utils.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.298665 cg-60.9.3/cg/services/orders/order_summary_service/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.298665 cg-60.9.3/cg/services/orders/order_summary_service/dto/__init__.py
+-rw-r--r--   0        0        0      236 2024-06-03 12:38:31.298665 cg-60.9.3/cg/services/orders/order_summary_service/dto/case_summary.py
+-rw-r--r--   0        0        0      319 2024-06-03 12:38:31.298665 cg-60.9.3/cg/services/orders/order_summary_service/dto/order_summary.py
+-rw-r--r--   0        0        0     2029 2024-06-03 12:38:31.298665 cg-60.9.3/cg/services/orders/order_summary_service/order_summary_service.py
+-rw-r--r--   0        0        0     2208 2024-06-03 12:38:31.298665 cg-60.9.3/cg/services/orders/order_summary_service/utils.py
+-rw-r--r--   0        0        0     1175 2024-06-03 12:38:31.298665 cg-60.9.3/cg/services/parse_run_completion_status_service/parse_run_completion_status_service.py
+-rw-r--r--   0        0        0       88 2024-06-03 12:38:31.298665 cg-60.9.3/cg/services/sequencing_qc_service/__init__.py
+-rw-r--r--   0        0        0     1822 2024-06-03 12:38:31.298665 cg-60.9.3/cg/services/sequencing_qc_service/quality_checks/checks.py
+-rw-r--r--   0        0        0     4987 2024-06-03 12:38:31.298665 cg-60.9.3/cg/services/sequencing_qc_service/quality_checks/utils.py
+-rw-r--r--   0        0        0      930 2024-06-03 12:38:31.298665 cg-60.9.3/cg/services/sequencing_qc_service/sequencing_qc_service.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.298665 cg-60.9.3/cg/services/slurm_service/__init__.py
+-rw-r--r--   0        0        0      703 2024-06-03 12:38:31.298665 cg-60.9.3/cg/services/slurm_service/slurm_cli_service.py
+-rw-r--r--   0        0        0      242 2024-06-03 12:38:31.298665 cg-60.9.3/cg/services/slurm_service/slurm_service.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.298665 cg-60.9.3/cg/services/slurm_upload_service/__init__.py
+-rw-r--r--   0        0        0      175 2024-06-03 12:38:31.298665 cg-60.9.3/cg/services/slurm_upload_service/slurm_upload_config.py
+-rw-r--r--   0        0        0     2074 2024-06-03 12:38:31.298665 cg-60.9.3/cg/services/slurm_upload_service/slurm_upload_service.py
+-rw-r--r--   0        0        0      203 2024-06-03 12:38:31.298665 cg-60.9.3/cg/services/slurm_upload_service/utils.py
+-rw-r--r--   0        0        0     2904 2024-06-03 12:38:31.298665 cg-60.9.3/cg/services/validate_file_transfer_service/validate_file_transfer_service.py
+-rw-r--r--   0        0        0     4161 2024-06-03 12:38:31.298665 cg-60.9.3/cg/services/validate_file_transfer_service/validate_pacbio_file_transfer_service.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.298665 cg-60.9.3/cg/store/__init__.py
+-rw-r--r--   0        0        0     4650 2024-06-03 12:38:31.298665 cg-60.9.3/cg/store/base.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.298665 cg-60.9.3/cg/store/crud/__init__.py
+-rw-r--r--   0        0        0    16830 2024-06-03 12:38:31.298665 cg-60.9.3/cg/store/crud/create.py
+-rw-r--r--   0        0        0     2144 2024-06-03 12:38:31.298665 cg-60.9.3/cg/store/crud/delete.py
+-rw-r--r--   0        0        0    60570 2024-06-03 12:38:31.298665 cg-60.9.3/cg/store/crud/read.py
+-rw-r--r--   0        0        0     1121 2024-06-03 12:38:31.298665 cg-60.9.3/cg/store/crud/update.py
+-rw-r--r--   0        0        0     1662 2024-06-03 12:38:31.298665 cg-60.9.3/cg/store/database.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.298665 cg-60.9.3/cg/store/filters/__init__.py
+-rw-r--r--   0        0        0     5371 2024-06-03 12:38:31.298665 cg-60.9.3/cg/store/filters/status_analysis_filters.py
+-rw-r--r--   0        0        0     1712 2024-06-03 12:38:31.298665 cg-60.9.3/cg/store/filters/status_application_filters.py
+-rw-r--r--   0        0        0     1440 2024-06-03 12:38:31.298665 cg-60.9.3/cg/store/filters/status_application_limitations_filters.py
+-rw-r--r--   0        0        0     2523 2024-06-03 12:38:31.298665 cg-60.9.3/cg/store/filters/status_application_version_filters.py
+-rw-r--r--   0        0        0     1390 2024-06-03 12:38:31.298665 cg-60.9.3/cg/store/filters/status_bed_filters.py
+-rw-r--r--   0        0        0     1317 2024-06-03 12:38:31.298665 cg-60.9.3/cg/store/filters/status_bed_version_filters.py
+-rw-r--r--   0        0        0    10801 2024-06-03 12:38:31.298665 cg-60.9.3/cg/store/filters/status_case_filters.py
+-rw-r--r--   0        0        0     3272 2024-06-03 12:38:31.298665 cg-60.9.3/cg/store/filters/status_case_sample_filters.py
+-rw-r--r--   0        0        0      903 2024-06-03 12:38:31.298665 cg-60.9.3/cg/store/filters/status_collaboration_filters.py
+-rw-r--r--   0        0        0     1412 2024-06-03 12:38:31.298665 cg-60.9.3/cg/store/filters/status_customer_filters.py
+-rw-r--r--   0        0        0     1880 2024-06-03 12:38:31.298665 cg-60.9.3/cg/store/filters/status_flow_cell_filters.py
+-rw-r--r--   0        0        0      896 2024-06-03 12:38:31.298665 cg-60.9.3/cg/store/filters/status_illumina_flow_cell_filters.py
+-rw-r--r--   0        0        0     1255 2024-06-03 12:38:31.298665 cg-60.9.3/cg/store/filters/status_invoice_filters.py
+-rw-r--r--   0        0        0     2792 2024-06-03 12:38:31.298665 cg-60.9.3/cg/store/filters/status_metrics_filters.py
+-rw-r--r--   0        0        0     3225 2024-06-03 12:38:31.298665 cg-60.9.3/cg/store/filters/status_order_filters.py
+-rw-r--r--   0        0        0      851 2024-06-03 12:38:31.298665 cg-60.9.3/cg/store/filters/status_organism_filters.py
+-rw-r--r--   0        0        0      783 2024-06-03 12:38:31.298665 cg-60.9.3/cg/store/filters/status_panel_filters.py
+-rw-r--r--   0        0        0     3923 2024-06-03 12:38:31.298665 cg-60.9.3/cg/store/filters/status_pool_filters.py
+-rw-r--r--   0        0        0     8660 2024-06-03 12:38:31.298665 cg-60.9.3/cg/store/filters/status_sample_filters.py
+-rw-r--r--   0        0        0      731 2024-06-03 12:38:31.298665 cg-60.9.3/cg/store/filters/status_user_filters.py
+-rw-r--r--   0        0        0    41645 2024-06-03 12:38:31.298665 cg-60.9.3/cg/store/models.py
+-rw-r--r--   0        0        0      706 2024-06-03 12:38:31.298665 cg-60.9.3/cg/store/store.py
+-rw-r--r--   0        0        0       30 2024-06-03 12:38:31.298665 cg-60.9.3/cg/utils/__init__.py
+-rw-r--r--   0        0        0      187 2024-06-03 12:38:31.298665 cg-60.9.3/cg/utils/calculations.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.298665 cg-60.9.3/cg/utils/checksum/__init__.py
+-rw-r--r--   0        0        0     1992 2024-06-03 12:38:31.298665 cg-60.9.3/cg/utils/checksum/checksum.py
+-rw-r--r--   0        0        0     1655 2024-06-03 12:38:31.298665 cg-60.9.3/cg/utils/click/EnumChoice.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.298665 cg-60.9.3/cg/utils/click/__init__.py
+-rw-r--r--   0        0        0     4910 2024-06-03 12:38:31.298665 cg-60.9.3/cg/utils/commands.py
+-rw-r--r--   0        0        0     1811 2024-06-03 12:38:31.302666 cg-60.9.3/cg/utils/date.py
+-rw-r--r--   0        0        0      635 2024-06-03 12:38:31.302666 cg-60.9.3/cg/utils/dict.py
+-rw-r--r--   0        0        0     2111 2024-06-03 12:38:31.302666 cg-60.9.3/cg/utils/dispatcher.py
+-rw-r--r--   0        0        0     1251 2024-06-03 12:38:31.302666 cg-60.9.3/cg/utils/email.py
+-rw-r--r--   0        0        0      134 2024-06-03 12:38:31.302666 cg-60.9.3/cg/utils/enums.py
+-rw-r--r--   0        0        0     3727 2024-06-03 12:38:31.302666 cg-60.9.3/cg/utils/files.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.302666 cg-60.9.3/cg/utils/flask/__init__.py
+-rw-r--r--   0        0        0     1052 2024-06-03 12:38:31.302666 cg-60.9.3/cg/utils/flask/enum.py
+-rw-r--r--   0        0        0      233 2024-06-03 12:38:31.302666 cg-60.9.3/cg/utils/flow_cell.py
+-rw-r--r--   0        0        0     1552 2024-06-03 12:38:31.302666 cg-60.9.3/cg/utils/time.py
+-rw-r--r--   0        0        0     1410 2024-06-03 12:38:31.302666 cg-60.9.3/cg/utils/utils.py
+-rw-r--r--   0        0        0     1697 2024-06-03 12:38:31.302666 cg-60.9.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.302666 cg-60.9.3/tests/__init__.py
+-rw-r--r--   0        0        0     1158 2024-06-03 12:38:31.302666 cg-60.9.3/tests/apps/conftest.py
+-rw-r--r--   0        0        0      231 2024-06-03 12:38:31.302666 cg-60.9.3/tests/apps/coverage/conftest.py
+-rw-r--r--   0        0        0     6188 2024-06-03 12:38:31.302666 cg-60.9.3/tests/apps/coverage/test_coverage.py
+-rw-r--r--   0        0        0     1693 2024-06-03 12:38:31.302666 cg-60.9.3/tests/apps/crunchy/conftest.py
+-rw-r--r--   0        0        0     5438 2024-06-03 12:38:31.302666 cg-60.9.3/tests/apps/crunchy/test_compress_fastq.py
+-rw-r--r--   0        0        0     2283 2024-06-03 12:38:31.302666 cg-60.9.3/tests/apps/crunchy/test_config.py
+-rw-r--r--   0        0        0    14032 2024-06-03 12:38:31.302666 cg-60.9.3/tests/apps/crunchy/test_crunchy.py
+-rw-r--r--   0        0        0     9109 2024-06-03 12:38:31.302666 cg-60.9.3/tests/apps/crunchy/test_spring_decompression.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.302666 cg-60.9.3/tests/apps/demultiplex/__init__.py
+-rw-r--r--   0        0        0     4994 2024-06-03 12:38:31.302666 cg-60.9.3/tests/apps/demultiplex/conftest.py
+-rw-r--r--   0        0        0     4039 2024-06-03 12:38:31.302666 cg-60.9.3/tests/apps/demultiplex/test_create_sample_sheet.py
+-rw-r--r--   0        0        0     8033 2024-06-03 12:38:31.302666 cg-60.9.3/tests/apps/demultiplex/test_demultiplex_api.py
+-rw-r--r--   0        0        0     4782 2024-06-03 12:38:31.302666 cg-60.9.3/tests/apps/demultiplex/test_index.py
+-rw-r--r--   0        0        0     9468 2024-06-03 12:38:31.302666 cg-60.9.3/tests/apps/demultiplex/test_override_cycles_validator.py
+-rw-r--r--   0        0        0     4042 2024-06-03 12:38:31.302666 cg-60.9.3/tests/apps/demultiplex/test_read_sample_sheet.py
+-rw-r--r--   0        0        0    12389 2024-06-03 12:38:31.302666 cg-60.9.3/tests/apps/demultiplex/test_sample_models.py
+-rw-r--r--   0        0        0      951 2024-06-03 12:38:31.302666 cg-60.9.3/tests/apps/demultiplex/test_sample_sheet_creator.py
+-rw-r--r--   0        0        0     3175 2024-06-03 12:38:31.302666 cg-60.9.3/tests/apps/demultiplex/test_sample_sheet_models.py
+-rw-r--r--   0        0        0    10932 2024-06-03 12:38:31.302666 cg-60.9.3/tests/apps/demultiplex/test_sample_sheet_validator.py
+-rw-r--r--   0        0        0     4993 2024-06-03 12:38:31.302666 cg-60.9.3/tests/apps/demultiplex/test_translate_sample_sheet.py
+-rw-r--r--   0        0        0     1450 2024-06-03 12:38:31.302666 cg-60.9.3/tests/apps/demultiplex/test_validate.py
+-rw-r--r--   0        0        0     5105 2024-06-03 12:38:31.306666 cg-60.9.3/tests/apps/downsample/test_downsample.py
+-rw-r--r--   0        0        0     1419 2024-06-03 12:38:31.306666 cg-60.9.3/tests/apps/downsample/test_downsample_utils.py
+-rw-r--r--   0        0        0     1716 2024-06-03 12:38:31.306666 cg-60.9.3/tests/apps/gens/test_gens_api.py
+-rw-r--r--   0        0        0     1950 2024-06-03 12:38:31.306666 cg-60.9.3/tests/apps/gt/conftest.py
+-rw-r--r--   0        0        0     4276 2024-06-03 12:38:31.306666 cg-60.9.3/tests/apps/gt/test_gt_api.py
+-rw-r--r--   0        0        0     1453 2024-06-03 12:38:31.306666 cg-60.9.3/tests/apps/hk/conftest.py
+-rw-r--r--   0        0        0      684 2024-06-03 12:38:31.306666 cg-60.9.3/tests/apps/hk/test__getattr__.py
+-rw-r--r--   0        0        0     1593 2024-06-03 12:38:31.306666 cg-60.9.3/tests/apps/hk/test_add_file.py
+-rw-r--r--   0        0        0     3523 2024-06-03 12:38:31.306666 cg-60.9.3/tests/apps/hk/test_bundles.py
+-rw-r--r--   0        0        0      871 2024-06-03 12:38:31.306666 cg-60.9.3/tests/apps/hk/test_core.py
+-rw-r--r--   0        0        0    31172 2024-06-03 12:38:31.306666 cg-60.9.3/tests/apps/hk/test_file.py
+-rw-r--r--   0        0        0     5080 2024-06-03 12:38:31.306666 cg-60.9.3/tests/apps/hk/test_version.py
+-rw-r--r--   0        0        0     1840 2024-06-03 12:38:31.306666 cg-60.9.3/tests/apps/lims/conftest.py
+-rw-r--r--   0        0        0     3197 2024-06-03 12:38:31.306666 cg-60.9.3/tests/apps/lims/test_api.py
+-rw-r--r--   0        0        0     1451 2024-06-03 12:38:31.306666 cg-60.9.3/tests/apps/lims/test_sample_sheet.py
+-rw-r--r--   0        0        0     9146 2024-06-03 12:38:31.306666 cg-60.9.3/tests/apps/loqus/test_loqusdb_api.py
+-rw-r--r--   0        0        0     2439 2024-06-03 12:38:31.306666 cg-60.9.3/tests/apps/madeline/conftest.py
+-rw-r--r--   0        0        0     4653 2024-06-03 12:38:31.306666 cg-60.9.3/tests/apps/madeline/test_madeline.py
+-rw-r--r--   0        0        0     3328 2024-06-03 12:38:31.306666 cg-60.9.3/tests/apps/mip/conftest.py
+-rw-r--r--   0        0        0     2487 2024-06-03 12:38:31.306666 cg-60.9.3/tests/apps/mip/test_config_mip.py
+-rw-r--r--   0        0        0      883 2024-06-03 12:38:31.306666 cg-60.9.3/tests/apps/mutacc_auto/conftest.py
+-rw-r--r--   0        0        0     2473 2024-06-03 12:38:31.306666 cg-60.9.3/tests/apps/mutacc_auto/test_mutacc_auto.py
+-rw-r--r--   0        0        0    12196 2024-06-03 12:38:31.306666 cg-60.9.3/tests/apps/orderform/conftest.py
+-rw-r--r--   0        0        0     9484 2024-06-03 12:38:31.306666 cg-60.9.3/tests/apps/orderform/test_excel_orderform_parser.py
+-rw-r--r--   0        0        0     4351 2024-06-03 12:38:31.306666 cg-60.9.3/tests/apps/orderform/test_excel_sample_schema.py
+-rw-r--r--   0        0        0     1032 2024-06-03 12:38:31.306666 cg-60.9.3/tests/apps/orderform/test_json_orderform_parser.py
+-rw-r--r--   0        0        0     2474 2024-06-03 12:38:31.306666 cg-60.9.3/tests/apps/orderform/test_orderform_parser.py
+-rw-r--r--   0        0        0    16002 2024-06-03 12:38:31.306666 cg-60.9.3/tests/apps/orderform/validators/test_excel_sample_validators.py
+-rw-r--r--   0        0        0     3670 2024-06-03 12:38:31.306666 cg-60.9.3/tests/apps/scout/conftest.py
+-rw-r--r--   0        0        0     2269 2024-06-03 12:38:31.306666 cg-60.9.3/tests/apps/scout/test_get_causative_variants.py
+-rw-r--r--   0        0        0     1376 2024-06-03 12:38:31.306666 cg-60.9.3/tests/apps/scout/test_get_scout_cases.py
+-rw-r--r--   0        0        0     1840 2024-06-03 12:38:31.306666 cg-60.9.3/tests/apps/scout/test_scout_load_config.py
+-rw-r--r--   0        0        0     7047 2024-06-03 12:38:31.306666 cg-60.9.3/tests/apps/scout/test_scout_models.py
+-rw-r--r--   0        0        0     1131 2024-06-03 12:38:31.306666 cg-60.9.3/tests/apps/slurm/conftest.py
+-rw-r--r--   0        0        0     4412 2024-06-03 12:38:31.306666 cg-60.9.3/tests/apps/slurm/test_slurm_api.py
+-rw-r--r--   0        0        0      831 2024-06-03 12:38:31.306666 cg-60.9.3/tests/apps/test_apps_environ.py
+-rw-r--r--   0        0        0      957 2024-06-03 12:38:31.306666 cg-60.9.3/tests/apps/test_osticket.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.306666 cg-60.9.3/tests/cli/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.306666 cg-60.9.3/tests/cli/add/__init__.py
+-rw-r--r--   0        0        0     1174 2024-06-03 12:38:31.306666 cg-60.9.3/tests/cli/add/test_cli_add.py
+-rw-r--r--   0        0        0     2471 2024-06-03 12:38:31.306666 cg-60.9.3/tests/cli/add/test_cli_add_customer.py
+-rw-r--r--   0        0        0     6841 2024-06-03 12:38:31.306666 cg-60.9.3/tests/cli/add/test_cli_add_family.py
+-rw-r--r--   0        0        0     7588 2024-06-03 12:38:31.306666 cg-60.9.3/tests/cli/add/test_cli_add_relationship.py
+-rw-r--r--   0        0        0     8382 2024-06-03 12:38:31.306666 cg-60.9.3/tests/cli/add/test_cli_add_sample.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.306666 cg-60.9.3/tests/cli/backup/__init__.py
+-rw-r--r--   0        0        0      705 2024-06-03 12:38:31.306666 cg-60.9.3/tests/cli/backup/conftest.py
+-rw-r--r--   0        0        0    11172 2024-06-03 12:38:31.306666 cg-60.9.3/tests/cli/backup/test_backup_command.py
+-rw-r--r--   0        0        0     6819 2024-06-03 12:38:31.306666 cg-60.9.3/tests/cli/clean/conftest.py
+-rw-r--r--   0        0        0     5564 2024-06-03 12:38:31.306666 cg-60.9.3/tests/cli/clean/test_balsamic_clean.py
+-rw-r--r--   0        0        0     2564 2024-06-03 12:38:31.306666 cg-60.9.3/tests/cli/clean/test_clean_flow_cell.py
+-rw-r--r--   0        0        0     1830 2024-06-03 12:38:31.306666 cg-60.9.3/tests/cli/clean/test_clean_hk_bundle_files.py
+-rw-r--r--   0        0        0     2098 2024-06-03 12:38:31.306666 cg-60.9.3/tests/cli/clean/test_hk_bundle_files.py
+-rw-r--r--   0        0        0     4610 2024-06-03 12:38:31.306666 cg-60.9.3/tests/cli/clean/test_hk_case_bundle_files.py
+-rw-r--r--   0        0        0     3592 2024-06-03 12:38:31.306666 cg-60.9.3/tests/cli/clean/test_microbial_clean.py
+-rw-r--r--   0        0        0     1888 2024-06-03 12:38:31.306666 cg-60.9.3/tests/cli/clean/test_rsync_past_run_dirs.py
+-rw-r--r--   0        0        0     9707 2024-06-03 12:38:31.306666 cg-60.9.3/tests/cli/compress/conftest.py
+-rw-r--r--   0        0        0     7709 2024-06-03 12:38:31.306666 cg-60.9.3/tests/cli/compress/test_cli_compress_fastq.py
+-rw-r--r--   0        0        0     1416 2024-06-03 12:38:31.306666 cg-60.9.3/tests/cli/compress/test_cli_decompress_spring.py
+-rw-r--r--   0        0        0     5205 2024-06-03 12:38:31.306666 cg-60.9.3/tests/cli/compress/test_compress_helpers.py
+-rw-r--r--   0        0        0     1239 2024-06-03 12:38:31.306666 cg-60.9.3/tests/cli/compress/test_store_fastq.py
+-rw-r--r--   0        0        0     7558 2024-06-03 12:38:31.306666 cg-60.9.3/tests/cli/conftest.py
+-rw-r--r--   0        0        0    12747 2024-06-03 12:38:31.306666 cg-60.9.3/tests/cli/delete/test_cli_delete_case.py
+-rw-r--r--   0        0        0     1873 2024-06-03 12:38:31.306666 cg-60.9.3/tests/cli/delete/test_cli_delete_cases.py
+-rw-r--r--   0        0        0     3794 2024-06-03 12:38:31.306666 cg-60.9.3/tests/cli/deliver/conftest.py
+-rw-r--r--   0        0        0     4428 2024-06-03 12:38:31.306666 cg-60.9.3/tests/cli/deliver/test_deliver_base.py
+-rw-r--r--   0        0        0     1166 2024-06-03 12:38:31.306666 cg-60.9.3/tests/cli/deliver/test_rsync_base.py
+-rw-r--r--   0        0        0     8569 2024-06-03 12:38:31.306666 cg-60.9.3/tests/cli/deliver/test_run_deliver_cmd.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.306666 cg-60.9.3/tests/cli/demultiplex/__init__.py
+-rw-r--r--   0        0        0     5224 2024-06-03 12:38:31.306666 cg-60.9.3/tests/cli/demultiplex/test_create_sample_sheet.py
+-rw-r--r--   0        0        0     5483 2024-06-03 12:38:31.306666 cg-60.9.3/tests/cli/demultiplex/test_demultiplex_flowcell.py
+-rw-r--r--   0        0        0     1639 2024-06-03 12:38:31.306666 cg-60.9.3/tests/cli/demultiplex/test_finish_demux.py
+-rw-r--r--   0        0        0     3015 2024-06-03 12:38:31.306666 cg-60.9.3/tests/cli/demultiplex/test_validate_sample_sheet.py
+-rw-r--r--   0        0        0     4291 2024-06-03 12:38:31.306666 cg-60.9.3/tests/cli/demultiplex/test_verify_syncing.py
+-rw-r--r--   0        0        0     1585 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/downsample/test_cli_downsample.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/generate/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/generate/report/__init__.py
+-rw-r--r--   0        0        0     1622 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/generate/report/conftest.py
+-rw-r--r--   0        0        0     2477 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/generate/report/test_cli_delivery_report.py
+-rw-r--r--   0        0        0     2760 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/generate/report/test_utils.py
+-rw-r--r--   0        0        0      563 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/generate/test_cli_base.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/get/__init__.py
+-rw-r--r--   0        0        0      863 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/get/test_cli_get.py
+-rw-r--r--   0        0        0     1526 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/get/test_cli_get_analysis.py
+-rw-r--r--   0        0        0     1242 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/get/test_cli_get_case.py
+-rw-r--r--   0        0        0     6208 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/get/test_cli_get_flow_cell.py
+-rw-r--r--   0        0        0     8835 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/get/test_cli_get_sample.py
+-rw-r--r--   0        0        0     1364 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/set/conftest.py
+-rw-r--r--   0        0        0     7311 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/set/test_cli_set_case.py
+-rw-r--r--   0        0        0     1460 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/set/test_cli_set_cases.py
+-rw-r--r--   0        0        0     2018 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/set/test_cli_set_flowcell.py
+-rw-r--r--   0        0        0     1685 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/set/test_cli_set_list_keys.py
+-rw-r--r--   0        0        0    12450 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/set/test_cli_set_sample.py
+-rw-r--r--   0        0        0     6124 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/set/test_cli_set_samples.py
+-rw-r--r--   0        0        0     7015 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/store/test_store.py
+-rw-r--r--   0        0        0     2332 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/test_base.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/upload/__init__.py
+-rw-r--r--   0        0        0    10102 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/upload/conftest.py
+-rw-r--r--   0        0        0     2295 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/upload/test_cli_scout.py
+-rw-r--r--   0        0        0     1789 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/upload/test_cli_upload.py
+-rw-r--r--   0        0        0      971 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/upload/test_cli_upload_auto.py
+-rw-r--r--   0        0        0     1669 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/upload/test_cli_upload_delivery_report.py
+-rw-r--r--   0        0        0      895 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/upload/test_cli_upload_fastq.py
+-rw-r--r--   0        0        0     1199 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/upload/test_cli_upload_genotype.py
+-rw-r--r--   0        0        0      694 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/upload/test_cli_upload_gens.py
+-rw-r--r--   0        0        0     9965 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/upload/test_cli_upload_nipt.py
+-rw-r--r--   0        0        0     4684 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/upload/test_cli_upload_nipt_ftp.py
+-rw-r--r--   0        0        0     1839 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/upload/test_cli_upload_nipt_statina.py
+-rw-r--r--   0        0        0     4193 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/upload/test_cli_upload_observations.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/workflow/__init__.py
+-rw-r--r--   0        0        0    31369 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/workflow/balsamic/conftest.py
+-rw-r--r--   0        0        0    13938 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py
+-rw-r--r--   0        0        0     7950 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/workflow/balsamic/test_compound_commands.py
+-rw-r--r--   0        0        0     2336 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/workflow/balsamic/test_link.py
+-rw-r--r--   0        0        0     3554 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/workflow/balsamic/test_report_deliver.py
+-rw-r--r--   0        0        0     6209 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/workflow/balsamic/test_run.py
+-rw-r--r--   0        0        0     7014 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/workflow/balsamic/test_store_housekeeper.py
+-rw-r--r--   0        0        0     8171 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/workflow/conftest.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/workflow/fastq/__init__.py
+-rw-r--r--   0        0        0     2332 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/workflow/fastq/test_fastq_base.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/workflow/fluffy/__init__.py
+-rw-r--r--   0        0        0     5237 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/workflow/fluffy/conftest.py
+-rw-r--r--   0        0        0     5687 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py
+-rw-r--r--   0        0        0     3302 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/workflow/fluffy/test_cli_link.py
+-rw-r--r--   0        0        0     1896 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/workflow/fluffy/test_cli_run.py
+-rw-r--r--   0        0        0     2968 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/workflow/fluffy/test_cli_start.py
+-rw-r--r--   0        0        0     7815 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/workflow/fluffy/test_cli_store.py
+-rw-r--r--   0        0        0     2775 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/workflow/microsalt/conftest.py
+-rw-r--r--   0        0        0     7059 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/workflow/microsalt/test_microsalt_case_config.py
+-rw-r--r--   0        0        0     1007 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/workflow/microsalt/test_microsalt_run.py
+-rw-r--r--   0        0        0     6544 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/workflow/mip/conftest.py
+-rw-r--r--   0        0        0     7011 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/workflow/mip/test_cli_mip_base.py
+-rw-r--r--   0        0        0     1542 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py
+-rw-r--r--   0        0        0      431 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/workflow/mip/test_cli_mip_dna_link.py
+-rw-r--r--   0        0        0     2108 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/workflow/mip/test_cli_mip_dna_manged_variants.py
+-rw-r--r--   0        0        0     1273 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/workflow/mip/test_cli_mip_dna_panel.py
+-rw-r--r--   0        0        0     3595 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/workflow/mip/test_cli_mip_dna_run.py
+-rw-r--r--   0        0        0     3884 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/workflow/mip/test_cli_mip_dna_start.py
+-rw-r--r--   0        0        0     1004 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py
+-rw-r--r--   0        0        0      527 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/workflow/mip/test_cli_mip_rna_link.py
+-rw-r--r--   0        0        0      716 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/workflow/mip/test_cli_mip_rna_run.py
+-rw-r--r--   0        0        0     8559 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/workflow/mip/test_cli_mip_store.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/workflow/nf_analysis/__init__.py
+-rw-r--r--   0        0        0     8504 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/workflow/nf_analysis/test_cli_config_case.py
+-rw-r--r--   0        0        0     3831 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/workflow/nf_analysis/test_cli_metrics_deliver.py
+-rw-r--r--   0        0        0     5087 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/workflow/nf_analysis/test_cli_report_deliver.py
+-rw-r--r--   0        0        0     9211 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/workflow/nf_analysis/test_cli_run.py
+-rw-r--r--   0        0        0     3331 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/workflow/nf_analysis/test_cli_start.py
+-rw-r--r--   0        0        0     9877 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/workflow/nf_analysis/test_cli_store.py
+-rw-r--r--   0        0        0    10453 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/workflow/nf_analysis/test_cli_store_housekeeper.py
+-rw-r--r--   0        0        0      978 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/workflow/nf_analysis/test_cli_workflow_base.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/workflow/raredisease/__init__.py
+-rw-r--r--   0        0        0     3940 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/workflow/raredisease/test_cli_raredisease_compound_commands.py
+-rw-r--r--   0        0        0      921 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/workflow/test_cli_workflow.py
+-rw-r--r--   0        0        0     4310 2024-06-03 12:38:31.310665 cg-60.9.3/tests/cli/workflow/test_cli_workflow_clean.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.310665 cg-60.9.3/tests/clients/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.310665 cg-60.9.3/tests/clients/arnold/__init__.py
+-rw-r--r--   0        0        0     1080 2024-06-03 12:38:31.310665 cg-60.9.3/tests/clients/arnold/conftest.py
+-rw-r--r--   0        0        0     1503 2024-06-03 12:38:31.314666 cg-60.9.3/tests/clients/arnold/test_arnold_api_client.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.314666 cg-60.9.3/tests/clients/janus/__init__.py
+-rw-r--r--   0        0        0     2381 2024-06-03 12:38:31.314666 cg-60.9.3/tests/clients/janus/conftest.py
+-rw-r--r--   0        0        0     1716 2024-06-03 12:38:31.314666 cg-60.9.3/tests/clients/janus/test_janus_api_client.py
+-rw-r--r--   0        0        0   128129 2024-06-03 12:38:31.314666 cg-60.9.3/tests/conftest.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.314666 cg-60.9.3/tests/fixture_plugins/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.314666 cg-60.9.3/tests/fixture_plugins/delivery_fixtures/__init__.py
+-rw-r--r--   0        0        0     2653 2024-06-03 12:38:31.314666 cg-60.9.3/tests/fixture_plugins/delivery_fixtures/bundle_fixtures.py
+-rw-r--r--   0        0        0     4972 2024-06-03 12:38:31.314666 cg-60.9.3/tests/fixture_plugins/delivery_fixtures/context_fixtures.py
+-rw-r--r--   0        0        0     1494 2024-06-03 12:38:31.314666 cg-60.9.3/tests/fixture_plugins/delivery_fixtures/path_fixtures.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.314666 cg-60.9.3/tests/fixture_plugins/demultiplex_fixtures/__init__.py
+-rw-r--r--   0        0        0     5237 2024-06-03 12:38:31.314666 cg-60.9.3/tests/fixture_plugins/demultiplex_fixtures/flow_cell_fixtures.py
+-rw-r--r--   0        0        0     3413 2024-06-03 12:38:31.314666 cg-60.9.3/tests/fixture_plugins/demultiplex_fixtures/name_fixtures.py
+-rw-r--r--   0        0        0    21023 2024-06-03 12:38:31.314666 cg-60.9.3/tests/fixture_plugins/demultiplex_fixtures/path_fixtures.py
+-rw-r--r--   0        0        0     3419 2024-06-03 12:38:31.314666 cg-60.9.3/tests/fixture_plugins/demultiplex_fixtures/run_parameters_fixtures.py
+-rw-r--r--   0        0        0     6014 2024-06-03 12:38:31.314666 cg-60.9.3/tests/fixture_plugins/demultiplex_fixtures/sample_fixtures.py
+-rw-r--r--   0        0        0     8960 2024-06-03 12:38:31.314666 cg-60.9.3/tests/fixture_plugins/demultiplex_fixtures/sample_sheet_fixtures.py
+-rw-r--r--   0        0        0     1768 2024-06-03 12:38:31.314666 cg-60.9.3/tests/fixture_plugins/loqusdb_fixtures/loqusdb_api_fixtures.py
+-rw-r--r--   0        0        0     6190 2024-06-03 12:38:31.314666 cg-60.9.3/tests/fixture_plugins/loqusdb_fixtures/loqusdb_output_fixtures.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.314666 cg-60.9.3/tests/fixture_plugins/observations_fixtures/__init__.py
+-rw-r--r--   0        0        0     2953 2024-06-03 12:38:31.314666 cg-60.9.3/tests/fixture_plugins/observations_fixtures/observations_api_fixtures.py
+-rw-r--r--   0        0        0     1512 2024-06-03 12:38:31.314666 cg-60.9.3/tests/fixture_plugins/observations_fixtures/observations_input_files_fixtures.py
+-rw-r--r--   0        0        0     3174 2024-06-03 12:38:31.314666 cg-60.9.3/tests/fixture_plugins/quality_controller_fixtures/sequencing_qc_check_scenario.py
+-rw-r--r--   0        0        0     4801 2024-06-03 12:38:31.314666 cg-60.9.3/tests/fixture_plugins/quality_controller_fixtures/sequencing_qc_fixtures.py
+-rw-r--r--   0        0        0     1304 2024-06-03 12:38:31.314666 cg-60.9.3/tests/fixture_plugins/timestamp_fixtures.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.314666 cg-60.9.3/tests/fixtures/analysis/balsamic/tn_wgs/adm1.cram
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.314666 cg-60.9.3/tests/fixtures/analysis/balsamic/tn_wgs/ascat.output.pdf
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.314666 cg-60.9.3/tests/fixtures/analysis/balsamic/tn_wgs/snv.vcf
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.314666 cg-60.9.3/tests/fixtures/analysis/balsamic/tn_wgs/sv.vcf
+-rw-r--r--   0        0        0    14644 2024-06-03 12:38:31.314666 cg-60.9.3/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json
+-rw-r--r--   0        0        0    15921 2024-06-03 12:38:31.314666 cg-60.9.3/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.314666 cg-60.9.3/tests/fixtures/analysis/mip/dna/ADM1.baf.bed.gz
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.314666 cg-60.9.3/tests/fixtures/analysis/mip/dna/ADM1.cov.bed.gz
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.314666 cg-60.9.3/tests/fixtures/analysis/mip/dna/ADM2.cram
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.314666 cg-60.9.3/tests/fixtures/analysis/mip/dna/ADM3.cram
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.314666 cg-60.9.3/tests/fixtures/analysis/mip/dna/adm1.cram
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.314666 cg-60.9.3/tests/fixtures/analysis/mip/dna/adm1.mt.bam
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.314666 cg-60.9.3/tests/fixtures/analysis/mip/dna/multiqc.html
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.314666 cg-60.9.3/tests/fixtures/analysis/mip/dna/report.pdf
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.314666 cg-60.9.3/tests/fixtures/analysis/mip/dna/smn.vcf
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.314666 cg-60.9.3/tests/fixtures/analysis/mip/dna/snv.vcf
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.314666 cg-60.9.3/tests/fixtures/analysis/mip/dna/snv_research.vcf
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.314666 cg-60.9.3/tests/fixtures/analysis/mip/dna/str.vcf
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.314666 cg-60.9.3/tests/fixtures/analysis/mip/dna/sv.vcf
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.314666 cg-60.9.3/tests/fixtures/analysis/mip/dna/sv_research.vcf
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.314666 cg-60.9.3/tests/fixtures/analysis/mip/dna/vcf2cytosure.txt
+-rw-r--r--   0        0        0       70 2024-06-03 12:38:31.314666 cg-60.9.3/tests/fixtures/analysis/nf-analysis/pipeline_params.config
+-rw-r--r--   0        0        0      195 2024-06-03 12:38:31.314666 cg-60.9.3/tests/fixtures/analysis/nf-analysis/pipeline_resource_optimisation.config
+-rw-r--r--   0        0        0      195 2024-06-03 12:38:31.314666 cg-60.9.3/tests/fixtures/analysis/nf-analysis/platform.config
+-rw-r--r--   0        0        0     8177 2024-06-03 12:38:31.314666 cg-60.9.3/tests/fixtures/analysis/raredisease/multiqc_data.json
+-rw-r--r--   0        0        0    20039 2024-06-03 12:38:31.314666 cg-60.9.3/tests/fixtures/analysis/raredisease/raredisease_case_enough_reads_metrics_deliverables.yaml
+-rw-r--r--   0        0        0     5497 2024-06-03 12:38:31.314666 cg-60.9.3/tests/fixtures/analysis/rnafusion/multiqc_data.json
+-rw-r--r--   0        0        0    12499 2024-06-03 12:38:31.314666 cg-60.9.3/tests/fixtures/analysis/rnafusion/rnafusion_case_enough_reads_metrics_deliverables.yaml
+-rw-r--r--   0        0        0     2873 2024-06-03 12:38:31.314666 cg-60.9.3/tests/fixtures/analysis/sample_coverage.bed
+-rw-r--r--   0        0        0     6506 2024-06-03 12:38:31.314666 cg-60.9.3/tests/fixtures/analysis/taxprofiler/multiqc_data.json
+-rw-r--r--   0        0        0    10513 2024-06-03 12:38:31.314666 cg-60.9.3/tests/fixtures/analysis/taxprofiler/taxprofiler_case_metrics_deliverables.yaml
+-rw-r--r--   0        0        0     5771 2024-06-03 12:38:31.314666 cg-60.9.3/tests/fixtures/analysis/tomte/multiqc_data.json
+-rw-r--r--   0        0        0    14859 2024-06-03 12:38:31.314666 cg-60.9.3/tests/fixtures/analysis/tomte/tomte_case_enough_reads_metrics_deliverables.yaml
+-rw-r--r--   0        0        0    10961 2024-06-03 12:38:31.314666 cg-60.9.3/tests/fixtures/apps/balsamic/case/config.json
+-rw-r--r--   0        0        0     3465 2024-06-03 12:38:31.314666 cg-60.9.3/tests/fixtures/apps/balsamic/case/metadata.yml
+-rw-r--r--   0        0        0       63 2024-06-03 12:38:31.314666 cg-60.9.3/tests/fixtures/apps/balsamic/case/metadata_directory.yml
+-rw-r--r--   0        0        0      165 2024-06-03 12:38:31.314666 cg-60.9.3/tests/fixtures/apps/balsamic/case/metadata_file_tags.yml
+-rw-r--r--   0        0        0     2705 2024-06-03 12:38:31.314666 cg-60.9.3/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml
+-rw-r--r--   0        0        0      692 2024-06-03 12:38:31.314666 cg-60.9.3/tests/fixtures/apps/crunchy/spring_metadata.json
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.318666 cg-60.9.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/ACC2655A1_S2_L002_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.318666 cg-60.9.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/ACC2655A1_S2_L002_R2_001.fastq.gz
+-rw-r--r--   0        0        0      412 2024-06-03 12:38:31.318666 cg-60.9.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/Reports/Adapter_Metrics.csv
+-rw-r--r--   0        0        0      484 2024-06-03 12:38:31.318666 cg-60.9.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/Reports/Demultiplex_Stats.csv
+-rw-r--r--   0        0        0      658 2024-06-03 12:38:31.318666 cg-60.9.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/Reports/Quality_Metrics.csv
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.318666 cg-60.9.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/SVE2648A1_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.318666 cg-60.9.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/SVE2648A1_S1_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.318666 cg-60.9.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/Undetermined_S0_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.318666 cg-60.9.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/Undetermined_S0_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.318666 cg-60.9.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/demuxcomplete.txt
+-rw-r--r--   0        0        0     1757 2024-06-03 12:38:31.318666 cg-60.9.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
+-rw-r--r--   0        0        0        7 2024-06-03 12:38:31.318666 cg-60.9.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.318666 cg-60.9.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.318666 cg-60.9.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0     6034 2024-06-03 12:38:31.318666 cg-60.9.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
+-rw-r--r--   0        0        0     1172 2024-06-03 12:38:31.318666 cg-60.9.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
+-rw-r--r--   0        0        0        7 2024-06-03 12:38:31.318666 cg-60.9.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/fastq_1.fastq.gz
+-rw-r--r--   0        0        0        7 2024-06-03 12:38:31.318666 cg-60.9.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/fastq_2.fastq.gz
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.318666 cg-60.9.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/BCLConvert/fastq/ACC13169A1_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.318666 cg-60.9.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/BCLConvert/fastq/ACC13169A1_S1_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.318666 cg-60.9.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/BCLConvert/fastq/ACC13170A6_S2_L002_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.318666 cg-60.9.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/BCLConvert/fastq/ACC13170A6_S2_L002_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.318666 cg-60.9.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/BCLConvert/fastq/Undetermined_S0_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.318666 cg-60.9.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/BCLConvert/fastq/Undetermined_S0_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0      288 2024-06-03 12:38:31.318666 cg-60.9.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/Reports/Adapter_Metrics.csv
+-rw-r--r--   0        0        0      361 2024-06-03 12:38:31.318666 cg-60.9.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/Reports/Demultiplex_Stats.csv
+-rw-r--r--   0        0        0      414 2024-06-03 12:38:31.318666 cg-60.9.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/Reports/Quality_Metrics.csv
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.318666 cg-60.9.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/demuxcomplete.txt
+-rw-r--r--   0        0        0    47757 2024-06-03 12:38:31.318666 cg-60.9.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/dragen-replay.json
+-rw-r--r--   0        0        0      315 2024-06-03 12:38:31.318666 cg-60.9.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRZZ/Unaligned/Reports/Adapter_Metrics.csv
+-rw-r--r--   0        0        0      434 2024-06-03 12:38:31.318666 cg-60.9.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRZZ/Unaligned/Reports/Quality_Metrics.csv
+-rw-r--r--   0        0        0     8624 2024-06-03 12:38:31.318666 cg-60.9.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRZZ/Unaligned/Reports/RunInfo.xml
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.318666 cg-60.9.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/ACC12642A4_S2_L002_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.318666 cg-60.9.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/ACC12642A4_S2_L002_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.318666 cg-60.9.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/ACC12642A7_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.318666 cg-60.9.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/ACC12642A7_S1_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0      303 2024-06-03 12:38:31.318666 cg-60.9.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/Reports/Adapter_Metrics.csv
+-rw-r--r--   0        0        0      364 2024-06-03 12:38:31.318666 cg-60.9.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/Reports/Demultiplex_Stats.csv
+-rw-r--r--   0        0        0      427 2024-06-03 12:38:31.318666 cg-60.9.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/Reports/Quality_Metrics.csv
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.318666 cg-60.9.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/Undetermined_S0_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.318666 cg-60.9.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/Undetermined_S0_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.318666 cg-60.9.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/demuxcomplete.txt
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.314666 cg-60.9.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.314666 cg-60.9.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0     4439 2024-06-03 12:38:31.318666 cg-60.9.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
+-rw-r--r--   0        0        0     1172 2024-06-03 12:38:31.318666 cg-60.9.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.318666 cg-60.9.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.318666 cg-60.9.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.318666 cg-60.9.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.318666 cg-60.9.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R2_001.fastq.gz
+-rw-r--r--   0        0        0     5127 2024-06-03 12:38:31.318666 cg-60.9.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/230912_A00187_1009_AHK33MDRX3/SampleSheet.csv
+-rw-r--r--   0        0        0       43 2024-06-03 12:38:31.318666 cg-60.9.3/tests/fixtures/apps/demultiplexing/fastq/dummy_run_R1_001.fastq.gz
+-rw-r--r--   0        0        0       67 2024-06-03 12:38:31.318666 cg-60.9.3/tests/fixtures/apps/demultiplexing/fastq/dummy_run_R1_001.fastq.gz.md5
+-rw-r--r--   0        0        0   338370 2024-06-03 12:38:31.318666 cg-60.9.3/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R1_001.fastq.gz
+-rw-r--r--   0        0        0       67 2024-06-03 12:38:31.318666 cg-60.9.3/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R1_001.fastq.gz.md5
+-rw-r--r--   0        0        0   338349 2024-06-03 12:38:31.318666 cg-60.9.3/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.318666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/CopyComplete.txt
+-rw-r--r--   0        0        0     2126 2024-06-03 12:38:31.318666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/HJCFFALXX_bcl2fastq_raw.json
+-rw-r--r--   0        0        0     1827 2024-06-03 12:38:31.318666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/HJCFFALXX_bcl_convert_raw.json
+-rw-r--r--   0        0        0       78 2024-06-03 12:38:31.318666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/README.txt
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.318666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTAComplete.txt
+-rw-r--r--   0        0        0     6895 2024-06-03 12:38:31.318666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTAConfiguration.xml
+-rw-r--r--   0        0        0       37 2024-06-03 12:38:31.318666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTARead1Complete.txt
+-rw-r--r--   0        0        0       36 2024-06-03 12:38:31.318666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTARead2Complete.txt
+-rw-r--r--   0        0        0       36 2024-06-03 12:38:31.318666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTARead3Complete.txt
+-rw-r--r--   0        0        0    24755 2024-06-03 12:38:31.322666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RunInfo.xml
+-rw-r--r--   0        0        0      692 2024-06-03 12:38:31.322666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet.csv
+-rw-r--r--   0        0        0      724 2024-06-03 12:38:31.322666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet_bcl2fastq.csv
+-rw-r--r--   0        0        0       61 2024-06-03 12:38:31.322666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SequencingComplete.txt
+-rw-r--r--   0        0        0     5775 2024-06-03 12:38:31.322666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/runParameters.xml
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.322666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/CopyComplete.txt
+-rw-r--r--   0        0        0     2282 2024-06-03 12:38:31.322666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/HL32LCCXY_bcl2fastq_raw.json
+-rw-r--r--   0        0        0     1632 2024-06-03 12:38:31.322666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/HL32LCCXY_bcl_convert_raw.json
+-rw-r--r--   0        0        0       76 2024-06-03 12:38:31.322666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/README.txt
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.322666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTAComplete.txt
+-rw-r--r--   0        0        0     6912 2024-06-03 12:38:31.322666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTAConfiguration.xml
+-rw-r--r--   0        0        0       36 2024-06-03 12:38:31.322666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTARead1Complete.txt
+-rw-r--r--   0        0        0       36 2024-06-03 12:38:31.322666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTARead2Complete.txt
+-rw-r--r--   0        0        0       36 2024-06-03 12:38:31.322666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTARead3Complete.txt
+-rw-r--r--   0        0        0       36 2024-06-03 12:38:31.322666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTARead4Complete.txt
+-rw-r--r--   0        0        0    24814 2024-06-03 12:38:31.322666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RunInfo.xml
+-rw-r--r--   0        0        0      814 2024-06-03 12:38:31.322666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SampleSheet.csv
+-rw-r--r--   0        0        0      660 2024-06-03 12:38:31.322666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SampleSheet_bcl2fastq.csv
+-rw-r--r--   0        0        0       61 2024-06-03 12:38:31.322666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SequencingComplete.txt
+-rw-r--r--   0        0        0     5853 2024-06-03 12:38:31.322666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/runParameters.xml
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.322666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/CopyComplete.txt
+-rw-r--r--   0        0        0    21848 2024-06-03 12:38:31.322666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/HGYFNBCX2_bcl2fastq_raw.json
+-rw-r--r--   0        0        0    15512 2024-06-03 12:38:31.322666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/HGYFNBCX2_bcl_convert_raw.json
+-rw-r--r--   0        0        0       79 2024-06-03 12:38:31.322666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/README.txt
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.322666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/RTAComplete.txt
+-rw-r--r--   0        0        0      756 2024-06-03 12:38:31.322666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/RunInfo.xml
+-rw-r--r--   0        0        0     4118 2024-06-03 12:38:31.322666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/SampleSheet.csv
+-rw-r--r--   0        0        0     1408 2024-06-03 12:38:31.322666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/SampleSheet_bcl2fastq.csv
+-rw-r--r--   0        0        0     5326 2024-06-03 12:38:31.322666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/runParameters.xml
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.322666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/CopyComplete.txt
+-rw-r--r--   0        0        0    15041 2024-06-03 12:38:31.322666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/HM2LNBCX2_bcl2fastq_raw.json
+-rw-r--r--   0        0        0    10649 2024-06-03 12:38:31.322666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/HM2LNBCX2_bcl_convert_raw.json
+-rw-r--r--   0        0        0       81 2024-06-03 12:38:31.322666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/README.txt
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.322666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/RTAComplete.txt
+-rw-r--r--   0        0        0      755 2024-06-03 12:38:31.322666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/RunInfo.xml
+-rw-r--r--   0        0        0     2878 2024-06-03 12:38:31.322666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/SampleSheet.csv
+-rw-r--r--   0        0        0      928 2024-06-03 12:38:31.322666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/SampleSheet_bcl2fastq.csv
+-rw-r--r--   0        0        0     5359 2024-06-03 12:38:31.322666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/runParameters.xml
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.322666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/CopyComplete.txt
+-rw-r--r--   0        0        0    27887 2024-06-03 12:38:31.322666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/CorrectSampleSheet.csv
+-rw-r--r--   0        0        0   141870 2024-06-03 12:38:31.322666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/HLYWYDSXX_bcl2fastq_raw.json
+-rwxr-xr-x   0        0        0   122682 2024-06-03 12:38:31.322666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/HLYWYDSXX_bcl_convert_raw.json
+-rw-r--r--   0        0        0      243 2024-06-03 12:38:31.322666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/README.txt
+-rw-r--r--   0        0        0    28230 2024-06-03 12:38:31.322666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RTA3.cfg
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.322666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RTAComplete.txt
+-rw-r--r--   0        0        0    94426 2024-06-03 12:38:31.322666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RunInfo.xml
+-rw-r--r--   0        0        0     5819 2024-06-03 12:38:31.322666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RunParameters.xml
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.322666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/SequenceComplete.txt
+-rw-r--r--   0        0        0     1757 2024-06-03 12:38:31.322666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
+-rw-r--r--   0        0        0     1757 2024-06-03 12:38:31.322666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stdout
+-rw-r--r--   0        0        0    47522 2024-06-03 12:38:31.322666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_raw.json
+-rw-r--r--   0        0        0       12 2024-06-03 12:38:31.322666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/README.txt
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.322666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/RTAComplete.txt
+-rw-r--r--   0        0        0     6666 2024-06-03 12:38:31.322666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/RunParameters.xml
+-rw-r--r--   0        0        0      254 2024-06-03 12:38:31.322666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.322666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/copycomplete.txt
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.322666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/delivery.txt
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.322666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/demuxstarted.txt
+-rwxr-xr-x   0        0        0    47434 2024-06-03 12:38:31.322666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/22F52TLT3_raw.json
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.322666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/CopyComplete.txt
+-rw-r--r--   0        0        0    10950 2024-06-03 12:38:31.322666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/CorrectSampleSheet.csv
+-rw-r--r--   0        0        0      225 2024-06-03 12:38:31.322666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/Manifest.tsv
+-rw-r--r--   0        0        0       55 2024-06-03 12:38:31.322666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/README.txt
+-rwxr-xr-x   0        0        0     2493 2024-06-03 12:38:31.322666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RTA.cfg
+-rwxr-xr-x   0        0        0        1 2024-06-03 12:38:31.322666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RTAComplete.txt
+-rwxr-xr-x   0        0        0        2 2024-06-03 12:38:31.322666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RTAExited.txt
+-rwxr-xr-x   0        0        0      730 2024-06-03 12:38:31.322666 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunCompletionStatus.xml
+-rwxr-xr-x   0        0        0    79277 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunInfo.xml
+-rwxr-xr-x   0        0        0     2694 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunParameters.xml
+-rw-r--r--   0        0        0    10950 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/CopyComplete.txt
+-rw-r--r--   0        0        0      509 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stderr
+-rw-r--r--   0        0        0     2229 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stdout
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/RTAComplete.txt
+-rw-r--r--   0        0        0     6665 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/RunParameters.xml
+-rw-r--r--   0        0        0      619 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/CopyComplete.txt
+-rw-r--r--   0        0        0     4941 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/CorrectSampleSheet.csv
+-rwxr-xr-x   0        0        0    20050 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/HK33MDRX3_bcl_convert_raw.json
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/HK33MDRX3_demultiplex.stderr
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/HK33MDRX3_demultiplex.stdout
+-rw-r--r--   0        0        0      244 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/README.txt
+-rw-r--r--   0        0        0     6391 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RTA3.cfg
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RTAComplete.txt
+-rw-r--r--   0        0        0    16428 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RunInfo.xml
+-rw-r--r--   0        0        0     6728 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RunParameters.xml
+-rw-r--r--   0        0        0     5127 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/SequenceComplete.txt
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/demuxstarted.txt
+-rw-r--r--   0        0        0      133 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells_broken/170517_ST-E00266_0210_BHJCFFALXX/README.txt
+-rw-r--r--   0        0        0      724 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells_broken/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet.csv
+-rw-r--r--   0        0        0     5775 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells_broken/170517_ST-E00266_0210_BHJCFFALXX/runParameters.xml
+-rw-r--r--   0        0        0      124 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells_broken/180509_D00450_0598_BHGYFNBCX2/README.txt
+-rw-r--r--   0        0        0      310 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells_broken/190927_A00689_0069_BHLYWYDSXX/README.txt
+-rw-r--r--   0        0        0     5819 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells_broken/190927_A00689_0069_BHLYWYDSXX/RunParameters.xml
+-rw-r--r--   0        0        0      122 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells_broken/20231108_LH00188_0028_B22F52TLT3/README.txt
+-rwxr-xr-x   0        0        0     2694 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells_broken/20231108_LH00188_0028_B22F52TLT3/RunParameters.xml
+-rw-r--r--   0        0        0      311 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells_broken/230912_A00187_1009_AHK33MDRX3/README.txt
+-rw-r--r--   0        0        0     6728 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells_broken/230912_A00187_1009_AHK33MDRX3/RunParameters.xml
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/CopyComplete.txt
+-rw-r--r--   0        0        0      509 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stderr
+-rw-r--r--   0        0        0     2229 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/RTAComplete.txt
+-rw-r--r--   0        0        0     6665 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml
+-rw-r--r--   0        0        0      399 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/CopyComplete.txt
+-rw-r--r--   0        0        0      509 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stderr
+-rw-r--r--   0        0        0     2229 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stdout
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/RTAComplete.txt
+-rw-r--r--   0        0        0     6665 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/RunParameters.xml
+-rw-r--r--   0        0        0      399 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/fastq_pass/PAS86456_pass_72d9fceb_8a4fd683_0.fastq.gz
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/fastq_pass/PAS86456_pass_72d9fceb_8a4fd683_1.fastq.gz
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/final_summary_PAS86456_72d9fceb_8a4fd683.txt
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/pod5_pass/PAS86456_pass_72d9fceb_8a4fd683_0.pod5
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/pod5_pass/PAS86456_pass_72d9fceb_8a4fd683_1.pod5
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/fastq_pass/PAS97781_pass_595b5663_efc7f02e_0.fastq.gz
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/fastq_pass/PAS97781_pass_595b5663_efc7f02e_1.fastq.gz
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/final_summary_PAS97781_595b5663_efc7f02e.txt
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/pod5_pass/PAS97781_pass_595b5663_efc7f02e_0.pod5
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/pod5_pass/PAS97781_pass_595b5663_efc7f02e_1.pod5
+-rw-r--r--   0        0        0     5319 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_hiseq_2500_different_index_cycles.xml
+-rw-r--r--   0        0        0     5944 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_6000_different_index_cycles.xml
+-rwxr-xr-x   0        0        0     2603 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_different_index_cycles.xml
+-rwxr-xr-x   0        0        0     2597 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_wrong_instrument.xml
+-rw-r--r--   0        0        0     5899 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_no_software_nor_reagent_version.xml
+-rw-r--r--   0        0        0     4941 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/demultiplexing/sample_sheets/novaseq_6000_sample_sheet_with_reversed_cycles.csv
+-rw-r--r--   0        0        0    10950 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/demultiplexing/sample_sheets/novaseq_x_sample_sheet_with_forward_cycles.csv
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/demultiplexing/spring/dummy_run_001.spring
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/demultiplexing/spring/dummy_run_002.spring
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/demultiplexing/spring/dummy_spring_meta_data.json
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/fluffy/2020-23219-05/2020-23219-05.WCXpredict_aberrations.filt.bed
+-rw-r--r--   0        0        0     5554 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/fluffy/SampleSheet.csv
+-rw-r--r--   0        0        0      901 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/fluffy/deliverables.yaml
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/fluffy/fluffy_fastq.fastq.gz
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/fluffy/multiqc_report.html
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/fluffy/summary.csv
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/gt/yellowhog.bcf
+-rw-r--r--   0        0        0     5114 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/madeline/madeline.xml
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/mip/case_file.txt
+-rw-r--r--   0        0        0     3241 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/mip/case_metrics_deliverables.yaml
+-rw-r--r--   0        0        0    21811 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/mip/dna/store/case_config.yaml
+-rw-r--r--   0        0        0    23364 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml
+-rw-r--r--   0        0        0    37367 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml
+-rw-r--r--   0        0        0       16 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/mip/dna/store/empty_case_config.yaml
+-rw-r--r--   0        0        0       16 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/mip/dna/store/empty_case_metrics_deliverables.yaml
+-rw-r--r--   0        0        0       16 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/mip/dna/store/empty_case_qc_sample_info.yaml
+-rw-r--r--   0        0        0      123 2024-06-03 12:38:31.326665 cg-60.9.3/tests/fixtures/apps/mip/dna/store/empty_delivery_report.html
+-rw-r--r--   0        0        0    62741 2024-06-03 12:38:31.330666 cg-60.9.3/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf
+-rw-r--r--   0        0        0    11242 2024-06-03 12:38:31.330666 cg-60.9.3/tests/fixtures/apps/mip/rna/case_config.yaml
+-rw-r--r--   0        0        0    12164 2024-06-03 12:38:31.330666 cg-60.9.3/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml
+-rw-r--r--   0        0        0     5231 2024-06-03 12:38:31.330666 cg-60.9.3/tests/fixtures/apps/mip/rna/store/bundle_data.yaml
+-rw-r--r--   0        0        0     9774 2024-06-03 12:38:31.330666 cg-60.9.3/tests/fixtures/apps/mip/rna/store/case_config.yaml
+-rw-r--r--   0        0        0     4624 2024-06-03 12:38:31.330666 cg-60.9.3/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml
+-rw-r--r--   0        0        0    13666 2024-06-03 12:38:31.330666 cg-60.9.3/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.330666 cg-60.9.3/tests/fixtures/apps/mip/sample_file.txt
+-rw-r--r--   0        0        0     1885 2024-06-03 12:38:31.330666 cg-60.9.3/tests/fixtures/apps/scout/643594.config.yaml
+-rw-r--r--   0        0        0     6027 2024-06-03 12:38:31.330666 cg-60.9.3/tests/fixtures/apps/scout/case_export.json
+-rw-r--r--   0        0        0     9349 2024-06-03 12:38:31.330666 cg-60.9.3/tests/fixtures/apps/scout/export_causatives.json
+-rw-r--r--   0        0        0     1315 2024-06-03 12:38:31.330666 cg-60.9.3/tests/fixtures/apps/scout/none_case_export.json
+-rw-r--r--   0        0        0     3518 2024-06-03 12:38:31.330666 cg-60.9.3/tests/fixtures/apps/scout/other_sex_case.json
+-rw-r--r--   0        0        0     8874 2024-06-03 12:38:31.330666 cg-60.9.3/tests/fixtures/apps/scout/panel_export.bed
+-rw-r--r--   0        0        0     4169 2024-06-03 12:38:31.330666 cg-60.9.3/tests/fixtures/apps/scout/panel_export.csv
+-rw-r--r--   0        0        0       42 2024-06-03 12:38:31.330666 cg-60.9.3/tests/fixtures/apps/shipping/scout-deploy.yaml
+-rw-r--r--   0        0        0     1036 2024-06-03 12:38:31.330666 cg-60.9.3/tests/fixtures/cgweb_orders/balsamic.json
+-rw-r--r--   0        0        0     1104 2024-06-03 12:38:31.330666 cg-60.9.3/tests/fixtures/cgweb_orders/fastq.json
+-rw-r--r--   0        0        0     1313 2024-06-03 12:38:31.330666 cg-60.9.3/tests/fixtures/cgweb_orders/metagenome.json
+-rw-r--r--   0        0        0     3038 2024-06-03 12:38:31.330666 cg-60.9.3/tests/fixtures/cgweb_orders/microsalt.json
+-rw-r--r--   0        0        0     3705 2024-06-03 12:38:31.330666 cg-60.9.3/tests/fixtures/cgweb_orders/mip.json
+-rw-r--r--   0        0        0     1364 2024-06-03 12:38:31.330666 cg-60.9.3/tests/fixtures/cgweb_orders/mip_rna.json
+-rw-r--r--   0        0        0     2125 2024-06-03 12:38:31.330666 cg-60.9.3/tests/fixtures/cgweb_orders/rml.json
+-rw-r--r--   0        0        0     1368 2024-06-03 12:38:31.330666 cg-60.9.3/tests/fixtures/cgweb_orders/rnafusion.json
+-rw-r--r--   0        0        0     4684 2024-06-03 12:38:31.330666 cg-60.9.3/tests/fixtures/cgweb_orders/sarscov2.json
+-rw-r--r--   0        0        0     3811 2024-06-03 12:38:31.330666 cg-60.9.3/tests/fixtures/cgweb_orders/tomte.json
+-rw-r--r--   0        0        0     5609 2024-06-03 12:38:31.330666 cg-60.9.3/tests/fixtures/data/SampleSheet.csv
+-rw-r--r--   0        0        0      511 2024-06-03 12:38:31.330666 cg-60.9.3/tests/fixtures/data/bcl_convert_sample_sheet.csv
+-rw-r--r--   0        0        0   258048 2024-06-03 12:38:31.330666 cg-60.9.3/tests/fixtures/data/cgfixture.db
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.330666 cg-60.9.3/tests/fixtures/data/fastq.fastq.gz
+-rw-r--r--   0        0        0    49152 2024-06-03 12:38:31.330666 cg-60.9.3/tests/fixtures/data/hkstore.db
+-rw-r--r--   0        0        0       73 2024-06-03 12:38:31.330666 cg-60.9.3/tests/fixtures/data/yellowhog/pedigree.yaml
+-rw-r--r--   0        0        0       76 2024-06-03 12:38:31.330666 cg-60.9.3/tests/fixtures/io/casava_five_parts.fastq.gz
+-rw-r--r--   0        0        0       90 2024-06-03 12:38:31.330666 cg-60.9.3/tests/fixtures/io/casava_seven_parts.fastq.gz
+-rw-r--r--   0        0        0       96 2024-06-03 12:38:31.330666 cg-60.9.3/tests/fixtures/io/casava_ten_parts.fastq.gz
+-rw-r--r--   0        0        0      153 2024-06-03 12:38:31.330666 cg-60.9.3/tests/fixtures/io/example.csv
+-rw-r--r--   0        0        0       46 2024-06-03 12:38:31.330666 cg-60.9.3/tests/fixtures/io/example.gz
+-rw-r--r--   0        0        0      147 2024-06-03 12:38:31.330666 cg-60.9.3/tests/fixtures/io/example.tsv
+-rw-r--r--   0        0        0       20 2024-06-03 12:38:31.330666 cg-60.9.3/tests/fixtures/io/example.txt
+-rw-r--r--   0        0        0       20 2024-06-03 12:38:31.330666 cg-60.9.3/tests/fixtures/io/example2.txt
+-rw-r--r--   0        0        0      582 2024-06-03 12:38:31.330666 cg-60.9.3/tests/fixtures/io/example_json.json
+-rw-r--r--   0        0        0      103 2024-06-03 12:38:31.334666 cg-60.9.3/tests/fixtures/io/example_xml.xml
+-rw-r--r--   0        0        0       20 2024-06-03 12:38:31.334666 cg-60.9.3/tests/fixtures/meta/qc_metrics/file_with_right_tags.json
+-rw-r--r--   0        0        0       20 2024-06-03 12:38:31.334666 cg-60.9.3/tests/fixtures/meta/qc_metrics/file_without_right_tags.json
+-rw-r--r--   0        0        0   258670 2024-06-03 12:38:31.334666 cg-60.9.3/tests/fixtures/orderforms/1508.31.balsamic.xlsx
+-rw-r--r--   0        0        0   258572 2024-06-03 12:38:31.334666 cg-60.9.3/tests/fixtures/orderforms/1508.31.balsamic_qc.xlsx
+-rw-r--r--   0        0        0   258081 2024-06-03 12:38:31.334666 cg-60.9.3/tests/fixtures/orderforms/1508.31.balsamic_umi.xlsx
+-rw-r--r--   0        0        0   258109 2024-06-03 12:38:31.338666 cg-60.9.3/tests/fixtures/orderforms/1508.31.fastq.xlsx
+-rw-r--r--   0        0        0   256330 2024-06-03 12:38:31.338666 cg-60.9.3/tests/fixtures/orderforms/1508.31.metagenome.xlsx
+-rw-r--r--   0        0        0   258966 2024-06-03 12:38:31.338666 cg-60.9.3/tests/fixtures/orderforms/1508.31.mip.xlsx
+-rw-r--r--   0        0        0   258987 2024-06-03 12:38:31.338666 cg-60.9.3/tests/fixtures/orderforms/1508.31.mip_rna.xlsx
+-rw-r--r--   0        0        0   258708 2024-06-03 12:38:31.338666 cg-60.9.3/tests/fixtures/orderforms/1508.31.rnafusion.xlsx
+-rw-r--r--   0        0        0   258603 2024-06-03 12:38:31.338666 cg-60.9.3/tests/fixtures/orderforms/1508.31.tomte.xlsx
+-rw-r--r--   0        0        0    82677 2024-06-03 12:38:31.342666 cg-60.9.3/tests/fixtures/orderforms/1603.11.microbial.xlsx
+-rw-r--r--   0        0        0   149394 2024-06-03 12:38:31.342666 cg-60.9.3/tests/fixtures/orderforms/1604.17.rml.xlsx
+-rw-r--r--   0        0        0   223184 2024-06-03 12:38:31.342666 cg-60.9.3/tests/fixtures/orderforms/2184.9.sarscov2.xlsx
+-rw-r--r--   0        0        0    18639 2024-06-03 12:38:31.342666 cg-60.9.3/tests/fixtures/orderforms/NIPT-json.json
+-rw-r--r--   0        0        0     6052 2024-06-03 12:38:31.342666 cg-60.9.3/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json
+-rw-r--r--   0        0        0     6611 2024-06-03 12:38:31.342666 cg-60.9.3/tests/fixtures/orderforms/mip_uploaded_json_orderform.json
+-rw-r--r--   0        0        0     1417 2024-06-03 12:38:31.342666 cg-60.9.3/tests/fixtures/report/case_data.json
+-rw-r--r--   0        0        0     1109 2024-06-03 12:38:31.342666 cg-60.9.3/tests/fixtures/report/lims_exported_samples.json
+-rw-r--r--   0        0        0     1562 2024-06-03 12:38:31.342666 cg-60.9.3/tests/fixtures/report/lims_family.json
+-rw-r--r--   0        0        0      619 2024-06-03 12:38:31.342666 cg-60.9.3/tests/fixtures/services/illumina_metrics_service/230622_A00621_0864_AHY7FFDRX2/SampleSheet.csv
+-rw-r--r--   0        0        0     2554 2024-06-03 12:38:31.342666 cg-60.9.3/tests/fixtures/services/illumina_metrics_service/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Adapter_Metrics.csv
+-rw-r--r--   0        0        0     2016 2024-06-03 12:38:31.342666 cg-60.9.3/tests/fixtures/services/illumina_metrics_service/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Demultiplex_Stats.csv
+-rw-r--r--   0        0        0     3607 2024-06-03 12:38:31.342666 cg-60.9.3/tests/fixtures/services/illumina_metrics_service/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Quality_Metrics.csv
+-rw-r--r--   0        0        0      248 2024-06-03 12:38:31.342666 cg-60.9.3/tests/fixtures/services/validate_file_transfer_service/pacbio_transfer_done
+-rw-r--r--   0        0        0      279 2024-06-03 12:38:31.342666 cg-60.9.3/tests/fixtures/services/validate_file_transfer_service/pacbio_transfer_done_fail
+-rw-r--r--   0        0        0     3296 2024-06-03 12:38:31.342666 cg-60.9.3/tests/io/conftest.py
+-rw-r--r--   0        0        0      431 2024-06-03 12:38:31.342666 cg-60.9.3/tests/io/test_io_config.py
+-rw-r--r--   0        0        0     8639 2024-06-03 12:38:31.342666 cg-60.9.3/tests/io/test_io_controller.py
+-rw-r--r--   0        0        0     3877 2024-06-03 12:38:31.342666 cg-60.9.3/tests/io/test_io_csv.py
+-rw-r--r--   0        0        0      482 2024-06-03 12:38:31.342666 cg-60.9.3/tests/io/test_io_gzip.py
+-rw-r--r--   0        0        0     1779 2024-06-03 12:38:31.342666 cg-60.9.3/tests/io/test_io_json.py
+-rw-r--r--   0        0        0     2914 2024-06-03 12:38:31.342666 cg-60.9.3/tests/io/test_io_txt.py
+-rw-r--r--   0        0        0     1027 2024-06-03 12:38:31.342666 cg-60.9.3/tests/io/test_io_xml.py
+-rw-r--r--   0        0        0     2131 2024-06-03 12:38:31.342666 cg-60.9.3/tests/io/test_io_yaml.py
+-rw-r--r--   0        0        0     1233 2024-06-03 12:38:31.342666 cg-60.9.3/tests/io/test_validate_path.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.342666 cg-60.9.3/tests/meta/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.342666 cg-60.9.3/tests/meta/archive/__init__.py
+-rw-r--r--   0        0        0    13482 2024-06-03 12:38:31.342666 cg-60.9.3/tests/meta/archive/conftest.py
+-rw-r--r--   0        0        0    20911 2024-06-03 12:38:31.342666 cg-60.9.3/tests/meta/archive/test_archive_api.py
+-rw-r--r--   0        0        0    10246 2024-06-03 12:38:31.342666 cg-60.9.3/tests/meta/archive/test_archive_cli.py
+-rw-r--r--   0        0        0    15766 2024-06-03 12:38:31.342666 cg-60.9.3/tests/meta/archive/test_archiving.py
+-rw-r--r--   0        0        0     3809 2024-06-03 12:38:31.342666 cg-60.9.3/tests/meta/backup/conftest.py
+-rw-r--r--   0        0        0    26401 2024-06-03 12:38:31.342666 cg-60.9.3/tests/meta/backup/test_meta_backup.py
+-rw-r--r--   0        0        0    10055 2024-06-03 12:38:31.342666 cg-60.9.3/tests/meta/backup/test_meta_pdc.py
+-rw-r--r--   0        0        0    12617 2024-06-03 12:38:31.342666 cg-60.9.3/tests/meta/clean/conftest.py
+-rw-r--r--   0        0        0    16944 2024-06-03 12:38:31.342666 cg-60.9.3/tests/meta/clean/test_clean_flow_cells_api.py
+-rw-r--r--   0        0        0     2286 2024-06-03 12:38:31.342666 cg-60.9.3/tests/meta/clean/test_clean_retrieved_spring_files.py
+-rw-r--r--   0        0        0     7691 2024-06-03 12:38:31.342666 cg-60.9.3/tests/meta/compress/conftest.py
+-rw-r--r--   0        0        0     7961 2024-06-03 12:38:31.342666 cg-60.9.3/tests/meta/compress/test_clean_fastq.py
+-rw-r--r--   0        0        0     1778 2024-06-03 12:38:31.342666 cg-60.9.3/tests/meta/compress/test_compress_files.py
+-rw-r--r--   0        0        0     3644 2024-06-03 12:38:31.342666 cg-60.9.3/tests/meta/compress/test_compress_meta_fastq.py
+-rw-r--r--   0        0        0     1180 2024-06-03 12:38:31.342666 cg-60.9.3/tests/meta/compress/test_decompress_spring_meta.py
+-rw-r--r--   0        0        0     7045 2024-06-03 12:38:31.342666 cg-60.9.3/tests/meta/compress/test_meta_compress_update_hk.py
+-rw-r--r--   0        0        0     8269 2024-06-03 12:38:31.342666 cg-60.9.3/tests/meta/conftest.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.342666 cg-60.9.3/tests/meta/deliver/__init__.py
+-rw-r--r--   0        0        0     3525 2024-06-03 12:38:31.342666 cg-60.9.3/tests/meta/deliver/conftest.py
+-rw-r--r--   0        0        0     5533 2024-06-03 12:38:31.342666 cg-60.9.3/tests/meta/deliver/test_deliver_ticket.py
+-rw-r--r--   0        0        0    10331 2024-06-03 12:38:31.342666 cg-60.9.3/tests/meta/deliver/test_delivery_api.py
+-rw-r--r--   0        0        0     1057 2024-06-03 12:38:31.342666 cg-60.9.3/tests/meta/deliver/test_fastq_path_generator.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.346666 cg-60.9.3/tests/meta/delivery/__init__.py
+-rw-r--r--   0        0        0    16660 2024-06-03 12:38:31.346666 cg-60.9.3/tests/meta/delivery/test_delivery_api.py
+-rw-r--r--   0        0        0     8066 2024-06-03 12:38:31.346666 cg-60.9.3/tests/meta/demultiplex/conftest.py
+-rw-r--r--   0        0        0     5382 2024-06-03 12:38:31.346666 cg-60.9.3/tests/meta/demultiplex/test_combine_sequencing_metrics.py
+-rw-r--r--   0        0        0     8691 2024-06-03 12:38:31.346666 cg-60.9.3/tests/meta/demultiplex/test_demux_post_processing.py
+-rw-r--r--   0        0        0    13775 2024-06-03 12:38:31.346666 cg-60.9.3/tests/meta/demultiplex/test_housekeeper_storage_functions.py
+-rw-r--r--   0        0        0     4392 2024-06-03 12:38:31.346666 cg-60.9.3/tests/meta/demultiplex/test_status_db_storage_functions.py
+-rw-r--r--   0        0        0    22819 2024-06-03 12:38:31.346666 cg-60.9.3/tests/meta/demultiplex/test_utils.py
+-rw-r--r--   0        0        0     6343 2024-06-03 12:38:31.346666 cg-60.9.3/tests/meta/demultiplex/test_validation.py
+-rw-r--r--   0        0        0     4943 2024-06-03 12:38:31.346666 cg-60.9.3/tests/meta/encryption/conftest.py
+-rw-r--r--   0        0        0    18252 2024-06-03 12:38:31.346666 cg-60.9.3/tests/meta/encryption/test_encryption.py
+-rw-r--r--   0        0        0     7289 2024-06-03 12:38:31.346666 cg-60.9.3/tests/meta/observations/test_balsamic_observations_api.py
+-rw-r--r--   0        0        0     6177 2024-06-03 12:38:31.346666 cg-60.9.3/tests/meta/observations/test_mip_dna_observations_api.py
+-rw-r--r--   0        0        0    18356 2024-06-03 12:38:31.346666 cg-60.9.3/tests/meta/observations/test_observations_api.py
+-rw-r--r--   0        0        0     5345 2024-06-03 12:38:31.346666 cg-60.9.3/tests/meta/orders/conftest.py
+-rw-r--r--   0        0        0     1749 2024-06-03 12:38:31.346666 cg-60.9.3/tests/meta/orders/test_PoolSubmitter_validate_order.py
+-rw-r--r--   0        0        0     1470 2024-06-03 12:38:31.346666 cg-60.9.3/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py
+-rw-r--r--   0        0        0     1768 2024-06-03 12:38:31.346666 cg-60.9.3/tests/meta/orders/test_SarsCov2Submitter_store_order.py
+-rw-r--r--   0        0        0     2032 2024-06-03 12:38:31.346666 cg-60.9.3/tests/meta/orders/test_SarsCov2Submitter_validate_order.py
+-rw-r--r--   0        0        0    19783 2024-06-03 12:38:31.346666 cg-60.9.3/tests/meta/orders/test_meta_orders_api.py
+-rw-r--r--   0        0        0     7086 2024-06-03 12:38:31.346666 cg-60.9.3/tests/meta/orders/test_meta_orders_lims.py
+-rw-r--r--   0        0        0    28893 2024-06-03 12:38:31.346666 cg-60.9.3/tests/meta/orders/test_meta_orders_status.py
+-rw-r--r--   0        0        0     1677 2024-06-03 12:38:31.346666 cg-60.9.3/tests/meta/orders/test_rnafusion_submitter.py
+-rw-r--r--   0        0        0     1068 2024-06-03 12:38:31.346666 cg-60.9.3/tests/meta/orders/test_ticket_handler.py
+-rw-r--r--   0        0        0     4336 2024-06-03 12:38:31.346666 cg-60.9.3/tests/meta/qc_metrics/conftest.py
+-rw-r--r--   0        0        0     1972 2024-06-03 12:38:31.346666 cg-60.9.3/tests/meta/qc_metrics/test_collect_qc_metrics.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.346666 cg-60.9.3/tests/meta/report/__init__.py
+-rw-r--r--   0        0        0     6512 2024-06-03 12:38:31.346666 cg-60.9.3/tests/meta/report/conftest.py
+-rw-r--r--   0        0        0      434 2024-06-03 12:38:31.346666 cg-60.9.3/tests/meta/report/helper.py
+-rw-r--r--   0        0        0     2604 2024-06-03 12:38:31.346666 cg-60.9.3/tests/meta/report/test_balsamic_api.py
+-rw-r--r--   0        0        0     4056 2024-06-03 12:38:31.346666 cg-60.9.3/tests/meta/report/test_field_validators.py
+-rw-r--r--   0        0        0     2858 2024-06-03 12:38:31.346666 cg-60.9.3/tests/meta/report/test_mip_dna_api.py
+-rw-r--r--   0        0        0    16042 2024-06-03 12:38:31.346666 cg-60.9.3/tests/meta/report/test_report_api.py
+-rw-r--r--   0        0        0     3123 2024-06-03 12:38:31.346666 cg-60.9.3/tests/meta/report/test_rnafusion_api.py
+-rw-r--r--   0        0        0     1250 2024-06-03 12:38:31.346666 cg-60.9.3/tests/meta/report/test_tomte_api.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.346666 cg-60.9.3/tests/meta/rsync/__init__.py
+-rw-r--r--   0        0        0      916 2024-06-03 12:38:31.346666 cg-60.9.3/tests/meta/rsync/conftest.py
+-rw-r--r--   0        0        0     9442 2024-06-03 12:38:31.346666 cg-60.9.3/tests/meta/rsync/test_rsync.py
+-rw-r--r--   0        0        0     3147 2024-06-03 12:38:31.346666 cg-60.9.3/tests/meta/test_invoice.py
+-rw-r--r--   0        0        0     1220 2024-06-03 12:38:31.346666 cg-60.9.3/tests/meta/transfer/conftest.py
+-rw-r--r--   0        0        0    10552 2024-06-03 12:38:31.346666 cg-60.9.3/tests/meta/transfer/test_external_data.py
+-rw-r--r--   0        0        0     4395 2024-06-03 12:38:31.346666 cg-60.9.3/tests/meta/transfer/test_meta_transfer_lims.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.346666 cg-60.9.3/tests/meta/upload/__init__.py
+-rw-r--r--   0        0        0     2210 2024-06-03 12:38:31.346666 cg-60.9.3/tests/meta/upload/balsamic/test_balsamic.py
+-rw-r--r--   0        0        0     4002 2024-06-03 12:38:31.346666 cg-60.9.3/tests/meta/upload/conftest.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.346666 cg-60.9.3/tests/meta/upload/gisaid/__init__.py
+-rw-r--r--   0        0        0     2557 2024-06-03 12:38:31.346666 cg-60.9.3/tests/meta/upload/gisaid/fixtures/four_samples.csv
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.346666 cg-60.9.3/tests/meta/upload/gisaid/fixtures/invalid_housekeeper.fasta
+-rw-r--r--   0        0        0      211 2024-06-03 12:38:31.346666 cg-60.9.3/tests/meta/upload/gisaid/fixtures/valid_gisaid.fasta
+-rw-r--r--   0        0        0      371 2024-06-03 12:38:31.346666 cg-60.9.3/tests/meta/upload/gisaid/fixtures/valid_housekeeper.fasta
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.346666 cg-60.9.3/tests/meta/upload/mutacc/__init__.py
+-rw-r--r--   0        0        0     3684 2024-06-03 12:38:31.346666 cg-60.9.3/tests/meta/upload/mutacc/conftest.py
+-rw-r--r--   0        0        0     4188 2024-06-03 12:38:31.346666 cg-60.9.3/tests/meta/upload/mutacc/test_meta_upload_mutacc.py
+-rw-r--r--   0        0        0     1149 2024-06-03 12:38:31.346666 cg-60.9.3/tests/meta/upload/nipt/conftest.py
+-rw-r--r--   0        0        0     1683 2024-06-03 12:38:31.346666 cg-60.9.3/tests/meta/upload/nipt/test_models.py
+-rw-r--r--   0        0        0     1242 2024-06-03 12:38:31.346666 cg-60.9.3/tests/meta/upload/nipt/test_nipt_upload_api.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.346666 cg-60.9.3/tests/meta/upload/scout/__init__.py
+-rw-r--r--   0        0        0    23954 2024-06-03 12:38:31.346666 cg-60.9.3/tests/meta/upload/scout/conftest.py
+-rw-r--r--   0        0        0     4734 2024-06-03 12:38:31.346666 cg-60.9.3/tests/meta/upload/scout/test_generate_load_config.py
+-rw-r--r--   0        0        0     4182 2024-06-03 12:38:31.346666 cg-60.9.3/tests/meta/upload/scout/test_meta_upload_scoutapi.py
+-rw-r--r--   0        0        0    33260 2024-06-03 12:38:31.346666 cg-60.9.3/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py
+-rw-r--r--   0        0        0     7372 2024-06-03 12:38:31.346666 cg-60.9.3/tests/meta/upload/scout/test_scout_config_builder.py
+-rw-r--r--   0        0        0     2511 2024-06-03 12:38:31.346666 cg-60.9.3/tests/meta/upload/test_meta_upload_coverage.py
+-rw-r--r--   0        0        0     1473 2024-06-03 12:38:31.346666 cg-60.9.3/tests/meta/upload/test_upload_api.py
+-rw-r--r--   0        0        0     2547 2024-06-03 12:38:31.346666 cg-60.9.3/tests/meta/upload/test_upload_genotypes_api.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.346666 cg-60.9.3/tests/meta/workflow/__init__.py
+-rw-r--r--   0        0        0    10262 2024-06-03 12:38:31.346666 cg-60.9.3/tests/meta/workflow/conftest.py
+-rw-r--r--   0        0        0     3679 2024-06-03 12:38:31.346666 cg-60.9.3/tests/meta/workflow/microsalt/conftest.py
+-rw-r--r--   0        0        0      318 2024-06-03 12:38:31.346666 cg-60.9.3/tests/meta/workflow/microsalt/test_parsing_metrics.py
+-rw-r--r--   0        0        0     3759 2024-06-03 12:38:31.350666 cg-60.9.3/tests/meta/workflow/microsalt/test_quality_controller.py
+-rw-r--r--   0        0        0    14367 2024-06-03 12:38:31.350666 cg-60.9.3/tests/meta/workflow/microsalt/test_quality_controller_utils.py
+-rw-r--r--   0        0        0      825 2024-06-03 12:38:31.350666 cg-60.9.3/tests/meta/workflow/microsalt/test_report_generation.py
+-rw-r--r--   0        0        0    20894 2024-06-03 12:38:31.350666 cg-60.9.3/tests/meta/workflow/test_analysis.py
+-rw-r--r--   0        0        0     7934 2024-06-03 12:38:31.350666 cg-60.9.3/tests/meta/workflow/test_balsamic.py
+-rw-r--r--   0        0        0     3034 2024-06-03 12:38:31.350666 cg-60.9.3/tests/meta/workflow/test_fastq.py
+-rw-r--r--   0        0        0     1532 2024-06-03 12:38:31.350666 cg-60.9.3/tests/meta/workflow/test_microsalt.py
+-rw-r--r--   0        0        0     2721 2024-06-03 12:38:31.350666 cg-60.9.3/tests/meta/workflow/test_nf_analysis.py
+-rw-r--r--   0        0        0     7741 2024-06-03 12:38:31.350666 cg-60.9.3/tests/meta/workflow/test_prepare_fastq_api.py
+-rw-r--r--   0        0        0     2095 2024-06-03 12:38:31.350666 cg-60.9.3/tests/meta/workflow/test_raredisease.py
+-rw-r--r--   0        0        0     1674 2024-06-03 12:38:31.350666 cg-60.9.3/tests/meta/workflow/test_rnafusion.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.350666 cg-60.9.3/tests/mocks/__init__.py
+-rw-r--r--   0        0        0     1168 2024-06-03 12:38:31.350666 cg-60.9.3/tests/mocks/balsamic_analysis_mock.py
+-rw-r--r--   0        0        0     3500 2024-06-03 12:38:31.350666 cg-60.9.3/tests/mocks/crunchy.py
+-rw-r--r--   0        0        0    21787 2024-06-03 12:38:31.350666 cg-60.9.3/tests/mocks/hk_mock.py
+-rw-r--r--   0        0        0     4215 2024-06-03 12:38:31.350666 cg-60.9.3/tests/mocks/limsmock.py
+-rw-r--r--   0        0        0      572 2024-06-03 12:38:31.350666 cg-60.9.3/tests/mocks/madeline.py
+-rw-r--r--   0        0        0     1297 2024-06-03 12:38:31.350666 cg-60.9.3/tests/mocks/mip_analysis_mock.py
+-rw-r--r--   0        0        0     1525 2024-06-03 12:38:31.350666 cg-60.9.3/tests/mocks/osticket.py
+-rw-r--r--   0        0        0     3239 2024-06-03 12:38:31.350666 cg-60.9.3/tests/mocks/process_mock.py
+-rw-r--r--   0        0        0     4713 2024-06-03 12:38:31.350666 cg-60.9.3/tests/mocks/report.py
+-rw-r--r--   0        0        0     3915 2024-06-03 12:38:31.350666 cg-60.9.3/tests/mocks/scout.py
+-rw-r--r--   0        0        0      750 2024-06-03 12:38:31.350666 cg-60.9.3/tests/mocks/store_model.py
+-rw-r--r--   0        0        0     1620 2024-06-03 12:38:31.350666 cg-60.9.3/tests/mocks/tb_mock.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.350666 cg-60.9.3/tests/models/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.350666 cg-60.9.3/tests/models/balsamic/__init__.py
+-rw-r--r--   0        0        0     1194 2024-06-03 12:38:31.350666 cg-60.9.3/tests/models/balsamic/conftest.py
+-rw-r--r--   0        0        0     1030 2024-06-03 12:38:31.350666 cg-60.9.3/tests/models/balsamic/test_balsamic_analysis.py
+-rw-r--r--   0        0        0     1050 2024-06-03 12:38:31.350666 cg-60.9.3/tests/models/conftest.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.350666 cg-60.9.3/tests/models/demultiplexing/__init__.py
+-rw-r--r--   0        0        0    12705 2024-06-03 12:38:31.350666 cg-60.9.3/tests/models/demultiplexing/test_run_parameters.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.350666 cg-60.9.3/tests/models/downsample/__init__.py
+-rw-r--r--   0        0        0     2096 2024-06-03 12:38:31.350666 cg-60.9.3/tests/models/downsample/test_down_sample_meta_data.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.350666 cg-60.9.3/tests/models/flow_cell/__init__.py
+-rw-r--r--   0        0        0     7871 2024-06-03 12:38:31.350666 cg-60.9.3/tests/models/flow_cell/test_flowcell_model.py
+-rw-r--r--   0        0        0     6637 2024-06-03 12:38:31.350666 cg-60.9.3/tests/models/mip/conftest.py
+-rw-r--r--   0        0        0     1239 2024-06-03 12:38:31.350666 cg-60.9.3/tests/models/mip/test_mip_analysis.py
+-rw-r--r--   0        0        0     2348 2024-06-03 12:38:31.350666 cg-60.9.3/tests/models/mip/test_mip_config.py
+-rw-r--r--   0        0        0     6392 2024-06-03 12:38:31.350666 cg-60.9.3/tests/models/mip/test_mip_metrics_deliverables.py
+-rw-r--r--   0        0        0     3959 2024-06-03 12:38:31.350666 cg-60.9.3/tests/models/mip/test_mip_sample_info.py
+-rw-r--r--   0        0        0     3314 2024-06-03 12:38:31.350666 cg-60.9.3/tests/models/nextflow/test_nextflow_deliver.py
+-rw-r--r--   0        0        0     2663 2024-06-03 12:38:31.350666 cg-60.9.3/tests/models/observations/test_observations_input_files.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.350666 cg-60.9.3/tests/models/report/__init__.py
+-rw-r--r--   0        0        0     7879 2024-06-03 12:38:31.350666 cg-60.9.3/tests/models/report/test_validators.py
+-rw-r--r--   0        0        0     3855 2024-06-03 12:38:31.350666 cg-60.9.3/tests/models/rnafusion/test_rnafusion_sample.py
+-rw-r--r--   0        0        0     1374 2024-06-03 12:38:31.350666 cg-60.9.3/tests/models/test_cg_models.py
+-rw-r--r--   0        0        0      990 2024-06-03 12:38:31.350666 cg-60.9.3/tests/models/test_compression_data.py
+-rw-r--r--   0        0        0      729 2024-06-03 12:38:31.350666 cg-60.9.3/tests/models/test_fastq.py
+-rw-r--r--   0        0        0     2860 2024-06-03 12:38:31.350666 cg-60.9.3/tests/models/test_file_data.py
+-rw-r--r--   0        0        0     5094 2024-06-03 12:38:31.350666 cg-60.9.3/tests/server/conftest.py
+-rw-r--r--   0        0        0     3135 2024-06-03 12:38:31.350666 cg-60.9.3/tests/server/endpoints/test_delivery_message_endpoint.py
+-rw-r--r--   0        0        0     3239 2024-06-03 12:38:31.350666 cg-60.9.3/tests/server/endpoints/test_orders_endpoint.py
+-rw-r--r--   0        0        0      271 2024-06-03 12:38:31.350666 cg-60.9.3/tests/server/test_server_auto.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.350666 cg-60.9.3/tests/services/__init__.py
+-rw-r--r--   0        0        0     1092 2024-06-03 12:38:31.350666 cg-60.9.3/tests/services/fastq_file_service/conftest.py
+-rw-r--r--   0        0        0     3712 2024-06-03 12:38:31.350666 cg-60.9.3/tests/services/fastq_file_service/test_fastq_file_service.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.350666 cg-60.9.3/tests/services/illumina_services/__init__.py
+-rw-r--r--   0        0        0      738 2024-06-03 12:38:31.350666 cg-60.9.3/tests/services/illumina_services/illumina_demux_version_service/conftest.py
+-rw-r--r--   0        0        0     1344 2024-06-03 12:38:31.350666 cg-60.9.3/tests/services/illumina_services/illumina_demux_version_service/test_illumina_demux_version_service.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.350666 cg-60.9.3/tests/services/illumina_services/illumina_metrics_service/__init__.py
+-rw-r--r--   0        0        0     4020 2024-06-03 12:38:31.350666 cg-60.9.3/tests/services/illumina_services/illumina_metrics_service/conftest.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.350666 cg-60.9.3/tests/services/illumina_services/illumina_metrics_service/parsers/__init__.py
+-rw-r--r--   0        0        0    10501 2024-06-03 12:38:31.350666 cg-60.9.3/tests/services/illumina_services/illumina_metrics_service/parsers/test_bclconvert_metrics_parser.py
+-rw-r--r--   0        0        0     3291 2024-06-03 12:38:31.350666 cg-60.9.3/tests/services/illumina_services/illumina_metrics_service/parsers/test_illumina_metrics_service.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.350666 cg-60.9.3/tests/services/illumina_services/illumina_post_processing_service/__init__.py
+-rw-r--r--   0        0        0     1464 2024-06-03 12:38:31.350666 cg-60.9.3/tests/services/illumina_services/illumina_post_processing_service/conftest.py
+-rw-r--r--   0        0        0     4476 2024-06-03 12:38:31.350666 cg-60.9.3/tests/services/illumina_services/illumina_post_processing_service/test_illumina_post_processing_service.py
+-rw-r--r--   0        0        0     4862 2024-06-03 12:38:31.350666 cg-60.9.3/tests/services/orders/order_status_service/conftest.py
+-rw-r--r--   0        0        0     2876 2024-06-03 12:38:31.350666 cg-60.9.3/tests/services/orders/order_status_service/test_order_summary_service.py
+-rw-r--r--   0        0        0      748 2024-06-03 12:38:31.350666 cg-60.9.3/tests/services/parse_completion_status_service/conftest.py
+-rw-r--r--   0        0        0     1249 2024-06-03 12:38:31.350666 cg-60.9.3/tests/services/parse_completion_status_service/test_parse_completion_status_service.py
+-rw-r--r--   0        0        0     9598 2024-06-03 12:38:31.350666 cg-60.9.3/tests/services/sequencing_qc_service/test_sequencing_quality_checks_utils.py
+-rw-r--r--   0        0        0     3427 2024-06-03 12:38:31.350666 cg-60.9.3/tests/services/validate_file_transfer_service/conftest.py
+-rw-r--r--   0        0        0     4258 2024-06-03 12:38:31.350666 cg-60.9.3/tests/services/validate_file_transfer_service/test_validate_file_transfer_service.py
+-rw-r--r--   0        0        0     2952 2024-06-03 12:38:31.350666 cg-60.9.3/tests/services/validate_file_transfer_service/test_validate_pacbio_file_transfer_service.py
+-rw-r--r--   0        0        0      318 2024-06-03 12:38:31.350666 cg-60.9.3/tests/small_helpers.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.350666 cg-60.9.3/tests/store/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.350666 cg-60.9.3/tests/store/api/__init__.py
+-rw-r--r--   0        0        0     3032 2024-06-03 12:38:31.350666 cg-60.9.3/tests/store/api/conftest.py
+-rw-r--r--   0        0        0     1557 2024-06-03 12:38:31.354666 cg-60.9.3/tests/store/api/test_base.py
+-rw-r--r--   0        0        0    21033 2024-06-03 12:38:31.354666 cg-60.9.3/tests/store/conftest.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.354666 cg-60.9.3/tests/store/crud/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.354666 cg-60.9.3/tests/store/crud/add/__init__.py
+-rw-r--r--   0        0        0     1497 2024-06-03 12:38:31.354666 cg-60.9.3/tests/store/crud/add/test_store_add_application_version.py
+-rw-r--r--   0        0        0     5254 2024-06-03 12:38:31.354666 cg-60.9.3/tests/store/crud/add/test_store_add_base.py
+-rw-r--r--   0        0        0     2502 2024-06-03 12:38:31.354666 cg-60.9.3/tests/store/crud/add/test_store_add_customer.py
+-rw-r--r--   0        0        0     1704 2024-06-03 12:38:31.354666 cg-60.9.3/tests/store/crud/add/test_store_add_flow_celll.py
+-rw-r--r--   0        0        0    12288 2024-06-03 12:38:31.354666 cg-60.9.3/tests/store/crud/conftest.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.354666 cg-60.9.3/tests/store/crud/delete/__init__.py
+-rw-r--r--   0        0        0     5611 2024-06-03 12:38:31.354666 cg-60.9.3/tests/store/crud/delete/test_delete.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.354666 cg-60.9.3/tests/store/crud/read/__init__.py
+-rw-r--r--   0        0        0    56073 2024-06-03 12:38:31.354666 cg-60.9.3/tests/store/crud/read/test_read.py
+-rw-r--r--   0        0        0     5461 2024-06-03 12:38:31.354666 cg-60.9.3/tests/store/crud/read/test_read_analyses_to_clean.py
+-rw-r--r--   0        0        0     3553 2024-06-03 12:38:31.354666 cg-60.9.3/tests/store/crud/read/test_read_analyses_to_delivery_report.py
+-rw-r--r--   0        0        0    17328 2024-06-03 12:38:31.354666 cg-60.9.3/tests/store/crud/read/test_read_analysis.py
+-rw-r--r--   0        0        0     2743 2024-06-03 12:38:31.354666 cg-60.9.3/tests/store/crud/read/test_read_application_version.py
+-rw-r--r--   0        0        0     1105 2024-06-03 12:38:31.354666 cg-60.9.3/tests/store/crud/read/test_read_customer.py
+-rw-r--r--   0        0        0      732 2024-06-03 12:38:31.354666 cg-60.9.3/tests/store/crud/read/test_read_illumina_flow_cell.py
+-rw-r--r--   0        0        0     1530 2024-06-03 12:38:31.354666 cg-60.9.3/tests/store/crud/read/test_read_pool.py
+-rw-r--r--   0        0        0    21503 2024-06-03 12:38:31.354666 cg-60.9.3/tests/store/crud/read/test_read_sample.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.354666 cg-60.9.3/tests/store/crud/update/__init__.py
+-rw-r--r--   0        0        0      737 2024-06-03 12:38:31.354666 cg-60.9.3/tests/store/crud/update/test_update.py
+-rw-r--r--   0        0        0    11693 2024-06-03 12:38:31.354666 cg-60.9.3/tests/store/filters/test_status_analyses_filters.py
+-rw-r--r--   0        0        0     3397 2024-06-03 12:38:31.354666 cg-60.9.3/tests/store/filters/test_status_application_filters.py
+-rw-r--r--   0        0        0     2073 2024-06-03 12:38:31.354666 cg-60.9.3/tests/store/filters/test_status_application_limitations_filters.py
+-rw-r--r--   0        0        0    10452 2024-06-03 12:38:31.354666 cg-60.9.3/tests/store/filters/test_status_application_version_filters.py
+-rw-r--r--   0        0        0     2804 2024-06-03 12:38:31.354666 cg-60.9.3/tests/store/filters/test_status_bed_filters.py
+-rw-r--r--   0        0        0     2362 2024-06-03 12:38:31.354666 cg-60.9.3/tests/store/filters/test_status_bed_version_filters.py
+-rw-r--r--   0        0        0     3495 2024-06-03 12:38:31.354666 cg-60.9.3/tests/store/filters/test_status_case_sample_filters.py
+-rw-r--r--   0        0        0    39100 2024-06-03 12:38:31.354666 cg-60.9.3/tests/store/filters/test_status_cases_filters.py
+-rw-r--r--   0        0        0     1345 2024-06-03 12:38:31.354666 cg-60.9.3/tests/store/filters/test_status_collaboration_filters.py
+-rw-r--r--   0        0        0     2482 2024-06-03 12:38:31.354666 cg-60.9.3/tests/store/filters/test_status_customer_filters.py
+-rw-r--r--   0        0        0     5153 2024-06-03 12:38:31.354666 cg-60.9.3/tests/store/filters/test_status_flow_cell_filters.py
+-rw-r--r--   0        0        0     1095 2024-06-03 12:38:31.354666 cg-60.9.3/tests/store/filters/test_status_illumina_flow_cell_filters.py
+-rw-r--r--   0        0        0     2226 2024-06-03 12:38:31.354666 cg-60.9.3/tests/store/filters/test_status_invoice_filters.py
+-rw-r--r--   0        0        0     5871 2024-06-03 12:38:31.354666 cg-60.9.3/tests/store/filters/test_status_metrics_filters.py
+-rw-r--r--   0        0        0     2404 2024-06-03 12:38:31.354666 cg-60.9.3/tests/store/filters/test_status_organism_filters.py
+-rw-r--r--   0        0        0     1804 2024-06-03 12:38:31.354666 cg-60.9.3/tests/store/filters/test_status_panel_filters.py
+-rw-r--r--   0        0        0     8720 2024-06-03 12:38:31.354666 cg-60.9.3/tests/store/filters/test_status_pool_filters.py
+-rw-r--r--   0        0        0    22875 2024-06-03 12:38:31.354666 cg-60.9.3/tests/store/filters/test_status_samples_filters.py
+-rw-r--r--   0        0        0     1576 2024-06-03 12:38:31.354666 cg-60.9.3/tests/store/filters/test_status_user_filters.py
+-rw-r--r--   0        0        0     2147 2024-06-03 12:38:31.354666 cg-60.9.3/tests/store/test_delivery.py
+-rw-r--r--   0        0        0     4127 2024-06-03 12:38:31.354666 cg-60.9.3/tests/store/test_store_models.py
+-rw-r--r--   0        0        0    37125 2024-06-03 12:38:31.354666 cg-60.9.3/tests/store_helpers.py
+-rw-r--r--   0        0        0     4988 2024-06-03 12:38:31.354666 cg-60.9.3/tests/test_copy_novaseqx_flow_cell.py
+-rw-r--r--   0        0        0      911 2024-06-03 12:38:31.354666 cg-60.9.3/tests/test_store_helpers.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:38:31.354666 cg-60.9.3/tests/utils/__init__.py
+-rw-r--r--   0        0        0     1749 2024-06-03 12:38:31.354666 cg-60.9.3/tests/utils/conftest.py
+-rw-r--r--   0        0        0      371 2024-06-03 12:38:31.354666 cg-60.9.3/tests/utils/test_calculations.py
+-rw-r--r--   0        0        0     1906 2024-06-03 12:38:31.354666 cg-60.9.3/tests/utils/test_checksum.py
+-rw-r--r--   0        0        0     2920 2024-06-03 12:38:31.354666 cg-60.9.3/tests/utils/test_commands.py
+-rw-r--r--   0        0        0      953 2024-06-03 12:38:31.354666 cg-60.9.3/tests/utils/test_date.py
+-rw-r--r--   0        0        0     1508 2024-06-03 12:38:31.354666 cg-60.9.3/tests/utils/test_dict.py
+-rw-r--r--   0        0        0     7154 2024-06-03 12:38:31.354666 cg-60.9.3/tests/utils/test_dispatcher.py
+-rw-r--r--   0        0        0     5204 2024-06-03 12:38:31.354666 cg-60.9.3/tests/utils/test_files.py
+-rw-r--r--   0        0        0     2052 2024-06-03 12:38:31.354666 cg-60.9.3/tests/utils/test_time.py
+-rw-r--r--   0        0        0     2752 2024-06-03 12:38:31.354666 cg-60.9.3/tests/utils/test_utils.py
+-rw-r--r--   0        0        0     4369 1970-01-01 00:00:00.000000 cg-60.9.3/PKG-INFO
```

### Comparing `cg-60.9.1/README.md` & `cg-60.9.3/README.md`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/apps/coverage/api.py` & `cg-60.9.3/cg/apps/coverage/api.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/apps/crunchy/crunchy.py` & `cg-60.9.3/cg/apps/crunchy/crunchy.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/apps/crunchy/files.py` & `cg-60.9.3/cg/apps/crunchy/files.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/apps/crunchy/sbatch.py` & `cg-60.9.3/cg/apps/crunchy/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/apps/demultiplex/demultiplex_api.py` & `cg-60.9.3/cg/apps/demultiplex/demultiplex_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from cg.constants.constants import FileFormat, Workflow
 from cg.constants.demultiplexing import DemultiplexingDirsAndFiles
 from cg.constants.priority import SlurmQos
 from cg.constants.tb import AnalysisTypes
 from cg.exc import HousekeeperFileMissingError
 from cg.io.controller import WriteFile
 from cg.models.demultiplex.sbatch import SbatchCommand, SbatchError
-from cg.models.flow_cell.flow_cell import FlowCellDirectoryData
+from cg.models.run_devices.illumina_run_directory_data import IlluminaRunDirectoryData
 from cg.models.slurm.sbatch import SbatchDragen
 
 LOG = logging.getLogger(__name__)
 
 
 class DemultiplexingAPI:
     """Demultiplexing API should deal with anything related to demultiplexing.
@@ -51,15 +51,15 @@
         """Set dry run."""
         LOG.debug(f"DemultiplexingAPI: Set dry run to {dry_run}")
         self.dry_run = dry_run
         self.slurm_api.set_dry_run(dry_run=dry_run)
 
     @staticmethod
     def get_sbatch_error(
-        flow_cell: FlowCellDirectoryData,
+        flow_cell: IlluminaRunDirectoryData,
         email: str,
         demux_dir: Path,
     ) -> str:
         """Create the sbatch error string."""
         LOG.debug("Creating the sbatch error string")
         error_parameters: SbatchError = SbatchError(
             flow_cell_id=flow_cell.id,
@@ -91,71 +91,71 @@
             sample_sheet=sample_sheet.as_posix(),
             demux_completed_file=demux_completed.as_posix(),
             environment=environment,
         )
         return DEMULTIPLEX_COMMAND.format(**command_parameters.model_dump())
 
     @staticmethod
-    def demultiplex_sbatch_path(flow_cell: FlowCellDirectoryData) -> Path:
+    def demultiplex_sbatch_path(flow_cell: IlluminaRunDirectoryData) -> Path:
         """Get the path to where sbatch script file should be kept."""
         return Path(flow_cell.path, "demux-novaseq.sh")
 
     @staticmethod
-    def get_run_name(flow_cell: FlowCellDirectoryData) -> str:
+    def get_run_name(flow_cell: IlluminaRunDirectoryData) -> str:
         """Create the run name for the sbatch job."""
         return f"{flow_cell.id}_demultiplex"
 
     @staticmethod
-    def get_stderr_logfile(flow_cell: FlowCellDirectoryData) -> Path:
+    def get_stderr_logfile(flow_cell: IlluminaRunDirectoryData) -> Path:
         """Create the path to the stderr logfile."""
         return Path(flow_cell.path, f"{DemultiplexingAPI.get_run_name(flow_cell)}.stderr")
 
     @staticmethod
-    def get_stdout_logfile(flow_cell: FlowCellDirectoryData) -> Path:
+    def get_stdout_logfile(flow_cell: IlluminaRunDirectoryData) -> Path:
         """Create the path to the stdout logfile."""
         return Path(flow_cell.path, f"{DemultiplexingAPI.get_run_name(flow_cell)}.stdout")
 
-    def flow_cell_out_dir_path(self, flow_cell: FlowCellDirectoryData) -> Path:
+    def flow_cell_out_dir_path(self, flow_cell: IlluminaRunDirectoryData) -> Path:
         """Create the path to where the demultiplexed result should be produced."""
         return Path(self.demultiplexed_runs_dir, flow_cell.path.name)
 
     def is_sample_sheet_in_housekeeper(self, flow_cell_id: str) -> bool:
         """Returns True if the sample sheet for the flow cell exists in Housekeeper."""
         try:
             self.hk_api.get_sample_sheet_path(flow_cell_id)
             return True
         except HousekeeperFileMissingError:
             return False
 
-    def get_flow_cell_unaligned_dir(self, flow_cell: FlowCellDirectoryData) -> Path:
+    def get_flow_cell_unaligned_dir(self, flow_cell: IlluminaRunDirectoryData) -> Path:
         """Returns the path to where the demultiplexed result are located."""
         return Path(
             self.flow_cell_out_dir_path(flow_cell), DemultiplexingDirsAndFiles.UNALIGNED_DIR_NAME
         )
 
-    def demultiplexing_completed_path(self, flow_cell: FlowCellDirectoryData) -> Path:
+    def demultiplexing_completed_path(self, flow_cell: IlluminaRunDirectoryData) -> Path:
         """Return the path to demultiplexing complete file."""
         LOG.info(
             Path(self.flow_cell_out_dir_path(flow_cell), DemultiplexingDirsAndFiles.DEMUX_COMPLETE)
         )
         return Path(
             self.flow_cell_out_dir_path(flow_cell), DemultiplexingDirsAndFiles.DEMUX_COMPLETE
         )
 
-    def is_demultiplexing_possible(self, flow_cell: FlowCellDirectoryData) -> bool:
+    def is_demultiplexing_possible(self, flow_cell: IlluminaRunDirectoryData) -> bool:
         """Check if it is possible to start demultiplexing.
 
         This means that
             - flow cell should be ready for demultiplexing (all files in place)
             - sample sheet needs to exist
             - demultiplexing should not be running
         """
         LOG.info(f"Check if demultiplexing is possible for {flow_cell.id}")
         demultiplexing_possible = True
-        if not flow_cell.is_flow_cell_ready():
+        if not flow_cell.is_sequencing_run_ready():
             demultiplexing_possible = False
 
         if not flow_cell.sample_sheet_exists():
             LOG.warning(f"Could not find sample sheet in flow cell directory for {flow_cell.id}")
             demultiplexing_possible = False
 
         if not self.is_sample_sheet_in_housekeeper(flow_cell_id=flow_cell.id):
@@ -186,15 +186,15 @@
         """Write the content to a yaml file"""
         LOG.info(f"Writing yaml content {content} to {file_path}")
         WriteFile.write_file_from_content(
             content=content, file_format=FileFormat.YAML, file_path=file_path
         )
 
     def add_to_trailblazer(
-        self, tb_api: TrailblazerAPI, slurm_job_id: int, flow_cell: FlowCellDirectoryData
+        self, tb_api: TrailblazerAPI, slurm_job_id: int, flow_cell: IlluminaRunDirectoryData
     ):
         """Add demultiplexing entry to trailblazer."""
         if self.dry_run:
             return
         self.write_trailblazer_config(
             content=self.get_trailblazer_config(slurm_job_id=slurm_job_id),
             file_path=flow_cell.trailblazer_config_path,
@@ -205,15 +205,15 @@
             config_path=flow_cell.trailblazer_config_path.as_posix(),
             out_dir=flow_cell.trailblazer_config_path.parent.as_posix(),
             slurm_quality_of_service=self.slurm_quality_of_service,
             email=self.mail,
             workflow=Workflow.DEMULTIPLEX,
         )
 
-    def start_demultiplexing(self, flow_cell: FlowCellDirectoryData):
+    def start_demultiplexing(self, flow_cell: IlluminaRunDirectoryData):
         """Start demultiplexing for a flow cell."""
         self.create_demultiplexing_started_file(flow_cell.demultiplexing_started_path)
         log_path: Path = self.get_stderr_logfile(flow_cell=flow_cell)
         error_function: str = self.get_sbatch_error(
             flow_cell=flow_cell, email=self.mail, demux_dir=self.flow_cell_out_dir_path(flow_cell)
         )
         commands: str = self.get_sbatch_command(
@@ -239,21 +239,21 @@
         sbatch_path: Path = self.demultiplex_sbatch_path(flow_cell=flow_cell)
         sbatch_number: int = self.slurm_api.submit_sbatch(
             sbatch_content=sbatch_content, sbatch_path=sbatch_path
         )
         LOG.info(f"Demultiplexing running as job {sbatch_number}")
         return sbatch_number
 
-    def prepare_output_directory(self, flow_cell: FlowCellDirectoryData) -> None:
+    def prepare_output_directory(self, flow_cell: IlluminaRunDirectoryData) -> None:
         """Makes sure the output directory is ready for demultiplexing."""
         self.remove_demultiplexing_output_directory(flow_cell)
         self.create_demultiplexing_output_dir(flow_cell)
 
-    def remove_demultiplexing_output_directory(self, flow_cell: FlowCellDirectoryData) -> None:
+    def remove_demultiplexing_output_directory(self, flow_cell: IlluminaRunDirectoryData) -> None:
         if not self.dry_run and self.flow_cell_out_dir_path(flow_cell=flow_cell).exists():
             shutil.rmtree(self.flow_cell_out_dir_path(flow_cell=flow_cell), ignore_errors=False)
 
-    def create_demultiplexing_output_dir(self, flow_cell: FlowCellDirectoryData) -> None:
+    def create_demultiplexing_output_dir(self, flow_cell: IlluminaRunDirectoryData) -> None:
         """Creates the demultiplexing output directory for the flow cell."""
         output_directory: Path = self.flow_cell_out_dir_path(flow_cell)
         LOG.debug(f"Creating demultiplexing output directory: {output_directory}")
         output_directory.mkdir(exist_ok=False, parents=True)
```

### Comparing `cg-60.9.1/cg/apps/demultiplex/sample_sheet/api.py` & `cg-60.9.3/cg/apps/demultiplex/sample_sheet/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from cg.constants.demultiplexing import SampleSheetBcl2FastqSections, SampleSheetBCLConvertSections
 from cg.exc import FlowCellError, HousekeeperFileMissingError, SampleSheetError
 from cg.io.controller import ReadFile, WriteFile, WriteStream
 from cg.meta.demultiplex.housekeeper_storage_functions import (
     add_and_include_sample_sheet_path_to_housekeeper,
     delete_sample_sheet_from_housekeeper,
 )
-from cg.models.flow_cell.flow_cell import FlowCellDirectoryData
+from cg.models.run_devices.illumina_run_directory_data import IlluminaRunDirectoryData
 from cg.utils.files import get_directories_in_path, link_or_overwrite_file
 
 LOG = logging.getLogger(__name__)
 
 
 class SampleSheetAPI:
     """Sample Sheet API class."""
@@ -41,27 +41,27 @@
         self.dry_run = dry_run
 
     def set_force(self, force: bool) -> None:
         """Set force."""
         LOG.debug(f"Set force to {force}")
         self.force = force
 
-    def _get_flow_cell(self, flow_cell_name: str) -> FlowCellDirectoryData:
+    def _get_flow_cell(self, flow_cell_name: str) -> IlluminaRunDirectoryData:
         """
         Return a flow cell given a path.
         Raises:
             SampleSheetError: If the flow cell directory or the data it contains is not valid.
         """
         flow_cell_path: Path = Path(self.flow_cell_runs_dir, flow_cell_name)
         if not flow_cell_path.exists():
             message: str = f"Could not find flow cell {flow_cell_path}"
             LOG.warning(message)
             raise SampleSheetError(message)
         try:
-            flow_cell = FlowCellDirectoryData(flow_cell_path)
+            flow_cell = IlluminaRunDirectoryData(flow_cell_path)
         except FlowCellError as error:
             raise SampleSheetError from error
         return flow_cell
 
     def validate_sample_sheet(self, sample_sheet_path: Path) -> None:
         """Return the sample sheet path if it exists and if it passes validation.
         Raises:
@@ -73,15 +73,15 @@
             raise SampleSheetError(message)
         sample_sheet_content: list[list[str]] = ReadFile.get_content_from_file(
             file_format=FileFormat.CSV, file_path=sample_sheet_path
         )
         self.validator.validate_sample_sheet_from_content(sample_sheet_content)
 
     @staticmethod
-    def _are_necessary_files_in_flow_cell(flow_cell: FlowCellDirectoryData) -> bool:
+    def _are_necessary_files_in_flow_cell(flow_cell: IlluminaRunDirectoryData) -> bool:
         """Determine if the flow cell has a Run Parameters file and a sample sheet."""
         try:
             flow_cell.run_parameters_path.exists()
         except FlowCellError:
             LOG.error(f"Run parameters file for flow cell {flow_cell.full_name} does not exist")
             return False
         if not flow_cell.sample_sheet_path.exists():
@@ -104,15 +104,15 @@
                 )
                 line[idx] = SampleSheetBCLConvertSections.Data.SAMPLE_INTERNAL_ID.value
                 return sample_sheet_content
         raise SampleSheetError("Could not find BCL2FASTQ data header in sample sheet")
 
     def translate_sample_sheet(self, flow_cell_name: str) -> None:
         """Translate a Bcl2Fastq sample sheet to a BCLConvert sample sheet."""
-        flow_cell: FlowCellDirectoryData = self._get_flow_cell(flow_cell_name)
+        flow_cell: IlluminaRunDirectoryData = self._get_flow_cell(flow_cell_name)
         if not self._are_necessary_files_in_flow_cell(flow_cell):
             raise SampleSheetError("Could not translate sample sheet")
         original_content: list[list[str]] = ReadFile.get_content_from_file(
             file_format=FileFormat.CSV, file_path=flow_cell.sample_sheet_path
         )
         content_with_fixed_header: list[list[str]] = self._replace_sample_header(original_content)
 
@@ -133,45 +133,45 @@
             return
         WriteFile.write_file_from_content(
             content=new_content,
             file_format=FileFormat.CSV,
             file_path=flow_cell.sample_sheet_path,
         )
 
-    def _use_sample_sheet_from_housekeeper(self, flow_cell: FlowCellDirectoryData) -> None:
+    def _use_sample_sheet_from_housekeeper(self, flow_cell: IlluminaRunDirectoryData) -> None:
         """
         Copy the sample sheet from Housekeeper to the flow cell directory if it exists and is valid.
         """
         try:
             sample_sheet_path: Path = self.hk_api.get_sample_sheet_path(flow_cell.id)
         except HousekeeperFileMissingError:
             raise SampleSheetError(
                 f"Sample sheet for flow cell {flow_cell.id} does not exist in Housekeeper"
             )
         self.validate_sample_sheet(sample_sheet_path)
         LOG.info("Sample sheet from Housekeeper is valid. Copying it to flow cell directory")
         if not self.dry_run:
             link_or_overwrite_file(src=sample_sheet_path, dst=flow_cell.sample_sheet_path)
 
-    def _use_flow_cell_sample_sheet(self, flow_cell: FlowCellDirectoryData) -> None:
+    def _use_flow_cell_sample_sheet(self, flow_cell: IlluminaRunDirectoryData) -> None:
         """Use the sample sheet from the flow cell directory if it is valid."""
         self.validate_sample_sheet(flow_cell.sample_sheet_path)
         LOG.info("Sample sheet from flow cell directory is valid. Adding it to Housekeeper")
         if not self.dry_run:
             try:
                 delete_sample_sheet_from_housekeeper(flow_cell_id=flow_cell.id, hk_api=self.hk_api)
             except HousekeeperFileMissingError:
                 pass
             add_and_include_sample_sheet_path_to_housekeeper(
                 flow_cell_directory=flow_cell.path,
                 flow_cell_name=flow_cell.id,
                 hk_api=self.hk_api,
             )
 
-    def _get_sample_sheet_content(self, flow_cell: FlowCellDirectoryData) -> list[list[str]]:
+    def _get_sample_sheet_content(self, flow_cell: IlluminaRunDirectoryData) -> list[list[str]]:
         """Return the sample sheet content for a flow cell."""
         lims_samples: list[FlowCellSample] = list(
             get_flow_cell_samples(
                 lims=self.lims_api,
                 flow_cell_id=flow_cell.id,
             )
         )
@@ -181,15 +181,15 @@
             raise SampleSheetError(message)
         creator = SampleSheetCreator(flow_cell=flow_cell, lims_samples=lims_samples)
         LOG.info(
             f"Constructing sample sheet for the {flow_cell.sequencer_type} flow cell {flow_cell.id}"
         )
         return creator.construct_sample_sheet()
 
-    def _create_sample_sheet_file(self, flow_cell: FlowCellDirectoryData) -> None:
+    def _create_sample_sheet_file(self, flow_cell: IlluminaRunDirectoryData) -> None:
         """Create a valid sample sheet in the flow cell directory and add it to Housekeeper."""
         sample_sheet_content: list[list[str]] = self._get_sample_sheet_content(flow_cell)
         if not self.force:
             self.validator.validate_sample_sheet_from_content(sample_sheet_content)
         LOG.info(f"Writing sample sheet to {flow_cell.sample_sheet_path.resolve()}")
         if self.dry_run:
             click.echo(
@@ -212,15 +212,15 @@
         )
 
     def get_or_create_sample_sheet(self, flow_cell_name: str) -> None:
         """
         Ensure that a valid sample sheet is present in the flow cell directory by fetching it from
         housekeeper or creating it if there is not a valid sample sheet.
         """
-        flow_cell: FlowCellDirectoryData = self._get_flow_cell(flow_cell_name)
+        flow_cell: IlluminaRunDirectoryData = self._get_flow_cell(flow_cell_name)
         LOG.info("Fetching and validating sample sheet from Housekeeper")
         try:
             self._use_sample_sheet_from_housekeeper(flow_cell)
             return
         except SampleSheetError:
             LOG.warning(
                 "It was not possible to use sample sheet from Housekeeper, "
```

### Comparing `cg-60.9.1/cg/apps/demultiplex/sample_sheet/index.py` & `cg-60.9.3/cg/apps/demultiplex/sample_sheet/index.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/apps/demultiplex/sample_sheet/override_cycles_validator.py` & `cg-60.9.3/cg/apps/demultiplex/sample_sheet/override_cycles_validator.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/apps/demultiplex/sample_sheet/read_sample_sheet.py` & `cg-60.9.3/cg/apps/demultiplex/sample_sheet/read_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/apps/demultiplex/sample_sheet/sample_models.py` & `cg-60.9.3/cg/apps/demultiplex/sample_sheet/sample_models.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/apps/demultiplex/sample_sheet/sample_sheet_creator.py` & `cg-60.9.3/cg/apps/demultiplex/sample_sheet/sample_sheet_creator.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 
 import logging
 
 from cg.apps.demultiplex.sample_sheet.read_sample_sheet import get_samples_by_lane
 from cg.apps.demultiplex.sample_sheet.sample_models import FlowCellSample
 from cg.constants.demultiplexing import IndexSettings, SampleSheetBCLConvertSections
 from cg.models.demultiplex.run_parameters import RunParameters
-from cg.models.flow_cell.flow_cell import FlowCellDirectoryData
+from cg.models.run_devices.illumina_run_directory_data import IlluminaRunDirectoryData
 
 LOG = logging.getLogger(__name__)
 
 
 class SampleSheetCreator:
     """Base class for sample sheet creation."""
 
     def __init__(
         self,
-        flow_cell: FlowCellDirectoryData,
+        flow_cell: IlluminaRunDirectoryData,
         lims_samples: list[FlowCellSample],
     ):
-        self.flow_cell: FlowCellDirectoryData = flow_cell
+        self.flow_cell: IlluminaRunDirectoryData = flow_cell
         self.flow_cell_id: str = flow_cell.id
         self.lims_samples: list[FlowCellSample] = lims_samples
         self.run_parameters: RunParameters = flow_cell.run_parameters
         self.index_settings: IndexSettings = self.run_parameters.index_settings
 
     def convert_sample_to_header_dict(
         self,
```

### Comparing `cg-60.9.1/cg/apps/demultiplex/sample_sheet/sample_sheet_models.py` & `cg-60.9.3/cg/apps/demultiplex/sample_sheet/sample_sheet_models.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/apps/demultiplex/sample_sheet/sample_sheet_validator.py` & `cg-60.9.3/cg/apps/demultiplex/sample_sheet/sample_sheet_validator.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/apps/demultiplex/sample_sheet/validators.py` & `cg-60.9.3/cg/apps/demultiplex/sample_sheet/validators.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/apps/demultiplex/sbatch.py` & `cg-60.9.3/cg/apps/demultiplex/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/apps/downsample/downsample.py` & `cg-60.9.3/cg/apps/downsample/downsample.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/apps/downsample/utils.py` & `cg-60.9.3/cg/apps/downsample/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/apps/gens.py` & `cg-60.9.3/cg/apps/gens.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/apps/gt.py` & `cg-60.9.3/cg/apps/gt.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/apps/hermes/hermes_api.py` & `cg-60.9.3/cg/apps/hermes/hermes_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/apps/hermes/models.py` & `cg-60.9.3/cg/apps/hermes/models.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/apps/housekeeper/hk.py` & `cg-60.9.3/cg/apps/housekeeper/hk.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/apps/invoice/render.py` & `cg-60.9.3/cg/apps/invoice/render.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/apps/invoice/templates/KI_pool_invoice.xlsx` & `cg-60.9.3/cg/apps/invoice/templates/KI_pool_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/apps/invoice/templates/KI_sample_invoice.xlsx` & `cg-60.9.3/cg/apps/invoice/templates/KI_sample_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/apps/invoice/templates/KTH_pool_invoice.xlsx` & `cg-60.9.3/cg/apps/invoice/templates/KTH_pool_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/apps/invoice/templates/KTH_sample_invoice.xlsx` & `cg-60.9.3/cg/apps/invoice/templates/KTH_sample_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/apps/lims/api.py` & `cg-60.9.3/cg/apps/lims/api.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/apps/lims/batch.py` & `cg-60.9.3/cg/apps/lims/batch.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/apps/lims/order.py` & `cg-60.9.3/cg/apps/lims/order.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/apps/lims/sample_sheet.py` & `cg-60.9.3/cg/apps/lims/sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/apps/loqus.py` & `cg-60.9.3/cg/apps/loqus.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/apps/madeline/api.py` & `cg-60.9.3/cg/apps/madeline/api.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/apps/mip/confighandler.py` & `cg-60.9.3/cg/apps/mip/confighandler.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/apps/mutacc_auto.py` & `cg-60.9.3/cg/apps/mutacc_auto.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/apps/orderform/excel_orderform_parser.py` & `cg-60.9.3/cg/apps/orderform/excel_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/apps/orderform/json_orderform_parser.py` & `cg-60.9.3/cg/apps/orderform/json_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/apps/orderform/orderform_parser.py` & `cg-60.9.3/cg/apps/orderform/orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/apps/osticket.py` & `cg-60.9.3/cg/apps/osticket.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/apps/scout/scout_export.py` & `cg-60.9.3/cg/apps/scout/scout_export.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/apps/scout/scoutapi.py` & `cg-60.9.3/cg/apps/scout/scoutapi.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/apps/slurm/sbatch.py` & `cg-60.9.3/cg/apps/slurm/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/apps/slurm/slurm_api.py` & `cg-60.9.3/cg/apps/slurm/slurm_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/apps/tb/api.py` & `cg-60.9.3/cg/apps/tb/api.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/apps/tb/models.py` & `cg-60.9.3/cg/apps/tb/models.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/cli/add.py` & `cg-60.9.3/cg/cli/add.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/cli/archive.py` & `cg-60.9.3/cg/cli/archive.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/cli/backup.py` & `cg-60.9.3/cg/cli/backup.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,17 +23,17 @@
 from cg.meta.encryption.encryption import (
     EncryptionAPI,
     FlowCellEncryptionAPI,
     SpringEncryptionAPI,
 )
 from cg.meta.tar.tar import TarAPI
 from cg.models.cg_config import CGConfig
-from cg.models.flow_cell.flow_cell import (
-    FlowCellDirectoryData,
-    get_flow_cells_from_path,
+from cg.models.run_devices.illumina_run_directory_data import (
+    IlluminaRunDirectoryData,
+    get_sequencing_runs_from_path,
 )
 from cg.store.models import Flowcell, Sample
 from cg.store.store import Store
 
 LOG = logging.getLogger(__name__)
 
 
@@ -48,16 +48,16 @@
 @DRY_RUN
 @click.pass_obj
 def backup_flow_cells(context: CGConfig, dry_run: bool):
     """Back-up flow cells."""
     pdc_api = context.pdc_api
     pdc_api.dry_run = dry_run
     status_db: Store = context.status_db
-    flow_cells: list[FlowCellDirectoryData] = get_flow_cells_from_path(
-        flow_cells_dir=Path(context.illumina_flow_cells_directory)
+    flow_cells: list[IlluminaRunDirectoryData] = get_sequencing_runs_from_path(
+        sequencing_run_dir=Path(context.illumina_flow_cells_directory)
     )
     for flow_cell in flow_cells:
         db_flow_cell: Flowcell | None = status_db.get_flow_cell_by_name(flow_cell_name=flow_cell.id)
         flow_cell_encryption_api = FlowCellEncryptionAPI(
             binary_path=context.encryption.binary_path,
             dry_run=dry_run,
             encryption_dir=Path(context.encryption.encryption_dir),
@@ -84,16 +84,16 @@
 
 @backup.command("encrypt-flow-cells")
 @DRY_RUN
 @click.pass_obj
 def encrypt_flow_cells(context: CGConfig, dry_run: bool):
     """Encrypt flow cells."""
     status_db: Store = context.status_db
-    flow_cells: list[FlowCellDirectoryData] = get_flow_cells_from_path(
-        flow_cells_dir=Path(context.illumina_flow_cells_directory)
+    flow_cells: list[IlluminaRunDirectoryData] = get_sequencing_runs_from_path(
+        sequencing_run_dir=Path(context.illumina_flow_cells_directory)
     )
     for flow_cell in flow_cells:
         db_flow_cell: Flowcell | None = status_db.get_flow_cell_by_name(flow_cell_name=flow_cell.id)
         if db_flow_cell and db_flow_cell.has_backup:
             LOG.debug(f"Flow cell: {flow_cell.id} is already backed-up")
             continue
         flow_cell_encryption_api = FlowCellEncryptionAPI(
@@ -202,15 +202,15 @@
     spring_backup_api.encrypt_and_archive_spring_file(Path(spring_file_path))
 
 
 @backup.command("retrieve-spring-files")
 @DRY_RUN
 @click.option("-s", "--sample-id", "object_type", flag_value="sample", type=str)
 @click.option("-c", "--case-id", "object_type", flag_value="case", type=str)
-@click.option("-f", "--flow-cell-id", "object_type", flag_value="flow_cell", type=str)
+@click.option("-f", "--flow-cell-id", "object_type", flag_value="run_devices", type=str)
 @click.argument("identifier", type=str)
 @click.pass_context
 @click.pass_obj
 def retrieve_spring_files(
     config: CGConfig,
     context: click.Context,
     object_type: str,
```

### Comparing `cg-60.9.1/cg/cli/base.py` & `cg-60.9.3/cg/cli/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/cli/clean.py` & `cg-60.9.3/cg/cli/clean.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/cli/compress/base.py` & `cg-60.9.3/cg/cli/compress/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/cli/compress/fastq.py` & `cg-60.9.3/cg/cli/compress/fastq.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/cli/compress/helpers.py` & `cg-60.9.3/cg/cli/compress/helpers.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/cli/delete/base.py` & `cg-60.9.3/cg/cli/delete/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/cli/delete/case.py` & `cg-60.9.3/cg/cli/delete/case.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/cli/delete/cases.py` & `cg-60.9.3/cg/cli/delete/cases.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/cli/delete/observations.py` & `cg-60.9.3/cg/cli/delete/observations.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/cli/deliver/base.py` & `cg-60.9.3/cg/cli/deliver/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/cli/demultiplex/base.py` & `cg-60.9.3/cg/cli/demultiplex/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/cli/demultiplex/copy_novaseqx_demultiplex_data.py` & `cg-60.9.3/cg/cli/demultiplex/copy_novaseqx_demultiplex_data.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/cli/demultiplex/demux.py` & `cg-60.9.3/cg/cli/demultiplex/demux.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from cg.meta.demultiplex.utils import (
     create_manifest_file,
     is_flow_cell_sync_confirmed,
     is_manifest_file_required,
     is_syncing_complete,
 )
 from cg.models.cg_config import CGConfig
-from cg.models.flow_cell.flow_cell import FlowCellDirectoryData
+from cg.models.run_devices.illumina_run_directory_data import IlluminaRunDirectoryData
 
 LOG = logging.getLogger(__name__)
 
 
 @click.command(name="all")
 @click.option("--flow-cells-directory", type=click.Path(exists=True, file_okay=False))
 @DRY_RUN
@@ -46,15 +46,15 @@
 
     LOG.info(f"Search for flow cells ready to demultiplex in {flow_cells_directory}")
     for sub_dir in flow_cells_directory.iterdir():
         if not sub_dir.is_dir():
             continue
         LOG.info(f"Found directory {sub_dir}")
         try:
-            flow_cell = FlowCellDirectoryData(flow_cell_path=sub_dir)
+            flow_cell = IlluminaRunDirectoryData(sequencing_run_path=sub_dir)
         except FlowCellError:
             continue
 
         if not demultiplex_api.is_demultiplexing_possible(flow_cell=flow_cell):
             LOG.warning(f"Can not start demultiplexing for flow cell {flow_cell.id}!")
             continue
 
@@ -94,15 +94,15 @@
     demultiplex_api: DemultiplexingAPI = context.demultiplex_api
     flow_cell_directory: Path = Path(context.demultiplex_api.flow_cells_dir, flow_cell_name)
     demultiplex_api.set_dry_run(dry_run=dry_run)
     LOG.info(f"setting flow cell id to {flow_cell_name}")
     LOG.info(f"setting demultiplexed runs dir to {demultiplex_api.demultiplexed_runs_dir}")
 
     try:
-        flow_cell = FlowCellDirectoryData(flow_cell_directory)
+        flow_cell = IlluminaRunDirectoryData(flow_cell_directory)
     except FlowCellError as error:
         raise click.Abort from error
 
     if not demultiplex_api.is_demultiplexing_possible(flow_cell=flow_cell):
         LOG.warning("Can not start demultiplexing!")
         return
```

### Comparing `cg-60.9.1/cg/cli/demultiplex/finish.py` & `cg-60.9.3/cg/cli/demultiplex/finish.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/cli/demultiplex/sample_sheet.py` & `cg-60.9.3/cg/cli/demultiplex/sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/cli/downsample.py` & `cg-60.9.3/cg/cli/downsample.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/cli/generate/report/base.py` & `cg-60.9.3/cg/cli/generate/report/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/cli/generate/report/options.py` & `cg-60.9.3/cg/cli/generate/report/options.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/cli/generate/report/utils.py` & `cg-60.9.3/cg/cli/generate/report/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/cli/get.py` & `cg-60.9.3/cg/cli/get.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/cli/set/base.py` & `cg-60.9.3/cg/cli/set/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/cli/set/case.py` & `cg-60.9.3/cg/cli/set/case.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/cli/set/cases.py` & `cg-60.9.3/cg/cli/set/cases.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/cli/store/base.py` & `cg-60.9.3/cg/cli/store/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/cli/store/store.py` & `cg-60.9.3/cg/cli/store/store.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/cli/transfer.py` & `cg-60.9.3/cg/cli/transfer.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/cli/upload/base.py` & `cg-60.9.3/cg/cli/upload/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/cli/upload/clinical_delivery.py` & `cg-60.9.3/cg/cli/upload/clinical_delivery.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/cli/upload/coverage.py` & `cg-60.9.3/cg/cli/upload/coverage.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/cli/upload/delivery_report.py` & `cg-60.9.3/cg/cli/upload/delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/cli/upload/fohm.py` & `cg-60.9.3/cg/cli/upload/fohm.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/cli/upload/genotype.py` & `cg-60.9.3/cg/cli/upload/genotype.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/cli/upload/gens.py` & `cg-60.9.3/cg/cli/upload/gens.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/cli/upload/gisaid.py` & `cg-60.9.3/cg/cli/upload/gisaid.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/cli/upload/mutacc.py` & `cg-60.9.3/cg/cli/upload/mutacc.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/cli/upload/nipt/base.py` & `cg-60.9.3/cg/cli/upload/nipt/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/cli/upload/nipt/ftp.py` & `cg-60.9.3/cg/cli/upload/nipt/ftp.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/cli/upload/nipt/statina.py` & `cg-60.9.3/cg/cli/upload/nipt/statina.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/cli/upload/observations/observations.py` & `cg-60.9.3/cg/cli/upload/observations/observations.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/cli/upload/observations/utils.py` & `cg-60.9.3/cg/cli/upload/observations/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/cli/upload/scout.py` & `cg-60.9.3/cg/cli/upload/scout.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/cli/upload/utils.py` & `cg-60.9.3/cg/cli/upload/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/cli/upload/validate.py` & `cg-60.9.3/cg/cli/upload/validate.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/cli/validate.py` & `cg-60.9.3/cg/cli/validate.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/cli/workflow/balsamic/base.py` & `cg-60.9.3/cg/cli/workflow/balsamic/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/cli/workflow/balsamic/options.py` & `cg-60.9.3/cg/cli/workflow/balsamic/options.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/cli/workflow/balsamic/pon.py` & `cg-60.9.3/cg/cli/workflow/balsamic/pon.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/cli/workflow/balsamic/qc.py` & `cg-60.9.3/cg/cli/workflow/balsamic/qc.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/cli/workflow/balsamic/umi.py` & `cg-60.9.3/cg/cli/workflow/balsamic/umi.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/cli/workflow/base.py` & `cg-60.9.3/cg/cli/workflow/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/cli/workflow/commands.py` & `cg-60.9.3/cg/cli/workflow/commands.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/cli/workflow/fastq/base.py` & `cg-60.9.3/cg/cli/workflow/fastq/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/cli/workflow/fastq/fastq_service.py` & `cg-60.9.3/cg/cli/workflow/fastq/fastq_service.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/cli/workflow/fluffy/base.py` & `cg-60.9.3/cg/cli/workflow/fluffy/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/cli/workflow/jasen/base.py` & `cg-60.9.3/cg/cli/workflow/jasen/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/cli/workflow/microsalt/base.py` & `cg-60.9.3/cg/cli/workflow/microsalt/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/cli/workflow/mip/base.py` & `cg-60.9.3/cg/cli/workflow/mip/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/cli/workflow/mip/options.py` & `cg-60.9.3/cg/cli/workflow/mip/options.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/cli/workflow/mip_dna/base.py` & `cg-60.9.3/cg/cli/workflow/mip_dna/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/cli/workflow/mip_rna/base.py` & `cg-60.9.3/cg/cli/workflow/mip_rna/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/cli/workflow/mutant/base.py` & `cg-60.9.3/cg/cli/workflow/mutant/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/cli/workflow/nf_analysis.py` & `cg-60.9.3/cg/cli/workflow/nf_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/cli/workflow/raredisease/base.py` & `cg-60.9.3/cg/cli/workflow/raredisease/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/cli/workflow/rnafusion/base.py` & `cg-60.9.3/cg/cli/workflow/rnafusion/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/cli/workflow/taxprofiler/base.py` & `cg-60.9.3/cg/cli/workflow/taxprofiler/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/cli/workflow/tomte/base.py` & `cg-60.9.3/cg/cli/workflow/tomte/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/clients/arnold/api.py` & `cg-60.9.3/cg/clients/arnold/api.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/clients/janus/api.py` & `cg-60.9.3/cg/clients/janus/api.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/constants/__init__.py` & `cg-60.9.3/cg/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/constants/bcl_convert_metrics.py` & `cg-60.9.3/cg/constants/bcl_convert_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/constants/constants.py` & `cg-60.9.3/cg/constants/constants.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/constants/delivery.py` & `cg-60.9.3/cg/constants/delivery.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/constants/demultiplexing.py` & `cg-60.9.3/cg/constants/demultiplexing.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/constants/encryption.py` & `cg-60.9.3/cg/constants/encryption.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/constants/gene_panel.py` & `cg-60.9.3/cg/constants/gene_panel.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/constants/housekeeper_tags.py` & `cg-60.9.3/cg/constants/housekeeper_tags.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/constants/lims.py` & `cg-60.9.3/cg/constants/lims.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/constants/metrics.py` & `cg-60.9.3/cg/constants/metrics.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/constants/nextflow.py` & `cg-60.9.3/cg/constants/nextflow.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/constants/nf_analysis.py` & `cg-60.9.3/cg/constants/nf_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/constants/observations.py` & `cg-60.9.3/cg/constants/observations.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/constants/orderforms.py` & `cg-60.9.3/cg/constants/orderforms.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/constants/priority.py` & `cg-60.9.3/cg/constants/priority.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/constants/report.py` & `cg-60.9.3/cg/constants/report.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/constants/sample_sources.py` & `cg-60.9.3/cg/constants/sample_sources.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/constants/scout.py` & `cg-60.9.3/cg/constants/scout.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/constants/sequencing.py` & `cg-60.9.3/cg/constants/sequencing.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/constants/subject.py` & `cg-60.9.3/cg/constants/subject.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/exc.py` & `cg-60.9.3/cg/exc.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/io/api.py` & `cg-60.9.3/cg/io/api.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/io/config.py` & `cg-60.9.3/cg/io/config.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/io/controller.py` & `cg-60.9.3/cg/io/controller.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/io/csv.py` & `cg-60.9.3/cg/io/csv.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/io/json.py` & `cg-60.9.3/cg/io/json.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/io/png.py` & `cg-60.9.3/cg/io/png.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/io/txt.py` & `cg-60.9.3/cg/io/txt.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/io/validate_path.py` & `cg-60.9.3/cg/io/validate_path.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/io/xml.py` & `cg-60.9.3/cg/io/xml.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/io/yaml.py` & `cg-60.9.3/cg/io/yaml.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/archive/archive.py` & `cg-60.9.3/cg/meta/archive/archive.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/archive/ddn/constants.py` & `cg-60.9.3/cg/meta/archive/ddn/constants.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/archive/ddn/ddn_data_flow_client.py` & `cg-60.9.3/cg/meta/archive/ddn/ddn_data_flow_client.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/archive/ddn/models.py` & `cg-60.9.3/cg/meta/archive/ddn/models.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/archive/ddn/utils.py` & `cg-60.9.3/cg/meta/archive/ddn/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/archive/models.py` & `cg-60.9.3/cg/meta/archive/models.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/backup/backup.py` & `cg-60.9.3/cg/meta/backup/backup.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/backup/pdc.py` & `cg-60.9.3/cg/meta/backup/pdc.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/clean/api.py` & `cg-60.9.3/cg/meta/clean/api.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/clean/clean_flow_cells.py` & `cg-60.9.3/cg/meta/clean/clean_flow_cells.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from cg.constants import SequencingFileTag
 from cg.constants.time import TWENTY_ONE_DAYS
 from cg.exc import (
     CleanFlowCellFailedError,
     HousekeeperBundleVersionMissingError,
     HousekeeperFileMissingError,
 )
-from cg.models.flow_cell.flow_cell import FlowCellDirectoryData
+from cg.models.run_devices.illumina_run_directory_data import IlluminaRunDirectoryData
 from cg.store.models import Flowcell, SampleLaneSequencingMetrics
 from cg.store.store import Store
 from cg.utils.files import remove_directory_and_contents
 from cg.utils.time import is_directory_older_than_days_old
 
 LOG = logging.getLogger(__name__)
 
@@ -38,15 +38,15 @@
     """
 
     def __init__(
         self, status_db: Store, housekeeper_api: HousekeeperAPI, flow_cell_path: Path, dry_run: bool
     ):
         self.status_db: Store = status_db
         self.hk_api: HousekeeperAPI = housekeeper_api
-        self.flow_cell = FlowCellDirectoryData(flow_cell_path=flow_cell_path)
+        self.flow_cell = IlluminaRunDirectoryData(sequencing_run_path=flow_cell_path)
         self.dry_run: bool = dry_run
         LOG.info(f"Trying to delete {flow_cell_path}")
 
     def delete_flow_cell_directory(self) -> None:
         """
         Delete the flow cell directory if it fulfills all requirements.
         Raises:
```

### Comparing `cg-60.9.1/cg/meta/clean/clean_retrieved_spring_files.py` & `cg-60.9.3/cg/meta/clean/clean_retrieved_spring_files.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/compress/compress.py` & `cg-60.9.3/cg/meta/compress/compress.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/compress/files.py` & `cg-60.9.3/cg/meta/compress/files.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/deliver/deliver.py` & `cg-60.9.3/cg/meta/deliver/deliver.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/deliver/deliver_ticket.py` & `cg-60.9.3/cg/meta/deliver/deliver_ticket.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/deliver/fastq_path_generator.py` & `cg-60.9.3/cg/meta/deliver/fastq_path_generator.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/delivery/delivery.py` & `cg-60.9.3/cg/meta/delivery/delivery.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/demultiplex/combine_sequencing_metrics.py` & `cg-60.9.3/cg/meta/demultiplex/combine_sequencing_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/demultiplex/demux_post_processing.py` & `cg-60.9.3/cg/meta/demultiplex/demux_post_processing.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     store_sequencing_metrics_in_status_db,
 )
 from cg.meta.demultiplex.utils import create_delivery_file_in_flow_cell_directory
 from cg.services.illumina_services.illumina_post_processing_service.validation import (
     is_flow_cell_ready_for_postprocessing,
 )
 from cg.models.cg_config import CGConfig
-from cg.models.flow_cell.flow_cell import FlowCellDirectoryData
+from cg.models.run_devices.illumina_run_directory_data import IlluminaRunDirectoryData
 from cg.store.store import Store
 
 LOG = logging.getLogger(__name__)
 
 
 class DemuxPostProcessingAPI:
     """Post demultiplexing API class."""
@@ -66,15 +66,15 @@
             LOG.info(f"Dry run will not finish flow cell {flow_cell_directory_name}")
             return
 
         LOG.info(f"Finish flow cell {flow_cell_directory_name}")
 
         flow_cell_out_directory = Path(self.demultiplexed_runs_dir, flow_cell_directory_name)
 
-        flow_cell = FlowCellDirectoryData(flow_cell_out_directory)
+        flow_cell = IlluminaRunDirectoryData(flow_cell_out_directory)
 
         sample_sheet_path: Path = self.hk_api.get_sample_sheet_path(flow_cell.id)
         flow_cell.set_sample_sheet_path_hk(hk_path=sample_sheet_path)
         LOG.debug("Set path for Housekeeper sample sheet in flow cell")
 
         try:
             is_flow_cell_ready_for_postprocessing(
@@ -104,15 +104,15 @@
                 self.finish_flow_cell(flow_cell_dir.name)
             except Exception as error:
                 LOG.error(f"Failed to finish flow cell {flow_cell_dir.name}: {str(error)}")
                 is_error_raised = True
                 continue
         return is_error_raised
 
-    def store_flow_cell_data(self, parsed_flow_cell: FlowCellDirectoryData) -> None:
+    def store_flow_cell_data(self, parsed_flow_cell: IlluminaRunDirectoryData) -> None:
         """Store data from the flow cell directory in status db and housekeeper."""
         store_flow_cell_data_in_status_db(
             parsed_flow_cell=parsed_flow_cell,
             store=self.status_db,
         )
         store_sequencing_metrics_in_status_db(flow_cell=parsed_flow_cell, store=self.status_db)
         store_sample_data_in_status_db(flow_cell=parsed_flow_cell, store=self.status_db)
```

### Comparing `cg-60.9.1/cg/meta/demultiplex/housekeeper_storage_functions.py` & `cg-60.9.3/cg/meta/demultiplex/housekeeper_storage_functions.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,23 +13,23 @@
     get_lane_from_sample_fastq,
     get_q30_threshold,
     get_sample_fastqs_from_flow_cell,
     get_sample_sheet_path_from_flow_cell_dir,
     get_undetermined_fastqs,
     rename_fastq_file_if_needed,
 )
-from cg.models.flow_cell.flow_cell import FlowCellDirectoryData
+from cg.models.run_devices.illumina_run_directory_data import IlluminaRunDirectoryData
 from cg.store.store import Store
 from cg.utils.files import get_files_matching_pattern
 
 LOG = logging.getLogger(__name__)
 
 
 def store_flow_cell_data_in_housekeeper(
-    flow_cell: FlowCellDirectoryData,
+    flow_cell: IlluminaRunDirectoryData,
     hk_api: HousekeeperAPI,
     flow_cell_run_dir: Path,
     store: Store,
 ) -> None:
     LOG.info(f"Add flow cell data to Housekeeper for {flow_cell.id}")
 
     hk_api.add_bundle_and_version_if_non_existent(flow_cell.id)
@@ -44,15 +44,15 @@
     )
     add_run_parameters_file_to_housekeeper(
         flow_cell_name=flow_cell.full_name, flow_cell_run_dir=flow_cell_run_dir, hk_api=hk_api
     )
 
 
 def store_undetermined_fastq_files(
-    flow_cell: FlowCellDirectoryData, hk_api: HousekeeperAPI, store: Store
+    flow_cell: IlluminaRunDirectoryData, hk_api: HousekeeperAPI, store: Store
 ) -> None:
     """Store undetermined fastq files for non-pooled samples in Housekeeper."""
     non_pooled_lanes_and_samples: list[tuple[int, str]] = (
         flow_cell.sample_sheet.get_non_pooled_lanes_and_samples()
     )
 
     for lane, sample_id in non_pooled_lanes_and_samples:
@@ -72,15 +72,15 @@
                     sample_internal_id=sample_id,
                     sample_fastq_path=fastq_path,
                     flow_cell_id=flow_cell.id,
                 )
 
 
 def add_demux_logs_to_housekeeper(
-    flow_cell: FlowCellDirectoryData, hk_api: HousekeeperAPI, flow_cell_run_dir: Path
+    flow_cell: IlluminaRunDirectoryData, hk_api: HousekeeperAPI, flow_cell_run_dir: Path
 ) -> None:
     """Add demux logs to Housekeeper."""
     log_file_name_pattern: str = r"*_demultiplex.std*"
     demux_log_file_paths: list[Path] = get_files_matching_pattern(
         directory=Path(flow_cell_run_dir, flow_cell.full_name), pattern=log_file_name_pattern
     )
 
@@ -96,27 +96,27 @@
 
 
 def add_run_parameters_file_to_housekeeper(
     flow_cell_name: str, flow_cell_run_dir: Path, hk_api: HousekeeperAPI
 ) -> None:
     """Add run parameters file to Housekeeper."""
     flow_cell_path = Path(flow_cell_run_dir, flow_cell_name)
-    flow_cell = FlowCellDirectoryData(flow_cell_path)
+    flow_cell = IlluminaRunDirectoryData(flow_cell_path)
     run_parameters_file_path: Path = flow_cell.run_parameters_path
     tag_names: list[str] = [SequencingFileTag.RUN_PARAMETERS, flow_cell.id]
     hk_api.add_file_to_bundle_if_non_existent(
         file_path=run_parameters_file_path, bundle_name=flow_cell.id, tag_names=tag_names
     )
     LOG.info(
         f"Added run parameters file {run_parameters_file_path} to {flow_cell.id} in Housekeeper."
     )
 
 
 def add_sample_fastq_files_to_housekeeper(
-    flow_cell: FlowCellDirectoryData, hk_api: HousekeeperAPI, store: Store
+    flow_cell: IlluminaRunDirectoryData, hk_api: HousekeeperAPI, store: Store
 ) -> None:
     """Add sample fastq files from flow cell to Housekeeper."""
     sample_internal_ids: list[str] = flow_cell.sample_sheet.get_sample_ids()
 
     for sample_internal_id in sample_internal_ids:
         sample_fastq_paths: list[Path] | None = get_sample_fastqs_from_flow_cell(
             flow_cell_directory=flow_cell.path, sample_internal_id=sample_internal_id
```

### Comparing `cg-60.9.1/cg/meta/demultiplex/status_db_storage_functions.py` & `cg-60.9.3/cg/meta/demultiplex/status_db_storage_functions.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 import datetime
 import logging
 
 
 from cg.constants import FlowCellStatus
 from cg.meta.demultiplex.combine_sequencing_metrics import combine_mapped_metrics_with_undetermined
 from cg.meta.demultiplex.utils import get_q30_threshold
-from cg.models.flow_cell.flow_cell import FlowCellDirectoryData
+from cg.models.run_devices.illumina_run_directory_data import IlluminaRunDirectoryData
 from cg.services.illumina_services.illumina_metrics_service.illumina_metrics_service import (
     IlluminaMetricsService,
 )
 
 from cg.store.models import Flowcell, Sample, SampleLaneSequencingMetrics
 from cg.store.store import Store
 
 LOG = logging.getLogger(__name__)
 
 
 def store_flow_cell_data_in_status_db(
-    parsed_flow_cell: FlowCellDirectoryData,
+    parsed_flow_cell: IlluminaRunDirectoryData,
     store: Store,
 ) -> None:
     """
     Create flow cell from the parsed and validated flow cell data.
     And add the samples on the flow cell to the model.
     """
     flow_cell: Flowcell | None = store.get_flow_cell_by_name(flow_cell_name=parsed_flow_cell.id)
@@ -39,15 +39,17 @@
         LOG.info(f"Flow cell already exists in status db: {parsed_flow_cell.id}.")
         flow_cell.status = FlowCellStatus.ON_DISK
     LOG.info(f"Added samples to flow cell: {parsed_flow_cell.id}.")
     store.session.add(flow_cell)
     store.session.commit()
 
 
-def store_sequencing_metrics_in_status_db(flow_cell: FlowCellDirectoryData, store: Store) -> None:
+def store_sequencing_metrics_in_status_db(
+    flow_cell: IlluminaRunDirectoryData, store: Store
+) -> None:
     metrics_service = IlluminaMetricsService()
     mapped_metrics: list[SampleLaneSequencingMetrics] = (
         metrics_service.create_sample_lane_sequencing_metrics_for_flow_cell(
             flow_cell_directory=flow_cell.path
         )
     )
     undetermined_metrics: list[SampleLaneSequencingMetrics] = (
@@ -99,15 +101,15 @@
     if existing_metrics_entry:
         LOG.warning(
             f"Sample lane sequencing metrics already exist for {metric.flow_cell_name}, {metric.sample_internal_id}, and lane {metric.flow_cell_lane_number}. Skipping."
         )
     return bool(existing_metrics_entry)
 
 
-def store_sample_data_in_status_db(flow_cell: FlowCellDirectoryData, store: Store) -> None:
+def store_sample_data_in_status_db(flow_cell: IlluminaRunDirectoryData, store: Store) -> None:
     """Update samples on the flow cell with read counts and sequencing date."""
     q30_threshold: int = get_q30_threshold(flow_cell.sequencer_type)
     sample_internal_ids: list[str] = flow_cell.sample_sheet.get_sample_ids()
     sequenced_at: datetime = flow_cell.sequenced_at
 
     for sample_id in sample_internal_ids:
         sample: Sample | None = store.get_sample_by_internal_id(sample_id)
```

### Comparing `cg-60.9.1/cg/meta/demultiplex/utils.py` & `cg-60.9.3/cg/meta/demultiplex/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/encryption/encryption.py` & `cg-60.9.3/cg/meta/encryption/encryption.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from cg.constants.priority import SlurmQos
 from cg.exc import ChecksumFailedError, FlowCellEncryptionError, FlowCellError
 from cg.meta.encryption.sbatch import (
     FLOW_CELL_ENCRYPT_COMMANDS,
     FLOW_CELL_ENCRYPT_ERROR,
 )
 from cg.meta.tar.tar import TarAPI
-from cg.models.flow_cell.flow_cell import FlowCellDirectoryData
+from cg.models.run_devices.illumina_run_directory_data import IlluminaRunDirectoryData
 from cg.models.slurm.sbatch import Sbatch
 from cg.utils import Process
 from cg.utils.checksum.checksum import sha512_checksum
 
 LOG = logging.getLogger(__name__)
 LIMIT_PIGZ_TASK: int = 3
 
@@ -143,23 +143,23 @@
 class FlowCellEncryptionAPI(EncryptionAPI):
     """Encryption functionality for flow cells."""
 
     def __init__(
         self,
         binary_path: str,
         encryption_dir: Path,
-        flow_cell: FlowCellDirectoryData,
+        flow_cell: IlluminaRunDirectoryData,
         pigz_binary_path: str,
         sbatch_parameter: dict[str, str | int],
         slurm_api: SlurmAPI,
         tar_api: TarAPI,
         dry_run: bool = False,
     ):
         super().__init__(binary_path=binary_path, dry_run=dry_run)
-        self.flow_cell: FlowCellDirectoryData = flow_cell
+        self.flow_cell: IlluminaRunDirectoryData = flow_cell
         self.encryption_dir: Path = encryption_dir
         self.tar_api: TarAPI = tar_api
         self.pigz_binary_path: str = pigz_binary_path
         self.slurm_api: SlurmAPI = slurm_api
         self.slurm_account: str = sbatch_parameter.get("account")
         self.slurm_hours: int = sbatch_parameter.get("hours")
         self.slurm_mail_user: str = sbatch_parameter.get("mail_user")
@@ -246,15 +246,15 @@
         return SPACE.join(decryption_parameters)
 
     def is_encryption_possible(self) -> bool | None:
         """Check if requirements for encryption are meet.
         Raises:
             FlowCellError if sequencing is not ready, encryption is pending or complete.
         """
-        if not self.flow_cell.is_flow_cell_ready():
+        if not self.flow_cell.is_sequencing_run_ready():
             raise FlowCellError(f"Flow cell: {self.flow_cell.id} is not ready")
         if self.complete_file_path.exists():
             raise FlowCellEncryptionError(
                 f"Encryption already completed for flow cell: {self.flow_cell.id}"
             )
         if self.pending_file_path.exists():
             raise FlowCellEncryptionError(
```

### Comparing `cg-60.9.1/cg/meta/encryption/sbatch.py` & `cg-60.9.3/cg/meta/encryption/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/invoice.py` & `cg-60.9.3/cg/meta/invoice.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/meta.py` & `cg-60.9.3/cg/meta/meta.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/observations/balsamic_observations_api.py` & `cg-60.9.3/cg/meta/observations/balsamic_observations_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/observations/mip_dna_observations_api.py` & `cg-60.9.3/cg/meta/observations/mip_dna_observations_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/observations/observations_api.py` & `cg-60.9.3/cg/meta/observations/observations_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/orders/api.py` & `cg-60.9.3/cg/meta/orders/api.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/orders/case_submitter.py` & `cg-60.9.3/cg/meta/orders/case_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/orders/fastq_submitter.py` & `cg-60.9.3/cg/meta/orders/fastq_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/orders/lims.py` & `cg-60.9.3/cg/meta/orders/lims.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/orders/metagenome_submitter.py` & `cg-60.9.3/cg/meta/orders/metagenome_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/orders/microbial_submitter.py` & `cg-60.9.3/cg/meta/orders/microbial_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/orders/pool_submitter.py` & `cg-60.9.3/cg/meta/orders/pool_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/orders/rnafusion_submitter.py` & `cg-60.9.3/cg/meta/orders/rnafusion_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/orders/sars_cov_2_submitter.py` & `cg-60.9.3/cg/meta/orders/sars_cov_2_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/orders/submitter.py` & `cg-60.9.3/cg/meta/orders/submitter.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/orders/ticket_handler.py` & `cg-60.9.3/cg/meta/orders/ticket_handler.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/qc_metrics/collect_qc_metrics.py` & `cg-60.9.3/cg/meta/qc_metrics/collect_qc_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/report/balsamic.py` & `cg-60.9.3/cg/meta/report/balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/report/balsamic_qc.py` & `cg-60.9.3/cg/meta/report/balsamic_qc.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/report/balsamic_umi.py` & `cg-60.9.3/cg/meta/report/balsamic_umi.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/report/field_validators.py` & `cg-60.9.3/cg/meta/report/field_validators.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/report/mip_dna.py` & `cg-60.9.3/cg/meta/report/mip_dna.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/report/report_api.py` & `cg-60.9.3/cg/meta/report/report_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/report/rnafusion.py` & `cg-60.9.3/cg/meta/report/rnafusion.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/report/taxprofiler.py` & `cg-60.9.3/cg/meta/report/taxprofiler.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/report/templates/delivery-report.html` & `cg-60.9.3/cg/meta/report/templates/delivery-report.html`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/report/templates/macros/data_analysis/data_analysis.html` & `cg-60.9.3/cg/meta/report/templates/macros/data_analysis/data_analysis.html`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/report/templates/macros/data_analysis/limitations.html` & `cg-60.9.3/cg/meta/report/templates/macros/data_analysis/limitations.html`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/report/templates/macros/data_analysis/qc_metrics/balsamic_qc_metrics.html` & `cg-60.9.3/cg/meta/report/templates/macros/data_analysis/qc_metrics/balsamic_qc_metrics.html`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/report/templates/macros/data_analysis/qc_metrics/mip_dna_qc_metrics.html` & `cg-60.9.3/cg/meta/report/templates/macros/data_analysis/qc_metrics/mip_dna_qc_metrics.html`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/report/templates/macros/data_analysis/qc_metrics/qc_metrics.html` & `cg-60.9.3/cg/meta/report/templates/macros/data_analysis/qc_metrics/qc_metrics.html`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/report/templates/macros/data_analysis/qc_metrics/rnafusion_qc_metrics.html` & `cg-60.9.3/cg/meta/report/templates/macros/data_analysis/qc_metrics/rnafusion_qc_metrics.html`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/report/templates/macros/data_analysis/qc_metrics/tomte_qc_metrics.html` & `cg-60.9.3/cg/meta/report/templates/macros/data_analysis/qc_metrics/tomte_qc_metrics.html`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/report/templates/macros/header.html` & `cg-60.9.3/cg/meta/report/templates/macros/header.html`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/report/templates/macros/order.html` & `cg-60.9.3/cg/meta/report/templates/macros/order.html`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/report/templates/macros/sample_prep.html` & `cg-60.9.3/cg/meta/report/templates/macros/sample_prep.html`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/report/templates/macros/uploaded_files/balsamic_uploaded_files.html` & `cg-60.9.3/cg/meta/report/templates/macros/uploaded_files/balsamic_uploaded_files.html`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/report/templates/macros/uploaded_files/mip_dna_uploaded_files.html` & `cg-60.9.3/cg/meta/report/templates/macros/uploaded_files/mip_dna_uploaded_files.html`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/report/templates/macros/uploaded_files/uploaded_files.html` & `cg-60.9.3/cg/meta/report/templates/macros/uploaded_files/uploaded_files.html`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/report/templates/static/css/bootstrap.min.css` & `cg-60.9.3/cg/meta/report/templates/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/report/templates/static/images/SWEDAC_logo.png` & `cg-60.9.3/cg/meta/report/templates/static/images/SWEDAC_logo.png`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/report/tomte.py` & `cg-60.9.3/cg/meta/report/tomte.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/rsync/rsync_api.py` & `cg-60.9.3/cg/meta/rsync/rsync_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/tar/tar.py` & `cg-60.9.3/cg/meta/tar/tar.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/transfer/external_data.py` & `cg-60.9.3/cg/meta/transfer/external_data.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/transfer/lims.py` & `cg-60.9.3/cg/meta/transfer/lims.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/upload/balsamic/balsamic.py` & `cg-60.9.3/cg/meta/upload/balsamic/balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/upload/coverage.py` & `cg-60.9.3/cg/meta/upload/coverage.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/upload/fohm/fohm.py` & `cg-60.9.3/cg/meta/upload/fohm/fohm.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/upload/gisaid/constants.py` & `cg-60.9.3/cg/meta/upload/gisaid/constants.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/upload/gisaid/gisaid.py` & `cg-60.9.3/cg/meta/upload/gisaid/gisaid.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/upload/gisaid/models.py` & `cg-60.9.3/cg/meta/upload/gisaid/models.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/upload/gt.py` & `cg-60.9.3/cg/meta/upload/gt.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/upload/microsalt/microsalt_upload_api.py` & `cg-60.9.3/cg/meta/upload/microsalt/microsalt_upload_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/upload/mip/mip_dna.py` & `cg-60.9.3/cg/meta/upload/mip/mip_dna.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/upload/mip/mip_rna.py` & `cg-60.9.3/cg/meta/upload/mip/mip_rna.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/upload/mutacc.py` & `cg-60.9.3/cg/meta/upload/mutacc.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/upload/nf_analysis.py` & `cg-60.9.3/cg/meta/upload/nf_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/upload/nipt/models.py` & `cg-60.9.3/cg/meta/upload/nipt/models.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/upload/nipt/nipt.py` & `cg-60.9.3/cg/meta/upload/nipt/nipt.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/upload/scout/balsamic_config_builder.py` & `cg-60.9.3/cg/meta/upload/scout/balsamic_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/upload/scout/balsamic_umi_config_builder.py` & `cg-60.9.3/cg/meta/upload/scout/balsamic_umi_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/upload/scout/hk_tags.py` & `cg-60.9.3/cg/meta/upload/scout/hk_tags.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/upload/scout/mip_config_builder.py` & `cg-60.9.3/cg/meta/upload/scout/mip_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/upload/scout/rnafusion_config_builder.py` & `cg-60.9.3/cg/meta/upload/scout/rnafusion_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/upload/scout/scout_config_builder.py` & `cg-60.9.3/cg/meta/upload/scout/scout_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/upload/scout/uploadscoutapi.py` & `cg-60.9.3/cg/meta/upload/scout/uploadscoutapi.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/upload/upload_api.py` & `cg-60.9.3/cg/meta/upload/upload_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/workflow/analysis.py` & `cg-60.9.3/cg/meta/workflow/analysis.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/workflow/balsamic.py` & `cg-60.9.3/cg/meta/workflow/balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/workflow/balsamic_pon.py` & `cg-60.9.3/cg/meta/workflow/balsamic_pon.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/workflow/balsamic_qc.py` & `cg-60.9.3/cg/meta/workflow/balsamic_qc.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/workflow/balsamic_umi.py` & `cg-60.9.3/cg/meta/workflow/balsamic_umi.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/workflow/downsample/downsample.py` & `cg-60.9.3/cg/meta/workflow/downsample/downsample.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/workflow/downsample/sbatch.py` & `cg-60.9.3/cg/meta/workflow/downsample/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/workflow/fastq.py` & `cg-60.9.3/cg/meta/workflow/fastq.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/workflow/fluffy.py` & `cg-60.9.3/cg/meta/workflow/fluffy.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/workflow/jasen.py` & `cg-60.9.3/cg/meta/workflow/jasen.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/workflow/microsalt/metrics_parser/models.py` & `cg-60.9.3/cg/meta/workflow/microsalt/metrics_parser/models.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/workflow/microsalt/microsalt.py` & `cg-60.9.3/cg/meta/workflow/microsalt/microsalt.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/workflow/microsalt/quality_controller/models.py` & `cg-60.9.3/cg/meta/workflow/microsalt/quality_controller/models.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/workflow/microsalt/quality_controller/quality_controller.py` & `cg-60.9.3/cg/meta/workflow/microsalt/quality_controller/quality_controller.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/workflow/microsalt/quality_controller/report_generator.py` & `cg-60.9.3/cg/meta/workflow/microsalt/quality_controller/report_generator.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/workflow/microsalt/quality_controller/result_logger.py` & `cg-60.9.3/cg/meta/workflow/microsalt/quality_controller/result_logger.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/workflow/microsalt/quality_controller/utils.py` & `cg-60.9.3/cg/meta/workflow/microsalt/quality_controller/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/workflow/microsalt/utils.py` & `cg-60.9.3/cg/meta/workflow/microsalt/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/workflow/mip.py` & `cg-60.9.3/cg/meta/workflow/mip.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/workflow/mip_dna.py` & `cg-60.9.3/cg/meta/workflow/mip_dna.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/workflow/mip_rna.py` & `cg-60.9.3/cg/meta/workflow/mip_rna.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/workflow/mutant.py` & `cg-60.9.3/cg/meta/workflow/mutant.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/workflow/nf_analysis.py` & `cg-60.9.3/cg/meta/workflow/nf_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/workflow/nf_handlers.py` & `cg-60.9.3/cg/meta/workflow/nf_handlers.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/workflow/prepare_fastq.py` & `cg-60.9.3/cg/meta/workflow/prepare_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/workflow/raredisease.py` & `cg-60.9.3/cg/meta/workflow/raredisease.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/workflow/rnafusion.py` & `cg-60.9.3/cg/meta/workflow/rnafusion.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/workflow/taxprofiler.py` & `cg-60.9.3/cg/meta/workflow/taxprofiler.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/meta/workflow/tomte.py` & `cg-60.9.3/cg/meta/workflow/tomte.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/models/balsamic/config.py` & `cg-60.9.3/cg/models/balsamic/config.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/models/balsamic/metrics.py` & `cg-60.9.3/cg/models/balsamic/metrics.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/models/cg_config.py` & `cg-60.9.3/cg/models/cg_config.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/models/compression_data.py` & `cg-60.9.3/cg/models/compression_data.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/models/deliverables/metric_deliverables.py` & `cg-60.9.3/cg/models/deliverables/metric_deliverables.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/models/demultiplex/run_parameters.py` & `cg-60.9.3/cg/models/demultiplex/run_parameters.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/models/demultiplex/sbatch.py` & `cg-60.9.3/cg/models/demultiplex/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/models/downsample/downsample_data.py` & `cg-60.9.3/cg/models/downsample/downsample_data.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/models/fastq.py` & `cg-60.9.3/cg/models/fastq.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/models/file_data.py` & `cg-60.9.3/cg/models/file_data.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/models/flow_cell/flow_cell.py` & `cg-60.9.3/cg/models/run_devices/illumina_run_directory_data.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from cg.exc import FlowCellError
 from cg.models.demultiplex.run_parameters import (
     RunParameters,
     RunParametersHiSeq,
     RunParametersNovaSeq6000,
     RunParametersNovaSeqX,
 )
-from cg.models.flow_cell.utils import parse_date
+from cg.models.run_devices.utils import parse_date
 from cg.services.parse_run_completion_status_service.parse_run_completion_status_service import (
     ParseRunCompletionStatusService,
 )
 from cg.utils.files import get_source_creation_time_stamp
 from cg.utils.time import format_time_from_string, format_time_from_ctime
 
 LOG = logging.getLogger(__name__)
@@ -32,61 +32,61 @@
     Sequencers.HISEQGA: RunParametersHiSeq,
     Sequencers.HISEQX: RunParametersHiSeq,
     Sequencers.NOVASEQ: RunParametersNovaSeq6000,
     Sequencers.NOVASEQX: RunParametersNovaSeqX,
 }
 
 
-class FlowCellDirectoryData:
-    """Class to collect information about flow cell directories and their particular files."""
+class IlluminaRunDirectoryData:
+    """Class to collect information about sequencing run directories and their particular files."""
 
-    def __init__(self, flow_cell_path: Path):
-        LOG.debug(f"Instantiating FlowCellDirectoryData with path {flow_cell_path}")
-        self.path: Path = flow_cell_path
+    def __init__(self, sequencing_run_path: Path):
+        LOG.debug(f"Instantiating FlowCellDirectoryData with path {sequencing_run_path}")
+        self.path: Path = sequencing_run_path
         self.machine_name: str = EMPTY_STRING
         self._run_parameters: RunParameters | None = None
         self.run_date: datetime.datetime = datetime.datetime.now()
         self.machine_number: int = 0
         self.base_name: str = EMPTY_STRING  # Base name is flow cell-id + flow cell position
         self.id: str = EMPTY_STRING
         self.position: Literal["A", "B"] = "A"
-        self.parse_flow_cell_dir_name()
+        self.parse_sequencing_run_dir_name()
         self._sample_sheet_path_hk: Path | None = None
         self.sample_sheet_validator = SampleSheetValidator()
 
-    def parse_flow_cell_dir_name(self):
-        """Parse relevant information from flow cell name.
-        This will assume that the flow cell naming convention is used. If not we skip the flow cell.
+    def parse_sequencing_run_dir_name(self):
+        """Parse relevant information from sequencing run name.
+        This will assume that the sequencing run naming convention is used. If not we skip the sequencing run.
         Convention is: <date>_<machine>_<run_numbers>_<A|B><flow_cell_id>
         Example: '230912_A00187_1009_AHK33MDRX3'.
         """
 
-        self.validate_flow_cell_dir_name()
+        self.validate_sequencing_run_dir_name()
         self.run_date = self._parse_date()
-        self.machine_name = self.split_flow_cell_name[1]
-        self.machine_number = int(self.split_flow_cell_name[2])
-        base_name: str = self.split_flow_cell_name[-1]
+        self.machine_name = self.split_sequencing_run_name[1]
+        self.machine_number = int(self.split_sequencing_run_name[2])
+        base_name: str = self.split_sequencing_run_name[-1]
         self.base_name = base_name
-        LOG.debug(f"Set flow cell id to {base_name}")
+        LOG.debug(f"Set sequencing run id to {base_name}")
         self.id = base_name[1:]
         self.position = base_name[0]
 
     @property
-    def split_flow_cell_name(self) -> list[str]:
-        """Return split flow cell name."""
+    def split_sequencing_run_name(self) -> list[str]:
+        """Return split sequencing run name."""
         return self.path.name.split("_")
 
     @property
     def full_name(self) -> str:
-        """Return flow cell full name."""
+        """Return sequencing run full name."""
         return self.path.name
 
     @property
     def sequenced_at(self) -> list[str]:
-        """Return the sequencing date for the flow cell."""
+        """Return the sequencing date for the sequencing run."""
         date_part: str = self.full_name.split("_")[0]
         return parse_date(date_part)
 
     @property
     def sample_sheet_path(self) -> Path:
         """
         Return sample sheet path.
@@ -97,32 +97,32 @@
         self._sample_sheet_path_hk = hk_path
 
     def get_sample_sheet_path_hk(self) -> Path:
         if not self._sample_sheet_path_hk:
             raise FlowCellError("Attribute _sample_sheet_path_hk has not been assigned yet")
         return self._sample_sheet_path_hk
 
-    def get_flow_cell_run_dir(self) -> Path:
+    def get_sequencing_runs_dir(self) -> Path:
         """
-        Return the flow cells run directory regardless of the path used to initialise the FlowCellsDirectoryData.
+        Return the flow cells run directory regardless of the path used to initialise the IlluminaRunDirectoryData.
         """
         current_path: str = self.path.as_posix()
         if DemultiplexingDirsAndFiles.DEMULTIPLEXED_RUNS_DIRECTORY_NAME in current_path:
             return Path(
                 str.replace(
                     current_path,
                     DemultiplexingDirsAndFiles.DEMULTIPLEXED_RUNS_DIRECTORY_NAME,
                     DemultiplexingDirsAndFiles.FLOW_CELLS_DIRECTORY_NAME,
                 )
             )
         return self.path
 
     def get_demultiplexed_runs_dir(self) -> Path:
         """
-        Return the demultiplexed run directory regardless of the path used to initialise the FlowCellsDirectoryData.
+        Return the demultiplexed run directory regardless of the path used to initialise the IlluminaRunDirectoryData.
         """
         current_path: str = self.path.as_posix()
         if DemultiplexingDirsAndFiles.FLOW_CELLS_DIRECTORY_NAME in current_path:
             return Path(
                 str.replace(
                     current_path,
                     DemultiplexingDirsAndFiles.FLOW_CELLS_DIRECTORY_NAME,
@@ -131,22 +131,22 @@
             )
         return self.path
 
     @property
     def run_parameters_path(self) -> Path:
         """Return path to run parameters file if it exists.
         Raises:
-            FlowCellError if the flow cell has no run parameters file."""
-        flow_cell_run_dir: Path = self.get_flow_cell_run_dir()
+            FlowCellError if the sequencing run has no run parameters file."""
+        flow_cell_run_dir: Path = self.get_sequencing_runs_dir()
         if DemultiplexingDirsAndFiles.RUN_PARAMETERS_PASCAL_CASE in os.listdir(flow_cell_run_dir):
             return Path(flow_cell_run_dir, DemultiplexingDirsAndFiles.RUN_PARAMETERS_PASCAL_CASE)
         elif DemultiplexingDirsAndFiles.RUN_PARAMETERS_CAMEL_CASE in os.listdir(flow_cell_run_dir):
             return Path(flow_cell_run_dir, DemultiplexingDirsAndFiles.RUN_PARAMETERS_CAMEL_CASE)
         else:
-            message: str = f"No run parameters file found in flow cell {flow_cell_run_dir}"
+            message: str = f"No run parameters file found in sequencing run {flow_cell_run_dir}"
             LOG.error(message)
             raise FlowCellError(message)
 
     @property
     def run_parameters(self) -> RunParameters:
         """Return run parameters object."""
         if not self._run_parameters:
@@ -171,15 +171,15 @@
     def copy_complete_path(self) -> Path:
         """Return copy complete path."""
         return Path(self.path, DemultiplexingDirsAndFiles.COPY_COMPLETE)
 
     @property
     def demultiplexing_started_path(self) -> Path:
         """Return demux started path."""
-        flow_cell_run_dir: Path = self.get_flow_cell_run_dir()
+        flow_cell_run_dir: Path = self.get_sequencing_runs_dir()
         return Path(flow_cell_run_dir, DemultiplexingDirsAndFiles.DEMUX_STARTED)
 
     @property
     def demultiplex_software_info_path(self) -> Path:
         """Return demultiplex software info path."""
         demux_run_dir = self.get_demultiplexed_runs_dir()
         return Path(demux_run_dir, DemultiplexingDirsAndFiles.DEMUX_VERSION_FILE)
@@ -197,26 +197,28 @@
 
     @property
     def is_demultiplexing_complete(self) -> bool:
         return Path(self.demux_complete_path).exists()
 
     def _parse_date(self):
         """Return the parsed date in the correct format."""
-        if len(self.split_flow_cell_name[0]) == LENGTH_LONG_DATE:
-            return datetime.datetime.strptime(self.split_flow_cell_name[0], "%Y%m%d")
-        return datetime.datetime.strptime(self.split_flow_cell_name[0], "%y%m%d")
+        if len(self.split_sequencing_run_name[0]) == LENGTH_LONG_DATE:
+            return datetime.datetime.strptime(self.split_sequencing_run_name[0], "%Y%m%d")
+        return datetime.datetime.strptime(self.split_sequencing_run_name[0], "%y%m%d")
 
-    def validate_flow_cell_dir_name(self) -> None:
+    def validate_sequencing_run_dir_name(self) -> None:
         """
         Validate on the following criteria:
         Convention is: <date>_<machine>_<run_numbers>_<A|B><flow_cell_id>
         Example: '230912_A00187_1009_AHK33MDRX3'.
         """
-        if len(self.split_flow_cell_name) != 4:
-            message = f"Flowcell {self.full_name} does not follow the flow cell naming convention"
+        if len(self.split_sequencing_run_name) != 4:
+            message = (
+                f"Flowcell {self.full_name} does not follow the sequencing run naming convention"
+            )
             LOG.warning(message)
             raise FlowCellError(message)
 
     def has_demultiplexing_started_locally(self) -> bool:
         """Check if demultiplexing has started path exists on the cluster."""
         return self.demultiplexing_started_path.exists()
 
@@ -247,41 +249,41 @@
         """Check if sequencing is done.
         This is indicated by that the file RTAComplete.txt exists.
         """
         LOG.info("Check if sequencing is done")
         return self.rta_complete_path.exists()
 
     def is_copy_completed(self) -> bool:
-        """Check if copy of flow cell is done.
+        """Check if copy of sequencing run is done.
         This is indicated by that the file CopyComplete.txt exists.
         """
         LOG.info("Check if copy of data from sequence instrument is ready")
         return self.copy_complete_path.exists()
 
-    def is_flow_cell_ready(self) -> bool:
-        """Check if a flow cell is ready for downstream processing.
+    def is_sequencing_run_ready(self) -> bool:
+        """Check if a sequencing run is ready for downstream processing.
 
-        A flow cell is ready if the two files RTAComplete.txt and CopyComplete.txt exist in the
-        flow cell directory.
+        A sequencing run is ready if the two files RTAComplete.txt and CopyComplete.txt exist in the
+        sequencing run directory.
         """
-        LOG.info("Check if flow cell is ready for downstream processing")
+        LOG.info("Check if sequencing run is ready for downstream processing")
         if not self.is_sequencing_done():
-            LOG.warning(f"Sequencing is not completed for flow cell {self.id}")
+            LOG.warning(f"Sequencing is not completed for sequencing run {self.id}")
             return False
-        LOG.debug(f"Sequence is done for flow cell {self.id}")
+        LOG.debug(f"Sequence is done for sequencing run {self.id}")
         if not self.is_copy_completed():
-            LOG.warning(f"Copy of sequence data is not ready for flow cell {self.id}")
+            LOG.warning(f"Copy of sequence data is not ready for sequencing run {self.id}")
             return False
-        LOG.debug(f"All data has been transferred for flow cell {self.id}")
-        LOG.info(f"Flow cell {self.id} is ready for downstream processing")
+        LOG.debug(f"All data has been transferred for sequencing run {self.id}")
+        LOG.info(f"Sequencing run {self.id} is ready for downstream processing")
         return True
 
     def get_run_completion_status(self) -> Path | None:
         """Return the run completion status path."""
-        flow_cells_dir: Path = self.get_flow_cell_run_dir()
+        flow_cells_dir: Path = self.get_sequencing_runs_dir()
         file_path = Path(flow_cells_dir, DemultiplexingDirsAndFiles.RUN_COMPLETION_STATUS)
         if file_path.exists():
             return file_path
         return None
 
     @property
     def sequencing_started_at(self) -> datetime.datetime | None:
@@ -293,15 +295,15 @@
     def sequencing_completed_at(self) -> datetime.datetime | None:
         parser = ParseRunCompletionStatusService()
         file_path: Path = self.get_run_completion_status()
         return parser.get_end_time(file_path) if file_path else None
 
     @property
     def demultiplexing_started_at(self) -> datetime.datetime | None:
-        """Get the demultiplexing started time stamp from the flow cell run dir."""
+        """Get the demultiplexing started time stamp from the sequencing run dir."""
         try:
             time: float = get_source_creation_time_stamp(self.demultiplexing_started_path)
             return format_time_from_ctime(time)
         except FileNotFoundError:
             return None
 
     @property
@@ -313,21 +315,21 @@
         except FileNotFoundError:
             return None
 
     def __str__(self):
         return f"FlowCell(path={self.path},run_parameters_path={self.run_parameters_path})"
 
 
-def get_flow_cells_from_path(flow_cells_dir: Path) -> list[FlowCellDirectoryData]:
-    """Return flow cell objects from flow cell dir."""
-    flow_cells: list[FlowCellDirectoryData] = []
-    LOG.debug(f"Search for flow cells ready to encrypt in {flow_cells_dir}")
-    for flow_cell_dir in flow_cells_dir.iterdir():
-        if not flow_cell_dir.is_dir():
+def get_sequencing_runs_from_path(sequencing_run_dir: Path) -> list[IlluminaRunDirectoryData]:
+    """Return sequencing run objects from sequencing run dir."""
+    sequencing_runs: list[IlluminaRunDirectoryData] = []
+    LOG.debug(f"Search for flow cells ready to encrypt in {sequencing_run_dir}")
+    for run_dir in sequencing_run_dir.iterdir():
+        if not run_dir.is_dir():
             continue
-        LOG.debug(f"Found directory: {flow_cell_dir}")
+        LOG.debug(f"Found directory: {run_dir}")
         try:
-            flow_cell = FlowCellDirectoryData(flow_cell_path=flow_cell_dir)
+            sequencing_run = IlluminaRunDirectoryData(sequencing_run_path=run_dir)
         except FlowCellError:
             continue
-        flow_cells.append(flow_cell)
-    return flow_cells
+        sequencing_runs.append(sequencing_run)
+    return sequencing_runs
```

### Comparing `cg-60.9.1/cg/models/invoice/invoice.py` & `cg-60.9.3/cg/models/invoice/invoice.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/models/lims/sample.py` & `cg-60.9.3/cg/models/lims/sample.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/models/mip/mip_config.py` & `cg-60.9.3/cg/models/mip/mip_config.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/models/mip/mip_metrics_deliverables.py` & `cg-60.9.3/cg/models/mip/mip_metrics_deliverables.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/models/mip/mip_sample_info.py` & `cg-60.9.3/cg/models/mip/mip_sample_info.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/models/nf_analysis.py` & `cg-60.9.3/cg/models/nf_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/models/observations/input_files.py` & `cg-60.9.3/cg/models/observations/input_files.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/models/orders/constants.py` & `cg-60.9.3/cg/models/orders/constants.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/models/orders/excel_sample.py` & `cg-60.9.3/cg/models/orders/excel_sample.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/models/orders/json_sample.py` & `cg-60.9.3/cg/models/orders/json_sample.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/models/orders/order.py` & `cg-60.9.3/cg/models/orders/order.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/models/orders/orderform_schema.py` & `cg-60.9.3/cg/models/orders/orderform_schema.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/models/orders/sample_base.py` & `cg-60.9.3/cg/models/orders/sample_base.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/models/orders/samples.py` & `cg-60.9.3/cg/models/orders/samples.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/models/orders/validators/excel_sample_validators.py` & `cg-60.9.3/cg/models/orders/validators/excel_sample_validators.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/models/orders/validators/json_sample_validators.py` & `cg-60.9.3/cg/models/orders/validators/json_sample_validators.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/models/raredisease/raredisease.py` & `cg-60.9.3/cg/models/raredisease/raredisease.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/models/report/metadata.py` & `cg-60.9.3/cg/models/report/metadata.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/models/report/report.py` & `cg-60.9.3/cg/models/report/report.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/models/report/sample.py` & `cg-60.9.3/cg/models/report/sample.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/models/report/validators.py` & `cg-60.9.3/cg/models/report/validators.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/models/rnafusion/rnafusion.py` & `cg-60.9.3/cg/models/rnafusion/rnafusion.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/models/scout/scout_load_config.py` & `cg-60.9.3/cg/models/scout/scout_load_config.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/models/slurm/sbatch.py` & `cg-60.9.3/cg/models/slurm/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/models/taxprofiler/taxprofiler.py` & `cg-60.9.3/cg/models/taxprofiler/taxprofiler.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/models/tomte/tomte.py` & `cg-60.9.3/cg/models/tomte/tomte.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/models/workflow/mutant.py` & `cg-60.9.3/cg/models/workflow/mutant.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/resources/__init__.py` & `cg-60.9.3/cg/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/resources/rnafusion_bundle_filenames.yaml` & `cg-60.9.3/cg/resources/rnafusion_bundle_filenames.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/resources/taxprofiler_bundle_filenames.yaml` & `cg-60.9.3/cg/resources/taxprofiler_bundle_filenames.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/resources/tomte_bundle_filenames.yaml` & `cg-60.9.3/cg/resources/tomte_bundle_filenames.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/server/admin.py` & `cg-60.9.3/cg/server/admin.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,20 +29,14 @@
 
 def view_priority(unused1, unused2, model, unused3):
     """column formatter for priority"""
     del unused1, unused2, unused3
     return Markup("%s" % model.priority.name) if model else ""
 
 
-def view_flow_cell_internal_id(unused1, unused2, model, unused3):
-    """column formatter for priority"""
-    del unused1, unused2, unused3
-    return Markup("%s" % model.device.internal_id)
-
-
 def view_case_sample_link(unused1, unused2, model, unused3):
     """column formatter to open the case-sample view"""
 
     del unused1, unused2, unused3
 
     return Markup(
         "<a href='%s'>%s</a>"
@@ -443,60 +437,14 @@
     column_searchable_list = [
         "case.internal_id",
         "case.name",
     ]
     form_extra_fields = {"workflow": SelectEnumField(enum_class=Workflow)}
 
 
-class IlluminaFlowCellView(BaseView):
-    """Admin view for Model.IlluminaSequencingRun"""
-
-    column_list = (
-        "internal_id",
-        "sequencer_type",
-        "sequencer_name",
-        "data_availability",
-        "has_backup",
-        "total_reads",
-        "total_undetermined_reads",
-        "percent_undetermined_reads",
-        "percent_q30",
-        "mean_quality_score",
-        "total_yield",
-        "yield_q30",
-        "cycles",
-        "demultiplexing_software",
-        "demultiplexing_software_version",
-        "sequencing_started_at",
-        "sequencing_completed_at",
-        "demultiplexing_started_at",
-        "demultiplexing_completed_at",
-        "archived_at",
-    )
-    column_formatters = {
-        "internal_id": view_flow_cell_internal_id,
-    }
-
-    column_default_sort = ("sequencing_completed_at", True)
-    column_filters = ["sequencer_type", "sequencer_name", "data_availability"]
-    column_editable_list = ["data_availability"]
-    column_searchable_list = ["sequencer_type", "sequencer_name", "device.internal_id"]
-    column_sortable_list = [
-        "sequencer_type",
-        "sequencer_name",
-        "data_availability",
-        "has_backup",
-        "sequencing_started_at",
-        "sequencing_completed_at",
-        "demultiplexing_started_at",
-        "demultiplexing_completed_at",
-        "archived_at",
-    ]
-
-
 class OrganismView(BaseView):
     """Admin view for Model.Organism"""
 
     column_default_sort = ("created_at", True)
     column_editable_list = ["internal_id", "name", "reference_genome", "comment"]
     column_searchable_list = ["internal_id", "name", "reference_genome"]
```

### Comparing `cg-60.9.1/cg/server/api.py` & `cg-60.9.3/cg/server/api.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/server/app.py` & `cg-60.9.3/cg/server/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,39 +2,39 @@
 import requests
 from flask import Flask, redirect, session, url_for
 from flask_admin.base import AdminIndexView
 from flask_dance.consumer import oauth_authorized
 from flask_dance.contrib.google import google, make_google_blueprint
 from sqlalchemy.orm import scoped_session
 
-from cg.server import admin, api, ext, invoices
 from cg.store.database import get_scoped_session_registry
 from cg.store.models import (
     Analysis,
     Application,
     ApplicationLimitations,
     ApplicationVersion,
     Bed,
     BedVersion,
     Case,
     CaseSample,
     Collaboration,
     Customer,
     Flowcell,
-    IlluminaSequencingRun,
     Invoice,
     Order,
     Organism,
     Panel,
     Pool,
     Sample,
     SampleLaneSequencingMetrics,
     User,
 )
 
+from . import admin, api, ext, invoices
+
 
 def create_app():
     """Generate a flask application."""
     app = Flask(__name__, template_folder="templates")
     _load_config(app)
     _configure_extensions(app)
     _register_blueprints(app)
@@ -124,17 +124,14 @@
     ext.admin.add_view(admin.CaseView(Case, ext.db.session))
     ext.admin.add_view(admin.CaseSampleView(CaseSample, ext.db.session))
     ext.admin.add_view(admin.SampleView(Sample, ext.db.session))
     ext.admin.add_view(admin.PoolView(Pool, ext.db.session))
     ext.admin.add_view(admin.FlowcellView(Flowcell, ext.db.session))
     ext.admin.add_view(admin.AnalysisView(Analysis, ext.db.session))
     ext.admin.add_view(admin.InvoiceView(Invoice, ext.db.session))
-    ext.admin.add_view(
-        admin.IlluminaFlowCellView(IlluminaSequencingRun, ext.db.session, name="Illumina Flow Cell")
-    )
 
 
 def _register_teardowns(app: Flask):
     """Register teardown functions."""
 
     @app.teardown_appcontext
     def remove_database_session(exception=None):
```

### Comparing `cg-60.9.1/cg/server/config.py` & `cg-60.9.3/cg/server/config.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/server/dto/orders/orders_request.py` & `cg-60.9.3/cg/server/dto/orders/orders_request.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/server/ext.py` & `cg-60.9.3/cg/server/ext.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/server/invoices/templates/invoices/index.html` & `cg-60.9.3/cg/server/invoices/templates/invoices/index.html`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/server/invoices/templates/invoices/invoice.html` & `cg-60.9.3/cg/server/invoices/templates/invoices/invoice.html`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/server/invoices/templates/invoices/layout.html` & `cg-60.9.3/cg/server/invoices/templates/invoices/layout.html`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/server/invoices/templates/invoices/new.html` & `cg-60.9.3/cg/server/invoices/templates/invoices/new.html`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/server/invoices/views.py` & `cg-60.9.3/cg/server/invoices/views.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/services/delivery_message/delivery_message_service.py` & `cg-60.9.3/cg/services/delivery_message/delivery_message_service.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/services/delivery_message/messages/__init__.py` & `cg-60.9.3/cg/services/delivery_message/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/services/delivery_message/messages/analysis_scout_message.py` & `cg-60.9.3/cg/services/delivery_message/messages/analysis_scout_message.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/services/delivery_message/messages/covid_message.py` & `cg-60.9.3/cg/services/delivery_message/messages/covid_message.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/services/delivery_message/messages/fastq_analysis_scout_message.py` & `cg-60.9.3/cg/services/delivery_message/messages/fastq_analysis_scout_message.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/services/delivery_message/messages/fastq_message.py` & `cg-60.9.3/cg/services/delivery_message/messages/fastq_message.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/services/delivery_message/messages/fastq_scout_message.py` & `cg-60.9.3/cg/services/delivery_message/messages/fastq_scout_message.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/services/delivery_message/messages/microsalt_mwr_message.py` & `cg-60.9.3/cg/services/delivery_message/messages/microsalt_mwr_message.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/services/delivery_message/messages/microsalt_mwx_message.py` & `cg-60.9.3/cg/services/delivery_message/messages/microsalt_mwx_message.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/services/delivery_message/messages/scout_message.py` & `cg-60.9.3/cg/services/delivery_message/messages/scout_message.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/services/delivery_message/messages/statina_message.py` & `cg-60.9.3/cg/services/delivery_message/messages/statina_message.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/services/delivery_message/messages/utils.py` & `cg-60.9.3/cg/services/delivery_message/messages/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/services/delivery_message/utils.py` & `cg-60.9.3/cg/services/delivery_message/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/services/fastq_concatenation_service/fastq_concatenation_service.py` & `cg-60.9.3/cg/services/fastq_concatenation_service/fastq_concatenation_service.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/services/fastq_concatenation_service/utils.py` & `cg-60.9.3/cg/services/fastq_concatenation_service/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/services/illumina_services/illumina_metrics_service/bcl_convert_metrics_parser.py` & `cg-60.9.3/cg/services/illumina_services/illumina_metrics_service/bcl_convert_metrics_parser.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/services/illumina_services/illumina_metrics_service/illumina_demux_version_service.py` & `cg-60.9.3/cg/services/illumina_services/illumina_metrics_service/illumina_demux_version_service.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/services/illumina_services/illumina_metrics_service/illumina_metrics_service.py` & `cg-60.9.3/cg/services/illumina_services/illumina_metrics_service/illumina_metrics_service.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from datetime import datetime
 from pathlib import Path
 
 from cg.constants import FlowCellStatus
 from cg.constants.demultiplexing import UNDETERMINED
 from cg.constants.devices import DeviceType
-from cg.models.flow_cell.flow_cell import FlowCellDirectoryData
+from cg.models.run_devices.illumina_run_directory_data import IlluminaRunDirectoryData
 from cg.services.illumina_services.illumina_metrics_service.bcl_convert_metrics_parser import (
     BCLConvertMetricsParser,
 )
 from cg.services.illumina_services.illumina_metrics_service.illumina_demux_version_service import (
     IlluminaDemuxVersionService,
 )
 from cg.services.illumina_services.illumina_metrics_service.models import (
@@ -39,15 +39,15 @@
                     sample_internal_id=sample_internal_id, lane=lane, metrics_parser=metrics_parser
                 )
                 sample_lane_sequencing_metrics.append(metrics)
         return sample_lane_sequencing_metrics
 
     def create_undetermined_non_pooled_metrics(
         self,
-        flow_cell: FlowCellDirectoryData,
+        flow_cell: IlluminaRunDirectoryData,
     ) -> list[SampleLaneSequencingMetrics]:
         """Return sequencing metrics for any undetermined reads in non-pooled lanes."""
 
         non_pooled_lanes_and_samples: list[tuple[int, str]] = (
             flow_cell.sample_sheet.get_non_pooled_lanes_and_samples()
         )
         metrics_parser = BCLConvertMetricsParser(flow_cell.path)
@@ -144,40 +144,40 @@
                     metrics_parser=metrics_parser,
                 )
                 sample_lane_sequencing_metrics.append(metrics)
         return sample_lane_sequencing_metrics
 
     @staticmethod
     def create_illumina_sequencing_dto(
-        flow_cell_dir_data: FlowCellDirectoryData,
+        demultiplexed_run_dir: IlluminaRunDirectoryData,
     ) -> IlluminaSequencingRunDTO:
-        metrics_parser = BCLConvertMetricsParser(flow_cell_dir_data.path)
+        metrics_parser = BCLConvertMetricsParser(demultiplexed_run_dir.path)
         total_reads: int = metrics_parser.get_total_reads_for_flow_cell()
         total_undetermined_reads: int = metrics_parser.get_undetermined_reads_for_flow_cell()
         percent_undetermined_reads: float = (
             metrics_parser.get_percent_undetermined_reads_for_flow_cell()
         )
         percent_q30: float = metrics_parser.get_mean_percent_q30_for_flow_cell()
         mean_quality_score: float = metrics_parser.get_mean_quality_score_sum_for_flow_cell()
         total_yield: int = metrics_parser.get_yield_for_flow_cell()
         yield_q30: int = metrics_parser.get_yield_q30_for_flow_cell()
-        cycles: int = flow_cell_dir_data.run_parameters.get_read_1_cycles()
+        cycles: int = demultiplexed_run_dir.run_parameters.get_read_1_cycles()
         software_service = IlluminaDemuxVersionService()
         demux_software: str = software_service.get_demux_software(
-            flow_cell_dir_data.demultiplex_software_info_path
+            demultiplexed_run_dir.demultiplex_software_info_path
         )
         demux_software_version: str = software_service.get_demux_software_version(
-            flow_cell_dir_data.demultiplex_software_info_path
+            demultiplexed_run_dir.demultiplex_software_info_path
         )
-        sequencing_started_at: datetime = flow_cell_dir_data.sequencing_started_at
-        sequencing_comleted_at: datetime = flow_cell_dir_data.sequencing_completed_at
-        demultiplexing_started_at: datetime = flow_cell_dir_data.demultiplexing_started_at
-        demultiplexing_completed_at: datetime = flow_cell_dir_data.demultiplexing_completed_at
-        sequencer_type: str = flow_cell_dir_data.sequencer_type
-        sequencer_name: str = flow_cell_dir_data.machine_name
+        sequencing_started_at: datetime = demultiplexed_run_dir.sequencing_started_at
+        sequencing_comleted_at: datetime = demultiplexed_run_dir.sequencing_completed_at
+        demultiplexing_started_at: datetime = demultiplexed_run_dir.demultiplexing_started_at
+        demultiplexing_completed_at: datetime = demultiplexed_run_dir.demultiplexing_completed_at
+        sequencer_type: str = demultiplexed_run_dir.sequencer_type
+        sequencer_name: str = demultiplexed_run_dir.machine_name
 
         return IlluminaSequencingRunDTO(
             sequencer_type=sequencer_type,
             sequencer_name=sequencer_name,
             data_availability=FlowCellStatus.ON_DISK,
             archived_at=None,
             has_backup=False,
```

### Comparing `cg-60.9.1/cg/services/illumina_services/illumina_metrics_service/models.py` & `cg-60.9.3/cg/services/illumina_services/illumina_metrics_service/models.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/services/illumina_services/illumina_post_processing_service/illumina_post_processing_service.py` & `cg-60.9.3/cg/services/illumina_services/illumina_post_processing_service/illumina_post_processing_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import logging
 from pathlib import Path
 
 from cg.apps.housekeeper.hk import HousekeeperAPI
 from cg.constants.devices import DeviceType
 from cg.exc import MissingFilesError, FlowCellError
-from cg.models.flow_cell.flow_cell import FlowCellDirectoryData
+from cg.models.run_devices.illumina_run_directory_data import IlluminaRunDirectoryData
 from cg.services.illumina_services.illumina_metrics_service.illumina_metrics_service import (
     IlluminaMetricsService,
 )
 from cg.services.illumina_services.illumina_metrics_service.models import (
     IlluminaFlowCellDTO,
     IlluminaSequencingRunDTO,
     IlluminaSampleSequencingMetricsDTO,
@@ -31,57 +31,57 @@
     def __init__(self, status_db: Store, housekeeper_api: HousekeeperAPI, dry_run: bool) -> None:
         self.status_db: Store = status_db
         self.hk_api: HousekeeperAPI = housekeeper_api
         self.dry_run: bool = dry_run
 
     def store_illumina_flow_cell(
         self,
-        flow_cell_dir_data: FlowCellDirectoryData,
+        flow_cell_dir_data: IlluminaRunDirectoryData,
     ) -> IlluminaFlowCell:
         """
         Create Illumina flow cell from the parsed and validated flow cell directory data.
         And add the samples on the flow cell to the model.
         """
         model: str | None = flow_cell_dir_data.run_parameters.get_flow_cell_model()
         flow_cell_dto = IlluminaFlowCellDTO(
             internal_id=flow_cell_dir_data.id, type=DeviceType.ILLUMINA, model=model
         )
         return self.status_db.add_illumina_flow_cell(flow_cell_dto)
 
     def store_illumina_sequencing_run(
         self,
-        flow_cell_dir_data: FlowCellDirectoryData,
+        flow_cell_dir_data: IlluminaRunDirectoryData,
         flow_cell: IlluminaFlowCell,
     ) -> IlluminaSequencingRun:
         """Store illumina run metrics in the status database."""
         metrics_service = IlluminaMetricsService()
         sequencing_run_dto: IlluminaSequencingRunDTO = (
             metrics_service.create_illumina_sequencing_dto(flow_cell_dir_data)
         )
         return self.status_db.add_illumina_sequencing_run(
             sequencing_run_dto=sequencing_run_dto, flow_cell=flow_cell
         )
 
     def store_illumina_sample_sequencing_metrics(
         self,
-        flow_cell_dir_data: FlowCellDirectoryData,
+        flow_cell_dir_data: IlluminaRunDirectoryData,
         sequencing_run: IlluminaSequencingRun,
     ):
         """Store illumina sample sequencing metrics in the status database."""
         metrics_service = IlluminaMetricsService()
         sample_metrics: list[IlluminaSampleSequencingMetricsDTO] = (
             metrics_service.create_sample_sequencing_metrics_dto_for_flow_cell(
                 flow_cell_directory=flow_cell_dir_data.path,
             )
         )
         return self.status_db.add_illumina_sample_metrics(
             sample_metrics_dto=sample_metrics, sequencing_run=sequencing_run
         )
 
-    def store_illumina_flow_cell_data(self, flow_cell_dir_data: FlowCellDirectoryData) -> None:
+    def store_illumina_flow_cell_data(self, flow_cell_dir_data: IlluminaRunDirectoryData) -> None:
         """Store flow cell data in the status database."""
         flow_cell: IlluminaFlowCell = self.store_illumina_flow_cell(
             flow_cell_dir_data=flow_cell_dir_data
         )
         sequencing_run: IlluminaSequencingRun = self.store_illumina_sequencing_run(
             flow_cell_dir_data=flow_cell_dir_data, flow_cell=flow_cell
         )
@@ -104,15 +104,15 @@
             - Creates a delivery file in the flow cell directory
         Raises:
             FlowCellError: If the flow cell directory or the data it contains is not valid.
         """
 
         LOG.info(f"Post-process flow cell {flow_cell_directory_name}")
         flow_cell_out_directory = Path(demultiplexed_runs_dir, flow_cell_directory_name)
-        flow_cell = FlowCellDirectoryData(flow_cell_out_directory)
+        flow_cell = IlluminaRunDirectoryData(flow_cell_out_directory)
         sample_sheet_path: Path = self.hk_api.get_sample_sheet_path(flow_cell.id)
         flow_cell.set_sample_sheet_path_hk(hk_path=sample_sheet_path)
 
         LOG.debug("Set path for Housekeeper sample sheet in flow cell")
         try:
             is_flow_cell_ready_for_postprocessing(
                 flow_cell_output_directory=flow_cell_out_directory,
```

### Comparing `cg-60.9.1/cg/services/illumina_services/illumina_post_processing_service/validation.py` & `cg-60.9.3/cg/services/illumina_services/illumina_post_processing_service/validation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import logging
 from pathlib import Path
 
 from cg.constants.demultiplexing import DemultiplexingDirsAndFiles
 from cg.exc import FlowCellError, MissingFilesError
 from cg.meta.demultiplex.utils import get_sample_fastqs_from_flow_cell
-from cg.models.flow_cell.flow_cell import FlowCellDirectoryData
+from cg.models.run_devices.illumina_run_directory_data import IlluminaRunDirectoryData
 
 LOG = logging.getLogger(__name__)
 
 
 def is_demultiplexing_complete(flow_cell_directory: Path) -> bool:
     return Path(flow_cell_directory, DemultiplexingDirsAndFiles.DEMUX_COMPLETE).exists()
 
 
 def is_flow_cell_ready_for_delivery(flow_cell_directory: Path) -> bool:
     return Path(flow_cell_directory, DemultiplexingDirsAndFiles.DELIVERY).exists()
 
 
-def validate_sample_sheet_exists(flow_cell: FlowCellDirectoryData) -> None:
+def validate_sample_sheet_exists(flow_cell: IlluminaRunDirectoryData) -> None:
     sample_sheet_path: Path = flow_cell.get_sample_sheet_path_hk()
     if not sample_sheet_path or not sample_sheet_path.exists():
         raise FlowCellError(f"Sample sheet {sample_sheet_path} does not exist in housekeeper.")
     LOG.debug(f"Found sample sheet {sample_sheet_path} in housekeeper.")
 
 
 def validate_demultiplexing_complete(flow_cell_output_directory: Path) -> None:
@@ -35,15 +35,15 @@
     if is_flow_cell_ready_for_delivery(flow_cell_output_directory) and not force:
         raise FlowCellError(
             f"Flow cell output directory {flow_cell_output_directory}"
             " has already been processed and is ready for delivery."
         )
 
 
-def validate_flow_cell_has_fastq_files(flow_cell: FlowCellDirectoryData) -> None:
+def validate_flow_cell_has_fastq_files(flow_cell: IlluminaRunDirectoryData) -> None:
     """Check if any sample from the flow cell has fastq files.
     Raises: MissingFilesError
         When all samples have missing fastq files in the flow cell
     """
     sample_ids: list[str] = flow_cell.sample_sheet.get_sample_ids()
     for sample_id in sample_ids:
         fastq_files: list[Path] | None = get_sample_fastqs_from_flow_cell(
@@ -55,15 +55,15 @@
     raise MissingFilesError(
         f"No fastq files were found for any sample in flow cell {flow_cell.id} path: {flow_cell.path}"
     )
 
 
 def is_flow_cell_ready_for_postprocessing(
     flow_cell_output_directory: Path,
-    flow_cell: FlowCellDirectoryData,
+    flow_cell: IlluminaRunDirectoryData,
     force: bool = False,
 ) -> None:
     validate_flow_cell_delivery_status(
         flow_cell_output_directory=flow_cell_output_directory, force=force
     )
     validate_sample_sheet_exists(flow_cell)
     validate_demultiplexing_complete(flow_cell_output_directory)
```

### Comparing `cg-60.9.1/cg/services/orders/order_service/order_service.py` & `cg-60.9.3/cg/services/orders/order_service/order_service.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/services/orders/order_service/utils.py` & `cg-60.9.3/cg/services/orders/order_service/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/services/orders/order_summary_service/order_summary_service.py` & `cg-60.9.3/cg/services/orders/order_summary_service/order_summary_service.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/services/orders/order_summary_service/utils.py` & `cg-60.9.3/cg/services/orders/order_summary_service/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/services/parse_run_completion_status_service/parse_run_completion_status_service.py` & `cg-60.9.3/cg/services/parse_run_completion_status_service/parse_run_completion_status_service.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/services/sequencing_qc_service/quality_checks/checks.py` & `cg-60.9.3/cg/services/sequencing_qc_service/quality_checks/checks.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/services/sequencing_qc_service/quality_checks/utils.py` & `cg-60.9.3/cg/services/sequencing_qc_service/quality_checks/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/services/sequencing_qc_service/sequencing_qc_service.py` & `cg-60.9.3/cg/services/sequencing_qc_service/sequencing_qc_service.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/services/slurm_service/slurm_cli_service.py` & `cg-60.9.3/cg/services/slurm_service/slurm_cli_service.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/services/slurm_upload_service/slurm_upload_service.py` & `cg-60.9.3/cg/services/slurm_upload_service/slurm_upload_service.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/services/validate_file_transfer_service/validate_file_transfer_service.py` & `cg-60.9.3/cg/services/validate_file_transfer_service/validate_file_transfer_service.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/services/validate_file_transfer_service/validate_pacbio_file_transfer_service.py` & `cg-60.9.3/cg/services/validate_file_transfer_service/validate_pacbio_file_transfer_service.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/store/base.py` & `cg-60.9.3/cg/store/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/store/crud/create.py` & `cg-60.9.3/cg/store/crud/create.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/store/crud/delete.py` & `cg-60.9.3/cg/store/crud/delete.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/store/crud/read.py` & `cg-60.9.3/cg/store/crud/read.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/store/crud/update.py` & `cg-60.9.3/cg/store/crud/update.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/store/database.py` & `cg-60.9.3/cg/store/database.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/store/filters/status_analysis_filters.py` & `cg-60.9.3/cg/store/filters/status_analysis_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/store/filters/status_application_filters.py` & `cg-60.9.3/cg/store/filters/status_application_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/store/filters/status_application_limitations_filters.py` & `cg-60.9.3/cg/store/filters/status_application_limitations_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/store/filters/status_application_version_filters.py` & `cg-60.9.3/cg/store/filters/status_application_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/store/filters/status_bed_filters.py` & `cg-60.9.3/cg/store/filters/status_bed_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/store/filters/status_bed_version_filters.py` & `cg-60.9.3/cg/store/filters/status_bed_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/store/filters/status_case_filters.py` & `cg-60.9.3/cg/store/filters/status_case_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/store/filters/status_case_sample_filters.py` & `cg-60.9.3/cg/store/filters/status_case_sample_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/store/filters/status_collaboration_filters.py` & `cg-60.9.3/cg/store/filters/status_collaboration_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/store/filters/status_customer_filters.py` & `cg-60.9.3/cg/store/filters/status_customer_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/store/filters/status_flow_cell_filters.py` & `cg-60.9.3/cg/store/filters/status_flow_cell_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/store/filters/status_illumina_flow_cell_filters.py` & `cg-60.9.3/cg/store/filters/status_illumina_flow_cell_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/store/filters/status_invoice_filters.py` & `cg-60.9.3/cg/store/filters/status_invoice_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/store/filters/status_metrics_filters.py` & `cg-60.9.3/cg/store/filters/status_metrics_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/store/filters/status_order_filters.py` & `cg-60.9.3/cg/store/filters/status_order_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/store/filters/status_organism_filters.py` & `cg-60.9.3/cg/store/filters/status_organism_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/store/filters/status_panel_filters.py` & `cg-60.9.3/cg/store/filters/status_panel_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/store/filters/status_pool_filters.py` & `cg-60.9.3/cg/store/filters/status_pool_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/store/filters/status_sample_filters.py` & `cg-60.9.3/cg/store/filters/status_sample_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/store/filters/status_user_filters.py` & `cg-60.9.3/cg/store/filters/status_user_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/store/models.py` & `cg-60.9.3/cg/store/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -402,15 +402,17 @@
     def to_dict(self):
         return to_dict(model_instance=self)
 
 
 class Collaboration(Base):
     __tablename__ = "collaboration"
     id: Mapped[PrimaryKeyInt]
-    internal_id: Mapped[Str32] = mapped_column(unique=True)
+    internal_id: Mapped[Str32] = mapped_column(
+        unique=True,
+    )
     name: Mapped[Str128]
     customers: Mapped[list[Customer]] = orm.relationship(
         secondary="customer_collaboration", back_populates="collaborations"
     )
 
     def __str__(self) -> str:
         return f"{self.internal_id} ({self.name})"
@@ -852,15 +854,15 @@
         if self.received_at:
             return f"Received {self.received_at.date()}"
 
         return f"Ordered {self.ordered_at.date()}"
 
     @property
     def _run_devices(self) -> list["RunDevice"]:
-        """Return the devices a sample has been sequenced on."""
+        """Return the run_devices a sample has been sequenced on."""
         return list({metric.run_metrics.device for metric in self._new_run_metrics})
 
     def to_dict(self, links: bool = False, flowcells: bool = False) -> dict:
         """Represent as dictionary"""
         data = to_dict(model_instance=self)
         data["priority"] = self.priority_human
         data["customer"] = self.customer.to_dict()
@@ -968,15 +970,15 @@
     is_delivered: Mapped[bool] = mapped_column(default=False)
 
     def to_dict(self):
         return to_dict(model_instance=self)
 
 
 class RunDevice(Base):
-    """Parent model for the different types of run devices."""
+    """Parent model for the different types of run run_devices."""
 
     __tablename__ = "run_device"
 
     id: Mapped[PrimaryKeyInt]
     type: Mapped[DeviceType]
     internal_id: Mapped[UniqueStr64]
```

### Comparing `cg-60.9.1/cg/store/store.py` & `cg-60.9.3/cg/store/store.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/utils/checksum/checksum.py` & `cg-60.9.3/cg/utils/checksum/checksum.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/utils/click/EnumChoice.py` & `cg-60.9.3/cg/utils/click/EnumChoice.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/utils/commands.py` & `cg-60.9.3/cg/utils/commands.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/utils/date.py` & `cg-60.9.3/cg/utils/date.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/utils/dict.py` & `cg-60.9.3/cg/utils/dict.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/utils/dispatcher.py` & `cg-60.9.3/cg/utils/dispatcher.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/utils/email.py` & `cg-60.9.3/cg/utils/email.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/utils/files.py` & `cg-60.9.3/cg/utils/files.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/utils/flask/enum.py` & `cg-60.9.3/cg/utils/flask/enum.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/utils/time.py` & `cg-60.9.3/cg/utils/time.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/cg/utils/utils.py` & `cg-60.9.3/cg/utils/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/pyproject.toml` & `cg-60.9.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "cg"
-version = "60.9.1"
+version = "60.9.3"
 description = "Clinical Genomics command center"
 authors = ["Clinical Genomics <support@clinicalgenomics.se>"]
 readme = "README.md"
 homepage = "https://github.com/Clinical-Genomics/cg"
 repository = "https://github.com/Clinical-Genomics/cg"
 classifiers = [
   "Programming Language :: Python",
```

### Comparing `cg-60.9.1/tests/apps/conftest.py` & `cg-60.9.3/tests/apps/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/apps/coverage/test_coverage.py` & `cg-60.9.3/tests/apps/coverage/test_coverage.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/apps/crunchy/conftest.py` & `cg-60.9.3/tests/apps/crunchy/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/apps/crunchy/test_compress_fastq.py` & `cg-60.9.3/tests/apps/crunchy/test_compress_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/apps/crunchy/test_config.py` & `cg-60.9.3/tests/apps/crunchy/test_config.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/apps/crunchy/test_crunchy.py` & `cg-60.9.3/tests/apps/crunchy/test_crunchy.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/apps/crunchy/test_spring_decompression.py` & `cg-60.9.3/tests/apps/crunchy/test_spring_decompression.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/apps/demultiplex/conftest.py` & `cg-60.9.3/tests/apps/demultiplex/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/apps/demultiplex/test_create_sample_sheet.py` & `cg-60.9.3/tests/apps/demultiplex/test_create_sample_sheet.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import pytest
 from _pytest.logging import LogCaptureFixture
 from pytest_mock import MockFixture
 
 from cg.apps.demultiplex.sample_sheet.sample_models import FlowCellSample
 from cg.exc import HousekeeperFileMissingError
 from cg.models.cg_config import CGConfig
-from cg.models.flow_cell.flow_cell import FlowCellDirectoryData
+from cg.models.run_devices.illumina_run_directory_data import IlluminaRunDirectoryData
 from tests.store_helpers import StoreHelpers
 
 GET_FLOW_CELL_SAMPLES: str = "cg.apps.demultiplex.sample_sheet.api.get_flow_cell_samples"
 
 
 def test_get_create_sample_sheet_hk_has_bcl2fastq_sample_sheet(
     sample_sheet_context_broken_flow_cells: CGConfig,
@@ -24,15 +24,15 @@
 ):
     """Test that a BCL2FASTQ sample sheet in Housekeeper is updated to BCLConvert."""
     # GIVEN a sample sheet context with a sample sheet API and a Housekeeper API
     sample_sheet_api = sample_sheet_context_broken_flow_cells.sample_sheet_api
     hk_api = sample_sheet_context_broken_flow_cells.housekeeper_api
 
     # GIVEN a a flow cell with a BCL2FASTQ sample sheet going to be updated to BCLConvert
-    flow_cell = FlowCellDirectoryData(tmp_flow_cell_with_bcl2fastq_sample_sheet)
+    flow_cell = IlluminaRunDirectoryData(tmp_flow_cell_with_bcl2fastq_sample_sheet)
 
     # GIVEN that the sample sheet is in Housekeeper
     helpers.ensure_hk_bundle(store=hk_api, bundle_data=sample_sheet_bcl2fastq_bundle_data)
     sample_sheet_path_hk: Path = hk_api.get_sample_sheet_path(flow_cell.id)
 
     # GIVEN that the flow cell samples are in LIMS
     mocker.patch(
@@ -62,15 +62,15 @@
     and added to Housekeeeper.
     """
     # GIVEN a sample sheet context with a sample sheet API and a Housekeeper API
     sample_sheet_api = sample_sheet_context_broken_flow_cells.sample_sheet_api
     hk_api = sample_sheet_context_broken_flow_cells.housekeeper_api
 
     # GIVEN a a flow cell with a BCL2FASTQ sample sheet going to be updated to BCLConvert
-    flow_cell = FlowCellDirectoryData(tmp_flow_cell_with_bcl2fastq_sample_sheet)
+    flow_cell = IlluminaRunDirectoryData(tmp_flow_cell_with_bcl2fastq_sample_sheet)
 
     # GIVEN that the sample sheet is not in Housekeeper
     with pytest.raises(HousekeeperFileMissingError):
         hk_api.get_sample_sheet_path(flow_cell.id)
     assert f"Sample sheet file for flowcell {flow_cell.id} not found in Housekeeper!" in caplog.text
 
     # GIVEN that the flow cell samples are in LIMS
```

### Comparing `cg-60.9.1/tests/apps/demultiplex/test_demultiplex_api.py` & `cg-60.9.3/tests/apps/demultiplex/test_demultiplex_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 
 from cg.apps.demultiplex.demultiplex_api import DemultiplexingAPI
 from cg.constants.demultiplexing import DemultiplexingDirsAndFiles
 from cg.meta.demultiplex.housekeeper_storage_functions import (
     add_and_include_sample_sheet_path_to_housekeeper,
 )
 from cg.models.cg_config import CGConfig
-from cg.models.flow_cell.flow_cell import FlowCellDirectoryData
+from cg.models.run_devices.illumina_run_directory_data import IlluminaRunDirectoryData
 
 
 def test_is_sample_sheet_in_housekeeper_exists(
-    demultiplexing_context_for_demux: CGConfig, tmp_bcl_convert_flow_cell: FlowCellDirectoryData
+    demultiplexing_context_for_demux: CGConfig, tmp_bcl_convert_flow_cell: IlluminaRunDirectoryData
 ):
     """Test that checking the existence of an existing sample sheet in Housekeeper returns True."""
     # GIVEN a DemultiplexAPI and a flow cell with a sample sheet
     demux_api: DemultiplexingAPI = demultiplexing_context_for_demux.demultiplex_api
     demultiplexing_context_for_demux.illumina_flow_cells_directory = (
         tmp_bcl_convert_flow_cell.path.parent
     )
@@ -36,15 +36,15 @@
     )
 
     # THEN the sample sheet should be in Housekeeper
     assert result
 
 
 def test_is_sample_sheet_in_housekeeper_not_in_hk(
-    demultiplexing_context_for_demux: CGConfig, tmp_bcl_convert_flow_cell: FlowCellDirectoryData
+    demultiplexing_context_for_demux: CGConfig, tmp_bcl_convert_flow_cell: IlluminaRunDirectoryData
 ):
     """Test that checking the existence of a non-existing sample sheet in Housekeeper returns False."""
     # GIVEN a DemultiplexAPI and a flow cell with a sample sheet
     demux_api: DemultiplexingAPI = demultiplexing_context_for_demux.demultiplex_api
     demultiplexing_context_for_demux.illumina_flow_cells_directory = (
         tmp_bcl_convert_flow_cell.path.parent
     )
@@ -57,15 +57,15 @@
     )
 
     # THEN the sample sheet should be in Housekeeper
     assert not result
 
 
 def test_create_demultiplexing_output_dir_for_bcl_convert(
-    tmp_bcl_convert_flow_cell: FlowCellDirectoryData,
+    tmp_bcl_convert_flow_cell: IlluminaRunDirectoryData,
     tmp_path: Path,
     demultiplexing_api: DemultiplexingAPI,
 ):
     """Test that the correct demultiplexing output directory is created."""
     # GIVEN BCL Convert FlowCellDirectoryData object
 
     # GIVEN that the demultiplexing output directory does not exist
@@ -83,15 +83,15 @@
     # THEN the demultiplexing output directory should exist
     assert output_directory.exists()
     assert not unaligned_directory.exists()
 
 
 def test_is_demultiplexing_possible_true(
     demultiplexing_api: DemultiplexingAPI,
-    tmp_bcl_convert_flow_cell: FlowCellDirectoryData,
+    tmp_bcl_convert_flow_cell: IlluminaRunDirectoryData,
 ):
     """Test demultiplexing pre-check when all criteria are fulfilled."""
     add_and_include_sample_sheet_path_to_housekeeper(
         flow_cell_directory=tmp_bcl_convert_flow_cell.path,
         flow_cell_name=tmp_bcl_convert_flow_cell.id,
         hk_api=demultiplexing_api.hk_api,
     )
@@ -105,15 +105,15 @@
     assert result is True
 
 
 @pytest.mark.parametrize("missing_file", ["RTAComplete.txt", "CopyComplete.txt", "SampleSheet.csv"])
 def test_is_demultiplexing_possible_missing_files(
     demultiplexing_api: DemultiplexingAPI,
     missing_file: str,
-    tmp_bcl_convert_flow_cell: FlowCellDirectoryData,
+    tmp_bcl_convert_flow_cell: IlluminaRunDirectoryData,
 ):
     """Test demultiplexing pre-check when files are missing in flow cell directory."""
     # GIVEN a flow cell with a sample sheet in Housekeeper
     add_and_include_sample_sheet_path_to_housekeeper(
         flow_cell_directory=tmp_bcl_convert_flow_cell.path,
         flow_cell_name=tmp_bcl_convert_flow_cell.id,
         hk_api=demultiplexing_api.hk_api,
@@ -133,15 +133,15 @@
     )
     # THEN the flow cell should not be deemed ready for demultiplexing
     assert result is False
 
 
 def is_demultiplexing_possible_no_sample_sheet_in_hk(
     demultiplexing_api: DemultiplexingAPI,
-    tmp_bcl_convert_flow_cell: FlowCellDirectoryData,
+    tmp_bcl_convert_flow_cell: IlluminaRunDirectoryData,
 ):
     """Test demultiplexing pre-check when no sample sheet exists in Housekeeper."""
     # GIVEN a flow cell with no sample sheet in Housekeeper
     assert (
         demultiplexing_api.is_sample_sheet_in_housekeeper(flow_cell_id=tmp_bcl_convert_flow_cell.id)
         is False
     )
@@ -152,15 +152,15 @@
     )
     # THEN the flow cell should not be deemed ready for demultiplexing
     assert result is False
 
 
 def test_is_demultiplexing_possible_already_started(
     demultiplexing_api: DemultiplexingAPI,
-    tmp_bcl_convert_flow_cell: FlowCellDirectoryData,
+    tmp_bcl_convert_flow_cell: IlluminaRunDirectoryData,
 ):
     """Test demultiplexing pre-check demultiplexing has already started."""
     # GIVEN a flow cell with a sample sheet in Housekeeper
     add_and_include_sample_sheet_path_to_housekeeper(
         flow_cell_directory=tmp_bcl_convert_flow_cell.path,
         flow_cell_name=tmp_bcl_convert_flow_cell.id,
         hk_api=demultiplexing_api.hk_api,
@@ -180,15 +180,15 @@
     # THEN the flow cell should not be deemed ready for demultiplexing
     assert result is False
 
 
 def test_remove_demultiplexing_output_directory(
     demultiplexing_api: DemultiplexingAPI,
     tmp_path: Path,
-    novaseq_6000_post_1_5_kits_flow_cell: FlowCellDirectoryData,
+    novaseq_6000_post_1_5_kits_flow_cell: IlluminaRunDirectoryData,
 ):
     """Test that the demultiplexing output directory is removed."""
     # GIVEN a flow cell with a demultiplexing output directory
     demultiplexing_api.demultiplexed_runs_dir = tmp_path
     demultiplexing_api.create_demultiplexing_output_dir(novaseq_6000_post_1_5_kits_flow_cell)
     assert demultiplexing_api.flow_cell_out_dir_path(novaseq_6000_post_1_5_kits_flow_cell).exists()
```

### Comparing `cg-60.9.1/tests/apps/demultiplex/test_index.py` & `cg-60.9.3/tests/apps/demultiplex/test_index.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/apps/demultiplex/test_override_cycles_validator.py` & `cg-60.9.3/tests/apps/demultiplex/test_override_cycles_validator.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/apps/demultiplex/test_read_sample_sheet.py` & `cg-60.9.3/tests/apps/demultiplex/test_read_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/apps/demultiplex/test_sample_models.py` & `cg-60.9.3/tests/apps/demultiplex/test_sample_models.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/apps/demultiplex/test_sample_sheet_creator.py` & `cg-60.9.3/tests/apps/demultiplex/test_sample_sheet_creator.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/apps/demultiplex/test_sample_sheet_models.py` & `cg-60.9.3/tests/apps/demultiplex/test_sample_sheet_models.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/apps/demultiplex/test_sample_sheet_validator.py` & `cg-60.9.3/tests/apps/demultiplex/test_sample_sheet_validator.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/apps/demultiplex/test_translate_sample_sheet.py` & `cg-60.9.3/tests/apps/demultiplex/test_translate_sample_sheet.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,27 +2,29 @@
 
 import pytest
 from _pytest.logging import LogCaptureFixture
 
 from cg.apps.demultiplex.sample_sheet.api import SampleSheetAPI
 from cg.exc import SampleSheetError
 from cg.models.cg_config import CGConfig
-from cg.models.flow_cell.flow_cell import FlowCellDirectoryData
+from cg.models.run_devices.illumina_run_directory_data import IlluminaRunDirectoryData
 
 
 def test_are_necessary_files_in_flow_cell_passes(
     sample_sheet_context_broken_flow_cells: CGConfig,
     tmp_flow_cell_with_bcl2fastq_sample_sheet: Path,
 ):
     """Test that a flow cell with sample sheet and run parameters has necessary files."""
     # GIVEN a sample sheet API
     api: SampleSheetAPI = sample_sheet_context_broken_flow_cells.sample_sheet_api
 
     # GIVEN a flow cell with a sample sheet
-    flow_cell = FlowCellDirectoryData(flow_cell_path=tmp_flow_cell_with_bcl2fastq_sample_sheet)
+    flow_cell = IlluminaRunDirectoryData(
+        sequencing_run_path=tmp_flow_cell_with_bcl2fastq_sample_sheet
+    )
 
     # WHEN checking if the flow cell has the necessary files
     result: bool = api._are_necessary_files_in_flow_cell(flow_cell=flow_cell)
 
     # THEN assert that all files are present
     assert result
 
@@ -33,15 +35,17 @@
     caplog: LogCaptureFixture,
 ):
     """Test that a flow cell without run parameters can't have its sample sheet translated."""
     # GIVEN a sample sheet API
     api: SampleSheetAPI = sample_sheet_context_broken_flow_cells.sample_sheet_api
 
     # GIVEN a flow cell without run parameters
-    flow_cell = FlowCellDirectoryData(flow_cell_path=tmp_flow_cell_without_run_parameters_path)
+    flow_cell = IlluminaRunDirectoryData(
+        sequencing_run_path=tmp_flow_cell_without_run_parameters_path
+    )
 
     # WHEN checking if the flow cell has the necessary files
     result: bool = api._are_necessary_files_in_flow_cell(flow_cell)
 
     # THEN it returns False and informs that the run parameters are not present
     assert not result
     assert f"Run parameters file for flow cell {flow_cell.full_name} does not exist" in caplog.text
@@ -53,16 +57,16 @@
     caplog: LogCaptureFixture,
 ):
     """Test that a flow cell without sample sheet can not be translated."""
     # GIVEN a sample sheet API
     api: SampleSheetAPI = sample_sheet_context_broken_flow_cells.sample_sheet_api
 
     # GIVEN a flow cell without a sample sheet
-    flow_cell = FlowCellDirectoryData(
-        flow_cell_path=tmp_novaseq_x_without_sample_sheet_flow_cell_path
+    flow_cell = IlluminaRunDirectoryData(
+        sequencing_run_path=tmp_novaseq_x_without_sample_sheet_flow_cell_path
     )
 
     # WHEN checking if the flow cell has the necessary files
     result: bool = api._are_necessary_files_in_flow_cell(flow_cell)
 
     # THEN it returns False and informs that the sample sheet is not present
     assert not result
@@ -109,14 +113,16 @@
     tmp_flow_cell_with_bcl2fastq_sample_sheet: Path,
 ):
     """Test that a Bcl2Fastq sample sheet is translated to BCLConvert format."""
     # GIVEN a sample sheet API
     api: SampleSheetAPI = sample_sheet_context_broken_flow_cells.sample_sheet_api
 
     # GIVEN a flow cell with a translatable sample sheet
-    flow_cell = FlowCellDirectoryData(flow_cell_path=tmp_flow_cell_with_bcl2fastq_sample_sheet)
+    flow_cell = IlluminaRunDirectoryData(
+        sequencing_run_path=tmp_flow_cell_with_bcl2fastq_sample_sheet
+    )
 
     # WHEN translating the sample sheet
     api.translate_sample_sheet(flow_cell_name=flow_cell.full_name)
 
     # THEN the sample sheet is translated correctly to BCConvert format
     api.validate_sample_sheet(flow_cell.sample_sheet_path)
```

### Comparing `cg-60.9.1/tests/apps/demultiplex/test_validate.py` & `cg-60.9.3/tests/apps/demultiplex/test_validate.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/apps/downsample/test_downsample.py` & `cg-60.9.3/tests/apps/downsample/test_downsample.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/apps/downsample/test_downsample_utils.py` & `cg-60.9.3/tests/apps/downsample/test_downsample_utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/apps/gens/test_gens_api.py` & `cg-60.9.3/tests/apps/gens/test_gens_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/apps/gt/conftest.py` & `cg-60.9.3/tests/apps/gt/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/apps/gt/test_gt_api.py` & `cg-60.9.3/tests/apps/gt/test_gt_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/apps/hk/conftest.py` & `cg-60.9.3/tests/apps/hk/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/apps/hk/test__getattr__.py` & `cg-60.9.3/tests/apps/hk/test__getattr__.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/apps/hk/test_add_file.py` & `cg-60.9.3/tests/apps/hk/test_add_file.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/apps/hk/test_bundles.py` & `cg-60.9.3/tests/apps/hk/test_bundles.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/apps/hk/test_core.py` & `cg-60.9.3/tests/apps/hk/test_core.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/apps/hk/test_file.py` & `cg-60.9.3/tests/apps/hk/test_file.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/apps/hk/test_version.py` & `cg-60.9.3/tests/apps/hk/test_version.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/apps/lims/conftest.py` & `cg-60.9.3/tests/apps/lims/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/apps/lims/test_api.py` & `cg-60.9.3/tests/apps/lims/test_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/apps/lims/test_sample_sheet.py` & `cg-60.9.3/tests/apps/lims/test_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/apps/loqus/test_loqusdb_api.py` & `cg-60.9.3/tests/apps/loqus/test_loqusdb_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/apps/madeline/conftest.py` & `cg-60.9.3/tests/apps/madeline/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/apps/madeline/test_madeline.py` & `cg-60.9.3/tests/apps/madeline/test_madeline.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/apps/mip/conftest.py` & `cg-60.9.3/tests/apps/mip/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/apps/mip/test_config_mip.py` & `cg-60.9.3/tests/apps/mip/test_config_mip.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/apps/mutacc_auto/conftest.py` & `cg-60.9.3/tests/apps/mutacc_auto/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/apps/mutacc_auto/test_mutacc_auto.py` & `cg-60.9.3/tests/apps/mutacc_auto/test_mutacc_auto.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/apps/orderform/conftest.py` & `cg-60.9.3/tests/apps/orderform/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/apps/orderform/test_excel_orderform_parser.py` & `cg-60.9.3/tests/apps/orderform/test_excel_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/apps/orderform/test_excel_sample_schema.py` & `cg-60.9.3/tests/apps/orderform/test_excel_sample_schema.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/apps/orderform/test_json_orderform_parser.py` & `cg-60.9.3/tests/apps/orderform/test_json_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/apps/orderform/test_orderform_parser.py` & `cg-60.9.3/tests/apps/orderform/test_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/apps/orderform/validators/test_excel_sample_validators.py` & `cg-60.9.3/tests/apps/orderform/validators/test_excel_sample_validators.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/apps/scout/conftest.py` & `cg-60.9.3/tests/apps/scout/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/apps/scout/test_get_causative_variants.py` & `cg-60.9.3/tests/apps/scout/test_get_causative_variants.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/apps/scout/test_get_scout_cases.py` & `cg-60.9.3/tests/apps/scout/test_get_scout_cases.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/apps/scout/test_scout_load_config.py` & `cg-60.9.3/tests/apps/scout/test_scout_load_config.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/apps/scout/test_scout_models.py` & `cg-60.9.3/tests/apps/scout/test_scout_models.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/apps/slurm/conftest.py` & `cg-60.9.3/tests/apps/slurm/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/apps/slurm/test_slurm_api.py` & `cg-60.9.3/tests/apps/slurm/test_slurm_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/apps/test_apps_environ.py` & `cg-60.9.3/tests/apps/test_apps_environ.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/apps/test_osticket.py` & `cg-60.9.3/tests/apps/test_osticket.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/add/test_cli_add.py` & `cg-60.9.3/tests/cli/add/test_cli_add.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/add/test_cli_add_customer.py` & `cg-60.9.3/tests/cli/add/test_cli_add_customer.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/add/test_cli_add_family.py` & `cg-60.9.3/tests/cli/add/test_cli_add_family.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/add/test_cli_add_relationship.py` & `cg-60.9.3/tests/cli/add/test_cli_add_relationship.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/add/test_cli_add_sample.py` & `cg-60.9.3/tests/cli/add/test_cli_add_sample.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/backup/conftest.py` & `cg-60.9.3/tests/cli/backup/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/backup/test_backup_command.py` & `cg-60.9.3/tests/cli/backup/test_backup_command.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from click.testing import CliRunner
 from psutil import Process
 
 from cg.cli.backup import backup_flow_cells, encrypt_flow_cells, fetch_flow_cell
 from cg.constants import EXIT_SUCCESS, FileExtensions, FlowCellStatus
 from cg.models.cg_config import CGConfig
-from cg.models.flow_cell.flow_cell import FlowCellDirectoryData
+from cg.models.run_devices.illumina_run_directory_data import IlluminaRunDirectoryData
 from tests.store_helpers import StoreHelpers
 
 
 def test_backup_flow_cells(
     cli_runner: CliRunner,
     cg_context: CGConfig,
     caplog,
@@ -169,16 +169,16 @@
     mocker,
     flow_cell_name: str,
 ):
     """Test encrypt flow cell in dry run mode when sequencing is not done."""
     caplog.set_level(logging.DEBUG)
 
     # GIVEN flow cells that are being sequenced
-    mocker.patch.object(FlowCellDirectoryData, "is_flow_cell_ready")
-    FlowCellDirectoryData.is_flow_cell_ready.return_value = False
+    mocker.patch.object(IlluminaRunDirectoryData, "is_sequencing_run_ready")
+    IlluminaRunDirectoryData.is_sequencing_run_ready.return_value = False
 
     # GIVEN a flow cells directory
 
     # WHEN encrypting flow cells in dry run mode
     result = cli_runner.invoke(encrypt_flow_cells, ["--dry-run"], obj=cg_context)
 
     # THEN exits without any errors
@@ -197,16 +197,16 @@
     flow_cell_full_name: str,
     mocker,
 ):
     """Test encrypt flow cell in dry run mode when pending file exists"""
     caplog.set_level(logging.DEBUG)
 
     # GIVEN flow cells that are ready
-    mocker.patch.object(FlowCellDirectoryData, "is_flow_cell_ready")
-    FlowCellDirectoryData.is_flow_cell_ready.return_value = True
+    mocker.patch.object(IlluminaRunDirectoryData, "is_sequencing_run_ready")
+    IlluminaRunDirectoryData.is_sequencing_run_ready.return_value = True
 
     # GIVEN a pending flag file
     flow_cells_encrypt_dir = Path(cg_context.encryption.encryption_dir, flow_cell_full_name)
     flow_cells_encrypt_dir.mkdir(parents=True, exist_ok=True)
     Path(flow_cells_encrypt_dir, flow_cell_name).with_suffix(FileExtensions.PENDING).touch()
 
     # GIVEN a flow cells directory
@@ -230,16 +230,16 @@
     flow_cell_full_name: str,
     mocker,
 ):
     """Test encrypt flow cell in dry run mode when completed file exists"""
     caplog.set_level(logging.DEBUG)
 
     # GIVEN flow cells that are ready
-    mocker.patch.object(FlowCellDirectoryData, "is_flow_cell_ready")
-    FlowCellDirectoryData.is_flow_cell_ready.return_value = True
+    mocker.patch.object(IlluminaRunDirectoryData, "is_sequencing_run_ready")
+    IlluminaRunDirectoryData.is_sequencing_run_ready.return_value = True
 
     # GIVEN a complete flag file
     flow_cells_encrypt_dir = Path(cg_context.encryption.encryption_dir, flow_cell_full_name)
     flow_cells_encrypt_dir.mkdir(parents=True, exist_ok=True)
     Path(flow_cells_encrypt_dir, flow_cell_name).with_suffix(FileExtensions.COMPLETE).touch()
 
     # GIVEN a flow cells directory
```

### Comparing `cg-60.9.1/tests/cli/clean/conftest.py` & `cg-60.9.3/tests/cli/clean/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/clean/test_balsamic_clean.py` & `cg-60.9.3/tests/cli/clean/test_balsamic_clean.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/clean/test_clean_flow_cell.py` & `cg-60.9.3/tests/cli/clean/test_clean_flow_cell.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/clean/test_clean_hk_bundle_files.py` & `cg-60.9.3/tests/cli/clean/test_clean_hk_bundle_files.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/clean/test_hk_bundle_files.py` & `cg-60.9.3/tests/cli/clean/test_hk_bundle_files.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/clean/test_hk_case_bundle_files.py` & `cg-60.9.3/tests/cli/clean/test_hk_case_bundle_files.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/clean/test_microbial_clean.py` & `cg-60.9.3/tests/cli/clean/test_microbial_clean.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/clean/test_rsync_past_run_dirs.py` & `cg-60.9.3/tests/cli/clean/test_rsync_past_run_dirs.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/compress/conftest.py` & `cg-60.9.3/tests/cli/compress/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/compress/test_cli_compress_fastq.py` & `cg-60.9.3/tests/cli/compress/test_cli_compress_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/compress/test_cli_decompress_spring.py` & `cg-60.9.3/tests/cli/compress/test_cli_decompress_spring.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/compress/test_compress_helpers.py` & `cg-60.9.3/tests/cli/compress/test_compress_helpers.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/compress/test_store_fastq.py` & `cg-60.9.3/tests/cli/compress/test_store_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/conftest.py` & `cg-60.9.3/tests/cli/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/delete/test_cli_delete_case.py` & `cg-60.9.3/tests/cli/delete/test_cli_delete_case.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/delete/test_cli_delete_cases.py` & `cg-60.9.3/tests/cli/delete/test_cli_delete_cases.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/deliver/conftest.py` & `cg-60.9.3/tests/cli/deliver/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/deliver/test_deliver_base.py` & `cg-60.9.3/tests/cli/deliver/test_deliver_base.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/deliver/test_rsync_base.py` & `cg-60.9.3/tests/cli/deliver/test_rsync_base.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/deliver/test_run_deliver_cmd.py` & `cg-60.9.3/tests/cli/deliver/test_run_deliver_cmd.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/demultiplex/test_create_sample_sheet.py` & `cg-60.9.3/tests/cli/demultiplex/test_create_sample_sheet.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,53 +7,53 @@
 
 from cg.apps.demultiplex.sample_sheet.api import SampleSheetAPI
 from cg.apps.demultiplex.sample_sheet.sample_models import FlowCellSample
 from cg.cli.demultiplex.sample_sheet import create_sheet
 from cg.constants.process import EXIT_SUCCESS
 from cg.io.txt import read_txt
 from cg.models.cg_config import CGConfig
-from cg.models.flow_cell.flow_cell import FlowCellDirectoryData
+from cg.models.run_devices.illumina_run_directory_data import IlluminaRunDirectoryData
 
 GET_FLOW_CELL_SAMPLES: str = "cg.apps.demultiplex.sample_sheet.api.get_flow_cell_samples"
 
 
 def test_create_sample_sheet_no_run_parameters_fails(
     cli_runner: CliRunner,
     tmp_flow_cell_without_run_parameters_path: Path,
     sample_sheet_context_broken_flow_cells: CGConfig,
     hiseq_2500_custom_index_bcl_convert_lims_samples: list[FlowCellSample],
     caplog,
     mocker,
 ):
-    """Test that creating a flow cell sample sheet fails if there is no run parameters file."""
-    # GIVEN a flow cell directory with a non-existing sample sheet nor RunParameters file
-    flow_cell = FlowCellDirectoryData(tmp_flow_cell_without_run_parameters_path)
+    """Test that creating a sequencing run sample sheet fails if there is no run parameters file."""
+    # GIVEN a sequencing run directory with a non-existing sample sheet nor RunParameters file
+    flow_cell = IlluminaRunDirectoryData(tmp_flow_cell_without_run_parameters_path)
 
-    # GIVEN that the context's flow cell directory holds the given flow cell
+    # GIVEN that the context's sequencing run directory holds the given sequencing run
     assert (
         sample_sheet_context_broken_flow_cells.illumina_demultiplexed_runs_directory
         == flow_cell.path.parent.as_posix()
     )
 
-    # GIVEN flow cell samples
+    # GIVEN sequencing run samples
     mocker.patch(
         GET_FLOW_CELL_SAMPLES,
         return_value=hiseq_2500_custom_index_bcl_convert_lims_samples,
     )
 
     # WHEN running the create sample sheet command
     result: Result = cli_runner.invoke(
         create_sheet, [flow_cell.full_name], obj=sample_sheet_context_broken_flow_cells
     )
 
     # THEN the process exits with a non-zero exit code
     assert result.exit_code != EXIT_SUCCESS
 
     # THEN the correct information is communicated
-    assert "No run parameters file found in flow cell" in caplog.text
+    assert "No run parameters file found in sequencing run" in caplog.text
 
 
 class SampleSheetScenario(BaseModel):
     flow_cell_directory: str
     lims_samples: str
     correct_sample_sheet: str
 
@@ -73,33 +73,37 @@
         ),
         SampleSheetScenario(
             flow_cell_directory="tmp_novaseq_x_without_sample_sheet_flow_cell_path",
             lims_samples="novaseq_x_lims_samples",
             correct_sample_sheet="novaseq_x_correct_sample_sheet",
         ),
     ],
-    ids=["Old NovaSeq 6000 flow cell", "New NovaSeq 6000 flow cell", "NovaSeq X flow cell"],
+    ids=[
+        "Old NovaSeq 6000 sequencing run",
+        "New NovaSeq 6000 sequencing run",
+        "NovaSeq X sequencing run",
+    ],
 )
 def test_create_v2_sample_sheet(
     cli_runner: CliRunner,
     scenario: SampleSheetScenario,
     sample_sheet_context: CGConfig,
     mocker,
     request: FixtureRequest,
 ):
     """Test that creating a v2 sample sheet works."""
     # GIVEN a sample sheet context with a sample sheet api
     sample_sheet_api: SampleSheetAPI = sample_sheet_context.sample_sheet_api
 
-    # GIVEN a flow cell directory with some run parameters
+    # GIVEN a sequencing run directory with some run parameters
     flow_cell_directory: Path = request.getfixturevalue(scenario.flow_cell_directory)
-    flow_cell = FlowCellDirectoryData(flow_cell_directory)
+    flow_cell = IlluminaRunDirectoryData(flow_cell_directory)
     assert flow_cell.run_parameters_path.exists()
 
-    # GIVEN that there is no sample sheet in the flow cell dir
+    # GIVEN that there is no sample sheet in the sequencing run dir
     assert not flow_cell.sample_sheet_exists()
 
     # GIVEN that there are no sample sheet in Housekeeper
     assert not sample_sheet_context.housekeeper_api.get_sample_sheets_from_latest_version(
         flow_cell.id
     )
```

### Comparing `cg-60.9.1/tests/cli/demultiplex/test_demultiplex_flowcell.py` & `cg-60.9.3/tests/cli/demultiplex/test_demultiplex_flowcell.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,29 +8,29 @@
 from cg.apps.demultiplex.demultiplex_api import DemultiplexingAPI
 from cg.cli.demultiplex.demux import demultiplex_all, demultiplex_flow_cell
 from cg.constants.demultiplexing import DemultiplexingDirsAndFiles
 from cg.meta.demultiplex.housekeeper_storage_functions import (
     add_and_include_sample_sheet_path_to_housekeeper,
 )
 from cg.models.cg_config import CGConfig
-from cg.models.flow_cell.flow_cell import FlowCellDirectoryData
+from cg.models.run_devices.illumina_run_directory_data import IlluminaRunDirectoryData
 
 
 def test_demultiplex_dragen_flowcell(
     cli_runner: testing.CliRunner,
     tmp_flow_cell_directory_bcl_convert: Path,
     demultiplexing_context_for_demux: CGConfig,
     caplog,
     mocker,
 ):
     caplog.set_level(logging.INFO)
 
     # GIVEN that all files are present for Dragen demultiplexing
 
-    flow_cell = FlowCellDirectoryData(tmp_flow_cell_directory_bcl_convert)
+    flow_cell = IlluminaRunDirectoryData(tmp_flow_cell_directory_bcl_convert)
     add_and_include_sample_sheet_path_to_housekeeper(
         flow_cell_directory=tmp_flow_cell_directory_bcl_convert,
         flow_cell_name=flow_cell.id,
         hk_api=demultiplexing_context_for_demux.housekeeper_api,
     )
 
     # GIVEN a flow cell that is ready for demultiplexing
@@ -76,15 +76,17 @@
 
     # GIVEN a demultiplexing context with an API and correct structure
     demux_api: DemultiplexingAPI = demultiplexing_context_for_demux.demultiplex_api
     assert demux_api.flow_cells_dir == tmp_illumina_flow_cells_demux_all_directory
 
     # GIVEN sequenced flow cells with their sample sheet in Housekeeper
     for flow_cell_dir in tmp_illumina_flow_cells_demux_all_directory.iterdir():
-        flow_cell: FlowCellDirectoryData = FlowCellDirectoryData(flow_cell_path=flow_cell_dir)
+        flow_cell: IlluminaRunDirectoryData = IlluminaRunDirectoryData(
+            sequencing_run_path=flow_cell_dir
+        )
         add_and_include_sample_sheet_path_to_housekeeper(
             flow_cell_directory=flow_cell_dir,
             flow_cell_name=flow_cell.id,
             hk_api=demultiplexing_context_for_demux.housekeeper_api,
         )
         assert demultiplexing_context_for_demux.housekeeper_api.last_version(bundle=flow_cell.id)
 
@@ -98,19 +100,19 @@
     # THEN assert it exits without problems
     assert result.exit_code == 0
 
     # THEN assert it found the directory
     assert "Found directory" in caplog.text
 
     # THEN assert it found a flow cell that is ready for demultiplexing
-    assert f"Flow cell {flow_cell.id} is ready for downstream processing" in caplog.text
+    assert f"Sequencing run {flow_cell.id} is ready for downstream processing" in caplog.text
 
 
 def test_is_demultiplexing_complete(
-    hiseq_x_single_index_demultiplexed_flow_cell_with_sample_sheet: FlowCellDirectoryData,
+    hiseq_x_single_index_demultiplexed_flow_cell_with_sample_sheet: IlluminaRunDirectoryData,
 ):
     """Tests the is_demultiplexing_complete property of FlowCellDirectoryData."""
 
     # GIVEN a demultiplexing directory with a demuxcomplete.txt file
     assert Path(
         hiseq_x_single_index_demultiplexed_flow_cell_with_sample_sheet.path,
         DemultiplexingDirsAndFiles.DEMUX_COMPLETE,
@@ -119,15 +121,15 @@
     # WHEN checking if the demultiplexing is complete
 
     # THEN the property should return true
     assert hiseq_x_single_index_demultiplexed_flow_cell_with_sample_sheet.is_demultiplexing_complete
 
 
 def test_is_demultiplexing_not_complete(
-    hiseq_2500_dual_index_demux_runs_flow_cell: FlowCellDirectoryData,
+    hiseq_2500_dual_index_demux_runs_flow_cell: IlluminaRunDirectoryData,
 ):
     """Tests the is_demultiplexing_complete property of FlowCellDirectoryData."""
 
     # GIVEN a demultiplexing directory with a demuxcomplete.txt file
     assert not Path(
         hiseq_2500_dual_index_demux_runs_flow_cell.path,
         DemultiplexingDirsAndFiles.DEMUX_COMPLETE,
```

### Comparing `cg-60.9.1/tests/cli/demultiplex/test_finish_demux.py` & `cg-60.9.3/tests/cli/demultiplex/test_finish_demux.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/demultiplex/test_validate_sample_sheet.py` & `cg-60.9.3/tests/cli/demultiplex/test_validate_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/demultiplex/test_verify_syncing.py` & `cg-60.9.3/tests/cli/demultiplex/test_verify_syncing.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/downsample/test_cli_downsample.py` & `cg-60.9.3/tests/cli/downsample/test_cli_downsample.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/generate/report/conftest.py` & `cg-60.9.3/tests/cli/generate/report/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/generate/report/test_cli_delivery_report.py` & `cg-60.9.3/tests/cli/generate/report/test_cli_delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/generate/report/test_utils.py` & `cg-60.9.3/tests/cli/generate/report/test_utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/generate/test_cli_base.py` & `cg-60.9.3/tests/cli/generate/test_cli_base.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/get/test_cli_get.py` & `cg-60.9.3/tests/cli/get/test_cli_get.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/get/test_cli_get_analysis.py` & `cg-60.9.3/tests/cli/get/test_cli_get_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/get/test_cli_get_case.py` & `cg-60.9.3/tests/cli/get/test_cli_get_case.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/get/test_cli_get_flow_cell.py` & `cg-60.9.3/tests/cli/get/test_cli_get_flow_cell.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/get/test_cli_get_sample.py` & `cg-60.9.3/tests/cli/get/test_cli_get_sample.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/set/conftest.py` & `cg-60.9.3/tests/cli/set/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/set/test_cli_set_case.py` & `cg-60.9.3/tests/cli/set/test_cli_set_case.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/set/test_cli_set_cases.py` & `cg-60.9.3/tests/cli/set/test_cli_set_cases.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/set/test_cli_set_flowcell.py` & `cg-60.9.3/tests/cli/set/test_cli_set_flowcell.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     # THEN it should have been set
     assert result.exit_code == SUCCESS
 
 
 def test_set_flowcell_status(
     cli_runner: CliRunner, base_context: CGConfig, base_store: Store, helpers
 ):
-    """Test that the updated flow_cell get the status we send in."""
+    """Test that the updated run_devices get the status we send in."""
     # GIVEN a database with a flow cell
     flow_cell_name = helpers.add_flow_cell(base_store).name
     status = FlowCellStatus.statuses()[2]
     flow_cell_query = base_store._get_query(table=Flowcell)
     assert flow_cell_query.first().status != status
 
     # WHEN setting a flowcell
```

### Comparing `cg-60.9.1/tests/cli/set/test_cli_set_list_keys.py` & `cg-60.9.3/tests/cli/set/test_cli_set_list_keys.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/set/test_cli_set_sample.py` & `cg-60.9.3/tests/cli/set/test_cli_set_sample.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/set/test_cli_set_samples.py` & `cg-60.9.3/tests/cli/set/test_cli_set_samples.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/store/test_store.py` & `cg-60.9.3/tests/cli/store/test_store.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/test_base.py` & `cg-60.9.3/tests/cli/test_base.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/upload/conftest.py` & `cg-60.9.3/tests/cli/upload/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/upload/test_cli_scout.py` & `cg-60.9.3/tests/cli/upload/test_cli_scout.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/upload/test_cli_upload.py` & `cg-60.9.3/tests/cli/upload/test_cli_upload.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/upload/test_cli_upload_auto.py` & `cg-60.9.3/tests/cli/upload/test_cli_upload_auto.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/upload/test_cli_upload_delivery_report.py` & `cg-60.9.3/tests/cli/upload/test_cli_upload_delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/upload/test_cli_upload_fastq.py` & `cg-60.9.3/tests/cli/upload/test_cli_upload_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/upload/test_cli_upload_genotype.py` & `cg-60.9.3/tests/cli/upload/test_cli_upload_genotype.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/upload/test_cli_upload_gens.py` & `cg-60.9.3/tests/cli/upload/test_cli_upload_gens.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/upload/test_cli_upload_nipt.py` & `cg-60.9.3/tests/cli/upload/test_cli_upload_nipt.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/upload/test_cli_upload_nipt_ftp.py` & `cg-60.9.3/tests/cli/upload/test_cli_upload_nipt_ftp.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/upload/test_cli_upload_nipt_statina.py` & `cg-60.9.3/tests/cli/upload/test_cli_upload_nipt_statina.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/upload/test_cli_upload_observations.py` & `cg-60.9.3/tests/cli/upload/test_cli_upload_observations.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/workflow/balsamic/conftest.py` & `cg-60.9.3/tests/cli/workflow/balsamic/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py` & `cg-60.9.3/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/workflow/balsamic/test_compound_commands.py` & `cg-60.9.3/tests/cli/workflow/balsamic/test_compound_commands.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/workflow/balsamic/test_link.py` & `cg-60.9.3/tests/cli/workflow/balsamic/test_link.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/workflow/balsamic/test_report_deliver.py` & `cg-60.9.3/tests/cli/workflow/balsamic/test_report_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/workflow/balsamic/test_run.py` & `cg-60.9.3/tests/cli/workflow/balsamic/test_run.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/workflow/balsamic/test_store_housekeeper.py` & `cg-60.9.3/tests/cli/workflow/balsamic/test_store_housekeeper.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/workflow/conftest.py` & `cg-60.9.3/tests/cli/workflow/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/workflow/fastq/test_fastq_base.py` & `cg-60.9.3/tests/cli/workflow/fastq/test_fastq_base.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/workflow/fluffy/conftest.py` & `cg-60.9.3/tests/cli/workflow/fluffy/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py` & `cg-60.9.3/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/workflow/fluffy/test_cli_link.py` & `cg-60.9.3/tests/cli/workflow/fluffy/test_cli_link.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/workflow/fluffy/test_cli_run.py` & `cg-60.9.3/tests/cli/workflow/fluffy/test_cli_run.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/workflow/fluffy/test_cli_start.py` & `cg-60.9.3/tests/cli/workflow/fluffy/test_cli_start.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/workflow/fluffy/test_cli_store.py` & `cg-60.9.3/tests/cli/workflow/fluffy/test_cli_store.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/workflow/microsalt/conftest.py` & `cg-60.9.3/tests/cli/workflow/microsalt/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/workflow/microsalt/test_microsalt_case_config.py` & `cg-60.9.3/tests/cli/workflow/microsalt/test_microsalt_case_config.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/workflow/microsalt/test_microsalt_run.py` & `cg-60.9.3/tests/cli/workflow/microsalt/test_microsalt_run.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/workflow/mip/conftest.py` & `cg-60.9.3/tests/cli/workflow/mip/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/workflow/mip/test_cli_mip_base.py` & `cg-60.9.3/tests/cli/workflow/mip/test_cli_mip_base.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py` & `cg-60.9.3/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/workflow/mip/test_cli_mip_dna_manged_variants.py` & `cg-60.9.3/tests/cli/workflow/mip/test_cli_mip_dna_manged_variants.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/workflow/mip/test_cli_mip_dna_panel.py` & `cg-60.9.3/tests/cli/workflow/mip/test_cli_mip_dna_panel.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/workflow/mip/test_cli_mip_dna_run.py` & `cg-60.9.3/tests/cli/workflow/mip/test_cli_mip_dna_run.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/workflow/mip/test_cli_mip_dna_start.py` & `cg-60.9.3/tests/cli/workflow/mip/test_cli_mip_dna_start.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py` & `cg-60.9.3/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/workflow/mip/test_cli_mip_rna_link.py` & `cg-60.9.3/tests/cli/workflow/mip/test_cli_mip_rna_link.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/workflow/mip/test_cli_mip_rna_run.py` & `cg-60.9.3/tests/cli/workflow/mip/test_cli_mip_rna_run.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/workflow/mip/test_cli_mip_store.py` & `cg-60.9.3/tests/cli/workflow/mip/test_cli_mip_store.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/workflow/nf_analysis/test_cli_config_case.py` & `cg-60.9.3/tests/cli/workflow/nf_analysis/test_cli_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/workflow/nf_analysis/test_cli_metrics_deliver.py` & `cg-60.9.3/tests/cli/workflow/nf_analysis/test_cli_metrics_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/workflow/nf_analysis/test_cli_report_deliver.py` & `cg-60.9.3/tests/cli/workflow/nf_analysis/test_cli_report_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/workflow/nf_analysis/test_cli_run.py` & `cg-60.9.3/tests/cli/workflow/nf_analysis/test_cli_run.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/workflow/nf_analysis/test_cli_start.py` & `cg-60.9.3/tests/cli/workflow/nf_analysis/test_cli_start.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/workflow/nf_analysis/test_cli_store.py` & `cg-60.9.3/tests/cli/workflow/nf_analysis/test_cli_store.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/workflow/nf_analysis/test_cli_store_housekeeper.py` & `cg-60.9.3/tests/cli/workflow/nf_analysis/test_cli_store_housekeeper.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/workflow/nf_analysis/test_cli_workflow_base.py` & `cg-60.9.3/tests/cli/workflow/nf_analysis/test_cli_workflow_base.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/workflow/raredisease/test_cli_raredisease_compound_commands.py` & `cg-60.9.3/tests/cli/workflow/raredisease/test_cli_raredisease_compound_commands.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/workflow/test_cli_workflow.py` & `cg-60.9.3/tests/cli/workflow/test_cli_workflow.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/cli/workflow/test_cli_workflow_clean.py` & `cg-60.9.3/tests/cli/workflow/test_cli_workflow_clean.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/clients/arnold/conftest.py` & `cg-60.9.3/tests/clients/arnold/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/clients/arnold/test_arnold_api_client.py` & `cg-60.9.3/tests/clients/arnold/test_arnold_api_client.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/clients/janus/conftest.py` & `cg-60.9.3/tests/clients/janus/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/clients/janus/test_janus_api_client.py` & `cg-60.9.3/tests/clients/janus/test_janus_api_client.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/conftest.py` & `cg-60.9.3/tests/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 from cg.meta.workflow.raredisease import RarediseaseAnalysisAPI
 from cg.meta.workflow.rnafusion import RnafusionAnalysisAPI
 from cg.meta.workflow.taxprofiler import TaxprofilerAnalysisAPI
 from cg.meta.workflow.tomte import TomteAnalysisAPI
 from cg.models import CompressionData
 from cg.models.cg_config import CGConfig, PDCArchivingDirectory
 from cg.models.downsample.downsample_data import DownsampleData
-from cg.models.flow_cell.flow_cell import FlowCellDirectoryData
+from cg.models.run_devices.illumina_run_directory_data import IlluminaRunDirectoryData
 from cg.models.raredisease.raredisease import RarediseaseParameters, RarediseaseSampleSheetHeaders
 from cg.models.rnafusion.rnafusion import RnafusionParameters, RnafusionSampleSheetEntry
 from cg.models.taxprofiler.taxprofiler import TaxprofilerParameters, TaxprofilerSampleSheetEntry
 from cg.models.tomte.tomte import TomteParameters, TomteSampleSheetHeaders
 from cg.services.illumina_services.illumina_metrics_service.illumina_metrics_service import (
     IlluminaMetricsService,
 )
@@ -1253,15 +1253,15 @@
     return store
 
 
 @pytest.fixture
 def updated_store_with_demultiplexed_samples(
     store: Store,
     helpers: StoreHelpers,
-    seven_canonical_flow_cells: list[FlowCellDirectoryData],
+    seven_canonical_flow_cells: list[IlluminaRunDirectoryData],
     seven_canonical_flow_cells_selected_sample_ids: list[list[str]],
 ) -> Store:
     """Return a store with the 7 canonical flow cells with samples added to store."""
     for flow_cell, sample_internal_ids in zip(
         seven_canonical_flow_cells, seven_canonical_flow_cells_selected_sample_ids
     ):
         helpers.add_flow_cell_and_samples_with_sequencing_metrics(
@@ -3801,16 +3801,16 @@
 def flow_cell_encryption_api(
     cg_context: CGConfig, flow_cell_full_name: str
 ) -> FlowCellEncryptionAPI:
     flow_cell_encryption_api = FlowCellEncryptionAPI(
         binary_path=cg_context.encryption.binary_path,
         encryption_dir=Path(cg_context.backup.pdc_archiving_directory.current),
         dry_run=True,
-        flow_cell=FlowCellDirectoryData(
-            flow_cell_path=Path(cg_context.illumina_flow_cells_directory, flow_cell_full_name)
+        flow_cell=IlluminaRunDirectoryData(
+            sequencing_run_path=Path(cg_context.illumina_flow_cells_directory, flow_cell_full_name)
         ),
         pigz_binary_path=cg_context.pigz.binary_path,
         slurm_api=SlurmAPI(),
         sbatch_parameter=cg_context.backup.slurm_flow_cell_encryption.dict(),
         tar_api=TarAPI(binary_path=cg_context.tar.binary_path, dry_run=True),
     )
     flow_cell_encryption_api.slurm_api.set_dry_run(dry_run=True)
```

### Comparing `cg-60.9.1/tests/fixture_plugins/delivery_fixtures/bundle_fixtures.py` & `cg-60.9.3/tests/fixture_plugins/delivery_fixtures/bundle_fixtures.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixture_plugins/delivery_fixtures/context_fixtures.py` & `cg-60.9.3/tests/fixture_plugins/delivery_fixtures/context_fixtures.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixture_plugins/delivery_fixtures/path_fixtures.py` & `cg-60.9.3/tests/fixture_plugins/delivery_fixtures/path_fixtures.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixture_plugins/demultiplex_fixtures/flow_cell_fixtures.py` & `cg-60.9.3/tests/fixture_plugins/demultiplex_fixtures/flow_cell_fixtures.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,89 +1,89 @@
 """Fixtures for Illumina flow cell objects."""
 
 from pathlib import Path
 
 import pytest
 
 from cg.constants.demultiplexing import DemultiplexingDirsAndFiles
-from cg.models.flow_cell.flow_cell import FlowCellDirectoryData
+from cg.models.run_devices.illumina_run_directory_data import IlluminaRunDirectoryData
 
 # Canonical flow cell runs
 
 
 @pytest.fixture(scope="module")
 def hiseq_x_single_index_flow_cell(
     hiseq_x_single_index_flow_cell_dir: Path,
-) -> FlowCellDirectoryData:
+) -> IlluminaRunDirectoryData:
     """Return a single-index HiSeqX flow cell."""
-    return FlowCellDirectoryData(flow_cell_path=hiseq_x_single_index_flow_cell_dir)
+    return IlluminaRunDirectoryData(sequencing_run_path=hiseq_x_single_index_flow_cell_dir)
 
 
 @pytest.fixture(scope="module")
 def hiseq_x_dual_index_flow_cell(
     hiseq_x_dual_index_flow_cell_dir: Path,
-) -> FlowCellDirectoryData:
+) -> IlluminaRunDirectoryData:
     """Return a dual-index HiSeqX flow cell."""
-    return FlowCellDirectoryData(flow_cell_path=hiseq_x_dual_index_flow_cell_dir)
+    return IlluminaRunDirectoryData(sequencing_run_path=hiseq_x_dual_index_flow_cell_dir)
 
 
 @pytest.fixture(scope="module")
 def hiseq_2500_dual_index_flow_cell(
     hiseq_2500_dual_index_flow_cell_dir: Path,
-) -> FlowCellDirectoryData:
+) -> IlluminaRunDirectoryData:
     """Return a dual-index HiSeq2500 flow cell."""
-    return FlowCellDirectoryData(flow_cell_path=hiseq_2500_dual_index_flow_cell_dir)
+    return IlluminaRunDirectoryData(sequencing_run_path=hiseq_2500_dual_index_flow_cell_dir)
 
 
 @pytest.fixture(scope="module")
 def hiseq_2500_custom_index_flow_cell(
     hiseq_2500_custom_index_flow_cell_dir: Path,
-) -> FlowCellDirectoryData:
+) -> IlluminaRunDirectoryData:
     """Return a custom-index HiSeq2500 flow cell."""
-    return FlowCellDirectoryData(flow_cell_path=hiseq_2500_custom_index_flow_cell_dir)
+    return IlluminaRunDirectoryData(sequencing_run_path=hiseq_2500_custom_index_flow_cell_dir)
 
 
 @pytest.fixture
 def novaseq_6000_pre_1_5_kits_flow_cell(
     illumina_flow_cells_directory: Path,
     novaseq_6000_pre_1_5_kits_flow_cell_full_name: str,
-) -> FlowCellDirectoryData:
+) -> IlluminaRunDirectoryData:
     """Return a Novaseq6000 flow cell with index settings pre 1.5 kits."""
-    return FlowCellDirectoryData(
+    return IlluminaRunDirectoryData(
         Path(illumina_flow_cells_directory, novaseq_6000_pre_1_5_kits_flow_cell_full_name)
     )
 
 
 @pytest.fixture
 def novaseq_6000_post_1_5_kits_flow_cell(
     illumina_flow_cells_directory: Path,
     novaseq_6000_post_1_5_kits_flow_cell_full_name: str,
-) -> FlowCellDirectoryData:
+) -> IlluminaRunDirectoryData:
     """Return a Novaseq6000 flow cell with index settings post 1.5 kits."""
-    return FlowCellDirectoryData(
+    return IlluminaRunDirectoryData(
         Path(illumina_flow_cells_directory, novaseq_6000_post_1_5_kits_flow_cell_full_name)
     )
 
 
 @pytest.fixture
-def novaseq_x_flow_cell(novaseq_x_flow_cell_dir: Path) -> FlowCellDirectoryData:
+def novaseq_x_flow_cell(novaseq_x_flow_cell_dir: Path) -> IlluminaRunDirectoryData:
     """Return a NovaSeqX flow cell."""
-    return FlowCellDirectoryData(novaseq_x_flow_cell_dir)
+    return IlluminaRunDirectoryData(novaseq_x_flow_cell_dir)
 
 
 @pytest.fixture
 def seven_canonical_flow_cells(
-    hiseq_x_single_index_flow_cell: FlowCellDirectoryData,
-    hiseq_x_dual_index_flow_cell: FlowCellDirectoryData,
-    hiseq_2500_dual_index_flow_cell: FlowCellDirectoryData,
-    hiseq_2500_custom_index_flow_cell: FlowCellDirectoryData,
-    novaseq_6000_pre_1_5_kits_flow_cell: FlowCellDirectoryData,
-    novaseq_6000_post_1_5_kits_flow_cell: FlowCellDirectoryData,
-    novaseq_x_flow_cell: FlowCellDirectoryData,
-) -> list[FlowCellDirectoryData]:
+    hiseq_x_single_index_flow_cell: IlluminaRunDirectoryData,
+    hiseq_x_dual_index_flow_cell: IlluminaRunDirectoryData,
+    hiseq_2500_dual_index_flow_cell: IlluminaRunDirectoryData,
+    hiseq_2500_custom_index_flow_cell: IlluminaRunDirectoryData,
+    novaseq_6000_pre_1_5_kits_flow_cell: IlluminaRunDirectoryData,
+    novaseq_6000_post_1_5_kits_flow_cell: IlluminaRunDirectoryData,
+    novaseq_x_flow_cell: IlluminaRunDirectoryData,
+) -> list[IlluminaRunDirectoryData]:
     """Return a list with the seven canonical flow cells."""
     return [
         hiseq_x_single_index_flow_cell,
         hiseq_x_dual_index_flow_cell,
         hiseq_2500_dual_index_flow_cell,
         hiseq_2500_custom_index_flow_cell,
         novaseq_6000_pre_1_5_kits_flow_cell,
@@ -94,49 +94,49 @@
 
 # Demultiplexed runs
 
 
 @pytest.fixture
 def novaseqx_flow_cell_with_sample_sheet_no_fastq(
     tmp_demultiplexed_flow_cell_no_fastq_files: Path,
-) -> FlowCellDirectoryData:
+) -> IlluminaRunDirectoryData:
     """Return a flow cell from a tmp dir with a sample sheet and no sample fastq files."""
     tmp_demultiplexed_flow_cell_no_fastq_files.mkdir(parents=True, exist_ok=True)
-    flow_cell = FlowCellDirectoryData(tmp_demultiplexed_flow_cell_no_fastq_files)
+    flow_cell = IlluminaRunDirectoryData(tmp_demultiplexed_flow_cell_no_fastq_files)
     sample_sheet_path = Path(flow_cell.path, DemultiplexingDirsAndFiles.SAMPLE_SHEET_FILE_NAME)
     flow_cell._sample_sheet_path_hk = sample_sheet_path
     return flow_cell
 
 
 @pytest.fixture
 def tmp_bcl_convert_flow_cell(
     tmp_flow_cell_directory_bcl_convert: Path,
-) -> FlowCellDirectoryData:
+) -> IlluminaRunDirectoryData:
     """Create a flow cell object with flow cell that is demultiplexed."""
-    return FlowCellDirectoryData(tmp_flow_cell_directory_bcl_convert)
+    return IlluminaRunDirectoryData(tmp_flow_cell_directory_bcl_convert)
 
 
 @pytest.fixture
 def hiseq_x_single_index_demultiplexed_flow_cell_with_sample_sheet(
     illumina_demultiplexed_runs_directory: Path,
     hiseq_x_single_index_flow_cell_name: str,
     hiseq_x_single_index_sample_sheet_path: Path,
-) -> FlowCellDirectoryData:
+) -> IlluminaRunDirectoryData:
     """Return a Novaseq6000 flow cell with a sample sheet."""
     path = Path(illumina_demultiplexed_runs_directory, hiseq_x_single_index_flow_cell_name)
-    flow_cell = FlowCellDirectoryData(path)
+    flow_cell = IlluminaRunDirectoryData(path)
     flow_cell.set_sample_sheet_path_hk(hiseq_x_single_index_sample_sheet_path)
     return flow_cell
 
 
 @pytest.fixture
-def novaseq_x_demux_runs_flow_cell(novaseq_x_demux_runs_dir: Path) -> FlowCellDirectoryData:
+def novaseq_x_demux_runs_flow_cell(novaseq_x_demux_runs_dir: Path) -> IlluminaRunDirectoryData:
     """Return a NovaSeqX flow cell."""
-    return FlowCellDirectoryData(novaseq_x_demux_runs_dir)
+    return IlluminaRunDirectoryData(novaseq_x_demux_runs_dir)
 
 
 @pytest.fixture
 def hiseq_2500_dual_index_demux_runs_flow_cell(
     hiseq_2500_dual_index_demux_runs_dir: Path,
-) -> FlowCellDirectoryData:
+) -> IlluminaRunDirectoryData:
     """Return a HiSeq2500 flow cell."""
-    return FlowCellDirectoryData(hiseq_2500_dual_index_demux_runs_dir)
+    return IlluminaRunDirectoryData(hiseq_2500_dual_index_demux_runs_dir)
```

### Comparing `cg-60.9.1/tests/fixture_plugins/demultiplex_fixtures/name_fixtures.py` & `cg-60.9.3/tests/fixture_plugins/demultiplex_fixtures/name_fixtures.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixture_plugins/demultiplex_fixtures/path_fixtures.py` & `cg-60.9.3/tests/fixture_plugins/demultiplex_fixtures/path_fixtures.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixture_plugins/demultiplex_fixtures/run_parameters_fixtures.py` & `cg-60.9.3/tests/fixture_plugins/demultiplex_fixtures/run_parameters_fixtures.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixture_plugins/demultiplex_fixtures/sample_fixtures.py` & `cg-60.9.3/tests/fixture_plugins/demultiplex_fixtures/sample_fixtures.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import pytest
 
 from cg.apps.demultiplex.sample_sheet.sample_models import FlowCellSample
 from cg.apps.demultiplex.sample_sheet.sample_sheet_creator import SampleSheetCreator
 from cg.constants import FileExtensions
 from cg.io.json import read_json
-from cg.models.flow_cell.flow_cell import FlowCellDirectoryData
+from cg.models.run_devices.illumina_run_directory_data import IlluminaRunDirectoryData
 
 
 @pytest.fixture
 def hiseq_x_single_index_bcl_convert_lims_samples(
     hiseq_x_single_index_flow_cell_dir: Path,
 ) -> list[FlowCellSample]:
     """Return a list of BCLConvert samples parsed from LIMS for a HiSeqX single index flow cell."""
@@ -139,15 +139,15 @@
 
 
 # Sample sheet creators
 
 
 @pytest.fixture
 def bcl_convert_sample_sheet_creator(
-    novaseq_x_flow_cell: FlowCellDirectoryData,
+    novaseq_x_flow_cell: IlluminaRunDirectoryData,
     novaseq_x_lims_samples: list[FlowCellSample],
 ) -> SampleSheetCreator:
     """Returns a sample sheet creator for sample sheet v2."""
     return SampleSheetCreator(
         flow_cell=novaseq_x_flow_cell,
         lims_samples=novaseq_x_lims_samples,
     )
```

### Comparing `cg-60.9.1/tests/fixture_plugins/demultiplex_fixtures/sample_sheet_fixtures.py` & `cg-60.9.3/tests/fixture_plugins/demultiplex_fixtures/sample_sheet_fixtures.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixture_plugins/loqusdb_fixtures/loqusdb_api_fixtures.py` & `cg-60.9.3/tests/fixture_plugins/loqusdb_fixtures/loqusdb_api_fixtures.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixture_plugins/loqusdb_fixtures/loqusdb_output_fixtures.py` & `cg-60.9.3/tests/fixture_plugins/loqusdb_fixtures/loqusdb_output_fixtures.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixture_plugins/observations_fixtures/observations_api_fixtures.py` & `cg-60.9.3/tests/fixture_plugins/observations_fixtures/observations_api_fixtures.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixture_plugins/observations_fixtures/observations_input_files_fixtures.py` & `cg-60.9.3/tests/fixture_plugins/observations_fixtures/observations_input_files_fixtures.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixture_plugins/quality_controller_fixtures/sequencing_qc_check_scenario.py` & `cg-60.9.3/tests/fixture_plugins/quality_controller_fixtures/sequencing_qc_check_scenario.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixture_plugins/quality_controller_fixtures/sequencing_qc_fixtures.py` & `cg-60.9.3/tests/fixture_plugins/quality_controller_fixtures/sequencing_qc_fixtures.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixture_plugins/timestamp_fixtures.py` & `cg-60.9.3/tests/fixture_plugins/timestamp_fixtures.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json` & `cg-60.9.3/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json` & `cg-60.9.3/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/analysis/raredisease/multiqc_data.json` & `cg-60.9.3/tests/fixtures/analysis/raredisease/multiqc_data.json`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/analysis/raredisease/raredisease_case_enough_reads_metrics_deliverables.yaml` & `cg-60.9.3/tests/fixtures/analysis/raredisease/raredisease_case_enough_reads_metrics_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/analysis/rnafusion/multiqc_data.json` & `cg-60.9.3/tests/fixtures/analysis/rnafusion/multiqc_data.json`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/analysis/rnafusion/rnafusion_case_enough_reads_metrics_deliverables.yaml` & `cg-60.9.3/tests/fixtures/analysis/rnafusion/rnafusion_case_enough_reads_metrics_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/analysis/sample_coverage.bed` & `cg-60.9.3/tests/fixtures/analysis/sample_coverage.bed`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/analysis/taxprofiler/multiqc_data.json` & `cg-60.9.3/tests/fixtures/analysis/taxprofiler/multiqc_data.json`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/analysis/taxprofiler/taxprofiler_case_metrics_deliverables.yaml` & `cg-60.9.3/tests/fixtures/analysis/taxprofiler/taxprofiler_case_metrics_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/analysis/tomte/multiqc_data.json` & `cg-60.9.3/tests/fixtures/analysis/tomte/multiqc_data.json`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/analysis/tomte/tomte_case_enough_reads_metrics_deliverables.yaml` & `cg-60.9.3/tests/fixtures/analysis/tomte/tomte_case_enough_reads_metrics_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/balsamic/case/config.json` & `cg-60.9.3/tests/fixtures/apps/balsamic/case/config.json`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/balsamic/case/metadata.yml` & `cg-60.9.3/tests/fixtures/apps/balsamic/case/metadata.yml`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml` & `cg-60.9.3/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/crunchy/spring_metadata.json` & `cg-60.9.3/tests/fixtures/apps/crunchy/spring_metadata.json`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/Reports/Quality_Metrics.csv` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/Reports/Quality_Metrics.csv`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/dragen-replay.json` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/dragen-replay.json`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRZZ/Unaligned/Reports/RunInfo.xml` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRZZ/Unaligned/Reports/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/230912_A00187_1009_AHK33MDRX3/SampleSheet.csv` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/230912_A00187_1009_AHK33MDRX3/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R1_001.fastq.gz` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R1_001.fastq.gz`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R2_001.fastq.gz` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R2_001.fastq.gz`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/HJCFFALXX_bcl2fastq_raw.json` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/HJCFFALXX_bcl2fastq_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/HJCFFALXX_bcl_convert_raw.json` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/HJCFFALXX_bcl_convert_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTAConfiguration.xml` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTAConfiguration.xml`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RunInfo.xml` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet.csv` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet_bcl2fastq.csv` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet_bcl2fastq.csv`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/runParameters.xml` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/runParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/HL32LCCXY_bcl2fastq_raw.json` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/HL32LCCXY_bcl2fastq_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/HL32LCCXY_bcl_convert_raw.json` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/HL32LCCXY_bcl_convert_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTAConfiguration.xml` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTAConfiguration.xml`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RunInfo.xml` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SampleSheet.csv` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SampleSheet_bcl2fastq.csv` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SampleSheet_bcl2fastq.csv`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/runParameters.xml` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/runParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/HGYFNBCX2_bcl2fastq_raw.json` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/HGYFNBCX2_bcl2fastq_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/HGYFNBCX2_bcl_convert_raw.json` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/HGYFNBCX2_bcl_convert_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/RunInfo.xml` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/SampleSheet.csv` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/SampleSheet_bcl2fastq.csv` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/SampleSheet_bcl2fastq.csv`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/runParameters.xml` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/runParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/HM2LNBCX2_bcl2fastq_raw.json` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/HM2LNBCX2_bcl2fastq_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/HM2LNBCX2_bcl_convert_raw.json` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/HM2LNBCX2_bcl_convert_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/RunInfo.xml` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/SampleSheet.csv` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/SampleSheet_bcl2fastq.csv` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/SampleSheet_bcl2fastq.csv`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/runParameters.xml` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/runParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/CorrectSampleSheet.csv` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/CorrectSampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/HLYWYDSXX_bcl2fastq_raw.json` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/HLYWYDSXX_bcl2fastq_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/HLYWYDSXX_bcl_convert_raw.json` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/HLYWYDSXX_bcl_convert_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RTA3.cfg` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RTA3.cfg`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RunInfo.xml` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RunParameters.xml` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stdout` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stdout`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_raw.json` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/RunParameters.xml` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/22F52TLT3_raw.json` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/22F52TLT3_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/CorrectSampleSheet.csv` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/CorrectSampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RTA.cfg` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RTA.cfg`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunCompletionStatus.xml` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunCompletionStatus.xml`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunInfo.xml` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunParameters.xml` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/SampleSheet.csv` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stdout` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stdout`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/RunParameters.xml` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/SampleSheet.csv` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/CorrectSampleSheet.csv` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/CorrectSampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/HK33MDRX3_bcl_convert_raw.json` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/HK33MDRX3_bcl_convert_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RTA3.cfg` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RTA3.cfg`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RunInfo.xml` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RunParameters.xml` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/SampleSheet.csv` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet.csv` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells_broken/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/170517_ST-E00266_0210_BHJCFFALXX/runParameters.xml` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells_broken/170517_ST-E00266_0210_BHJCFFALXX/runParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/190927_A00689_0069_BHLYWYDSXX/RunParameters.xml` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells_broken/190927_A00689_0069_BHLYWYDSXX/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/20231108_LH00188_0028_B22F52TLT3/RunParameters.xml` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells_broken/20231108_LH00188_0028_B22F52TLT3/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/230912_A00187_1009_AHK33MDRX3/RunParameters.xml` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells_broken/230912_A00187_1009_AHK33MDRX3/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stdout` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stdout`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/RunParameters.xml` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_hiseq_2500_different_index_cycles.xml` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_hiseq_2500_different_index_cycles.xml`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_6000_different_index_cycles.xml` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_6000_different_index_cycles.xml`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_different_index_cycles.xml` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_different_index_cycles.xml`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_wrong_instrument.xml` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_wrong_instrument.xml`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_no_software_nor_reagent_version.xml` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_no_software_nor_reagent_version.xml`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/sample_sheets/novaseq_6000_sample_sheet_with_reversed_cycles.csv` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/sample_sheets/novaseq_6000_sample_sheet_with_reversed_cycles.csv`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/demultiplexing/sample_sheets/novaseq_x_sample_sheet_with_forward_cycles.csv` & `cg-60.9.3/tests/fixtures/apps/demultiplexing/sample_sheets/novaseq_x_sample_sheet_with_forward_cycles.csv`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/fluffy/SampleSheet.csv` & `cg-60.9.3/tests/fixtures/apps/fluffy/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/fluffy/deliverables.yaml` & `cg-60.9.3/tests/fixtures/apps/fluffy/deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/madeline/madeline.xml` & `cg-60.9.3/tests/fixtures/apps/madeline/madeline.xml`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/mip/case_metrics_deliverables.yaml` & `cg-60.9.3/tests/fixtures/apps/mip/case_metrics_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/mip/dna/store/case_config.yaml` & `cg-60.9.3/tests/fixtures/apps/mip/dna/store/case_config.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml` & `cg-60.9.3/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml` & `cg-60.9.3/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf` & `cg-60.9.3/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/mip/rna/case_config.yaml` & `cg-60.9.3/tests/fixtures/apps/mip/rna/case_config.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml` & `cg-60.9.3/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/mip/rna/store/bundle_data.yaml` & `cg-60.9.3/tests/fixtures/apps/mip/rna/store/bundle_data.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/mip/rna/store/case_config.yaml` & `cg-60.9.3/tests/fixtures/apps/mip/rna/store/case_config.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml` & `cg-60.9.3/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml` & `cg-60.9.3/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/scout/643594.config.yaml` & `cg-60.9.3/tests/fixtures/apps/scout/643594.config.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/scout/case_export.json` & `cg-60.9.3/tests/fixtures/apps/scout/case_export.json`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/scout/export_causatives.json` & `cg-60.9.3/tests/fixtures/apps/scout/export_causatives.json`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/scout/none_case_export.json` & `cg-60.9.3/tests/fixtures/apps/scout/none_case_export.json`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/scout/other_sex_case.json` & `cg-60.9.3/tests/fixtures/apps/scout/other_sex_case.json`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/scout/panel_export.bed` & `cg-60.9.3/tests/fixtures/apps/scout/panel_export.bed`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/apps/scout/panel_export.csv` & `cg-60.9.3/tests/fixtures/apps/scout/panel_export.csv`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/cgweb_orders/balsamic.json` & `cg-60.9.3/tests/fixtures/cgweb_orders/balsamic.json`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/cgweb_orders/fastq.json` & `cg-60.9.3/tests/fixtures/cgweb_orders/fastq.json`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/cgweb_orders/metagenome.json` & `cg-60.9.3/tests/fixtures/cgweb_orders/metagenome.json`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/cgweb_orders/microsalt.json` & `cg-60.9.3/tests/fixtures/cgweb_orders/microsalt.json`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/cgweb_orders/mip.json` & `cg-60.9.3/tests/fixtures/cgweb_orders/mip.json`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/cgweb_orders/mip_rna.json` & `cg-60.9.3/tests/fixtures/cgweb_orders/mip_rna.json`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/cgweb_orders/rml.json` & `cg-60.9.3/tests/fixtures/cgweb_orders/rml.json`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/cgweb_orders/rnafusion.json` & `cg-60.9.3/tests/fixtures/cgweb_orders/rnafusion.json`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/cgweb_orders/sarscov2.json` & `cg-60.9.3/tests/fixtures/cgweb_orders/sarscov2.json`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/cgweb_orders/tomte.json` & `cg-60.9.3/tests/fixtures/cgweb_orders/tomte.json`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/data/SampleSheet.csv` & `cg-60.9.3/tests/fixtures/data/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/data/cgfixture.db` & `cg-60.9.3/tests/fixtures/data/cgfixture.db`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/data/hkstore.db` & `cg-60.9.3/tests/fixtures/data/hkstore.db`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/io/example_json.json` & `cg-60.9.3/tests/fixtures/io/example_json.json`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/orderforms/1508.31.balsamic.xlsx` & `cg-60.9.3/tests/fixtures/orderforms/1508.31.balsamic.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/orderforms/1508.31.balsamic_qc.xlsx` & `cg-60.9.3/tests/fixtures/orderforms/1508.31.balsamic_qc.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/orderforms/1508.31.balsamic_umi.xlsx` & `cg-60.9.3/tests/fixtures/orderforms/1508.31.balsamic_umi.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/orderforms/1508.31.fastq.xlsx` & `cg-60.9.3/tests/fixtures/orderforms/1508.31.fastq.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/orderforms/1508.31.metagenome.xlsx` & `cg-60.9.3/tests/fixtures/orderforms/1508.31.metagenome.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/orderforms/1508.31.mip.xlsx` & `cg-60.9.3/tests/fixtures/orderforms/1508.31.mip.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/orderforms/1508.31.mip_rna.xlsx` & `cg-60.9.3/tests/fixtures/orderforms/1508.31.mip_rna.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/orderforms/1508.31.rnafusion.xlsx` & `cg-60.9.3/tests/fixtures/orderforms/1508.31.rnafusion.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/orderforms/1508.31.tomte.xlsx` & `cg-60.9.3/tests/fixtures/orderforms/1508.31.tomte.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/orderforms/1603.11.microbial.xlsx` & `cg-60.9.3/tests/fixtures/orderforms/1603.11.microbial.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/orderforms/1604.17.rml.xlsx` & `cg-60.9.3/tests/fixtures/orderforms/1604.17.rml.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/orderforms/2184.9.sarscov2.xlsx` & `cg-60.9.3/tests/fixtures/orderforms/2184.9.sarscov2.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/orderforms/NIPT-json.json` & `cg-60.9.3/tests/fixtures/orderforms/NIPT-json.json`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json` & `cg-60.9.3/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/orderforms/mip_uploaded_json_orderform.json` & `cg-60.9.3/tests/fixtures/orderforms/mip_uploaded_json_orderform.json`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/report/case_data.json` & `cg-60.9.3/tests/fixtures/report/case_data.json`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/report/lims_exported_samples.json` & `cg-60.9.3/tests/fixtures/report/lims_exported_samples.json`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/report/lims_family.json` & `cg-60.9.3/tests/fixtures/report/lims_family.json`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/services/illumina_metrics_service/230622_A00621_0864_AHY7FFDRX2/SampleSheet.csv` & `cg-60.9.3/tests/fixtures/services/illumina_metrics_service/230622_A00621_0864_AHY7FFDRX2/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/services/illumina_metrics_service/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Adapter_Metrics.csv` & `cg-60.9.3/tests/fixtures/services/illumina_metrics_service/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Adapter_Metrics.csv`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/services/illumina_metrics_service/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Demultiplex_Stats.csv` & `cg-60.9.3/tests/fixtures/services/illumina_metrics_service/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Demultiplex_Stats.csv`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/fixtures/services/illumina_metrics_service/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Quality_Metrics.csv` & `cg-60.9.3/tests/fixtures/services/illumina_metrics_service/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Quality_Metrics.csv`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/io/conftest.py` & `cg-60.9.3/tests/io/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/io/test_io_controller.py` & `cg-60.9.3/tests/io/test_io_controller.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/io/test_io_csv.py` & `cg-60.9.3/tests/io/test_io_csv.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/io/test_io_json.py` & `cg-60.9.3/tests/io/test_io_json.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/io/test_io_txt.py` & `cg-60.9.3/tests/io/test_io_txt.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/io/test_io_xml.py` & `cg-60.9.3/tests/io/test_io_xml.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/io/test_io_yaml.py` & `cg-60.9.3/tests/io/test_io_yaml.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/io/test_validate_path.py` & `cg-60.9.3/tests/io/test_validate_path.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/archive/conftest.py` & `cg-60.9.3/tests/meta/archive/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/archive/test_archive_api.py` & `cg-60.9.3/tests/meta/archive/test_archive_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/archive/test_archive_cli.py` & `cg-60.9.3/tests/meta/archive/test_archive_cli.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/archive/test_archiving.py` & `cg-60.9.3/tests/meta/archive/test_archiving.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/backup/conftest.py` & `cg-60.9.3/tests/meta/backup/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,14 +90,14 @@
     """Return path to a file used in the backup process"""
     return "/path/to/backup_file.extension"
 
 
 @pytest.fixture
 def archived_flow_cell() -> Path:
     """Path of archived flow cell"""
-    return Path("/path/to/archived/flow_cell.tar.gz.gpg")
+    return Path("/path/to/archived/run_devices.tar.gz.gpg")
 
 
 @pytest.fixture
 def archived_key() -> Path:
     """Path of archived key"""
     return Path("/path/to/archived/encryption_key.key.gpg")
```

### Comparing `cg-60.9.1/tests/meta/backup/test_meta_backup.py` & `cg-60.9.3/tests/meta/backup/test_meta_backup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from cg.constants.demultiplexing import DemultiplexingDirsAndFiles
 from cg.constants.sequencing import Sequencers
 from cg.exc import ChecksumFailedError
 from cg.meta.backup.backup import BackupAPI, SpringBackupAPI
 from cg.meta.backup.pdc import PdcAPI
 from cg.meta.encryption.encryption import SpringEncryptionAPI
 from cg.models.cg_config import PDCArchivingDirectory
-from cg.models.flow_cell.flow_cell import FlowCellDirectoryData
+from cg.models.run_devices.illumina_run_directory_data import IlluminaRunDirectoryData
 from tests.mocks.hk_mock import MockFile
 
 
 @pytest.mark.parametrize(
     "flow_cell_name",
     ["new_flow_cell", "old_flow_cell", "ancient_flow_cell"],
 )
@@ -665,20 +665,20 @@
 
     # THEN the decryption failure should be logged
     assert "Decryption failed" in caplog.text
 
 
 def test_create_copy_complete_file_exist(
     backup_api: BackupAPI,
-    novaseq_x_flow_cell: FlowCellDirectoryData,
+    novaseq_x_flow_cell: IlluminaRunDirectoryData,
 ):
     """Tests creating a copy complete file in the flow cell directory. There are two cases: when
     the file exists and when it does not exist."""
 
-    # GIVEN a flow cell that has been decrypted in flow_cell directory
+    # GIVEN a flow cell that has been decrypted in run_devices directory
     flow_cell_dir: Path = novaseq_x_flow_cell.path
 
     # GIVEN the copy complete to be created
     copy_complete_txt: str = DemultiplexingDirsAndFiles.COPY_COMPLETE
 
     # GIVEN a copy complete file exists
     flow_cell_dir.joinpath(copy_complete_txt).touch()
@@ -688,20 +688,20 @@
 
     # THEN the copy complete file should exist in the flow cell directory
     assert flow_cell_dir.joinpath(copy_complete_txt).exists() is True
 
 
 def test_create_copy_complete_file_does_not_exist(
     backup_api: BackupAPI,
-    novaseq_x_flow_cell: FlowCellDirectoryData,
+    novaseq_x_flow_cell: IlluminaRunDirectoryData,
 ):
     """Tests creating a copy complete file in the flow cell directory. There are two cases: when
     the file exists and when it does not exist."""
 
-    # GIVEN a flow cell that has been decrypted in flow_cell directory
+    # GIVEN a flow cell that has been decrypted in run_devices directory
     flow_cell_dir: Path = novaseq_x_flow_cell.path
 
     # GIVEN the copy complete to be created
     copy_complete_txt: str = DemultiplexingDirsAndFiles.COPY_COMPLETE
 
     # GIVEN that the copy complete file does not exists
     flow_cell_dir.joinpath(copy_complete_txt).unlink(missing_ok=True)
```

### Comparing `cg-60.9.1/tests/meta/backup/test_meta_pdc.py` & `cg-60.9.3/tests/meta/backup/test_meta_pdc.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/clean/conftest.py` & `cg-60.9.3/tests/meta/clean/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import pytest
 
 from cg.apps.housekeeper.hk import HousekeeperAPI
 from cg.constants import SequencingFileTag
 from cg.constants.subject import Sex
 from cg.meta.clean.clean_flow_cells import CleanFlowCellAPI
 from cg.meta.clean.clean_retrieved_spring_files import CleanRetrievedSpringFilesAPI
-from cg.models.flow_cell.flow_cell import FlowCellDirectoryData
+from cg.models.run_devices.illumina_run_directory_data import IlluminaRunDirectoryData
 from cg.store.models import Flowcell
 from cg.store.store import Store
 from tests.store_helpers import StoreHelpers
 
 
 @pytest.fixture(scope="function")
 def flow_cell_clean_api_can_be_removed(
@@ -52,42 +52,42 @@
 @pytest.fixture(scope="function")
 def tmp_flow_cell_to_clean_path(tmp_flow_cell_directory_bcl_convert: Path):
     """Returns the path to a flow cell fulfilling all cleaning criteria."""
     return tmp_flow_cell_directory_bcl_convert
 
 
 @pytest.fixture(scope="function")
-def tmp_flow_cell_to_clean(tmp_flow_cell_to_clean_path: Path) -> FlowCellDirectoryData:
+def tmp_flow_cell_to_clean(tmp_flow_cell_to_clean_path: Path) -> IlluminaRunDirectoryData:
     """Returns a flow cell directory object for a flow cell that fulfills all cleaning criteria."""
-    return FlowCellDirectoryData(tmp_flow_cell_to_clean_path)
+    return IlluminaRunDirectoryData(tmp_flow_cell_to_clean_path)
 
 
 @pytest.fixture(scope="function")
 def tmp_flow_cell_not_to_clean_path(tmp_novaseq_6000_pre_1_5_kits_flow_cell_path: Path):
     """Return the path to a flow cell not fulfilling all cleaning criteria."""
     return tmp_novaseq_6000_pre_1_5_kits_flow_cell_path
 
 
 @pytest.fixture(scope="function")
-def tmp_flow_cell_not_to_clean(tmp_flow_cell_not_to_clean_path: Path) -> FlowCellDirectoryData:
+def tmp_flow_cell_not_to_clean(tmp_flow_cell_not_to_clean_path: Path) -> IlluminaRunDirectoryData:
     """Returns a flow cell directory object for a flow cell that does not fulfill all cleaning criteria."""
-    return FlowCellDirectoryData(tmp_flow_cell_not_to_clean_path)
+    return IlluminaRunDirectoryData(tmp_flow_cell_not_to_clean_path)
 
 
 @pytest.fixture(scope="session")
 def tmp_sample_sheet_clean_flow_cell_path(tmp_path_factory) -> Path:
     sample_sheet_path = tmp_path_factory.mktemp("SampleSheet.csv")
     return sample_sheet_path
 
 
 @pytest.fixture
 def store_with_flow_cell_to_clean(
     store: Store,
     sample_id: str,
-    tmp_flow_cell_to_clean: FlowCellDirectoryData,
+    tmp_flow_cell_to_clean: IlluminaRunDirectoryData,
     helpers: StoreHelpers,
 ) -> Store:
     """Return a store with multiple samples with sample lane sequencing metrics."""
     sample_sequencing_metrics_details: list[tuple] = [
         (sample_id, tmp_flow_cell_to_clean.id, 1, 50_000_0000, 90.5, 32),
         (sample_id, tmp_flow_cell_to_clean.id, 2, 50_000_0000, 90.4, 31),
     ]
@@ -107,15 +107,15 @@
     return store
 
 
 @pytest.fixture
 def store_with_flow_cell_not_to_clean(
     store: Store,
     sample_id: str,
-    tmp_flow_cell_not_to_clean: FlowCellDirectoryData,
+    tmp_flow_cell_not_to_clean: IlluminaRunDirectoryData,
     helpers: StoreHelpers,
 ) -> Store:
     """Return a store with multiple samples with sample lane sequencing metrics."""
     sample_sequencing_metrics_details: list[str | int | float] = [
         (sample_id, tmp_flow_cell_not_to_clean.id, 1, 50_000_0000, 90.5, 32),
         (sample_id, tmp_flow_cell_not_to_clean.id, 2, 50_000_0000, 90.4, 31),
     ]
@@ -167,15 +167,15 @@
         store=real_housekeeper_api, bundle_data=hk_sample_bundle_for_flow_cell_not_to_clean
     )
     return real_housekeeper_api
 
 
 @pytest.fixture(scope="function")
 def hk_flow_cell_to_clean_bundle(
-    tmp_flow_cell_to_clean: FlowCellDirectoryData,
+    tmp_flow_cell_to_clean: IlluminaRunDirectoryData,
     timestamp_yesterday: datetime,
     tmp_sample_sheet_clean_flow_cell_path: Path,
 ) -> dict:
     """Housekeeper bundle information for a flow cell that can be cleaned."""
     return {
         "name": tmp_flow_cell_to_clean.id,
         "created": timestamp_yesterday,
@@ -193,15 +193,15 @@
 @pytest.fixture(scope="function")
 def hk_sample_bundle_for_flow_cell_to_clean(
     sample_id: str,
     timestamp_yesterday: datetime,
     spring_file: Path,
     fastq_file: Path,
     spring_meta_data_file: Path,
-    tmp_flow_cell_to_clean: FlowCellDirectoryData,
+    tmp_flow_cell_to_clean: IlluminaRunDirectoryData,
 ) -> dict:
     return {
         "name": sample_id,
         "created": timestamp_yesterday,
         "expires": timestamp_yesterday,
         "files": [
             {
```

### Comparing `cg-60.9.1/tests/meta/clean/test_clean_flow_cells_api.py` & `cg-60.9.3/tests/meta/clean/test_clean_flow_cells_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/clean/test_clean_retrieved_spring_files.py` & `cg-60.9.3/tests/meta/clean/test_clean_retrieved_spring_files.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/compress/conftest.py` & `cg-60.9.3/tests/meta/compress/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/compress/test_clean_fastq.py` & `cg-60.9.3/tests/meta/compress/test_clean_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/compress/test_compress_files.py` & `cg-60.9.3/tests/meta/compress/test_compress_files.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/compress/test_compress_meta_fastq.py` & `cg-60.9.3/tests/meta/compress/test_compress_meta_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/compress/test_decompress_spring_meta.py` & `cg-60.9.3/tests/meta/compress/test_decompress_spring_meta.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/compress/test_meta_compress_update_hk.py` & `cg-60.9.3/tests/meta/compress/test_meta_compress_update_hk.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/conftest.py` & `cg-60.9.3/tests/meta/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/deliver/conftest.py` & `cg-60.9.3/tests/meta/deliver/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/deliver/test_deliver_ticket.py` & `cg-60.9.3/tests/meta/deliver/test_deliver_ticket.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/deliver/test_delivery_api.py` & `cg-60.9.3/tests/meta/deliver/test_delivery_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/deliver/test_fastq_path_generator.py` & `cg-60.9.3/tests/meta/deliver/test_fastq_path_generator.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/delivery/test_delivery_api.py` & `cg-60.9.3/tests/meta/delivery/test_delivery_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/demultiplex/conftest.py` & `cg-60.9.3/tests/meta/demultiplex/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/demultiplex/test_combine_sequencing_metrics.py` & `cg-60.9.3/tests/meta/demultiplex/test_combine_sequencing_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/demultiplex/test_demux_post_processing.py` & `cg-60.9.3/tests/meta/demultiplex/test_demux_post_processing.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from cg.constants.demultiplexing import DemultiplexingDirsAndFiles
 from cg.constants.housekeeper_tags import SequencingFileTag
 from cg.meta.demultiplex.demux_post_processing import DemuxPostProcessingAPI
 from cg.meta.demultiplex.housekeeper_storage_functions import (
     add_and_include_sample_sheet_path_to_housekeeper,
 )
 from cg.models.cg_config import CGConfig
-from cg.models.flow_cell.flow_cell import FlowCellDirectoryData
+from cg.models.run_devices.illumina_run_directory_data import IlluminaRunDirectoryData
 from cg.store.models import Sample
 
 
 def test_set_dry_run(
     demultiplex_context: CGConfig,
 ):
     # GIVEN a demultiplex context
@@ -51,15 +51,15 @@
     tmp_illumina_demultiplexed_flow_cells_directory: Path,
     request: pytest.FixtureRequest,
 ):
     """Test adding a demultiplexed flow cell to the databases with. Runs on each type of
     demultiplexing software and setting used."""
 
     # GIVEN a demultiplexed flow cell
-    flow_cell: FlowCellDirectoryData = request.getfixturevalue(flow_cell_fixture)
+    flow_cell: IlluminaRunDirectoryData = request.getfixturevalue(flow_cell_fixture)
     flow_cell_demultiplexing_directory: str = flow_cell.full_name
     flow_cell_name: str = flow_cell.id
     sample_internal_ids: list[str] = request.getfixturevalue(sample_ids_fixture)
 
     # GIVEN the sample_internal_ids are present in statusdb
     for sample_internal_id in sample_internal_ids:
         assert updated_demultiplex_context.status_db.get_sample_by_internal_id(sample_internal_id)
@@ -149,15 +149,15 @@
         tmp_illumina_demultiplexed_flow_cells_directory, hiseq_x_single_index_flow_cell_name
     )
     assert demuxed_flow_cell_path in demultiplexed_flow_cell_dirs
 
 
 def test_post_processing_tracks_undetermined_fastq_files(
     updated_demux_post_processing_api: DemuxPostProcessingAPI,
-    hiseq_x_single_index_flow_cell: FlowCellDirectoryData,
+    hiseq_x_single_index_flow_cell: IlluminaRunDirectoryData,
     selected_hiseq_x_single_index_sample_ids: list[str],
 ):
     # GIVEN a flow cell with undetermined fastqs in a non-pooled lane
 
     # GIVEN that the flow cell has the sample sheet in housekeeper
     add_and_include_sample_sheet_path_to_housekeeper(
         flow_cell_directory=hiseq_x_single_index_flow_cell.path,
@@ -177,15 +177,15 @@
 
     undetermined_fastq_files = [file for file in fastq_files if "Undetermined" in file.path]
     assert undetermined_fastq_files
 
 
 def test_sample_read_count_update_is_idempotent(
     updated_demux_post_processing_api: DemuxPostProcessingAPI,
-    hiseq_x_single_index_flow_cell: FlowCellDirectoryData,
+    hiseq_x_single_index_flow_cell: IlluminaRunDirectoryData,
     selected_hiseq_x_single_index_sample_ids: list[str],
 ):
     """Test that sample read counts are the same if the flow cell is processed twice."""
 
     # GIVEN a demultiplexed flow cell with the sample sheet in housekeeper
     add_and_include_sample_sheet_path_to_housekeeper(
         flow_cell_directory=hiseq_x_single_index_flow_cell.path,
```

### Comparing `cg-60.9.1/tests/meta/demultiplex/test_housekeeper_storage_functions.py` & `cg-60.9.3/tests/meta/demultiplex/test_housekeeper_storage_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     add_and_include_sample_sheet_path_to_housekeeper,
     add_demux_logs_to_housekeeper,
     add_run_parameters_file_to_housekeeper,
     add_sample_fastq_files_to_housekeeper,
     delete_sequencing_data_from_housekeeper,
 )
 from cg.models.cg_config import CGConfig
-from cg.models.flow_cell.flow_cell import FlowCellDirectoryData
+from cg.models.run_devices.illumina_run_directory_data import IlluminaRunDirectoryData
 from tests.store_helpers import StoreHelpers
 
 
 def test_add_bundle_and_version_if_non_existent(demultiplex_context: CGConfig):
     # GIVEN a DemuxPostProcessing API
     demux_post_processing_api = DemuxPostProcessingAPI(demultiplex_context)
 
@@ -95,15 +95,15 @@
     demux_post_processing_api.hk_api.get_tag.assert_has_calls(
         [call(name="tag1"), call(name="tag2")]
     )
     demux_post_processing_api.hk_api.add_tag.assert_not_called()
 
 
 def test_add_fastq_files_without_sample_id(
-    demultiplex_context: CGConfig, novaseq_6000_post_1_5_kits_flow_cell: FlowCellDirectoryData
+    demultiplex_context: CGConfig, novaseq_6000_post_1_5_kits_flow_cell: IlluminaRunDirectoryData
 ):
     # GIVEN a DemuxPostProcessing API
     demux_post_processing_api = DemuxPostProcessingAPI(demultiplex_context)
 
     # GIVEN that the sample sheet exists in housekeeper and the path is in the flow cell
     add_and_include_sample_sheet_path_to_housekeeper(
         flow_cell_directory=novaseq_6000_post_1_5_kits_flow_cell.path,
@@ -126,15 +126,15 @@
 
     # THEN no files were added to housekeeper
     demux_post_processing_api.hk_api.add_file_to_bundle_if_non_existent.assert_not_called()
 
 
 def test_add_existing_sample_sheet(
     demultiplex_context: CGConfig,
-    novaseq_6000_post_1_5_kits_flow_cell: FlowCellDirectoryData,
+    novaseq_6000_post_1_5_kits_flow_cell: IlluminaRunDirectoryData,
     tmp_illumina_flow_cells_directory: Path,
 ):
     # GIVEN a DemuxPostProcessing API
     demux_post_processing_api = DemuxPostProcessingAPI(demultiplex_context)
 
     # GIVEN a flow cell directory and name
     flow_cell_directory = Path(
@@ -159,15 +159,15 @@
     files = demux_post_processing_api.hk_api.get_files(
         bundle=novaseq_6000_post_1_5_kits_flow_cell.id, tags=expected_tag_names
     ).all()
     assert len(files) == 1
 
 
 def test_add_demux_logs_to_housekeeper(
-    demultiplex_context: CGConfig, novaseq_6000_post_1_5_kits_flow_cell: FlowCellDirectoryData
+    demultiplex_context: CGConfig, novaseq_6000_post_1_5_kits_flow_cell: IlluminaRunDirectoryData
 ):
     # GIVEN a DemuxPostProcessing API
     demux_post_processing_api = DemuxPostProcessingAPI(demultiplex_context)
 
     # GIVEN a bundle and flow cell version exists in housekeeper
     demux_post_processing_api.hk_api.add_bundle_and_version_if_non_existent(
         bundle_name=novaseq_6000_post_1_5_kits_flow_cell.id
@@ -210,15 +210,15 @@
     # THEN the demux logs were added to housekeeper with the correct names
     assert len(files) == 2
     for file in files:
         assert file.path.split("/")[-1] in expected_file_names
 
 
 def test_add_run_parameters_to_housekeeper(
-    demultiplex_context: CGConfig, novaseq_x_flow_cell: FlowCellDirectoryData
+    demultiplex_context: CGConfig, novaseq_x_flow_cell: IlluminaRunDirectoryData
 ):
     """Test that the run parameters file of a flow cell is added to Housekeeper."""
     # GIVEN a flow cell with a run parameters file and a Housekeeper API
     hk_api = demultiplex_context.housekeeper_api
 
     # GIVEN that a run parameters file does not exist for the flow cell in Housekeeper
     assert not hk_api.files(tags=[SequencingFileTag.RUN_PARAMETERS, novaseq_x_flow_cell.id]).all()
```

### Comparing `cg-60.9.1/tests/meta/demultiplex/test_status_db_storage_functions.py` & `cg-60.9.3/tests/meta/demultiplex/test_status_db_storage_functions.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/demultiplex/test_utils.py` & `cg-60.9.3/tests/meta/demultiplex/test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     is_manifest_file_required,
     is_nanopore_sequencing_complete,
     is_sample_id_in_directory_name,
     is_syncing_complete,
     is_valid_sample_fastq_file,
     parse_manifest_file,
 )
-from cg.models.flow_cell.flow_cell import FlowCellDirectoryData
+from cg.models.run_devices.illumina_run_directory_data import IlluminaRunDirectoryData
 from tests.meta.demultiplex.conftest import get_all_files_in_directory_tree
 
 
 def test_validate_sample_fastq_with_valid_file():
     # GIVEN a sample fastq file with a lane number and sample id in the parent directory name
     sample_fastq = Path("Sample_123/sample_L0002.fastq.gz")
 
@@ -258,25 +258,25 @@
     with pytest.raises(FileNotFoundError):
         get_sample_sheet_path_from_flow_cell_dir(flow_cell_directory)
 
 
 def test_parse_flow_cell_directory_data_invalid():
     """Test that a FlowCellDirectoryData object is not created when the given path is invalid."""
     with pytest.raises(FlowCellError):
-        FlowCellDirectoryData(Path("invalid_path"))
+        IlluminaRunDirectoryData(Path("invalid_path"))
 
 
 def test_parse_flow_cell_directory_data_valid(novaseq_6000_post_1_5_kits_flow_cell_full_name: str):
     # GIVEN a flow cell directory which is valid
 
     # WHEN parsing the flow cell directory data
-    result = FlowCellDirectoryData(Path(novaseq_6000_post_1_5_kits_flow_cell_full_name))
+    result = IlluminaRunDirectoryData(Path(novaseq_6000_post_1_5_kits_flow_cell_full_name))
 
     # THEN a FlowCellDirectoryData object should be returned
-    assert isinstance(result, FlowCellDirectoryData)
+    assert isinstance(result, IlluminaRunDirectoryData)
 
     # THEN the flow cell path and bcl converter should be set
     assert result.path == Path(novaseq_6000_post_1_5_kits_flow_cell_full_name)
 
 
 def test_parse_manifest_file(novaseq_x_manifest_file: Path):
     # GIVEN a manifest file
```

### Comparing `cg-60.9.1/tests/meta/demultiplex/test_validation.py` & `cg-60.9.3/tests/meta/demultiplex/test_validation.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     is_demultiplexing_complete,
     is_flow_cell_ready_for_delivery,
     validate_demultiplexing_complete,
     validate_flow_cell_delivery_status,
     validate_flow_cell_has_fastq_files,
     validate_sample_sheet_exists,
 )
-from cg.models.flow_cell.flow_cell import FlowCellDirectoryData
+from cg.models.run_devices.illumina_run_directory_data import IlluminaRunDirectoryData
 
 
 def test_is_demultiplexing_complete_true(tmp_path: Path):
     # GIVEN a path where DEMUX_COMPLETE file is present
     (tmp_path / DemultiplexingDirsAndFiles.DEMUX_COMPLETE).touch()
 
     # WHEN checking if demultiplexing is complete
@@ -56,26 +56,26 @@
 
     # THEN the result should be False
     assert not result
 
 
 def test_validate_sample_sheet_exists_raises_error(hiseq_2500_custom_index_flow_cell_dir: Path):
     # GIVEN a flow cell without a sample sheet in housekeeper
-    flow_cell = FlowCellDirectoryData(flow_cell_path=hiseq_2500_custom_index_flow_cell_dir)
+    flow_cell = IlluminaRunDirectoryData(sequencing_run_path=hiseq_2500_custom_index_flow_cell_dir)
     flow_cell._sample_sheet_path_hk = None
     # WHEN validating the existence of the sample sheet
     # THEN it should raise a FlowCellError
     with pytest.raises(FlowCellError):
         validate_sample_sheet_exists(flow_cell=flow_cell)
 
 
 def test_validate_sample_sheet_exists(hiseq_2500_custom_index_flow_cell_dir: Path):
     # GIVEN a path with a sample sheet
     # GIVEN a flow cell without a sample sheet in housekeeper
-    flow_cell = FlowCellDirectoryData(flow_cell_path=hiseq_2500_custom_index_flow_cell_dir)
+    flow_cell = IlluminaRunDirectoryData(sequencing_run_path=hiseq_2500_custom_index_flow_cell_dir)
     sample_sheet_path = Path(
         hiseq_2500_custom_index_flow_cell_dir, DemultiplexingDirsAndFiles.SAMPLE_SHEET_FILE_NAME
     )
     sample_sheet_path.touch()
     flow_cell._sample_sheet_path_hk = sample_sheet_path
 
     # WHEN validating the existence of the sample sheet
@@ -129,15 +129,15 @@
     # THEN it should not raise a FlowCellError
     assert (
         validate_flow_cell_delivery_status(flow_cell_output_directory=tmp_path, force=True) is None
     )
 
 
 def test_validate_samples_have_fastq_files_passes(
-    novaseqx_flow_cell_with_sample_sheet_no_fastq: FlowCellDirectoryData,
+    novaseqx_flow_cell_with_sample_sheet_no_fastq: IlluminaRunDirectoryData,
 ):
     """Test the check of a flow cells with one sample fastq file does not raise an error."""
     # GIVEN a demultiplexed flow cell with no fastq files and a sample sheet
 
     # GIVEN that a valid sample fastq file is added to the directory
     sample_id: str = novaseqx_flow_cell_with_sample_sheet_no_fastq.sample_sheet.get_sample_ids()[0]
     fastq_file_path = Path(
```

### Comparing `cg-60.9.1/tests/meta/encryption/conftest.py` & `cg-60.9.3/tests/meta/encryption/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/encryption/test_encryption.py` & `cg-60.9.3/tests/meta/encryption/test_encryption.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 from cg.exc import FlowCellEncryptionError, FlowCellError
 from cg.meta.encryption.encryption import (
     EncryptionAPI,
     FlowCellEncryptionAPI,
     SpringEncryptionAPI,
 )
-from cg.models.flow_cell.flow_cell import FlowCellDirectoryData
+from cg.models.run_devices.illumina_run_directory_data import IlluminaRunDirectoryData
 
 
 @mock.patch("cg.utils.Process")
 def test_run_gpg_command(mock_process, binary_path: str, test_command: list[str]):
     """Tests the run_gpg_command method"""
     # GIVEN a CLI command input for the Process API
     command = test_command
@@ -378,16 +378,16 @@
     assert not flow_cell_encryption_api.pending_file_path.exists()
 
 
 def test_is_encryption_possible(flow_cell_encryption_api: FlowCellEncryptionAPI, mocker):
     # GIVEN a FlowCellEncryptionAPI
 
     # GIVEN that sequencing is ready
-    mocker.patch.object(FlowCellDirectoryData, "is_flow_cell_ready")
-    FlowCellDirectoryData.is_flow_cell_ready.return_value = True
+    mocker.patch.object(IlluminaRunDirectoryData, "is_sequencing_run_ready")
+    IlluminaRunDirectoryData.is_sequencing_run_ready.return_value = True
 
     # WHEN checking if encryption is possible
     is_possible: bool = flow_cell_encryption_api.is_encryption_possible()
 
     # THEN return True
     assert is_possible
 
@@ -396,16 +396,16 @@
     caplog, flow_cell_encryption_api: FlowCellEncryptionAPI, flow_cell_name: str, mocker
 ):
     caplog.set_level(logging.ERROR)
 
     # GIVEN a FlowCellEncryptionAPI
 
     # GIVEN that sequencing is not ready
-    mocker.patch.object(FlowCellDirectoryData, "is_flow_cell_ready")
-    FlowCellDirectoryData.is_flow_cell_ready.return_value = False
+    mocker.patch.object(IlluminaRunDirectoryData, "is_sequencing_run_ready")
+    IlluminaRunDirectoryData.is_sequencing_run_ready.return_value = False
 
     # WHEN checking if encryption is possible
     with pytest.raises(FlowCellError):
         flow_cell_encryption_api.is_encryption_possible()
 
         # THEN error should be raised
         assert f"Flow cell: {flow_cell_name} is not ready" in caplog.text
@@ -413,16 +413,16 @@
 
 def test_is_encryption_possible_when_encryption_is_completed(
     caplog, flow_cell_encryption_api: FlowCellEncryptionAPI, flow_cell_name: str, mocker
 ):
     # GIVEN a FlowCellEncryptionAPI
 
     # GIVEN that sequencing is ready
-    mocker.patch.object(FlowCellDirectoryData, "is_flow_cell_ready")
-    FlowCellDirectoryData.is_flow_cell_ready.return_value = True
+    mocker.patch.object(IlluminaRunDirectoryData, "is_sequencing_run_ready")
+    IlluminaRunDirectoryData.is_sequencing_run_ready.return_value = True
 
     # GIVEN that encryption is completed
     flow_cell_encryption_api.flow_cell_encryption_dir.mkdir(parents=True)
     flow_cell_encryption_api.complete_file_path.touch()
 
     # WHEN checking if encryption is possible
     with pytest.raises(FlowCellEncryptionError):
@@ -437,16 +437,16 @@
 
 def test_is_encryption_possible_when_encryption_is_pending(
     caplog, flow_cell_encryption_api: FlowCellEncryptionAPI, flow_cell_name: str, mocker
 ):
     # GIVEN a FlowCellEncryptionAPI
 
     # GIVEN that sequencing is ready
-    mocker.patch.object(FlowCellDirectoryData, "is_flow_cell_ready")
-    FlowCellDirectoryData.is_flow_cell_ready.return_value = True
+    mocker.patch.object(IlluminaRunDirectoryData, "is_sequencing_run_ready")
+    IlluminaRunDirectoryData.is_sequencing_run_ready.return_value = True
 
     # GIVEN that encryption is pending
     flow_cell_encryption_api.flow_cell_encryption_dir.mkdir(parents=True)
     flow_cell_encryption_api.pending_file_path.touch()
 
     # WHEN checking if encryption is possible
     with pytest.raises(FlowCellEncryptionError):
@@ -462,16 +462,16 @@
 def test_encrypt_flow_cell(
     caplog, flow_cell_encryption_api: FlowCellEncryptionAPI, mocker, sbatch_job_number: int
 ):
     caplog.set_level(logging.INFO)
     # GIVEN a FlowCellEncryptionAPI
 
     # GIVEN that sequencing is ready
-    mocker.patch.object(FlowCellDirectoryData, "is_flow_cell_ready")
-    FlowCellDirectoryData.is_flow_cell_ready.return_value = True
+    mocker.patch.object(IlluminaRunDirectoryData, "is_sequencing_run_ready")
+    IlluminaRunDirectoryData.is_sequencing_run_ready.return_value = True
 
     # WHEN encrypting flow cell
     flow_cell_encryption_api.encrypt_flow_cell()
 
     # THEN sbatch should be submitted
     assert f"Flow cell encryption running as job {sbatch_job_number}" in caplog.text
 
@@ -479,15 +479,15 @@
 def test_start_encryption(
     caplog, flow_cell_encryption_api: FlowCellEncryptionAPI, mocker, sbatch_job_number: int
 ):
     caplog.set_level(logging.INFO)
     # GIVEN a FlowCellEncryptionAPI
 
     # GIVEN that sequencing is ready
-    mocker.patch.object(FlowCellDirectoryData, "is_flow_cell_ready")
-    FlowCellDirectoryData.is_flow_cell_ready.return_value = True
+    mocker.patch.object(IlluminaRunDirectoryData, "is_sequencing_run_ready")
+    IlluminaRunDirectoryData.is_sequencing_run_ready.return_value = True
 
     # WHEN trying to start encrypting flow cell
     flow_cell_encryption_api.start_encryption()
 
     # THEN sbatch should be submitted
     assert f"Flow cell encryption running as job {sbatch_job_number}" in caplog.text
```

### Comparing `cg-60.9.1/tests/meta/observations/test_balsamic_observations_api.py` & `cg-60.9.3/tests/meta/observations/test_balsamic_observations_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/observations/test_mip_dna_observations_api.py` & `cg-60.9.3/tests/meta/observations/test_mip_dna_observations_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/observations/test_observations_api.py` & `cg-60.9.3/tests/meta/observations/test_observations_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/orders/conftest.py` & `cg-60.9.3/tests/meta/orders/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/orders/test_PoolSubmitter_validate_order.py` & `cg-60.9.3/tests/meta/orders/test_PoolSubmitter_validate_order.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py` & `cg-60.9.3/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/orders/test_SarsCov2Submitter_store_order.py` & `cg-60.9.3/tests/meta/orders/test_SarsCov2Submitter_store_order.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/orders/test_SarsCov2Submitter_validate_order.py` & `cg-60.9.3/tests/meta/orders/test_SarsCov2Submitter_validate_order.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/orders/test_meta_orders_api.py` & `cg-60.9.3/tests/meta/orders/test_meta_orders_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/orders/test_meta_orders_lims.py` & `cg-60.9.3/tests/meta/orders/test_meta_orders_lims.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/orders/test_meta_orders_status.py` & `cg-60.9.3/tests/meta/orders/test_meta_orders_status.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/orders/test_rnafusion_submitter.py` & `cg-60.9.3/tests/meta/orders/test_rnafusion_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/orders/test_ticket_handler.py` & `cg-60.9.3/tests/meta/orders/test_ticket_handler.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/qc_metrics/conftest.py` & `cg-60.9.3/tests/meta/qc_metrics/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/qc_metrics/test_collect_qc_metrics.py` & `cg-60.9.3/tests/meta/qc_metrics/test_collect_qc_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/report/conftest.py` & `cg-60.9.3/tests/meta/report/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/report/test_balsamic_api.py` & `cg-60.9.3/tests/meta/report/test_balsamic_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/report/test_field_validators.py` & `cg-60.9.3/tests/meta/report/test_field_validators.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/report/test_mip_dna_api.py` & `cg-60.9.3/tests/meta/report/test_mip_dna_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/report/test_report_api.py` & `cg-60.9.3/tests/meta/report/test_report_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/report/test_rnafusion_api.py` & `cg-60.9.3/tests/meta/report/test_rnafusion_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/report/test_tomte_api.py` & `cg-60.9.3/tests/meta/report/test_tomte_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/rsync/conftest.py` & `cg-60.9.3/tests/meta/rsync/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/rsync/test_rsync.py` & `cg-60.9.3/tests/meta/rsync/test_rsync.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/test_invoice.py` & `cg-60.9.3/tests/meta/test_invoice.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/transfer/conftest.py` & `cg-60.9.3/tests/meta/transfer/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/transfer/test_external_data.py` & `cg-60.9.3/tests/meta/transfer/test_external_data.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/transfer/test_meta_transfer_lims.py` & `cg-60.9.3/tests/meta/transfer/test_meta_transfer_lims.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/upload/balsamic/test_balsamic.py` & `cg-60.9.3/tests/meta/upload/balsamic/test_balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/upload/conftest.py` & `cg-60.9.3/tests/meta/upload/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/upload/gisaid/fixtures/four_samples.csv` & `cg-60.9.3/tests/meta/upload/gisaid/fixtures/four_samples.csv`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/upload/mutacc/conftest.py` & `cg-60.9.3/tests/meta/upload/mutacc/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/upload/mutacc/test_meta_upload_mutacc.py` & `cg-60.9.3/tests/meta/upload/mutacc/test_meta_upload_mutacc.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/upload/nipt/conftest.py` & `cg-60.9.3/tests/meta/upload/nipt/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/upload/nipt/test_models.py` & `cg-60.9.3/tests/meta/upload/nipt/test_models.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/upload/nipt/test_nipt_upload_api.py` & `cg-60.9.3/tests/meta/upload/nipt/test_nipt_upload_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/upload/scout/conftest.py` & `cg-60.9.3/tests/meta/upload/scout/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/upload/scout/test_generate_load_config.py` & `cg-60.9.3/tests/meta/upload/scout/test_generate_load_config.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/upload/scout/test_meta_upload_scoutapi.py` & `cg-60.9.3/tests/meta/upload/scout/test_meta_upload_scoutapi.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py` & `cg-60.9.3/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/upload/scout/test_scout_config_builder.py` & `cg-60.9.3/tests/meta/upload/scout/test_scout_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/upload/test_meta_upload_coverage.py` & `cg-60.9.3/tests/meta/upload/test_meta_upload_coverage.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/upload/test_upload_api.py` & `cg-60.9.3/tests/meta/upload/test_upload_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/upload/test_upload_genotypes_api.py` & `cg-60.9.3/tests/meta/upload/test_upload_genotypes_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/workflow/conftest.py` & `cg-60.9.3/tests/meta/workflow/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/workflow/microsalt/conftest.py` & `cg-60.9.3/tests/meta/workflow/microsalt/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/workflow/microsalt/test_quality_controller.py` & `cg-60.9.3/tests/meta/workflow/microsalt/test_quality_controller.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/workflow/microsalt/test_quality_controller_utils.py` & `cg-60.9.3/tests/meta/workflow/microsalt/test_quality_controller_utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/workflow/microsalt/test_report_generation.py` & `cg-60.9.3/tests/meta/workflow/microsalt/test_report_generation.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/workflow/test_analysis.py` & `cg-60.9.3/tests/meta/workflow/test_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/workflow/test_balsamic.py` & `cg-60.9.3/tests/meta/workflow/test_balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/workflow/test_fastq.py` & `cg-60.9.3/tests/meta/workflow/test_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/workflow/test_microsalt.py` & `cg-60.9.3/tests/meta/workflow/test_microsalt.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/workflow/test_nf_analysis.py` & `cg-60.9.3/tests/meta/workflow/test_nf_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/workflow/test_prepare_fastq_api.py` & `cg-60.9.3/tests/meta/workflow/test_prepare_fastq_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/workflow/test_raredisease.py` & `cg-60.9.3/tests/meta/workflow/test_raredisease.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/meta/workflow/test_rnafusion.py` & `cg-60.9.3/tests/meta/workflow/test_rnafusion.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/mocks/balsamic_analysis_mock.py` & `cg-60.9.3/tests/mocks/balsamic_analysis_mock.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/mocks/crunchy.py` & `cg-60.9.3/tests/mocks/crunchy.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/mocks/hk_mock.py` & `cg-60.9.3/tests/mocks/hk_mock.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/mocks/limsmock.py` & `cg-60.9.3/tests/mocks/limsmock.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/mocks/madeline.py` & `cg-60.9.3/tests/mocks/madeline.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/mocks/mip_analysis_mock.py` & `cg-60.9.3/tests/mocks/mip_analysis_mock.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/mocks/osticket.py` & `cg-60.9.3/tests/mocks/osticket.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/mocks/process_mock.py` & `cg-60.9.3/tests/mocks/process_mock.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/mocks/report.py` & `cg-60.9.3/tests/mocks/report.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/mocks/scout.py` & `cg-60.9.3/tests/mocks/scout.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/mocks/store_model.py` & `cg-60.9.3/tests/mocks/store_model.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/mocks/tb_mock.py` & `cg-60.9.3/tests/mocks/tb_mock.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/models/balsamic/conftest.py` & `cg-60.9.3/tests/models/balsamic/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/models/balsamic/test_balsamic_analysis.py` & `cg-60.9.3/tests/models/balsamic/test_balsamic_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/models/conftest.py` & `cg-60.9.3/tests/models/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/models/demultiplexing/test_run_parameters.py` & `cg-60.9.3/tests/models/demultiplexing/test_run_parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from cg.exc import RunParametersError, XMLError
 from cg.models.demultiplex.run_parameters import (
     RunParameters,
     RunParametersHiSeq,
     RunParametersNovaSeq6000,
     RunParametersNovaSeqX,
 )
-from cg.models.flow_cell.flow_cell import FlowCellDirectoryData
+from cg.models.run_devices.illumina_run_directory_data import IlluminaRunDirectoryData
 
 
 @pytest.mark.parametrize(
     "run_parameters_path_fixture",
     [
         "hiseq_x_single_index_run_parameters_path",
         "hiseq_2500_dual_index_run_parameters_path",
@@ -274,39 +274,39 @@
     ],
 )
 def test_is_novaseq6000_post_1_5_kit(
     flow_cell_fixture: str, expected_result: bool, request: FixtureRequest
 ):
     """Test that the correct index settings are returned for each NovaSeq flow cell type."""
     # GIVEN run parameters from a flow cell
-    flow_cell: FlowCellDirectoryData = request.getfixturevalue(flow_cell_fixture)
+    flow_cell: IlluminaRunDirectoryData = request.getfixturevalue(flow_cell_fixture)
     # WHEN checking if the flow cell was sequenced after the NovaSeq 6000 1.5 kits
     result: bool = flow_cell.run_parameters._is_novaseq6000_post_1_5_kit()
     # THEN the correct index settings are returned
     assert result == expected_result
 
 
 @pytest.mark.parametrize(
-    "flow_cell, correct_settings",
+    "sequencing_run, correct_settings",
     [
         ("novaseq_6000_pre_1_5_kits_flow_cell", NO_REVERSE_COMPLEMENTS_INDEX_SETTINGS),
         ("novaseq_6000_post_1_5_kits_flow_cell", NOVASEQ_6000_POST_1_5_KITS_INDEX_SETTINGS),
         ("novaseq_x_flow_cell", NOVASEQ_X_INDEX_SETTINGS),
     ],
 )
 def test_get_index_settings(
     correct_settings: IndexSettings,
-    flow_cell: str,
+    sequencing_run: str,
     request: FixtureRequest,
 ):
     """Test that the correct index settings are returned for each NovaSeq flow cell type."""
     # GIVEN run parameters for a flow cell
-    flow_cell: FlowCellDirectoryData = request.getfixturevalue(flow_cell)
+    sequencing_run: IlluminaRunDirectoryData = request.getfixturevalue(sequencing_run)
     # WHEN getting the index settings
-    settings: IndexSettings = flow_cell.run_parameters.index_settings
+    settings: IndexSettings = sequencing_run.run_parameters.index_settings
     # THEN the correct index settings are returned
     assert settings == correct_settings
 
 
 @pytest.mark.parametrize(
     "run_parameters_fixture, expected_result",
     [
```

### Comparing `cg-60.9.1/tests/models/downsample/test_down_sample_meta_data.py` & `cg-60.9.3/tests/models/downsample/test_down_sample_meta_data.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/models/flow_cell/test_flowcell_model.py` & `cg-60.9.3/tests/models/flow_cell/test_flowcell_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,45 +5,45 @@
 from _pytest.fixtures import FixtureRequest
 
 from cg.cli.demultiplex.copy_novaseqx_demultiplex_data import get_latest_analysis_path
 from cg.constants.demultiplexing import DemultiplexingDirsAndFiles
 from cg.constants.sequencing import Sequencers
 from cg.exc import FlowCellError
 from cg.models.demultiplex.run_parameters import RunParameters
-from cg.models.flow_cell.flow_cell import FlowCellDirectoryData
+from cg.models.run_devices.illumina_run_directory_data import IlluminaRunDirectoryData
 from cg.utils.flow_cell import get_flow_cell_id
 
 
 def test_flow_cell_id(hiseq_2500_dual_index_flow_cell_dir: Path):
     """Test parsing of flow cell id."""
     # GIVEN the path to a finished flow cell run
     # GIVEN the flow cell id
     flowcell_id: str = get_flow_cell_id(hiseq_2500_dual_index_flow_cell_dir.name)
 
     # WHEN instantiating a flow cell object
-    flowcell_obj = FlowCellDirectoryData(flow_cell_path=hiseq_2500_dual_index_flow_cell_dir)
+    flowcell_obj = IlluminaRunDirectoryData(sequencing_run_path=hiseq_2500_dual_index_flow_cell_dir)
 
     # THEN assert that the flow cell id is parsed
     assert flowcell_obj.id == flowcell_id
 
 
 def test_flow_cell_position(hiseq_2500_dual_index_flow_cell_dir: Path):
     """Test getting flow cell position."""
     # GIVEN the path to a finished flow cell
     # GIVEN a flow cell object
-    flow_cell = FlowCellDirectoryData(flow_cell_path=hiseq_2500_dual_index_flow_cell_dir)
+    flow_cell = IlluminaRunDirectoryData(sequencing_run_path=hiseq_2500_dual_index_flow_cell_dir)
 
     # WHEN fetching the flow cell position
     position = flow_cell.position
 
     # THEN assert it is A or B
     assert position in ["A", "B"]
 
 
-def test_rta_exists(novaseq_6000_pre_1_5_kits_flow_cell: FlowCellDirectoryData):
+def test_rta_exists(novaseq_6000_pre_1_5_kits_flow_cell: IlluminaRunDirectoryData):
     """Test return of RTS file."""
     # GIVEN the path to a finished flow cell
     # GIVEN a flow cell object
 
     # WHEN fetching the path to the RTA file
     rta_file: Path = novaseq_6000_pre_1_5_kits_flow_cell.rta_complete_path
 
@@ -59,15 +59,15 @@
         "hiseq_2500_dual_index_flow_cell",
         "hiseq_2500_custom_index_flow_cell",
     ],
 )
 def test_run_parameters_path(flow_cell_fixture: str, request: FixtureRequest):
     """Test that the run parameters file is being fetched correctly for the HiSeq flow cells."""
     # GIVEN a flow cell with a run parameters
-    flow_cell: FlowCellDirectoryData = request.getfixturevalue(flow_cell_fixture)
+    flow_cell: IlluminaRunDirectoryData = request.getfixturevalue(flow_cell_fixture)
 
     # WHEN getting the run parameters file name
     run_parameters_path: Path = flow_cell.run_parameters_path
 
     # THEN it should exist and be the expected one
     assert run_parameters_path.exists()
     assert (
@@ -75,21 +75,23 @@
         or run_parameters_path.name == DemultiplexingDirsAndFiles.RUN_PARAMETERS_PASCAL_CASE
     )
 
 
 def test_run_parameters_path_when_non_existing(tmp_flow_cell_without_run_parameters_path: Path):
     """Test that getting the path of the run parameters path fails if the file does not exist."""
     # GIVEN a flowcell object with a directory without a run parameters file
-    flow_cell = FlowCellDirectoryData(flow_cell_path=tmp_flow_cell_without_run_parameters_path)
+    flow_cell = IlluminaRunDirectoryData(
+        sequencing_run_path=tmp_flow_cell_without_run_parameters_path
+    )
 
     # WHEN fetching the run parameters path
     with pytest.raises(FlowCellError) as exc:
         # THEN a FlowCellError is raised
         flow_cell.run_parameters_path
-    assert "No run parameters file found in flow cell" in str(exc.value)
+    assert "No run parameters file found in sequencing run" in str(exc.value)
 
 
 @pytest.mark.parametrize(
     "flow_cell_fixture, expected_sequencer",
     [
         ("hiseq_2500_custom_index_flow_cell", Sequencers.HISEQGA),
         ("hiseq_x_single_index_flow_cell", Sequencers.HISEQX),
@@ -98,55 +100,55 @@
     ],
 )
 def test_flow_cell_run_parameters_type(
     flow_cell_fixture: str, expected_sequencer: str, request: FixtureRequest
 ):
     """Test that the run parameters of the flow cell is of the expected type."""
     # GIVEN a flow cell without _run_parameters
-    flow_cell: FlowCellDirectoryData = request.getfixturevalue(flow_cell_fixture)
+    flow_cell: IlluminaRunDirectoryData = request.getfixturevalue(flow_cell_fixture)
     assert not flow_cell._run_parameters
 
     # WHEN creating the run parameters of the flow cell
     run_parameters: RunParameters = flow_cell.run_parameters
 
     # THEN the run parameters sequencer is the same as of the flow cell
     assert run_parameters.sequencer == expected_sequencer
 
 
 def test_has_demultiplexing_started_locally_false(tmp_flow_cell_directory_bcl_convert: Path):
     # GIVEN a flow cell without a demuxstarted.txt file
-    flow_cell = FlowCellDirectoryData(tmp_flow_cell_directory_bcl_convert)
+    flow_cell = IlluminaRunDirectoryData(tmp_flow_cell_directory_bcl_convert)
     assert not Path(flow_cell.path, DemultiplexingDirsAndFiles.DEMUX_STARTED).exists()
 
     # WHEN checking if the flow cell has started demultiplexing
     has_demux_started: bool = flow_cell.has_demultiplexing_started_locally()
 
     # THEN the response should be False
     assert not has_demux_started
 
 
 def test_has_demultiplexing_started_locally_true(
     tmp_flow_cell_directory_bcl_convert: Path,
 ):
     # GIVEN a flow cell with a demuxstarted.txt file
-    flow_cell = FlowCellDirectoryData(tmp_flow_cell_directory_bcl_convert)
+    flow_cell = IlluminaRunDirectoryData(tmp_flow_cell_directory_bcl_convert)
     Path(flow_cell.path, DemultiplexingDirsAndFiles.DEMUX_STARTED).touch()
 
     # WHEN checking if the flow cell has started demultiplexing
     has_demux_started: bool = flow_cell.has_demultiplexing_started_locally()
 
     # THEN the response should be True
     assert has_demux_started
 
 
 def test_has_demultiplexing_started_on_sequencer_true(
     novaseqx_flow_cell_dir_with_analysis_data: Path,
 ):
     # GIVEN a flow cell with a BCLConvert folder
-    flow_cell = FlowCellDirectoryData(novaseqx_flow_cell_dir_with_analysis_data)
+    flow_cell = IlluminaRunDirectoryData(novaseqx_flow_cell_dir_with_analysis_data)
     Path.mkdir(
         Path(
             flow_cell.path,
             get_latest_analysis_path(flow_cell.path),
             DemultiplexingDirsAndFiles.DATA,
             DemultiplexingDirsAndFiles.BCL_CONVERT,
         )
@@ -159,15 +161,15 @@
     assert has_demux_started
 
 
 def test_has_demultiplexing_started_on_sequencer_false(
     novaseqx_flow_cell_dir_with_analysis_data: Path,
 ):
     # GIVEN a flow cell without a BCLConvert folder
-    flow_cell = FlowCellDirectoryData(novaseqx_flow_cell_dir_with_analysis_data)
+    flow_cell = IlluminaRunDirectoryData(novaseqx_flow_cell_dir_with_analysis_data)
     assert not Path(
         flow_cell.path,
         get_latest_analysis_path(flow_cell.path),
         DemultiplexingDirsAndFiles.DATA,
         DemultiplexingDirsAndFiles.BCL_CONVERT,
     ).exists()
 
@@ -176,28 +178,28 @@
 
     # THEN the response should be False
     assert not has_demux_started
 
 
 def test_sequencing_dates_novaseqx_flow_cell(novaseq_x_flow_cell_dir: Path):
     # GIVEN a flow cell directory data for a novaseq x flow cell
-    flow_cell = FlowCellDirectoryData(novaseq_x_flow_cell_dir)
+    flow_cell = IlluminaRunDirectoryData(novaseq_x_flow_cell_dir)
 
     # WHEN fetching the sequencing start and end dates
     start_date: datetime = flow_cell.sequencing_started_at
     end_date: datetime = flow_cell.sequencing_completed_at
 
     # THEN the dates should be set
     assert isinstance(start_date, datetime.datetime)
     assert isinstance(end_date, datetime.datetime)
 
 
 def test_sequencing_dates_novaseq_6000_flow_cell(novaseq_6000_post_1_5_kits_flow_cell_path: Path):
     # GIVEN a flow cell directory data for a novaseq 6000 flow cell
-    flow_cell = FlowCellDirectoryData(novaseq_6000_post_1_5_kits_flow_cell_path)
+    flow_cell = IlluminaRunDirectoryData(novaseq_6000_post_1_5_kits_flow_cell_path)
 
     # WHEN fetching the sequencing start and end dates
     start_date: datetime = flow_cell.sequencing_started_at
     end_date: datetime = flow_cell.sequencing_completed_at
 
     # THEN none of the dates should be set
     assert not start_date
```

### Comparing `cg-60.9.1/tests/models/mip/conftest.py` & `cg-60.9.3/tests/models/mip/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/models/mip/test_mip_analysis.py` & `cg-60.9.3/tests/models/mip/test_mip_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/models/mip/test_mip_config.py` & `cg-60.9.3/tests/models/mip/test_mip_config.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/models/mip/test_mip_metrics_deliverables.py` & `cg-60.9.3/tests/models/mip/test_mip_metrics_deliverables.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/models/mip/test_mip_sample_info.py` & `cg-60.9.3/tests/models/mip/test_mip_sample_info.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/models/nextflow/test_nextflow_deliver.py` & `cg-60.9.3/tests/models/nextflow/test_nextflow_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/models/observations/test_observations_input_files.py` & `cg-60.9.3/tests/models/observations/test_observations_input_files.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/models/report/test_validators.py` & `cg-60.9.3/tests/models/report/test_validators.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/models/rnafusion/test_rnafusion_sample.py` & `cg-60.9.3/tests/models/rnafusion/test_rnafusion_sample.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/models/test_cg_models.py` & `cg-60.9.3/tests/models/test_cg_models.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/models/test_compression_data.py` & `cg-60.9.3/tests/models/test_compression_data.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/models/test_fastq.py` & `cg-60.9.3/tests/models/test_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/models/test_file_data.py` & `cg-60.9.3/tests/models/test_file_data.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/server/conftest.py` & `cg-60.9.3/tests/server/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/server/endpoints/test_delivery_message_endpoint.py` & `cg-60.9.3/tests/server/endpoints/test_delivery_message_endpoint.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/server/endpoints/test_orders_endpoint.py` & `cg-60.9.3/tests/server/endpoints/test_orders_endpoint.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/services/fastq_file_service/conftest.py` & `cg-60.9.3/tests/services/fastq_file_service/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/services/fastq_file_service/test_fastq_file_service.py` & `cg-60.9.3/tests/services/fastq_file_service/test_fastq_file_service.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/services/illumina_services/illumina_demux_version_service/conftest.py` & `cg-60.9.3/tests/services/illumina_services/illumina_demux_version_service/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/services/illumina_services/illumina_demux_version_service/test_illumina_demux_version_service.py` & `cg-60.9.3/tests/services/illumina_services/illumina_demux_version_service/test_illumina_demux_version_service.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/services/illumina_services/illumina_metrics_service/conftest.py` & `cg-60.9.3/tests/services/illumina_services/illumina_metrics_service/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/services/illumina_services/illumina_metrics_service/parsers/test_bclconvert_metrics_parser.py` & `cg-60.9.3/tests/services/illumina_services/illumina_metrics_service/parsers/test_bclconvert_metrics_parser.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/services/illumina_services/illumina_metrics_service/parsers/test_illumina_metrics_service.py` & `cg-60.9.3/tests/services/illumina_services/illumina_metrics_service/parsers/test_illumina_metrics_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Tests for the sequencing metrics parser API."""
 
 from pathlib import Path
 
-from cg.models.flow_cell.flow_cell import FlowCellDirectoryData
+from cg.models.run_devices.illumina_run_directory_data import IlluminaRunDirectoryData
 
 
 from cg.services.illumina_services.illumina_metrics_service.bcl_convert_metrics_parser import (
     BCLConvertMetricsParser,
 )
 from cg.services.illumina_services.illumina_metrics_service.illumina_metrics_service import (
     IlluminaMetricsService,
@@ -37,15 +37,15 @@
     assert (
         len(sequencing_statistics_list)
         == len(parsed_bcl_convert_metrics.get_sample_internal_ids()) * 2
     )
 
 
 def test_create_undetermined_non_pooled_metrics(
-    hiseq_x_single_index_demultiplexed_flow_cell_with_sample_sheet: FlowCellDirectoryData,
+    hiseq_x_single_index_demultiplexed_flow_cell_with_sample_sheet: IlluminaRunDirectoryData,
     illumina_metrics_service: IlluminaMetricsService,
 ):
     """Test creating undetermined sequencing statistics from demultiplex metrics."""
     # GIVEN a directory with a demultiplexed flow cell with undetermined reads
 
     # WHEN creating undetermined sequencing statistics from bcl convert metrics
     metrics: list[SampleLaneSequencingMetrics] = (
@@ -65,15 +65,15 @@
 ):
     """
     Test creating undetermined sequencing statistics from demultiplex metrics without undetermined
     reads.
     """
 
     # GIVEN a directory with a demultiplexed flow cell without undetermined reads in a lane
-    flow_cell = FlowCellDirectoryData(bcl_convert_metrics_dir_path)
+    flow_cell = IlluminaRunDirectoryData(bcl_convert_metrics_dir_path)
     sample_sheet_path = Path(bcl_convert_metrics_dir_path, "SampleSheet.csv")
     flow_cell.set_sample_sheet_path_hk(hk_path=sample_sheet_path)
 
     # WHEN creating undetermined sequencing statistics specifying a lane without undetermined reads
     metrics: list[SampleLaneSequencingMetrics] = (
         illumina_metrics_service.create_undetermined_non_pooled_metrics(flow_cell=flow_cell)
     )
```

### Comparing `cg-60.9.1/tests/services/illumina_services/illumina_post_processing_service/conftest.py` & `cg-60.9.3/tests/services/illumina_services/illumina_post_processing_service/conftest.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 
 import pytest
 
 from cg.apps.housekeeper.hk import HousekeeperAPI
 from cg.constants.devices import DeviceType
-from cg.models.flow_cell.flow_cell import FlowCellDirectoryData
+from cg.models.run_devices.illumina_run_directory_data import IlluminaRunDirectoryData
 from cg.services.illumina_services.illumina_post_processing_service.illumina_post_processing_service import (
     IlluminaPostProcessingService,
 )
 from cg.store.models import IlluminaFlowCell
 from cg.store.store import Store
 from tests.store_helpers import StoreHelpers
 
@@ -27,14 +27,16 @@
         helpers.add_sample(store, internal_id=sample_id)
     return IlluminaPostProcessingService(
         status_db=store, housekeeper_api=real_housekeeper_api, dry_run=False
     )
 
 
 @pytest.fixture
-def illumina_flow_cell(novaseq_x_demux_runs_flow_cell: FlowCellDirectoryData) -> IlluminaFlowCell:
+def illumina_flow_cell(
+    novaseq_x_demux_runs_flow_cell: IlluminaRunDirectoryData,
+) -> IlluminaFlowCell:
     """Return an Illumina flow cell."""
     return IlluminaFlowCell(
         internal_id=novaseq_x_demux_runs_flow_cell.id,
         type=DeviceType.ILLUMINA,
         model=novaseq_x_demux_runs_flow_cell.run_parameters.get_flow_cell_model(),
     )
```

### Comparing `cg-60.9.1/tests/services/illumina_services/illumina_post_processing_service/test_illumina_post_processing_service.py` & `cg-60.9.3/tests/services/illumina_services/illumina_post_processing_service/test_illumina_post_processing_service.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Module to test the illumina post processing service."""
 
-from cg.models.flow_cell.flow_cell import FlowCellDirectoryData
+from cg.models.run_devices.illumina_run_directory_data import IlluminaRunDirectoryData
 from cg.services.illumina_services.illumina_post_processing_service.illumina_post_processing_service import (
     IlluminaPostProcessingService,
 )
 from cg.store.models import IlluminaFlowCell, IlluminaSequencingRun, IlluminaSampleSequencingMetrics
 
 
 def test_get_illumina_flow_cell(
-    novaseq_x_demux_runs_flow_cell: FlowCellDirectoryData,
+    novaseq_x_demux_runs_flow_cell: IlluminaRunDirectoryData,
     illumina_post_postprocessing_service: IlluminaPostProcessingService,
 ):
     # GIVEN a flow cell directory data and an Illumina post processing service
 
     # WHEN creating an Illumina flow cell
     flow_cell: IlluminaFlowCell = illumina_post_postprocessing_service.store_illumina_flow_cell(
         flow_cell_dir_data=novaseq_x_demux_runs_flow_cell
@@ -20,15 +20,15 @@
 
     # THEN assert that the flow cell is created
     assert isinstance(flow_cell, IlluminaFlowCell)
     assert flow_cell.internal_id == novaseq_x_demux_runs_flow_cell.id
 
 
 def test_get_illumina_sequencing_run(
-    novaseq_x_demux_runs_flow_cell: FlowCellDirectoryData,
+    novaseq_x_demux_runs_flow_cell: IlluminaRunDirectoryData,
     illumina_flow_cell: IlluminaFlowCell,
     illumina_post_postprocessing_service: IlluminaPostProcessingService,
 ):
     # GIVEN a flow cell directory data and an Illumina post processing service
 
     # WHEN creating an Illumina sequencing run
     sequencing_run: IlluminaSequencingRun = (
@@ -38,15 +38,15 @@
     )
 
     # THEN assert that the sequencing run is created
     assert isinstance(sequencing_run, IlluminaSequencingRun)
 
 
 def test_get_illumina_sample_sequencing_metrics(
-    novaseq_x_demux_runs_flow_cell: FlowCellDirectoryData,
+    novaseq_x_demux_runs_flow_cell: IlluminaRunDirectoryData,
     illumina_post_postprocessing_service: IlluminaPostProcessingService,
 ):
     # GIVEN a flow cell directory data and an Illumina post processing service
     flow_cell: IlluminaFlowCell = illumina_post_postprocessing_service.store_illumina_flow_cell(
         novaseq_x_demux_runs_flow_cell
     )
     sequencing_run: IlluminaSequencingRun = (
@@ -65,15 +65,15 @@
 
     # THEN assert that the sample metrics are created
     assert isinstance(sample_metrics, list)
     assert isinstance(sample_metrics[0], IlluminaSampleSequencingMetrics)
 
 
 def test_store_illumina_flow_cell_data(
-    novaseq_x_demux_runs_flow_cell: FlowCellDirectoryData,
+    novaseq_x_demux_runs_flow_cell: IlluminaRunDirectoryData,
     illumina_post_postprocessing_service: IlluminaPostProcessingService,
 ):
     # GIVEN a flow cell directory data and an Illumina post processing service
 
     # WHEN storing the flow cell data
     illumina_post_postprocessing_service.store_illumina_flow_cell_data(
         flow_cell_dir_data=novaseq_x_demux_runs_flow_cell
```

### Comparing `cg-60.9.1/tests/services/orders/order_status_service/conftest.py` & `cg-60.9.3/tests/services/orders/order_status_service/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/services/orders/order_status_service/test_order_summary_service.py` & `cg-60.9.3/tests/services/orders/order_status_service/test_order_summary_service.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/services/parse_completion_status_service/conftest.py` & `cg-60.9.3/tests/services/parse_completion_status_service/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/services/parse_completion_status_service/test_parse_completion_status_service.py` & `cg-60.9.3/tests/services/parse_completion_status_service/test_parse_completion_status_service.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/services/sequencing_qc_service/test_sequencing_quality_checks_utils.py` & `cg-60.9.3/tests/services/sequencing_qc_service/test_sequencing_quality_checks_utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/services/validate_file_transfer_service/conftest.py` & `cg-60.9.3/tests/services/validate_file_transfer_service/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/services/validate_file_transfer_service/test_validate_file_transfer_service.py` & `cg-60.9.3/tests/services/validate_file_transfer_service/test_validate_file_transfer_service.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/services/validate_file_transfer_service/test_validate_pacbio_file_transfer_service.py` & `cg-60.9.3/tests/services/validate_file_transfer_service/test_validate_pacbio_file_transfer_service.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/store/api/conftest.py` & `cg-60.9.3/tests/store/api/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/store/api/test_base.py` & `cg-60.9.3/tests/store/api/test_base.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/store/conftest.py` & `cg-60.9.3/tests/store/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/store/crud/add/test_store_add_application_version.py` & `cg-60.9.3/tests/store/crud/add/test_store_add_application_version.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/store/crud/add/test_store_add_base.py` & `cg-60.9.3/tests/store/crud/add/test_store_add_base.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/store/crud/add/test_store_add_customer.py` & `cg-60.9.3/tests/store/crud/add/test_store_add_customer.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/store/crud/add/test_store_add_flow_celll.py` & `cg-60.9.3/tests/store/crud/add/test_store_add_flow_celll.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/store/crud/conftest.py` & `cg-60.9.3/tests/store/crud/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/store/crud/delete/test_delete.py` & `cg-60.9.3/tests/store/crud/delete/test_delete.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/store/crud/read/test_read.py` & `cg-60.9.3/tests/store/crud/read/test_read.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/store/crud/read/test_read_analyses_to_clean.py` & `cg-60.9.3/tests/store/crud/read/test_read_analyses_to_clean.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/store/crud/read/test_read_analyses_to_delivery_report.py` & `cg-60.9.3/tests/store/crud/read/test_read_analyses_to_delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/store/crud/read/test_read_analysis.py` & `cg-60.9.3/tests/store/crud/read/test_read_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/store/crud/read/test_read_application_version.py` & `cg-60.9.3/tests/store/crud/read/test_read_application_version.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/store/crud/read/test_read_customer.py` & `cg-60.9.3/tests/store/crud/read/test_read_customer.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/store/crud/read/test_read_illumina_flow_cell.py` & `cg-60.9.3/tests/store/crud/read/test_read_illumina_flow_cell.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/store/crud/read/test_read_pool.py` & `cg-60.9.3/tests/store/crud/read/test_read_pool.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/store/crud/read/test_read_sample.py` & `cg-60.9.3/tests/store/crud/read/test_read_sample.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/store/crud/update/test_update.py` & `cg-60.9.3/tests/store/crud/update/test_update.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/store/filters/test_status_analyses_filters.py` & `cg-60.9.3/tests/store/filters/test_status_analyses_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/store/filters/test_status_application_filters.py` & `cg-60.9.3/tests/store/filters/test_status_application_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/store/filters/test_status_application_limitations_filters.py` & `cg-60.9.3/tests/store/filters/test_status_application_limitations_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/store/filters/test_status_application_version_filters.py` & `cg-60.9.3/tests/store/filters/test_status_application_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/store/filters/test_status_bed_filters.py` & `cg-60.9.3/tests/store/filters/test_status_bed_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/store/filters/test_status_bed_version_filters.py` & `cg-60.9.3/tests/store/filters/test_status_bed_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/store/filters/test_status_case_sample_filters.py` & `cg-60.9.3/tests/store/filters/test_status_case_sample_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/store/filters/test_status_cases_filters.py` & `cg-60.9.3/tests/store/filters/test_status_cases_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/store/filters/test_status_collaboration_filters.py` & `cg-60.9.3/tests/store/filters/test_status_collaboration_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/store/filters/test_status_customer_filters.py` & `cg-60.9.3/tests/store/filters/test_status_customer_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/store/filters/test_status_flow_cell_filters.py` & `cg-60.9.3/tests/store/filters/test_status_flow_cell_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/store/filters/test_status_illumina_flow_cell_filters.py` & `cg-60.9.3/tests/store/filters/test_status_illumina_flow_cell_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/store/filters/test_status_invoice_filters.py` & `cg-60.9.3/tests/store/filters/test_status_invoice_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/store/filters/test_status_metrics_filters.py` & `cg-60.9.3/tests/store/filters/test_status_metrics_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/store/filters/test_status_organism_filters.py` & `cg-60.9.3/tests/store/filters/test_status_organism_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/store/filters/test_status_panel_filters.py` & `cg-60.9.3/tests/store/filters/test_status_panel_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/store/filters/test_status_pool_filters.py` & `cg-60.9.3/tests/store/filters/test_status_pool_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/store/filters/test_status_samples_filters.py` & `cg-60.9.3/tests/store/filters/test_status_samples_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/store/filters/test_status_user_filters.py` & `cg-60.9.3/tests/store/filters/test_status_user_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/store/test_delivery.py` & `cg-60.9.3/tests/store/test_delivery.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/store/test_store_models.py` & `cg-60.9.3/tests/store/test_store_models.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/store_helpers.py` & `cg-60.9.3/tests/store_helpers.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/test_copy_novaseqx_flow_cell.py` & `cg-60.9.3/tests/test_copy_novaseqx_flow_cell.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/test_store_helpers.py` & `cg-60.9.3/tests/test_store_helpers.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/utils/conftest.py` & `cg-60.9.3/tests/utils/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/utils/test_checksum.py` & `cg-60.9.3/tests/utils/test_checksum.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/utils/test_commands.py` & `cg-60.9.3/tests/utils/test_commands.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/utils/test_date.py` & `cg-60.9.3/tests/utils/test_date.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/utils/test_dict.py` & `cg-60.9.3/tests/utils/test_dict.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/utils/test_dispatcher.py` & `cg-60.9.3/tests/utils/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/utils/test_files.py` & `cg-60.9.3/tests/utils/test_files.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/utils/test_time.py` & `cg-60.9.3/tests/utils/test_time.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/tests/utils/test_utils.py` & `cg-60.9.3/tests/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.9.1/PKG-INFO` & `cg-60.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cg
-Version: 60.9.1
+Version: 60.9.3
 Summary: Clinical Genomics command center
 Home-page: https://github.com/Clinical-Genomics/cg
 Author: Clinical Genomics
 Author-email: support@clinicalgenomics.se
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

