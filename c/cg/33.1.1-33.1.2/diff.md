# Comparing `tmp/cg-33.1.1.tar.gz` & `tmp/cg-33.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cg-33.1.1.tar", last modified: Thu Jun  1 12:37:10 2023, max compression
+gzip compressed data, was "dist/cg-33.1.2.tar", last modified: Thu Jun  1 13:39:27 2023, max compression
```

## Comparing `cg-33.1.1.tar` & `cg-33.1.2.tar`

### file list

```diff
@@ -1,1283 +1,1269 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-01 12:37:02.000000 cg-33.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-06-01 12:37:10.000000 cg-33.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-06-01 12:37:02.000000 cg-33.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-01 12:37:02.000000 cg-33.1.1/cg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/apps/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/apps/cgstats/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/cgstats/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/apps/cgstats/crud/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/cgstats/crud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16023 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/cgstats/crud/create.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/cgstats/crud/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     7927 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/cgstats/crud/find.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/apps/cgstats/db/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/cgstats/db/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/apps/cgstats/db/models/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/cgstats/db/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/cgstats/db/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/cgstats/db/models/datasource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/cgstats/db/models/demux.py
--rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/cgstats/db/models/demux_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/cgstats/db/models/dragen_demux_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/cgstats/db/models/flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/cgstats/db/models/project.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/cgstats/db/models/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/cgstats/db/models/support_params.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/cgstats/db/models/unaligned.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/cgstats/db/models/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/apps/cgstats/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/cgstats/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/cgstats/parsers/adapter_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    11317 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/cgstats/parsers/conversion_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/cgstats/parsers/demux_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/cgstats/parsers/dragen_demultiplexing_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/cgstats/parsers/quality_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/cgstats/parsers/run_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     6315 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/cgstats/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/apps/coverage/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/coverage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/coverage/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/apps/crunchy/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/crunchy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12884 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/crunchy/crunchy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/crunchy/files.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/crunchy/sbatch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/apps/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/demultiplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11469 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/demultiplex/demultiplex_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/demultiplex/demux_report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/apps/demultiplex/sample_sheet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/demultiplex/sample_sheet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/demultiplex/sample_sheet/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/demultiplex/sample_sheet/dummy_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/demultiplex/sample_sheet/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/demultiplex/sample_sheet/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/demultiplex/sample_sheet/novaseq_sample_sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/demultiplex/sample_sheet/validate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/demultiplex/sbatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/environ.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/gens.py
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/gt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/apps/hermes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/hermes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/hermes/hermes_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/hermes/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/apps/housekeeper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/housekeeper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17304 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/housekeeper/hk.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/housekeeper/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/apps/invoice/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/invoice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/invoice/render.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/apps/invoice/templates/
--rw-r--r--   0 runner    (1001) docker     (123)   113439 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/invoice/templates/KI_pool_invoice.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    81032 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/invoice/templates/KI_sample_invoice.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   113363 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/invoice/templates/KTH_pool_invoice.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    80886 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/invoice/templates/KTH_sample_invoice.xlsx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/apps/lims/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/lims/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16393 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/lims/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/lims/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     8243 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/lims/order.py
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/lims/sample_sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/loqus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/apps/madeline/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/madeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/madeline/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/apps/mip/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/mip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/mip/confighandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/mutacc_auto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/apps/orderform/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/orderform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9233 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/orderform/excel_orderform_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/orderform/json_orderform_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6387 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/orderform/orderform_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/osticket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/apps/scout/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/scout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/scout/scout_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     9438 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/scout/scoutapi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/apps/sequencing_metrics_parser/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/sequencing_metrics_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/sequencing_metrics_parser/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/apps/sequencing_metrics_parser/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/sequencing_metrics_parser/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/sequencing_metrics_parser/models/bcl2fastq_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/sequencing_metrics_parser/models/bcl_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/apps/sequencing_metrics_parser/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/sequencing_metrics_parser/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5659 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/sequencing_metrics_parser/parsers/bcl2fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/sequencing_metrics_parser/parsers/bcl2fastq_to_sequencing_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     8990 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/sequencing_metrics_parser/parsers/bcl_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/sequencing_metrics_parser/parsers/bcl_convert_to_sequencing_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/sequencing_metrics_parser/sequencing_metrics_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/apps/slurm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/slurm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/slurm/sbatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/slurm/slurm_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/apps/tb/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/tb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7646 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/tb/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/tb/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-06-01 12:37:02.000000 cg-33.1.1/cg/apps/vogue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10329 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     7057 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    19665 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/clean.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/cli/compress/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/compress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/compress/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/compress/fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     8507 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/compress/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/cli/delete/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/delete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/delete/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/delete/case.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/delete/cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/delete/observations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/cli/deliver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/deliver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/deliver/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/cli/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/demultiplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/demultiplex/add.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/demultiplex/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/demultiplex/demux.py
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/demultiplex/finish.py
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/demultiplex/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/demultiplex/sample_sheet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/cli/generate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/generate/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/cli/generate/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/generate/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/generate/report/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/generate/report/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/generate/report/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8386 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/cli/set/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/set/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/set/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/set/case.py
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/set/cases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/cli/store/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/store/fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/store/store.py
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/transfer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/cli/upload/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/upload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/upload/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/upload/clinical_delivery.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/upload/coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/upload/delivery_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/upload/fohm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/upload/genotype.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/upload/gens.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/upload/gisaid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/upload/mutacc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/cli/upload/nipt/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/upload/nipt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/upload/nipt/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/upload/nipt/ftp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/upload/nipt/statina.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/cli/upload/observations/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/upload/observations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/upload/observations/observations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/upload/observations/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9563 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/upload/scout.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/upload/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/upload/validate.py
--rw-r--r--   0 runner    (1001) docker     (123)    11932 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/upload/vogue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/cli/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/workflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/cli/workflow/balsamic/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/workflow/balsamic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8860 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/workflow/balsamic/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/workflow/balsamic/options.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/workflow/balsamic/pon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/workflow/balsamic/qc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/workflow/balsamic/umi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/workflow/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12622 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/workflow/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/cli/workflow/fastq/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/workflow/fastq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/workflow/fastq/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/cli/workflow/fluffy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/workflow/fluffy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/workflow/fluffy/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/cli/workflow/microsalt/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/workflow/microsalt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11101 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/workflow/microsalt/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/cli/workflow/mip/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/workflow/mip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/workflow/mip/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/workflow/mip/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/cli/workflow/mip_dna/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/workflow/mip_dna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/workflow/mip_dna/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/cli/workflow/mip_rna/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/workflow/mip_rna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/workflow/mip_rna/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/cli/workflow/mutant/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/workflow/mutant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/workflow/mutant/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/cli/workflow/nextflow/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/workflow/nextflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/workflow/nextflow/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/cli/workflow/rnafusion/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/workflow/rnafusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12229 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/workflow/rnafusion/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/workflow/rnafusion/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/cli/workflow/taxprofiler/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/workflow/taxprofiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/workflow/taxprofiler/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/workflow/taxprofiler/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/cli/workflow/tower/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/workflow/tower/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-01 12:37:02.000000 cg-33.1.1/cg/cli/workflow/tower/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/constants/
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-01 12:37:02.000000 cg-33.1.1/cg/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-01 12:37:02.000000 cg-33.1.1/cg/constants/backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-01 12:37:02.000000 cg-33.1.1/cg/constants/bcl_convert_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-01 12:37:02.000000 cg-33.1.1/cg/constants/cgstats.py
--rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-06-01 12:37:02.000000 cg-33.1.1/cg/constants/compression.py
--rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-06-01 12:37:02.000000 cg-33.1.1/cg/constants/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-06-01 12:37:02.000000 cg-33.1.1/cg/constants/delivery.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-06-01 12:37:02.000000 cg-33.1.1/cg/constants/demultiplexing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-01 12:37:02.000000 cg-33.1.1/cg/constants/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-01 12:37:02.000000 cg-33.1.1/cg/constants/extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-01 12:37:02.000000 cg-33.1.1/cg/constants/gene_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-06-01 12:37:02.000000 cg-33.1.1/cg/constants/housekeeper_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-01 12:37:02.000000 cg-33.1.1/cg/constants/indexes.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-01 12:37:02.000000 cg-33.1.1/cg/constants/invoice.py
--rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-06-01 12:37:02.000000 cg-33.1.1/cg/constants/lims.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-01 12:37:02.000000 cg-33.1.1/cg/constants/nextflow.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-01 12:37:02.000000 cg-33.1.1/cg/constants/nipt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-06-01 12:37:02.000000 cg-33.1.1/cg/constants/observations.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-06-01 12:37:02.000000 cg-33.1.1/cg/constants/orderforms.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-01 12:37:02.000000 cg-33.1.1/cg/constants/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-01 12:37:02.000000 cg-33.1.1/cg/constants/pdc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-01 12:37:02.000000 cg-33.1.1/cg/constants/pedigree.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-01 12:37:02.000000 cg-33.1.1/cg/constants/priority.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-01 12:37:02.000000 cg-33.1.1/cg/constants/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-06-01 12:37:02.000000 cg-33.1.1/cg/constants/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-01 12:37:02.000000 cg-33.1.1/cg/constants/rnafusion.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-01 12:37:02.000000 cg-33.1.1/cg/constants/sample_sources.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-06-01 12:37:02.000000 cg-33.1.1/cg/constants/scout_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-01 12:37:02.000000 cg-33.1.1/cg/constants/sequencing.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-01 12:37:02.000000 cg-33.1.1/cg/constants/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-01 12:37:02.000000 cg-33.1.1/cg/constants/subject.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-01 12:37:02.000000 cg-33.1.1/cg/constants/symbols.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-01 12:37:02.000000 cg-33.1.1/cg/constants/taxprofiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-01 12:37:02.000000 cg-33.1.1/cg/constants/tb.py
--rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-06-01 12:37:02.000000 cg-33.1.1/cg/exc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/cg/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-01 12:37:02.000000 cg-33.1.1/cg/io/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-06-01 12:37:02.000000 cg-33.1.1/cg/io/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-01 12:37:02.000000 cg-33.1.1/cg/io/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-01 12:37:02.000000 cg-33.1.1/cg/io/json.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-01 12:37:02.000000 cg-33.1.1/cg/io/validate_path.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-01 12:37:02.000000 cg-33.1.1/cg/io/xml.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-01 12:37:02.000000 cg-33.1.1/cg/io/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/meta/archive/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8577 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/archive/ddn_dataflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/meta/backup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/backup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18893 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/backup/backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/backup/pdc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/meta/clean/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/clean/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/clean/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14404 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/clean/demultiplexed_flow_cells.py
--rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/clean/flow_cell_run_directories.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/meta/compress/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/compress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12476 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/compress/compress.py
--rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/compress/files.py
--rw-r--r--   0 runner    (1001) docker     (123)    13049 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/deliver.py
--rw-r--r--   0 runner    (1001) docker     (123)     8032 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/deliver_ticket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/meta/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/demultiplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/demultiplex/delete_demultiplex_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18178 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/demultiplex/demux_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/demultiplex/files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/meta/encryption/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/encryption/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10256 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/encryption/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)    10954 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/invoice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/meta/observations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/observations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/observations/balsamic_observations_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/observations/mip_dna_observations_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/observations/observations_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/meta/orders/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/orders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/orders/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/orders/balsamic_qc_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/orders/balsamic_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/orders/balsamic_umi_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)    15376 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/orders/case_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/orders/fastq_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/orders/fluffy_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/orders/lims.py
--rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/orders/metagenome_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/orders/microbial_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/orders/microsalt_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/orders/mip_dna_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/orders/mip_rna_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/orders/pool_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/orders/rml_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/orders/sars_cov_2_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/orders/submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/orders/ticket_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/meta/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10470 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/report/balsamic.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/report/balsamic_umi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/report/field_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     7274 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/report/mip_dna.py
--rw-r--r--   0 runner    (1001) docker     (123)    18537 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/report/report_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/report/rnafusion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/meta/report/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    78964 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/report/templates/balsamic_report.html
--rw-r--r--   0 runner    (1001) docker     (123)   151463 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/report/templates/bootstrap.html
--rw-r--r--   0 runner    (1001) docker     (123)    77831 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/report/templates/mip-dna_report.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/meta/rsync/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/rsync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12066 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/rsync/rsync_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/rsync/sbatch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/meta/tar/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/tar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/tar/tar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/meta/transfer/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/transfer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10070 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/transfer/external_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8417 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/transfer/flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/transfer/lims.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/meta/upload/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/upload/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/meta/upload/balsamic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/upload/balsamic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/upload/balsamic/balsamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/upload/coverage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/meta/upload/fohm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/upload/fohm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12140 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/upload/fohm/fohm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/meta/upload/gisaid/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/upload/gisaid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/upload/gisaid/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    13572 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/upload/gisaid/gisaid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/upload/gisaid/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/upload/gt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/meta/upload/mip/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/upload/mip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/upload/mip/mip_dna.py
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/upload/mip/mip_rna.py
--rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/upload/mutacc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/meta/upload/nipt/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/upload/nipt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/upload/nipt/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     7542 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/upload/nipt/nipt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/meta/upload/rnafusion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/upload/rnafusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/upload/rnafusion/rnafusion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/meta/upload/scout/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/upload/scout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/upload/scout/balsamic_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/upload/scout/balsamic_umi_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/upload/scout/hk_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/upload/scout/mip_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/upload/scout/rnafusion_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/upload/scout/scout_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    18719 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/upload/scout/uploadscoutapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/upload/upload_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/upload/vogue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/meta/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20004 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/workflow/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    26519 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/workflow/balsamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/workflow/balsamic_pon.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/workflow/balsamic_qc.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/workflow/balsamic_umi.py
--rw-r--r--   0 runner    (1001) docker     (123)    11670 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/workflow/fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)    13390 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/workflow/fluffy.py
--rw-r--r--   0 runner    (1001) docker     (123)    18121 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/workflow/microsalt.py
--rw-r--r--   0 runner    (1001) docker     (123)    14033 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/workflow/mip.py
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/workflow/mip_dna.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/workflow/mip_rna.py
--rw-r--r--   0 runner    (1001) docker     (123)    10762 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/workflow/mutant.py
--rw-r--r--   0 runner    (1001) docker     (123)    10236 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/workflow/nextflow_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/workflow/prepare_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)    18235 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/workflow/rnafusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/workflow/taxprofiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-06-01 12:37:02.000000 cg-33.1.1/cg/meta/workflow/tower_common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/models/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-01 12:37:02.000000 cg-33.1.1/cg/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-01 12:37:02.000000 cg-33.1.1/cg/models/analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/models/balsamic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/cg/models/balsamic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-01 12:37:02.000000 cg-33.1.1/cg/models/balsamic/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-06-01 12:37:02.000000 cg-33.1.1/cg/models/balsamic/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-01 12:37:02.000000 cg-33.1.1/cg/models/balsamic/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    13073 2023-06-01 12:37:02.000000 cg-33.1.1/cg/models/cg_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/models/cgstats/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/cg/models/cgstats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-01 12:37:02.000000 cg-33.1.1/cg/models/cgstats/flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-06-01 12:37:02.000000 cg-33.1.1/cg/models/cgstats/stats_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-06-01 12:37:02.000000 cg-33.1.1/cg/models/compression_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/models/deliverables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/cg/models/deliverables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-06-01 12:37:02.000000 cg-33.1.1/cg/models/deliverables/metric_deliverables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/models/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/cg/models/demultiplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10905 2023-06-01 12:37:02.000000 cg-33.1.1/cg/models/demultiplex/demux_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     8513 2023-06-01 12:37:02.000000 cg-33.1.1/cg/models/demultiplex/flow_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-06-01 12:37:02.000000 cg-33.1.1/cg/models/demultiplex/run_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-01 12:37:02.000000 cg-33.1.1/cg/models/demultiplex/sbatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-01 12:37:02.000000 cg-33.1.1/cg/models/email.py
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-06-01 12:37:02.000000 cg-33.1.1/cg/models/file_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/models/invoice/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/cg/models/invoice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-06-01 12:37:02.000000 cg-33.1.1/cg/models/invoice/invoice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/models/lims/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/cg/models/lims/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-06-01 12:37:02.000000 cg-33.1.1/cg/models/lims/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/models/mip/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/cg/models/mip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-01 12:37:02.000000 cg-33.1.1/cg/models/mip/mip_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-01 12:37:02.000000 cg-33.1.1/cg/models/mip/mip_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-06-01 12:37:02.000000 cg-33.1.1/cg/models/mip/mip_metrics_deliverables.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-06-01 12:37:02.000000 cg-33.1.1/cg/models/mip/mip_sample_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/models/nextflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/cg/models/nextflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-06-01 12:37:02.000000 cg-33.1.1/cg/models/nextflow/deliverables.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-01 12:37:02.000000 cg-33.1.1/cg/models/nextflow/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/models/observations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/cg/models/observations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-06-01 12:37:02.000000 cg-33.1.1/cg/models/observations/input_files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/models/orders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/cg/models/orders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-01 12:37:02.000000 cg-33.1.1/cg/models/orders/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6002 2023-06-01 12:37:02.000000 cg-33.1.1/cg/models/orders/excel_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-06-01 12:37:02.000000 cg-33.1.1/cg/models/orders/json_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-06-01 12:37:02.000000 cg-33.1.1/cg/models/orders/order.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-01 12:37:02.000000 cg-33.1.1/cg/models/orders/orderform_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-06-01 12:37:02.000000 cg-33.1.1/cg/models/orders/sample_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9856 2023-06-01 12:37:02.000000 cg-33.1.1/cg/models/orders/samples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/models/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/cg/models/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-06-01 12:37:02.000000 cg-33.1.1/cg/models/report/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-06-01 12:37:02.000000 cg-33.1.1/cg/models/report/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-06-01 12:37:02.000000 cg-33.1.1/cg/models/report/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-06-01 12:37:02.000000 cg-33.1.1/cg/models/report/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/models/rnafusion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/cg/models/rnafusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-01 12:37:02.000000 cg-33.1.1/cg/models/rnafusion/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-01 12:37:02.000000 cg-33.1.1/cg/models/rnafusion/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-01 12:37:02.000000 cg-33.1.1/cg/models/rnafusion/rnafusion_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/models/scout/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/cg/models/scout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-06-01 12:37:02.000000 cg-33.1.1/cg/models/scout/scout_load_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/models/slurm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/cg/models/slurm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-01 12:37:02.000000 cg-33.1.1/cg/models/slurm/sbatch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/models/taxprofiler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/cg/models/taxprofiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-01 12:37:02.000000 cg-33.1.1/cg/models/taxprofiler/taxprofiler_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/models/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/cg/models/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-01 12:37:02.000000 cg-33.1.1/cg/models/workflow/mutant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/resources/
--rw-r--r--   0 runner    (1001) docker     (123)    25590 2023-06-01 12:37:02.000000 cg-33.1.1/cg/resources/20181012_Indices.csv
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-01 12:37:02.000000 cg-33.1.1/cg/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-06-01 12:37:02.000000 cg-33.1.1/cg/resources/rnafusion_bundle_filenames.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/cg/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16940 2023-06-01 12:37:02.000000 cg-33.1.1/cg/server/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)    18031 2023-06-01 12:37:02.000000 cg-33.1.1/cg/server/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-06-01 12:37:02.000000 cg-33.1.1/cg/server/app.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-01 12:37:02.000000 cg-33.1.1/cg/server/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-06-01 12:37:02.000000 cg-33.1.1/cg/server/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-01 12:37:02.000000 cg-33.1.1/cg/server/ext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/server/invoices/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-01 12:37:02.000000 cg-33.1.1/cg/server/invoices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/server/invoices/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/server/invoices/templates/invoices/
--rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-06-01 12:37:02.000000 cg-33.1.1/cg/server/invoices/templates/invoices/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-06-01 12:37:02.000000 cg-33.1.1/cg/server/invoices/templates/invoices/invoice.html
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-06-01 12:37:02.000000 cg-33.1.1/cg/server/invoices/templates/invoices/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-06-01 12:37:02.000000 cg-33.1.1/cg/server/invoices/templates/invoices/new.html
--rw-r--r--   0 runner    (1001) docker     (123)     7794 2023-06-01 12:37:02.000000 cg-33.1.1/cg/server/invoices/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/server/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/server/templates/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-01 12:37:02.000000 cg-33.1.1/cg/server/templates/admin/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/store/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-01 12:37:02.000000 cg-33.1.1/cg/store/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/store/api/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-01 12:37:02.000000 cg-33.1.1/cg/store/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10616 2023-06-01 12:37:02.000000 cg-33.1.1/cg/store/api/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     6942 2023-06-01 12:37:02.000000 cg-33.1.1/cg/store/api/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-06-01 12:37:02.000000 cg-33.1.1/cg/store/api/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-06-01 12:37:02.000000 cg-33.1.1/cg/store/api/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-06-01 12:37:02.000000 cg-33.1.1/cg/store/api/find_basic_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    28994 2023-06-01 12:37:02.000000 cg-33.1.1/cg/store/api/find_business_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    38700 2023-06-01 12:37:02.000000 cg-33.1.1/cg/store/api/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/store/filters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/cg/store/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-06-01 12:37:02.000000 cg-33.1.1/cg/store/filters/status_analysis_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-06-01 12:37:02.000000 cg-33.1.1/cg/store/filters/status_application_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-06-01 12:37:02.000000 cg-33.1.1/cg/store/filters/status_application_version_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-01 12:37:02.000000 cg-33.1.1/cg/store/filters/status_bed_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-01 12:37:02.000000 cg-33.1.1/cg/store/filters/status_bed_version_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    10388 2023-06-01 12:37:02.000000 cg-33.1.1/cg/store/filters/status_case_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-01 12:37:02.000000 cg-33.1.1/cg/store/filters/status_case_sample_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-01 12:37:02.000000 cg-33.1.1/cg/store/filters/status_collaboration_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-06-01 12:37:02.000000 cg-33.1.1/cg/store/filters/status_customer_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-06-01 12:37:02.000000 cg-33.1.1/cg/store/filters/status_flow_cell_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-01 12:37:02.000000 cg-33.1.1/cg/store/filters/status_invoice_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-01 12:37:02.000000 cg-33.1.1/cg/store/filters/status_organism_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-01 12:37:02.000000 cg-33.1.1/cg/store/filters/status_panel_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-06-01 12:37:02.000000 cg-33.1.1/cg/store/filters/status_pool_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8892 2023-06-01 12:37:02.000000 cg-33.1.1/cg/store/filters/status_sample_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-01 12:37:02.000000 cg-33.1.1/cg/store/filters/status_user_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    29946 2023-06-01 12:37:02.000000 cg-33.1.1/cg/store/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-01 12:37:02.000000 cg-33.1.1/cg/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/utils/checksum/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/cg/utils/checksum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-01 12:37:02.000000 cg-33.1.1/cg/utils/checksum/checksum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/utils/click/
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-06-01 12:37:02.000000 cg-33.1.1/cg/utils/click/EnumChoice.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/cg/utils/click/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-06-01 12:37:02.000000 cg-33.1.1/cg/utils/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-06-01 12:37:02.000000 cg-33.1.1/cg/utils/date.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-01 12:37:02.000000 cg-33.1.1/cg/utils/dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-06-01 12:37:02.000000 cg-33.1.1/cg/utils/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-01 12:37:02.000000 cg-33.1.1/cg/utils/email.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-01 12:37:02.000000 cg-33.1.1/cg/utils/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-01 12:37:02.000000 cg-33.1.1/cg/utils/files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg/utils/flask/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/cg/utils/flask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-01 12:37:02.000000 cg-33.1.1/cg/utils/flask/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-01 12:37:02.000000 cg-33.1.1/cg/utils/time.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-01 12:37:02.000000 cg-33.1.1/cg/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/cg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-06-01 12:37:09.000000 cg-33.1.1/cg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    40973 2023-06-01 12:37:10.000000 cg-33.1.1/cg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 12:37:09.000000 cg-33.1.1/cg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-01 12:37:09.000000 cg-33.1.1/cg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 12:37:09.000000 cg-33.1.1/cg.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-01 12:37:09.000000 cg-33.1.1/cg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-01 12:37:09.000000 cg-33.1.1/cg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-01 12:37:02.000000 cg-33.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-01 12:37:02.000000 cg-33.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 12:37:10.000000 cg-33.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-01 12:37:02.000000 cg-33.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/apps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/apps/cgstats/
--rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-06-01 12:37:02.000000 cg-33.1.1/tests/apps/cgstats/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/apps/cgstats/crud/
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-06-01 12:37:02.000000 cg-33.1.1/tests/apps/cgstats/crud/test_create_novaseq.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-01 12:37:02.000000 cg-33.1.1/tests/apps/cgstats/crud/test_delete.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/apps/cgstats/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-01 12:37:02.000000 cg-33.1.1/tests/apps/cgstats/parsers/test_adapter_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-01 12:37:02.000000 cg-33.1.1/tests/apps/cgstats/parsers/test_conversion_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-01 12:37:02.000000 cg-33.1.1/tests/apps/cgstats/parsers/test_demux_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-01 12:37:02.000000 cg-33.1.1/tests/apps/cgstats/parsers/test_quality_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-01 12:37:02.000000 cg-33.1.1/tests/apps/cgstats/parsers/test_run_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-06-01 12:37:02.000000 cg-33.1.1/tests/apps/cgstats/test_cgstats_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-01 12:37:02.000000 cg-33.1.1/tests/apps/cgstats/test_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-01 12:37:02.000000 cg-33.1.1/tests/apps/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/apps/coverage/
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-01 12:37:02.000000 cg-33.1.1/tests/apps/coverage/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-06-01 12:37:02.000000 cg-33.1.1/tests/apps/coverage/test_coverage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/apps/crunchy/
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-06-01 12:37:02.000000 cg-33.1.1/tests/apps/crunchy/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-06-01 12:37:02.000000 cg-33.1.1/tests/apps/crunchy/test_compress_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-06-01 12:37:02.000000 cg-33.1.1/tests/apps/crunchy/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    14590 2023-06-01 12:37:02.000000 cg-33.1.1/tests/apps/crunchy/test_crunchy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9107 2023-06-01 12:37:02.000000 cg-33.1.1/tests/apps/crunchy/test_spring_decompression.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/apps/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/apps/demultiplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9961 2023-06-01 12:37:02.000000 cg-33.1.1/tests/apps/demultiplex/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-01 12:37:02.000000 cg-33.1.1/tests/apps/demultiplex/test_convert_to_sample_sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-01 12:37:02.000000 cg-33.1.1/tests/apps/demultiplex/test_demultiplex_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-06-01 12:37:02.000000 cg-33.1.1/tests/apps/demultiplex/test_sample_sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-06-01 12:37:02.000000 cg-33.1.1/tests/apps/demultiplex/test_validate_sample_sheet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/apps/gens/
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-06-01 12:37:02.000000 cg-33.1.1/tests/apps/gens/test_gens_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/apps/gt/
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-06-01 12:37:02.000000 cg-33.1.1/tests/apps/gt/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-06-01 12:37:02.000000 cg-33.1.1/tests/apps/gt/test_gt_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/apps/hk/
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-06-01 12:37:02.000000 cg-33.1.1/tests/apps/hk/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-01 12:37:02.000000 cg-33.1.1/tests/apps/hk/test__getattr__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-01 12:37:02.000000 cg-33.1.1/tests/apps/hk/test_add_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-06-01 12:37:02.000000 cg-33.1.1/tests/apps/hk/test_bundles.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-01 12:37:02.000000 cg-33.1.1/tests/apps/hk/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    24046 2023-06-01 12:37:02.000000 cg-33.1.1/tests/apps/hk/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-06-01 12:37:02.000000 cg-33.1.1/tests/apps/hk/test_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/apps/lims/
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-06-01 12:37:02.000000 cg-33.1.1/tests/apps/lims/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-06-01 12:37:02.000000 cg-33.1.1/tests/apps/lims/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-01 12:37:02.000000 cg-33.1.1/tests/apps/lims/test_sample_sheet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/apps/loqus/
--rw-r--r--   0 runner    (1001) docker     (123)     9785 2023-06-01 12:37:02.000000 cg-33.1.1/tests/apps/loqus/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-06-01 12:37:02.000000 cg-33.1.1/tests/apps/loqus/test_loqusdb_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/apps/madeline/
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-06-01 12:37:02.000000 cg-33.1.1/tests/apps/madeline/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-06-01 12:37:02.000000 cg-33.1.1/tests/apps/madeline/test_madeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/apps/mip/
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-06-01 12:37:02.000000 cg-33.1.1/tests/apps/mip/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-06-01 12:37:02.000000 cg-33.1.1/tests/apps/mip/test_config_mip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/apps/mutacc_auto/
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-01 12:37:02.000000 cg-33.1.1/tests/apps/mutacc_auto/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-06-01 12:37:02.000000 cg-33.1.1/tests/apps/mutacc_auto/test_mutacc_auto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/apps/orderform/
--rw-r--r--   0 runner    (1001) docker     (123)    11900 2023-06-01 12:37:02.000000 cg-33.1.1/tests/apps/orderform/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-06-01 12:37:02.000000 cg-33.1.1/tests/apps/orderform/test_excel_orderform_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-06-01 12:37:02.000000 cg-33.1.1/tests/apps/orderform/test_excel_sample_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-01 12:37:02.000000 cg-33.1.1/tests/apps/orderform/test_json_orderform_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-06-01 12:37:02.000000 cg-33.1.1/tests/apps/orderform/test_orderform_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/apps/scout/
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-06-01 12:37:02.000000 cg-33.1.1/tests/apps/scout/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-01 12:37:02.000000 cg-33.1.1/tests/apps/scout/test_get_causative_variants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-06-01 12:37:02.000000 cg-33.1.1/tests/apps/scout/test_get_scout_cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-06-01 12:37:02.000000 cg-33.1.1/tests/apps/scout/test_scout_load_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-06-01 12:37:02.000000 cg-33.1.1/tests/apps/scout/test_scout_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/apps/sequencing_metrics_parser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/apps/sequencing_metrics_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7152 2023-06-01 12:37:02.000000 cg-33.1.1/tests/apps/sequencing_metrics_parser/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/apps/sequencing_metrics_parser/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-06-01 12:37:02.000000 cg-33.1.1/tests/apps/sequencing_metrics_parser/parsers/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-01 12:37:02.000000 cg-33.1.1/tests/apps/sequencing_metrics_parser/parsers/test_bcl2fastq_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-06-01 12:37:02.000000 cg-33.1.1/tests/apps/sequencing_metrics_parser/parsers/test_bcl_convert_to_sequencing_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)    10062 2023-06-01 12:37:02.000000 cg-33.1.1/tests/apps/sequencing_metrics_parser/parsers/test_bclconvert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-01 12:37:02.000000 cg-33.1.1/tests/apps/sequencing_metrics_parser/test_sequencing_metrics_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/apps/slurm/
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-01 12:37:02.000000 cg-33.1.1/tests/apps/slurm/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-06-01 12:37:02.000000 cg-33.1.1/tests/apps/slurm/test_slurm_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-01 12:37:02.000000 cg-33.1.1/tests/apps/test_apps_environ.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-01 12:37:02.000000 cg-33.1.1/tests/apps/test_osticket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/apps/vogue/
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-01 12:37:02.000000 cg-33.1.1/tests/apps/vogue/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-06-01 12:37:02.000000 cg-33.1.1/tests/apps/vogue/test_vogue_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/cli/add/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/add/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/add/test_cli_add.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/add/test_cli_add_customer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/add/test_cli_add_family.py
--rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/add/test_cli_add_relationship.py
--rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/add/test_cli_add_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/cli/backup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/backup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/backup/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/backup/test_backup_command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/cli/clean/
--rw-r--r--   0 runner    (1001) docker     (123)     6069 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/clean/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/clean/test_balsamic_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/clean/test_clean_hk_bundle_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/clean/test_hk_bundle_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/clean/test_hk_case_bundle_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/clean/test_microbial_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/clean/test_rsync_past_run_dirs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/cli/compress/
--rw-r--r--   0 runner    (1001) docker     (123)    10311 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/compress/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6929 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/compress/test_cli_compress_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/compress/test_cli_decompress_spring.py
--rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/compress/test_compress_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/compress/test_store_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/cli/delete/
--rw-r--r--   0 runner    (1001) docker     (123)    12781 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/delete/test_cli_delete_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/delete/test_cli_delete_cases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/cli/deliver/
--rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/deliver/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/deliver/test_deliver_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/deliver/test_rsync_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8562 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/deliver/test_run_deliver_cmd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/cli/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/demultiplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11372 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/demultiplex/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/demultiplex/test_add_flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/demultiplex/test_create_sample_sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)    11412 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/demultiplex/test_demultiplex_flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/demultiplex/test_finish_demux.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/demultiplex/test_stats_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/demultiplex/test_validate_sample_sheet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/cli/generate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/generate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/cli/generate/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/generate/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/generate/report/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/generate/report/test_cli_delivery_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/generate/report/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/generate/test_cli_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/cli/get/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/get/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/get/test_cli_get.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/get/test_cli_get_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/get/test_cli_get_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/get/test_cli_get_flow_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     8862 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/get/test_cli_get_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/cli/set/
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/set/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7320 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/set/test_cli_set_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/set/test_cli_set_cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/set/test_cli_set_flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/set/test_cli_set_list_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)    12516 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/set/test_cli_set_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/set/test_cli_set_samples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/cli/store/
--rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/store/test_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/test_clean.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/cli/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/cli/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/cli/tests/fixtures/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/tests/fixtures/data/fastq.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/cli/upload/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/upload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10414 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/upload/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/upload/test_cli_scout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/upload/test_cli_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/upload/test_cli_upload_auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/upload/test_cli_upload_delivery_report.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/upload/test_cli_upload_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/upload/test_cli_upload_genotype.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/upload/test_cli_upload_gens.py
--rw-r--r--   0 runner    (1001) docker     (123)     9971 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/upload/test_cli_upload_nipt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/upload/test_cli_upload_nipt_ftp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/upload/test_cli_upload_nipt_statina.py
--rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/upload/test_cli_upload_observations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/upload/test_cli_upload_vogue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/cli/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/workflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/cli/workflow/balsamic/
--rw-r--r--   0 runner    (1001) docker     (123)    30801 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/workflow/balsamic/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    15328 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/workflow/balsamic/test_compound_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/workflow/balsamic/test_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/workflow/balsamic/test_report_deliver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/workflow/balsamic/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/workflow/balsamic/test_store_housekeeper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/workflow/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/cli/workflow/fastq/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/workflow/fastq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/workflow/fastq/test_fastq_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/cli/workflow/fluffy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/workflow/fluffy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/workflow/fluffy/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/workflow/fluffy/test_cli_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/workflow/fluffy/test_cli_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/workflow/fluffy/test_cli_start.py
--rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/workflow/fluffy/test_cli_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/cli/workflow/microsalt/
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/workflow/microsalt/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/cli/workflow/microsalt/snapshots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/workflow/microsalt/snapshots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/workflow/microsalt/snapshots/snap_test_microsalt_case_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7185 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/workflow/microsalt/test_microsalt_case_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/workflow/microsalt/test_microsalt_run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/cli/workflow/mip/
--rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/workflow/mip/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6796 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/workflow/mip/test_cli_mip_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/workflow/mip/test_cli_mip_dna_link.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/workflow/mip/test_cli_mip_dna_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/workflow/mip/test_cli_mip_dna_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/workflow/mip/test_cli_mip_dna_start.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/workflow/mip/test_cli_mip_rna_link.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/workflow/mip/test_cli_mip_rna_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     8558 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/workflow/mip/test_cli_mip_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/cli/workflow/rnafusion/
--rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/workflow/rnafusion/test_cli_rnafusion_compound_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/workflow/rnafusion/test_cli_rnafusion_config_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/workflow/rnafusion/test_cli_rnafusion_metrics_deliver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/workflow/rnafusion/test_cli_rnafusion_report_deliver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/workflow/rnafusion/test_cli_rnafusion_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     8449 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/workflow/rnafusion/test_cli_rnafusion_store_housekeeper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/cli/workflow/taxprofiler/
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/workflow/taxprofiler/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/workflow/taxprofiler/test_cli_taxprofiler_compound_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/workflow/taxprofiler/test_cli_taxprofiler_config_case.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/workflow/test_cli_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-06-01 12:37:02.000000 cg-33.1.1/tests/cli/workflow/test_cli_workflow_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)    71693 2023-06-01 12:37:02.000000 cg-33.1.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/fixtures/DEMUX/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/ADM1136A3_XTC08_AGTGGTCA_L001_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/ADM1136A3_XTC08_AGTGGTCA_L001_R2_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/ADM1136A3_XTC08_AGTGGTCA_L002_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/ADM1136A3_XTC08_AGTGGTCA_L002_R2_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/runParameters.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/fixtures/analysis/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/fixtures/analysis/balsamic/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/fixtures/analysis/balsamic/tn_wgs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/analysis/balsamic/tn_wgs/adm1.cram
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/analysis/balsamic/tn_wgs/ascat.output.pdf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/analysis/balsamic/tn_wgs/snv.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/analysis/balsamic/tn_wgs/sv.vcf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/fixtures/analysis/microsalt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/
--rw-r--r--   0 runner    (1001) docker     (123)    14644 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/
--rw-r--r--   0 runner    (1001) docker     (123)    15713 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/fixtures/analysis/mip/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/fixtures/analysis/mip/dna/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/analysis/mip/dna/ADM1.baf.bed.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/analysis/mip/dna/ADM1.cov.bed.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/analysis/mip/dna/ADM2.cram
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/analysis/mip/dna/ADM3.cram
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/analysis/mip/dna/adm1.cram
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/analysis/mip/dna/adm1.mt.bam
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/analysis/mip/dna/multiqc.html
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/analysis/mip/dna/report.pdf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/analysis/mip/dna/smn.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/analysis/mip/dna/snv.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/analysis/mip/dna/snv_research.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/analysis/mip/dna/str.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/analysis/mip/dna/sv.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/analysis/mip/dna/sv_research.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/analysis/mip/dna/vcf2cytosure.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/fixtures/analysis/rnafusion/
--rw-r--r--   0 runner    (1001) docker     (123)     5587 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/analysis/rnafusion/multiqc_data.json
--rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/analysis/sample_coverage.bed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/fixtures/apps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/fixtures/apps/balsamic/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/fixtures/apps/balsamic/case/
--rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/balsamic/case/config.json
--rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/balsamic/case/metadata.yml
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/balsamic/case/metadata_directory.yml
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/balsamic/case/metadata_file_tags.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/fixtures/apps/crunchy/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/crunchy/spring_metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/fixtures/apps/demultiplexing/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml
--rw-r--r--   0 runner    (1001) docker     (123)    53877 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/demultiplexing/RunParameters_different_index_cycles.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/demultiplexing/SampleSheetS2_Bcl2Fastq.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/demultiplexing/SampleSheetS2_Dragen.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/
--rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/Adapter_Metrics.csv
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/Quality_Metrics.csv
--rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/RunInfo.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/dummy_run_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/dummy_run_R1_001.fastq.gz.md5
--rw-r--r--   0 runner    (1001) docker     (123)   338370 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R1_001.fastq.gz.md5
--rw-r--r--   0 runner    (1001) docker     (123)   338349 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R2_001.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R2_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R2_001.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/fixtures/apps/demultiplexing/flow-cell-runs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/CopyComplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/RTAComplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/demuxstarted.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/CopyComplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stderr
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/RTAComplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/demuxstarted.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/fixtures/apps/demultiplexing/hiseq_run/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/fixtures/apps/demultiplexing/hiseq_run/201203_A00689_0200_AHVKJCDRXX/
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/demultiplexing/hiseq_run/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/demultiplexing/hiseq_run/201203_A00689_0200_AHVKJCDRXX/RTAComplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/demultiplexing/hiseq_run/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/demultiplexing/hiseq_run/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/demultiplexing/hiseq_run/201203_A00689_0200_AHVKJCDRXX/copycomplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/demultiplexing/hiseq_run/201203_A00689_0200_AHVKJCDRXX/demuxstarted.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/demultiplexing/hiseq_run/runParameters.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/fixtures/apps/demultiplexing/raw_lims_samples/
--rw-r--r--   0 runner    (1001) docker     (123)    92887 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/demultiplexing/raw_lims_samples/raw_samplesheet_novaseq.json
--rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/demultiplexing/runParameters_missing_flowcell_run_field.xml
--rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/demultiplexing/unknown_run_parameters.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/fixtures/apps/fluffy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/fixtures/apps/fluffy/2020-23219-05/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/fluffy/2020-23219-05/2020-23219-05.WCXpredict_aberrations.filt.bed
--rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/fluffy/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/fluffy/deliverables.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/fluffy/fluffy_fastq.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/fluffy/multiqc_report.html
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/fluffy/summary.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/fixtures/apps/gt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/gt/yellowhog.bcf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/fixtures/apps/madeline/
--rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/madeline/madeline.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/fixtures/apps/mip/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/mip/case_file.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/mip/case_metrics_deliverables.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/fixtures/apps/mip/dna/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/fixtures/apps/mip/dna/store/
--rw-r--r--   0 runner    (1001) docker     (123)    21811 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/mip/dna/store/case_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    23364 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    37367 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/mip/dna/store/empty_case_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/mip/dna/store/empty_case_metrics_deliverables.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/mip/dna/store/empty_case_qc_sample_info.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/mip/dna/store/empty_delivery_report.html
--rw-r--r--   0 runner    (1001) docker     (123)    62741 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/fixtures/apps/mip/rna/
--rw-r--r--   0 runner    (1001) docker     (123)    11242 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/mip/rna/case_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    12164 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/fixtures/apps/mip/rna/store/
--rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/mip/rna/store/bundle_data.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/mip/rna/store/case_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/mip/sample_file.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/fixtures/apps/scout/
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/scout/643594.config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/scout/case_export.json
--rw-r--r--   0 runner    (1001) docker     (123)     9349 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/scout/export_causatives.json
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/scout/none_case_export.json
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/scout/other_sex_case.json
--rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/scout/panel_export.bed
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/scout/panel_export.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/fixtures/apps/sequencing_metrics_parser/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/fixtures/apps/sequencing_metrics_parser/Unaligned/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/fixtures/apps/sequencing_metrics_parser/Unaligned/Reports/
--rw-r--r--   0 runner    (1001) docker     (123)    63569 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/sequencing_metrics_parser/Unaligned/Reports/Adapter_Metrics.csv
--rw-r--r--   0 runner    (1001) docker     (123)    42478 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/sequencing_metrics_parser/Unaligned/Reports/Demultiplex_Stats.csv
--rw-r--r--   0 runner    (1001) docker     (123)    69862 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/sequencing_metrics_parser/Unaligned/Reports/Quality_Metrics.csv
--rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/sequencing_metrics_parser/Unaligned/Reports/RunInfo.xml
--rw-r--r--   0 runner    (1001) docker     (123)    42872 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/sequencing_metrics_parser/Unaligned/Reports/SampleSheet.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/fixtures/apps/shipping/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/apps/shipping/scout-deploy.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/fixtures/cgweb_orders/
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/cgweb_orders/balsamic.json
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/cgweb_orders/fastq.json
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/cgweb_orders/metagenome.json
--rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/cgweb_orders/microsalt.json
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/cgweb_orders/mip.json
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/cgweb_orders/mip_rna.json
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/cgweb_orders/rml.json
--rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/cgweb_orders/sarscov2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/fixtures/data/
--rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/data/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)   258048 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/data/cgfixture.db
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/data/fastq.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)    49152 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/data/hkstore.db
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/fixtures/data/yellowhog/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/data/yellowhog/pedigree.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/fixtures/io/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/io/example_csv.csv
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/io/example_json.json
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/io/example_xml.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/fixtures/orderforms/
--rw-r--r--   0 runner    (1001) docker     (123)   257271 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/orderforms/1508.27.balsamic.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   256694 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/orderforms/1508.27.balsamic_qc.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   257319 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/orderforms/1508.27.balsamic_umi.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   256733 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/orderforms/1508.27.fastq.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   257317 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/orderforms/1508.27.mip.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   257230 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/orderforms/1508.27.mip_rna.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    95490 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/orderforms/1603.11.microbial.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   158941 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/orderforms/1604.15.rml.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    88438 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/orderforms/1605.10.metagenome.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   228196 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/orderforms/2184.7.sarscov2.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    18639 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/orderforms/NIPT-json.json
--rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json
--rw-r--r--   0 runner    (1001) docker     (123)     6611 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/orderforms/mip_uploaded_json_orderform.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/fixtures/report/
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/report/case_data.json
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/report/lims_exported_samples.json
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-01 12:37:02.000000 cg-33.1.1/tests/fixtures/report/lims_family.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/io/
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-06-01 12:37:02.000000 cg-33.1.1/tests/io/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7766 2023-06-01 12:37:02.000000 cg-33.1.1/tests/io/test_io_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-06-01 12:37:02.000000 cg-33.1.1/tests/io/test_io_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-06-01 12:37:02.000000 cg-33.1.1/tests/io/test_io_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-01 12:37:02.000000 cg-33.1.1/tests/io/test_io_xml.py
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-06-01 12:37:02.000000 cg-33.1.1/tests/io/test_io_yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-06-01 12:37:02.000000 cg-33.1.1/tests/io/test_validate_path.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/meta/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/meta/archive/
--rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/archive/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    12864 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/archive/test_archiving.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/meta/backup/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/backup/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    24493 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/backup/test_meta_backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/backup/test_meta_pdc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/meta/clean/
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/clean/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/clean/test_clean_demultiplexed_runs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/clean/test_clean_flow_cell_run_directories.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/meta/compress/
--rw-r--r--   0 runner    (1001) docker     (123)     7793 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/compress/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7115 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/compress/test_clean_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/compress/test_compress_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/compress/test_compress_meta_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/compress/test_decompress_spring_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/compress/test_meta_compress_update_hk.py
--rw-r--r--   0 runner    (1001) docker     (123)     9965 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/meta/deliver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/deliver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/deliver/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/deliver/test_deliver_ticket.py
--rw-r--r--   0 runner    (1001) docker     (123)    10178 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/deliver/test_delivery_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/meta/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)    12217 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/demultiplex/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    13452 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/demultiplex/test_delete_demultiplex_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    15635 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/demultiplex/test_demux_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/demultiplex/test_rename_files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/meta/demultiplex/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/meta/demultiplex/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/meta/demultiplex/tests/fixtures/apps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/meta/demultiplex/tests/fixtures/apps/demultiplexing/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/meta/demultiplex/tests/fixtures/apps/demultiplexing/flow-cell-runs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/meta/demultiplex/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/demultiplex/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/copycomplete.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/meta/encryption/
--rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/encryption/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    11132 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/encryption/test_encryption.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/meta/observations/
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/observations/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    16497 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/observations/test_meta_upload_observations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/meta/orders/
--rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/orders/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/orders/test_PoolSubmitter_validate_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/orders/test_SarsCov2Submitter_store_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/orders/test_SarsCov2Submitter_validate_order.py
--rw-r--r--   0 runner    (1001) docker     (123)    19748 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/orders/test_meta_orders_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7123 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/orders/test_meta_orders_lims.py
--rw-r--r--   0 runner    (1001) docker     (123)    29658 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/orders/test_meta_orders_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/orders/test_ticket_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/meta/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/report/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/report/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/report/test_balsamic_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/report/test_field_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/report/test_mip_dna_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13311 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/report/test_report_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/report/test_rnafusion_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/meta/rsync/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/rsync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/rsync/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8811 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/rsync/test_rsync.py
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/test_invoice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/meta/transfer/
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/transfer/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    10019 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/transfer/test_external_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    16507 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/transfer/test_meta_transfer_flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/transfer/test_meta_transfer_lims.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/meta/upload/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/upload/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/meta/upload/balsamic/
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/upload/balsamic/test_balsamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/upload/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/meta/upload/gisaid/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/upload/gisaid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/meta/upload/gisaid/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/upload/gisaid/fixtures/four_samples.csv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/upload/gisaid/fixtures/invalid_housekeeper.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/upload/gisaid/fixtures/valid_gisaid.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/upload/gisaid/fixtures/valid_housekeeper.fasta
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/meta/upload/mutacc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/upload/mutacc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/upload/mutacc/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/upload/mutacc/test_meta_upload_mutacc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/meta/upload/nipt/
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/upload/nipt/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/upload/nipt/test_nipt_upload_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/meta/upload/scout/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/upload/scout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23429 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/upload/scout/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/upload/scout/test_generate_load_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/upload/scout/test_meta_upload_scoutapi.py
--rw-r--r--   0 runner    (1001) docker     (123)    32141 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py
--rw-r--r--   0 runner    (1001) docker     (123)     7857 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/upload/scout/test_scout_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/upload/test_meta_upload_coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/upload/test_upload_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/upload/test_upload_genotypes_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/meta/upload/vogue/
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/upload/vogue/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/upload/vogue/test_upload_vogue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/meta/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7681 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/workflow/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/workflow/test_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/workflow/test_balsamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/workflow/test_microsalt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/workflow/test_prepare_fastq_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-06-01 12:37:02.000000 cg-33.1.1/tests/meta/workflow/test_rnafusion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/mocks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-06-01 12:37:02.000000 cg-33.1.1/tests/mocks/balsamic_analysis_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-06-01 12:37:02.000000 cg-33.1.1/tests/mocks/crunchy.py
--rw-r--r--   0 runner    (1001) docker     (123)    20596 2023-06-01 12:37:02.000000 cg-33.1.1/tests/mocks/hk_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-06-01 12:37:02.000000 cg-33.1.1/tests/mocks/limsmock.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-01 12:37:02.000000 cg-33.1.1/tests/mocks/madeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-06-01 12:37:02.000000 cg-33.1.1/tests/mocks/mip_analysis_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-06-01 12:37:02.000000 cg-33.1.1/tests/mocks/osticket.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-06-01 12:37:02.000000 cg-33.1.1/tests/mocks/process_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-06-01 12:37:02.000000 cg-33.1.1/tests/mocks/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-06-01 12:37:02.000000 cg-33.1.1/tests/mocks/scout.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-01 12:37:02.000000 cg-33.1.1/tests/mocks/store_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-01 12:37:02.000000 cg-33.1.1/tests/mocks/tb_mock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/models/balsamic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/models/balsamic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-01 12:37:02.000000 cg-33.1.1/tests/models/balsamic/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-01 12:37:02.000000 cg-33.1.1/tests/models/balsamic/test_balsamic_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-01 12:37:02.000000 cg-33.1.1/tests/models/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/models/demultiplexing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/models/demultiplexing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-01 12:37:02.000000 cg-33.1.1/tests/models/demultiplexing/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-01 12:37:02.000000 cg-33.1.1/tests/models/demultiplexing/test_demux_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-06-01 12:37:02.000000 cg-33.1.1/tests/models/demultiplexing/test_flowcell_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4894 2023-06-01 12:37:02.000000 cg-33.1.1/tests/models/demultiplexing/test_run_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/models/mip/
--rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-06-01 12:37:02.000000 cg-33.1.1/tests/models/mip/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-06-01 12:37:02.000000 cg-33.1.1/tests/models/mip/test_mip_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-06-01 12:37:02.000000 cg-33.1.1/tests/models/mip/test_mip_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-06-01 12:37:02.000000 cg-33.1.1/tests/models/mip/test_mip_metrics_deliverables.py
--rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-06-01 12:37:02.000000 cg-33.1.1/tests/models/mip/test_mip_sample_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/models/nextflow/
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-01 12:37:02.000000 cg-33.1.1/tests/models/nextflow/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-01 12:37:02.000000 cg-33.1.1/tests/models/nextflow/test_nextflow_deliver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/models/observations/
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-01 12:37:02.000000 cg-33.1.1/tests/models/observations/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-06-01 12:37:02.000000 cg-33.1.1/tests/models/observations/test_observations_input_files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/models/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/models/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5459 2023-06-01 12:37:02.000000 cg-33.1.1/tests/models/report/test_validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/models/rnafusion/
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-06-01 12:37:02.000000 cg-33.1.1/tests/models/rnafusion/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-06-01 12:37:02.000000 cg-33.1.1/tests/models/rnafusion/test_rnafusion_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-06-01 12:37:02.000000 cg-33.1.1/tests/models/test_cg_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-01 12:37:02.000000 cg-33.1.1/tests/models/test_compression_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-06-01 12:37:02.000000 cg-33.1.1/tests/models/test_file_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-01 12:37:02.000000 cg-33.1.1/tests/models/test_flowcell_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/server/
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-01 12:37:02.000000 cg-33.1.1/tests/server/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-01 12:37:02.000000 cg-33.1.1/tests/server/test_server_app.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-01 12:37:02.000000 cg-33.1.1/tests/server/test_server_auto.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-01 12:37:02.000000 cg-33.1.1/tests/small_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/store/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/store/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/store/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/store/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/store/api/add/
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-06-01 12:37:02.000000 cg-33.1.1/tests/store/api/add/test_store_add_application_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-06-01 12:37:02.000000 cg-33.1.1/tests/store/api/add/test_store_add_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-06-01 12:37:02.000000 cg-33.1.1/tests/store/api/add/test_store_add_customer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-06-01 12:37:02.000000 cg-33.1.1/tests/store/api/add/test_store_add_flow_celll.py
--rw-r--r--   0 runner    (1001) docker     (123)    17674 2023-06-01 12:37:02.000000 cg-33.1.1/tests/store/api/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/store/api/delete/
--rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-06-01 12:37:02.000000 cg-33.1.1/tests/store/api/delete/test_store_api_delete.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/store/api/find/
--rw-r--r--   0 runner    (1001) docker     (123)     8342 2023-06-01 12:37:02.000000 cg-33.1.1/tests/store/api/find/test_find_basic_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-06-01 12:37:02.000000 cg-33.1.1/tests/store/api/find/test_find_basic_data_application_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    27415 2023-06-01 12:37:02.000000 cg-33.1.1/tests/store/api/find/test_find_business_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-06-01 12:37:02.000000 cg-33.1.1/tests/store/api/find/test_find_business_data_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-06-01 12:37:02.000000 cg-33.1.1/tests/store/api/find/test_find_business_data_case.py
--rw-r--r--   0 runner    (1001) docker     (123)    12223 2023-06-01 12:37:02.000000 cg-33.1.1/tests/store/api/find/test_find_business_data_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/store/api/status/
--rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-06-01 12:37:02.000000 cg-33.1.1/tests/store/api/status/test_analyses_to_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-06-01 12:37:02.000000 cg-33.1.1/tests/store/api/status/test_analyses_to_delivery_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     9780 2023-06-01 12:37:02.000000 cg-33.1.1/tests/store/api/status/test_store_api_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    15265 2023-06-01 12:37:02.000000 cg-33.1.1/tests/store/api/status/test_store_api_status_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    54170 2023-06-01 12:37:02.000000 cg-33.1.1/tests/store/api/status/test_store_api_status_cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-01 12:37:02.000000 cg-33.1.1/tests/store/api/status/test_store_api_status_customer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-01 12:37:02.000000 cg-33.1.1/tests/store/api/status/test_store_api_status_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     8763 2023-06-01 12:37:02.000000 cg-33.1.1/tests/store/api/status/test_store_api_status_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-06-01 12:37:02.000000 cg-33.1.1/tests/store/api/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15566 2023-06-01 12:37:02.000000 cg-33.1.1/tests/store/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/store/filters/
--rw-r--r--   0 runner    (1001) docker     (123)    14547 2023-06-01 12:37:02.000000 cg-33.1.1/tests/store/filters/test_status_analyses_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-06-01 12:37:02.000000 cg-33.1.1/tests/store/filters/test_status_application_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    10505 2023-06-01 12:37:02.000000 cg-33.1.1/tests/store/filters/test_status_application_version_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-06-01 12:37:02.000000 cg-33.1.1/tests/store/filters/test_status_bed_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-01 12:37:02.000000 cg-33.1.1/tests/store/filters/test_status_bed_version_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-06-01 12:37:02.000000 cg-33.1.1/tests/store/filters/test_status_case_sample_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    38171 2023-06-01 12:37:02.000000 cg-33.1.1/tests/store/filters/test_status_cases_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-01 12:37:02.000000 cg-33.1.1/tests/store/filters/test_status_collaboration_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-06-01 12:37:02.000000 cg-33.1.1/tests/store/filters/test_status_customer_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-06-01 12:37:02.000000 cg-33.1.1/tests/store/filters/test_status_flow_cell_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-06-01 12:37:02.000000 cg-33.1.1/tests/store/filters/test_status_invoice_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-06-01 12:37:02.000000 cg-33.1.1/tests/store/filters/test_status_organism_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-06-01 12:37:02.000000 cg-33.1.1/tests/store/filters/test_status_panel_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-06-01 12:37:02.000000 cg-33.1.1/tests/store/filters/test_status_pool_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    22968 2023-06-01 12:37:02.000000 cg-33.1.1/tests/store/filters/test_status_samples_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-01 12:37:02.000000 cg-33.1.1/tests/store/filters/test_status_user_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-06-01 12:37:02.000000 cg-33.1.1/tests/store/test_delivery.py
--rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-06-01 12:37:02.000000 cg-33.1.1/tests/store/test_store_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    29888 2023-06-01 12:37:02.000000 cg-33.1.1/tests/store_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-01 12:37:02.000000 cg-33.1.1/tests/test_store_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/tests/fixtures/apps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/tests/fixtures/apps/demultiplexing/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/tests/fixtures/apps/demultiplexing/flowcell-runs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/copycomplete.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/tests/fixtures/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/tests/fixtures/data/fastq.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:10.000000 cg-33.1.1/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:37:02.000000 cg-33.1.1/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-01 12:37:02.000000 cg-33.1.1/tests/utils/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-06-01 12:37:02.000000 cg-33.1.1/tests/utils/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-01 12:37:02.000000 cg-33.1.1/tests/utils/test_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-01 12:37:02.000000 cg-33.1.1/tests/utils/test_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     7176 2023-06-01 12:37:02.000000 cg-33.1.1/tests/utils/test_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-06-01 12:37:02.000000 cg-33.1.1/tests/utils/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-01 13:39:13.000000 cg-33.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-06-01 13:39:27.000000 cg-33.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-06-01 13:39:13.000000 cg-33.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-01 13:39:13.000000 cg-33.1.2/cg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/apps/cgstats/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/cgstats/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/apps/cgstats/crud/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/cgstats/crud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16023 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/cgstats/crud/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/cgstats/crud/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7927 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/cgstats/crud/find.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/apps/cgstats/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/cgstats/db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/apps/cgstats/db/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/cgstats/db/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/cgstats/db/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/cgstats/db/models/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/cgstats/db/models/demux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/cgstats/db/models/demux_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/cgstats/db/models/dragen_demux_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/cgstats/db/models/flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/cgstats/db/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/cgstats/db/models/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/cgstats/db/models/support_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/cgstats/db/models/unaligned.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/cgstats/db/models/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/apps/cgstats/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/cgstats/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/cgstats/parsers/adapter_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11317 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/cgstats/parsers/conversion_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/cgstats/parsers/demux_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/cgstats/parsers/dragen_demultiplexing_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/cgstats/parsers/quality_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/cgstats/parsers/run_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6315 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/cgstats/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/apps/coverage/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/coverage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/coverage/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/apps/crunchy/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/crunchy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12884 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/crunchy/crunchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/crunchy/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/crunchy/sbatch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/apps/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/demultiplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11469 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/demultiplex/demultiplex_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/demultiplex/demux_report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/apps/demultiplex/sample_sheet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/demultiplex/sample_sheet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/demultiplex/sample_sheet/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/demultiplex/sample_sheet/dummy_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/demultiplex/sample_sheet/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/demultiplex/sample_sheet/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/demultiplex/sample_sheet/novaseq_sample_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/demultiplex/sample_sheet/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/demultiplex/sbatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/environ.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/gens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/gt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/apps/hermes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/hermes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/hermes/hermes_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/hermes/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/apps/housekeeper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/housekeeper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17304 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/housekeeper/hk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/housekeeper/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/apps/invoice/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/invoice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/invoice/render.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/apps/invoice/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)   113439 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/invoice/templates/KI_pool_invoice.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    81032 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/invoice/templates/KI_sample_invoice.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   113363 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/invoice/templates/KTH_pool_invoice.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    80886 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/invoice/templates/KTH_sample_invoice.xlsx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/apps/lims/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/lims/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16393 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/lims/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/lims/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8243 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/lims/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/lims/sample_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/loqus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/apps/madeline/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/madeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/madeline/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/apps/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/mip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/mip/confighandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/mutacc_auto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/apps/orderform/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/orderform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9233 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/orderform/excel_orderform_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/orderform/json_orderform_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6387 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/orderform/orderform_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/osticket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/apps/scout/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/scout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/scout/scout_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9438 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/scout/scoutapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/apps/sequencing_metrics_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/sequencing_metrics_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/sequencing_metrics_parser/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/apps/sequencing_metrics_parser/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/sequencing_metrics_parser/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/sequencing_metrics_parser/models/bcl2fastq_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/sequencing_metrics_parser/models/bcl_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/apps/sequencing_metrics_parser/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/sequencing_metrics_parser/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5659 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/sequencing_metrics_parser/parsers/bcl2fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/sequencing_metrics_parser/parsers/bcl2fastq_to_sequencing_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8990 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/sequencing_metrics_parser/parsers/bcl_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/sequencing_metrics_parser/parsers/bcl_convert_to_sequencing_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/sequencing_metrics_parser/sequencing_metrics_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/apps/slurm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/slurm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/slurm/sbatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/slurm/slurm_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/apps/tb/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/tb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7646 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/tb/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/tb/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-06-01 13:39:13.000000 cg-33.1.2/cg/apps/vogue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10329 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7057 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19665 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/clean.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/cli/compress/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/compress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/compress/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/compress/fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8507 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/compress/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/cli/delete/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/delete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/delete/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/delete/case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/delete/cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/delete/observations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/cli/deliver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/deliver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/deliver/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/cli/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/demultiplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/demultiplex/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/demultiplex/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/demultiplex/demux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/demultiplex/finish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/demultiplex/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/demultiplex/sample_sheet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/cli/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/generate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/generate/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/cli/generate/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/generate/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/generate/report/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/generate/report/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/generate/report/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8386 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/cli/set/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/set/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/set/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/set/case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/set/cases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/cli/store/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/store/fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/store/store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/transfer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/cli/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/upload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/upload/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/upload/clinical_delivery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/upload/coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/upload/delivery_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/upload/fohm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/upload/genotype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/upload/gens.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/upload/gisaid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/upload/mutacc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/cli/upload/nipt/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/upload/nipt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/upload/nipt/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/upload/nipt/ftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/upload/nipt/statina.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/cli/upload/observations/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/upload/observations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/upload/observations/observations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/upload/observations/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9563 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/upload/scout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/upload/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/upload/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11932 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/upload/vogue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/cli/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/workflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/cli/workflow/balsamic/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/workflow/balsamic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8860 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/workflow/balsamic/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/workflow/balsamic/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/workflow/balsamic/pon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/workflow/balsamic/qc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/workflow/balsamic/umi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/workflow/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12622 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/workflow/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/cli/workflow/fastq/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/workflow/fastq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/workflow/fastq/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/cli/workflow/fluffy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/workflow/fluffy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/workflow/fluffy/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/cli/workflow/microsalt/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/workflow/microsalt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11101 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/workflow/microsalt/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/cli/workflow/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/workflow/mip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/workflow/mip/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/workflow/mip/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/cli/workflow/mip_dna/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/workflow/mip_dna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/workflow/mip_dna/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/cli/workflow/mip_rna/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/workflow/mip_rna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/workflow/mip_rna/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/cli/workflow/mutant/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/workflow/mutant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/workflow/mutant/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/cli/workflow/nextflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/workflow/nextflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/workflow/nextflow/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/cli/workflow/rnafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/workflow/rnafusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12229 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/workflow/rnafusion/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/workflow/rnafusion/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/cli/workflow/taxprofiler/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/workflow/taxprofiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/workflow/taxprofiler/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/workflow/taxprofiler/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/cli/workflow/tower/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/workflow/tower/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-01 13:39:13.000000 cg-33.1.2/cg/cli/workflow/tower/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/constants/
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-01 13:39:13.000000 cg-33.1.2/cg/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-01 13:39:13.000000 cg-33.1.2/cg/constants/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-01 13:39:13.000000 cg-33.1.2/cg/constants/bcl_convert_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-01 13:39:13.000000 cg-33.1.2/cg/constants/cgstats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-06-01 13:39:13.000000 cg-33.1.2/cg/constants/compression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-06-01 13:39:13.000000 cg-33.1.2/cg/constants/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-06-01 13:39:13.000000 cg-33.1.2/cg/constants/delivery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-06-01 13:39:13.000000 cg-33.1.2/cg/constants/demultiplexing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-01 13:39:13.000000 cg-33.1.2/cg/constants/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-01 13:39:13.000000 cg-33.1.2/cg/constants/extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-01 13:39:13.000000 cg-33.1.2/cg/constants/gene_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-06-01 13:39:13.000000 cg-33.1.2/cg/constants/housekeeper_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-01 13:39:13.000000 cg-33.1.2/cg/constants/indexes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-01 13:39:13.000000 cg-33.1.2/cg/constants/invoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-06-01 13:39:13.000000 cg-33.1.2/cg/constants/lims.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-01 13:39:13.000000 cg-33.1.2/cg/constants/nextflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-01 13:39:13.000000 cg-33.1.2/cg/constants/nipt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-06-01 13:39:13.000000 cg-33.1.2/cg/constants/observations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-06-01 13:39:13.000000 cg-33.1.2/cg/constants/orderforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-01 13:39:13.000000 cg-33.1.2/cg/constants/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-01 13:39:13.000000 cg-33.1.2/cg/constants/pdc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-01 13:39:13.000000 cg-33.1.2/cg/constants/pedigree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-01 13:39:13.000000 cg-33.1.2/cg/constants/priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-01 13:39:13.000000 cg-33.1.2/cg/constants/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-06-01 13:39:13.000000 cg-33.1.2/cg/constants/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-01 13:39:13.000000 cg-33.1.2/cg/constants/rnafusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-01 13:39:13.000000 cg-33.1.2/cg/constants/sample_sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-06-01 13:39:13.000000 cg-33.1.2/cg/constants/scout_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-01 13:39:13.000000 cg-33.1.2/cg/constants/sequencing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-01 13:39:13.000000 cg-33.1.2/cg/constants/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-01 13:39:13.000000 cg-33.1.2/cg/constants/subject.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-01 13:39:13.000000 cg-33.1.2/cg/constants/symbols.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-01 13:39:13.000000 cg-33.1.2/cg/constants/taxprofiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-01 13:39:13.000000 cg-33.1.2/cg/constants/tb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-06-01 13:39:13.000000 cg-33.1.2/cg/exc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:13.000000 cg-33.1.2/cg/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-01 13:39:13.000000 cg-33.1.2/cg/io/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-06-01 13:39:13.000000 cg-33.1.2/cg/io/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-01 13:39:13.000000 cg-33.1.2/cg/io/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-01 13:39:13.000000 cg-33.1.2/cg/io/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-01 13:39:13.000000 cg-33.1.2/cg/io/validate_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-01 13:39:13.000000 cg-33.1.2/cg/io/xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-01 13:39:13.000000 cg-33.1.2/cg/io/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/meta/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8577 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/archive/ddn_dataflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/meta/backup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/backup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18893 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/backup/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/backup/pdc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/meta/clean/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/clean/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/clean/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14404 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/clean/demultiplexed_flow_cells.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/clean/flow_cell_run_directories.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/meta/compress/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/compress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12476 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/compress/compress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/compress/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13049 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/deliver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8032 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/deliver_ticket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/meta/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/demultiplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/demultiplex/delete_demultiplex_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18178 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/demultiplex/demux_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/demultiplex/files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/meta/encryption/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/encryption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10256 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/encryption/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10954 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/invoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/meta/observations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/observations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/observations/balsamic_observations_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/observations/mip_dna_observations_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/observations/observations_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/meta/orders/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/orders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/orders/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/orders/balsamic_qc_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/orders/balsamic_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/orders/balsamic_umi_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15376 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/orders/case_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/orders/fastq_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/orders/fluffy_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/orders/lims.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/orders/metagenome_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/orders/microbial_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/orders/microsalt_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/orders/mip_dna_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/orders/mip_rna_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/orders/pool_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/orders/rml_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/orders/sars_cov_2_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/orders/submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/orders/ticket_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/meta/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10470 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/report/balsamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/report/balsamic_umi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/report/field_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7274 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/report/mip_dna.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18537 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/report/report_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/report/rnafusion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/meta/report/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    78964 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/report/templates/balsamic_report.html
+-rw-r--r--   0 runner    (1001) docker     (123)   151463 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/report/templates/bootstrap.html
+-rw-r--r--   0 runner    (1001) docker     (123)    77831 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/report/templates/mip-dna_report.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/meta/rsync/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/rsync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12066 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/rsync/rsync_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/rsync/sbatch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/meta/tar/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/tar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/tar/tar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/meta/transfer/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/transfer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10070 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/transfer/external_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8417 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/transfer/flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/transfer/lims.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/meta/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/upload/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/meta/upload/balsamic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/upload/balsamic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/upload/balsamic/balsamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/upload/coverage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/meta/upload/fohm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/upload/fohm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12140 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/upload/fohm/fohm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/meta/upload/gisaid/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/upload/gisaid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/upload/gisaid/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13572 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/upload/gisaid/gisaid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/upload/gisaid/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/upload/gt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/meta/upload/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/upload/mip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/upload/mip/mip_dna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/upload/mip/mip_rna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/upload/mutacc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/meta/upload/nipt/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/upload/nipt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/upload/nipt/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7542 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/upload/nipt/nipt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/meta/upload/rnafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/upload/rnafusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/upload/rnafusion/rnafusion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/meta/upload/scout/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/upload/scout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/upload/scout/balsamic_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/upload/scout/balsamic_umi_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/upload/scout/hk_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/upload/scout/mip_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/upload/scout/rnafusion_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/upload/scout/scout_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18719 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/upload/scout/uploadscoutapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/upload/upload_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/upload/vogue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/meta/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20004 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/workflow/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26519 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/workflow/balsamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/workflow/balsamic_pon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/workflow/balsamic_qc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/workflow/balsamic_umi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11670 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/workflow/fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13390 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/workflow/fluffy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18121 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/workflow/microsalt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14033 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/workflow/mip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/workflow/mip_dna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/workflow/mip_rna.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10762 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/workflow/mutant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10236 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/workflow/nextflow_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/workflow/prepare_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18235 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/workflow/rnafusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/workflow/taxprofiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-06-01 13:39:13.000000 cg-33.1.2/cg/meta/workflow/tower_common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-01 13:39:13.000000 cg-33.1.2/cg/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-01 13:39:13.000000 cg-33.1.2/cg/models/analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/models/balsamic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:13.000000 cg-33.1.2/cg/models/balsamic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-01 13:39:13.000000 cg-33.1.2/cg/models/balsamic/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-06-01 13:39:13.000000 cg-33.1.2/cg/models/balsamic/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-01 13:39:13.000000 cg-33.1.2/cg/models/balsamic/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13073 2023-06-01 13:39:13.000000 cg-33.1.2/cg/models/cg_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/models/cgstats/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:13.000000 cg-33.1.2/cg/models/cgstats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-01 13:39:13.000000 cg-33.1.2/cg/models/cgstats/flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-06-01 13:39:13.000000 cg-33.1.2/cg/models/cgstats/stats_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-06-01 13:39:13.000000 cg-33.1.2/cg/models/compression_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/models/deliverables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:13.000000 cg-33.1.2/cg/models/deliverables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-06-01 13:39:13.000000 cg-33.1.2/cg/models/deliverables/metric_deliverables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/models/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:13.000000 cg-33.1.2/cg/models/demultiplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10905 2023-06-01 13:39:13.000000 cg-33.1.2/cg/models/demultiplex/demux_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8513 2023-06-01 13:39:13.000000 cg-33.1.2/cg/models/demultiplex/flow_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-06-01 13:39:13.000000 cg-33.1.2/cg/models/demultiplex/run_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-01 13:39:13.000000 cg-33.1.2/cg/models/demultiplex/sbatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-01 13:39:13.000000 cg-33.1.2/cg/models/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-06-01 13:39:13.000000 cg-33.1.2/cg/models/file_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/models/invoice/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:13.000000 cg-33.1.2/cg/models/invoice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-06-01 13:39:13.000000 cg-33.1.2/cg/models/invoice/invoice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/models/lims/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:13.000000 cg-33.1.2/cg/models/lims/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-06-01 13:39:13.000000 cg-33.1.2/cg/models/lims/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/models/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:13.000000 cg-33.1.2/cg/models/mip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-01 13:39:13.000000 cg-33.1.2/cg/models/mip/mip_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-01 13:39:13.000000 cg-33.1.2/cg/models/mip/mip_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-06-01 13:39:13.000000 cg-33.1.2/cg/models/mip/mip_metrics_deliverables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-06-01 13:39:13.000000 cg-33.1.2/cg/models/mip/mip_sample_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/models/nextflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:13.000000 cg-33.1.2/cg/models/nextflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-06-01 13:39:13.000000 cg-33.1.2/cg/models/nextflow/deliverables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-01 13:39:13.000000 cg-33.1.2/cg/models/nextflow/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/models/observations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:13.000000 cg-33.1.2/cg/models/observations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-06-01 13:39:13.000000 cg-33.1.2/cg/models/observations/input_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/models/orders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:13.000000 cg-33.1.2/cg/models/orders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-01 13:39:13.000000 cg-33.1.2/cg/models/orders/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6002 2023-06-01 13:39:13.000000 cg-33.1.2/cg/models/orders/excel_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-06-01 13:39:13.000000 cg-33.1.2/cg/models/orders/json_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-06-01 13:39:13.000000 cg-33.1.2/cg/models/orders/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-01 13:39:13.000000 cg-33.1.2/cg/models/orders/orderform_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-06-01 13:39:13.000000 cg-33.1.2/cg/models/orders/sample_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9856 2023-06-01 13:39:13.000000 cg-33.1.2/cg/models/orders/samples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/models/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:13.000000 cg-33.1.2/cg/models/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-06-01 13:39:13.000000 cg-33.1.2/cg/models/report/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-06-01 13:39:13.000000 cg-33.1.2/cg/models/report/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-06-01 13:39:13.000000 cg-33.1.2/cg/models/report/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-06-01 13:39:13.000000 cg-33.1.2/cg/models/report/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/models/rnafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:13.000000 cg-33.1.2/cg/models/rnafusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-01 13:39:13.000000 cg-33.1.2/cg/models/rnafusion/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-01 13:39:13.000000 cg-33.1.2/cg/models/rnafusion/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-01 13:39:13.000000 cg-33.1.2/cg/models/rnafusion/rnafusion_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/models/scout/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:13.000000 cg-33.1.2/cg/models/scout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-06-01 13:39:13.000000 cg-33.1.2/cg/models/scout/scout_load_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/models/slurm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:13.000000 cg-33.1.2/cg/models/slurm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-01 13:39:13.000000 cg-33.1.2/cg/models/slurm/sbatch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/models/taxprofiler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:13.000000 cg-33.1.2/cg/models/taxprofiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-01 13:39:13.000000 cg-33.1.2/cg/models/taxprofiler/taxprofiler_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/models/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:13.000000 cg-33.1.2/cg/models/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-01 13:39:13.000000 cg-33.1.2/cg/models/workflow/mutant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    25590 2023-06-01 13:39:13.000000 cg-33.1.2/cg/resources/20181012_Indices.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-01 13:39:13.000000 cg-33.1.2/cg/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-06-01 13:39:13.000000 cg-33.1.2/cg/resources/rnafusion_bundle_filenames.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:13.000000 cg-33.1.2/cg/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16940 2023-06-01 13:39:13.000000 cg-33.1.2/cg/server/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18031 2023-06-01 13:39:13.000000 cg-33.1.2/cg/server/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-06-01 13:39:13.000000 cg-33.1.2/cg/server/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-01 13:39:13.000000 cg-33.1.2/cg/server/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-06-01 13:39:13.000000 cg-33.1.2/cg/server/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-01 13:39:13.000000 cg-33.1.2/cg/server/ext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/server/invoices/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-01 13:39:13.000000 cg-33.1.2/cg/server/invoices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/server/invoices/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/server/invoices/templates/invoices/
+-rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-06-01 13:39:13.000000 cg-33.1.2/cg/server/invoices/templates/invoices/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-06-01 13:39:13.000000 cg-33.1.2/cg/server/invoices/templates/invoices/invoice.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-06-01 13:39:13.000000 cg-33.1.2/cg/server/invoices/templates/invoices/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-06-01 13:39:14.000000 cg-33.1.2/cg/server/invoices/templates/invoices/new.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7794 2023-06-01 13:39:14.000000 cg-33.1.2/cg/server/invoices/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/server/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/server/templates/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-01 13:39:14.000000 cg-33.1.2/cg/server/templates/admin/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/store/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-01 13:39:14.000000 cg-33.1.2/cg/store/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/store/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-01 13:39:14.000000 cg-33.1.2/cg/store/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10616 2023-06-01 13:39:14.000000 cg-33.1.2/cg/store/api/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6942 2023-06-01 13:39:14.000000 cg-33.1.2/cg/store/api/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-06-01 13:39:14.000000 cg-33.1.2/cg/store/api/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-06-01 13:39:14.000000 cg-33.1.2/cg/store/api/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-06-01 13:39:14.000000 cg-33.1.2/cg/store/api/find_basic_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28994 2023-06-01 13:39:14.000000 cg-33.1.2/cg/store/api/find_business_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38700 2023-06-01 13:39:14.000000 cg-33.1.2/cg/store/api/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/store/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/cg/store/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-06-01 13:39:14.000000 cg-33.1.2/cg/store/filters/status_analysis_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-06-01 13:39:14.000000 cg-33.1.2/cg/store/filters/status_application_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-06-01 13:39:14.000000 cg-33.1.2/cg/store/filters/status_application_version_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-01 13:39:14.000000 cg-33.1.2/cg/store/filters/status_bed_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-01 13:39:14.000000 cg-33.1.2/cg/store/filters/status_bed_version_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10388 2023-06-01 13:39:14.000000 cg-33.1.2/cg/store/filters/status_case_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-01 13:39:14.000000 cg-33.1.2/cg/store/filters/status_case_sample_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-01 13:39:14.000000 cg-33.1.2/cg/store/filters/status_collaboration_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-06-01 13:39:14.000000 cg-33.1.2/cg/store/filters/status_customer_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-06-01 13:39:14.000000 cg-33.1.2/cg/store/filters/status_flow_cell_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-01 13:39:14.000000 cg-33.1.2/cg/store/filters/status_invoice_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-01 13:39:14.000000 cg-33.1.2/cg/store/filters/status_organism_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-01 13:39:14.000000 cg-33.1.2/cg/store/filters/status_panel_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-06-01 13:39:14.000000 cg-33.1.2/cg/store/filters/status_pool_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8892 2023-06-01 13:39:14.000000 cg-33.1.2/cg/store/filters/status_sample_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-01 13:39:14.000000 cg-33.1.2/cg/store/filters/status_user_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29946 2023-06-01 13:39:14.000000 cg-33.1.2/cg/store/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-01 13:39:14.000000 cg-33.1.2/cg/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/utils/checksum/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/cg/utils/checksum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-01 13:39:14.000000 cg-33.1.2/cg/utils/checksum/checksum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/utils/click/
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-06-01 13:39:14.000000 cg-33.1.2/cg/utils/click/EnumChoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/cg/utils/click/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-06-01 13:39:14.000000 cg-33.1.2/cg/utils/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-06-01 13:39:14.000000 cg-33.1.2/cg/utils/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-01 13:39:14.000000 cg-33.1.2/cg/utils/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-06-01 13:39:14.000000 cg-33.1.2/cg/utils/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-01 13:39:14.000000 cg-33.1.2/cg/utils/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-01 13:39:14.000000 cg-33.1.2/cg/utils/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-01 13:39:14.000000 cg-33.1.2/cg/utils/files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg/utils/flask/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/cg/utils/flask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-01 13:39:14.000000 cg-33.1.2/cg/utils/flask/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-01 13:39:14.000000 cg-33.1.2/cg/utils/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-01 13:39:14.000000 cg-33.1.2/cg/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/cg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-06-01 13:39:26.000000 cg-33.1.2/cg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    40093 2023-06-01 13:39:27.000000 cg-33.1.2/cg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 13:39:26.000000 cg-33.1.2/cg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-01 13:39:26.000000 cg-33.1.2/cg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 13:39:26.000000 cg-33.1.2/cg.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-01 13:39:26.000000 cg-33.1.2/cg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-01 13:39:26.000000 cg-33.1.2/cg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-01 13:39:14.000000 cg-33.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-01 13:39:14.000000 cg-33.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 13:39:27.000000 cg-33.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-01 13:39:14.000000 cg-33.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/apps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/apps/cgstats/
+-rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-06-01 13:39:14.000000 cg-33.1.2/tests/apps/cgstats/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/apps/cgstats/crud/
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-06-01 13:39:14.000000 cg-33.1.2/tests/apps/cgstats/crud/test_create_novaseq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-01 13:39:14.000000 cg-33.1.2/tests/apps/cgstats/crud/test_delete.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/apps/cgstats/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-01 13:39:14.000000 cg-33.1.2/tests/apps/cgstats/parsers/test_adapter_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-01 13:39:14.000000 cg-33.1.2/tests/apps/cgstats/parsers/test_conversion_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-01 13:39:14.000000 cg-33.1.2/tests/apps/cgstats/parsers/test_demux_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-01 13:39:14.000000 cg-33.1.2/tests/apps/cgstats/parsers/test_quality_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-01 13:39:14.000000 cg-33.1.2/tests/apps/cgstats/parsers/test_run_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-06-01 13:39:14.000000 cg-33.1.2/tests/apps/cgstats/test_cgstats_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-01 13:39:14.000000 cg-33.1.2/tests/apps/cgstats/test_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-01 13:39:14.000000 cg-33.1.2/tests/apps/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/apps/coverage/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-01 13:39:14.000000 cg-33.1.2/tests/apps/coverage/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-06-01 13:39:14.000000 cg-33.1.2/tests/apps/coverage/test_coverage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/apps/crunchy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-06-01 13:39:14.000000 cg-33.1.2/tests/apps/crunchy/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-06-01 13:39:14.000000 cg-33.1.2/tests/apps/crunchy/test_compress_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-06-01 13:39:14.000000 cg-33.1.2/tests/apps/crunchy/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14590 2023-06-01 13:39:14.000000 cg-33.1.2/tests/apps/crunchy/test_crunchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9107 2023-06-01 13:39:14.000000 cg-33.1.2/tests/apps/crunchy/test_spring_decompression.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/apps/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/apps/demultiplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9961 2023-06-01 13:39:14.000000 cg-33.1.2/tests/apps/demultiplex/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-01 13:39:14.000000 cg-33.1.2/tests/apps/demultiplex/test_convert_to_sample_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-01 13:39:14.000000 cg-33.1.2/tests/apps/demultiplex/test_demultiplex_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-06-01 13:39:14.000000 cg-33.1.2/tests/apps/demultiplex/test_sample_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-06-01 13:39:14.000000 cg-33.1.2/tests/apps/demultiplex/test_validate_sample_sheet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/apps/gens/
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-06-01 13:39:14.000000 cg-33.1.2/tests/apps/gens/test_gens_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/apps/gt/
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-06-01 13:39:14.000000 cg-33.1.2/tests/apps/gt/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-06-01 13:39:14.000000 cg-33.1.2/tests/apps/gt/test_gt_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/apps/hk/
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-06-01 13:39:14.000000 cg-33.1.2/tests/apps/hk/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-01 13:39:14.000000 cg-33.1.2/tests/apps/hk/test__getattr__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-01 13:39:14.000000 cg-33.1.2/tests/apps/hk/test_add_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-06-01 13:39:14.000000 cg-33.1.2/tests/apps/hk/test_bundles.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-01 13:39:14.000000 cg-33.1.2/tests/apps/hk/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24046 2023-06-01 13:39:14.000000 cg-33.1.2/tests/apps/hk/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-06-01 13:39:14.000000 cg-33.1.2/tests/apps/hk/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/apps/lims/
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-06-01 13:39:14.000000 cg-33.1.2/tests/apps/lims/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-06-01 13:39:14.000000 cg-33.1.2/tests/apps/lims/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-01 13:39:14.000000 cg-33.1.2/tests/apps/lims/test_sample_sheet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/apps/loqus/
+-rw-r--r--   0 runner    (1001) docker     (123)     9785 2023-06-01 13:39:14.000000 cg-33.1.2/tests/apps/loqus/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-06-01 13:39:14.000000 cg-33.1.2/tests/apps/loqus/test_loqusdb_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/apps/madeline/
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-06-01 13:39:14.000000 cg-33.1.2/tests/apps/madeline/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-06-01 13:39:14.000000 cg-33.1.2/tests/apps/madeline/test_madeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/apps/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-06-01 13:39:14.000000 cg-33.1.2/tests/apps/mip/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-06-01 13:39:14.000000 cg-33.1.2/tests/apps/mip/test_config_mip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/apps/mutacc_auto/
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-01 13:39:14.000000 cg-33.1.2/tests/apps/mutacc_auto/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-06-01 13:39:14.000000 cg-33.1.2/tests/apps/mutacc_auto/test_mutacc_auto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/apps/orderform/
+-rw-r--r--   0 runner    (1001) docker     (123)    11900 2023-06-01 13:39:14.000000 cg-33.1.2/tests/apps/orderform/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-06-01 13:39:14.000000 cg-33.1.2/tests/apps/orderform/test_excel_orderform_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-06-01 13:39:14.000000 cg-33.1.2/tests/apps/orderform/test_excel_sample_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-01 13:39:14.000000 cg-33.1.2/tests/apps/orderform/test_json_orderform_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-06-01 13:39:14.000000 cg-33.1.2/tests/apps/orderform/test_orderform_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/apps/scout/
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-06-01 13:39:14.000000 cg-33.1.2/tests/apps/scout/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-01 13:39:14.000000 cg-33.1.2/tests/apps/scout/test_get_causative_variants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-06-01 13:39:14.000000 cg-33.1.2/tests/apps/scout/test_get_scout_cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-06-01 13:39:14.000000 cg-33.1.2/tests/apps/scout/test_scout_load_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-06-01 13:39:14.000000 cg-33.1.2/tests/apps/scout/test_scout_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/apps/sequencing_metrics_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/apps/sequencing_metrics_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7152 2023-06-01 13:39:14.000000 cg-33.1.2/tests/apps/sequencing_metrics_parser/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/apps/sequencing_metrics_parser/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-06-01 13:39:14.000000 cg-33.1.2/tests/apps/sequencing_metrics_parser/parsers/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-01 13:39:14.000000 cg-33.1.2/tests/apps/sequencing_metrics_parser/parsers/test_bcl2fastq_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-06-01 13:39:14.000000 cg-33.1.2/tests/apps/sequencing_metrics_parser/parsers/test_bcl_convert_to_sequencing_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10062 2023-06-01 13:39:14.000000 cg-33.1.2/tests/apps/sequencing_metrics_parser/parsers/test_bclconvert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-01 13:39:14.000000 cg-33.1.2/tests/apps/sequencing_metrics_parser/test_sequencing_metrics_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/apps/slurm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-01 13:39:14.000000 cg-33.1.2/tests/apps/slurm/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-06-01 13:39:14.000000 cg-33.1.2/tests/apps/slurm/test_slurm_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-01 13:39:14.000000 cg-33.1.2/tests/apps/test_apps_environ.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-01 13:39:14.000000 cg-33.1.2/tests/apps/test_osticket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/apps/vogue/
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-01 13:39:14.000000 cg-33.1.2/tests/apps/vogue/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-06-01 13:39:14.000000 cg-33.1.2/tests/apps/vogue/test_vogue_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/cli/add/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/add/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/add/test_cli_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/add/test_cli_add_customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/add/test_cli_add_family.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/add/test_cli_add_relationship.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/add/test_cli_add_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/cli/backup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/backup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/backup/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/backup/test_backup_command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/cli/clean/
+-rw-r--r--   0 runner    (1001) docker     (123)     6069 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/clean/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/clean/test_balsamic_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/clean/test_clean_hk_bundle_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/clean/test_hk_bundle_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/clean/test_hk_case_bundle_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/clean/test_microbial_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/clean/test_rsync_past_run_dirs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/cli/compress/
+-rw-r--r--   0 runner    (1001) docker     (123)    10311 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/compress/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6929 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/compress/test_cli_compress_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/compress/test_cli_decompress_spring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/compress/test_compress_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/compress/test_store_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/cli/delete/
+-rw-r--r--   0 runner    (1001) docker     (123)    12781 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/delete/test_cli_delete_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/delete/test_cli_delete_cases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/cli/deliver/
+-rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/deliver/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/deliver/test_deliver_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/deliver/test_rsync_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8562 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/deliver/test_run_deliver_cmd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/cli/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/demultiplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11390 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/demultiplex/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/demultiplex/test_add_flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/demultiplex/test_create_sample_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11526 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/demultiplex/test_demultiplex_flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/demultiplex/test_finish_demux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/demultiplex/test_stats_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/demultiplex/test_validate_sample_sheet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/cli/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/generate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/cli/generate/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/generate/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/generate/report/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/generate/report/test_cli_delivery_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/generate/report/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/generate/test_cli_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/cli/get/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/get/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/get/test_cli_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/get/test_cli_get_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/get/test_cli_get_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/get/test_cli_get_flow_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8862 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/get/test_cli_get_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/cli/set/
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/set/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7320 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/set/test_cli_set_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/set/test_cli_set_cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/set/test_cli_set_flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/set/test_cli_set_list_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12516 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/set/test_cli_set_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/set/test_cli_set_samples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/cli/store/
+-rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/store/test_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/test_clean.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/cli/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/cli/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/cli/tests/fixtures/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/tests/fixtures/data/fastq.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/cli/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/upload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10414 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/upload/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/upload/test_cli_scout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/upload/test_cli_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/upload/test_cli_upload_auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/upload/test_cli_upload_delivery_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/upload/test_cli_upload_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/upload/test_cli_upload_genotype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/upload/test_cli_upload_gens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9971 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/upload/test_cli_upload_nipt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/upload/test_cli_upload_nipt_ftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/upload/test_cli_upload_nipt_statina.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/upload/test_cli_upload_observations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/upload/test_cli_upload_vogue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/cli/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/workflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/cli/workflow/balsamic/
+-rw-r--r--   0 runner    (1001) docker     (123)    30801 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/workflow/balsamic/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15328 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/workflow/balsamic/test_compound_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/workflow/balsamic/test_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/workflow/balsamic/test_report_deliver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/workflow/balsamic/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/workflow/balsamic/test_store_housekeeper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/workflow/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/cli/workflow/fastq/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/workflow/fastq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/workflow/fastq/test_fastq_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/cli/workflow/fluffy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/workflow/fluffy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/workflow/fluffy/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/workflow/fluffy/test_cli_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/workflow/fluffy/test_cli_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/workflow/fluffy/test_cli_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/workflow/fluffy/test_cli_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/cli/workflow/microsalt/
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/workflow/microsalt/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/cli/workflow/microsalt/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/workflow/microsalt/snapshots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/workflow/microsalt/snapshots/snap_test_microsalt_case_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7185 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/workflow/microsalt/test_microsalt_case_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/workflow/microsalt/test_microsalt_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/cli/workflow/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/workflow/mip/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6796 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/workflow/mip/test_cli_mip_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/workflow/mip/test_cli_mip_dna_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/workflow/mip/test_cli_mip_dna_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/workflow/mip/test_cli_mip_dna_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/workflow/mip/test_cli_mip_dna_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/workflow/mip/test_cli_mip_rna_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/workflow/mip/test_cli_mip_rna_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8558 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/workflow/mip/test_cli_mip_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/cli/workflow/rnafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/workflow/rnafusion/test_cli_rnafusion_compound_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/workflow/rnafusion/test_cli_rnafusion_config_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/workflow/rnafusion/test_cli_rnafusion_metrics_deliver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/workflow/rnafusion/test_cli_rnafusion_report_deliver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/workflow/rnafusion/test_cli_rnafusion_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8449 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/workflow/rnafusion/test_cli_rnafusion_store_housekeeper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/cli/workflow/taxprofiler/
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/workflow/taxprofiler/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/workflow/taxprofiler/test_cli_taxprofiler_compound_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/workflow/taxprofiler/test_cli_taxprofiler_config_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/workflow/test_cli_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-06-01 13:39:14.000000 cg-33.1.2/tests/cli/workflow/test_cli_workflow_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72597 2023-06-01 13:39:14.000000 cg-33.1.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/fixtures/analysis/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/fixtures/analysis/balsamic/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/fixtures/analysis/balsamic/tn_wgs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/analysis/balsamic/tn_wgs/adm1.cram
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/analysis/balsamic/tn_wgs/ascat.output.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/analysis/balsamic/tn_wgs/snv.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/analysis/balsamic/tn_wgs/sv.vcf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/fixtures/analysis/microsalt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/
+-rw-r--r--   0 runner    (1001) docker     (123)    14644 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/
+-rw-r--r--   0 runner    (1001) docker     (123)    15713 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/fixtures/analysis/mip/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/fixtures/analysis/mip/dna/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/analysis/mip/dna/ADM1.baf.bed.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/analysis/mip/dna/ADM1.cov.bed.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/analysis/mip/dna/ADM2.cram
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/analysis/mip/dna/ADM3.cram
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/analysis/mip/dna/adm1.cram
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/analysis/mip/dna/adm1.mt.bam
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/analysis/mip/dna/multiqc.html
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/analysis/mip/dna/report.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/analysis/mip/dna/smn.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/analysis/mip/dna/snv.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/analysis/mip/dna/snv_research.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/analysis/mip/dna/str.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/analysis/mip/dna/sv.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/analysis/mip/dna/sv_research.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/analysis/mip/dna/vcf2cytosure.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/fixtures/analysis/rnafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)     5587 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/analysis/rnafusion/multiqc_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/analysis/sample_coverage.bed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/fixtures/apps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/fixtures/apps/balsamic/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/fixtures/apps/balsamic/case/
+-rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/balsamic/case/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/balsamic/case/metadata.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/balsamic/case/metadata_directory.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/balsamic/case/metadata_file_tags.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/fixtures/apps/crunchy/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/crunchy/spring_metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/fixtures/apps/demultiplexing/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/
+-rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/Adapter_Metrics.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/Quality_Metrics.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/RunInfo.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/dummy_run_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/dummy_run_R1_001.fastq.gz.md5
+-rw-r--r--   0 runner    (1001) docker     (123)   338370 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R1_001.fastq.gz.md5
+-rw-r--r--   0 runner    (1001) docker     (123)   338349 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R2_001.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R2_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R2_001.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/hiseq/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/hiseq/180522_ST-E00198_0301_BHLCKNCCXY/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/hiseq/180522_ST-E00198_0301_BHLCKNCCXY/RTAComplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/hiseq/180522_ST-E00198_0301_BHLCKNCCXY/SampleSheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/hiseq/180522_ST-E00198_0301_BHLCKNCCXY/copy_complete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/hiseq/180522_ST-E00198_0301_BHLCKNCCXY/runParameters.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/CopyComplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/RTAComplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/demuxstarted.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/CopyComplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stderr
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/RTAComplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/SampleSheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/demuxstarted.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_x/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_x/20230508_LH00188_0003_A22522YLT3/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2584 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_x/20230508_LH00188_0003_A22522YLT3/RunParameters.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/fixtures/apps/demultiplexing/raw_lims_samples/
+-rw-r--r--   0 runner    (1001) docker     (123)    92887 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/demultiplexing/raw_lims_samples/raw_samplesheet_novaseq.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/fixtures/apps/demultiplexing/run_parameters/
+-rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_different_index_cycles.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/demultiplexing/run_parameters/runParameters_missing_flowcell_run_field.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/fixtures/apps/fluffy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/fixtures/apps/fluffy/2020-23219-05/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/fluffy/2020-23219-05/2020-23219-05.WCXpredict_aberrations.filt.bed
+-rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/fluffy/SampleSheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/fluffy/deliverables.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/fluffy/fluffy_fastq.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/fluffy/multiqc_report.html
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/fluffy/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/fixtures/apps/gt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/gt/yellowhog.bcf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/fixtures/apps/madeline/
+-rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/madeline/madeline.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/fixtures/apps/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/mip/case_file.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/mip/case_metrics_deliverables.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/fixtures/apps/mip/dna/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/fixtures/apps/mip/dna/store/
+-rw-r--r--   0 runner    (1001) docker     (123)    21811 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/mip/dna/store/case_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    23364 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    37367 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/mip/dna/store/empty_case_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/mip/dna/store/empty_case_metrics_deliverables.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/mip/dna/store/empty_case_qc_sample_info.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/mip/dna/store/empty_delivery_report.html
+-rw-r--r--   0 runner    (1001) docker     (123)    62741 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/fixtures/apps/mip/rna/
+-rw-r--r--   0 runner    (1001) docker     (123)    11242 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/mip/rna/case_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    12164 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/fixtures/apps/mip/rna/store/
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/mip/rna/store/bundle_data.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/mip/rna/store/case_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/mip/sample_file.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/fixtures/apps/scout/
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/scout/643594.config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/scout/case_export.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9349 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/scout/export_causatives.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/scout/none_case_export.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/scout/other_sex_case.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/scout/panel_export.bed
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/scout/panel_export.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/fixtures/apps/sequencing_metrics_parser/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/fixtures/apps/sequencing_metrics_parser/Unaligned/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/fixtures/apps/sequencing_metrics_parser/Unaligned/Reports/
+-rw-r--r--   0 runner    (1001) docker     (123)    63569 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/sequencing_metrics_parser/Unaligned/Reports/Adapter_Metrics.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    42478 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/sequencing_metrics_parser/Unaligned/Reports/Demultiplex_Stats.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    69862 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/sequencing_metrics_parser/Unaligned/Reports/Quality_Metrics.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/sequencing_metrics_parser/Unaligned/Reports/RunInfo.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    42872 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/sequencing_metrics_parser/Unaligned/Reports/SampleSheet.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/fixtures/apps/shipping/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/apps/shipping/scout-deploy.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/fixtures/cgweb_orders/
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/cgweb_orders/balsamic.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/cgweb_orders/fastq.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/cgweb_orders/metagenome.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/cgweb_orders/microsalt.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/cgweb_orders/mip.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/cgweb_orders/mip_rna.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/cgweb_orders/rml.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/cgweb_orders/sarscov2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/fixtures/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/data/SampleSheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   258048 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/data/cgfixture.db
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/data/fastq.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    49152 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/data/hkstore.db
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/fixtures/data/yellowhog/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/data/yellowhog/pedigree.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/fixtures/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/io/example_csv.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/io/example_json.json
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/io/example_xml.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/fixtures/orderforms/
+-rw-r--r--   0 runner    (1001) docker     (123)   257271 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/orderforms/1508.27.balsamic.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   256694 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/orderforms/1508.27.balsamic_qc.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   257319 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/orderforms/1508.27.balsamic_umi.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   256733 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/orderforms/1508.27.fastq.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   257317 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/orderforms/1508.27.mip.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   257230 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/orderforms/1508.27.mip_rna.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    95490 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/orderforms/1603.11.microbial.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   158941 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/orderforms/1604.15.rml.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    88438 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/orderforms/1605.10.metagenome.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   228196 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/orderforms/2184.7.sarscov2.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    18639 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/orderforms/NIPT-json.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6611 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/orderforms/mip_uploaded_json_orderform.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/fixtures/report/
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/report/case_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/report/lims_exported_samples.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-01 13:39:14.000000 cg-33.1.2/tests/fixtures/report/lims_family.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/io/
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-06-01 13:39:14.000000 cg-33.1.2/tests/io/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7766 2023-06-01 13:39:14.000000 cg-33.1.2/tests/io/test_io_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-06-01 13:39:14.000000 cg-33.1.2/tests/io/test_io_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-06-01 13:39:14.000000 cg-33.1.2/tests/io/test_io_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-01 13:39:14.000000 cg-33.1.2/tests/io/test_io_xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-06-01 13:39:14.000000 cg-33.1.2/tests/io/test_io_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-06-01 13:39:14.000000 cg-33.1.2/tests/io/test_validate_path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/meta/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/archive/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12864 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/archive/test_archiving.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/meta/backup/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/backup/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24493 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/backup/test_meta_backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/backup/test_meta_pdc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/meta/clean/
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/clean/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/clean/test_clean_demultiplexed_runs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/clean/test_clean_flow_cell_run_directories.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/meta/compress/
+-rw-r--r--   0 runner    (1001) docker     (123)     7793 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/compress/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7115 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/compress/test_clean_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/compress/test_compress_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/compress/test_compress_meta_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/compress/test_decompress_spring_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/compress/test_meta_compress_update_hk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/meta/deliver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/deliver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/deliver/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/deliver/test_deliver_ticket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10178 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/deliver/test_delivery_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/meta/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)    12217 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/demultiplex/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13452 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/demultiplex/test_delete_demultiplex_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15635 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/demultiplex/test_demux_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/demultiplex/test_rename_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/meta/demultiplex/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/meta/demultiplex/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/meta/demultiplex/tests/fixtures/apps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/meta/demultiplex/tests/fixtures/apps/demultiplexing/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/meta/demultiplex/tests/fixtures/apps/demultiplexing/flow-cell-runs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/meta/demultiplex/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/demultiplex/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/copycomplete.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/meta/encryption/
+-rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/encryption/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11132 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/encryption/test_encryption.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/meta/observations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/observations/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16497 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/observations/test_meta_upload_observations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/meta/orders/
+-rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/orders/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/orders/test_PoolSubmitter_validate_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/orders/test_SarsCov2Submitter_store_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/orders/test_SarsCov2Submitter_validate_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19748 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/orders/test_meta_orders_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7123 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/orders/test_meta_orders_lims.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29658 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/orders/test_meta_orders_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/orders/test_ticket_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/meta/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/report/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/report/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/report/test_balsamic_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/report/test_field_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/report/test_mip_dna_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13311 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/report/test_report_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/report/test_rnafusion_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/meta/rsync/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/rsync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/rsync/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8811 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/rsync/test_rsync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/test_invoice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/meta/transfer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/transfer/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10019 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/transfer/test_external_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16433 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/transfer/test_meta_transfer_flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/transfer/test_meta_transfer_lims.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/meta/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/upload/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/meta/upload/balsamic/
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/upload/balsamic/test_balsamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/upload/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/meta/upload/gisaid/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/upload/gisaid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/meta/upload/gisaid/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/upload/gisaid/fixtures/four_samples.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/upload/gisaid/fixtures/invalid_housekeeper.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/upload/gisaid/fixtures/valid_gisaid.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/upload/gisaid/fixtures/valid_housekeeper.fasta
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/meta/upload/mutacc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/upload/mutacc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/upload/mutacc/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/upload/mutacc/test_meta_upload_mutacc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/meta/upload/nipt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/upload/nipt/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/upload/nipt/test_nipt_upload_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/meta/upload/scout/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/upload/scout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23429 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/upload/scout/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/upload/scout/test_generate_load_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/upload/scout/test_meta_upload_scoutapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32141 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7857 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/upload/scout/test_scout_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/upload/test_meta_upload_coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/upload/test_upload_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/upload/test_upload_genotypes_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/meta/upload/vogue/
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/upload/vogue/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/upload/vogue/test_upload_vogue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/meta/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7681 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/workflow/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/workflow/test_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/workflow/test_balsamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/workflow/test_microsalt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/workflow/test_prepare_fastq_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-06-01 13:39:14.000000 cg-33.1.2/tests/meta/workflow/test_rnafusion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-06-01 13:39:14.000000 cg-33.1.2/tests/mocks/balsamic_analysis_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-06-01 13:39:14.000000 cg-33.1.2/tests/mocks/crunchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20596 2023-06-01 13:39:14.000000 cg-33.1.2/tests/mocks/hk_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-06-01 13:39:14.000000 cg-33.1.2/tests/mocks/limsmock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-01 13:39:14.000000 cg-33.1.2/tests/mocks/madeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-06-01 13:39:14.000000 cg-33.1.2/tests/mocks/mip_analysis_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-06-01 13:39:14.000000 cg-33.1.2/tests/mocks/osticket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-06-01 13:39:14.000000 cg-33.1.2/tests/mocks/process_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-06-01 13:39:14.000000 cg-33.1.2/tests/mocks/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-06-01 13:39:14.000000 cg-33.1.2/tests/mocks/scout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-01 13:39:14.000000 cg-33.1.2/tests/mocks/store_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-01 13:39:14.000000 cg-33.1.2/tests/mocks/tb_mock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/models/balsamic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/models/balsamic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-01 13:39:14.000000 cg-33.1.2/tests/models/balsamic/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-01 13:39:14.000000 cg-33.1.2/tests/models/balsamic/test_balsamic_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-01 13:39:14.000000 cg-33.1.2/tests/models/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/models/demultiplexing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/models/demultiplexing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-01 13:39:14.000000 cg-33.1.2/tests/models/demultiplexing/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-01 13:39:14.000000 cg-33.1.2/tests/models/demultiplexing/test_demux_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-06-01 13:39:14.000000 cg-33.1.2/tests/models/demultiplexing/test_flowcell_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4894 2023-06-01 13:39:14.000000 cg-33.1.2/tests/models/demultiplexing/test_run_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/models/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-06-01 13:39:14.000000 cg-33.1.2/tests/models/mip/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-06-01 13:39:14.000000 cg-33.1.2/tests/models/mip/test_mip_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-06-01 13:39:14.000000 cg-33.1.2/tests/models/mip/test_mip_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-06-01 13:39:14.000000 cg-33.1.2/tests/models/mip/test_mip_metrics_deliverables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-06-01 13:39:14.000000 cg-33.1.2/tests/models/mip/test_mip_sample_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/models/nextflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-01 13:39:14.000000 cg-33.1.2/tests/models/nextflow/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-01 13:39:14.000000 cg-33.1.2/tests/models/nextflow/test_nextflow_deliver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/models/observations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-01 13:39:14.000000 cg-33.1.2/tests/models/observations/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-06-01 13:39:14.000000 cg-33.1.2/tests/models/observations/test_observations_input_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/models/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/models/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5459 2023-06-01 13:39:14.000000 cg-33.1.2/tests/models/report/test_validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/models/rnafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-06-01 13:39:14.000000 cg-33.1.2/tests/models/rnafusion/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-06-01 13:39:14.000000 cg-33.1.2/tests/models/rnafusion/test_rnafusion_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-06-01 13:39:14.000000 cg-33.1.2/tests/models/test_cg_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-01 13:39:14.000000 cg-33.1.2/tests/models/test_compression_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-06-01 13:39:14.000000 cg-33.1.2/tests/models/test_file_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-01 13:39:14.000000 cg-33.1.2/tests/models/test_flowcell_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-01 13:39:14.000000 cg-33.1.2/tests/server/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-01 13:39:14.000000 cg-33.1.2/tests/server/test_server_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-01 13:39:14.000000 cg-33.1.2/tests/server/test_server_auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-01 13:39:14.000000 cg-33.1.2/tests/small_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/store/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/store/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/store/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/store/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/store/api/add/
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-06-01 13:39:14.000000 cg-33.1.2/tests/store/api/add/test_store_add_application_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-06-01 13:39:14.000000 cg-33.1.2/tests/store/api/add/test_store_add_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-06-01 13:39:14.000000 cg-33.1.2/tests/store/api/add/test_store_add_customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-06-01 13:39:14.000000 cg-33.1.2/tests/store/api/add/test_store_add_flow_celll.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17672 2023-06-01 13:39:14.000000 cg-33.1.2/tests/store/api/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/store/api/delete/
+-rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-06-01 13:39:14.000000 cg-33.1.2/tests/store/api/delete/test_store_api_delete.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/store/api/find/
+-rw-r--r--   0 runner    (1001) docker     (123)     8342 2023-06-01 13:39:14.000000 cg-33.1.2/tests/store/api/find/test_find_basic_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-06-01 13:39:14.000000 cg-33.1.2/tests/store/api/find/test_find_basic_data_application_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27372 2023-06-01 13:39:14.000000 cg-33.1.2/tests/store/api/find/test_find_business_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-06-01 13:39:14.000000 cg-33.1.2/tests/store/api/find/test_find_business_data_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-06-01 13:39:14.000000 cg-33.1.2/tests/store/api/find/test_find_business_data_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12223 2023-06-01 13:39:14.000000 cg-33.1.2/tests/store/api/find/test_find_business_data_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/store/api/status/
+-rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-06-01 13:39:14.000000 cg-33.1.2/tests/store/api/status/test_analyses_to_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-06-01 13:39:14.000000 cg-33.1.2/tests/store/api/status/test_analyses_to_delivery_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9780 2023-06-01 13:39:14.000000 cg-33.1.2/tests/store/api/status/test_store_api_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15265 2023-06-01 13:39:14.000000 cg-33.1.2/tests/store/api/status/test_store_api_status_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54170 2023-06-01 13:39:14.000000 cg-33.1.2/tests/store/api/status/test_store_api_status_cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-01 13:39:14.000000 cg-33.1.2/tests/store/api/status/test_store_api_status_customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-01 13:39:14.000000 cg-33.1.2/tests/store/api/status/test_store_api_status_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8763 2023-06-01 13:39:14.000000 cg-33.1.2/tests/store/api/status/test_store_api_status_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-06-01 13:39:14.000000 cg-33.1.2/tests/store/api/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15566 2023-06-01 13:39:14.000000 cg-33.1.2/tests/store/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/store/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)    14547 2023-06-01 13:39:14.000000 cg-33.1.2/tests/store/filters/test_status_analyses_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-06-01 13:39:14.000000 cg-33.1.2/tests/store/filters/test_status_application_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10505 2023-06-01 13:39:14.000000 cg-33.1.2/tests/store/filters/test_status_application_version_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-06-01 13:39:14.000000 cg-33.1.2/tests/store/filters/test_status_bed_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-01 13:39:14.000000 cg-33.1.2/tests/store/filters/test_status_bed_version_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-06-01 13:39:14.000000 cg-33.1.2/tests/store/filters/test_status_case_sample_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38171 2023-06-01 13:39:14.000000 cg-33.1.2/tests/store/filters/test_status_cases_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-01 13:39:14.000000 cg-33.1.2/tests/store/filters/test_status_collaboration_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-06-01 13:39:14.000000 cg-33.1.2/tests/store/filters/test_status_customer_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-06-01 13:39:14.000000 cg-33.1.2/tests/store/filters/test_status_flow_cell_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-06-01 13:39:14.000000 cg-33.1.2/tests/store/filters/test_status_invoice_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-06-01 13:39:14.000000 cg-33.1.2/tests/store/filters/test_status_organism_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-06-01 13:39:14.000000 cg-33.1.2/tests/store/filters/test_status_panel_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-06-01 13:39:14.000000 cg-33.1.2/tests/store/filters/test_status_pool_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22968 2023-06-01 13:39:14.000000 cg-33.1.2/tests/store/filters/test_status_samples_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-01 13:39:14.000000 cg-33.1.2/tests/store/filters/test_status_user_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-06-01 13:39:14.000000 cg-33.1.2/tests/store/test_delivery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-06-01 13:39:14.000000 cg-33.1.2/tests/store/test_store_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29888 2023-06-01 13:39:14.000000 cg-33.1.2/tests/store_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-01 13:39:14.000000 cg-33.1.2/tests/test_store_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/tests/fixtures/apps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/tests/fixtures/apps/demultiplexing/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/tests/fixtures/apps/demultiplexing/flowcell-runs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/copycomplete.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/tests/fixtures/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/tests/fixtures/data/fastq.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:27.000000 cg-33.1.2/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:39:14.000000 cg-33.1.2/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-01 13:39:14.000000 cg-33.1.2/tests/utils/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-06-01 13:39:14.000000 cg-33.1.2/tests/utils/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-01 13:39:14.000000 cg-33.1.2/tests/utils/test_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-01 13:39:14.000000 cg-33.1.2/tests/utils/test_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7176 2023-06-01 13:39:14.000000 cg-33.1.2/tests/utils/test_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-06-01 13:39:14.000000 cg-33.1.2/tests/utils/test_utils.py
```

### Comparing `cg-33.1.1/PKG-INFO` & `cg-33.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cg
-Version: 33.1.1
+Version: 33.1.2
 Summary: Clinical Genomics command center
 Home-page: https://github.com/Clinical-Genomics/cg
 Author: Clinical Genomics
 Author-email: support@clinicalgenomics.se
 License: UNKNOWN
 Description: 
         # cg
```

### Comparing `cg-33.1.1/README.md` & `cg-33.1.2/README.md`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/apps/cgstats/crud/create.py` & `cg-33.1.2/cg/apps/cgstats/crud/create.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/apps/cgstats/crud/delete.py` & `cg-33.1.2/cg/apps/cgstats/crud/delete.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/apps/cgstats/crud/find.py` & `cg-33.1.2/cg/apps/cgstats/crud/find.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/apps/cgstats/db/models/base.py` & `cg-33.1.2/cg/apps/cgstats/db/models/base.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/apps/cgstats/db/models/datasource.py` & `cg-33.1.2/cg/apps/cgstats/db/models/datasource.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/apps/cgstats/db/models/demux.py` & `cg-33.1.2/cg/apps/cgstats/db/models/demux.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/apps/cgstats/db/models/demux_sample.py` & `cg-33.1.2/cg/apps/cgstats/db/models/demux_sample.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/apps/cgstats/db/models/dragen_demux_sample.py` & `cg-33.1.2/cg/apps/cgstats/db/models/dragen_demux_sample.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/apps/cgstats/db/models/sample.py` & `cg-33.1.2/cg/apps/cgstats/db/models/sample.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/apps/cgstats/db/models/support_params.py` & `cg-33.1.2/cg/apps/cgstats/db/models/support_params.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/apps/cgstats/db/models/unaligned.py` & `cg-33.1.2/cg/apps/cgstats/db/models/unaligned.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/apps/cgstats/db/models/version.py` & `cg-33.1.2/cg/apps/cgstats/db/models/version.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/apps/cgstats/parsers/adapter_metrics.py` & `cg-33.1.2/cg/apps/cgstats/parsers/adapter_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/apps/cgstats/parsers/conversion_stats.py` & `cg-33.1.2/cg/apps/cgstats/parsers/conversion_stats.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/apps/cgstats/parsers/demux_stats.py` & `cg-33.1.2/cg/apps/cgstats/parsers/demux_stats.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/apps/cgstats/parsers/dragen_demultiplexing_stats.py` & `cg-33.1.2/cg/apps/cgstats/parsers/dragen_demultiplexing_stats.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/apps/cgstats/parsers/quality_metrics.py` & `cg-33.1.2/cg/apps/cgstats/parsers/quality_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/apps/cgstats/parsers/run_info.py` & `cg-33.1.2/cg/apps/cgstats/parsers/run_info.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/apps/cgstats/stats.py` & `cg-33.1.2/cg/apps/cgstats/stats.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/apps/coverage/api.py` & `cg-33.1.2/cg/apps/coverage/api.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/apps/crunchy/crunchy.py` & `cg-33.1.2/cg/apps/crunchy/crunchy.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/apps/crunchy/files.py` & `cg-33.1.2/cg/apps/crunchy/files.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/apps/crunchy/sbatch.py` & `cg-33.1.2/cg/apps/crunchy/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/apps/demultiplex/demultiplex_api.py` & `cg-33.1.2/cg/apps/demultiplex/demultiplex_api.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/apps/demultiplex/demux_report.py` & `cg-33.1.2/cg/apps/demultiplex/demux_report.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/apps/demultiplex/sample_sheet/create.py` & `cg-33.1.2/cg/apps/demultiplex/sample_sheet/create.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/apps/demultiplex/sample_sheet/dummy_sample.py` & `cg-33.1.2/cg/apps/demultiplex/sample_sheet/dummy_sample.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/apps/demultiplex/sample_sheet/index.py` & `cg-33.1.2/cg/apps/demultiplex/sample_sheet/index.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/apps/demultiplex/sample_sheet/models.py` & `cg-33.1.2/cg/apps/demultiplex/sample_sheet/models.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/apps/demultiplex/sample_sheet/novaseq_sample_sheet.py` & `cg-33.1.2/cg/apps/demultiplex/sample_sheet/novaseq_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/apps/demultiplex/sample_sheet/validate.py` & `cg-33.1.2/cg/apps/demultiplex/sample_sheet/validate.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/apps/demultiplex/sbatch.py` & `cg-33.1.2/cg/apps/demultiplex/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/apps/gens.py` & `cg-33.1.2/cg/apps/gens.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/apps/gt.py` & `cg-33.1.2/cg/apps/gt.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/apps/hermes/hermes_api.py` & `cg-33.1.2/cg/apps/hermes/hermes_api.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/apps/hermes/models.py` & `cg-33.1.2/cg/apps/hermes/models.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/apps/housekeeper/hk.py` & `cg-33.1.2/cg/apps/housekeeper/hk.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/apps/invoice/render.py` & `cg-33.1.2/cg/apps/invoice/render.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/apps/invoice/templates/KI_pool_invoice.xlsx` & `cg-33.1.2/cg/apps/invoice/templates/KI_pool_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/apps/invoice/templates/KI_sample_invoice.xlsx` & `cg-33.1.2/cg/apps/invoice/templates/KI_sample_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/apps/invoice/templates/KTH_pool_invoice.xlsx` & `cg-33.1.2/cg/apps/invoice/templates/KTH_pool_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/apps/invoice/templates/KTH_sample_invoice.xlsx` & `cg-33.1.2/cg/apps/invoice/templates/KTH_sample_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/apps/lims/api.py` & `cg-33.1.2/cg/apps/lims/api.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/apps/lims/batch.py` & `cg-33.1.2/cg/apps/lims/batch.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/apps/lims/order.py` & `cg-33.1.2/cg/apps/lims/order.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/apps/lims/sample_sheet.py` & `cg-33.1.2/cg/apps/lims/sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/apps/loqus.py` & `cg-33.1.2/cg/apps/loqus.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/apps/madeline/api.py` & `cg-33.1.2/cg/apps/madeline/api.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/apps/mip/confighandler.py` & `cg-33.1.2/cg/apps/mip/confighandler.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/apps/mutacc_auto.py` & `cg-33.1.2/cg/apps/mutacc_auto.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/apps/orderform/excel_orderform_parser.py` & `cg-33.1.2/cg/apps/orderform/excel_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/apps/orderform/json_orderform_parser.py` & `cg-33.1.2/cg/apps/orderform/json_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/apps/orderform/orderform_parser.py` & `cg-33.1.2/cg/apps/orderform/orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/apps/osticket.py` & `cg-33.1.2/cg/apps/osticket.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/apps/scout/scout_export.py` & `cg-33.1.2/cg/apps/scout/scout_export.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/apps/scout/scoutapi.py` & `cg-33.1.2/cg/apps/scout/scoutapi.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/apps/sequencing_metrics_parser/api.py` & `cg-33.1.2/cg/apps/sequencing_metrics_parser/api.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/apps/sequencing_metrics_parser/models/bcl2fastq_metrics.py` & `cg-33.1.2/cg/apps/sequencing_metrics_parser/models/bcl2fastq_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/apps/sequencing_metrics_parser/models/bcl_convert.py` & `cg-33.1.2/cg/apps/sequencing_metrics_parser/models/bcl_convert.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/apps/sequencing_metrics_parser/parsers/bcl2fastq.py` & `cg-33.1.2/cg/apps/sequencing_metrics_parser/parsers/bcl2fastq.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/apps/sequencing_metrics_parser/parsers/bcl2fastq_to_sequencing_statistics.py` & `cg-33.1.2/cg/apps/sequencing_metrics_parser/parsers/bcl2fastq_to_sequencing_statistics.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/apps/sequencing_metrics_parser/parsers/bcl_convert.py` & `cg-33.1.2/cg/apps/sequencing_metrics_parser/parsers/bcl_convert.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/apps/sequencing_metrics_parser/parsers/bcl_convert_to_sequencing_statistics.py` & `cg-33.1.2/cg/apps/sequencing_metrics_parser/parsers/bcl_convert_to_sequencing_statistics.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/apps/sequencing_metrics_parser/sequencing_metrics_calculator.py` & `cg-33.1.2/cg/apps/sequencing_metrics_parser/sequencing_metrics_calculator.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/apps/slurm/sbatch.py` & `cg-33.1.2/cg/apps/slurm/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/apps/slurm/slurm_api.py` & `cg-33.1.2/cg/apps/slurm/slurm_api.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/apps/tb/api.py` & `cg-33.1.2/cg/apps/tb/api.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/apps/tb/models.py` & `cg-33.1.2/cg/apps/tb/models.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/apps/vogue.py` & `cg-33.1.2/cg/apps/vogue.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/cli/add.py` & `cg-33.1.2/cg/cli/add.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/cli/backup.py` & `cg-33.1.2/cg/cli/backup.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/cli/base.py` & `cg-33.1.2/cg/cli/base.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/cli/clean.py` & `cg-33.1.2/cg/cli/clean.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/cli/compress/base.py` & `cg-33.1.2/cg/cli/compress/base.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/cli/compress/fastq.py` & `cg-33.1.2/cg/cli/compress/fastq.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/cli/compress/helpers.py` & `cg-33.1.2/cg/cli/compress/helpers.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/cli/delete/base.py` & `cg-33.1.2/cg/cli/delete/base.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/cli/delete/case.py` & `cg-33.1.2/cg/cli/delete/case.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/cli/delete/cases.py` & `cg-33.1.2/cg/cli/delete/cases.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/cli/delete/observations.py` & `cg-33.1.2/cg/cli/delete/observations.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/cli/deliver/base.py` & `cg-33.1.2/cg/cli/deliver/base.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/cli/demultiplex/add.py` & `cg-33.1.2/cg/cli/demultiplex/add.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/cli/demultiplex/base.py` & `cg-33.1.2/cg/cli/demultiplex/base.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/cli/demultiplex/demux.py` & `cg-33.1.2/cg/cli/demultiplex/demux.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/cli/demultiplex/finish.py` & `cg-33.1.2/cg/cli/demultiplex/finish.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/cli/demultiplex/report.py` & `cg-33.1.2/cg/cli/demultiplex/report.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/cli/demultiplex/sample_sheet.py` & `cg-33.1.2/cg/cli/demultiplex/sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/cli/generate/report/base.py` & `cg-33.1.2/cg/cli/generate/report/base.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/cli/generate/report/options.py` & `cg-33.1.2/cg/cli/generate/report/options.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/cli/generate/report/utils.py` & `cg-33.1.2/cg/cli/generate/report/utils.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/cli/get.py` & `cg-33.1.2/cg/cli/get.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/cli/set/base.py` & `cg-33.1.2/cg/cli/set/base.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/cli/set/case.py` & `cg-33.1.2/cg/cli/set/case.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/cli/set/cases.py` & `cg-33.1.2/cg/cli/set/cases.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/cli/store/fastq.py` & `cg-33.1.2/cg/cli/store/fastq.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/cli/store/store.py` & `cg-33.1.2/cg/cli/store/store.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/cli/transfer.py` & `cg-33.1.2/cg/cli/transfer.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/cli/upload/base.py` & `cg-33.1.2/cg/cli/upload/base.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/cli/upload/clinical_delivery.py` & `cg-33.1.2/cg/cli/upload/clinical_delivery.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/cli/upload/coverage.py` & `cg-33.1.2/cg/cli/upload/coverage.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/cli/upload/delivery_report.py` & `cg-33.1.2/cg/cli/upload/delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/cli/upload/fohm.py` & `cg-33.1.2/cg/cli/upload/fohm.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/cli/upload/genotype.py` & `cg-33.1.2/cg/cli/upload/genotype.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/cli/upload/gens.py` & `cg-33.1.2/cg/cli/upload/gens.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/cli/upload/gisaid.py` & `cg-33.1.2/cg/cli/upload/gisaid.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/cli/upload/mutacc.py` & `cg-33.1.2/cg/cli/upload/mutacc.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/cli/upload/nipt/base.py` & `cg-33.1.2/cg/cli/upload/nipt/base.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/cli/upload/nipt/ftp.py` & `cg-33.1.2/cg/cli/upload/nipt/ftp.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/cli/upload/nipt/statina.py` & `cg-33.1.2/cg/cli/upload/nipt/statina.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/cli/upload/observations/observations.py` & `cg-33.1.2/cg/cli/upload/observations/observations.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/cli/upload/observations/utils.py` & `cg-33.1.2/cg/cli/upload/observations/utils.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/cli/upload/scout.py` & `cg-33.1.2/cg/cli/upload/scout.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/cli/upload/utils.py` & `cg-33.1.2/cg/cli/upload/utils.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/cli/upload/validate.py` & `cg-33.1.2/cg/cli/upload/validate.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/cli/upload/vogue.py` & `cg-33.1.2/cg/cli/upload/vogue.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/cli/workflow/balsamic/base.py` & `cg-33.1.2/cg/cli/workflow/balsamic/base.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/cli/workflow/balsamic/options.py` & `cg-33.1.2/cg/cli/workflow/balsamic/options.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/cli/workflow/balsamic/pon.py` & `cg-33.1.2/cg/cli/workflow/balsamic/pon.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/cli/workflow/balsamic/qc.py` & `cg-33.1.2/cg/cli/workflow/balsamic/qc.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/cli/workflow/balsamic/umi.py` & `cg-33.1.2/cg/cli/workflow/balsamic/umi.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/cli/workflow/base.py` & `cg-33.1.2/cg/cli/workflow/base.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/cli/workflow/commands.py` & `cg-33.1.2/cg/cli/workflow/commands.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/cli/workflow/fastq/base.py` & `cg-33.1.2/cg/cli/workflow/fastq/base.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/cli/workflow/fluffy/base.py` & `cg-33.1.2/cg/cli/workflow/fluffy/base.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/cli/workflow/microsalt/base.py` & `cg-33.1.2/cg/cli/workflow/microsalt/base.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/cli/workflow/mip/base.py` & `cg-33.1.2/cg/cli/workflow/mip/base.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/cli/workflow/mip/options.py` & `cg-33.1.2/cg/cli/workflow/mip/options.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/cli/workflow/mip_dna/base.py` & `cg-33.1.2/cg/cli/workflow/mip_dna/base.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/cli/workflow/mip_rna/base.py` & `cg-33.1.2/cg/cli/workflow/mip_rna/base.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/cli/workflow/mutant/base.py` & `cg-33.1.2/cg/cli/workflow/mutant/base.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/cli/workflow/nextflow/options.py` & `cg-33.1.2/cg/cli/workflow/nextflow/options.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/cli/workflow/rnafusion/base.py` & `cg-33.1.2/cg/cli/workflow/rnafusion/base.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/cli/workflow/rnafusion/options.py` & `cg-33.1.2/cg/cli/workflow/rnafusion/options.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/cli/workflow/taxprofiler/base.py` & `cg-33.1.2/cg/cli/workflow/taxprofiler/base.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/cli/workflow/taxprofiler/options.py` & `cg-33.1.2/cg/cli/workflow/taxprofiler/options.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/constants/__init__.py` & `cg-33.1.2/cg/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/constants/bcl_convert_metrics.py` & `cg-33.1.2/cg/constants/bcl_convert_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/constants/compression.py` & `cg-33.1.2/cg/constants/compression.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/constants/constants.py` & `cg-33.1.2/cg/constants/constants.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/constants/delivery.py` & `cg-33.1.2/cg/constants/delivery.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/constants/demultiplexing.py` & `cg-33.1.2/cg/constants/demultiplexing.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/constants/encryption.py` & `cg-33.1.2/cg/constants/encryption.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/constants/gene_panel.py` & `cg-33.1.2/cg/constants/gene_panel.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/constants/housekeeper_tags.py` & `cg-33.1.2/cg/constants/housekeeper_tags.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/constants/lims.py` & `cg-33.1.2/cg/constants/lims.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/constants/nextflow.py` & `cg-33.1.2/cg/constants/nextflow.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/constants/observations.py` & `cg-33.1.2/cg/constants/observations.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/constants/orderforms.py` & `cg-33.1.2/cg/constants/orderforms.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/constants/priority.py` & `cg-33.1.2/cg/constants/priority.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/constants/report.py` & `cg-33.1.2/cg/constants/report.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/constants/rnafusion.py` & `cg-33.1.2/cg/constants/rnafusion.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/constants/scout_upload.py` & `cg-33.1.2/cg/constants/scout_upload.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/constants/sequencing.py` & `cg-33.1.2/cg/constants/sequencing.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/constants/subject.py` & `cg-33.1.2/cg/constants/subject.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/constants/taxprofiler.py` & `cg-33.1.2/cg/constants/taxprofiler.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/exc.py` & `cg-33.1.2/cg/exc.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/io/api.py` & `cg-33.1.2/cg/io/api.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/io/controller.py` & `cg-33.1.2/cg/io/controller.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/io/csv.py` & `cg-33.1.2/cg/io/csv.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/io/json.py` & `cg-33.1.2/cg/io/json.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/io/validate_path.py` & `cg-33.1.2/cg/io/validate_path.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/io/xml.py` & `cg-33.1.2/cg/io/xml.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/io/yaml.py` & `cg-33.1.2/cg/io/yaml.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/archive/ddn_dataflow.py` & `cg-33.1.2/cg/meta/archive/ddn_dataflow.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/backup/backup.py` & `cg-33.1.2/cg/meta/backup/backup.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/backup/pdc.py` & `cg-33.1.2/cg/meta/backup/pdc.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/clean/api.py` & `cg-33.1.2/cg/meta/clean/api.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/clean/demultiplexed_flow_cells.py` & `cg-33.1.2/cg/meta/clean/demultiplexed_flow_cells.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/clean/flow_cell_run_directories.py` & `cg-33.1.2/cg/meta/clean/flow_cell_run_directories.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/compress/compress.py` & `cg-33.1.2/cg/meta/compress/compress.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/compress/files.py` & `cg-33.1.2/cg/meta/compress/files.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/deliver.py` & `cg-33.1.2/cg/meta/deliver.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/deliver_ticket.py` & `cg-33.1.2/cg/meta/deliver_ticket.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/demultiplex/delete_demultiplex_api.py` & `cg-33.1.2/cg/meta/demultiplex/delete_demultiplex_api.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/demultiplex/demux_post_processing.py` & `cg-33.1.2/cg/meta/demultiplex/demux_post_processing.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/demultiplex/files.py` & `cg-33.1.2/cg/meta/demultiplex/files.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/encryption/encryption.py` & `cg-33.1.2/cg/meta/encryption/encryption.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/invoice.py` & `cg-33.1.2/cg/meta/invoice.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/meta.py` & `cg-33.1.2/cg/meta/meta.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/observations/balsamic_observations_api.py` & `cg-33.1.2/cg/meta/observations/balsamic_observations_api.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/observations/mip_dna_observations_api.py` & `cg-33.1.2/cg/meta/observations/mip_dna_observations_api.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/observations/observations_api.py` & `cg-33.1.2/cg/meta/observations/observations_api.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/orders/api.py` & `cg-33.1.2/cg/meta/orders/api.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/orders/case_submitter.py` & `cg-33.1.2/cg/meta/orders/case_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/orders/fastq_submitter.py` & `cg-33.1.2/cg/meta/orders/fastq_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/orders/lims.py` & `cg-33.1.2/cg/meta/orders/lims.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/orders/metagenome_submitter.py` & `cg-33.1.2/cg/meta/orders/metagenome_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/orders/microbial_submitter.py` & `cg-33.1.2/cg/meta/orders/microbial_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/orders/pool_submitter.py` & `cg-33.1.2/cg/meta/orders/pool_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/orders/sars_cov_2_submitter.py` & `cg-33.1.2/cg/meta/orders/sars_cov_2_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/orders/submitter.py` & `cg-33.1.2/cg/meta/orders/submitter.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/orders/ticket_handler.py` & `cg-33.1.2/cg/meta/orders/ticket_handler.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/report/balsamic.py` & `cg-33.1.2/cg/meta/report/balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/report/balsamic_umi.py` & `cg-33.1.2/cg/meta/report/balsamic_umi.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/report/field_validators.py` & `cg-33.1.2/cg/meta/report/field_validators.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/report/mip_dna.py` & `cg-33.1.2/cg/meta/report/mip_dna.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/report/report_api.py` & `cg-33.1.2/cg/meta/report/report_api.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/report/rnafusion.py` & `cg-33.1.2/cg/meta/report/rnafusion.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/report/templates/balsamic_report.html` & `cg-33.1.2/cg/meta/report/templates/balsamic_report.html`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/report/templates/bootstrap.html` & `cg-33.1.2/cg/meta/report/templates/bootstrap.html`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/report/templates/mip-dna_report.html` & `cg-33.1.2/cg/meta/report/templates/mip-dna_report.html`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/rsync/rsync_api.py` & `cg-33.1.2/cg/meta/rsync/rsync_api.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/tar/tar.py` & `cg-33.1.2/cg/meta/tar/tar.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/transfer/external_data.py` & `cg-33.1.2/cg/meta/transfer/external_data.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/transfer/flowcell.py` & `cg-33.1.2/cg/meta/transfer/flowcell.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/transfer/lims.py` & `cg-33.1.2/cg/meta/transfer/lims.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/upload/balsamic/balsamic.py` & `cg-33.1.2/cg/meta/upload/balsamic/balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/upload/coverage.py` & `cg-33.1.2/cg/meta/upload/coverage.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/upload/fohm/fohm.py` & `cg-33.1.2/cg/meta/upload/fohm/fohm.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/upload/gisaid/constants.py` & `cg-33.1.2/cg/meta/upload/gisaid/constants.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/upload/gisaid/gisaid.py` & `cg-33.1.2/cg/meta/upload/gisaid/gisaid.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/upload/gisaid/models.py` & `cg-33.1.2/cg/meta/upload/gisaid/models.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/upload/gt.py` & `cg-33.1.2/cg/meta/upload/gt.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/upload/mip/mip_dna.py` & `cg-33.1.2/cg/meta/upload/mip/mip_dna.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/upload/mip/mip_rna.py` & `cg-33.1.2/cg/meta/upload/mip/mip_rna.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/upload/mutacc.py` & `cg-33.1.2/cg/meta/upload/mutacc.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/upload/nipt/nipt.py` & `cg-33.1.2/cg/meta/upload/nipt/nipt.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/upload/rnafusion/rnafusion.py` & `cg-33.1.2/cg/meta/upload/rnafusion/rnafusion.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/upload/scout/balsamic_config_builder.py` & `cg-33.1.2/cg/meta/upload/scout/balsamic_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/upload/scout/balsamic_umi_config_builder.py` & `cg-33.1.2/cg/meta/upload/scout/balsamic_umi_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/upload/scout/hk_tags.py` & `cg-33.1.2/cg/meta/upload/scout/hk_tags.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/upload/scout/mip_config_builder.py` & `cg-33.1.2/cg/meta/upload/scout/mip_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/upload/scout/rnafusion_config_builder.py` & `cg-33.1.2/cg/meta/upload/scout/rnafusion_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/upload/scout/scout_config_builder.py` & `cg-33.1.2/cg/meta/upload/scout/scout_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/upload/scout/uploadscoutapi.py` & `cg-33.1.2/cg/meta/upload/scout/uploadscoutapi.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/upload/upload_api.py` & `cg-33.1.2/cg/meta/upload/upload_api.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/upload/vogue.py` & `cg-33.1.2/cg/meta/upload/vogue.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/workflow/analysis.py` & `cg-33.1.2/cg/meta/workflow/analysis.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/workflow/balsamic.py` & `cg-33.1.2/cg/meta/workflow/balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/workflow/balsamic_pon.py` & `cg-33.1.2/cg/meta/workflow/balsamic_pon.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/workflow/balsamic_qc.py` & `cg-33.1.2/cg/meta/workflow/balsamic_qc.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/workflow/balsamic_umi.py` & `cg-33.1.2/cg/meta/workflow/balsamic_umi.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/workflow/fastq.py` & `cg-33.1.2/cg/meta/workflow/fastq.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/workflow/fluffy.py` & `cg-33.1.2/cg/meta/workflow/fluffy.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/workflow/microsalt.py` & `cg-33.1.2/cg/meta/workflow/microsalt.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/workflow/mip.py` & `cg-33.1.2/cg/meta/workflow/mip.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/workflow/mip_dna.py` & `cg-33.1.2/cg/meta/workflow/mip_dna.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/workflow/mip_rna.py` & `cg-33.1.2/cg/meta/workflow/mip_rna.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/workflow/mutant.py` & `cg-33.1.2/cg/meta/workflow/mutant.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/workflow/nextflow_common.py` & `cg-33.1.2/cg/meta/workflow/nextflow_common.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/workflow/prepare_fastq.py` & `cg-33.1.2/cg/meta/workflow/prepare_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/workflow/rnafusion.py` & `cg-33.1.2/cg/meta/workflow/rnafusion.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/workflow/taxprofiler.py` & `cg-33.1.2/cg/meta/workflow/taxprofiler.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/meta/workflow/tower_common.py` & `cg-33.1.2/cg/meta/workflow/tower_common.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/models/balsamic/config.py` & `cg-33.1.2/cg/models/balsamic/config.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/models/balsamic/metrics.py` & `cg-33.1.2/cg/models/balsamic/metrics.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/models/cg_config.py` & `cg-33.1.2/cg/models/cg_config.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/models/cgstats/stats_sample.py` & `cg-33.1.2/cg/models/cgstats/stats_sample.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/models/compression_data.py` & `cg-33.1.2/cg/models/compression_data.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/models/deliverables/metric_deliverables.py` & `cg-33.1.2/cg/models/deliverables/metric_deliverables.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/models/demultiplex/demux_results.py` & `cg-33.1.2/cg/models/demultiplex/demux_results.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/models/demultiplex/flow_cell.py` & `cg-33.1.2/cg/models/demultiplex/flow_cell.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,15 +129,15 @@
     def validate_flow_cell_name(self) -> None:
         """
         Validate on the following criteria:
         Convention is: <date>_<machine>_<run_numbers>_<A|B><flow_cell_id>
         Example: '201203_A00689_0200_AHVKJCDRXX'.
         """
         if len(self.split_flow_cell_name) != 4:
-            message = f"Flowcell {self.path.name} does not follow the flow cell naming convention"
+            message = f"Flowcell {self.full_name} does not follow the flow cell naming convention"
             LOG.warning(message)
             raise FlowCellError(message)
 
     def is_demultiplexing_started(self) -> bool:
         """Check if demultiplexing started path exists."""
         return self.demultiplexing_started_path.exists()
```

### Comparing `cg-33.1.1/cg/models/demultiplex/run_parameters.py` & `cg-33.1.2/cg/models/demultiplex/run_parameters.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/models/demultiplex/sbatch.py` & `cg-33.1.2/cg/models/demultiplex/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/models/file_data.py` & `cg-33.1.2/cg/models/file_data.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/models/invoice/invoice.py` & `cg-33.1.2/cg/models/invoice/invoice.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/models/lims/sample.py` & `cg-33.1.2/cg/models/lims/sample.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/models/mip/mip_config.py` & `cg-33.1.2/cg/models/mip/mip_config.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/models/mip/mip_metrics_deliverables.py` & `cg-33.1.2/cg/models/mip/mip_metrics_deliverables.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/models/mip/mip_sample_info.py` & `cg-33.1.2/cg/models/mip/mip_sample_info.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/models/nextflow/deliverables.py` & `cg-33.1.2/cg/models/nextflow/deliverables.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/models/nextflow/sample.py` & `cg-33.1.2/cg/models/nextflow/sample.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/models/observations/input_files.py` & `cg-33.1.2/cg/models/observations/input_files.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/models/orders/constants.py` & `cg-33.1.2/cg/models/orders/constants.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/models/orders/excel_sample.py` & `cg-33.1.2/cg/models/orders/excel_sample.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/models/orders/json_sample.py` & `cg-33.1.2/cg/models/orders/json_sample.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/models/orders/order.py` & `cg-33.1.2/cg/models/orders/order.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/models/orders/orderform_schema.py` & `cg-33.1.2/cg/models/orders/orderform_schema.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/models/orders/sample_base.py` & `cg-33.1.2/cg/models/orders/sample_base.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/models/orders/samples.py` & `cg-33.1.2/cg/models/orders/samples.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/models/report/metadata.py` & `cg-33.1.2/cg/models/report/metadata.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/models/report/report.py` & `cg-33.1.2/cg/models/report/report.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/models/report/sample.py` & `cg-33.1.2/cg/models/report/sample.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/models/report/validators.py` & `cg-33.1.2/cg/models/report/validators.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/models/rnafusion/metrics.py` & `cg-33.1.2/cg/models/rnafusion/metrics.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/models/rnafusion/rnafusion_sample.py` & `cg-33.1.2/cg/models/rnafusion/rnafusion_sample.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/models/scout/scout_load_config.py` & `cg-33.1.2/cg/models/scout/scout_load_config.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/models/slurm/sbatch.py` & `cg-33.1.2/cg/models/slurm/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/models/workflow/mutant.py` & `cg-33.1.2/cg/models/workflow/mutant.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/resources/20181012_Indices.csv` & `cg-33.1.2/cg/resources/20181012_Indices.csv`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/resources/rnafusion_bundle_filenames.csv` & `cg-33.1.2/cg/resources/rnafusion_bundle_filenames.csv`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/server/admin.py` & `cg-33.1.2/cg/server/admin.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/server/api.py` & `cg-33.1.2/cg/server/api.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/server/app.py` & `cg-33.1.2/cg/server/app.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/server/config.py` & `cg-33.1.2/cg/server/config.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/server/ext.py` & `cg-33.1.2/cg/server/ext.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/server/invoices/templates/invoices/index.html` & `cg-33.1.2/cg/server/invoices/templates/invoices/index.html`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/server/invoices/templates/invoices/invoice.html` & `cg-33.1.2/cg/server/invoices/templates/invoices/invoice.html`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/server/invoices/templates/invoices/layout.html` & `cg-33.1.2/cg/server/invoices/templates/invoices/layout.html`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/server/invoices/templates/invoices/new.html` & `cg-33.1.2/cg/server/invoices/templates/invoices/new.html`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/server/invoices/views.py` & `cg-33.1.2/cg/server/invoices/views.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/store/api/add.py` & `cg-33.1.2/cg/store/api/add.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/store/api/base.py` & `cg-33.1.2/cg/store/api/base.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/store/api/core.py` & `cg-33.1.2/cg/store/api/core.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/store/api/delete.py` & `cg-33.1.2/cg/store/api/delete.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/store/api/find_basic_data.py` & `cg-33.1.2/cg/store/api/find_basic_data.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/store/api/find_business_data.py` & `cg-33.1.2/cg/store/api/find_business_data.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/store/api/status.py` & `cg-33.1.2/cg/store/api/status.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/store/filters/status_analysis_filters.py` & `cg-33.1.2/cg/store/filters/status_analysis_filters.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/store/filters/status_application_filters.py` & `cg-33.1.2/cg/store/filters/status_application_filters.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/store/filters/status_application_version_filters.py` & `cg-33.1.2/cg/store/filters/status_application_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/store/filters/status_bed_filters.py` & `cg-33.1.2/cg/store/filters/status_bed_filters.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/store/filters/status_bed_version_filters.py` & `cg-33.1.2/cg/store/filters/status_bed_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/store/filters/status_case_filters.py` & `cg-33.1.2/cg/store/filters/status_case_filters.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/store/filters/status_case_sample_filters.py` & `cg-33.1.2/cg/store/filters/status_case_sample_filters.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/store/filters/status_collaboration_filters.py` & `cg-33.1.2/cg/store/filters/status_collaboration_filters.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/store/filters/status_customer_filters.py` & `cg-33.1.2/cg/store/filters/status_customer_filters.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/store/filters/status_flow_cell_filters.py` & `cg-33.1.2/cg/store/filters/status_flow_cell_filters.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/store/filters/status_invoice_filters.py` & `cg-33.1.2/cg/store/filters/status_invoice_filters.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/store/filters/status_organism_filters.py` & `cg-33.1.2/cg/store/filters/status_organism_filters.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/store/filters/status_panel_filters.py` & `cg-33.1.2/cg/store/filters/status_panel_filters.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/store/filters/status_pool_filters.py` & `cg-33.1.2/cg/store/filters/status_pool_filters.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/store/filters/status_sample_filters.py` & `cg-33.1.2/cg/store/filters/status_sample_filters.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/store/filters/status_user_filters.py` & `cg-33.1.2/cg/store/filters/status_user_filters.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/store/models.py` & `cg-33.1.2/cg/store/models.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/utils/checksum/checksum.py` & `cg-33.1.2/cg/utils/checksum/checksum.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/utils/click/EnumChoice.py` & `cg-33.1.2/cg/utils/click/EnumChoice.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/utils/commands.py` & `cg-33.1.2/cg/utils/commands.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/utils/date.py` & `cg-33.1.2/cg/utils/date.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/utils/dict.py` & `cg-33.1.2/cg/utils/dict.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/utils/dispatcher.py` & `cg-33.1.2/cg/utils/dispatcher.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/utils/email.py` & `cg-33.1.2/cg/utils/email.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/utils/flask/enum.py` & `cg-33.1.2/cg/utils/flask/enum.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg/utils/utils.py` & `cg-33.1.2/cg/utils/utils.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/cg.egg-info/PKG-INFO` & `cg-33.1.2/cg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cg
-Version: 33.1.1
+Version: 33.1.2
 Summary: Clinical Genomics command center
 Home-page: https://github.com/Clinical-Genomics/cg
 Author: Clinical Genomics
 Author-email: support@clinicalgenomics.se
 License: UNKNOWN
 Description: 
         # cg
```

### Comparing `cg-33.1.1/cg.egg-info/SOURCES.txt` & `cg-33.1.2/cg.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -663,19 +663,14 @@
 tests/cli/workflow/rnafusion/test_cli_rnafusion_metrics_deliver.py
 tests/cli/workflow/rnafusion/test_cli_rnafusion_report_deliver.py
 tests/cli/workflow/rnafusion/test_cli_rnafusion_run.py
 tests/cli/workflow/rnafusion/test_cli_rnafusion_store_housekeeper.py
 tests/cli/workflow/taxprofiler/conftest.py
 tests/cli/workflow/taxprofiler/test_cli_taxprofiler_compound_commands.py
 tests/cli/workflow/taxprofiler/test_cli_taxprofiler_config_case.py
-tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/runParameters.xml
-tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/ADM1136A3_XTC08_AGTGGTCA_L001_R1_001.fastq.gz
-tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/ADM1136A3_XTC08_AGTGGTCA_L001_R2_001.fastq.gz
-tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/ADM1136A3_XTC08_AGTGGTCA_L002_R1_001.fastq.gz
-tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/ADM1136A3_XTC08_AGTGGTCA_L002_R2_001.fastq.gz
 tests/fixtures/analysis/sample_coverage.bed
 tests/fixtures/analysis/balsamic/tn_wgs/adm1.cram
 tests/fixtures/analysis/balsamic/tn_wgs/ascat.output.pdf
 tests/fixtures/analysis/balsamic/tn_wgs/snv.vcf
 tests/fixtures/analysis/balsamic/tn_wgs/sv.vcf
 tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json
 tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json
@@ -697,21 +692,14 @@
 tests/fixtures/analysis/rnafusion/multiqc_data.json
 tests/fixtures/apps/balsamic/case/config.json
 tests/fixtures/apps/balsamic/case/metadata.yml
 tests/fixtures/apps/balsamic/case/metadata_directory.yml
 tests/fixtures/apps/balsamic/case/metadata_file_tags.yml
 tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml
 tests/fixtures/apps/crunchy/spring_metadata.json
-tests/fixtures/apps/demultiplexing/RunParameters_different_index_cycles.xml
-tests/fixtures/apps/demultiplexing/SampleSheetS2_Bcl2Fastq.csv
-tests/fixtures/apps/demultiplexing/SampleSheetS2_Dragen.csv
-tests/fixtures/apps/demultiplexing/runParameters_missing_flowcell_run_field.xml
-tests/fixtures/apps/demultiplexing/unknown_run_parameters.xml
-tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml
-tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv
 tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R1_001.fastq.gz
 tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R2_001.fastq.gz
 tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R1_001.fastq.gz
 tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R2_001.fastq.gz
 tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
 tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
 tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
@@ -725,35 +713,35 @@
 tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/Quality_Metrics.csv
 tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/RunInfo.xml
 tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/dummy_run_R1_001.fastq.gz
 tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/dummy_run_R1_001.fastq.gz.md5
 tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R1_001.fastq.gz
 tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R1_001.fastq.gz.md5
 tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R2_001.fastq.gz
-tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/CopyComplete.txt
-tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
-tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/RTAComplete.txt
-tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml
-tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv
-tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/demuxstarted.txt
-tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/CopyComplete.txt
-tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stderr
-tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout
-tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/RTAComplete.txt
-tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml
-tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/SampleSheet.csv
-tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/demuxstarted.txt
-tests/fixtures/apps/demultiplexing/hiseq_run/runParameters.xml
-tests/fixtures/apps/demultiplexing/hiseq_run/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
-tests/fixtures/apps/demultiplexing/hiseq_run/201203_A00689_0200_AHVKJCDRXX/RTAComplete.txt
-tests/fixtures/apps/demultiplexing/hiseq_run/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml
-tests/fixtures/apps/demultiplexing/hiseq_run/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv
-tests/fixtures/apps/demultiplexing/hiseq_run/201203_A00689_0200_AHVKJCDRXX/copycomplete.txt
-tests/fixtures/apps/demultiplexing/hiseq_run/201203_A00689_0200_AHVKJCDRXX/demuxstarted.txt
+tests/fixtures/apps/demultiplexing/flow-cell-runs/hiseq/180522_ST-E00198_0301_BHLCKNCCXY/RTAComplete.txt
+tests/fixtures/apps/demultiplexing/flow-cell-runs/hiseq/180522_ST-E00198_0301_BHLCKNCCXY/SampleSheet.csv
+tests/fixtures/apps/demultiplexing/flow-cell-runs/hiseq/180522_ST-E00198_0301_BHLCKNCCXY/copy_complete.txt
+tests/fixtures/apps/demultiplexing/flow-cell-runs/hiseq/180522_ST-E00198_0301_BHLCKNCCXY/runParameters.xml
+tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/CopyComplete.txt
+tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
+tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/RTAComplete.txt
+tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml
+tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv
+tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/demuxstarted.txt
+tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/CopyComplete.txt
+tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stderr
+tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout
+tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/RTAComplete.txt
+tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml
+tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/SampleSheet.csv
+tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/demuxstarted.txt
+tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_x/20230508_LH00188_0003_A22522YLT3/RunParameters.xml
 tests/fixtures/apps/demultiplexing/raw_lims_samples/raw_samplesheet_novaseq.json
+tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_different_index_cycles.xml
+tests/fixtures/apps/demultiplexing/run_parameters/runParameters_missing_flowcell_run_field.xml
 tests/fixtures/apps/fluffy/SampleSheet.csv
 tests/fixtures/apps/fluffy/deliverables.yaml
 tests/fixtures/apps/fluffy/fluffy_fastq.fastq.gz
 tests/fixtures/apps/fluffy/multiqc_report.html
 tests/fixtures/apps/fluffy/summary.csv
 tests/fixtures/apps/fluffy/2020-23219-05/2020-23219-05.WCXpredict_aberrations.filt.bed
 tests/fixtures/apps/gt/yellowhog.bcf
```

### Comparing `cg-33.1.1/requirements.txt` & `cg-33.1.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/setup.py` & `cg-33.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     with io.open(os.path.join(HERE, "README.md"), encoding="utf-8") as f:
         LONG_DESCRIPTION = "\n" + f.read()
 except FileNotFoundError:
     LONG_DESCRIPTION = DESCRIPTION
 
 setup(
     name=NAME,
-    version="33.1.1",
+    version="33.1.2",
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     author=AUTHOR,
     author_email=EMAIL,
     url=URL,
     include_package_data=True,
```

### Comparing `cg-33.1.1/tests/apps/cgstats/conftest.py` & `cg-33.1.2/tests/apps/cgstats/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/apps/cgstats/crud/test_create_novaseq.py` & `cg-33.1.2/tests/apps/cgstats/crud/test_create_novaseq.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/apps/cgstats/crud/test_delete.py` & `cg-33.1.2/tests/apps/cgstats/crud/test_delete.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/apps/cgstats/parsers/test_conversion_stats.py` & `cg-33.1.2/tests/apps/cgstats/parsers/test_conversion_stats.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/apps/cgstats/parsers/test_demux_stats.py` & `cg-33.1.2/tests/apps/cgstats/parsers/test_demux_stats.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/apps/cgstats/parsers/test_run_info.py` & `cg-33.1.2/tests/apps/cgstats/parsers/test_run_info.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/apps/cgstats/test_cgstats_create.py` & `cg-33.1.2/tests/apps/cgstats/test_cgstats_create.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/apps/cgstats/test_stats.py` & `cg-33.1.2/tests/apps/cgstats/test_stats.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/apps/conftest.py` & `cg-33.1.2/tests/apps/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/apps/coverage/test_coverage.py` & `cg-33.1.2/tests/apps/coverage/test_coverage.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/apps/crunchy/conftest.py` & `cg-33.1.2/tests/apps/crunchy/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/apps/crunchy/test_compress_fastq.py` & `cg-33.1.2/tests/apps/crunchy/test_compress_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/apps/crunchy/test_config.py` & `cg-33.1.2/tests/apps/crunchy/test_config.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/apps/crunchy/test_crunchy.py` & `cg-33.1.2/tests/apps/crunchy/test_crunchy.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/apps/crunchy/test_spring_decompression.py` & `cg-33.1.2/tests/apps/crunchy/test_spring_decompression.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/apps/demultiplex/conftest.py` & `cg-33.1.2/tests/apps/demultiplex/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/apps/demultiplex/test_convert_to_sample_sheet.py` & `cg-33.1.2/tests/apps/demultiplex/test_convert_to_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/apps/demultiplex/test_demultiplex_api.py` & `cg-33.1.2/tests/apps/demultiplex/test_demultiplex_api.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/apps/demultiplex/test_sample_sheet.py` & `cg-33.1.2/tests/apps/demultiplex/test_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/apps/demultiplex/test_validate_sample_sheet.py` & `cg-33.1.2/tests/apps/demultiplex/test_validate_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/apps/gens/test_gens_api.py` & `cg-33.1.2/tests/apps/gens/test_gens_api.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/apps/gt/conftest.py` & `cg-33.1.2/tests/apps/gt/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/apps/gt/test_gt_api.py` & `cg-33.1.2/tests/apps/gt/test_gt_api.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/apps/hk/conftest.py` & `cg-33.1.2/tests/apps/hk/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/apps/hk/test__getattr__.py` & `cg-33.1.2/tests/apps/hk/test__getattr__.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/apps/hk/test_add_file.py` & `cg-33.1.2/tests/apps/hk/test_add_file.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/apps/hk/test_bundles.py` & `cg-33.1.2/tests/apps/hk/test_bundles.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/apps/hk/test_core.py` & `cg-33.1.2/tests/apps/hk/test_core.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/apps/hk/test_file.py` & `cg-33.1.2/tests/apps/hk/test_file.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/apps/hk/test_version.py` & `cg-33.1.2/tests/apps/hk/test_version.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/apps/lims/conftest.py` & `cg-33.1.2/tests/apps/lims/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/apps/lims/test_api.py` & `cg-33.1.2/tests/apps/lims/test_api.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/apps/lims/test_sample_sheet.py` & `cg-33.1.2/tests/apps/lims/test_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/apps/loqus/conftest.py` & `cg-33.1.2/tests/apps/loqus/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/apps/loqus/test_loqusdb_api.py` & `cg-33.1.2/tests/apps/loqus/test_loqusdb_api.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/apps/madeline/conftest.py` & `cg-33.1.2/tests/apps/madeline/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/apps/madeline/test_madeline.py` & `cg-33.1.2/tests/apps/madeline/test_madeline.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/apps/mip/conftest.py` & `cg-33.1.2/tests/apps/mip/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/apps/mip/test_config_mip.py` & `cg-33.1.2/tests/apps/mip/test_config_mip.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/apps/mutacc_auto/conftest.py` & `cg-33.1.2/tests/apps/mutacc_auto/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/apps/mutacc_auto/test_mutacc_auto.py` & `cg-33.1.2/tests/apps/mutacc_auto/test_mutacc_auto.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/apps/orderform/conftest.py` & `cg-33.1.2/tests/apps/orderform/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/apps/orderform/test_excel_orderform_parser.py` & `cg-33.1.2/tests/apps/orderform/test_excel_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/apps/orderform/test_excel_sample_schema.py` & `cg-33.1.2/tests/apps/orderform/test_excel_sample_schema.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/apps/orderform/test_json_orderform_parser.py` & `cg-33.1.2/tests/apps/orderform/test_json_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/apps/orderform/test_orderform_parser.py` & `cg-33.1.2/tests/apps/orderform/test_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/apps/scout/conftest.py` & `cg-33.1.2/tests/apps/scout/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/apps/scout/test_get_causative_variants.py` & `cg-33.1.2/tests/apps/scout/test_get_causative_variants.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/apps/scout/test_get_scout_cases.py` & `cg-33.1.2/tests/apps/scout/test_get_scout_cases.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/apps/scout/test_scout_load_config.py` & `cg-33.1.2/tests/apps/scout/test_scout_load_config.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/apps/scout/test_scout_models.py` & `cg-33.1.2/tests/apps/scout/test_scout_models.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/apps/sequencing_metrics_parser/conftest.py` & `cg-33.1.2/tests/apps/sequencing_metrics_parser/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/apps/sequencing_metrics_parser/parsers/conftest.py` & `cg-33.1.2/tests/apps/sequencing_metrics_parser/parsers/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/apps/sequencing_metrics_parser/parsers/test_bcl2fastq_parser.py` & `cg-33.1.2/tests/apps/sequencing_metrics_parser/parsers/test_bcl2fastq_parser.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/apps/sequencing_metrics_parser/parsers/test_bcl_convert_to_sequencing_statistics.py` & `cg-33.1.2/tests/apps/sequencing_metrics_parser/parsers/test_bcl_convert_to_sequencing_statistics.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/apps/sequencing_metrics_parser/parsers/test_bclconvert.py` & `cg-33.1.2/tests/apps/sequencing_metrics_parser/parsers/test_bclconvert.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/apps/sequencing_metrics_parser/test_sequencing_metrics_calculator.py` & `cg-33.1.2/tests/apps/sequencing_metrics_parser/test_sequencing_metrics_calculator.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/apps/slurm/conftest.py` & `cg-33.1.2/tests/apps/slurm/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/apps/slurm/test_slurm_api.py` & `cg-33.1.2/tests/apps/slurm/test_slurm_api.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/apps/test_apps_environ.py` & `cg-33.1.2/tests/apps/test_apps_environ.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/apps/test_osticket.py` & `cg-33.1.2/tests/apps/test_osticket.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/apps/vogue/conftest.py` & `cg-33.1.2/tests/apps/vogue/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/apps/vogue/test_vogue_api.py` & `cg-33.1.2/tests/apps/vogue/test_vogue_api.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/add/test_cli_add.py` & `cg-33.1.2/tests/cli/add/test_cli_add.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/add/test_cli_add_customer.py` & `cg-33.1.2/tests/cli/add/test_cli_add_customer.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/add/test_cli_add_family.py` & `cg-33.1.2/tests/cli/add/test_cli_add_family.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/add/test_cli_add_relationship.py` & `cg-33.1.2/tests/cli/add/test_cli_add_relationship.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/add/test_cli_add_sample.py` & `cg-33.1.2/tests/cli/add/test_cli_add_sample.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/backup/conftest.py` & `cg-33.1.2/tests/cli/backup/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/backup/test_backup_command.py` & `cg-33.1.2/tests/cli/backup/test_backup_command.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/clean/conftest.py` & `cg-33.1.2/tests/cli/clean/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/clean/test_balsamic_clean.py` & `cg-33.1.2/tests/cli/clean/test_balsamic_clean.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/clean/test_clean_hk_bundle_files.py` & `cg-33.1.2/tests/cli/clean/test_clean_hk_bundle_files.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/clean/test_hk_bundle_files.py` & `cg-33.1.2/tests/cli/clean/test_hk_bundle_files.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/clean/test_hk_case_bundle_files.py` & `cg-33.1.2/tests/cli/clean/test_hk_case_bundle_files.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/clean/test_microbial_clean.py` & `cg-33.1.2/tests/cli/clean/test_microbial_clean.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/clean/test_rsync_past_run_dirs.py` & `cg-33.1.2/tests/cli/clean/test_rsync_past_run_dirs.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/compress/conftest.py` & `cg-33.1.2/tests/cli/compress/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/compress/test_cli_compress_fastq.py` & `cg-33.1.2/tests/cli/compress/test_cli_compress_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/compress/test_cli_decompress_spring.py` & `cg-33.1.2/tests/cli/compress/test_cli_decompress_spring.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/compress/test_compress_helpers.py` & `cg-33.1.2/tests/cli/compress/test_compress_helpers.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/compress/test_store_fastq.py` & `cg-33.1.2/tests/cli/compress/test_store_fastq.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     # THEN assert the program exits with 2 since no argument was provided
     assert res.exit_code == 2
 
 
 def test_store_fastq_cli_non_existing_family(
     compress_context: CGConfig, cli_runner: CliRunner, caplog
 ):
-    """Test to run the compress command with a non existing case"""
+    """Test to run the compress command with a non-existing case"""
     caplog.set_level(logging.DEBUG)
     # GIVEN a context and a non existing case id
     case_id = "happychap"
 
     # WHEN running the store fastq command
     res = cli_runner.invoke(store_case, [case_id], obj=compress_context)
```

### Comparing `cg-33.1.1/tests/cli/conftest.py` & `cg-33.1.2/tests/cli/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/delete/test_cli_delete_case.py` & `cg-33.1.2/tests/cli/delete/test_cli_delete_case.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/delete/test_cli_delete_cases.py` & `cg-33.1.2/tests/cli/delete/test_cli_delete_cases.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/deliver/conftest.py` & `cg-33.1.2/tests/cli/deliver/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/deliver/test_deliver_base.py` & `cg-33.1.2/tests/cli/deliver/test_deliver_base.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/deliver/test_rsync_base.py` & `cg-33.1.2/tests/cli/deliver/test_rsync_base.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/deliver/test_run_deliver_cmd.py` & `cg-33.1.2/tests/cli/deliver/test_run_deliver_cmd.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/demultiplex/conftest.py` & `cg-33.1.2/tests/cli/demultiplex/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     """Return the path to a dir with demultiplexing results where demux has been done but nothing is cleaned."""
     return Path(demultiplex_fixtures, "demultiplexed-runs-unfinished")
 
 
 @pytest.fixture(name="flow_cell_runs_working_directory")
 def fixture_flow_cell_runs_working_directory(project_dir: Path) -> Path:
     """Return the path to a working directory with flow cells ready for demux."""
-    working_dir: Path = Path(project_dir, "flow-cell-runs")
+    working_dir: Path = Path(project_dir, "flow-cell-runs", "nova_seq_6000")
     working_dir.mkdir(parents=True)
     return working_dir
 
 
 @pytest.fixture(name="flow_cell_runs_working_directory_bcl2fastq")
 def fixture_flow_cell_runs_working_directory_bcl2fastq(
     flow_cell_runs_working_directory: Path,
@@ -269,12 +269,12 @@
 @pytest.fixture(name="demultiplex_context")
 def fixture_demultiplex_context(
     demultiplexing_api: DemultiplexingAPI,
     stats_api: StatsAPI,
     real_housekeeper_api: HousekeeperAPI,
     cg_context: CGConfig,
 ) -> CGConfig:
-    """Return cg context witha demultiplex context."""
+    """Return cg context with a demultiplex context."""
     cg_context.demultiplex_api_ = demultiplexing_api
     cg_context.cg_stats_api_ = stats_api
     cg_context.housekeeper_api_ = real_housekeeper_api
     return cg_context
```

### Comparing `cg-33.1.1/tests/cli/demultiplex/test_add_flowcell.py` & `cg-33.1.2/tests/cli/demultiplex/test_add_flowcell.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/demultiplex/test_create_sample_sheet.py` & `cg-33.1.2/tests/cli/demultiplex/test_create_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/demultiplex/test_demultiplex_flowcell.py` & `cg-33.1.2/tests/cli/demultiplex/test_demultiplex_flowcell.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,20 +160,22 @@
     assert demux_dir.exists()
     assert unaligned_dir.exists()
 
     # THEN assert that the sbatch script was created
     assert demux_api.demultiplex_sbatch_path(flow_cell).exists()
 
 
-def test_demultiplex_all(
+def test_demultiplex_all_novaseq(
     cli_runner: testing.CliRunner,
     demultiplex_context: CGConfig,
     demultiplex_ready_flow_cell: Path,
     caplog,
 ):
+    """Test the demultiplex-all command on a directory with newly sequenced NovaSeq6000 flow cells."""
+
     caplog.set_level(logging.INFO)
 
     # GIVEN a context with the path to a directory where at least one flowcell is ready for demux
     demux_api: DemultiplexingAPI = demultiplex_context.demultiplex_api
     flow_cell: FlowCell = FlowCell(flow_cell_path=demultiplex_ready_flow_cell)
 
     assert demux_api.run_dir == demultiplex_ready_flow_cell.parent
```

### Comparing `cg-33.1.1/tests/cli/demultiplex/test_finish_demux.py` & `cg-33.1.2/tests/cli/demultiplex/test_finish_demux.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/demultiplex/test_stats_command.py` & `cg-33.1.2/tests/cli/demultiplex/test_stats_command.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/demultiplex/test_validate_sample_sheet.py` & `cg-33.1.2/tests/cli/demultiplex/test_validate_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/generate/report/conftest.py` & `cg-33.1.2/tests/cli/generate/report/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/generate/report/test_cli_delivery_report.py` & `cg-33.1.2/tests/cli/generate/report/test_cli_delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/generate/report/test_utils.py` & `cg-33.1.2/tests/cli/generate/report/test_utils.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/generate/test_cli_base.py` & `cg-33.1.2/tests/cli/generate/test_cli_base.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/get/test_cli_get.py` & `cg-33.1.2/tests/cli/get/test_cli_get.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/get/test_cli_get_analysis.py` & `cg-33.1.2/tests/cli/get/test_cli_get_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/get/test_cli_get_case.py` & `cg-33.1.2/tests/cli/get/test_cli_get_case.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/get/test_cli_get_flow_cell.py` & `cg-33.1.2/tests/cli/get/test_cli_get_flow_cell.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/get/test_cli_get_sample.py` & `cg-33.1.2/tests/cli/get/test_cli_get_sample.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/set/conftest.py` & `cg-33.1.2/tests/cli/set/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/set/test_cli_set_case.py` & `cg-33.1.2/tests/cli/set/test_cli_set_case.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/set/test_cli_set_cases.py` & `cg-33.1.2/tests/cli/set/test_cli_set_cases.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/set/test_cli_set_flowcell.py` & `cg-33.1.2/tests/cli/set/test_cli_set_flowcell.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/set/test_cli_set_list_keys.py` & `cg-33.1.2/tests/cli/set/test_cli_set_list_keys.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/set/test_cli_set_sample.py` & `cg-33.1.2/tests/cli/set/test_cli_set_sample.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/set/test_cli_set_samples.py` & `cg-33.1.2/tests/cli/set/test_cli_set_samples.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/store/test_fastq.py` & `cg-33.1.2/tests/cli/store/test_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/test_base.py` & `cg-33.1.2/tests/cli/test_base.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/test_clean.py` & `cg-33.1.2/tests/cli/test_clean.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/upload/conftest.py` & `cg-33.1.2/tests/cli/upload/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/upload/test_cli_scout.py` & `cg-33.1.2/tests/cli/upload/test_cli_scout.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/upload/test_cli_upload.py` & `cg-33.1.2/tests/cli/upload/test_cli_upload.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/upload/test_cli_upload_auto.py` & `cg-33.1.2/tests/cli/upload/test_cli_upload_auto.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/upload/test_cli_upload_delivery_report.py` & `cg-33.1.2/tests/cli/upload/test_cli_upload_delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/upload/test_cli_upload_fastq.py` & `cg-33.1.2/tests/cli/upload/test_cli_upload_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/upload/test_cli_upload_genotype.py` & `cg-33.1.2/tests/cli/upload/test_cli_upload_genotype.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/upload/test_cli_upload_gens.py` & `cg-33.1.2/tests/cli/upload/test_cli_upload_gens.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/upload/test_cli_upload_nipt.py` & `cg-33.1.2/tests/cli/upload/test_cli_upload_nipt.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/upload/test_cli_upload_nipt_ftp.py` & `cg-33.1.2/tests/cli/upload/test_cli_upload_nipt_ftp.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/upload/test_cli_upload_nipt_statina.py` & `cg-33.1.2/tests/cli/upload/test_cli_upload_nipt_statina.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/upload/test_cli_upload_observations.py` & `cg-33.1.2/tests/cli/upload/test_cli_upload_observations.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/upload/test_cli_upload_vogue.py` & `cg-33.1.2/tests/cli/upload/test_cli_upload_vogue.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/workflow/balsamic/conftest.py` & `cg-33.1.2/tests/cli/workflow/balsamic/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py` & `cg-33.1.2/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/workflow/balsamic/test_compound_commands.py` & `cg-33.1.2/tests/cli/workflow/balsamic/test_compound_commands.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/workflow/balsamic/test_link.py` & `cg-33.1.2/tests/cli/workflow/balsamic/test_link.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/workflow/balsamic/test_report_deliver.py` & `cg-33.1.2/tests/cli/workflow/balsamic/test_report_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/workflow/balsamic/test_run.py` & `cg-33.1.2/tests/cli/workflow/balsamic/test_run.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/workflow/balsamic/test_store_housekeeper.py` & `cg-33.1.2/tests/cli/workflow/balsamic/test_store_housekeeper.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/workflow/conftest.py` & `cg-33.1.2/tests/cli/workflow/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/workflow/fastq/test_fastq_base.py` & `cg-33.1.2/tests/cli/workflow/fastq/test_fastq_base.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/workflow/fluffy/conftest.py` & `cg-33.1.2/tests/cli/workflow/fluffy/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py` & `cg-33.1.2/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/workflow/fluffy/test_cli_link.py` & `cg-33.1.2/tests/cli/workflow/fluffy/test_cli_link.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/workflow/fluffy/test_cli_run.py` & `cg-33.1.2/tests/cli/workflow/fluffy/test_cli_run.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/workflow/fluffy/test_cli_start.py` & `cg-33.1.2/tests/cli/workflow/fluffy/test_cli_start.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/workflow/fluffy/test_cli_store.py` & `cg-33.1.2/tests/cli/workflow/fluffy/test_cli_store.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/workflow/microsalt/conftest.py` & `cg-33.1.2/tests/cli/workflow/microsalt/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/workflow/microsalt/snapshots/snap_test_microsalt_case_config.py` & `cg-33.1.2/tests/cli/workflow/microsalt/snapshots/snap_test_microsalt_case_config.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/workflow/microsalt/test_microsalt_case_config.py` & `cg-33.1.2/tests/cli/workflow/microsalt/test_microsalt_case_config.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/workflow/microsalt/test_microsalt_run.py` & `cg-33.1.2/tests/cli/workflow/microsalt/test_microsalt_run.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/workflow/mip/conftest.py` & `cg-33.1.2/tests/cli/workflow/mip/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/workflow/mip/test_cli_mip_base.py` & `cg-33.1.2/tests/cli/workflow/mip/test_cli_mip_base.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py` & `cg-33.1.2/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/workflow/mip/test_cli_mip_dna_run.py` & `cg-33.1.2/tests/cli/workflow/mip/test_cli_mip_dna_run.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/workflow/mip/test_cli_mip_dna_start.py` & `cg-33.1.2/tests/cli/workflow/mip/test_cli_mip_dna_start.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py` & `cg-33.1.2/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/workflow/mip/test_cli_mip_rna_link.py` & `cg-33.1.2/tests/cli/workflow/mip/test_cli_mip_rna_link.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/workflow/mip/test_cli_mip_rna_run.py` & `cg-33.1.2/tests/cli/workflow/mip/test_cli_mip_rna_run.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/workflow/mip/test_cli_mip_store.py` & `cg-33.1.2/tests/cli/workflow/mip/test_cli_mip_store.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/workflow/rnafusion/test_cli_rnafusion_compound_commands.py` & `cg-33.1.2/tests/cli/workflow/rnafusion/test_cli_rnafusion_compound_commands.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/workflow/rnafusion/test_cli_rnafusion_config_case.py` & `cg-33.1.2/tests/cli/workflow/rnafusion/test_cli_rnafusion_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/workflow/rnafusion/test_cli_rnafusion_metrics_deliver.py` & `cg-33.1.2/tests/cli/workflow/rnafusion/test_cli_rnafusion_metrics_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/workflow/rnafusion/test_cli_rnafusion_report_deliver.py` & `cg-33.1.2/tests/cli/workflow/rnafusion/test_cli_rnafusion_report_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/workflow/rnafusion/test_cli_rnafusion_run.py` & `cg-33.1.2/tests/cli/workflow/rnafusion/test_cli_rnafusion_run.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/workflow/rnafusion/test_cli_rnafusion_store_housekeeper.py` & `cg-33.1.2/tests/cli/workflow/rnafusion/test_cli_rnafusion_store_housekeeper.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/workflow/taxprofiler/conftest.py` & `cg-33.1.2/tests/cli/workflow/taxprofiler/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/workflow/taxprofiler/test_cli_taxprofiler_compound_commands.py` & `cg-33.1.2/tests/cli/workflow/taxprofiler/test_cli_taxprofiler_compound_commands.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/workflow/taxprofiler/test_cli_taxprofiler_config_case.py` & `cg-33.1.2/tests/cli/workflow/taxprofiler/test_cli_taxprofiler_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/workflow/test_cli_workflow.py` & `cg-33.1.2/tests/cli/workflow/test_cli_workflow.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/cli/workflow/test_cli_workflow_clean.py` & `cg-33.1.2/tests/cli/workflow/test_cli_workflow_clean.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/conftest.py` & `cg-33.1.2/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -507,15 +507,15 @@
 def tmp_file(project_dir) -> Path:
     """Return a temp file path."""
     return Path(project_dir, "test")
 
 
 @pytest.fixture(name="non_existing_file_path")
 def fixture_non_existing_file_path(project_dir: Path) -> Path:
-    """Return the path to a non existing file."""
+    """Return the path to a non-existing file."""
     return Path(project_dir, "a_file.txt")
 
 
 @pytest.fixture(name="content", scope="session")
 def fixture_content() -> str:
     """Return some content for a file."""
     return (
@@ -701,120 +701,142 @@
         shutil.copy(original_file, working_file)
     return working_files
 
 
 # Demultiplex fixtures
 
 
-@pytest.fixture(name="demultiplex_fixtures")
+@pytest.fixture(name="demultiplex_fixtures", scope="session")
 def fixture_demultiplex_fixtures(apps_dir: Path) -> Path:
-    """Return the path to the demultiplex fixtures."""
+    """Return the path to the demultiplex fixture directory."""
     return Path(apps_dir, "demultiplexing")
 
 
-@pytest.fixture(name="novaseq_bcl2fastq_sample_sheet_path")
-def fixture_novaseq_bcl2fastq_sample_sheet_path(demultiplex_fixtures: Path) -> Path:
-    """Return the path to a Novaseq bcl2fastq sample sheet."""
-    return Path(demultiplex_fixtures, "SampleSheetS2_Bcl2Fastq.csv")
-
-
-@pytest.fixture(name="novaseq_dragen_sample_sheet_path")
-def fixture_novaseq_dragen_sample_sheet_path(demultiplex_fixtures: Path) -> Path:
-    """Return the path to a Novaseq dragen sample sheet."""
-    return Path(demultiplex_fixtures, "SampleSheetS2_Dragen.csv")
-
-
-@pytest.fixture(name="raw_lims_sample_dir")
+@pytest.fixture(name="raw_lims_sample_dir", scope="session")
 def fixture_raw_lims_sample_dir(demultiplex_fixtures: Path) -> Path:
-    """Return the path to the raw samples fixtures."""
+    """Return the path to the raw samples fixture directory."""
     return Path(demultiplex_fixtures, "raw_lims_samples")
 
 
-@pytest.fixture(name="demultiplexed_runs")
+@pytest.fixture(name="run_parameters_dir", scope="session")
+def fixture_run_parameters_dir(demultiplex_fixtures: Path) -> Path:
+    """Return the path to the run parameters fixture directory."""
+    return Path(demultiplex_fixtures, "run_parameters")
+
+
+@pytest.fixture(name="demultiplexed_runs", scope="session")
 def fixture_demultiplexed_runs(demultiplex_fixtures: Path) -> Path:
-    """Return the path to a dir with flow cells ready for demultiplexing."""
+    """Return the path to the demultiplexed flow cells fixture directory."""
     return Path(demultiplex_fixtures, "demultiplexed-runs")
 
 
-@pytest.fixture(name="flow_cell_runs_dir")
+@pytest.fixture(name="flow_cell_runs_dir", scope="session")
 def fixture_demux_run_dir(demultiplex_fixtures: Path) -> Path:
-    """Return the path to a dir with flow cells ready for demultiplexing."""
+    """Return the path to the sequenced flow cells fixture directory."""
     return Path(demultiplex_fixtures, "flow-cell-runs")
 
 
-@pytest.fixture(name="bcl2fastq_flow_cell_dir")
+@pytest.fixture(name="hiseq_dir", scope="session")
+def fixture_hiseq_dir(flow_cell_runs_dir: Path) -> Path:
+    """Return the path to the hiseq sequencing fixture directory."""
+    return Path(flow_cell_runs_dir, "hiseq")
+
+
+@pytest.fixture(name="novaseq_6000_dir", scope="session")
+def fixture_novaseq_6000_dir(flow_cell_runs_dir: Path) -> Path:
+    """Return the path to the NovaSeq6000 sequencing fixture directory."""
+    return Path(flow_cell_runs_dir, "nova_seq_6000")
+
+
+@pytest.fixture(name="novaseq_x_dir", scope="session")
+def fixture_novaseq_x_dir(flow_cell_runs_dir: Path) -> Path:
+    """Return the path to the NovaSeqX sequencing fixture directory."""
+    return Path(flow_cell_runs_dir, "nova_seq_x")
+
+
+@pytest.fixture(name="bcl2fastq_flow_cell_full_name", scope="session")
+def fixture_flow_cell_full_name() -> str:
+    """Return full flow cell name."""
+    return "201203_A00689_0200_AHVKJCDRXX"
+
+
+@pytest.fixture(name="dragen_flow_cell_full_name", scope="session")
+def fixture_dragen_flow_cell_full_name() -> str:
+    """Return the full name of a dragen flow cell."""
+    return "211101_A00187_0615_AHLG5GDRXY"
+
+
+@pytest.fixture(name="bcl2fastq_flow_cell_dir", scope="session")
 def fixture_bcl2fastq_flow_cell_dir(
-    flow_cell_runs_dir: Path, bcl2fastq_flow_cell_full_name: str
+    novaseq_6000_dir: Path, bcl2fastq_flow_cell_full_name: str
 ) -> Path:
     """Return the path to the bcl2fastq flow cell demultiplex fixture directory."""
-    return Path(flow_cell_runs_dir, bcl2fastq_flow_cell_full_name)
+    return Path(novaseq_6000_dir, bcl2fastq_flow_cell_full_name)
 
 
-@pytest.fixture(name="dragen_flow_cell_dir")
-def fixture_dragen_flow_cell_path(
-    flow_cell_runs_dir: Path, dragen_flow_cell_full_name: str
-) -> Path:
+@pytest.fixture(name="dragen_flow_cell_dir", scope="session")
+def fixture_dragen_flow_cell_path(novaseq_6000_dir: Path, dragen_flow_cell_full_name: str) -> Path:
     """Return the path to the dragen flow cell demultiplex fixture directory."""
-    return Path(flow_cell_runs_dir, dragen_flow_cell_full_name)
+    return Path(novaseq_6000_dir, dragen_flow_cell_full_name)
+
 
+@pytest.fixture(name="novaseq_bcl2fastq_sample_sheet_path", scope="session")
+def fixture_novaseq_bcl2fastq_sample_sheet_path(bcl2fastq_flow_cell_dir: Path) -> Path:
+    """Return the path to a NovaSeq6000 Bcl2fastq sample sheet."""
+    return Path(bcl2fastq_flow_cell_dir, "SampleSheet.csv")
 
-@pytest.fixture(name="hiseq_dir")
-def fixture_hiseq_dir(demultiplex_fixtures: Path) -> Path:
-    """Return the path to the hiseq demultiplex fixtures."""
-    return Path(demultiplex_fixtures, "hiseq_run")
 
+@pytest.fixture(name="novaseq_dragen_sample_sheet_path", scope="session")
+def fixture_novaseq_dragen_sample_sheet_path(dragen_flow_cell_dir: Path) -> Path:
+    """Return the path to a NovaSeq6000 dragen sample sheet."""
+    return Path(dragen_flow_cell_dir, "SampleSheet.csv")
 
-@pytest.fixture(name="run_parameters_missing_flowcell_type")
-def fixture_run_parameters_missing_flowcell_type(demultiplex_fixtures: Path) -> Path:
+
+@pytest.fixture(name="run_parameters_missing_flowcell_type", scope="session")
+def fixture_run_parameters_missing_flowcell_type(run_parameters_dir: Path) -> Path:
     """Return the path to a file with hiseq run parameters without flow cell."""
-    return Path(demultiplex_fixtures, "runParameters_missing_flowcell_run_field.xml")
+    return Path(run_parameters_dir, "runParameters_missing_flowcell_run_field.xml")
 
 
-@pytest.fixture(name="novaseq_run_parameters")
+@pytest.fixture(name="novaseq_run_parameters", scope="session")
 def fixture_novaseq_run_parameters(bcl2fastq_flow_cell_dir: Path) -> Path:
-    """Return the path to a file with novaseq run parameters."""
+    """Return the path to a file with NovaSeq6000 run parameters."""
     return Path(bcl2fastq_flow_cell_dir, "RunParameters.xml")
 
 
-@pytest.fixture(name="run_parameters_different_index")
-def fixture_run_parameters_different_index(demultiplex_fixtures: Path) -> Path:
+@pytest.fixture(name="run_parameters_different_index", scope="session")
+def fixture_run_parameters_different_index(run_parameters_dir: Path) -> Path:
     """Return the path to a file with novaseq run parameters with different index cycles."""
-    return Path(demultiplex_fixtures, "RunParameters_different_index_cycles.xml")
+    return Path(run_parameters_dir, "RunParameters_different_index_cycles.xml")
 
 
-@pytest.fixture(name="bcl2fastq_flow_cell")
-def fixture_flow_cell(bcl2fastq_flow_cell_dir: str) -> FlowCell:
+@pytest.fixture(name="bcl2fastq_flow_cell", scope="session")
+def fixture_flow_cell(bcl2fastq_flow_cell_dir: Path) -> FlowCell:
     """Create a flow cell object with flow cell that is demultiplexed."""
     return FlowCell(flow_cell_path=bcl2fastq_flow_cell_dir)
 
 
-@pytest.fixture(name="dragen_flow_cell")
-def fixture_dragen_flow_cell(dragen_flow_cell_dir: str) -> FlowCell:
+@pytest.fixture(name="dragen_flow_cell", scope="session")
+def fixture_dragen_flow_cell(dragen_flow_cell_dir: Path) -> FlowCell:
     """Create a dragen flow cell object with flow cell that is demultiplexed."""
     return FlowCell(flow_cell_path=dragen_flow_cell_dir)
 
 
-@pytest.fixture(name="bcl2fastq_flow_cell_id")
+@pytest.fixture(name="bcl2fastq_flow_cell_id", scope="session")
 def fixture_bcl2fast2_flow_cell_id(bcl2fastq_flow_cell: FlowCell) -> str:
     """Return flow cell id from bcl2fastq flow cell object."""
     return bcl2fastq_flow_cell.id
 
 
-@pytest.fixture(name="dragen_flow_cell_id")
+@pytest.fixture(name="dragen_flow_cell_id", scope="session")
 def fixture_dragen_flow_cell_id(dragen_flow_cell: FlowCell) -> str:
     """Return flow cell id from dragen flow cell object."""
     return dragen_flow_cell.id
 
 
-@pytest.fixture(name="another_flow_cell_id")
-def fixture_another_flow_cell_id() -> str:
-    """Return another flow cell id."""
-    return "HF57HDRXY"
-
-
 @pytest.fixture(name="demultiplexing_delivery_file")
 def fixture_demultiplexing_delivery_file(bcl2fastq_flow_cell: FlowCell) -> Path:
     """Return demultiplexing delivery started file."""
     return Path(bcl2fastq_flow_cell.path, DemultiplexingDirsAndFiles.DELIVERY)
 
 
 @pytest.fixture(name="hiseq_x_tile_dir")
@@ -833,26 +855,14 @@
 def fixture_lims_novaseq_samples_raw(lims_novaseq_samples_file: Path) -> List[dict]:
     """Return a list of raw flow cell samples."""
     return ReadFile.get_content_from_file(
         file_format=FileFormat.JSON, file_path=lims_novaseq_samples_file
     )
 
 
-@pytest.fixture(name="bcl2fastq_flow_cell_full_name")
-def fixture_flow_cell_full_name() -> str:
-    """Return full flow cell name."""
-    return "201203_A00689_0200_AHVKJCDRXX"
-
-
-@pytest.fixture(name="dragen_flow_cell_full_name")
-def fixture_dragen_flow_cell_full_name() -> str:
-    """Return the full name of a dragen flow cell."""
-    return "211101_A00187_0615_AHLG5GDRXY"
-
-
 @pytest.fixture(name="demultiplexed_flow_cell")
 def fixture_demultiplexed_flow_cell(
     demultiplexed_runs: Path, bcl2fastq_flow_cell_full_name: str
 ) -> Path:
     return Path(demultiplexed_runs, bcl2fastq_flow_cell_full_name)
 
 
@@ -1619,15 +1629,15 @@
             "base_path": "/another/path",
             "covid_destination_path": "server.name.se:/another/%s/foldername/",
             "covid_report_path": "/folder_structure/%s/yet_another_folder/filename_%s_data_*.csv",
             "destination_path": "server.name.se:/some",
             "mail_user": "an@email.com",
         },
         "demultiplex": {
-            "run_dir": "tests/fixtures/apps/demultiplexing/flow-cell-runs",
+            "run_dir": "tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000",
             "out_dir": "tests/fixtures/apps/demultiplexing/demultiplexed-runs",
             "slurm": {
                 "account": "development",
                 "mail_user": "an@scilifelab.se",
             },
         },
         "encryption": {"binary_path": "bin/gpg"},
```

### Comparing `cg-33.1.1/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/runParameters.xml` & `cg-33.1.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml`

 * *Files 2% similar despite different names*

#### Comparing `cg-33.1.1/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/runParameters.xml` & `cg-33.1.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml`

```diff
@@ -10,55 +10,55 @@
   <PlannedRead1Cycles>151</PlannedRead1Cycles>
   <PlannedRead2Cycles>151</PlannedRead2Cycles>
   <PlannedIndex1ReadCycles>10</PlannedIndex1ReadCycles>
   <PlannedIndex2ReadCycles>10</PlannedIndex2ReadCycles>
   <RunNumber>226</RunNumber>
   <RtaVersion>v3.4.4</RtaVersion>
   <RecipeVersion>1.7.0</RecipeVersion>
-  <ExperimentName>HMYJ7DSXX</ExperimentName>
+  <ExperimentName>HMYJ7DSXY</ExperimentName>
   <RfidsInfo>
     <FlowCellSerialBarcode>HMYJ7DSXY</FlowCellSerialBarcode>
     <FlowCellPartNumber>20015843</FlowCellPartNumber>
     <FlowCellLotNumber>20482659</FlowCellLotNumber>
     <FlowCellExpirationdate>09/21/2021 00:00:00</FlowCellExpirationdate>
     <FlowCellStartDate>02/06/2021 12:40:00</FlowCellStartDate>
     <FlowCellNumberOfReuseRemaining>1</FlowCellNumberOfReuseRemaining>
-    <FlowCellSupportedModes>HTWashOnly;S1</FlowCellSupportedModes>
-    <FlowCellMode>S1</FlowCellMode>
+    <FlowCellSupportedModes>HTWashOnly;S4</FlowCellSupportedModes>
+    <FlowCellMode>S4</FlowCellMode>
     <FlowCellConsumableVersion>1</FlowCellConsumableVersion>
     <FlowCellRssi>2</FlowCellRssi>
     <LibraryTubeSerialBarcode>NV0297539-LIB</LibraryTubeSerialBarcode>
     <LibraryTubeSupportedModes>Universal</LibraryTubeSupportedModes>
     <LibraryTubePartNumber>20005221</LibraryTubePartNumber>
     <LibraryTubeLotNumber>1000008040</LibraryTubeLotNumber>
     <LibraryTubeExpirationdate>12/31/2169 00:00:00</LibraryTubeExpirationdate>
     <LibraryTubeStartDate>02/06/2021 12:40:00</LibraryTubeStartDate>
     <LibraryTubeRssi>4</LibraryTubeRssi>
     <SbsSerialBarcode>NV3040624-RGSBS</SbsSerialBarcode>
-    <SbsSupportedModes>S1</SbsSupportedModes>
+    <SbsSupportedModes>S4</SbsSupportedModes>
     <SbsPartNumber>20031051</SbsPartNumber>
     <SbsLotNumber>20485602</SbsLotNumber>
     <SbsExpirationdate>10/24/2021 00:00:00</SbsExpirationdate>
     <SbsStartDate>02/06/2021 12:40:00</SbsStartDate>
     <SbsCycleKit>338</SbsCycleKit>
     <SbsNumberOfCyclesRemaining>16</SbsNumberOfCyclesRemaining>
     <SbsNumberOfCyclesSupported>338</SbsNumberOfCyclesSupported>
     <SbsConsumableVersion>3</SbsConsumableVersion>
     <SbsRssi>4</SbsRssi>
     <ClusterSerialBarcode>NV3048388-RGCPE</ClusterSerialBarcode>
-    <ClusterSupportedModes>S1</ClusterSupportedModes>
+    <ClusterSupportedModes>S4</ClusterSupportedModes>
     <ClusterPartNumber>20031056</ClusterPartNumber>
     <ClusterLotNumber>20491402</ClusterLotNumber>
     <ClusterExpirationdate>10/31/2021 00:00:00</ClusterExpirationdate>
     <ClusterStartDate>02/06/2021 12:40:00</ClusterStartDate>
     <ClusterCycleKit>338</ClusterCycleKit>
     <ClusterNumberOfCyclesRemaining>16</ClusterNumberOfCyclesRemaining>
     <ClusterRssi>5</ClusterRssi>
     <BufferSerialBarcode>NV5091519-BUFFR</BufferSerialBarcode>
-    <BufferSupportedModes>S1</BufferSupportedModes>
+    <BufferSupportedModes>S4</BufferSupportedModes>
     <BufferPartNumber>20003187</BufferPartNumber>
     <BufferLotNumber>50000132</BufferLotNumber>
     <BufferExpirationdate>07/15/2021 00:00:00</BufferExpirationdate>
     <BufferNumberOfCyclesRemaining>8</BufferNumberOfCyclesRemaining>
     <BufferStartDate>02/06/2021 12:40:00</BufferStartDate>
     <BufferRssi>3</BufferRssi>
   </RfidsInfo>
```

### Comparing `cg-33.1.1/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json` & `cg-33.1.2/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json` & `cg-33.1.2/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/fixtures/analysis/rnafusion/multiqc_data.json` & `cg-33.1.2/tests/fixtures/analysis/rnafusion/multiqc_data.json`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/fixtures/analysis/sample_coverage.bed` & `cg-33.1.2/tests/fixtures/analysis/sample_coverage.bed`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/fixtures/apps/balsamic/case/config.json` & `cg-33.1.2/tests/fixtures/apps/balsamic/case/config.json`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/fixtures/apps/balsamic/case/metadata.yml` & `cg-33.1.2/tests/fixtures/apps/balsamic/case/metadata.yml`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml` & `cg-33.1.2/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/fixtures/apps/crunchy/spring_metadata.json` & `cg-33.1.2/tests/fixtures/apps/crunchy/spring_metadata.json`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml` & `cg-33.1.2/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_different_index_cycles.xml`

 * *Files 0% similar despite different names*

#### Comparing `cg-33.1.1/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml` & `cg-33.1.2/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_different_index_cycles.xml`

```diff
@@ -2,15 +2,15 @@
 <RunParameters xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
   <Surface>Both</Surface>
   <ReadType>PairedEnd</ReadType>
   <Side>A</Side>
   <Read1NumberOfCycles>151</Read1NumberOfCycles>
   <Read2NumberOfCycles>151</Read2NumberOfCycles>
   <IndexRead1NumberOfCycles>10</IndexRead1NumberOfCycles>
-  <IndexRead2NumberOfCycles>10</IndexRead2NumberOfCycles>
+  <IndexRead2NumberOfCycles>8</IndexRead2NumberOfCycles>
   <PlannedRead1Cycles>151</PlannedRead1Cycles>
   <PlannedRead2Cycles>151</PlannedRead2Cycles>
   <PlannedIndex1ReadCycles>10</PlannedIndex1ReadCycles>
   <PlannedIndex2ReadCycles>10</PlannedIndex2ReadCycles>
   <RunNumber>226</RunNumber>
   <RtaVersion>v3.4.4</RtaVersion>
   <RecipeVersion>1.7.0</RecipeVersion>
```

### Comparing `cg-33.1.1/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv` & `cg-33.1.2/tests/fixtures/apps/sequencing_metrics_parser/Unaligned/Reports/SampleSheet.csv`

 * *Files 23% similar despite different names*

```diff
@@ -1,582 +1,439 @@
+[Settings]
+BarcodeMismatchesIndex1,0
+BarcodeMismatchesIndex2,0
 [Data]
-FCID,Lane,SampleID,SampleRef,index,index2,SampleName,Control,Recipe,Operator,Project
-HVKJCDRXX,1,ACC7327A10,hg19,AACGACGCAT,AACTACAACG,468018,N,R1,script,468018
-HVKJCDRXX,1,ACC7327A27,hg19,GACGAACGTA,TCGTCCTTCA,468018,N,R1,script,468018
-HVKJCDRXX,1,ACC7327A17,hg19,ATACCTGTGA,GCATTGTGCT,468018,N,R1,script,468018
-HVKJCDRXX,1,ACC7327A34,hg19,CTATAGCGAG,AGTCGACTAG,468018,N,R1,script,468018
-HVKJCDRXX,1,ACC7327A16,hg19,CTATACACCA,CCAACTACGG,468018,N,R1,script,468018
-HVKJCDRXX,1,ACC7327A33,hg19,TTACGGAACA,TGACTCTGTC,468018,N,R1,script,468018
-HVKJCDRXX,1,ACC7327A35,hg19,ACGCGGACTT,TATTGCCTCG,468018,N,R1,script,468018
-HVKJCDRXX,1,ACC7327A9,hg19,CTTGTCTTGC,AACCAATGTG,468018,N,R1,script,468018
-HVKJCDRXX,1,ACC7327A26,hg19,CCGACTCCTT,ACTGTCCTTG,468018,N,R1,script,468018
-HVKJCDRXX,1,ACC7327A11,hg19,TTGGCCAGTT,ATGCTACCTG,468018,N,R1,script,468018
-HVKJCDRXX,1,ACC7327A28,hg19,CCACTGTGAC,TGGACAGATG,468018,N,R1,script,468018
-HVKJCDRXX,1,ACC7327A2,hg19,GACAATAGAG,TAGTGTACAC,468018,N,R1,script,468018
-HVKJCDRXX,1,ACC7327A19,hg19,AGAGATGGTA,GCTTACGGAA,468018,N,R1,script,468018
-HVKJCDRXX,1,ACC7327A7,hg19,GAGAGCTAAC,CAATACTTGC,468018,N,R1,script,468018
-HVKJCDRXX,1,ACC7327A24,hg19,GTGTTATCTC,ACACCAGACT,468018,N,R1,script,468018
-HVKJCDRXX,1,ACC7327A13,hg19,AGAGACTTAC,TAAGAGTTGG,468018,N,R1,script,468018
-HVKJCDRXX,1,ACC7327A30,hg19,GTTATTAGGC,CTCGATGAAC,468018,N,R1,script,468018
-HVKJCDRXX,1,ACC7327A12,hg19,ATTGCGGCTG,TGTCCTACAA,468018,N,R1,script,468018
-HVKJCDRXX,1,ACC7327A29,hg19,GAGCATCCAT,TCACGTCCAC,468018,N,R1,script,468018
-HVKJCDRXX,1,ACC7327A1,hg19,TGCCACTGTA,CAGCAGGTCA,468018,N,R1,script,468018
-HVKJCDRXX,1,ACC7327A18,hg19,TCAGATTCAC,TGGAGTGCGA,468018,N,R1,script,468018
-HVKJCDRXX,1,ACC7327A4,hg19,ACTGGTGTCG,CAAGTCCTGT,468018,N,R1,script,468018
-HVKJCDRXX,1,ACC7327A21,hg19,GTGTACGTCG,TCCTAGCAGG,468018,N,R1,script,468018
-HVKJCDRXX,1,ACC7327A5,hg19,TTAGGAGGAA,GAACTTGCGT,468018,N,R1,script,468018
-HVKJCDRXX,1,ACC7327A22,hg19,TCACCGTCAC,CAACTCCTTA,468018,N,R1,script,468018
-HVKJCDRXX,1,ACC7327A14,hg19,GCTGCCGATA,TATCCTACGT,468018,N,R1,script,468018
-HVKJCDRXX,1,ACC7327A31,hg19,TTATCGCTGA,TTAGGATTGG,468018,N,R1,script,468018
-HVKJCDRXX,1,ACC7327A6,hg19,ACAGAAGGTT,TGGAGATATC,468018,N,R1,script,468018
-HVKJCDRXX,1,ACC7327A23,hg19,TGTGAAGCTA,ACGCGATTCA,468018,N,R1,script,468018
-HVKJCDRXX,1,ACC7327A3,hg19,AGACGGCATC,AAGGTAACCT,468018,N,R1,script,468018
-HVKJCDRXX,1,ACC7327A20,hg19,ATGGAGACGG,CTGAGAGTTC,468018,N,R1,script,468018
-HVKJCDRXX,1,ACC7327A8,hg19,TTCAGGTCGT,TTGGTTGGTT,468018,N,R1,script,468018
-HVKJCDRXX,1,ACC7327A25,hg19,AACACAGCCG,AGACCTTGGT,468018,N,R1,script,468018
-HVKJCDRXX,1,ACC7327A15,hg19,GAATGTCCAA,GAATACCGTA,468018,N,R1,script,468018
-HVKJCDRXX,1,ACC7327A32,hg19,CGCTTAAGTA,ATTACTGCAC,468018,N,R1,script,468018
-HVKJCDRXX,1,ACC7327A66,hg19,GCTGAGAGCT,GTGATAGGTG,468018,N,R1,script,468018
-HVKJCDRXX,1,ACC7327A64,hg19,TCGTGGCTAG,GCCAGCAGTA,468018,N,R1,script,468018
-HVKJCDRXX,1,ACC7327A67,hg19,GAGCTTATGA,ACCAGTCATT,468018,N,R1,script,468018
-HVKJCDRXX,1,ACC7327A65,hg19,AGGACTGAAC,TGAAGCGACG,468018,N,R1,script,468018
-HVKJCDRXX,1,ACC7327A62,hg19,GCATACTCTA,TAGCGAGATA,468018,N,R1,script,468018
-HVKJCDRXX,1,ACC7327A63,hg19,GAGCTCCACA,CAGAACAGAA,468018,N,R1,script,468018
-HVKJCDRXX,1,ACC7327A45,hg19,ATCTTCCTAG,TGCGCGTGTA,468018,N,R1,script,468018
-HVKJCDRXX,1,ACC7327A46,hg19,TTCCACCTGG,ATGAGCTTCT,468018,N,R1,script,468018
-HVKJCDRXX,1,ACC7327A40,hg19,TCAGCACCGT,ACTGAATAGG,468018,N,R1,script,468018
-HVKJCDRXX,1,ACC7327A41,hg19,TCAAGTTCCT,CAAGTTCTAG,468018,N,R1,script,468018
-HVKJCDRXX,1,ACC7327A69,hg19,CAGCCTTGAG,TGAGTAGCAT,468018,N,R1,script,468018
-HVKJCDRXX,1,ACC7327A50,hg19,CTGCGTACTC,CTGATGGCAA,468018,N,R1,script,468018
-HVKJCDRXX,1,ACC7327A70,hg19,TCACCAGGAC,TCCTTGTCTC,468018,N,R1,script,468018
-HVKJCDRXX,1,ACC7327A68,hg19,AATGGTACTG,ACAGCAGTTA,468018,N,R1,script,468018
-HVKJCDRXX,1,ACC7327A42,hg19,AGACCTAGCT,CACAAGTATC,468018,N,R1,script,468018
-HVKJCDRXX,1,ACC7327A52,hg19,TGGATATGGC,TGGCGCGTAT,468018,N,R1,script,468018
-HVKJCDRXX,1,ACC7327A53,hg19,TATAACTCCG,TATGTGTCCT,468018,N,R1,script,468018
-HVKJCDRXX,1,ACC7327A43,hg19,GCCTTACTTA,GCACCTTAAC,468018,N,R1,script,468018
-HVKJCDRXX,1,ACC7327A44,hg19,GCCTAGGACT,GAGAACGGCT,468018,N,R1,script,468018
-HVKJCDRXX,1,ACC7327A47,hg19,TTATCTGTGC,CACTCAGTAT,468018,N,R1,script,468018
-HVKJCDRXX,1,ACC7327A49,hg19,TTCACACAGT,CTTCAGTGTT,468018,N,R1,script,468018
-HVKJCDRXX,1,ACC7327A48,hg19,ACTGTCAATC,CGTCCTTAAC,468018,N,R1,script,468018
-HVKJCDRXX,1,ACC7327A60,hg19,GTTCCACCGA,CCTGCTGTTA,468018,N,R1,script,468018
-HVKJCDRXX,1,ACC7327A58,hg19,CGCAGAACTT,TATCGACGTC,468018,N,R1,script,468018
-HVKJCDRXX,1,ACC7327A56,hg19,AATGTGGCGT,TGTCAGGTAG,468018,N,R1,script,468018
-HVKJCDRXX,1,ACC7327A54,hg19,CTCTCATGCG,ACGTCGGTTG,468018,N,R1,script,468018
-HVKJCDRXX,1,ACC7327A55,hg19,CAACCGATTA,TGCTGAGTTA,468018,N,R1,script,468018
-HVKJCDRXX,1,ACC7327A61,hg19,GACGTTCTCT,AGTAGAGCTA,468018,N,R1,script,468018
-HVKJCDRXX,1,ACC7327A57,hg19,GCTACTGTCG,CTTGCTCCAT,468018,N,R1,script,468018
-HVKJCDRXX,1,ACC7327A59,hg19,CCAAGACACT,ACCGACATGG,468018,N,R1,script,468018
-HVKJCDRXX,1,ACC7327A51,hg19,CAGAACGTGG,GACTTCACCG,468018,N,R1,script,468018
-HVKJCDRXX,1,ACC7327A39,hg19,CACGGTTGGT,CTAGCTGAAT,468018,N,R1,script,468018
-HVKJCDRXX,1,ACC7327A38,hg19,AACACAACGA,ACGCAGCCAA,468018,N,R1,script,468018
-HVKJCDRXX,1,ACC7327A37,hg19,CGGAACGAAG,ACCATCGCCT,468018,N,R1,script,468018
-HVKJCDRXX,1,ACC7327A36,hg19,AGAATCCTTC,TGCCAGGTGT,468018,N,R1,script,468018
-HVKJCDRXX,1,ACC7238A6,hg19,CCTAGCAATC,ACGTGACGTG,686153,N,R1,script,686153
-HVKJCDRXX,1,ACC7237A5,hg19,TTAGTACAGG,GAGGCTCGTT,686153,N,R1,script,686153
-HVKJCDRXX,1,ACC7238A2,hg19,CTTGTGCCAG,TAGTGGTCAT,686153,N,R1,script,686153
-HVKJCDRXX,1,ACC7237A7,hg19,GTCCTAACTT,GCAGCTGTGA,686153,N,R1,script,686153
-HVKJCDRXX,1,ACC7237A11,hg19,AGAGGTGATT,CGTGTACTGC,686153,N,R1,script,686153
-HVKJCDRXX,1,ACC7237A9,hg19,CATACCGTAG,CCTCCTCTTG,686153,N,R1,script,686153
-HVKJCDRXX,1,ACC7207A4,hg19,AGCACTATTC,CTATGTTACG,GMCKsolid-control-HD827,N,R1,script,GMCKsolid-control-HD827
-HVKJCDRXX,1,ACC7291A1,hg19,GATTCTCCGT,CAACTCCACG,171215,N,R1,script,171215
-HVKJCDRXX,1,ACC7302A4,hg19,AGGCGATCTG,CGTCGTAATT,223075,N,R1,script,223075
-HVKJCDRXX,1,ACC7302A5,hg19,GTTCGATAAG,CGTATCTGGC,223075,N,R1,script,223075
-HVKJCDRXX,1,ACC7291A4,hg19,ACTTGAAGTG,CACCACATTA,171215,N,R1,script,171215
-HVKJCDRXX,1,ACC7291A6,hg19,TGCTCCTAAC,CGGCTAGGAA,171215,N,R1,script,171215
-HVKJCDRXX,2,ACC7327A10,hg19,AACGACGCAT,AACTACAACG,468018,N,R1,script,468018
-HVKJCDRXX,2,ACC7327A27,hg19,GACGAACGTA,TCGTCCTTCA,468018,N,R1,script,468018
-HVKJCDRXX,2,ACC7327A17,hg19,ATACCTGTGA,GCATTGTGCT,468018,N,R1,script,468018
-HVKJCDRXX,2,ACC7327A34,hg19,CTATAGCGAG,AGTCGACTAG,468018,N,R1,script,468018
-HVKJCDRXX,2,ACC7327A16,hg19,CTATACACCA,CCAACTACGG,468018,N,R1,script,468018
-HVKJCDRXX,2,ACC7327A33,hg19,TTACGGAACA,TGACTCTGTC,468018,N,R1,script,468018
-HVKJCDRXX,2,ACC7327A35,hg19,ACGCGGACTT,TATTGCCTCG,468018,N,R1,script,468018
-HVKJCDRXX,2,ACC7327A9,hg19,CTTGTCTTGC,AACCAATGTG,468018,N,R1,script,468018
-HVKJCDRXX,2,ACC7327A26,hg19,CCGACTCCTT,ACTGTCCTTG,468018,N,R1,script,468018
-HVKJCDRXX,2,ACC7327A11,hg19,TTGGCCAGTT,ATGCTACCTG,468018,N,R1,script,468018
-HVKJCDRXX,2,ACC7327A28,hg19,CCACTGTGAC,TGGACAGATG,468018,N,R1,script,468018
-HVKJCDRXX,2,ACC7327A2,hg19,GACAATAGAG,TAGTGTACAC,468018,N,R1,script,468018
-HVKJCDRXX,2,ACC7327A19,hg19,AGAGATGGTA,GCTTACGGAA,468018,N,R1,script,468018
-HVKJCDRXX,2,ACC7327A7,hg19,GAGAGCTAAC,CAATACTTGC,468018,N,R1,script,468018
-HVKJCDRXX,2,ACC7327A24,hg19,GTGTTATCTC,ACACCAGACT,468018,N,R1,script,468018
-HVKJCDRXX,2,ACC7327A13,hg19,AGAGACTTAC,TAAGAGTTGG,468018,N,R1,script,468018
-HVKJCDRXX,2,ACC7327A30,hg19,GTTATTAGGC,CTCGATGAAC,468018,N,R1,script,468018
-HVKJCDRXX,2,ACC7327A12,hg19,ATTGCGGCTG,TGTCCTACAA,468018,N,R1,script,468018
-HVKJCDRXX,2,ACC7327A29,hg19,GAGCATCCAT,TCACGTCCAC,468018,N,R1,script,468018
-HVKJCDRXX,2,ACC7327A1,hg19,TGCCACTGTA,CAGCAGGTCA,468018,N,R1,script,468018
-HVKJCDRXX,2,ACC7327A18,hg19,TCAGATTCAC,TGGAGTGCGA,468018,N,R1,script,468018
-HVKJCDRXX,2,ACC7327A4,hg19,ACTGGTGTCG,CAAGTCCTGT,468018,N,R1,script,468018
-HVKJCDRXX,2,ACC7327A21,hg19,GTGTACGTCG,TCCTAGCAGG,468018,N,R1,script,468018
-HVKJCDRXX,2,ACC7327A5,hg19,TTAGGAGGAA,GAACTTGCGT,468018,N,R1,script,468018
-HVKJCDRXX,2,ACC7327A22,hg19,TCACCGTCAC,CAACTCCTTA,468018,N,R1,script,468018
-HVKJCDRXX,2,ACC7327A14,hg19,GCTGCCGATA,TATCCTACGT,468018,N,R1,script,468018
-HVKJCDRXX,2,ACC7327A31,hg19,TTATCGCTGA,TTAGGATTGG,468018,N,R1,script,468018
-HVKJCDRXX,2,ACC7327A6,hg19,ACAGAAGGTT,TGGAGATATC,468018,N,R1,script,468018
-HVKJCDRXX,2,ACC7327A23,hg19,TGTGAAGCTA,ACGCGATTCA,468018,N,R1,script,468018
-HVKJCDRXX,2,ACC7327A3,hg19,AGACGGCATC,AAGGTAACCT,468018,N,R1,script,468018
-HVKJCDRXX,2,ACC7327A20,hg19,ATGGAGACGG,CTGAGAGTTC,468018,N,R1,script,468018
-HVKJCDRXX,2,ACC7327A8,hg19,TTCAGGTCGT,TTGGTTGGTT,468018,N,R1,script,468018
-HVKJCDRXX,2,ACC7327A25,hg19,AACACAGCCG,AGACCTTGGT,468018,N,R1,script,468018
-HVKJCDRXX,2,ACC7327A15,hg19,GAATGTCCAA,GAATACCGTA,468018,N,R1,script,468018
-HVKJCDRXX,2,ACC7327A32,hg19,CGCTTAAGTA,ATTACTGCAC,468018,N,R1,script,468018
-HVKJCDRXX,2,ACC7327A66,hg19,GCTGAGAGCT,GTGATAGGTG,468018,N,R1,script,468018
-HVKJCDRXX,2,ACC7327A64,hg19,TCGTGGCTAG,GCCAGCAGTA,468018,N,R1,script,468018
-HVKJCDRXX,2,ACC7327A67,hg19,GAGCTTATGA,ACCAGTCATT,468018,N,R1,script,468018
-HVKJCDRXX,2,ACC7327A65,hg19,AGGACTGAAC,TGAAGCGACG,468018,N,R1,script,468018
-HVKJCDRXX,2,ACC7327A62,hg19,GCATACTCTA,TAGCGAGATA,468018,N,R1,script,468018
-HVKJCDRXX,2,ACC7327A63,hg19,GAGCTCCACA,CAGAACAGAA,468018,N,R1,script,468018
-HVKJCDRXX,2,ACC7327A45,hg19,ATCTTCCTAG,TGCGCGTGTA,468018,N,R1,script,468018
-HVKJCDRXX,2,ACC7327A46,hg19,TTCCACCTGG,ATGAGCTTCT,468018,N,R1,script,468018
-HVKJCDRXX,2,ACC7327A40,hg19,TCAGCACCGT,ACTGAATAGG,468018,N,R1,script,468018
-HVKJCDRXX,2,ACC7327A41,hg19,TCAAGTTCCT,CAAGTTCTAG,468018,N,R1,script,468018
-HVKJCDRXX,2,ACC7327A69,hg19,CAGCCTTGAG,TGAGTAGCAT,468018,N,R1,script,468018
-HVKJCDRXX,2,ACC7327A50,hg19,CTGCGTACTC,CTGATGGCAA,468018,N,R1,script,468018
-HVKJCDRXX,2,ACC7327A70,hg19,TCACCAGGAC,TCCTTGTCTC,468018,N,R1,script,468018
-HVKJCDRXX,2,ACC7327A68,hg19,AATGGTACTG,ACAGCAGTTA,468018,N,R1,script,468018
-HVKJCDRXX,2,ACC7327A42,hg19,AGACCTAGCT,CACAAGTATC,468018,N,R1,script,468018
-HVKJCDRXX,2,ACC7327A52,hg19,TGGATATGGC,TGGCGCGTAT,468018,N,R1,script,468018
-HVKJCDRXX,2,ACC7327A53,hg19,TATAACTCCG,TATGTGTCCT,468018,N,R1,script,468018
-HVKJCDRXX,2,ACC7327A43,hg19,GCCTTACTTA,GCACCTTAAC,468018,N,R1,script,468018
-HVKJCDRXX,2,ACC7327A44,hg19,GCCTAGGACT,GAGAACGGCT,468018,N,R1,script,468018
-HVKJCDRXX,2,ACC7327A47,hg19,TTATCTGTGC,CACTCAGTAT,468018,N,R1,script,468018
-HVKJCDRXX,2,ACC7327A49,hg19,TTCACACAGT,CTTCAGTGTT,468018,N,R1,script,468018
-HVKJCDRXX,2,ACC7327A48,hg19,ACTGTCAATC,CGTCCTTAAC,468018,N,R1,script,468018
-HVKJCDRXX,2,ACC7327A60,hg19,GTTCCACCGA,CCTGCTGTTA,468018,N,R1,script,468018
-HVKJCDRXX,2,ACC7327A58,hg19,CGCAGAACTT,TATCGACGTC,468018,N,R1,script,468018
-HVKJCDRXX,2,ACC7327A56,hg19,AATGTGGCGT,TGTCAGGTAG,468018,N,R1,script,468018
-HVKJCDRXX,2,ACC7327A54,hg19,CTCTCATGCG,ACGTCGGTTG,468018,N,R1,script,468018
-HVKJCDRXX,2,ACC7327A55,hg19,CAACCGATTA,TGCTGAGTTA,468018,N,R1,script,468018
-HVKJCDRXX,2,ACC7327A61,hg19,GACGTTCTCT,AGTAGAGCTA,468018,N,R1,script,468018
-HVKJCDRXX,2,ACC7327A57,hg19,GCTACTGTCG,CTTGCTCCAT,468018,N,R1,script,468018
-HVKJCDRXX,2,ACC7327A59,hg19,CCAAGACACT,ACCGACATGG,468018,N,R1,script,468018
-HVKJCDRXX,2,ACC7327A51,hg19,CAGAACGTGG,GACTTCACCG,468018,N,R1,script,468018
-HVKJCDRXX,2,ACC7327A39,hg19,CACGGTTGGT,CTAGCTGAAT,468018,N,R1,script,468018
-HVKJCDRXX,2,ACC7327A38,hg19,AACACAACGA,ACGCAGCCAA,468018,N,R1,script,468018
-HVKJCDRXX,2,ACC7327A37,hg19,CGGAACGAAG,ACCATCGCCT,468018,N,R1,script,468018
-HVKJCDRXX,2,ACC7327A36,hg19,AGAATCCTTC,TGCCAGGTGT,468018,N,R1,script,468018
-HVKJCDRXX,2,ACC7238A6,hg19,CCTAGCAATC,ACGTGACGTG,686153,N,R1,script,686153
-HVKJCDRXX,2,ACC7237A5,hg19,TTAGTACAGG,GAGGCTCGTT,686153,N,R1,script,686153
-HVKJCDRXX,2,ACC7238A2,hg19,CTTGTGCCAG,TAGTGGTCAT,686153,N,R1,script,686153
-HVKJCDRXX,2,ACC7237A7,hg19,GTCCTAACTT,GCAGCTGTGA,686153,N,R1,script,686153
-HVKJCDRXX,2,ACC7237A11,hg19,AGAGGTGATT,CGTGTACTGC,686153,N,R1,script,686153
-HVKJCDRXX,2,ACC7237A9,hg19,CATACCGTAG,CCTCCTCTTG,686153,N,R1,script,686153
-HVKJCDRXX,2,ACC7207A4,hg19,AGCACTATTC,CTATGTTACG,GMCKsolid-control-HD827,N,R1,script,GMCKsolid-control-HD827
-HVKJCDRXX,2,ACC7291A1,hg19,GATTCTCCGT,CAACTCCACG,171215,N,R1,script,171215
-HVKJCDRXX,2,ACC7302A4,hg19,AGGCGATCTG,CGTCGTAATT,223075,N,R1,script,223075
-HVKJCDRXX,2,ACC7302A5,hg19,GTTCGATAAG,CGTATCTGGC,223075,N,R1,script,223075
-HVKJCDRXX,2,ACC7291A4,hg19,ACTTGAAGTG,CACCACATTA,171215,N,R1,script,171215
-HVKJCDRXX,2,ACC7291A6,hg19,TGCTCCTAAC,CGGCTAGGAA,171215,N,R1,script,171215
-HVKJCDRXX,1,C07---UDI0051,hg19,AACAGGTTAT,CTTGGTATGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,H06---UDI0048,hg19,ACCTTGGCAT,ATGAGGCCGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,B07---UDI0050,hg19,GCGCTCTAAT,GTCGGAGCGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,G06---UDI0047,hg19,GTTCCAATAT,GCAGAATTGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,E07---UDI0053,hg19,CAACAATGAT,CCGTGAAGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,F07---UDI0054,hg19,TGGTGGCAAT,TTACAGGAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,C06---UDI0043,hg19,AAGATACTAT,ATGTAAGTGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,F06---UDI0046,hg19,GCAATGCAAT,AACGTTCCGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,A06---UDI0041,hg19,ATATGGATAT,TAATACAGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,G05---UDI0039,hg19,TAAGTGGTAT,GGCTTAAGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,F08---UDI0062,hg19,TAAGGTCAAT,CTACGACAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,B06---UDI0042,hg19,GCGCAAGCAT,CGGCGTGAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,H07---UDI0056,hg19,GAATGAGAAT,AATGCCTCGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,H10---UDI0080,hg19,GTGAATATAT,GAATGAGAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,G07---UDI0055,hg19,AGGCAGAGAT,GGCATTCTGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,G08---UDI0063,hg19,TTGCCTAGAT,TAAGTGGTGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,B05---UDI0034,hg19,CGTTAGAAAT,GACCTGAAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,E04---UDI0029,hg19,CCGTGAAGAT,ATCCACTGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,D05---UDI0036,hg19,GATTCTGCAT,CTCTCGTCGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,C05---UDI0035,hg19,AGCCTCATAT,TCTCTACTGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,D04---UDI0028,hg19,TCCAACGCAT,AAGTCCAAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,E08---UDI0061,hg19,CGGAACTGAT,TCGTAGTGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,D08---UDI0060,hg19,AGCTCGCTAT,GATTCTGCGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,C10---UDI0075,hg19,AGTACTCCAT,AACAGGTTGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,F05---UDI0038,hg19,CTACGACAAT,TTGGACTCGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,A10---UDI0073,hg19,CAATTAACAT,ATATCTCGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,E06---UDI0045,hg19,ATGGCATGAT,GGTACCTTGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,A11---UDI0081,hg19,AACTGTAGAT,TGCGGCGTGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,D06---UDI0044,hg19,GGAGCGTCAT,GCACGGACGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,B10---UDI0074,hg19,TGGCCGGTAT,GCGCTCTAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,E05---UDI0037,hg19,TCGTAGTGAT,CCAAGTCTGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,D07---UDI0052,hg19,GGTGAACCAT,TCCAACGCGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,A09---UDI0065,hg19,ACACTAAGAT,ATATGGATGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,C09---UDI0067,hg19,TTCCTGTTAT,AAGATACTGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,C12---UDI0091,hg19,GTATGTTCAT,TTCCTGTTGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,A03---UDI0017,hg19,TAATACAGAT,GTGAATATGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,E09---UDI0069,hg19,GCCACAGGAT,ATGGCATGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,G10---UDI0079,hg19,ACAGGCGCAT,AGGCAGAGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,B12---UDI0090,hg19,CGCTATGTAT,GTGTCGGAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,F04---UDI0030,hg19,TTACAGGAAT,GCTTGTCAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,B09---UDI0066,hg19,GTGTCGGAAT,GCGCAAGCGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,D10---UDI0076,hg19,GACGTCTTAT,GGTGAACCGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,E12---UDI0093,hg19,TACTCATAAT,GCCACAGGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,F10---UDI0078,hg19,CATAGAGTAT,TGGTGGCAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,B03---UDI0018,hg19,CGGCGTGAAT,ACAGGCGCGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,D09---UDI0068,hg19,CCTTCACCAT,GGAGCGTCGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,C03---UDI0019,hg19,ATGTAAGTAT,CATAGAGTGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,D12---UDI0092,hg19,ACGCACCTAT,CCTTCACCGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,E10---UDI0077,hg19,TGCGAGACAT,CAACAATGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,H02---UDI0016,hg19,AATCCGGAAT,AACTGTAGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,A05---UDI0033,hg19,TACCGAGGAT,AGTTCAGGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,A07---UDI0049,hg19,ATATCTCGAT,ACTAAGATGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,H08---UDI0064,hg19,CCATTCGAAT,CGGACAACGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,G02---UDI0015,hg19,GGCTTAAGAT,GGTCACGAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,F12---UDI0094,hg19,CGTCTGCGAT,ATTGTGAAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,H12---UDI0096,hg19,CTAGCGCTAT,GTCTACACGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,G04---UDI0031,hg19,GGCATTCTAT,CAAGCTAGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,H04---UDI0032,hg19,AATGCCTCAT,TGGATCGAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,G12---UDI0095,hg19,TCGATATCAT,ACTCGTGTGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,A01---UDI0001,hg19,CCGCGGTTAT,CTAGCGCTGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,B01---UDI0002,hg19,TTATAACCAT,TCGATATCGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,D01---UDI0004,hg19,AAGTCCAAAT,TACTCATAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,E01---UDI0005,hg19,ATCCACTGAT,ACGCACCTGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,G01---UDI0007,hg19,CAAGCTAGAT,CGCTATGTGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,A12---UDI0089,hg19,TATCGCACAT,ACACTAAGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,E02---UDI0013,hg19,CCAAGTCTAT,TCATCCTTGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,F02---UDI0014,hg19,TTGGACTCAT,CTGCTTCCGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,F01---UDI0006,hg19,GCTTGTCAAT,GTATGTTCGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,D03---UDI0020,hg19,GCACGGACAT,TGCGAGACGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,D02---UDI0012,hg19,CTCTCGTCAT,AGGTTATAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,B02---UDI0010,hg19,GACCTGAAAT,CTCACCAAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,C02---UDI0011,hg19,TCTCTACTAT,GAACCGCGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,C01---UDI0003,hg19,GGACTTGGAT,CGTCTGCGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,E11---UDI0085,hg19,AGGTTATAAT,CGGAACTGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,D11---UDI0084,hg19,TCATCCTTAT,AGCTCGCTGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,G11---UDI0087,hg19,CTCACCAAAT,TTGCCTAGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,A02---UDI0009,hg19,AGTTCAGGAT,TCTGTTGGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,H05---UDI0040,hg19,CGGACAACAT,AATCCGGAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,B11---UDI0082,hg19,GGTCACGAAT,CATAATACGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,C08---UDI0059,hg19,GATCTATCAT,AGCCTCATGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,C11---UDI0083,hg19,CTGCTTCCAT,GATCTATCGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,F11---UDI0086,hg19,GAACCGCGAT,TAAGGTCAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,C04---UDI0027,hg19,CTTGGTATAT,GGACTTGGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,B04---UDI0026,hg19,GTCGGAGCAT,TTATAACCGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,E03---UDI0021,hg19,GGTACCTTAT,GACGTCTTGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,F09---UDI0070,hg19,ATTGTGAAAT,GCAATGCAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,G09---UDI0071,hg19,ACTCGTGTAT,GTTCCAATGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,F03---UDI0022,hg19,AACGTTCCAT,AGTACTCCGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,G03---UDI0023,hg19,GCAGAATTAT,TGGCCGGTGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,H09---UDI0072,hg19,GTCTACACAT,ACCTTGGCGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,A04---UDI0025,hg19,ACTAAGATAT,CCGCGGTTGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,H01---UDI0008,hg19,TGGATCGAAT,TATCGCACGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,B08---UDI0058,hg19,CATAATACAT,CGTTAGAAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,H11---UDI0088,hg19,TCTGTTGGAT,CCATTCGAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,H03---UDI0024,hg19,ATGAGGCCAT,CAATTAACGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,A08---UDI0057,hg19,TGCGGCGTAT,TACCGAGGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,A01---D701-D501--ATTACTCG-TATAGCCT-,hg19,ATTACTCGAT,AGGCTATAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,B01---D701-D502--ATTACTCG-ATAGAGGC-,hg19,ATTACTCGAT,GCCTCTATGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,C01---D701-D503--ATTACTCG-CCTATCCT-,hg19,ATTACTCGAT,AGGATAGGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,D01---D701-D504--ATTACTCG-GGCTCTGA-,hg19,ATTACTCGAT,TCAGAGCCGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,E01---D701-D505--ATTACTCG-AGGCGAAG-,hg19,ATTACTCGAT,CTTCGCCTGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,F01---D701-D506--ATTACTCG-TAATCTTA-,hg19,ATTACTCGAT,TAAGATTAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,G01---D701-D507--ATTACTCG-CAGGACGT-,hg19,ATTACTCGAT,ACGTCCTGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,H01---D701-D508--ATTACTCG-GTACTGAC-,hg19,ATTACTCGAT,GTCAGTACGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,A02---D702-D501--TCCGGAGA-TATAGCCT-,hg19,TCCGGAGAAT,AGGCTATAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,B02---D702-D502--TCCGGAGA-ATAGAGGC-,hg19,TCCGGAGAAT,GCCTCTATGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,C02---D702-D503--TCCGGAGA-CCTATCCT-,hg19,TCCGGAGAAT,AGGATAGGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,D02---D702-D504--TCCGGAGA-GGCTCTGA-,hg19,TCCGGAGAAT,TCAGAGCCGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,E02---D702-D505--TCCGGAGA-AGGCGAAG-,hg19,TCCGGAGAAT,CTTCGCCTGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,F02---D702-D506--TCCGGAGA-TAATCTTA-,hg19,TCCGGAGAAT,TAAGATTAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,G02---D702-D507--TCCGGAGA-CAGGACGT-,hg19,TCCGGAGAAT,ACGTCCTGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,H02---D702-D508--TCCGGAGA-GTACTGAC-,hg19,TCCGGAGAAT,GTCAGTACGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,A03---D703-D501--CGCTCATT-TATAGCCT-,hg19,CGCTCATTAT,AGGCTATAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,B03---D703-D502--CGCTCATT-ATAGAGGC-,hg19,CGCTCATTAT,GCCTCTATGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,C03---D703-D503--CGCTCATT-CCTATCCT-,hg19,CGCTCATTAT,AGGATAGGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,D03---D703-D504--CGCTCATT-GGCTCTGA-,hg19,CGCTCATTAT,TCAGAGCCGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,E03---D703-D505--CGCTCATT-AGGCGAAG-,hg19,CGCTCATTAT,CTTCGCCTGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,F03---D703-D506--CGCTCATT-TAATCTTA-,hg19,CGCTCATTAT,TAAGATTAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,G03---D703-D507--CGCTCATT-CAGGACGT-,hg19,CGCTCATTAT,ACGTCCTGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,H03---D703-D508--CGCTCATT-GTACTGAC-,hg19,CGCTCATTAT,GTCAGTACGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,A04---D704-D501--GAGATTCC-TATAGCCT-,hg19,GAGATTCCAT,AGGCTATAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,B04---D704-D502--GAGATTCC-ATAGAGGC-,hg19,GAGATTCCAT,GCCTCTATGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,C04---D704-D503--GAGATTCC-CCTATCCT-,hg19,GAGATTCCAT,AGGATAGGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,D04---D704-D504--GAGATTCC-GGCTCTGA-,hg19,GAGATTCCAT,TCAGAGCCGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,E04---D704-D505--GAGATTCC-AGGCGAAG-,hg19,GAGATTCCAT,CTTCGCCTGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,F04---D704-D506--GAGATTCC-TAATCTTA-,hg19,GAGATTCCAT,TAAGATTAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,G04---D704-D507--GAGATTCC-CAGGACGT-,hg19,GAGATTCCAT,ACGTCCTGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,H04---D704-D508--GAGATTCC-GTACTGAC-,hg19,GAGATTCCAT,GTCAGTACGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,A05---D705-D501--ATTCAGAA-TATAGCCT-,hg19,ATTCAGAAAT,AGGCTATAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,B05---D705-D502--ATTCAGAA-ATAGAGGC-,hg19,ATTCAGAAAT,GCCTCTATGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,C05---D705-D503--ATTCAGAA-CCTATCCT-,hg19,ATTCAGAAAT,AGGATAGGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,D05---D705-D504--ATTCAGAA-GGCTCTGA-,hg19,ATTCAGAAAT,TCAGAGCCGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,E05---D705-D505--ATTCAGAA-AGGCGAAG-,hg19,ATTCAGAAAT,CTTCGCCTGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,F05---D705-D506--ATTCAGAA-TAATCTTA-,hg19,ATTCAGAAAT,TAAGATTAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,G05---D705-D507--ATTCAGAA-CAGGACGT-,hg19,ATTCAGAAAT,ACGTCCTGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,H05---D705-D508--ATTCAGAA-GTACTGAC-,hg19,ATTCAGAAAT,GTCAGTACGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,A06---D706-D501--GAATTCGT-TATAGCCT-,hg19,GAATTCGTAT,AGGCTATAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,B06---D706-D502--GAATTCGT-ATAGAGGC-,hg19,GAATTCGTAT,GCCTCTATGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,C06---D706-D503--GAATTCGT-CCTATCCT-,hg19,GAATTCGTAT,AGGATAGGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,D06---D706-D504--GAATTCGT-GGCTCTGA-,hg19,GAATTCGTAT,TCAGAGCCGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,E06---D706-D505--GAATTCGT-AGGCGAAG-,hg19,GAATTCGTAT,CTTCGCCTGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,F06---D706-D506--GAATTCGT-TAATCTTA-,hg19,GAATTCGTAT,TAAGATTAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,G06---D706-D507--GAATTCGT-CAGGACGT-,hg19,GAATTCGTAT,ACGTCCTGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,H06---D706-D508--GAATTCGT-GTACTGAC-,hg19,GAATTCGTAT,GTCAGTACGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,A07---D707-D501--CTGAAGCT-TATAGCCT-,hg19,CTGAAGCTAT,AGGCTATAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,B07---D707-D502--CTGAAGCT-ATAGAGGC-,hg19,CTGAAGCTAT,GCCTCTATGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,C07---D707-D503--CTGAAGCT-CCTATCCT-,hg19,CTGAAGCTAT,AGGATAGGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,D07---D707-D504--CTGAAGCT-GGCTCTGA-,hg19,CTGAAGCTAT,TCAGAGCCGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,E07---D707-D505--CTGAAGCT-AGGCGAAG-,hg19,CTGAAGCTAT,CTTCGCCTGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,F07---D707-D506--CTGAAGCT-TAATCTTA-,hg19,CTGAAGCTAT,TAAGATTAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,G07---D707-D507--CTGAAGCT-CAGGACGT-,hg19,CTGAAGCTAT,ACGTCCTGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,H07---D707-D508--CTGAAGCT-GTACTGAC-,hg19,CTGAAGCTAT,GTCAGTACGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,A08---D708-D501--TAATGCGC-TATAGCCT-,hg19,TAATGCGCAT,AGGCTATAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,B08---D708-D502--TAATGCGC-ATAGAGGC-,hg19,TAATGCGCAT,GCCTCTATGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,C08---D708-D503--TAATGCGC-CCTATCCT-,hg19,TAATGCGCAT,AGGATAGGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,D08---D708-D504--TAATGCGC-GGCTCTGA-,hg19,TAATGCGCAT,TCAGAGCCGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,E08---D708-D505--TAATGCGC-AGGCGAAG-,hg19,TAATGCGCAT,CTTCGCCTGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,F08---D708-D506--TAATGCGC-TAATCTTA-,hg19,TAATGCGCAT,TAAGATTAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,G08---D708-D507--TAATGCGC-CAGGACGT-,hg19,TAATGCGCAT,ACGTCCTGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,H08---D708-D508--TAATGCGC-GTACTGAC-,hg19,TAATGCGCAT,GTCAGTACGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,A09---D709-D501--CGGCTATG-TATAGCCT-,hg19,CGGCTATGAT,AGGCTATAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,B09---D709-D502--CGGCTATG-ATAGAGGC-,hg19,CGGCTATGAT,GCCTCTATGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,C09---D709-D503--CGGCTATG-CCTATCCT-,hg19,CGGCTATGAT,AGGATAGGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,D09---D709-D504--CGGCTATG-GGCTCTGA-,hg19,CGGCTATGAT,TCAGAGCCGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,E09---D709-D505--CGGCTATG-AGGCGAAG-,hg19,CGGCTATGAT,CTTCGCCTGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,F09---D709-D506--CGGCTATG-TAATCTTA-,hg19,CGGCTATGAT,TAAGATTAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,G09---D709-D507--CGGCTATG-CAGGACGT-,hg19,CGGCTATGAT,ACGTCCTGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,H09---D709-D508--CGGCTATG-GTACTGAC-,hg19,CGGCTATGAT,GTCAGTACGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,A10---D710-D501--TCCGCGAA-TATAGCCT-,hg19,TCCGCGAAAT,AGGCTATAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,B10---D710-D502--TCCGCGAA-ATAGAGGC-,hg19,TCCGCGAAAT,GCCTCTATGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,C10---D710-D503--TCCGCGAA-CCTATCCT-,hg19,TCCGCGAAAT,AGGATAGGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,D10---D710-D504--TCCGCGAA-GGCTCTGA-,hg19,TCCGCGAAAT,TCAGAGCCGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,E10---D710-D505--TCCGCGAA-AGGCGAAG-,hg19,TCCGCGAAAT,CTTCGCCTGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,F10---D710-D506--TCCGCGAA-TAATCTTA-,hg19,TCCGCGAAAT,TAAGATTAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,G10---D710-D507--TCCGCGAA-CAGGACGT-,hg19,TCCGCGAAAT,ACGTCCTGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,H10---D710-D508--TCCGCGAA-GTACTGAC-,hg19,TCCGCGAAAT,GTCAGTACGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,A11---D711-D501--TCTCGCGC-TATAGCCT-,hg19,TCTCGCGCAT,AGGCTATAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,B11---D711-D502--TCTCGCGC-ATAGAGGC-,hg19,TCTCGCGCAT,GCCTCTATGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,C11---D711-D503--TCTCGCGC-CCTATCCT-,hg19,TCTCGCGCAT,AGGATAGGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,D11---D711-D504--TCTCGCGC-GGCTCTGA-,hg19,TCTCGCGCAT,TCAGAGCCGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,E11---D711-D505--TCTCGCGC-AGGCGAAG-,hg19,TCTCGCGCAT,CTTCGCCTGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,F11---D711-D506--TCTCGCGC-TAATCTTA-,hg19,TCTCGCGCAT,TAAGATTAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,G11---D711-D507--TCTCGCGC-CAGGACGT-,hg19,TCTCGCGCAT,ACGTCCTGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,H11---D711-D508--TCTCGCGC-GTACTGAC-,hg19,TCTCGCGCAT,GTCAGTACGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,A12---D712-D501--AGCGATAG-TATAGCCT-,hg19,AGCGATAGAT,AGGCTATAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,B12---D712-D502--AGCGATAG-ATAGAGGC-,hg19,AGCGATAGAT,GCCTCTATGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,C12---D712-D503--AGCGATAG-CCTATCCT-,hg19,AGCGATAGAT,AGGATAGGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,D12---D712-D504--AGCGATAG-GGCTCTGA-,hg19,AGCGATAGAT,TCAGAGCCGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,E12---D712-D505--AGCGATAG-AGGCGAAG-,hg19,AGCGATAGAT,CTTCGCCTGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,F12---D712-D506--AGCGATAG-TAATCTTA-,hg19,AGCGATAGAT,TAAGATTAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,G12---D712-D507--AGCGATAG-CAGGACGT-,hg19,AGCGATAGAT,ACGTCCTGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,H12---D712-D508--AGCGATAG-GTACTGAC-,hg19,AGCGATAGAT,GTCAGTACGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,Duplex-primer--6-F1---TTCCAAGG-CCTTGTAG-,hg19,TTCCAAGGAT,CTACAAGGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,Duplex-primer--10-B2---ATCGATCG-TGCTTCCA-,hg19,ATCGATCGAT,TGGAAGCAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,Duplex-primer--14-F2---TGGACTCT-CCGTAAGA-,hg19,TGGACTCTAT,TCTTACGGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,Duplex-primer--4-D1---GAGACGAT-TAACCGGT-,hg19,GAGACGATAT,ACCGGTTAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,Duplex-primer--13-E2---TACGCTAC-ATCACACG-,hg19,TACGCTACAT,CGTGTGATGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,Duplex-primer--7-G1---CGCATGAT-TCAGGCTT-,hg19,CGCATGATAT,AAGCCTGAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,Duplex-primer--9-A2---CGGCTAAT-AGAACGAG-,hg19,CGGCTAATAT,CTCGTTCTGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,Duplex-primer--12-D2---GCTATCCT-CACCTGTT-,hg19,GCTATCCTAT,AACAGGTGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,Duplex-primer--1-A1---CTGATCGT-ATATGCGC-,hg19,CTGATCGTAT,GCGCATATGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,Duplex-primer--15-G2---AGAGTAGC-TACGCCTT-,hg19,AGAGTAGCAT,AAGGCGTAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,Duplex-primer--11-C2---GCAAGATC-CTTCGACT-,hg19,GCAAGATCAT,AGTCGAAGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,Duplex-primer--2-B1---ACTCTCGA-TGGTACAG-,hg19,ACTCTCGAAT,CTGTACCAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,Duplex-primer--3-C1---TGAGCTAG-AACCGTTC-,hg19,TGAGCTAGAT,GAACGGTTGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,Duplex-primer--8-H1---ACGGAACA-GTTCTCGT-,hg19,ACGGAACAAT,ACGAGAACGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,Duplex-primer--5-E1---CTTGTCGA-GAACATCG-,hg19,CTTGTCGAAT,CGATGTTCGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,1,Duplex-primer--16-H2---ATCCAGAG-CGACGTTA-,hg19,ATCCAGAGAT,TAACGTCGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,C07---UDI0051,hg19,AACAGGTTAT,CTTGGTATGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,H06---UDI0048,hg19,ACCTTGGCAT,ATGAGGCCGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,B07---UDI0050,hg19,GCGCTCTAAT,GTCGGAGCGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,G06---UDI0047,hg19,GTTCCAATAT,GCAGAATTGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,E07---UDI0053,hg19,CAACAATGAT,CCGTGAAGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,F07---UDI0054,hg19,TGGTGGCAAT,TTACAGGAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,C06---UDI0043,hg19,AAGATACTAT,ATGTAAGTGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,F06---UDI0046,hg19,GCAATGCAAT,AACGTTCCGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,A06---UDI0041,hg19,ATATGGATAT,TAATACAGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,G05---UDI0039,hg19,TAAGTGGTAT,GGCTTAAGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,F08---UDI0062,hg19,TAAGGTCAAT,CTACGACAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,B06---UDI0042,hg19,GCGCAAGCAT,CGGCGTGAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,H07---UDI0056,hg19,GAATGAGAAT,AATGCCTCGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,H10---UDI0080,hg19,GTGAATATAT,GAATGAGAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,G07---UDI0055,hg19,AGGCAGAGAT,GGCATTCTGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,G08---UDI0063,hg19,TTGCCTAGAT,TAAGTGGTGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,B05---UDI0034,hg19,CGTTAGAAAT,GACCTGAAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,E04---UDI0029,hg19,CCGTGAAGAT,ATCCACTGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,D05---UDI0036,hg19,GATTCTGCAT,CTCTCGTCGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,C05---UDI0035,hg19,AGCCTCATAT,TCTCTACTGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,D04---UDI0028,hg19,TCCAACGCAT,AAGTCCAAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,E08---UDI0061,hg19,CGGAACTGAT,TCGTAGTGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,D08---UDI0060,hg19,AGCTCGCTAT,GATTCTGCGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,C10---UDI0075,hg19,AGTACTCCAT,AACAGGTTGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,F05---UDI0038,hg19,CTACGACAAT,TTGGACTCGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,A10---UDI0073,hg19,CAATTAACAT,ATATCTCGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,E06---UDI0045,hg19,ATGGCATGAT,GGTACCTTGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,A11---UDI0081,hg19,AACTGTAGAT,TGCGGCGTGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,D06---UDI0044,hg19,GGAGCGTCAT,GCACGGACGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,B10---UDI0074,hg19,TGGCCGGTAT,GCGCTCTAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,E05---UDI0037,hg19,TCGTAGTGAT,CCAAGTCTGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,D07---UDI0052,hg19,GGTGAACCAT,TCCAACGCGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,A09---UDI0065,hg19,ACACTAAGAT,ATATGGATGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,C09---UDI0067,hg19,TTCCTGTTAT,AAGATACTGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,C12---UDI0091,hg19,GTATGTTCAT,TTCCTGTTGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,A03---UDI0017,hg19,TAATACAGAT,GTGAATATGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,E09---UDI0069,hg19,GCCACAGGAT,ATGGCATGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,G10---UDI0079,hg19,ACAGGCGCAT,AGGCAGAGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,B12---UDI0090,hg19,CGCTATGTAT,GTGTCGGAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,F04---UDI0030,hg19,TTACAGGAAT,GCTTGTCAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,B09---UDI0066,hg19,GTGTCGGAAT,GCGCAAGCGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,D10---UDI0076,hg19,GACGTCTTAT,GGTGAACCGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,E12---UDI0093,hg19,TACTCATAAT,GCCACAGGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,F10---UDI0078,hg19,CATAGAGTAT,TGGTGGCAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,B03---UDI0018,hg19,CGGCGTGAAT,ACAGGCGCGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,D09---UDI0068,hg19,CCTTCACCAT,GGAGCGTCGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,C03---UDI0019,hg19,ATGTAAGTAT,CATAGAGTGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,D12---UDI0092,hg19,ACGCACCTAT,CCTTCACCGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,E10---UDI0077,hg19,TGCGAGACAT,CAACAATGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,H02---UDI0016,hg19,AATCCGGAAT,AACTGTAGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,A05---UDI0033,hg19,TACCGAGGAT,AGTTCAGGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,A07---UDI0049,hg19,ATATCTCGAT,ACTAAGATGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,H08---UDI0064,hg19,CCATTCGAAT,CGGACAACGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,G02---UDI0015,hg19,GGCTTAAGAT,GGTCACGAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,F12---UDI0094,hg19,CGTCTGCGAT,ATTGTGAAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,H12---UDI0096,hg19,CTAGCGCTAT,GTCTACACGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,G04---UDI0031,hg19,GGCATTCTAT,CAAGCTAGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,H04---UDI0032,hg19,AATGCCTCAT,TGGATCGAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,G12---UDI0095,hg19,TCGATATCAT,ACTCGTGTGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,A01---UDI0001,hg19,CCGCGGTTAT,CTAGCGCTGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,B01---UDI0002,hg19,TTATAACCAT,TCGATATCGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,D01---UDI0004,hg19,AAGTCCAAAT,TACTCATAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,E01---UDI0005,hg19,ATCCACTGAT,ACGCACCTGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,G01---UDI0007,hg19,CAAGCTAGAT,CGCTATGTGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,A12---UDI0089,hg19,TATCGCACAT,ACACTAAGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,E02---UDI0013,hg19,CCAAGTCTAT,TCATCCTTGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,F02---UDI0014,hg19,TTGGACTCAT,CTGCTTCCGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,F01---UDI0006,hg19,GCTTGTCAAT,GTATGTTCGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,D03---UDI0020,hg19,GCACGGACAT,TGCGAGACGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,D02---UDI0012,hg19,CTCTCGTCAT,AGGTTATAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,B02---UDI0010,hg19,GACCTGAAAT,CTCACCAAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,C02---UDI0011,hg19,TCTCTACTAT,GAACCGCGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,C01---UDI0003,hg19,GGACTTGGAT,CGTCTGCGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,E11---UDI0085,hg19,AGGTTATAAT,CGGAACTGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,D11---UDI0084,hg19,TCATCCTTAT,AGCTCGCTGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,G11---UDI0087,hg19,CTCACCAAAT,TTGCCTAGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,A02---UDI0009,hg19,AGTTCAGGAT,TCTGTTGGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,H05---UDI0040,hg19,CGGACAACAT,AATCCGGAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,B11---UDI0082,hg19,GGTCACGAAT,CATAATACGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,C08---UDI0059,hg19,GATCTATCAT,AGCCTCATGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,C11---UDI0083,hg19,CTGCTTCCAT,GATCTATCGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,F11---UDI0086,hg19,GAACCGCGAT,TAAGGTCAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,C04---UDI0027,hg19,CTTGGTATAT,GGACTTGGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,B04---UDI0026,hg19,GTCGGAGCAT,TTATAACCGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,E03---UDI0021,hg19,GGTACCTTAT,GACGTCTTGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,F09---UDI0070,hg19,ATTGTGAAAT,GCAATGCAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,G09---UDI0071,hg19,ACTCGTGTAT,GTTCCAATGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,F03---UDI0022,hg19,AACGTTCCAT,AGTACTCCGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,G03---UDI0023,hg19,GCAGAATTAT,TGGCCGGTGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,H09---UDI0072,hg19,GTCTACACAT,ACCTTGGCGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,A04---UDI0025,hg19,ACTAAGATAT,CCGCGGTTGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,H01---UDI0008,hg19,TGGATCGAAT,TATCGCACGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,B08---UDI0058,hg19,CATAATACAT,CGTTAGAAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,H11---UDI0088,hg19,TCTGTTGGAT,CCATTCGAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,H03---UDI0024,hg19,ATGAGGCCAT,CAATTAACGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,A08---UDI0057,hg19,TGCGGCGTAT,TACCGAGGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,A01---D701-D501--ATTACTCG-TATAGCCT-,hg19,ATTACTCGAT,AGGCTATAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,B01---D701-D502--ATTACTCG-ATAGAGGC-,hg19,ATTACTCGAT,GCCTCTATGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,C01---D701-D503--ATTACTCG-CCTATCCT-,hg19,ATTACTCGAT,AGGATAGGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,D01---D701-D504--ATTACTCG-GGCTCTGA-,hg19,ATTACTCGAT,TCAGAGCCGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,E01---D701-D505--ATTACTCG-AGGCGAAG-,hg19,ATTACTCGAT,CTTCGCCTGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,F01---D701-D506--ATTACTCG-TAATCTTA-,hg19,ATTACTCGAT,TAAGATTAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,G01---D701-D507--ATTACTCG-CAGGACGT-,hg19,ATTACTCGAT,ACGTCCTGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,H01---D701-D508--ATTACTCG-GTACTGAC-,hg19,ATTACTCGAT,GTCAGTACGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,A02---D702-D501--TCCGGAGA-TATAGCCT-,hg19,TCCGGAGAAT,AGGCTATAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,B02---D702-D502--TCCGGAGA-ATAGAGGC-,hg19,TCCGGAGAAT,GCCTCTATGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,C02---D702-D503--TCCGGAGA-CCTATCCT-,hg19,TCCGGAGAAT,AGGATAGGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,D02---D702-D504--TCCGGAGA-GGCTCTGA-,hg19,TCCGGAGAAT,TCAGAGCCGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,E02---D702-D505--TCCGGAGA-AGGCGAAG-,hg19,TCCGGAGAAT,CTTCGCCTGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,F02---D702-D506--TCCGGAGA-TAATCTTA-,hg19,TCCGGAGAAT,TAAGATTAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,G02---D702-D507--TCCGGAGA-CAGGACGT-,hg19,TCCGGAGAAT,ACGTCCTGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,H02---D702-D508--TCCGGAGA-GTACTGAC-,hg19,TCCGGAGAAT,GTCAGTACGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,A03---D703-D501--CGCTCATT-TATAGCCT-,hg19,CGCTCATTAT,AGGCTATAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,B03---D703-D502--CGCTCATT-ATAGAGGC-,hg19,CGCTCATTAT,GCCTCTATGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,C03---D703-D503--CGCTCATT-CCTATCCT-,hg19,CGCTCATTAT,AGGATAGGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,D03---D703-D504--CGCTCATT-GGCTCTGA-,hg19,CGCTCATTAT,TCAGAGCCGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,E03---D703-D505--CGCTCATT-AGGCGAAG-,hg19,CGCTCATTAT,CTTCGCCTGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,F03---D703-D506--CGCTCATT-TAATCTTA-,hg19,CGCTCATTAT,TAAGATTAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,G03---D703-D507--CGCTCATT-CAGGACGT-,hg19,CGCTCATTAT,ACGTCCTGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,H03---D703-D508--CGCTCATT-GTACTGAC-,hg19,CGCTCATTAT,GTCAGTACGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,A04---D704-D501--GAGATTCC-TATAGCCT-,hg19,GAGATTCCAT,AGGCTATAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,B04---D704-D502--GAGATTCC-ATAGAGGC-,hg19,GAGATTCCAT,GCCTCTATGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,C04---D704-D503--GAGATTCC-CCTATCCT-,hg19,GAGATTCCAT,AGGATAGGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,D04---D704-D504--GAGATTCC-GGCTCTGA-,hg19,GAGATTCCAT,TCAGAGCCGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,E04---D704-D505--GAGATTCC-AGGCGAAG-,hg19,GAGATTCCAT,CTTCGCCTGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,F04---D704-D506--GAGATTCC-TAATCTTA-,hg19,GAGATTCCAT,TAAGATTAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,G04---D704-D507--GAGATTCC-CAGGACGT-,hg19,GAGATTCCAT,ACGTCCTGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,H04---D704-D508--GAGATTCC-GTACTGAC-,hg19,GAGATTCCAT,GTCAGTACGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,A05---D705-D501--ATTCAGAA-TATAGCCT-,hg19,ATTCAGAAAT,AGGCTATAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,B05---D705-D502--ATTCAGAA-ATAGAGGC-,hg19,ATTCAGAAAT,GCCTCTATGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,C05---D705-D503--ATTCAGAA-CCTATCCT-,hg19,ATTCAGAAAT,AGGATAGGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,D05---D705-D504--ATTCAGAA-GGCTCTGA-,hg19,ATTCAGAAAT,TCAGAGCCGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,E05---D705-D505--ATTCAGAA-AGGCGAAG-,hg19,ATTCAGAAAT,CTTCGCCTGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,F05---D705-D506--ATTCAGAA-TAATCTTA-,hg19,ATTCAGAAAT,TAAGATTAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,G05---D705-D507--ATTCAGAA-CAGGACGT-,hg19,ATTCAGAAAT,ACGTCCTGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,H05---D705-D508--ATTCAGAA-GTACTGAC-,hg19,ATTCAGAAAT,GTCAGTACGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,A06---D706-D501--GAATTCGT-TATAGCCT-,hg19,GAATTCGTAT,AGGCTATAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,B06---D706-D502--GAATTCGT-ATAGAGGC-,hg19,GAATTCGTAT,GCCTCTATGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,C06---D706-D503--GAATTCGT-CCTATCCT-,hg19,GAATTCGTAT,AGGATAGGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,D06---D706-D504--GAATTCGT-GGCTCTGA-,hg19,GAATTCGTAT,TCAGAGCCGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,E06---D706-D505--GAATTCGT-AGGCGAAG-,hg19,GAATTCGTAT,CTTCGCCTGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,F06---D706-D506--GAATTCGT-TAATCTTA-,hg19,GAATTCGTAT,TAAGATTAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,G06---D706-D507--GAATTCGT-CAGGACGT-,hg19,GAATTCGTAT,ACGTCCTGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,H06---D706-D508--GAATTCGT-GTACTGAC-,hg19,GAATTCGTAT,GTCAGTACGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,A07---D707-D501--CTGAAGCT-TATAGCCT-,hg19,CTGAAGCTAT,AGGCTATAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,B07---D707-D502--CTGAAGCT-ATAGAGGC-,hg19,CTGAAGCTAT,GCCTCTATGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,C07---D707-D503--CTGAAGCT-CCTATCCT-,hg19,CTGAAGCTAT,AGGATAGGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,D07---D707-D504--CTGAAGCT-GGCTCTGA-,hg19,CTGAAGCTAT,TCAGAGCCGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,E07---D707-D505--CTGAAGCT-AGGCGAAG-,hg19,CTGAAGCTAT,CTTCGCCTGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,F07---D707-D506--CTGAAGCT-TAATCTTA-,hg19,CTGAAGCTAT,TAAGATTAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,G07---D707-D507--CTGAAGCT-CAGGACGT-,hg19,CTGAAGCTAT,ACGTCCTGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,H07---D707-D508--CTGAAGCT-GTACTGAC-,hg19,CTGAAGCTAT,GTCAGTACGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,A08---D708-D501--TAATGCGC-TATAGCCT-,hg19,TAATGCGCAT,AGGCTATAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,B08---D708-D502--TAATGCGC-ATAGAGGC-,hg19,TAATGCGCAT,GCCTCTATGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,C08---D708-D503--TAATGCGC-CCTATCCT-,hg19,TAATGCGCAT,AGGATAGGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,D08---D708-D504--TAATGCGC-GGCTCTGA-,hg19,TAATGCGCAT,TCAGAGCCGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,E08---D708-D505--TAATGCGC-AGGCGAAG-,hg19,TAATGCGCAT,CTTCGCCTGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,F08---D708-D506--TAATGCGC-TAATCTTA-,hg19,TAATGCGCAT,TAAGATTAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,G08---D708-D507--TAATGCGC-CAGGACGT-,hg19,TAATGCGCAT,ACGTCCTGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,H08---D708-D508--TAATGCGC-GTACTGAC-,hg19,TAATGCGCAT,GTCAGTACGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,A09---D709-D501--CGGCTATG-TATAGCCT-,hg19,CGGCTATGAT,AGGCTATAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,B09---D709-D502--CGGCTATG-ATAGAGGC-,hg19,CGGCTATGAT,GCCTCTATGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,C09---D709-D503--CGGCTATG-CCTATCCT-,hg19,CGGCTATGAT,AGGATAGGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,D09---D709-D504--CGGCTATG-GGCTCTGA-,hg19,CGGCTATGAT,TCAGAGCCGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,E09---D709-D505--CGGCTATG-AGGCGAAG-,hg19,CGGCTATGAT,CTTCGCCTGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,F09---D709-D506--CGGCTATG-TAATCTTA-,hg19,CGGCTATGAT,TAAGATTAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,G09---D709-D507--CGGCTATG-CAGGACGT-,hg19,CGGCTATGAT,ACGTCCTGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,H09---D709-D508--CGGCTATG-GTACTGAC-,hg19,CGGCTATGAT,GTCAGTACGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,A10---D710-D501--TCCGCGAA-TATAGCCT-,hg19,TCCGCGAAAT,AGGCTATAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,B10---D710-D502--TCCGCGAA-ATAGAGGC-,hg19,TCCGCGAAAT,GCCTCTATGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,C10---D710-D503--TCCGCGAA-CCTATCCT-,hg19,TCCGCGAAAT,AGGATAGGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,D10---D710-D504--TCCGCGAA-GGCTCTGA-,hg19,TCCGCGAAAT,TCAGAGCCGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,E10---D710-D505--TCCGCGAA-AGGCGAAG-,hg19,TCCGCGAAAT,CTTCGCCTGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,F10---D710-D506--TCCGCGAA-TAATCTTA-,hg19,TCCGCGAAAT,TAAGATTAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,G10---D710-D507--TCCGCGAA-CAGGACGT-,hg19,TCCGCGAAAT,ACGTCCTGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,H10---D710-D508--TCCGCGAA-GTACTGAC-,hg19,TCCGCGAAAT,GTCAGTACGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,A11---D711-D501--TCTCGCGC-TATAGCCT-,hg19,TCTCGCGCAT,AGGCTATAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,B11---D711-D502--TCTCGCGC-ATAGAGGC-,hg19,TCTCGCGCAT,GCCTCTATGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,C11---D711-D503--TCTCGCGC-CCTATCCT-,hg19,TCTCGCGCAT,AGGATAGGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,D11---D711-D504--TCTCGCGC-GGCTCTGA-,hg19,TCTCGCGCAT,TCAGAGCCGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,E11---D711-D505--TCTCGCGC-AGGCGAAG-,hg19,TCTCGCGCAT,CTTCGCCTGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,F11---D711-D506--TCTCGCGC-TAATCTTA-,hg19,TCTCGCGCAT,TAAGATTAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,G11---D711-D507--TCTCGCGC-CAGGACGT-,hg19,TCTCGCGCAT,ACGTCCTGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,H11---D711-D508--TCTCGCGC-GTACTGAC-,hg19,TCTCGCGCAT,GTCAGTACGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,A12---D712-D501--AGCGATAG-TATAGCCT-,hg19,AGCGATAGAT,AGGCTATAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,B12---D712-D502--AGCGATAG-ATAGAGGC-,hg19,AGCGATAGAT,GCCTCTATGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,C12---D712-D503--AGCGATAG-CCTATCCT-,hg19,AGCGATAGAT,AGGATAGGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,D12---D712-D504--AGCGATAG-GGCTCTGA-,hg19,AGCGATAGAT,TCAGAGCCGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,E12---D712-D505--AGCGATAG-AGGCGAAG-,hg19,AGCGATAGAT,CTTCGCCTGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,F12---D712-D506--AGCGATAG-TAATCTTA-,hg19,AGCGATAGAT,TAAGATTAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,G12---D712-D507--AGCGATAG-CAGGACGT-,hg19,AGCGATAGAT,ACGTCCTGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,H12---D712-D508--AGCGATAG-GTACTGAC-,hg19,AGCGATAGAT,GTCAGTACGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,Duplex-primer--6-F1---TTCCAAGG-CCTTGTAG-,hg19,TTCCAAGGAT,CTACAAGGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,Duplex-primer--10-B2---ATCGATCG-TGCTTCCA-,hg19,ATCGATCGAT,TGGAAGCAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,Duplex-primer--14-F2---TGGACTCT-CCGTAAGA-,hg19,TGGACTCTAT,TCTTACGGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,Duplex-primer--4-D1---GAGACGAT-TAACCGGT-,hg19,GAGACGATAT,ACCGGTTAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,Duplex-primer--13-E2---TACGCTAC-ATCACACG-,hg19,TACGCTACAT,CGTGTGATGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,Duplex-primer--7-G1---CGCATGAT-TCAGGCTT-,hg19,CGCATGATAT,AAGCCTGAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,Duplex-primer--9-A2---CGGCTAAT-AGAACGAG-,hg19,CGGCTAATAT,CTCGTTCTGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,Duplex-primer--12-D2---GCTATCCT-CACCTGTT-,hg19,GCTATCCTAT,AACAGGTGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,Duplex-primer--1-A1---CTGATCGT-ATATGCGC-,hg19,CTGATCGTAT,GCGCATATGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,Duplex-primer--15-G2---AGAGTAGC-TACGCCTT-,hg19,AGAGTAGCAT,AAGGCGTAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,Duplex-primer--11-C2---GCAAGATC-CTTCGACT-,hg19,GCAAGATCAT,AGTCGAAGGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,Duplex-primer--2-B1---ACTCTCGA-TGGTACAG-,hg19,ACTCTCGAAT,CTGTACCAGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,Duplex-primer--3-C1---TGAGCTAG-AACCGTTC-,hg19,TGAGCTAGAT,GAACGGTTGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,Duplex-primer--8-H1---ACGGAACA-GTTCTCGT-,hg19,ACGGAACAAT,ACGAGAACGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,Duplex-primer--5-E1---CTTGTCGA-GAACATCG-,hg19,CTTGTCGAAT,CGATGTTCGT,indexcheck,N,R1,script,indexcheck
-HVKJCDRXX,2,Duplex-primer--16-H2---ATCCAGAG-CGACGTTA-,hg19,ATCCAGAGAT,TAACGTCGGT,indexcheck,N,R1,script,indexcheck
+FCID,Lane,Sample_ID,SampleRef,index,index2,SampleName,Control,Recipe,Operator,Sample_Project
+HY7FFDRX2,1,ACC11927A2,hg19,GTCCTTCGGC,CTGTGCATGA,p023BCR,N,R1,script,405887
+HY7FFDRX2,1,ACC11927A5,hg19,GTTTCACGAT,TTTGGCCGAA,p023bLBCR,N,R1,script,405887
+HY7FFDRX2,1,ACC11927A4,hg19,GAGCAAGGGC,CCAAGTCAAT,p023bLcDNA,N,R1,script,405887
+HY7FFDRX2,1,ACC11927A6,hg19,AATGTATCCA,TAAGCTCATT,p023bLTCR,N,R1,script,405887
+HY7FFDRX2,1,ACC11927A8,hg19,CGAAGTATAC,CTCCAAGTTC,p023bRBCR,N,R1,script,405887
+HY7FFDRX2,1,ACC11927A7,hg19,CTCCTTTAGA,GAGCTATGTC,p023bRcDNA,N,R1,script,405887
+HY7FFDRX2,1,ACC11927A9,hg19,ACCTCGAGCT,ATCGAACACA,p023bRTCR,N,R1,script,405887
+HY7FFDRX2,1,ACC11927A1,hg19,CGCTGAAATC,GCAGACACCT,p023cDNA,N,R1,script,405887
+HY7FFDRX2,1,ACC11927A3,hg19,CCTGTCAGGG,GTTACGGGCT,p023TCR,N,R1,script,405887
+HY7FFDRX2,2,ACC11927A2,hg19,GTCCTTCGGC,CTGTGCATGA,p023BCR,N,R1,script,405887
+HY7FFDRX2,2,ACC11927A5,hg19,GTTTCACGAT,TTTGGCCGAA,p023bLBCR,N,R1,script,405887
+HY7FFDRX2,2,ACC11927A4,hg19,GAGCAAGGGC,CCAAGTCAAT,p023bLcDNA,N,R1,script,405887
+HY7FFDRX2,2,ACC11927A6,hg19,AATGTATCCA,TAAGCTCATT,p023bLTCR,N,R1,script,405887
+HY7FFDRX2,2,ACC11927A8,hg19,CGAAGTATAC,CTCCAAGTTC,p023bRBCR,N,R1,script,405887
+HY7FFDRX2,2,ACC11927A7,hg19,CTCCTTTAGA,GAGCTATGTC,p023bRcDNA,N,R1,script,405887
+HY7FFDRX2,2,ACC11927A9,hg19,ACCTCGAGCT,ATCGAACACA,p023bRTCR,N,R1,script,405887
+HY7FFDRX2,2,ACC11927A1,hg19,CGCTGAAATC,GCAGACACCT,p023cDNA,N,R1,script,405887
+HY7FFDRX2,2,ACC11927A3,hg19,CCTGTCAGGG,GTTACGGGCT,p023TCR,N,R1,script,405887
+HY7FFDRX2,1,C07---UDI0051,hg19,AACAGGTTAT,CTTGGTATGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,H06---UDI0048,hg19,ACCTTGGCAT,ATGAGGCCGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,B07---UDI0050,hg19,GCGCTCTAAT,GTCGGAGCGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,G06---UDI0047,hg19,GTTCCAATAT,GCAGAATTGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,E07---UDI0053,hg19,CAACAATGAT,CCGTGAAGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,F07---UDI0054,hg19,TGGTGGCAAT,TTACAGGAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,C06---UDI0043,hg19,AAGATACTAT,ATGTAAGTGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,F06---UDI0046,hg19,GCAATGCAAT,AACGTTCCGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,A06---UDI0041,hg19,ATATGGATAT,TAATACAGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,G05---UDI0039,hg19,TAAGTGGTAT,GGCTTAAGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,F08---UDI0062,hg19,TAAGGTCAAT,CTACGACAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,B06---UDI0042,hg19,GCGCAAGCAT,CGGCGTGAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,H07---UDI0056,hg19,GAATGAGAAT,AATGCCTCGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,H10---UDI0080,hg19,GTGAATATAT,GAATGAGAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,G07---UDI0055,hg19,AGGCAGAGAT,GGCATTCTGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,G08---UDI0063,hg19,TTGCCTAGAT,TAAGTGGTGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,B05---UDI0034,hg19,CGTTAGAAAT,GACCTGAAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,E04---UDI0029,hg19,CCGTGAAGAT,ATCCACTGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,D05---UDI0036,hg19,GATTCTGCAT,CTCTCGTCGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,C05---UDI0035,hg19,AGCCTCATAT,TCTCTACTGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,D04---UDI0028,hg19,TCCAACGCAT,AAGTCCAAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,E08---UDI0061,hg19,CGGAACTGAT,TCGTAGTGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,D08---UDI0060,hg19,AGCTCGCTAT,GATTCTGCGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,C10---UDI0075,hg19,AGTACTCCAT,AACAGGTTGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,F05---UDI0038,hg19,CTACGACAAT,TTGGACTCGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,A10---UDI0073,hg19,CAATTAACAT,ATATCTCGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,E06---UDI0045,hg19,ATGGCATGAT,GGTACCTTGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,A11---UDI0081,hg19,AACTGTAGAT,TGCGGCGTGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,D06---UDI0044,hg19,GGAGCGTCAT,GCACGGACGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,B10---UDI0074,hg19,TGGCCGGTAT,GCGCTCTAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,E05---UDI0037,hg19,TCGTAGTGAT,CCAAGTCTGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,D07---UDI0052,hg19,GGTGAACCAT,TCCAACGCGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,A09---UDI0065,hg19,ACACTAAGAT,ATATGGATGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,C09---UDI0067,hg19,TTCCTGTTAT,AAGATACTGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,C12---UDI0091,hg19,GTATGTTCAT,TTCCTGTTGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,A03---UDI0017,hg19,TAATACAGAT,GTGAATATGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,E09---UDI0069,hg19,GCCACAGGAT,ATGGCATGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,G10---UDI0079,hg19,ACAGGCGCAT,AGGCAGAGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,B12---UDI0090,hg19,CGCTATGTAT,GTGTCGGAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,F04---UDI0030,hg19,TTACAGGAAT,GCTTGTCAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,B09---UDI0066,hg19,GTGTCGGAAT,GCGCAAGCGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,D10---UDI0076,hg19,GACGTCTTAT,GGTGAACCGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,E12---UDI0093,hg19,TACTCATAAT,GCCACAGGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,F10---UDI0078,hg19,CATAGAGTAT,TGGTGGCAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,B03---UDI0018,hg19,CGGCGTGAAT,ACAGGCGCGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,D09---UDI0068,hg19,CCTTCACCAT,GGAGCGTCGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,C03---UDI0019,hg19,ATGTAAGTAT,CATAGAGTGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,D12---UDI0092,hg19,ACGCACCTAT,CCTTCACCGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,E10---UDI0077,hg19,TGCGAGACAT,CAACAATGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,H02---UDI0016,hg19,AATCCGGAAT,AACTGTAGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,A05---UDI0033,hg19,TACCGAGGAT,AGTTCAGGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,A07---UDI0049,hg19,ATATCTCGAT,ACTAAGATGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,H08---UDI0064,hg19,CCATTCGAAT,CGGACAACGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,G02---UDI0015,hg19,GGCTTAAGAT,GGTCACGAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,F12---UDI0094,hg19,CGTCTGCGAT,ATTGTGAAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,H12---UDI0096,hg19,CTAGCGCTAT,GTCTACACGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,G04---UDI0031,hg19,GGCATTCTAT,CAAGCTAGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,H04---UDI0032,hg19,AATGCCTCAT,TGGATCGAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,G12---UDI0095,hg19,TCGATATCAT,ACTCGTGTGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,A01---UDI0001,hg19,CCGCGGTTAT,CTAGCGCTGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,B01---UDI0002,hg19,TTATAACCAT,TCGATATCGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,D01---UDI0004,hg19,AAGTCCAAAT,TACTCATAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,E01---UDI0005,hg19,ATCCACTGAT,ACGCACCTGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,G01---UDI0007,hg19,CAAGCTAGAT,CGCTATGTGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,A12---UDI0089,hg19,TATCGCACAT,ACACTAAGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,E02---UDI0013,hg19,CCAAGTCTAT,TCATCCTTGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,F02---UDI0014,hg19,TTGGACTCAT,CTGCTTCCGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,F01---UDI0006,hg19,GCTTGTCAAT,GTATGTTCGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,D03---UDI0020,hg19,GCACGGACAT,TGCGAGACGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,D02---UDI0012,hg19,CTCTCGTCAT,AGGTTATAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,B02---UDI0010,hg19,GACCTGAAAT,CTCACCAAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,C02---UDI0011,hg19,TCTCTACTAT,GAACCGCGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,C01---UDI0003,hg19,GGACTTGGAT,CGTCTGCGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,E11---UDI0085,hg19,AGGTTATAAT,CGGAACTGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,D11---UDI0084,hg19,TCATCCTTAT,AGCTCGCTGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,G11---UDI0087,hg19,CTCACCAAAT,TTGCCTAGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,A02---UDI0009,hg19,AGTTCAGGAT,TCTGTTGGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,H05---UDI0040,hg19,CGGACAACAT,AATCCGGAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,B11---UDI0082,hg19,GGTCACGAAT,CATAATACGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,C08---UDI0059,hg19,GATCTATCAT,AGCCTCATGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,C11---UDI0083,hg19,CTGCTTCCAT,GATCTATCGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,F11---UDI0086,hg19,GAACCGCGAT,TAAGGTCAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,C04---UDI0027,hg19,CTTGGTATAT,GGACTTGGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,B04---UDI0026,hg19,GTCGGAGCAT,TTATAACCGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,E03---UDI0021,hg19,GGTACCTTAT,GACGTCTTGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,F09---UDI0070,hg19,ATTGTGAAAT,GCAATGCAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,G09---UDI0071,hg19,ACTCGTGTAT,GTTCCAATGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,F03---UDI0022,hg19,AACGTTCCAT,AGTACTCCGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,G03---UDI0023,hg19,GCAGAATTAT,TGGCCGGTGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,H09---UDI0072,hg19,GTCTACACAT,ACCTTGGCGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,A04---UDI0025,hg19,ACTAAGATAT,CCGCGGTTGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,H01---UDI0008,hg19,TGGATCGAAT,TATCGCACGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,B08---UDI0058,hg19,CATAATACAT,CGTTAGAAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,H11---UDI0088,hg19,TCTGTTGGAT,CCATTCGAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,H03---UDI0024,hg19,ATGAGGCCAT,CAATTAACGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,A08---UDI0057,hg19,TGCGGCGTAT,TACCGAGGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,A01---D701-D501--ATTACTCG-TATAGCCT-,hg19,ATTACTCGAT,AGGCTATAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,B01---D701-D502--ATTACTCG-ATAGAGGC-,hg19,ATTACTCGAT,GCCTCTATGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,C01---D701-D503--ATTACTCG-CCTATCCT-,hg19,ATTACTCGAT,AGGATAGGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,D01---D701-D504--ATTACTCG-GGCTCTGA-,hg19,ATTACTCGAT,TCAGAGCCGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,E01---D701-D505--ATTACTCG-AGGCGAAG-,hg19,ATTACTCGAT,CTTCGCCTGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,F01---D701-D506--ATTACTCG-TAATCTTA-,hg19,ATTACTCGAT,TAAGATTAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,G01---D701-D507--ATTACTCG-CAGGACGT-,hg19,ATTACTCGAT,ACGTCCTGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,H01---D701-D508--ATTACTCG-GTACTGAC-,hg19,ATTACTCGAT,GTCAGTACGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,A02---D702-D501--TCCGGAGA-TATAGCCT-,hg19,TCCGGAGAAT,AGGCTATAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,B02---D702-D502--TCCGGAGA-ATAGAGGC-,hg19,TCCGGAGAAT,GCCTCTATGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,C02---D702-D503--TCCGGAGA-CCTATCCT-,hg19,TCCGGAGAAT,AGGATAGGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,D02---D702-D504--TCCGGAGA-GGCTCTGA-,hg19,TCCGGAGAAT,TCAGAGCCGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,E02---D702-D505--TCCGGAGA-AGGCGAAG-,hg19,TCCGGAGAAT,CTTCGCCTGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,F02---D702-D506--TCCGGAGA-TAATCTTA-,hg19,TCCGGAGAAT,TAAGATTAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,G02---D702-D507--TCCGGAGA-CAGGACGT-,hg19,TCCGGAGAAT,ACGTCCTGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,H02---D702-D508--TCCGGAGA-GTACTGAC-,hg19,TCCGGAGAAT,GTCAGTACGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,A03---D703-D501--CGCTCATT-TATAGCCT-,hg19,CGCTCATTAT,AGGCTATAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,B03---D703-D502--CGCTCATT-ATAGAGGC-,hg19,CGCTCATTAT,GCCTCTATGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,C03---D703-D503--CGCTCATT-CCTATCCT-,hg19,CGCTCATTAT,AGGATAGGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,D03---D703-D504--CGCTCATT-GGCTCTGA-,hg19,CGCTCATTAT,TCAGAGCCGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,E03---D703-D505--CGCTCATT-AGGCGAAG-,hg19,CGCTCATTAT,CTTCGCCTGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,F03---D703-D506--CGCTCATT-TAATCTTA-,hg19,CGCTCATTAT,TAAGATTAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,G03---D703-D507--CGCTCATT-CAGGACGT-,hg19,CGCTCATTAT,ACGTCCTGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,H03---D703-D508--CGCTCATT-GTACTGAC-,hg19,CGCTCATTAT,GTCAGTACGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,A04---D704-D501--GAGATTCC-TATAGCCT-,hg19,GAGATTCCAT,AGGCTATAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,B04---D704-D502--GAGATTCC-ATAGAGGC-,hg19,GAGATTCCAT,GCCTCTATGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,C04---D704-D503--GAGATTCC-CCTATCCT-,hg19,GAGATTCCAT,AGGATAGGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,D04---D704-D504--GAGATTCC-GGCTCTGA-,hg19,GAGATTCCAT,TCAGAGCCGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,E04---D704-D505--GAGATTCC-AGGCGAAG-,hg19,GAGATTCCAT,CTTCGCCTGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,F04---D704-D506--GAGATTCC-TAATCTTA-,hg19,GAGATTCCAT,TAAGATTAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,G04---D704-D507--GAGATTCC-CAGGACGT-,hg19,GAGATTCCAT,ACGTCCTGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,H04---D704-D508--GAGATTCC-GTACTGAC-,hg19,GAGATTCCAT,GTCAGTACGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,A05---D705-D501--ATTCAGAA-TATAGCCT-,hg19,ATTCAGAAAT,AGGCTATAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,B05---D705-D502--ATTCAGAA-ATAGAGGC-,hg19,ATTCAGAAAT,GCCTCTATGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,C05---D705-D503--ATTCAGAA-CCTATCCT-,hg19,ATTCAGAAAT,AGGATAGGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,D05---D705-D504--ATTCAGAA-GGCTCTGA-,hg19,ATTCAGAAAT,TCAGAGCCGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,E05---D705-D505--ATTCAGAA-AGGCGAAG-,hg19,ATTCAGAAAT,CTTCGCCTGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,F05---D705-D506--ATTCAGAA-TAATCTTA-,hg19,ATTCAGAAAT,TAAGATTAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,G05---D705-D507--ATTCAGAA-CAGGACGT-,hg19,ATTCAGAAAT,ACGTCCTGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,H05---D705-D508--ATTCAGAA-GTACTGAC-,hg19,ATTCAGAAAT,GTCAGTACGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,A06---D706-D501--GAATTCGT-TATAGCCT-,hg19,GAATTCGTAT,AGGCTATAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,B06---D706-D502--GAATTCGT-ATAGAGGC-,hg19,GAATTCGTAT,GCCTCTATGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,C06---D706-D503--GAATTCGT-CCTATCCT-,hg19,GAATTCGTAT,AGGATAGGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,D06---D706-D504--GAATTCGT-GGCTCTGA-,hg19,GAATTCGTAT,TCAGAGCCGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,E06---D706-D505--GAATTCGT-AGGCGAAG-,hg19,GAATTCGTAT,CTTCGCCTGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,F06---D706-D506--GAATTCGT-TAATCTTA-,hg19,GAATTCGTAT,TAAGATTAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,G06---D706-D507--GAATTCGT-CAGGACGT-,hg19,GAATTCGTAT,ACGTCCTGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,H06---D706-D508--GAATTCGT-GTACTGAC-,hg19,GAATTCGTAT,GTCAGTACGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,A07---D707-D501--CTGAAGCT-TATAGCCT-,hg19,CTGAAGCTAT,AGGCTATAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,B07---D707-D502--CTGAAGCT-ATAGAGGC-,hg19,CTGAAGCTAT,GCCTCTATGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,C07---D707-D503--CTGAAGCT-CCTATCCT-,hg19,CTGAAGCTAT,AGGATAGGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,D07---D707-D504--CTGAAGCT-GGCTCTGA-,hg19,CTGAAGCTAT,TCAGAGCCGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,E07---D707-D505--CTGAAGCT-AGGCGAAG-,hg19,CTGAAGCTAT,CTTCGCCTGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,F07---D707-D506--CTGAAGCT-TAATCTTA-,hg19,CTGAAGCTAT,TAAGATTAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,G07---D707-D507--CTGAAGCT-CAGGACGT-,hg19,CTGAAGCTAT,ACGTCCTGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,H07---D707-D508--CTGAAGCT-GTACTGAC-,hg19,CTGAAGCTAT,GTCAGTACGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,A08---D708-D501--TAATGCGC-TATAGCCT-,hg19,TAATGCGCAT,AGGCTATAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,B08---D708-D502--TAATGCGC-ATAGAGGC-,hg19,TAATGCGCAT,GCCTCTATGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,C08---D708-D503--TAATGCGC-CCTATCCT-,hg19,TAATGCGCAT,AGGATAGGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,D08---D708-D504--TAATGCGC-GGCTCTGA-,hg19,TAATGCGCAT,TCAGAGCCGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,E08---D708-D505--TAATGCGC-AGGCGAAG-,hg19,TAATGCGCAT,CTTCGCCTGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,F08---D708-D506--TAATGCGC-TAATCTTA-,hg19,TAATGCGCAT,TAAGATTAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,G08---D708-D507--TAATGCGC-CAGGACGT-,hg19,TAATGCGCAT,ACGTCCTGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,H08---D708-D508--TAATGCGC-GTACTGAC-,hg19,TAATGCGCAT,GTCAGTACGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,A09---D709-D501--CGGCTATG-TATAGCCT-,hg19,CGGCTATGAT,AGGCTATAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,B09---D709-D502--CGGCTATG-ATAGAGGC-,hg19,CGGCTATGAT,GCCTCTATGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,C09---D709-D503--CGGCTATG-CCTATCCT-,hg19,CGGCTATGAT,AGGATAGGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,D09---D709-D504--CGGCTATG-GGCTCTGA-,hg19,CGGCTATGAT,TCAGAGCCGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,E09---D709-D505--CGGCTATG-AGGCGAAG-,hg19,CGGCTATGAT,CTTCGCCTGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,F09---D709-D506--CGGCTATG-TAATCTTA-,hg19,CGGCTATGAT,TAAGATTAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,G09---D709-D507--CGGCTATG-CAGGACGT-,hg19,CGGCTATGAT,ACGTCCTGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,H09---D709-D508--CGGCTATG-GTACTGAC-,hg19,CGGCTATGAT,GTCAGTACGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,A10---D710-D501--TCCGCGAA-TATAGCCT-,hg19,TCCGCGAAAT,AGGCTATAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,B10---D710-D502--TCCGCGAA-ATAGAGGC-,hg19,TCCGCGAAAT,GCCTCTATGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,C10---D710-D503--TCCGCGAA-CCTATCCT-,hg19,TCCGCGAAAT,AGGATAGGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,D10---D710-D504--TCCGCGAA-GGCTCTGA-,hg19,TCCGCGAAAT,TCAGAGCCGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,E10---D710-D505--TCCGCGAA-AGGCGAAG-,hg19,TCCGCGAAAT,CTTCGCCTGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,F10---D710-D506--TCCGCGAA-TAATCTTA-,hg19,TCCGCGAAAT,TAAGATTAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,G10---D710-D507--TCCGCGAA-CAGGACGT-,hg19,TCCGCGAAAT,ACGTCCTGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,H10---D710-D508--TCCGCGAA-GTACTGAC-,hg19,TCCGCGAAAT,GTCAGTACGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,A11---D711-D501--TCTCGCGC-TATAGCCT-,hg19,TCTCGCGCAT,AGGCTATAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,B11---D711-D502--TCTCGCGC-ATAGAGGC-,hg19,TCTCGCGCAT,GCCTCTATGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,C11---D711-D503--TCTCGCGC-CCTATCCT-,hg19,TCTCGCGCAT,AGGATAGGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,D11---D711-D504--TCTCGCGC-GGCTCTGA-,hg19,TCTCGCGCAT,TCAGAGCCGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,E11---D711-D505--TCTCGCGC-AGGCGAAG-,hg19,TCTCGCGCAT,CTTCGCCTGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,F11---D711-D506--TCTCGCGC-TAATCTTA-,hg19,TCTCGCGCAT,TAAGATTAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,G11---D711-D507--TCTCGCGC-CAGGACGT-,hg19,TCTCGCGCAT,ACGTCCTGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,H11---D711-D508--TCTCGCGC-GTACTGAC-,hg19,TCTCGCGCAT,GTCAGTACGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,A12---D712-D501--AGCGATAG-TATAGCCT-,hg19,AGCGATAGAT,AGGCTATAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,B12---D712-D502--AGCGATAG-ATAGAGGC-,hg19,AGCGATAGAT,GCCTCTATGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,C12---D712-D503--AGCGATAG-CCTATCCT-,hg19,AGCGATAGAT,AGGATAGGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,D12---D712-D504--AGCGATAG-GGCTCTGA-,hg19,AGCGATAGAT,TCAGAGCCGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,E12---D712-D505--AGCGATAG-AGGCGAAG-,hg19,AGCGATAGAT,CTTCGCCTGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,F12---D712-D506--AGCGATAG-TAATCTTA-,hg19,AGCGATAGAT,TAAGATTAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,G12---D712-D507--AGCGATAG-CAGGACGT-,hg19,AGCGATAGAT,ACGTCCTGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,H12---D712-D508--AGCGATAG-GTACTGAC-,hg19,AGCGATAGAT,GTCAGTACGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,Duplex-primer--6-F1---TTCCAAGG-CCTTGTAG-,hg19,TTCCAAGGAT,CTACAAGGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,Duplex-primer--10-B2---ATCGATCG-TGCTTCCA-,hg19,ATCGATCGAT,TGGAAGCAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,Duplex-primer--14-F2---TGGACTCT-CCGTAAGA-,hg19,TGGACTCTAT,TCTTACGGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,Duplex-primer--4-D1---GAGACGAT-TAACCGGT-,hg19,GAGACGATAT,ACCGGTTAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,Duplex-primer--13-E2---TACGCTAC-ATCACACG-,hg19,TACGCTACAT,CGTGTGATGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,Duplex-primer--7-G1---CGCATGAT-TCAGGCTT-,hg19,CGCATGATAT,AAGCCTGAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,Duplex-primer--9-A2---CGGCTAAT-AGAACGAG-,hg19,CGGCTAATAT,CTCGTTCTGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,Duplex-primer--12-D2---GCTATCCT-CACCTGTT-,hg19,GCTATCCTAT,AACAGGTGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,Duplex-primer--1-A1---CTGATCGT-ATATGCGC-,hg19,CTGATCGTAT,GCGCATATGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,Duplex-primer--15-G2---AGAGTAGC-TACGCCTT-,hg19,AGAGTAGCAT,AAGGCGTAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,Duplex-primer--11-C2---GCAAGATC-CTTCGACT-,hg19,GCAAGATCAT,AGTCGAAGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,Duplex-primer--2-B1---ACTCTCGA-TGGTACAG-,hg19,ACTCTCGAAT,CTGTACCAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,Duplex-primer--3-C1---TGAGCTAG-AACCGTTC-,hg19,TGAGCTAGAT,GAACGGTTGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,Duplex-primer--8-H1---ACGGAACA-GTTCTCGT-,hg19,ACGGAACAAT,ACGAGAACGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,Duplex-primer--5-E1---CTTGTCGA-GAACATCG-,hg19,CTTGTCGAAT,CGATGTTCGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,1,Duplex-primer--16-H2---ATCCAGAG-CGACGTTA-,hg19,ATCCAGAGAT,TAACGTCGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,C07---UDI0051,hg19,AACAGGTTAT,CTTGGTATGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,H06---UDI0048,hg19,ACCTTGGCAT,ATGAGGCCGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,B07---UDI0050,hg19,GCGCTCTAAT,GTCGGAGCGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,G06---UDI0047,hg19,GTTCCAATAT,GCAGAATTGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,E07---UDI0053,hg19,CAACAATGAT,CCGTGAAGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,F07---UDI0054,hg19,TGGTGGCAAT,TTACAGGAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,C06---UDI0043,hg19,AAGATACTAT,ATGTAAGTGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,F06---UDI0046,hg19,GCAATGCAAT,AACGTTCCGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,A06---UDI0041,hg19,ATATGGATAT,TAATACAGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,G05---UDI0039,hg19,TAAGTGGTAT,GGCTTAAGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,F08---UDI0062,hg19,TAAGGTCAAT,CTACGACAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,B06---UDI0042,hg19,GCGCAAGCAT,CGGCGTGAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,H07---UDI0056,hg19,GAATGAGAAT,AATGCCTCGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,H10---UDI0080,hg19,GTGAATATAT,GAATGAGAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,G07---UDI0055,hg19,AGGCAGAGAT,GGCATTCTGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,G08---UDI0063,hg19,TTGCCTAGAT,TAAGTGGTGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,B05---UDI0034,hg19,CGTTAGAAAT,GACCTGAAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,E04---UDI0029,hg19,CCGTGAAGAT,ATCCACTGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,D05---UDI0036,hg19,GATTCTGCAT,CTCTCGTCGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,C05---UDI0035,hg19,AGCCTCATAT,TCTCTACTGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,D04---UDI0028,hg19,TCCAACGCAT,AAGTCCAAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,E08---UDI0061,hg19,CGGAACTGAT,TCGTAGTGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,D08---UDI0060,hg19,AGCTCGCTAT,GATTCTGCGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,C10---UDI0075,hg19,AGTACTCCAT,AACAGGTTGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,F05---UDI0038,hg19,CTACGACAAT,TTGGACTCGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,A10---UDI0073,hg19,CAATTAACAT,ATATCTCGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,E06---UDI0045,hg19,ATGGCATGAT,GGTACCTTGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,A11---UDI0081,hg19,AACTGTAGAT,TGCGGCGTGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,D06---UDI0044,hg19,GGAGCGTCAT,GCACGGACGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,B10---UDI0074,hg19,TGGCCGGTAT,GCGCTCTAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,E05---UDI0037,hg19,TCGTAGTGAT,CCAAGTCTGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,D07---UDI0052,hg19,GGTGAACCAT,TCCAACGCGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,A09---UDI0065,hg19,ACACTAAGAT,ATATGGATGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,C09---UDI0067,hg19,TTCCTGTTAT,AAGATACTGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,C12---UDI0091,hg19,GTATGTTCAT,TTCCTGTTGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,A03---UDI0017,hg19,TAATACAGAT,GTGAATATGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,E09---UDI0069,hg19,GCCACAGGAT,ATGGCATGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,G10---UDI0079,hg19,ACAGGCGCAT,AGGCAGAGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,B12---UDI0090,hg19,CGCTATGTAT,GTGTCGGAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,F04---UDI0030,hg19,TTACAGGAAT,GCTTGTCAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,B09---UDI0066,hg19,GTGTCGGAAT,GCGCAAGCGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,D10---UDI0076,hg19,GACGTCTTAT,GGTGAACCGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,E12---UDI0093,hg19,TACTCATAAT,GCCACAGGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,F10---UDI0078,hg19,CATAGAGTAT,TGGTGGCAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,B03---UDI0018,hg19,CGGCGTGAAT,ACAGGCGCGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,D09---UDI0068,hg19,CCTTCACCAT,GGAGCGTCGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,C03---UDI0019,hg19,ATGTAAGTAT,CATAGAGTGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,D12---UDI0092,hg19,ACGCACCTAT,CCTTCACCGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,E10---UDI0077,hg19,TGCGAGACAT,CAACAATGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,H02---UDI0016,hg19,AATCCGGAAT,AACTGTAGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,A05---UDI0033,hg19,TACCGAGGAT,AGTTCAGGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,A07---UDI0049,hg19,ATATCTCGAT,ACTAAGATGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,H08---UDI0064,hg19,CCATTCGAAT,CGGACAACGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,G02---UDI0015,hg19,GGCTTAAGAT,GGTCACGAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,F12---UDI0094,hg19,CGTCTGCGAT,ATTGTGAAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,H12---UDI0096,hg19,CTAGCGCTAT,GTCTACACGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,G04---UDI0031,hg19,GGCATTCTAT,CAAGCTAGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,H04---UDI0032,hg19,AATGCCTCAT,TGGATCGAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,G12---UDI0095,hg19,TCGATATCAT,ACTCGTGTGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,A01---UDI0001,hg19,CCGCGGTTAT,CTAGCGCTGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,B01---UDI0002,hg19,TTATAACCAT,TCGATATCGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,D01---UDI0004,hg19,AAGTCCAAAT,TACTCATAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,E01---UDI0005,hg19,ATCCACTGAT,ACGCACCTGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,G01---UDI0007,hg19,CAAGCTAGAT,CGCTATGTGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,A12---UDI0089,hg19,TATCGCACAT,ACACTAAGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,E02---UDI0013,hg19,CCAAGTCTAT,TCATCCTTGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,F02---UDI0014,hg19,TTGGACTCAT,CTGCTTCCGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,F01---UDI0006,hg19,GCTTGTCAAT,GTATGTTCGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,D03---UDI0020,hg19,GCACGGACAT,TGCGAGACGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,D02---UDI0012,hg19,CTCTCGTCAT,AGGTTATAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,B02---UDI0010,hg19,GACCTGAAAT,CTCACCAAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,C02---UDI0011,hg19,TCTCTACTAT,GAACCGCGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,C01---UDI0003,hg19,GGACTTGGAT,CGTCTGCGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,E11---UDI0085,hg19,AGGTTATAAT,CGGAACTGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,D11---UDI0084,hg19,TCATCCTTAT,AGCTCGCTGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,G11---UDI0087,hg19,CTCACCAAAT,TTGCCTAGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,A02---UDI0009,hg19,AGTTCAGGAT,TCTGTTGGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,H05---UDI0040,hg19,CGGACAACAT,AATCCGGAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,B11---UDI0082,hg19,GGTCACGAAT,CATAATACGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,C08---UDI0059,hg19,GATCTATCAT,AGCCTCATGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,C11---UDI0083,hg19,CTGCTTCCAT,GATCTATCGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,F11---UDI0086,hg19,GAACCGCGAT,TAAGGTCAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,C04---UDI0027,hg19,CTTGGTATAT,GGACTTGGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,B04---UDI0026,hg19,GTCGGAGCAT,TTATAACCGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,E03---UDI0021,hg19,GGTACCTTAT,GACGTCTTGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,F09---UDI0070,hg19,ATTGTGAAAT,GCAATGCAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,G09---UDI0071,hg19,ACTCGTGTAT,GTTCCAATGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,F03---UDI0022,hg19,AACGTTCCAT,AGTACTCCGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,G03---UDI0023,hg19,GCAGAATTAT,TGGCCGGTGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,H09---UDI0072,hg19,GTCTACACAT,ACCTTGGCGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,A04---UDI0025,hg19,ACTAAGATAT,CCGCGGTTGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,H01---UDI0008,hg19,TGGATCGAAT,TATCGCACGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,B08---UDI0058,hg19,CATAATACAT,CGTTAGAAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,H11---UDI0088,hg19,TCTGTTGGAT,CCATTCGAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,H03---UDI0024,hg19,ATGAGGCCAT,CAATTAACGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,A08---UDI0057,hg19,TGCGGCGTAT,TACCGAGGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,A01---D701-D501--ATTACTCG-TATAGCCT-,hg19,ATTACTCGAT,AGGCTATAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,B01---D701-D502--ATTACTCG-ATAGAGGC-,hg19,ATTACTCGAT,GCCTCTATGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,C01---D701-D503--ATTACTCG-CCTATCCT-,hg19,ATTACTCGAT,AGGATAGGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,D01---D701-D504--ATTACTCG-GGCTCTGA-,hg19,ATTACTCGAT,TCAGAGCCGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,E01---D701-D505--ATTACTCG-AGGCGAAG-,hg19,ATTACTCGAT,CTTCGCCTGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,F01---D701-D506--ATTACTCG-TAATCTTA-,hg19,ATTACTCGAT,TAAGATTAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,G01---D701-D507--ATTACTCG-CAGGACGT-,hg19,ATTACTCGAT,ACGTCCTGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,H01---D701-D508--ATTACTCG-GTACTGAC-,hg19,ATTACTCGAT,GTCAGTACGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,A02---D702-D501--TCCGGAGA-TATAGCCT-,hg19,TCCGGAGAAT,AGGCTATAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,B02---D702-D502--TCCGGAGA-ATAGAGGC-,hg19,TCCGGAGAAT,GCCTCTATGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,C02---D702-D503--TCCGGAGA-CCTATCCT-,hg19,TCCGGAGAAT,AGGATAGGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,D02---D702-D504--TCCGGAGA-GGCTCTGA-,hg19,TCCGGAGAAT,TCAGAGCCGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,E02---D702-D505--TCCGGAGA-AGGCGAAG-,hg19,TCCGGAGAAT,CTTCGCCTGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,F02---D702-D506--TCCGGAGA-TAATCTTA-,hg19,TCCGGAGAAT,TAAGATTAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,G02---D702-D507--TCCGGAGA-CAGGACGT-,hg19,TCCGGAGAAT,ACGTCCTGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,H02---D702-D508--TCCGGAGA-GTACTGAC-,hg19,TCCGGAGAAT,GTCAGTACGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,A03---D703-D501--CGCTCATT-TATAGCCT-,hg19,CGCTCATTAT,AGGCTATAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,B03---D703-D502--CGCTCATT-ATAGAGGC-,hg19,CGCTCATTAT,GCCTCTATGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,C03---D703-D503--CGCTCATT-CCTATCCT-,hg19,CGCTCATTAT,AGGATAGGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,D03---D703-D504--CGCTCATT-GGCTCTGA-,hg19,CGCTCATTAT,TCAGAGCCGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,E03---D703-D505--CGCTCATT-AGGCGAAG-,hg19,CGCTCATTAT,CTTCGCCTGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,F03---D703-D506--CGCTCATT-TAATCTTA-,hg19,CGCTCATTAT,TAAGATTAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,G03---D703-D507--CGCTCATT-CAGGACGT-,hg19,CGCTCATTAT,ACGTCCTGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,H03---D703-D508--CGCTCATT-GTACTGAC-,hg19,CGCTCATTAT,GTCAGTACGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,A04---D704-D501--GAGATTCC-TATAGCCT-,hg19,GAGATTCCAT,AGGCTATAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,B04---D704-D502--GAGATTCC-ATAGAGGC-,hg19,GAGATTCCAT,GCCTCTATGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,C04---D704-D503--GAGATTCC-CCTATCCT-,hg19,GAGATTCCAT,AGGATAGGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,D04---D704-D504--GAGATTCC-GGCTCTGA-,hg19,GAGATTCCAT,TCAGAGCCGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,E04---D704-D505--GAGATTCC-AGGCGAAG-,hg19,GAGATTCCAT,CTTCGCCTGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,F04---D704-D506--GAGATTCC-TAATCTTA-,hg19,GAGATTCCAT,TAAGATTAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,G04---D704-D507--GAGATTCC-CAGGACGT-,hg19,GAGATTCCAT,ACGTCCTGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,H04---D704-D508--GAGATTCC-GTACTGAC-,hg19,GAGATTCCAT,GTCAGTACGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,A05---D705-D501--ATTCAGAA-TATAGCCT-,hg19,ATTCAGAAAT,AGGCTATAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,B05---D705-D502--ATTCAGAA-ATAGAGGC-,hg19,ATTCAGAAAT,GCCTCTATGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,C05---D705-D503--ATTCAGAA-CCTATCCT-,hg19,ATTCAGAAAT,AGGATAGGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,D05---D705-D504--ATTCAGAA-GGCTCTGA-,hg19,ATTCAGAAAT,TCAGAGCCGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,E05---D705-D505--ATTCAGAA-AGGCGAAG-,hg19,ATTCAGAAAT,CTTCGCCTGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,F05---D705-D506--ATTCAGAA-TAATCTTA-,hg19,ATTCAGAAAT,TAAGATTAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,G05---D705-D507--ATTCAGAA-CAGGACGT-,hg19,ATTCAGAAAT,ACGTCCTGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,H05---D705-D508--ATTCAGAA-GTACTGAC-,hg19,ATTCAGAAAT,GTCAGTACGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,A06---D706-D501--GAATTCGT-TATAGCCT-,hg19,GAATTCGTAT,AGGCTATAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,B06---D706-D502--GAATTCGT-ATAGAGGC-,hg19,GAATTCGTAT,GCCTCTATGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,C06---D706-D503--GAATTCGT-CCTATCCT-,hg19,GAATTCGTAT,AGGATAGGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,D06---D706-D504--GAATTCGT-GGCTCTGA-,hg19,GAATTCGTAT,TCAGAGCCGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,E06---D706-D505--GAATTCGT-AGGCGAAG-,hg19,GAATTCGTAT,CTTCGCCTGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,F06---D706-D506--GAATTCGT-TAATCTTA-,hg19,GAATTCGTAT,TAAGATTAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,G06---D706-D507--GAATTCGT-CAGGACGT-,hg19,GAATTCGTAT,ACGTCCTGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,H06---D706-D508--GAATTCGT-GTACTGAC-,hg19,GAATTCGTAT,GTCAGTACGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,A07---D707-D501--CTGAAGCT-TATAGCCT-,hg19,CTGAAGCTAT,AGGCTATAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,B07---D707-D502--CTGAAGCT-ATAGAGGC-,hg19,CTGAAGCTAT,GCCTCTATGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,C07---D707-D503--CTGAAGCT-CCTATCCT-,hg19,CTGAAGCTAT,AGGATAGGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,D07---D707-D504--CTGAAGCT-GGCTCTGA-,hg19,CTGAAGCTAT,TCAGAGCCGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,E07---D707-D505--CTGAAGCT-AGGCGAAG-,hg19,CTGAAGCTAT,CTTCGCCTGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,F07---D707-D506--CTGAAGCT-TAATCTTA-,hg19,CTGAAGCTAT,TAAGATTAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,G07---D707-D507--CTGAAGCT-CAGGACGT-,hg19,CTGAAGCTAT,ACGTCCTGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,H07---D707-D508--CTGAAGCT-GTACTGAC-,hg19,CTGAAGCTAT,GTCAGTACGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,A08---D708-D501--TAATGCGC-TATAGCCT-,hg19,TAATGCGCAT,AGGCTATAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,B08---D708-D502--TAATGCGC-ATAGAGGC-,hg19,TAATGCGCAT,GCCTCTATGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,C08---D708-D503--TAATGCGC-CCTATCCT-,hg19,TAATGCGCAT,AGGATAGGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,D08---D708-D504--TAATGCGC-GGCTCTGA-,hg19,TAATGCGCAT,TCAGAGCCGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,E08---D708-D505--TAATGCGC-AGGCGAAG-,hg19,TAATGCGCAT,CTTCGCCTGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,F08---D708-D506--TAATGCGC-TAATCTTA-,hg19,TAATGCGCAT,TAAGATTAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,G08---D708-D507--TAATGCGC-CAGGACGT-,hg19,TAATGCGCAT,ACGTCCTGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,H08---D708-D508--TAATGCGC-GTACTGAC-,hg19,TAATGCGCAT,GTCAGTACGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,A09---D709-D501--CGGCTATG-TATAGCCT-,hg19,CGGCTATGAT,AGGCTATAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,B09---D709-D502--CGGCTATG-ATAGAGGC-,hg19,CGGCTATGAT,GCCTCTATGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,C09---D709-D503--CGGCTATG-CCTATCCT-,hg19,CGGCTATGAT,AGGATAGGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,D09---D709-D504--CGGCTATG-GGCTCTGA-,hg19,CGGCTATGAT,TCAGAGCCGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,E09---D709-D505--CGGCTATG-AGGCGAAG-,hg19,CGGCTATGAT,CTTCGCCTGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,F09---D709-D506--CGGCTATG-TAATCTTA-,hg19,CGGCTATGAT,TAAGATTAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,G09---D709-D507--CGGCTATG-CAGGACGT-,hg19,CGGCTATGAT,ACGTCCTGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,H09---D709-D508--CGGCTATG-GTACTGAC-,hg19,CGGCTATGAT,GTCAGTACGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,A10---D710-D501--TCCGCGAA-TATAGCCT-,hg19,TCCGCGAAAT,AGGCTATAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,B10---D710-D502--TCCGCGAA-ATAGAGGC-,hg19,TCCGCGAAAT,GCCTCTATGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,C10---D710-D503--TCCGCGAA-CCTATCCT-,hg19,TCCGCGAAAT,AGGATAGGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,D10---D710-D504--TCCGCGAA-GGCTCTGA-,hg19,TCCGCGAAAT,TCAGAGCCGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,E10---D710-D505--TCCGCGAA-AGGCGAAG-,hg19,TCCGCGAAAT,CTTCGCCTGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,F10---D710-D506--TCCGCGAA-TAATCTTA-,hg19,TCCGCGAAAT,TAAGATTAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,G10---D710-D507--TCCGCGAA-CAGGACGT-,hg19,TCCGCGAAAT,ACGTCCTGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,H10---D710-D508--TCCGCGAA-GTACTGAC-,hg19,TCCGCGAAAT,GTCAGTACGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,A11---D711-D501--TCTCGCGC-TATAGCCT-,hg19,TCTCGCGCAT,AGGCTATAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,B11---D711-D502--TCTCGCGC-ATAGAGGC-,hg19,TCTCGCGCAT,GCCTCTATGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,C11---D711-D503--TCTCGCGC-CCTATCCT-,hg19,TCTCGCGCAT,AGGATAGGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,D11---D711-D504--TCTCGCGC-GGCTCTGA-,hg19,TCTCGCGCAT,TCAGAGCCGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,E11---D711-D505--TCTCGCGC-AGGCGAAG-,hg19,TCTCGCGCAT,CTTCGCCTGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,F11---D711-D506--TCTCGCGC-TAATCTTA-,hg19,TCTCGCGCAT,TAAGATTAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,G11---D711-D507--TCTCGCGC-CAGGACGT-,hg19,TCTCGCGCAT,ACGTCCTGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,H11---D711-D508--TCTCGCGC-GTACTGAC-,hg19,TCTCGCGCAT,GTCAGTACGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,A12---D712-D501--AGCGATAG-TATAGCCT-,hg19,AGCGATAGAT,AGGCTATAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,B12---D712-D502--AGCGATAG-ATAGAGGC-,hg19,AGCGATAGAT,GCCTCTATGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,C12---D712-D503--AGCGATAG-CCTATCCT-,hg19,AGCGATAGAT,AGGATAGGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,D12---D712-D504--AGCGATAG-GGCTCTGA-,hg19,AGCGATAGAT,TCAGAGCCGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,E12---D712-D505--AGCGATAG-AGGCGAAG-,hg19,AGCGATAGAT,CTTCGCCTGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,F12---D712-D506--AGCGATAG-TAATCTTA-,hg19,AGCGATAGAT,TAAGATTAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,G12---D712-D507--AGCGATAG-CAGGACGT-,hg19,AGCGATAGAT,ACGTCCTGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,H12---D712-D508--AGCGATAG-GTACTGAC-,hg19,AGCGATAGAT,GTCAGTACGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,Duplex-primer--6-F1---TTCCAAGG-CCTTGTAG-,hg19,TTCCAAGGAT,CTACAAGGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,Duplex-primer--10-B2---ATCGATCG-TGCTTCCA-,hg19,ATCGATCGAT,TGGAAGCAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,Duplex-primer--14-F2---TGGACTCT-CCGTAAGA-,hg19,TGGACTCTAT,TCTTACGGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,Duplex-primer--4-D1---GAGACGAT-TAACCGGT-,hg19,GAGACGATAT,ACCGGTTAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,Duplex-primer--13-E2---TACGCTAC-ATCACACG-,hg19,TACGCTACAT,CGTGTGATGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,Duplex-primer--7-G1---CGCATGAT-TCAGGCTT-,hg19,CGCATGATAT,AAGCCTGAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,Duplex-primer--9-A2---CGGCTAAT-AGAACGAG-,hg19,CGGCTAATAT,CTCGTTCTGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,Duplex-primer--12-D2---GCTATCCT-CACCTGTT-,hg19,GCTATCCTAT,AACAGGTGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,Duplex-primer--1-A1---CTGATCGT-ATATGCGC-,hg19,CTGATCGTAT,GCGCATATGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,Duplex-primer--15-G2---AGAGTAGC-TACGCCTT-,hg19,AGAGTAGCAT,AAGGCGTAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,Duplex-primer--11-C2---GCAAGATC-CTTCGACT-,hg19,GCAAGATCAT,AGTCGAAGGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,Duplex-primer--2-B1---ACTCTCGA-TGGTACAG-,hg19,ACTCTCGAAT,CTGTACCAGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,Duplex-primer--3-C1---TGAGCTAG-AACCGTTC-,hg19,TGAGCTAGAT,GAACGGTTGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,Duplex-primer--8-H1---ACGGAACA-GTTCTCGT-,hg19,ACGGAACAAT,ACGAGAACGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,Duplex-primer--5-E1---CTTGTCGA-GAACATCG-,hg19,CTTGTCGAAT,CGATGTTCGT,indexcheck,N,R1,script,indexcheck
+HY7FFDRX2,2,Duplex-primer--16-H2---ATCCAGAG-CGACGTTA-,hg19,ATCCAGAGAT,TAACGTCGGT,indexcheck,N,R1,script,indexcheck
```

### Comparing `cg-33.1.1/tests/fixtures/apps/demultiplexing/RunParameters_different_index_cycles.xml` & `cg-33.1.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml`

 * *Files 15% similar despite different names*

#### Comparing `cg-33.1.1/tests/fixtures/apps/demultiplexing/RunParameters_different_index_cycles.xml` & `cg-33.1.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml`

```diff
@@ -1,100 +1,100 @@
 <?xml version="1.0" encoding="utf-8"?>
 <RunParameters xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
   <Surface>Both</Surface>
   <ReadType>PairedEnd</ReadType>
   <Side>A</Side>
-  <Read1NumberOfCycles>151</Read1NumberOfCycles>
-  <Read2NumberOfCycles>151</Read2NumberOfCycles>
-  <IndexRead1NumberOfCycles>10</IndexRead1NumberOfCycles>
+  <Read1NumberOfCycles>51</Read1NumberOfCycles>
+  <Read2NumberOfCycles>51</Read2NumberOfCycles>
+  <IndexRead1NumberOfCycles>8</IndexRead1NumberOfCycles>
   <IndexRead2NumberOfCycles>8</IndexRead2NumberOfCycles>
-  <PlannedRead1Cycles>151</PlannedRead1Cycles>
-  <PlannedRead2Cycles>151</PlannedRead2Cycles>
-  <PlannedIndex1ReadCycles>10</PlannedIndex1ReadCycles>
-  <PlannedIndex2ReadCycles>10</PlannedIndex2ReadCycles>
-  <RunNumber>226</RunNumber>
+  <PlannedRead1Cycles>51</PlannedRead1Cycles>
+  <PlannedRead2Cycles>51</PlannedRead2Cycles>
+  <PlannedIndex1ReadCycles>8</PlannedIndex1ReadCycles>
+  <PlannedIndex2ReadCycles>8</PlannedIndex2ReadCycles>
+  <RunNumber>615</RunNumber>
   <RtaVersion>v3.4.4</RtaVersion>
-  <RecipeVersion>1.7.0</RecipeVersion>
-  <ExperimentName>HMYJ7DSXY</ExperimentName>
+  <RecipeVersion>1.7.5</RecipeVersion>
+  <ExperimentName>HLG5GDRXY</ExperimentName>
   <RfidsInfo>
-    <FlowCellSerialBarcode>HMYJ7DSXY</FlowCellSerialBarcode>
-    <FlowCellPartNumber>20015843</FlowCellPartNumber>
-    <FlowCellLotNumber>20482659</FlowCellLotNumber>
-    <FlowCellExpirationdate>09/21/2021 00:00:00</FlowCellExpirationdate>
-    <FlowCellStartDate>02/06/2021 12:40:00</FlowCellStartDate>
+    <FlowCellSerialBarcode>HLG5GDRXY</FlowCellSerialBarcode>
+    <FlowCellPartNumber>20026406</FlowCellPartNumber>
+    <FlowCellLotNumber>20574340</FlowCellLotNumber>
+    <FlowCellExpirationdate>08/19/2022 00:00:00</FlowCellExpirationdate>
+    <FlowCellStartDate>11/01/2021 11:50:00</FlowCellStartDate>
     <FlowCellNumberOfReuseRemaining>1</FlowCellNumberOfReuseRemaining>
-    <FlowCellSupportedModes>HTWashOnly;S4</FlowCellSupportedModes>
-    <FlowCellMode>S4</FlowCellMode>
+    <FlowCellSupportedModes>LTWashOnly;SP</FlowCellSupportedModes>
+    <FlowCellMode>SP</FlowCellMode>
     <FlowCellConsumableVersion>1</FlowCellConsumableVersion>
     <FlowCellRssi>2</FlowCellRssi>
-    <LibraryTubeSerialBarcode>NV0297539-LIB</LibraryTubeSerialBarcode>
+    <LibraryTubeSerialBarcode>NV0394639-LIB</LibraryTubeSerialBarcode>
     <LibraryTubeSupportedModes>Universal</LibraryTubeSupportedModes>
     <LibraryTubePartNumber>20005221</LibraryTubePartNumber>
-    <LibraryTubeLotNumber>1000008040</LibraryTubeLotNumber>
+    <LibraryTubeLotNumber>1000010192</LibraryTubeLotNumber>
     <LibraryTubeExpirationdate>12/31/2169 00:00:00</LibraryTubeExpirationdate>
-    <LibraryTubeStartDate>02/06/2021 12:40:00</LibraryTubeStartDate>
-    <LibraryTubeRssi>4</LibraryTubeRssi>
-    <SbsSerialBarcode>NV3040624-RGSBS</SbsSerialBarcode>
-    <SbsSupportedModes>S4</SbsSupportedModes>
-    <SbsPartNumber>20031051</SbsPartNumber>
-    <SbsLotNumber>20485602</SbsLotNumber>
-    <SbsExpirationdate>10/24/2021 00:00:00</SbsExpirationdate>
-    <SbsStartDate>02/06/2021 12:40:00</SbsStartDate>
-    <SbsCycleKit>338</SbsCycleKit>
-    <SbsNumberOfCyclesRemaining>16</SbsNumberOfCyclesRemaining>
-    <SbsNumberOfCyclesSupported>338</SbsNumberOfCyclesSupported>
+    <LibraryTubeStartDate>11/01/2021 11:50:00</LibraryTubeStartDate>
+    <LibraryTubeRssi>3</LibraryTubeRssi>
+    <SbsSerialBarcode>NV3512584-RGSBS</SbsSerialBarcode>
+    <SbsSupportedModes>S2;S1;SP</SbsSupportedModes>
+    <SbsPartNumber>20031052</SbsPartNumber>
+    <SbsLotNumber>20559158</SbsLotNumber>
+    <SbsExpirationdate>07/20/2022 00:00:00</SbsExpirationdate>
+    <SbsStartDate>11/01/2021 11:50:00</SbsStartDate>
+    <SbsCycleKit>138</SbsCycleKit>
+    <SbsNumberOfCyclesRemaining>20</SbsNumberOfCyclesRemaining>
+    <SbsNumberOfCyclesSupported>138</SbsNumberOfCyclesSupported>
     <SbsConsumableVersion>3</SbsConsumableVersion>
     <SbsRssi>4</SbsRssi>
-    <ClusterSerialBarcode>NV3048388-RGCPE</ClusterSerialBarcode>
-    <ClusterSupportedModes>S4</ClusterSupportedModes>
-    <ClusterPartNumber>20031056</ClusterPartNumber>
-    <ClusterLotNumber>20491402</ClusterLotNumber>
-    <ClusterExpirationdate>10/31/2021 00:00:00</ClusterExpirationdate>
-    <ClusterStartDate>02/06/2021 12:40:00</ClusterStartDate>
-    <ClusterCycleKit>338</ClusterCycleKit>
-    <ClusterNumberOfCyclesRemaining>16</ClusterNumberOfCyclesRemaining>
+    <ClusterSerialBarcode>NV3552837-RGCPE</ClusterSerialBarcode>
+    <ClusterSupportedModes>SP</ClusterSupportedModes>
+    <ClusterPartNumber>20031059</ClusterPartNumber>
+    <ClusterLotNumber>20566881</ClusterLotNumber>
+    <ClusterExpirationdate>08/06/2022 00:00:00</ClusterExpirationdate>
+    <ClusterStartDate>11/01/2021 11:50:00</ClusterStartDate>
+    <ClusterCycleKit>545</ClusterCycleKit>
+    <ClusterNumberOfCyclesRemaining>427</ClusterNumberOfCyclesRemaining>
     <ClusterRssi>5</ClusterRssi>
-    <BufferSerialBarcode>NV5091519-BUFFR</BufferSerialBarcode>
-    <BufferSupportedModes>S4</BufferSupportedModes>
-    <BufferPartNumber>20003187</BufferPartNumber>
-    <BufferLotNumber>50000132</BufferLotNumber>
-    <BufferExpirationdate>07/15/2021 00:00:00</BufferExpirationdate>
-    <BufferNumberOfCyclesRemaining>8</BufferNumberOfCyclesRemaining>
-    <BufferStartDate>02/06/2021 12:40:00</BufferStartDate>
+    <BufferSerialBarcode>NV5203688-BUFFR</BufferSerialBarcode>
+    <BufferSupportedModes>S2;S1;SP</BufferSupportedModes>
+    <BufferPartNumber>20013524</BufferPartNumber>
+    <BufferLotNumber>50000217</BufferLotNumber>
+    <BufferExpirationdate>04/16/2022 00:00:00</BufferExpirationdate>
+    <BufferNumberOfCyclesRemaining>212</BufferNumberOfCyclesRemaining>
+    <BufferStartDate>11/01/2021 11:50:00</BufferStartDate>
     <BufferRssi>3</BufferRssi>
   </RfidsInfo>
   <RecipeFilePath>C:\Program Files\Illumina\NovaSeq Control Software\Recipe</RecipeFilePath>
   <SamplesheetFile/>
   <UsedLimsSetup>false</UsedLimsSetup>
-  <CeLinuxRunFolder>/ilmn/outputfolder/210206_A00689_0226_AHMYJ7DSXY/</CeLinuxRunFolder>
+  <CeLinuxRunFolder>/ilmn/outputfolder/211101_A00187_0615_AHLG5GDRXY/</CeLinuxRunFolder>
   <RtaRawRunFolder>/ilmn/outputfolder</RtaRawRunFolder>
-  <CeMountRunFolder>Z:\outputfolder\210206_A00689_0226_AHMYJ7DSXY\</CeMountRunFolder>
-  <OutputRunFolder>\\172.16.1.6\clinicaldata\Runs\210206_A00689_0226_AHMYJ7DSXY\</OutputRunFolder>
+  <CeMountRunFolder>Z:\outputfolder\211101_A00187_0615_AHLG5GDRXY\</CeMountRunFolder>
+  <OutputRunFolder>\\172.16.1.6\clinicaldata\Runs\211101_A00187_0615_AHLG5GDRXY\</OutputRunFolder>
   <OutputRootFolder>\\172.16.1.6\clinicaldata\Runs</OutputRootFolder>
-  <SbcRunFolder>C:\ProgramData\Illumina\NovaSeq\NovaSeqTemp\210206_A00689_0226_AHMYJ7DSXY\</SbcRunFolder>
-  <PreRunFolder>C:\ProgramData\Illumina\NovaSeq\NovaSeqTemp\RunSetupLogs\A00689_2021-02-06__11_58_48_SideA</PreRunFolder>
-  <RunStartDate>210206</RunStartDate>
-  <RunId>210206_A00689_0226_AHMYJ7DSXY</RunId>
+  <SbcRunFolder>C:\ProgramData\Illumina\NovaSeq\NovaSeqTemp\211101_A00187_0615_AHLG5GDRXY\</SbcRunFolder>
+  <PreRunFolder>C:\ProgramData\Illumina\NovaSeq\NovaSeqTemp\RunSetupLogs\A00187_2021-11-01__11_35_59_SideA</PreRunFolder>
+  <RunStartDate>211101</RunStartDate>
+  <RunId>211101_A00187_0615_AHLG5GDRXY</RunId>
   <UseBaseSpace>true</UseBaseSpace>
   <UseBaseSpaceMonitoringAndStorage>false</UseBaseSpaceMonitoringAndStorage>
-  <BaseSpaceRunId>6300294</BaseSpaceRunId>
+  <BaseSpaceRunId>7618619</BaseSpaceRunId>
   <BaseSpaceEnvironment>euc1-prod</BaseSpaceEnvironment>
   <BaseSpaceDomain/>
   <Autocenter>true</Autocenter>
   <BiDirectionalScanning>true</BiDirectionalScanning>
   <UseCustomRecipe>false</UseCustomRecipe>
   <UseCustomRead1Primer>false</UseCustomRead1Primer>
   <UseCustomRead2Primer>false</UseCustomRead2Primer>
   <UseCustomIndexRead1Primer>false</UseCustomIndexRead1Primer>
   <IsRehyb>false</IsRehyb>
-  <InstrumentName>A00689</InstrumentName>
+  <InstrumentName>A00187</InstrumentName>
   <PlatformType>HighThroughput</PlatformType>
   <Application>NovaSeq Control Software</Application>
-  <ApplicationVersion>1.7.0</ApplicationVersion>
-  <Build>16</Build>
+  <ApplicationVersion>1.7.5</ApplicationVersion>
+  <Build>27</Build>
   <FirmwareVersions>
     <FirmwareVersion>
       <Board>Fluidics Board</Board>
       <Version>novaseq_flu@NovaSeq_1.26.1</Version>
     </FirmwareVersion>
     <FirmwareVersion>
       <Board>Left Buffer Interface Board</Board>
@@ -130,12 +130,12 @@
     </FirmwareVersion>
     <FirmwareVersion>
       <Board>Right Reagent Chiller Board</Board>
       <Version>novaseq_rca@NovaSeq_1.26.1</Version>
     </FirmwareVersion>
   </FirmwareVersions>
   <SendIlluminaHealthData>true</SendIlluminaHealthData>
-  <UcsRunId>17A89287DCD6C742</UcsRunId>
+  <UcsRunId>187B23D04A498564</UcsRunId>
   <UcsVersion>1.6.3.1575</UcsVersion>
   <RunSetupMode>Manual</RunSetupMode>
   <WorkflowType>NovaSeqStandard</WorkflowType>
 </RunParameters>
```

### Comparing `cg-33.1.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr` & `cg-33.1.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml` & `cg-33.1.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml` & `cg-33.1.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/RunInfo.xml` & `cg-33.1.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R1_001.fastq.gz` & `cg-33.1.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R1_001.fastq.gz`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R2_001.fastq.gz` & `cg-33.1.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R2_001.fastq.gz`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml` & `cg-33.1.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml` & `cg-33.1.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr` & `cg-33.1.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout` & `cg-33.1.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/fixtures/apps/demultiplexing/hiseq_run/runParameters.xml` & `cg-33.1.2/tests/fixtures/apps/demultiplexing/run_parameters/runParameters_missing_flowcell_run_field.xml`

 * *Files 5% similar despite different names*

#### Comparing `cg-33.1.1/tests/fixtures/apps/demultiplexing/hiseq_run/runParameters.xml` & `cg-33.1.2/tests/fixtures/apps/demultiplexing/run_parameters/runParameters_missing_flowcell_run_field.xml`

```diff
@@ -28,15 +28,14 @@
       <Lane>2</Lane>
     </AlignToPhiX>
     <ClusteringChoice>OnBoardClustering</ClusteringChoice>
     <RunMode>RapidRun</RunMode>
     <Rehyb>None</Rehyb>
     <PerformPreRunFluidicsCheck>false</PerformPreRunFluidicsCheck>
     <ServiceRun>false</ServiceRun>
-    <ApplicationName>HiSeq Control Software</ApplicationName>
     <ApplicationVersion>2.0.12.0</ApplicationVersion>
     <RunID>140303_D00410_0050_BH8ETTADXX</RunID>
     <RunStartDate>140303</RunStartDate>
     <BaseSpaceSettings>
       <UseBaseSpace>false</UseBaseSpace>
       <RunMonitoringOnly>false</RunMonitoringOnly>
       <Username/>
```

### Comparing `cg-33.1.1/tests/fixtures/apps/demultiplexing/raw_lims_samples/raw_samplesheet_novaseq.json` & `cg-33.1.2/tests/fixtures/apps/demultiplexing/raw_lims_samples/raw_samplesheet_novaseq.json`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/fixtures/apps/demultiplexing/runParameters_missing_flowcell_run_field.xml` & `cg-33.1.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/hiseq/180522_ST-E00198_0301_BHLCKNCCXY/runParameters.xml`

 * *Files 23% similar despite different names*

#### Comparing `cg-33.1.1/tests/fixtures/apps/demultiplexing/runParameters_missing_flowcell_run_field.xml` & `cg-33.1.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/hiseq/180522_ST-E00198_0301_BHLCKNCCXY/runParameters.xml`

```diff
@@ -1,137 +1,165 @@
 <?xml version="1.0" encoding="utf-8"?>
 <RunParameters xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
   <Setup>
-    <ExperimentName>EXOME</ExperimentName>
+    <LimsIntegrationMode>false</LimsIntegrationMode>
+    <NumberOfRehybAttemptsRemaining>2</NumberOfRehybAttemptsRemaining>
+    <ExperimentName>HLCKNCCXY</ExperimentName>
     <ScanID>-999</ScanID>
     <FCPosition>B</FCPosition>
     <WorkFlowType>SINGLEINDEX</WorkFlowType>
-    <PairEndFC>true</PairEndFC>
-    <Read1>101</Read1>
-    <IndexRead1>7</IndexRead1>
+    <Read1>151</Read1>
+    <IndexRead1>8</IndexRead1>
     <IndexRead2>0</IndexRead2>
-    <Read2>101</Read2>
+    <Read2>151</Read2>
     <OutputFolder>X:\Runs</OutputFolder>
-    <CompressBcls>true</CompressBcls>
-    <RemapQScores>default</RemapQScores>
-    <NearNeighborCorrection>false</NearNeighborCorrection>
-    <PeriodicSave>Save Tile Thumbnails</PeriodicSave>
-    <Flowcell>HiSeq Rapid Flow Cell v1</Flowcell>
-    <FirstBaseConfirmation>false</FirstBaseConfirmation>
-    <SampleSheet>Z:\2014\H8ETTADXX.csv</SampleSheet>
-    <ControlLane>0</ControlLane>
-    <KeepIntensityFiles>false</KeepIntensityFiles>
-    <Sbs>TruSeq Rapid SBS Kit</Sbs>
-    <Pe>TruSeq Rapid PE Cluster Kit</Pe>
-    <Index>TruSeq Rapid PE Cluster Kit</Index>
-    <AlignToPhiX>
-      <Lane>1</Lane>
-      <Lane>2</Lane>
-    </AlignToPhiX>
-    <ClusteringChoice>OnBoardClustering</ClusteringChoice>
-    <RunMode>RapidRun</RunMode>
+    <PeriodicSave>Save All Thumbnails</PeriodicSave>
+    <Flowcell>HiSeq X</Flowcell>
+    <FirstBaseConfirmation>true</FirstBaseConfirmation>
+    <SampleSheet/>
+    <Sbs>HiSeq X SBS</Sbs>
+    <Pe>HiSeq X PE</Pe>
+    <Index>HiSeq X Sequencing Primer</Index>
     <Rehyb>None</Rehyb>
     <PerformPreRunFluidicsCheck>false</PerformPreRunFluidicsCheck>
-    <ServiceRun>false</ServiceRun>
-    <ApplicationVersion>2.0.12.0</ApplicationVersion>
-    <RunID>140303_D00410_0050_BH8ETTADXX</RunID>
-    <RunStartDate>140303</RunStartDate>
+    <ApplicationName>HiSeq Control Software</ApplicationName>
+    <ApplicationVersion>HD 3.5.0.7</ApplicationVersion>
+    <RunID>180522_ST-E00198_0301_BHLCKNCCXY</RunID>
+    <RunStartDate>180522</RunStartDate>
+    <IntegrationMode>BaseSpace</IntegrationMode>
     <BaseSpaceSettings>
-      <UseBaseSpace>false</UseBaseSpace>
-      <RunMonitoringOnly>false</RunMonitoringOnly>
-      <Username/>
-      <RunId>5643644</RunId>
-      <TempFolder>E:\Illumina\BaseSpaceTemp</TempFolder>
+      <Username>clinical.genomics@scilifelab.se</Username>
+      <RunId>89045957</RunId>
+      <InstrumentHealthRunId>89045957</InstrumentHealthRunId>
+      <TempFolder>O:\Illumina\HiSeqTemp</TempFolder>
+      <UseBaseSpace>true</UseBaseSpace>
       <SendInstrumentHealthToILMN>true</SendInstrumentHealthToILMN>
+      <RunMonitoringOnly>true</RunMonitoringOnly>
     </BaseSpaceSettings>
-    <ScannerID>D00410</ScannerID>
-    <ScanNumber>50</ScanNumber>
-    <ComputerName>HWI-D00410</ComputerName>
-    <FPGAVersion>7.7.2.5</FPGAVersion>
+    <ScannerID>ST-E00198</ScannerID>
+    <ScanNumber>301</ScanNumber>
+    <ComputerName>HWI-E00198</ComputerName>
+    <FPGAVersion>10.37.13</FPGAVersion>
     <CPLDVersion>3.0.0</CPLDVersion>
-    <RTAVersion>1.17.21.3</RTAVersion>
-    <ChemistryVersion>Illumina,Bruno Fluidics Controller,0,v2.0340</ChemistryVersion>
-    <CameraFirmware>2.01-F20-R02</CameraFirmware>
-    <CameraDriver>6.45.20.3690</CameraDriver>
+    <RTAVersion>2.7.7</RTAVersion>
+    <BaseSpaceBrokerVersion>2.9.2.15</BaseSpaceBrokerVersion>
+    <ChemistryVersion>Illumina,Bruno Fluidics Controller,0,v2.0420</ChemistryVersion>
+    <CameraFirmware>2.21-C00-R03</CameraFirmware>
+    <CameraDriver>7.5.180.4395</CameraDriver>
+    <FtdiDriver>2.12.0.0</FtdiDriver>
     <FocusCameraFirmware/>
-    <Barcode>H8ETTADXX</Barcode>
+    <Barcode>HLCKNCCXY</Barcode>
+    <WashBarcode>HHHHHCCX2</WashBarcode>
     <Username>sbsuser</Username>
     <SelectedSections>
       <Section Name="A_1"/>
       <Section Name="B_1"/>
+      <Section Name="C_1"/>
+      <Section Name="D_1"/>
+      <Section Name="E_1"/>
+      <Section Name="F_1"/>
+      <Section Name="G_1"/>
+      <Section Name="H_1"/>
     </SelectedSections>
     <FocusMethod>DynamicITF</FocusMethod>
     <SelectedSurface>BothLaneSurfaces</SelectedSurface>
-    <SwathScanMode>DualSwathFC</SwathScanMode>
+    <DoDualSurfaceAutoCenter>true</DoDualSurfaceAutoCenter>
+    <SwathScanMode>AutoSwath</SwathScanMode>
     <EnableLft>true</EnableLft>
     <AutoTiltOnce>true</AutoTiltOnce>
     <EnableAutoCenter>true</EnableAutoCenter>
-    <EnableAnalysis>true</EnableAnalysis>
     <EnableBasecalling>true</EnableBasecalling>
     <EnableCameraLogging>false</EnableCameraLogging>
-    <AdapterPlate>HiSeq Adapter Plate</AdapterPlate>
-    <SlideHolder>HiSeq Flow Cell Holder</SlideHolder>
-    <TemplateCycleCount>4</TemplateCycleCount>
-    <NumAnalysisThreads>8</NumAnalysisThreads>
     <FPGADynamicFocusSettings>
       <MaxInitialZJumpHalfUm>3</MaxInitialZJumpHalfUm>
       <MaxSubsequentZJumpHalfUm>7</MaxSubsequentZJumpHalfUm>
       <NumberOfInitialZJumps>0</NumberOfInitialZJumps>
-      <CVGainStart>500</CVGainStart>
-      <CVGainPosLocked>500</CVGainPosLocked>
-      <Offset>250</Offset>
-      <HotPixel>350</HotPixel>
-      <MotorDelayFrames>10</MotorDelayFrames>
-      <SoftwareLaserLag>200</SoftwareLaserLag>
+      <CVGainStart>250</CVGainStart>
+      <CVGainPosLocked>250</CVGainPosLocked>
+      <Offset>0</Offset>
+      <HotPixel>200</HotPixel>
+      <MotorDelayFrames>21</MotorDelayFrames>
+      <SoftwareLaserLag>1</SoftwareLaserLag>
       <DitherSize>100</DitherSize>
       <GroupSize>50</GroupSize>
-      <DitherShift>0</DitherShift>
+      <DitherShift>20</DitherShift>
       <IntensityCeiling>65535</IntensityCeiling>
-      <IGain>100</IGain>
+      <IGain>50</IGain>
       <IHistory>4</IHistory>
     </FPGADynamicFocusSettings>
-    <TileWidth>2048</TileWidth>
-    <TileHeight>10000</TileHeight>
-    <ImageWidth>2048</ImageWidth>
-    <ImageHeight>160000</ImageHeight>
-    <AreaPerPixelmm2>1.40625E-07</AreaPerPixelmm2>
-    <LaneLength>60</LaneLength>
-    <NumTilesPerSwath>16</NumTilesPerSwath>
+    <TileWidth>3200</TileWidth>
+    <TileHeight>7241</TileHeight>
+    <ImageWidth>3200</ImageWidth>
+    <ImageHeight>174420</ImageHeight>
+    <LaneLength>60.175</LaneLength>
+    <NumTilesPerSwath>24</NumTilesPerSwath>
     <NumSwaths>2</NumSwaths>
     <UseExistingRecipe>false</UseExistingRecipe>
     <Reads>
-      <Read Number="1" NumCycles="101" IsIndexedRead="N"/>
-      <Read Number="2" NumCycles="7" IsIndexedRead="Y"/>
-      <Read Number="3" NumCycles="101" IsIndexedRead="N"/>
+      <Read Number="1" NumCycles="151" IsIndexedRead="N"/>
+      <Read Number="2" NumCycles="8" IsIndexedRead="Y"/>
+      <Read Number="3" NumCycles="151" IsIndexedRead="N"/>
     </Reads>
-    <EnableNotifications>false</EnableNotifications>
     <ReagentKits>
       <Sbs>
         <SbsReagentKit>
-          <ID>xxx</ID>
+          <ID/>
           <Prime>false</Prime>
-          <NumberCyclesRemaining>225</NumberCyclesRemaining>
+          <NumberCyclesRemaining>325</NumberCyclesRemaining>
           <IsNew50Cycle>false</IsNew50Cycle>
-          <IsNew200Cycle>true</IsNew200Cycle>
+          <IsNew150Cycle>false</IsNew150Cycle>
+          <IsNew300Cycle>true</IsNew300Cycle>
         </SbsReagentKit>
       </Sbs>
-      <Index>
+      <Pe>
         <ReagentKit>
-          <ID>xxx</ID>
+          <ID/>
         </ReagentKit>
-      </Index>
-      <Pe/>
-      <Rehyb/>
+      </Pe>
     </ReagentKits>
     <ReagentBottles>
-      <Sbs/>
+      <Sbs>
+        <SbsReagents>
+          <BarcodedBottle>
+            <Type>CMR</Type>
+            <Barcode/>
+          </BarcodedBottle>
+          <BarcodedBottle>
+            <Type>SRE</Type>
+            <Barcode/>
+          </BarcodedBottle>
+          <BarcodedBottle>
+            <Type>EDP</Type>
+            <Barcode/>
+          </BarcodedBottle>
+          <BarcodedBottle>
+            <Type>LFN</Type>
+            <Barcode/>
+          </BarcodedBottle>
+          <BarcodedBottle>
+            <Type>ICB</Type>
+            <Barcode/>
+          </BarcodedBottle>
+          <BarcodedBottle>
+            <Type>SB1</Type>
+            <Barcode/>
+          </BarcodedBottle>
+          <BarcodedBottle>
+            <Type>SB2</Type>
+            <Barcode/>
+          </BarcodedBottle>
+          <BarcodedBottle>
+            <Type>SB3</Type>
+            <Barcode/>
+          </BarcodedBottle>
+        </SbsReagents>
+      </Sbs>
     </ReagentBottles>
-    <Resume>false</Resume>
-    <ResumeCycle>0</ResumeCycle>
-    <SupportMultipleSurfacesInUI>true</SupportMultipleSurfacesInUI>
-    <TempFolder>E:\Illumina\HiSeqTemp\140303_D00410_0050_BH8ETTADXX</TempFolder>
-    <RecipeFragmentVersion>1.3.61.0</RecipeFragmentVersion>
+    <TempFolder>O:\Illumina\HiSeqTemp\180522_ST-E00198_0301_BHLCKNCCXY</TempFolder>
+    <RecipeFragmentVersion>HD 3.6.0.4</RecipeFragmentVersion>
     <PromptForPeReagents>false</PromptForPeReagents>
     <MockRun>false</MockRun>
+    <ScannedBarcode/>
+    <CopyImages>false</CopyImages>
   </Setup>
   <Version>1</Version>
 </RunParameters>
```

### Comparing `cg-33.1.1/tests/fixtures/apps/fluffy/SampleSheet.csv` & `cg-33.1.2/tests/fixtures/apps/fluffy/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/fixtures/apps/fluffy/deliverables.yaml` & `cg-33.1.2/tests/fixtures/apps/fluffy/deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/fixtures/apps/madeline/madeline.xml` & `cg-33.1.2/tests/fixtures/apps/madeline/madeline.xml`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/fixtures/apps/mip/case_metrics_deliverables.yaml` & `cg-33.1.2/tests/fixtures/apps/mip/case_metrics_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/fixtures/apps/mip/dna/store/case_config.yaml` & `cg-33.1.2/tests/fixtures/apps/mip/dna/store/case_config.yaml`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml` & `cg-33.1.2/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml` & `cg-33.1.2/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf` & `cg-33.1.2/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/fixtures/apps/mip/rna/case_config.yaml` & `cg-33.1.2/tests/fixtures/apps/mip/rna/case_config.yaml`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml` & `cg-33.1.2/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/fixtures/apps/mip/rna/store/bundle_data.yaml` & `cg-33.1.2/tests/fixtures/apps/mip/rna/store/bundle_data.yaml`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/fixtures/apps/mip/rna/store/case_config.yaml` & `cg-33.1.2/tests/fixtures/apps/mip/rna/store/case_config.yaml`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml` & `cg-33.1.2/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml` & `cg-33.1.2/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/fixtures/apps/scout/643594.config.yaml` & `cg-33.1.2/tests/fixtures/apps/scout/643594.config.yaml`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/fixtures/apps/scout/case_export.json` & `cg-33.1.2/tests/fixtures/apps/scout/case_export.json`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/fixtures/apps/scout/export_causatives.json` & `cg-33.1.2/tests/fixtures/apps/scout/export_causatives.json`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/fixtures/apps/scout/none_case_export.json` & `cg-33.1.2/tests/fixtures/apps/scout/none_case_export.json`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/fixtures/apps/scout/other_sex_case.json` & `cg-33.1.2/tests/fixtures/apps/scout/other_sex_case.json`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/fixtures/apps/scout/panel_export.bed` & `cg-33.1.2/tests/fixtures/apps/scout/panel_export.bed`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/fixtures/apps/scout/panel_export.csv` & `cg-33.1.2/tests/fixtures/apps/scout/panel_export.csv`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/fixtures/apps/sequencing_metrics_parser/Unaligned/Reports/Adapter_Metrics.csv` & `cg-33.1.2/tests/fixtures/apps/sequencing_metrics_parser/Unaligned/Reports/Adapter_Metrics.csv`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/fixtures/apps/sequencing_metrics_parser/Unaligned/Reports/Demultiplex_Stats.csv` & `cg-33.1.2/tests/fixtures/apps/sequencing_metrics_parser/Unaligned/Reports/Demultiplex_Stats.csv`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/fixtures/apps/sequencing_metrics_parser/Unaligned/Reports/Quality_Metrics.csv` & `cg-33.1.2/tests/fixtures/apps/sequencing_metrics_parser/Unaligned/Reports/Quality_Metrics.csv`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/fixtures/apps/sequencing_metrics_parser/Unaligned/Reports/RunInfo.xml` & `cg-33.1.2/tests/fixtures/apps/sequencing_metrics_parser/Unaligned/Reports/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/fixtures/cgweb_orders/balsamic.json` & `cg-33.1.2/tests/fixtures/cgweb_orders/balsamic.json`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/fixtures/cgweb_orders/fastq.json` & `cg-33.1.2/tests/fixtures/cgweb_orders/fastq.json`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/fixtures/cgweb_orders/metagenome.json` & `cg-33.1.2/tests/fixtures/cgweb_orders/metagenome.json`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/fixtures/cgweb_orders/microsalt.json` & `cg-33.1.2/tests/fixtures/cgweb_orders/microsalt.json`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/fixtures/cgweb_orders/mip.json` & `cg-33.1.2/tests/fixtures/cgweb_orders/mip.json`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/fixtures/cgweb_orders/mip_rna.json` & `cg-33.1.2/tests/fixtures/cgweb_orders/mip_rna.json`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/fixtures/cgweb_orders/rml.json` & `cg-33.1.2/tests/fixtures/cgweb_orders/rml.json`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/fixtures/cgweb_orders/sarscov2.json` & `cg-33.1.2/tests/fixtures/cgweb_orders/sarscov2.json`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/fixtures/data/SampleSheet.csv` & `cg-33.1.2/tests/fixtures/data/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/fixtures/data/cgfixture.db` & `cg-33.1.2/tests/fixtures/data/cgfixture.db`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/fixtures/data/hkstore.db` & `cg-33.1.2/tests/fixtures/data/hkstore.db`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/fixtures/io/example_json.json` & `cg-33.1.2/tests/fixtures/io/example_json.json`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/fixtures/orderforms/1508.27.balsamic.xlsx` & `cg-33.1.2/tests/fixtures/orderforms/1508.27.balsamic.xlsx`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/fixtures/orderforms/1508.27.balsamic_qc.xlsx` & `cg-33.1.2/tests/fixtures/orderforms/1508.27.balsamic_qc.xlsx`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/fixtures/orderforms/1508.27.balsamic_umi.xlsx` & `cg-33.1.2/tests/fixtures/orderforms/1508.27.balsamic_umi.xlsx`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/fixtures/orderforms/1508.27.fastq.xlsx` & `cg-33.1.2/tests/fixtures/orderforms/1508.27.fastq.xlsx`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/fixtures/orderforms/1508.27.mip.xlsx` & `cg-33.1.2/tests/fixtures/orderforms/1508.27.mip.xlsx`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/fixtures/orderforms/1508.27.mip_rna.xlsx` & `cg-33.1.2/tests/fixtures/orderforms/1508.27.mip_rna.xlsx`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/fixtures/orderforms/1603.11.microbial.xlsx` & `cg-33.1.2/tests/fixtures/orderforms/1603.11.microbial.xlsx`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/fixtures/orderforms/1604.15.rml.xlsx` & `cg-33.1.2/tests/fixtures/orderforms/1604.15.rml.xlsx`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/fixtures/orderforms/1605.10.metagenome.xlsx` & `cg-33.1.2/tests/fixtures/orderforms/1605.10.metagenome.xlsx`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/fixtures/orderforms/2184.7.sarscov2.xlsx` & `cg-33.1.2/tests/fixtures/orderforms/2184.7.sarscov2.xlsx`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/fixtures/orderforms/NIPT-json.json` & `cg-33.1.2/tests/fixtures/orderforms/NIPT-json.json`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json` & `cg-33.1.2/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/fixtures/orderforms/mip_uploaded_json_orderform.json` & `cg-33.1.2/tests/fixtures/orderforms/mip_uploaded_json_orderform.json`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/fixtures/report/case_data.json` & `cg-33.1.2/tests/fixtures/report/case_data.json`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/fixtures/report/lims_exported_samples.json` & `cg-33.1.2/tests/fixtures/report/lims_exported_samples.json`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/fixtures/report/lims_family.json` & `cg-33.1.2/tests/fixtures/report/lims_family.json`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/io/conftest.py` & `cg-33.1.2/tests/io/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/io/test_io_controller.py` & `cg-33.1.2/tests/io/test_io_controller.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/io/test_io_csv.py` & `cg-33.1.2/tests/io/test_io_csv.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/io/test_io_json.py` & `cg-33.1.2/tests/io/test_io_json.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/io/test_io_xml.py` & `cg-33.1.2/tests/io/test_io_xml.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/io/test_io_yaml.py` & `cg-33.1.2/tests/io/test_io_yaml.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/io/test_validate_path.py` & `cg-33.1.2/tests/io/test_validate_path.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/meta/archive/conftest.py` & `cg-33.1.2/tests/meta/archive/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/meta/archive/test_archiving.py` & `cg-33.1.2/tests/meta/archive/test_archiving.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/meta/backup/conftest.py` & `cg-33.1.2/tests/meta/backup/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/meta/backup/test_meta_backup.py` & `cg-33.1.2/tests/meta/backup/test_meta_backup.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/meta/backup/test_meta_pdc.py` & `cg-33.1.2/tests/meta/backup/test_meta_pdc.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/meta/clean/conftest.py` & `cg-33.1.2/tests/meta/clean/conftest.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,61 +1,61 @@
 from pathlib import Path
 
 import pytest
 
 from tests.cli.demultiplex.conftest import fixture_demultiplexed_flow_cells_working_directory
 
 
-@pytest.fixture(name="correct_flow_cell")
-def fixture_correct_flow_cell() -> str:
-    """Correct flow cell name"""
-    return "201203_A00689_0200_AHVKJCDRXX"
+@pytest.fixture(name="correct_flow_cell_name")
+def fixture_correct_flow_cell_name(bcl2fastq_flow_cell_full_name: str) -> str:
+    """Correct flow cell name."""
+    return bcl2fastq_flow_cell_full_name
 
 
 @pytest.fixture(name="incorrect_flow_cell_too_long")
-def fixture_incorrect_flow_cell_too_long() -> str:
-    """Incorrect flow cell name"""
-    return "201203_A00689_0200_AHVKJCDRXX_r"
+def fixture_incorrect_flow_cell_too_long(correct_flow_cell_name: str) -> str:
+    """Incorrect flow cell name."""
+    return correct_flow_cell_name + "_r"
 
 
 @pytest.fixture(name="incorrect_flow_cell_extension")
-def fixture_incorrect_flow_cell_extension() -> str:
-    """Incorrect flow cell name"""
-    return "201203_A00689_0200_AHVKJCDRXX.someextension"
+def fixture_incorrect_flow_cell_extension(correct_flow_cell_name: str) -> str:
+    """Incorrect flow cell name."""
+    return correct_flow_cell_name + ".someextension"
 
 
 @pytest.fixture(name="incorrect_flow_cell_name")
 def fixture_incorrect_flow_cell_name() -> str:
-    """Incorrect flow cell name"""
+    """Incorrect flow cell name."""
     return "201203_A00689_0200_AZZZZZZZZZ"
 
 
 @pytest.fixture(name="correct_flow_cell_path")
 def fixture_correct_flow_cell_path(
-    demultiplexed_flow_cells_working_directory, correct_flow_cell
+    demultiplexed_flow_cells_working_directory, correct_flow_cell_name
 ) -> Path:
-    """Full path to a correctly named flow cell directory in demultiplexed-runs"""
-    return Path(demultiplexed_flow_cells_working_directory, correct_flow_cell)
+    """Full path to a correctly named flow cell directory in demultiplexed-runs."""
+    return Path(demultiplexed_flow_cells_working_directory, correct_flow_cell_name)
 
 
 @pytest.fixture(name="incorrect_flow_cell_path_too_long")
 def fixture_incorrect_flow_cell_path_too_long(
     demultiplexed_flow_cells_working_directory, incorrect_flow_cell_too_long
 ) -> Path:
-    """Full path to an incorrectly named flow cell directory in demultiplexed-runs"""
+    """Full path to an incorrectly named flow cell directory in demultiplexed-runs."""
     return Path(demultiplexed_flow_cells_working_directory, incorrect_flow_cell_too_long)
 
 
 @pytest.fixture(name="incorrect_flow_cell_path_extension")
 def fixture_incorrect_flow_cell_path_extension(
     demultiplexed_flow_cells_working_directory, incorrect_flow_cell_extension
 ) -> Path:
-    """Full path to an incorrectly named flow cell directory in demultiplexed-runs"""
+    """Full path to an incorrectly named flow cell directory in demultiplexed-runs."""
     return Path(demultiplexed_flow_cells_working_directory, incorrect_flow_cell_extension)
 
 
-@pytest.fixture(name="nonexistent_flow_cell_path")
-def fixture_nonexistent_flow_cell_path(
+@pytest.fixture(name="non-existent_flow_cell_path")
+def fixture_non_existent_flow_cell_path(
     demultiplexed_flow_cells_working_directory, incorrect_flow_cell_name
 ) -> Path:
-    """Full path to an incorrectly named flow cell directory in demultiplexed-runs"""
+    """Full path to an incorrectly named flow cell directory in demultiplexed-runs."""
     return Path(demultiplexed_flow_cells_working_directory, incorrect_flow_cell_name)
```

### Comparing `cg-33.1.1/tests/meta/clean/test_clean_demultiplexed_runs.py` & `cg-33.1.2/tests/meta/clean/test_clean_demultiplexed_runs.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     assert flow_cell_obj.is_correctly_named == result
 
 
 @pytest.mark.parametrize(
     "bcl2fastq_flow_cell_dir, statusdb_return_value, result",
     [
         ("correct_flow_cell_path", Flowcell(), True),
-        ("nonexistent_flow_cell_path", None, False),
+        ("non-existent_flow_cell_path", None, False),
     ],
 )
 @mock.patch("cg.apps.tb.api.TrailblazerAPI")
 @mock.patch("cg.apps.housekeeper.hk.HousekeeperAPI")
 @mock.patch("cg.store.Store")
 def test_flow_cell_exists_in_statusdb_(
     mock_statusdb: Store,
```

### Comparing `cg-33.1.1/tests/meta/clean/test_clean_flow_cell_run_directories.py` & `cg-33.1.2/tests/meta/clean/test_clean_flow_cell_run_directories.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/meta/compress/conftest.py` & `cg-33.1.2/tests/meta/compress/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/meta/compress/test_clean_fastq.py` & `cg-33.1.2/tests/meta/compress/test_clean_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/meta/compress/test_compress_files.py` & `cg-33.1.2/tests/meta/compress/test_compress_files.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/meta/compress/test_compress_meta_fastq.py` & `cg-33.1.2/tests/meta/compress/test_compress_meta_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/meta/compress/test_decompress_spring_meta.py` & `cg-33.1.2/tests/meta/compress/test_decompress_spring_meta.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/meta/compress/test_meta_compress_update_hk.py` & `cg-33.1.2/tests/meta/compress/test_meta_compress_update_hk.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/meta/conftest.py` & `cg-33.1.2/tests/meta/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 from cg.meta.transfer import TransferFlowCell
 from cg.meta.workflow.mip_dna import MipDNAAnalysisAPI
 from cg.store import Store
 from cg.store.models import Customer, ApplicationVersion, Invoice, Sample
 from tests.mocks.hk_mock import MockHousekeeperAPI
 from tests.store_helpers import StoreHelpers
 from tests.mocks.limsmock import MockLimsAPI
-from cg.constants.sequencing import RecordType
 from cg.constants.invoice import CustomerNames
 from cg.meta.invoice import InvoiceAPI
 
 
 @pytest.fixture(scope="function", name="mip_hk_store")
 def fixture_mip_hk_store(
     helpers: StoreHelpers,
@@ -120,37 +119,33 @@
 
 @pytest.fixture(name="binary_path")
 def fixture_binary_path() -> str:
     """Return the string of a path to a (fake) binary."""
     return Path("usr", "bin", "binary").as_posix()
 
 
-@pytest.fixture(name="yet_another_flow_cell_id")
-def fixture_yet_another_flow_cell_id() -> str:
-    """Return flow cell id."""
-    return "HJKMYBCXX"
-
-
 @pytest.fixture(name="stats_sample_data")
 def fixture_stats_sample_data(
-    sample_id: str, bcl2fastq_flow_cell_id: str, yet_another_flow_cell_id: str
+    sample_id: str,
+    bcl2fastq_flow_cell_id: str,
+    dragen_flow_cell_id: str,
 ) -> dict:
     return {
         "samples": [
             {
                 "name": sample_id,
                 "index": "ACGTACAT",
                 "flowcell": bcl2fastq_flow_cell_id,
-                "type": Sequencers.HISEQX,
+                "type": Sequencers.NOVASEQ,
             },
             {
                 "name": "ADM1136A3",
                 "index": "ACGTACAT",
-                "flowcell": yet_another_flow_cell_id,
-                "type": Sequencers.HISEQX,
+                "flowcell": dragen_flow_cell_id,
+                "type": Sequencers.NOVASEQ,
             },
         ]
     }
 
 
 @pytest.fixture(name="store_stats")
 def fixture_store_stats() -> Generator[StatsAPI, None, None]:
@@ -283,15 +278,14 @@
 
 @pytest.fixture(name="get_invoice_api_pool_generic_customer")
 def fixture_invoice_api_pool_generic_customer(
     store: Store,
     lims_api: MockLimsAPI,
     helpers: StoreHelpers,
     invoice_id: int = 0,
-    record_type: str = RecordType.Pool,
     customer_id: str = CustomerNames.cust132,
 ) -> InvoiceAPI:
     """Return an InvoiceAPI with a pool."""
     pool = helpers.ensure_pool(store=store, customer_id=customer_id)
     invoice: Invoice = helpers.ensure_invoice(
         store,
         invoice_id=invoice_id,
```

### Comparing `cg-33.1.1/tests/meta/deliver/conftest.py` & `cg-33.1.2/tests/meta/deliver/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/meta/deliver/test_deliver_ticket.py` & `cg-33.1.2/tests/meta/deliver/test_deliver_ticket.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/meta/deliver/test_delivery_api.py` & `cg-33.1.2/tests/meta/deliver/test_delivery_api.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/meta/demultiplex/conftest.py` & `cg-33.1.2/tests/meta/demultiplex/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/meta/demultiplex/test_delete_demultiplex_api.py` & `cg-33.1.2/tests/meta/demultiplex/test_delete_demultiplex_api.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/meta/demultiplex/test_demux_post_processing.py` & `cg-33.1.2/tests/meta/demultiplex/test_demux_post_processing.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/meta/demultiplex/test_rename_files.py` & `cg-33.1.2/tests/meta/demultiplex/test_rename_files.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/meta/encryption/conftest.py` & `cg-33.1.2/tests/meta/encryption/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/meta/encryption/test_encryption.py` & `cg-33.1.2/tests/meta/encryption/test_encryption.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/meta/observations/conftest.py` & `cg-33.1.2/tests/meta/observations/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/meta/observations/test_meta_upload_observations.py` & `cg-33.1.2/tests/meta/observations/test_meta_upload_observations.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/meta/orders/conftest.py` & `cg-33.1.2/tests/meta/orders/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/meta/orders/test_PoolSubmitter_validate_order.py` & `cg-33.1.2/tests/meta/orders/test_PoolSubmitter_validate_order.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py` & `cg-33.1.2/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/meta/orders/test_SarsCov2Submitter_store_order.py` & `cg-33.1.2/tests/meta/orders/test_SarsCov2Submitter_store_order.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/meta/orders/test_SarsCov2Submitter_validate_order.py` & `cg-33.1.2/tests/meta/orders/test_SarsCov2Submitter_validate_order.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/meta/orders/test_meta_orders_api.py` & `cg-33.1.2/tests/meta/orders/test_meta_orders_api.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/meta/orders/test_meta_orders_lims.py` & `cg-33.1.2/tests/meta/orders/test_meta_orders_lims.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/meta/orders/test_meta_orders_status.py` & `cg-33.1.2/tests/meta/orders/test_meta_orders_status.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/meta/orders/test_ticket_handler.py` & `cg-33.1.2/tests/meta/orders/test_ticket_handler.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/meta/report/conftest.py` & `cg-33.1.2/tests/meta/report/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/meta/report/test_balsamic_api.py` & `cg-33.1.2/tests/meta/report/test_balsamic_api.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/meta/report/test_field_validators.py` & `cg-33.1.2/tests/meta/report/test_field_validators.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/meta/report/test_mip_dna_api.py` & `cg-33.1.2/tests/meta/report/test_mip_dna_api.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/meta/report/test_report_api.py` & `cg-33.1.2/tests/meta/report/test_report_api.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/meta/report/test_rnafusion_api.py` & `cg-33.1.2/tests/meta/report/test_rnafusion_api.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/meta/rsync/conftest.py` & `cg-33.1.2/tests/meta/rsync/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/meta/rsync/test_rsync.py` & `cg-33.1.2/tests/meta/rsync/test_rsync.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/meta/test_invoice.py` & `cg-33.1.2/tests/meta/test_invoice.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/meta/transfer/conftest.py` & `cg-33.1.2/tests/meta/transfer/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/meta/transfer/test_external_data.py` & `cg-33.1.2/tests/meta/transfer/test_external_data.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/meta/transfer/test_meta_transfer_flowcell.py` & `cg-33.1.2/tests/meta/transfer/test_meta_transfer_flowcell.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,40 +34,38 @@
     )
 
     # THEN tha tags should be added
     assert transfer_flow_cell_api.hk.get_tag(name=bcl2fastq_flow_cell_id) is not None
 
 
 def test_add_flow_cell_to_status_db(
-    transfer_flow_cell_api: Generator[TransferFlowCell, None, None], yet_another_flow_cell_id: str
+    transfer_flow_cell_api: Generator[TransferFlowCell, None, None], bcl2fastq_flow_cell_id: str
 ):
     """Test adding flow cell to Status db."""
     # GIVEN transfer flow cell API
 
     # GIVEN a flow cell that does not exist in status db
     flow_cell: Flowcell = transfer_flow_cell_api.db.get_flow_cell_by_name(
-        flow_cell_name=yet_another_flow_cell_id
+        flow_cell_name=bcl2fastq_flow_cell_id
     )
 
     assert flow_cell is None
 
     # GIVEN a cgstats flow cell
-    cgstats_flow_cell: StatsFlowcell = transfer_flow_cell_api.stats.flowcell(
-        yet_another_flow_cell_id
-    )
+    cgstats_flow_cell: StatsFlowcell = transfer_flow_cell_api.stats.flowcell(bcl2fastq_flow_cell_id)
 
     # WHEN adding flow cell to status db
     added_flow_cell: Flowcell = transfer_flow_cell_api._add_flow_cell_to_status_db(
         cgstats_flow_cell=cgstats_flow_cell,
         flow_cell=flow_cell,
-        flow_cell_id=yet_another_flow_cell_id,
+        flow_cell_id=bcl2fastq_flow_cell_id,
     )
 
     # THEN the flow cell added/returned should have the same id
-    assert added_flow_cell.name == yet_another_flow_cell_id
+    assert added_flow_cell.name == bcl2fastq_flow_cell_id
 
 
 def test_add_flow_cell_to_status_db_existing_flow_cell(
     flowcell_store: Store,
     bcl2fastq_flow_cell_id: str,
     helpers: StoreHelpers,
     transfer_flow_cell_api: Generator[TransferFlowCell, None, None],
@@ -353,88 +351,84 @@
     assert f"[NOT DONE]" in caplog.text
 
 
 def test_parse_flow_cell_samples(
     flowcell_store: Store,
     helpers: StoreHelpers,
     transfer_flow_cell_api: Generator[TransferFlowCell, None, None],
-    yet_another_flow_cell_id: str,
+    bcl2fastq_flow_cell_id: str,
 ):
     """Test parsing of flow cell samples."""
 
     # GIVEN a cgstats flow cell
-    cgstats_flow_cell: StatsFlowcell = transfer_flow_cell_api.stats.flowcell(
-        yet_another_flow_cell_id
-    )
+    cgstats_flow_cell: StatsFlowcell = transfer_flow_cell_api.stats.flowcell(bcl2fastq_flow_cell_id)
 
     # GIVEN a flow cell that exist in status db
     flow_cell: Flowcell = helpers.add_flowcell(
-        store=flowcell_store, flow_cell_name=yet_another_flow_cell_id
+        store=flowcell_store, flow_cell_name=bcl2fastq_flow_cell_id
     )
 
     # GIVEN no sample in flow cell
     assert len(flow_cell.samples) == 0
 
     # WHEN parsing the flow cell samples
     transfer_flow_cell_api._parse_flow_cell_samples(
         cgstats_flow_cell=cgstats_flow_cell,
         flow_cell=flow_cell,
-        flow_cell_id=yet_another_flow_cell_id,
+        flow_cell_id=bcl2fastq_flow_cell_id,
         store=True,
     )
 
     # THEN a sample should have been added
     assert len(flow_cell.samples) == 1
 
 
 def test_parse_flow_cell_samples_when_no_cgstats_sample(
     caplog,
     flowcell_store: Store,
     helpers: StoreHelpers,
     transfer_flow_cell_api: Generator[TransferFlowCell, None, None],
-    yet_another_flow_cell_id: str,
+    bcl2fastq_flow_cell_id: str,
 ):
     """Test parsing of flow cell samples when no cgstats sample."""
 
     # GIVEN a cgstats flow cell
-    cgstats_flow_cell: StatsFlowcell = transfer_flow_cell_api.stats.flowcell(
-        yet_another_flow_cell_id
-    )
+    cgstats_flow_cell: StatsFlowcell = transfer_flow_cell_api.stats.flowcell(bcl2fastq_flow_cell_id)
 
     # GIVEN a sample name that does not exist in cgstats
     cgstats_flow_cell.samples[0].name = "sample_does_not_exist_in_cgstats"
 
     # GIVEN a flow cell that exist in status db
     flow_cell: Flowcell = helpers.add_flowcell(
-        store=flowcell_store, flow_cell_name=yet_another_flow_cell_id
+        store=flowcell_store, flow_cell_name=bcl2fastq_flow_cell_id
     )
 
     # GIVEN no sample in flow cell
     assert len(flow_cell.samples) == 0
 
     # WHEN parsing the flow cell samples
     transfer_flow_cell_api._parse_flow_cell_samples(
         cgstats_flow_cell=cgstats_flow_cell,
         flow_cell=flow_cell,
-        flow_cell_id=yet_another_flow_cell_id,
+        flow_cell_id=bcl2fastq_flow_cell_id,
         store=True,
     )
 
     # THEN no sample should have been added
     assert len(flow_cell.samples) == 0
 
     # THEN we should llog that sample cannot be found
     assert f"Unable to find sample: {cgstats_flow_cell.samples[0].name}" in caplog.text
 
 
 def test_transfer(
     bcl2fastq_demux_results: DemuxResults,
     flowcell_store: Store,
     transfer_flow_cell_api: Generator[TransferFlowCell, None, None],
-    yet_another_flow_cell_id: str,
+    bcl2fastq_flow_cell_id: str,
 ):
     """Test transfer of sequencing files."""
 
     # GIVEN a store with a received but not sequenced sample
     housekeeper_api: HousekeeperAPI = transfer_flow_cell_api.hk
     assert len(flowcell_store._get_query(table=Sample).all()) == 2
     assert flowcell_store._get_query(table=Flowcell).count() == 0
@@ -443,22 +437,22 @@
     # GIVEN a sample sheet
 
     # WHEN transferring the flowcell containing the sample
     with warnings.catch_warnings():
         warnings.simplefilter("ignore", category=sa_exc.SAWarning)
         flow_cell = transfer_flow_cell_api.transfer(
             flow_cell_dir=bcl2fastq_demux_results.flow_cell.path,
-            flow_cell_id=yet_another_flow_cell_id,
+            flow_cell_id=bcl2fastq_flow_cell_id,
         )
 
     # THEN it should create a new flow cell record
     assert flowcell_store._get_query(table=Flowcell).count() == 1
     assert flow_cell.status == FlowCellStatus.ON_DISK
     assert isinstance(flow_cell.id, int)
-    assert flow_cell.name == yet_another_flow_cell_id
+    assert flow_cell.name == bcl2fastq_flow_cell_id
     status_sample = flowcell_store._get_query(table=Sample).first()
     assert isinstance(status_sample.sequenced_at, datetime)
 
     # ... and it should store the fastq files and samplesheet for the sample in housekeeper
     hk_bundle = housekeeper_api.bundle(name=status_sample.internal_id)
 
     assert len(hk_bundle.versions[0].files) > 0
```

### Comparing `cg-33.1.1/tests/meta/transfer/test_meta_transfer_lims.py` & `cg-33.1.2/tests/meta/transfer/test_meta_transfer_lims.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/meta/upload/balsamic/test_balsamic.py` & `cg-33.1.2/tests/meta/upload/balsamic/test_balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/meta/upload/conftest.py` & `cg-33.1.2/tests/meta/upload/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/meta/upload/gisaid/fixtures/four_samples.csv` & `cg-33.1.2/tests/meta/upload/gisaid/fixtures/four_samples.csv`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/meta/upload/mutacc/conftest.py` & `cg-33.1.2/tests/meta/upload/mutacc/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/meta/upload/mutacc/test_meta_upload_mutacc.py` & `cg-33.1.2/tests/meta/upload/mutacc/test_meta_upload_mutacc.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/meta/upload/nipt/conftest.py` & `cg-33.1.2/tests/meta/upload/nipt/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/meta/upload/nipt/test_nipt_upload_api.py` & `cg-33.1.2/tests/meta/upload/nipt/test_nipt_upload_api.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/meta/upload/scout/conftest.py` & `cg-33.1.2/tests/meta/upload/scout/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/meta/upload/scout/test_generate_load_config.py` & `cg-33.1.2/tests/meta/upload/scout/test_generate_load_config.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/meta/upload/scout/test_meta_upload_scoutapi.py` & `cg-33.1.2/tests/meta/upload/scout/test_meta_upload_scoutapi.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py` & `cg-33.1.2/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/meta/upload/scout/test_scout_config_builder.py` & `cg-33.1.2/tests/meta/upload/scout/test_scout_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/meta/upload/test_meta_upload_coverage.py` & `cg-33.1.2/tests/meta/upload/test_meta_upload_coverage.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/meta/upload/test_upload_api.py` & `cg-33.1.2/tests/meta/upload/test_upload_api.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/meta/upload/test_upload_genotypes_api.py` & `cg-33.1.2/tests/meta/upload/test_upload_genotypes_api.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/meta/upload/vogue/conftest.py` & `cg-33.1.2/tests/meta/upload/vogue/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/meta/upload/vogue/test_upload_vogue.py` & `cg-33.1.2/tests/meta/upload/vogue/test_upload_vogue.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/meta/workflow/conftest.py` & `cg-33.1.2/tests/meta/workflow/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/meta/workflow/test_analysis.py` & `cg-33.1.2/tests/meta/workflow/test_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/meta/workflow/test_balsamic.py` & `cg-33.1.2/tests/meta/workflow/test_balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/meta/workflow/test_microsalt.py` & `cg-33.1.2/tests/meta/workflow/test_microsalt.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/meta/workflow/test_prepare_fastq_api.py` & `cg-33.1.2/tests/meta/workflow/test_prepare_fastq_api.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/meta/workflow/test_rnafusion.py` & `cg-33.1.2/tests/meta/workflow/test_rnafusion.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/mocks/balsamic_analysis_mock.py` & `cg-33.1.2/tests/mocks/balsamic_analysis_mock.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/mocks/crunchy.py` & `cg-33.1.2/tests/mocks/crunchy.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/mocks/hk_mock.py` & `cg-33.1.2/tests/mocks/hk_mock.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/mocks/limsmock.py` & `cg-33.1.2/tests/mocks/limsmock.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/mocks/madeline.py` & `cg-33.1.2/tests/mocks/madeline.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/mocks/mip_analysis_mock.py` & `cg-33.1.2/tests/mocks/mip_analysis_mock.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/mocks/osticket.py` & `cg-33.1.2/tests/mocks/osticket.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/mocks/process_mock.py` & `cg-33.1.2/tests/mocks/process_mock.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/mocks/report.py` & `cg-33.1.2/tests/mocks/report.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/mocks/scout.py` & `cg-33.1.2/tests/mocks/scout.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/mocks/store_model.py` & `cg-33.1.2/tests/mocks/store_model.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/mocks/tb_mock.py` & `cg-33.1.2/tests/mocks/tb_mock.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/models/balsamic/conftest.py` & `cg-33.1.2/tests/models/balsamic/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/models/balsamic/test_balsamic_analysis.py` & `cg-33.1.2/tests/models/balsamic/test_balsamic_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/models/conftest.py` & `cg-33.1.2/tests/models/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/models/demultiplexing/conftest.py` & `cg-33.1.2/tests/models/demultiplexing/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/models/demultiplexing/test_demux_results.py` & `cg-33.1.2/tests/models/demultiplexing/test_demux_results.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/models/demultiplexing/test_flowcell_model.py` & `cg-33.1.2/tests/models/demultiplexing/test_flowcell_model.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/models/demultiplexing/test_run_parameters.py` & `cg-33.1.2/tests/models/demultiplexing/test_run_parameters.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/models/mip/conftest.py` & `cg-33.1.2/tests/models/mip/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/models/mip/test_mip_analysis.py` & `cg-33.1.2/tests/models/mip/test_mip_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/models/mip/test_mip_config.py` & `cg-33.1.2/tests/models/mip/test_mip_config.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/models/mip/test_mip_metrics_deliverables.py` & `cg-33.1.2/tests/models/mip/test_mip_metrics_deliverables.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/models/mip/test_mip_sample_info.py` & `cg-33.1.2/tests/models/mip/test_mip_sample_info.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/models/nextflow/conftest.py` & `cg-33.1.2/tests/models/nextflow/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/models/nextflow/test_nextflow_deliver.py` & `cg-33.1.2/tests/models/nextflow/test_nextflow_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/models/observations/conftest.py` & `cg-33.1.2/tests/models/observations/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/models/observations/test_observations_input_files.py` & `cg-33.1.2/tests/models/observations/test_observations_input_files.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/models/report/test_validators.py` & `cg-33.1.2/tests/models/report/test_validators.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/models/rnafusion/conftest.py` & `cg-33.1.2/tests/models/rnafusion/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/models/rnafusion/test_rnafusion_sample.py` & `cg-33.1.2/tests/models/rnafusion/test_rnafusion_sample.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/models/test_cg_models.py` & `cg-33.1.2/tests/models/test_cg_models.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/models/test_compression_data.py` & `cg-33.1.2/tests/models/test_compression_data.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/models/test_file_data.py` & `cg-33.1.2/tests/models/test_file_data.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/models/test_flowcell_class.py` & `cg-33.1.2/tests/models/test_flowcell_class.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/server/conftest.py` & `cg-33.1.2/tests/server/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/store/api/add/test_store_add_application_version.py` & `cg-33.1.2/tests/store/api/add/test_store_add_application_version.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/store/api/add/test_store_add_base.py` & `cg-33.1.2/tests/store/api/add/test_store_add_base.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/store/api/add/test_store_add_customer.py` & `cg-33.1.2/tests/store/api/add/test_store_add_customer.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/store/api/add/test_store_add_flow_celll.py` & `cg-33.1.2/tests/store/api/add/test_store_add_flow_celll.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/store/api/conftest.py` & `cg-33.1.2/tests/store/api/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,15 @@
 
     yield store
 
 
 @pytest.fixture(name="re_sequenced_sample_store")
 def fixture_re_sequenced_sample_store(
     store: Store,
-    another_flow_cell_id: str,
+    dragen_flow_cell_id: str,
     case_id: str,
     family_name: str,
     bcl2fastq_flow_cell_id: str,
     sample_id: str,
     ticket_id: str,
     timestamp_now: dt.datetime,
     helpers,
@@ -137,15 +137,15 @@
         sequenced_at=timestamp_now,
     )
 
     one_day_ahead_of_now = timestamp_now + dt.timedelta(days=1)
 
     helpers.add_flowcell(
         store=re_sequenced_sample_store,
-        flow_cell_name=another_flow_cell_id,
+        flow_cell_name=dragen_flow_cell_id,
         samples=[store_sample],
         date=timestamp_now,
     )
 
     helpers.add_flowcell(
         store=re_sequenced_sample_store,
         flow_cell_name=bcl2fastq_flow_cell_id,
```

### Comparing `cg-33.1.1/tests/store/api/delete/test_store_api_delete.py` & `cg-33.1.2/tests/store/api/delete/test_store_api_delete.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/store/api/find/test_find_basic_data.py` & `cg-33.1.2/tests/store/api/find/test_find_basic_data.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/store/api/find/test_find_basic_data_application_version.py` & `cg-33.1.2/tests/store/api/find/test_find_basic_data_application_version.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/store/api/find/test_find_business_data.py` & `cg-33.1.2/tests/store/api/find/test_find_business_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,59 +81,57 @@
     # THEN the returned flow cell should have the same name as the one in the database
     assert flow_cell.name == bcl2fastq_flow_cell_id
 
 
 def test_get_flow_cells_by_case(
     base_store: Store,
     bcl2fastq_flow_cell_id: str,
-    another_flow_cell_id: str,
+    dragen_flow_cell_id: str,
     case: Family,
     helpers: StoreHelpers,
     sample: Sample,
 ):
     """Test returning the latest flow cell from the database by case."""
 
     # GIVEN a store with two flow cell
     helpers.add_flowcell(store=base_store, flow_cell_name=bcl2fastq_flow_cell_id, samples=[sample])
 
-    helpers.add_flowcell(store=base_store, flow_cell_name=another_flow_cell_id)
+    helpers.add_flowcell(store=base_store, flow_cell_name=dragen_flow_cell_id)
 
     # WHEN fetching the latest flow cell
     flow_cells: List[Flowcell] = base_store.get_flow_cells_by_case(case=case)
 
     # THEN the flow cell samples for the case should be returned
     for flow_cell in flow_cells:
         for sample in flow_cell.samples:
             assert sample in case.samples
 
     # THEN the returned flow cell should have the same name as the one in the database
     assert flow_cells[0].name == bcl2fastq_flow_cell_id
 
 
-def test_get_flow_cells_by_statuses(another_flow_cell_id: str, re_sequenced_sample_store: Store):
+def test_get_flow_cells_by_statuses(dragen_flow_cell_id: str, re_sequenced_sample_store: Store):
     """Test returning the latest flow cell from the database by statuses."""
 
     # GIVEN a store with two flow cells
 
     # WHEN fetching the latest flow cell
     flow_cells: List[Flowcell] = re_sequenced_sample_store.get_flow_cells_by_statuses(
         flow_cell_statuses=[FlowCellStatus.ON_DISK, FlowCellStatus.REQUESTED]
     )
 
     # THEN the flow cell status should be "ondisk"
     for flow_cell in flow_cells:
         assert flow_cell.status == FlowCellStatus.ON_DISK
 
     # THEN the returned flow cell should have the same name as the one in the database
-    assert flow_cells[0].name == another_flow_cell_id
+    assert flow_cells[0].name == dragen_flow_cell_id
 
 
-def test_get_flow_cells_by_statuses_when_multiple_matches(
-    another_flow_cell_id: str, re_sequenced_sample_store: Store
-):
+def test_get_flow_cells_by_statuses_when_multiple_matches(re_sequenced_sample_store: Store):
     """Test returning the latest flow cell from the database by statuses when multiple matches."""
 
     # GIVEN a store with two flow cells
 
     # GIVEN a flow cell that exist in status db with status "requested"
     flow_cells: List[Flowcell] = re_sequenced_sample_store._get_query(table=Flowcell)
     flow_cells[0].status = FlowCellStatus.REQUESTED
@@ -241,15 +239,15 @@
     assert "No flow cells found" in caplog.text
 
 
 def test_is_all_flow_cells_on_disk_when_not_on_disk(
     base_store: Store,
     caplog,
     bcl2fastq_flow_cell_id: str,
-    another_flow_cell_id: str,
+    dragen_flow_cell_id: str,
     case_id: str,
     helpers: StoreHelpers,
     sample: Sample,
 ):
     """Test check if all flow cells for samples on a case is on disk when not on disk."""
     caplog.set_level(logging.DEBUG)
     # GIVEN a store with two flow cell
@@ -258,15 +256,15 @@
         flow_cell_name=bcl2fastq_flow_cell_id,
         samples=[sample],
         status=FlowCellStatus.PROCESSING,
     )
 
     another_flow_cell = helpers.add_flowcell(
         store=base_store,
-        flow_cell_name=another_flow_cell_id,
+        flow_cell_name=dragen_flow_cell_id,
         samples=[sample],
         status=FlowCellStatus.RETRIEVED,
     )
 
     # WHEN fetching the latest flow cell
     is_on_disk = base_store.is_all_flow_cells_on_disk(case_id=case_id)
 
@@ -278,15 +276,15 @@
     assert f"{another_flow_cell.name}: {another_flow_cell.status}" in caplog.text
 
 
 def test_is_all_flow_cells_on_disk_when_requested(
     base_store: Store,
     caplog,
     bcl2fastq_flow_cell_id: str,
-    another_flow_cell_id: str,
+    dragen_flow_cell_id: str,
     case_id: str,
     helpers: StoreHelpers,
     sample: Sample,
 ):
     """Test check if all flow cells for samples on a case is on disk when requested."""
     caplog.set_level(logging.DEBUG)
     # GIVEN a store with two flow cell
@@ -295,15 +293,15 @@
         flow_cell_name=bcl2fastq_flow_cell_id,
         samples=[sample],
         status=FlowCellStatus.REMOVED,
     )
 
     another_flow_cell = helpers.add_flowcell(
         store=base_store,
-        flow_cell_name=another_flow_cell_id,
+        flow_cell_name=dragen_flow_cell_id,
         samples=[sample],
         status=FlowCellStatus.REQUESTED,
     )
 
     # WHEN fetching the latest flow cell
     is_on_disk = base_store.is_all_flow_cells_on_disk(case_id=case_id)
 
@@ -317,27 +315,27 @@
     assert f"{another_flow_cell.name}: {another_flow_cell.status}" in caplog.text
 
 
 def test_is_all_flow_cells_on_disk(
     base_store: Store,
     caplog,
     bcl2fastq_flow_cell_id: str,
-    another_flow_cell_id: str,
+    dragen_flow_cell_id: str,
     case_id: str,
     helpers: StoreHelpers,
     sample: Sample,
 ):
     """Test check if all flow cells for samples on a case is on disk."""
     caplog.set_level(logging.DEBUG)
     # GIVEN a store with two flow cell
     flow_cell = helpers.add_flowcell(
         store=base_store, flow_cell_name=bcl2fastq_flow_cell_id, samples=[sample]
     )
 
-    helpers.add_flowcell(store=base_store, flow_cell_name=another_flow_cell_id)
+    helpers.add_flowcell(store=base_store, flow_cell_name=dragen_flow_cell_id)
 
     # WHEN fetching the latest flow cell
     is_on_disk = base_store.is_all_flow_cells_on_disk(case_id=case_id)
 
     # THEN return true
     assert is_on_disk is True
```

### Comparing `cg-33.1.1/tests/store/api/find/test_find_business_data_analysis.py` & `cg-33.1.2/tests/store/api/find/test_find_business_data_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/store/api/find/test_find_business_data_case.py` & `cg-33.1.2/tests/store/api/find/test_find_business_data_case.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/store/api/find/test_find_business_data_sample.py` & `cg-33.1.2/tests/store/api/find/test_find_business_data_sample.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/store/api/status/test_analyses_to_clean.py` & `cg-33.1.2/tests/store/api/status/test_analyses_to_clean.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/store/api/status/test_analyses_to_delivery_report.py` & `cg-33.1.2/tests/store/api/status/test_analyses_to_delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/store/api/status/test_store_api_status.py` & `cg-33.1.2/tests/store/api/status/test_store_api_status.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/store/api/status/test_store_api_status_analysis.py` & `cg-33.1.2/tests/store/api/status/test_store_api_status_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/store/api/status/test_store_api_status_cases.py` & `cg-33.1.2/tests/store/api/status/test_store_api_status_cases.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/store/api/status/test_store_api_status_customer.py` & `cg-33.1.2/tests/store/api/status/test_store_api_status_customer.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/store/api/status/test_store_api_status_pool.py` & `cg-33.1.2/tests/store/api/status/test_store_api_status_pool.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/store/api/status/test_store_api_status_sample.py` & `cg-33.1.2/tests/store/api/status/test_store_api_status_sample.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/store/api/test_base.py` & `cg-33.1.2/tests/store/api/test_base.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/store/conftest.py` & `cg-33.1.2/tests/store/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/store/filters/test_status_analyses_filters.py` & `cg-33.1.2/tests/store/filters/test_status_analyses_filters.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/store/filters/test_status_application_filters.py` & `cg-33.1.2/tests/store/filters/test_status_application_filters.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/store/filters/test_status_application_version_filters.py` & `cg-33.1.2/tests/store/filters/test_status_application_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/store/filters/test_status_bed_filters.py` & `cg-33.1.2/tests/store/filters/test_status_bed_filters.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/store/filters/test_status_bed_version_filters.py` & `cg-33.1.2/tests/store/filters/test_status_bed_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/store/filters/test_status_case_sample_filters.py` & `cg-33.1.2/tests/store/filters/test_status_case_sample_filters.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/store/filters/test_status_cases_filters.py` & `cg-33.1.2/tests/store/filters/test_status_cases_filters.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/store/filters/test_status_collaboration_filters.py` & `cg-33.1.2/tests/store/filters/test_status_collaboration_filters.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/store/filters/test_status_customer_filters.py` & `cg-33.1.2/tests/store/filters/test_status_customer_filters.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/store/filters/test_status_flow_cell_filters.py` & `cg-33.1.2/tests/store/filters/test_status_flow_cell_filters.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/store/filters/test_status_invoice_filters.py` & `cg-33.1.2/tests/store/filters/test_status_invoice_filters.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/store/filters/test_status_organism_filters.py` & `cg-33.1.2/tests/store/filters/test_status_organism_filters.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/store/filters/test_status_panel_filters.py` & `cg-33.1.2/tests/store/filters/test_status_panel_filters.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/store/filters/test_status_pool_filters.py` & `cg-33.1.2/tests/store/filters/test_status_pool_filters.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/store/filters/test_status_samples_filters.py` & `cg-33.1.2/tests/store/filters/test_status_samples_filters.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/store/filters/test_status_user_filters.py` & `cg-33.1.2/tests/store/filters/test_status_user_filters.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/store/test_delivery.py` & `cg-33.1.2/tests/store/test_delivery.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/store/test_store_models.py` & `cg-33.1.2/tests/store/test_store_models.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/store_helpers.py` & `cg-33.1.2/tests/store_helpers.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/test_store_helpers.py` & `cg-33.1.2/tests/test_store_helpers.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/utils/conftest.py` & `cg-33.1.2/tests/utils/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/utils/test_commands.py` & `cg-33.1.2/tests/utils/test_commands.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/utils/test_date.py` & `cg-33.1.2/tests/utils/test_date.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/utils/test_dict.py` & `cg-33.1.2/tests/utils/test_dict.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/utils/test_dispatcher.py` & `cg-33.1.2/tests/utils/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `cg-33.1.1/tests/utils/test_utils.py` & `cg-33.1.2/tests/utils/test_utils.py`

 * *Files identical despite different names*

