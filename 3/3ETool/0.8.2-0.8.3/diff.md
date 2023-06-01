# Comparing `tmp/3ETool-0.8.2.tar.gz` & `tmp/3ETool-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "3ETool-0.8.2.tar", last modified: Mon Mar  6 08:26:15 2023, max compression
+gzip compressed data, was "3ETool-0.8.3.tar", last modified: Thu Jun  1 09:43:24 2023, max compression
```

## Comparing `3ETool-0.8.2.tar` & `3ETool-0.8.3.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxrwxrwx   0        0        0        0 2023-03-06 08:26:15.134237 3ETool-0.8.2/
-drwxrwxrwx   0        0        0        0 2023-03-06 08:26:14.853905 3ETool-0.8.2/3ETool.egg-info/
--rw-rw-rw-   0        0        0     5747 2023-03-06 08:26:13.000000 3ETool-0.8.2/3ETool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2784 2023-03-06 08:26:14.000000 3ETool-0.8.2/3ETool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-06 08:26:13.000000 3ETool-0.8.2/3ETool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      163 2023-03-06 08:26:13.000000 3ETool-0.8.2/3ETool.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-03-06 08:26:14.000000 3ETool-0.8.2/3ETool.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-06 08:26:14.864999 3ETool-0.8.2/EEETools/
-drwxrwxrwx   0        0        0        0 2023-03-06 08:26:14.939216 3ETool-0.8.2/EEETools/BlockSubClasses/
--rw-rw-rw-   0        0        0      438 2022-04-08 08:08:33.000000 3ETool-0.8.2/EEETools/BlockSubClasses/__init__.py
--rw-rw-rw-   0        0        0     6290 2022-04-08 08:08:33.000000 3ETool-0.8.2/EEETools/BlockSubClasses/alternator.py
--rw-rw-rw-   0        0        0     6198 2022-04-08 08:08:33.000000 3ETool-0.8.2/EEETools/BlockSubClasses/boiler.py
--rw-rw-rw-   0        0        0     6277 2022-04-08 08:08:33.000000 3ETool-0.8.2/EEETools/BlockSubClasses/combustion_chamber.py
--rw-rw-rw-   0        0        0     5580 2022-04-08 08:08:33.000000 3ETool-0.8.2/EEETools/BlockSubClasses/compressor.py
--rw-rw-rw-   0        0        0     6598 2022-04-08 08:08:33.000000 3ETool-0.8.2/EEETools/BlockSubClasses/condenser.py
--rw-rw-rw-   0        0        0     5662 2022-04-08 08:08:33.000000 3ETool-0.8.2/EEETools/BlockSubClasses/cooler.py
--rw-rw-rw-   0        0        0     6626 2022-04-08 08:08:33.000000 3ETool-0.8.2/EEETools/BlockSubClasses/ejector_simplified.py
--rw-rw-rw-   0        0        0     8566 2022-04-08 08:08:33.000000 3ETool-0.8.2/EEETools/BlockSubClasses/evaporator.py
--rw-rw-rw-   0        0        0     5558 2022-04-08 08:08:33.000000 3ETool-0.8.2/EEETools/BlockSubClasses/expander.py
--rw-rw-rw-   0        0        0     3969 2022-04-08 08:08:33.000000 3ETool-0.8.2/EEETools/BlockSubClasses/generic.py
--rw-rw-rw-   0        0        0    10161 2022-04-08 08:08:33.000000 3ETool-0.8.2/EEETools/BlockSubClasses/heat_exchanger.py
--rw-rw-rw-   0        0        0     3991 2022-04-08 08:08:33.000000 3ETool-0.8.2/EEETools/BlockSubClasses/mixer.py
--rw-rw-rw-   0        0        0     5494 2022-04-08 08:08:33.000000 3ETool-0.8.2/EEETools/BlockSubClasses/pump.py
--rw-rw-rw-   0        0        0     3998 2022-04-08 08:08:33.000000 3ETool-0.8.2/EEETools/BlockSubClasses/separator.py
--rw-rw-rw-   0        0        0     5561 2022-04-08 08:08:33.000000 3ETool-0.8.2/EEETools/BlockSubClasses/valve.py
-drwxrwxrwx   0        0        0        0 2023-03-06 08:26:14.959917 3ETool-0.8.2/EEETools/MainModules/
--rw-rw-rw-   0        0        0       60 2022-04-08 08:08:33.000000 3ETool-0.8.2/EEETools/MainModules/__init__.py
--rw-rw-rw-   0        0        0    61613 2023-03-03 11:18:05.000000 3ETool-0.8.2/EEETools/MainModules/main_module.py
--rw-rw-rw-   0        0        0     6853 2023-02-16 17:45:23.000000 3ETool-0.8.2/EEETools/MainModules/pf_diagram_generation_module.py
--rw-rw-rw-   0        0        0    16475 2022-04-08 08:08:33.000000 3ETool-0.8.2/EEETools/MainModules/support_blocks.py
-drwxrwxrwx   0        0        0        0 2023-03-06 08:26:14.964918 3ETool-0.8.2/EEETools/Tools/
-drwxrwxrwx   0        0        0        0 2023-03-06 08:26:14.970035 3ETool-0.8.2/EEETools/Tools/API/
-drwxrwxrwx   0        0        0        0 2023-03-06 08:26:14.976053 3ETool-0.8.2/EEETools/Tools/API/DatAPI/
--rw-rw-rw-   0        0        0        0 2022-04-08 08:08:33.000000 3ETool-0.8.2/EEETools/Tools/API/DatAPI/__init__.py
--rw-rw-rw-   0        0        0     1369 2022-04-08 08:08:33.000000 3ETool-0.8.2/EEETools/Tools/API/DatAPI/modules_importer.py
-drwxrwxrwx   0        0        0        0 2023-03-06 08:26:14.981049 3ETool-0.8.2/EEETools/Tools/API/ExcelAPI/
--rw-rw-rw-   0        0        0        0 2022-04-08 08:08:33.000000 3ETool-0.8.2/EEETools/Tools/API/ExcelAPI/__init__.py
--rw-rw-rw-   0        0        0     7057 2023-03-03 10:59:27.000000 3ETool-0.8.2/EEETools/Tools/API/ExcelAPI/modules_importer.py
-drwxrwxrwx   0        0        0        0 2023-03-06 08:26:14.995060 3ETool-0.8.2/EEETools/Tools/API/Tools/
--rw-rw-rw-   0        0        0        0 2022-04-08 08:08:33.000000 3ETool-0.8.2/EEETools/Tools/API/Tools/__init__.py
--rw-rw-rw-   0        0        0      414 2022-04-08 08:08:33.000000 3ETool-0.8.2/EEETools/Tools/API/Tools/file_handler.py
--rw-rw-rw-   0        0        0    10079 2023-03-03 11:18:05.000000 3ETool-0.8.2/EEETools/Tools/API/Tools/main_tools.py
--rw-rw-rw-   0        0        0     8637 2023-03-03 12:01:14.000000 3ETool-0.8.2/EEETools/Tools/API/Tools/sankey_diagram_generation.py
--rw-rw-rw-   0        0        0        0 2022-04-08 08:08:33.000000 3ETool-0.8.2/EEETools/Tools/API/__init__.py
--rw-rw-rw-   0        0        0     4983 2023-02-27 09:21:54.000000 3ETool-0.8.2/EEETools/Tools/API/terminal_api.py
-drwxrwxrwx   0        0        0        0 2023-03-06 08:26:15.007119 3ETool-0.8.2/EEETools/Tools/CostCorrelations/
-drwxrwxrwx   0        0        0        0 2023-03-06 08:26:15.016118 3ETool-0.8.2/EEETools/Tools/CostCorrelations/CorrelationClasses/
--rw-rw-rw-   0        0        0       49 2022-04-08 08:08:33.000000 3ETool-0.8.2/EEETools/Tools/CostCorrelations/CorrelationClasses/__init__.py
--rw-rw-rw-   0        0        0    16432 2022-04-08 08:08:33.000000 3ETool-0.8.2/EEETools/Tools/CostCorrelations/CorrelationClasses/turton_correlation.py
--rw-rw-rw-   0        0        0        0 2022-04-08 08:08:33.000000 3ETool-0.8.2/EEETools/Tools/CostCorrelations/__init__.py
--rw-rw-rw-   0        0        0     6224 2022-04-08 08:08:33.000000 3ETool-0.8.2/EEETools/Tools/CostCorrelations/cost_correlation_classes.py
--rw-rw-rw-   0        0        0    22171 2022-04-08 08:08:33.000000 3ETool-0.8.2/EEETools/Tools/CostCorrelations/cost_correlation_gui.py
-drwxrwxrwx   0        0        0        0 2023-03-06 08:26:15.036322 3ETool-0.8.2/EEETools/Tools/EESCodeGenerator/
--rw-rw-rw-   0        0        0     2109 2022-04-08 08:08:33.000000 3ETool-0.8.2/EEETools/Tools/EESCodeGenerator/EES_checker.py
--rw-rw-rw-   0        0        0    11583 2022-04-08 08:08:33.000000 3ETool-0.8.2/EEETools/Tools/EESCodeGenerator/EES_code.py
--rw-rw-rw-   0        0        0    16306 2022-04-08 08:08:33.000000 3ETool-0.8.2/EEETools/Tools/EESCodeGenerator/EES_creator_tool.py
--rw-rw-rw-   0        0        0    25888 2022-04-08 08:08:33.000000 3ETool-0.8.2/EEETools/Tools/EESCodeGenerator/EES_parser.py
--rw-rw-rw-   0        0        0        0 2022-04-08 08:08:33.000000 3ETool-0.8.2/EEETools/Tools/EESCodeGenerator/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-06 08:26:15.053545 3ETool-0.8.2/EEETools/Tools/GUIElements/
--rw-rw-rw-   0        0        0        0 2022-04-08 08:08:33.000000 3ETool-0.8.2/EEETools/Tools/GUIElements/__init__.py
--rw-rw-rw-   0        0        0    14888 2022-04-08 08:08:33.000000 3ETool-0.8.2/EEETools/Tools/GUIElements/connection_and_block_check.py
--rw-rw-rw-   0        0        0    14296 2022-04-08 08:08:33.000000 3ETool-0.8.2/EEETools/Tools/GUIElements/gui_base_classes.py
--rw-rw-rw-   0        0        0      804 2022-04-08 08:08:33.000000 3ETool-0.8.2/EEETools/Tools/GUIElements/net_plot_modules.py
-drwxrwxrwx   0        0        0        0 2023-03-06 08:26:15.084663 3ETool-0.8.2/EEETools/Tools/Other/
--rw-rw-rw-   0        0        0        0 2022-04-08 08:08:33.000000 3ETool-0.8.2/EEETools/Tools/Other/__init__.py
--rw-rw-rw-   0        0        0     2731 2022-04-08 08:08:33.000000 3ETool-0.8.2/EEETools/Tools/Other/fernet_handler.py
--rw-rw-rw-   0        0        0     3974 2022-04-08 08:08:33.000000 3ETool-0.8.2/EEETools/Tools/Other/google_drive_downloader.py
--rw-rw-rw-   0        0        0     6791 2022-04-08 08:08:33.000000 3ETool-0.8.2/EEETools/Tools/Other/handler.py
--rw-rw-rw-   0        0        0    15775 2022-10-17 20:26:04.000000 3ETool-0.8.2/EEETools/Tools/Other/matrix_analyzer.py
--rw-rw-rw-   0        0        0     2337 2022-04-08 08:08:33.000000 3ETool-0.8.2/EEETools/Tools/Other/resource_downloader.py
--rw-rw-rw-   0        0        0     3484 2022-04-08 08:08:33.000000 3ETool-0.8.2/EEETools/Tools/Other/unisim_connect.py
--rw-rw-rw-   0        0        0        0 2022-04-08 08:08:33.000000 3ETool-0.8.2/EEETools/Tools/__init__.py
--rw-rw-rw-   0        0        0     3329 2022-04-08 08:08:33.000000 3ETool-0.8.2/EEETools/Tools/modules_handler.py
--rw-rw-rw-   0        0        0      733 2023-02-16 15:00:21.000000 3ETool-0.8.2/EEETools/__init__.py
--rw-rw-rw-   0        0        0     2717 2022-04-08 08:08:33.000000 3ETool-0.8.2/EEETools/costants.py
--rw-rw-rw-   0        0        0    41227 2022-04-08 08:08:33.000000 3ETool-0.8.2/EEETools/qrc_resources.py
--rw-rw-rw-   0        0        0       19 2023-03-06 08:24:36.000000 3ETool-0.8.2/EEETools/version.py
--rw-rw-rw-   0        0        0    35823 2022-04-08 08:08:33.000000 3ETool-0.8.2/LICENSE
--rw-rw-rw-   0        0        0     5747 2023-03-06 08:26:15.134237 3ETool-0.8.2/PKG-INFO
--rw-rw-rw-   0        0        0     4865 2023-02-17 10:16:07.000000 3ETool-0.8.2/README.md
--rw-rw-rw-   0        0        0       86 2023-03-06 08:26:15.135238 3ETool-0.8.2/setup.cfg
--rw-rw-rw-   0        0        0     2683 2022-10-17 20:27:23.000000 3ETool-0.8.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-06 08:26:15.133256 3ETool-0.8.2/test/
--rw-rw-rw-   0        0        0        0 2022-04-08 08:08:33.000000 3ETool-0.8.2/test/__init__.py
--rw-rw-rw-   0        0        0     2073 2022-04-08 08:08:33.000000 3ETool-0.8.2/test/test_EES_code.py
--rw-rw-rw-   0        0        0     1658 2022-04-08 08:08:33.000000 3ETool-0.8.2/test/test_EES_generator_UI.py
--rw-rw-rw-   0        0        0     1364 2022-04-08 08:08:33.000000 3ETool-0.8.2/test/test_GUI.py
--rw-rw-rw-   0        0        0     2125 2022-04-08 08:08:33.000000 3ETool-0.8.2/test/test_array_handler.py
--rw-rw-rw-   0        0        0     2648 2022-04-08 08:08:33.000000 3ETool-0.8.2/test/test_block_class.py
--rw-rw-rw-   0        0        0     2261 2022-04-08 08:08:33.000000 3ETool-0.8.2/test/test_cost_correlation.py
--rw-rw-rw-   0        0        0     5179 2023-03-03 10:40:26.000000 3ETool-0.8.2/test/test_import_module.py
--rw-rw-rw-   0        0        0      844 2022-04-08 08:08:33.000000 3ETool-0.8.2/test/test_modules_handler.py
--rw-rw-rw-   0        0        0     1088 2022-04-08 08:08:33.000000 3ETool-0.8.2/test/test_package.py
--rw-rw-rw-   0        0        0      474 2022-04-08 08:08:33.000000 3ETool-0.8.2/test/test_unisim_connector.py
+drwxrwxrwx   0        0        0        0 2023-06-01 09:43:24.399089 3ETool-0.8.3/
+drwxrwxrwx   0        0        0        0 2023-06-01 09:43:24.106829 3ETool-0.8.3/3ETool.egg-info/
+-rw-rw-rw-   0        0        0     5747 2023-06-01 09:43:23.000000 3ETool-0.8.3/3ETool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2784 2023-06-01 09:43:23.000000 3ETool-0.8.3/3ETool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 09:43:23.000000 3ETool-0.8.3/3ETool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      163 2023-06-01 09:43:23.000000 3ETool-0.8.3/3ETool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-01 09:43:23.000000 3ETool-0.8.3/3ETool.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-01 09:43:24.122828 3ETool-0.8.3/EEETools/
+drwxrwxrwx   0        0        0        0 2023-06-01 09:43:24.200180 3ETool-0.8.3/EEETools/BlockSubClasses/
+-rw-rw-rw-   0        0        0      438 2022-04-08 08:08:33.000000 3ETool-0.8.3/EEETools/BlockSubClasses/__init__.py
+-rw-rw-rw-   0        0        0     6290 2023-05-31 10:57:00.000000 3ETool-0.8.3/EEETools/BlockSubClasses/alternator.py
+-rw-rw-rw-   0        0        0     6198 2022-04-08 08:08:33.000000 3ETool-0.8.3/EEETools/BlockSubClasses/boiler.py
+-rw-rw-rw-   0        0        0     6277 2022-04-08 08:08:33.000000 3ETool-0.8.3/EEETools/BlockSubClasses/combustion_chamber.py
+-rw-rw-rw-   0        0        0     5580 2022-04-08 08:08:33.000000 3ETool-0.8.3/EEETools/BlockSubClasses/compressor.py
+-rw-rw-rw-   0        0        0     6598 2023-05-31 10:57:00.000000 3ETool-0.8.3/EEETools/BlockSubClasses/condenser.py
+-rw-rw-rw-   0        0        0     5662 2022-04-08 08:08:33.000000 3ETool-0.8.3/EEETools/BlockSubClasses/cooler.py
+-rw-rw-rw-   0        0        0     6626 2023-05-31 10:57:00.000000 3ETool-0.8.3/EEETools/BlockSubClasses/ejector_simplified.py
+-rw-rw-rw-   0        0        0     8566 2022-04-08 08:08:33.000000 3ETool-0.8.3/EEETools/BlockSubClasses/evaporator.py
+-rw-rw-rw-   0        0        0     5558 2022-04-08 08:08:33.000000 3ETool-0.8.3/EEETools/BlockSubClasses/expander.py
+-rw-rw-rw-   0        0        0     3969 2022-04-08 08:08:33.000000 3ETool-0.8.3/EEETools/BlockSubClasses/generic.py
+-rw-rw-rw-   0        0        0    10161 2022-04-08 08:08:33.000000 3ETool-0.8.3/EEETools/BlockSubClasses/heat_exchanger.py
+-rw-rw-rw-   0        0        0     3991 2022-04-08 08:08:33.000000 3ETool-0.8.3/EEETools/BlockSubClasses/mixer.py
+-rw-rw-rw-   0        0        0     5494 2022-04-08 08:08:33.000000 3ETool-0.8.3/EEETools/BlockSubClasses/pump.py
+-rw-rw-rw-   0        0        0     3998 2022-04-08 08:08:33.000000 3ETool-0.8.3/EEETools/BlockSubClasses/separator.py
+-rw-rw-rw-   0        0        0     5561 2022-04-08 08:08:33.000000 3ETool-0.8.3/EEETools/BlockSubClasses/valve.py
+drwxrwxrwx   0        0        0        0 2023-06-01 09:43:24.221274 3ETool-0.8.3/EEETools/MainModules/
+-rw-rw-rw-   0        0        0       60 2022-04-08 08:08:33.000000 3ETool-0.8.3/EEETools/MainModules/__init__.py
+-rw-rw-rw-   0        0        0    62304 2023-05-31 10:57:00.000000 3ETool-0.8.3/EEETools/MainModules/main_module.py
+-rw-rw-rw-   0        0        0     7015 2023-05-31 10:57:00.000000 3ETool-0.8.3/EEETools/MainModules/pf_diagram_generation_module.py
+-rw-rw-rw-   0        0        0    16475 2022-04-08 08:08:33.000000 3ETool-0.8.3/EEETools/MainModules/support_blocks.py
+drwxrwxrwx   0        0        0        0 2023-06-01 09:43:24.226280 3ETool-0.8.3/EEETools/Tools/
+drwxrwxrwx   0        0        0        0 2023-06-01 09:43:24.232306 3ETool-0.8.3/EEETools/Tools/API/
+drwxrwxrwx   0        0        0        0 2023-06-01 09:43:24.238356 3ETool-0.8.3/EEETools/Tools/API/DatAPI/
+-rw-rw-rw-   0        0        0        0 2022-04-08 08:08:33.000000 3ETool-0.8.3/EEETools/Tools/API/DatAPI/__init__.py
+-rw-rw-rw-   0        0        0     1369 2022-04-08 08:08:33.000000 3ETool-0.8.3/EEETools/Tools/API/DatAPI/modules_importer.py
+drwxrwxrwx   0        0        0        0 2023-06-01 09:43:24.245356 3ETool-0.8.3/EEETools/Tools/API/ExcelAPI/
+-rw-rw-rw-   0        0        0        0 2022-04-08 08:08:33.000000 3ETool-0.8.3/EEETools/Tools/API/ExcelAPI/__init__.py
+-rw-rw-rw-   0        0        0     7057 2023-03-03 10:59:27.000000 3ETool-0.8.3/EEETools/Tools/API/ExcelAPI/modules_importer.py
+drwxrwxrwx   0        0        0        0 2023-06-01 09:43:24.260564 3ETool-0.8.3/EEETools/Tools/API/Tools/
+-rw-rw-rw-   0        0        0        0 2022-04-08 08:08:33.000000 3ETool-0.8.3/EEETools/Tools/API/Tools/__init__.py
+-rw-rw-rw-   0        0        0      414 2022-04-08 08:08:33.000000 3ETool-0.8.3/EEETools/Tools/API/Tools/file_handler.py
+-rw-rw-rw-   0        0        0    10079 2023-03-03 11:18:05.000000 3ETool-0.8.3/EEETools/Tools/API/Tools/main_tools.py
+-rw-rw-rw-   0        0        0     8739 2023-05-31 10:57:00.000000 3ETool-0.8.3/EEETools/Tools/API/Tools/sankey_diagram_generation.py
+-rw-rw-rw-   0        0        0        0 2022-04-08 08:08:33.000000 3ETool-0.8.3/EEETools/Tools/API/__init__.py
+-rw-rw-rw-   0        0        0     5055 2023-05-31 11:11:39.000000 3ETool-0.8.3/EEETools/Tools/API/terminal_api.py
+drwxrwxrwx   0        0        0        0 2023-06-01 09:43:24.272321 3ETool-0.8.3/EEETools/Tools/CostCorrelations/
+drwxrwxrwx   0        0        0        0 2023-06-01 09:43:24.282302 3ETool-0.8.3/EEETools/Tools/CostCorrelations/CorrelationClasses/
+-rw-rw-rw-   0        0        0       49 2022-04-08 08:08:33.000000 3ETool-0.8.3/EEETools/Tools/CostCorrelations/CorrelationClasses/__init__.py
+-rw-rw-rw-   0        0        0    16432 2022-04-08 08:08:33.000000 3ETool-0.8.3/EEETools/Tools/CostCorrelations/CorrelationClasses/turton_correlation.py
+-rw-rw-rw-   0        0        0        0 2022-04-08 08:08:33.000000 3ETool-0.8.3/EEETools/Tools/CostCorrelations/__init__.py
+-rw-rw-rw-   0        0        0     6224 2022-04-08 08:08:33.000000 3ETool-0.8.3/EEETools/Tools/CostCorrelations/cost_correlation_classes.py
+-rw-rw-rw-   0        0        0    22171 2022-04-08 08:08:33.000000 3ETool-0.8.3/EEETools/Tools/CostCorrelations/cost_correlation_gui.py
+drwxrwxrwx   0        0        0        0 2023-06-01 09:43:24.306450 3ETool-0.8.3/EEETools/Tools/EESCodeGenerator/
+-rw-rw-rw-   0        0        0     2109 2022-04-08 08:08:33.000000 3ETool-0.8.3/EEETools/Tools/EESCodeGenerator/EES_checker.py
+-rw-rw-rw-   0        0        0    11583 2022-04-08 08:08:33.000000 3ETool-0.8.3/EEETools/Tools/EESCodeGenerator/EES_code.py
+-rw-rw-rw-   0        0        0    16306 2022-04-08 08:08:33.000000 3ETool-0.8.3/EEETools/Tools/EESCodeGenerator/EES_creator_tool.py
+-rw-rw-rw-   0        0        0    25888 2022-04-08 08:08:33.000000 3ETool-0.8.3/EEETools/Tools/EESCodeGenerator/EES_parser.py
+-rw-rw-rw-   0        0        0        0 2022-04-08 08:08:33.000000 3ETool-0.8.3/EEETools/Tools/EESCodeGenerator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 09:43:24.324450 3ETool-0.8.3/EEETools/Tools/GUIElements/
+-rw-rw-rw-   0        0        0        0 2022-04-08 08:08:33.000000 3ETool-0.8.3/EEETools/Tools/GUIElements/__init__.py
+-rw-rw-rw-   0        0        0    14888 2022-04-08 08:08:33.000000 3ETool-0.8.3/EEETools/Tools/GUIElements/connection_and_block_check.py
+-rw-rw-rw-   0        0        0    14296 2022-04-08 08:08:33.000000 3ETool-0.8.3/EEETools/Tools/GUIElements/gui_base_classes.py
+-rw-rw-rw-   0        0        0      804 2022-04-08 08:08:33.000000 3ETool-0.8.3/EEETools/Tools/GUIElements/net_plot_modules.py
+drwxrwxrwx   0        0        0        0 2023-06-01 09:43:24.352626 3ETool-0.8.3/EEETools/Tools/Other/
+-rw-rw-rw-   0        0        0        0 2022-04-08 08:08:33.000000 3ETool-0.8.3/EEETools/Tools/Other/__init__.py
+-rw-rw-rw-   0        0        0     2731 2022-04-08 08:08:33.000000 3ETool-0.8.3/EEETools/Tools/Other/fernet_handler.py
+-rw-rw-rw-   0        0        0     3974 2022-04-08 08:08:33.000000 3ETool-0.8.3/EEETools/Tools/Other/google_drive_downloader.py
+-rw-rw-rw-   0        0        0     6791 2022-04-08 08:08:33.000000 3ETool-0.8.3/EEETools/Tools/Other/handler.py
+-rw-rw-rw-   0        0        0    15775 2022-10-17 20:26:04.000000 3ETool-0.8.3/EEETools/Tools/Other/matrix_analyzer.py
+-rw-rw-rw-   0        0        0     2337 2022-04-08 08:08:33.000000 3ETool-0.8.3/EEETools/Tools/Other/resource_downloader.py
+-rw-rw-rw-   0        0        0     3484 2022-04-08 08:08:33.000000 3ETool-0.8.3/EEETools/Tools/Other/unisim_connect.py
+-rw-rw-rw-   0        0        0        0 2022-04-08 08:08:33.000000 3ETool-0.8.3/EEETools/Tools/__init__.py
+-rw-rw-rw-   0        0        0     3329 2022-04-08 08:08:33.000000 3ETool-0.8.3/EEETools/Tools/modules_handler.py
+-rw-rw-rw-   0        0        0      733 2023-02-16 15:00:21.000000 3ETool-0.8.3/EEETools/__init__.py
+-rw-rw-rw-   0        0        0     2717 2022-04-08 08:08:33.000000 3ETool-0.8.3/EEETools/costants.py
+-rw-rw-rw-   0        0        0    41227 2022-04-08 08:08:33.000000 3ETool-0.8.3/EEETools/qrc_resources.py
+-rw-rw-rw-   0        0        0       19 2023-05-31 10:57:00.000000 3ETool-0.8.3/EEETools/version.py
+-rw-rw-rw-   0        0        0    35823 2022-04-08 08:08:33.000000 3ETool-0.8.3/LICENSE
+-rw-rw-rw-   0        0        0     5747 2023-06-01 09:43:24.399089 3ETool-0.8.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4865 2023-02-17 10:16:07.000000 3ETool-0.8.3/README.md
+-rw-rw-rw-   0        0        0       86 2023-06-01 09:43:24.400088 3ETool-0.8.3/setup.cfg
+-rw-rw-rw-   0        0        0     2683 2022-10-17 20:27:23.000000 3ETool-0.8.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 09:43:24.398090 3ETool-0.8.3/test/
+-rw-rw-rw-   0        0        0        0 2022-04-08 08:08:33.000000 3ETool-0.8.3/test/__init__.py
+-rw-rw-rw-   0        0        0     2073 2022-04-08 08:08:33.000000 3ETool-0.8.3/test/test_EES_code.py
+-rw-rw-rw-   0        0        0     1658 2022-04-08 08:08:33.000000 3ETool-0.8.3/test/test_EES_generator_UI.py
+-rw-rw-rw-   0        0        0     1364 2022-04-08 08:08:33.000000 3ETool-0.8.3/test/test_GUI.py
+-rw-rw-rw-   0        0        0     2125 2022-04-08 08:08:33.000000 3ETool-0.8.3/test/test_array_handler.py
+-rw-rw-rw-   0        0        0     2648 2022-04-08 08:08:33.000000 3ETool-0.8.3/test/test_block_class.py
+-rw-rw-rw-   0        0        0     2261 2022-04-08 08:08:33.000000 3ETool-0.8.3/test/test_cost_correlation.py
+-rw-rw-rw-   0        0        0     5276 2023-06-01 09:33:24.000000 3ETool-0.8.3/test/test_import_module.py
+-rw-rw-rw-   0        0        0      844 2022-04-08 08:08:33.000000 3ETool-0.8.3/test/test_modules_handler.py
+-rw-rw-rw-   0        0        0     1088 2022-04-08 08:08:33.000000 3ETool-0.8.3/test/test_package.py
+-rw-rw-rw-   0        0        0      474 2022-04-08 08:08:33.000000 3ETool-0.8.3/test/test_unisim_connector.py
```

### Comparing `3ETool-0.8.2/3ETool.egg-info/PKG-INFO` & `3ETool-0.8.3/3ETool.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: 3ETool
-Version: 0.8.2
+Version: 0.8.3
 Summary: Tools for performing exergo-economic and exergo-environmental analysis
 Home-page: https://tinyurl.com/SERG-3ETool
-Download-URL: https://github.com/SERGGroup/3ETool/archive/refs/tags/0.8.2.tar.gz
+Download-URL: https://github.com/SERGGroup/3ETool/archive/refs/tags/0.8.3.tar.gz
 Author: Pietro Ungar
 Author-email: pietro.ungar@unifi.it
 License: GNU GPLv3
 Project-URL: Documentation, https://drive.google.com/file/d/1Dzdz4_EAKyY9c8nOm2SKTIqSXfV74w2-/view?usp=sharing
 Project-URL: Source, https://github.com/SERGGroup/3ETool
 Project-URL: Tracker, https://github.com/SERGGroup/3ETool/issues
 Platform: UNKNOWN
```

### Comparing `3ETool-0.8.2/3ETool.egg-info/SOURCES.txt` & `3ETool-0.8.3/3ETool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `3ETool-0.8.2/EEETools/BlockSubClasses/alternator.py` & `3ETool-0.8.3/EEETools/BlockSubClasses/alternator.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         return len(self.support_block[0].input_connections) >= 1
 
     def prepare_for_calculation(self):
 
         self.support_block[0].prepare_for_calculation()
 
         new_conn = self.main_class.append_connection(from_block=self)
-        new_conn.name = "electrical power output"
+        new_conn.name = "Electrical Power Output"
         new_conn.is_useful_effect = True
         new_conn.automatically_generated_connection = True
         new_conn.exergy_value = self.exergy_balance
 
     def initialize_connection_list(self, input_list):
 
         self.efficiency = float(input_list[0])
```

### Comparing `3ETool-0.8.2/EEETools/BlockSubClasses/boiler.py` & `3ETool-0.8.3/EEETools/BlockSubClasses/boiler.py`

 * *Files identical despite different names*

### Comparing `3ETool-0.8.2/EEETools/BlockSubClasses/combustion_chamber.py` & `3ETool-0.8.3/EEETools/BlockSubClasses/combustion_chamber.py`

 * *Files identical despite different names*

### Comparing `3ETool-0.8.2/EEETools/BlockSubClasses/compressor.py` & `3ETool-0.8.3/EEETools/BlockSubClasses/compressor.py`

 * *Files identical despite different names*

### Comparing `3ETool-0.8.2/EEETools/BlockSubClasses/condenser.py` & `3ETool-0.8.3/EEETools/BlockSubClasses/condenser.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         if self.main_class.options.condenser_is_dissipative:
 
             self.support_block[0].prepare_for_calculation()
 
         if self.main_class.options.loss_cost_is_zero:
 
             new_conn = self.main_class.append_connection(from_block=self)
-            new_conn.name = "condenser exergy loss"
+            new_conn.name = "Condenser Exergy Loss"
             new_conn.automatically_generated_connection = True
             new_conn.exergy_value = self.exergy_balance
             new_conn.is_fluid_stream = False
 
     def initialize_connection_list(self, input_list):
 
         new_input_conn = self.main_class.find_connection_by_index(input_list[0])
```

### Comparing `3ETool-0.8.2/EEETools/BlockSubClasses/cooler.py` & `3ETool-0.8.3/EEETools/BlockSubClasses/cooler.py`

 * *Files identical despite different names*

### Comparing `3ETool-0.8.2/EEETools/BlockSubClasses/ejector_simplified.py` & `3ETool-0.8.3/EEETools/BlockSubClasses/ejector_simplified.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         new_conn = self.main_class.append_connection(from_block=self)
 
     def prepare_for_calculation(self):
 
         self.support_block[0].prepare_for_calculation()
 
         new_conn = self.main_class.append_connection(from_block=self)
-        new_conn.name = "electrical power output"
+        new_conn.name = "Electrical Power Output"
         new_conn.is_useful_effect = True
         new_conn.automatically_generated_connection = True
         new_conn.exergy_value = self.exergy_balance
 
     def export_xml_connection_list(self) -> ETree.Element:
 
         xml_connection_list = ETree.Element("Connections")
```

### Comparing `3ETool-0.8.2/EEETools/BlockSubClasses/evaporator.py` & `3ETool-0.8.3/EEETools/BlockSubClasses/evaporator.py`

 * *Files identical despite different names*

### Comparing `3ETool-0.8.2/EEETools/BlockSubClasses/expander.py` & `3ETool-0.8.3/EEETools/BlockSubClasses/expander.py`

 * *Files identical despite different names*

### Comparing `3ETool-0.8.2/EEETools/BlockSubClasses/generic.py` & `3ETool-0.8.3/EEETools/BlockSubClasses/generic.py`

 * *Files identical despite different names*

### Comparing `3ETool-0.8.2/EEETools/BlockSubClasses/heat_exchanger.py` & `3ETool-0.8.3/EEETools/BlockSubClasses/heat_exchanger.py`

 * *Files identical despite different names*

### Comparing `3ETool-0.8.2/EEETools/BlockSubClasses/mixer.py` & `3ETool-0.8.3/EEETools/BlockSubClasses/mixer.py`

 * *Files identical despite different names*

### Comparing `3ETool-0.8.2/EEETools/BlockSubClasses/pump.py` & `3ETool-0.8.3/EEETools/BlockSubClasses/pump.py`

 * *Files identical despite different names*

### Comparing `3ETool-0.8.2/EEETools/BlockSubClasses/separator.py` & `3ETool-0.8.3/EEETools/BlockSubClasses/separator.py`

 * *Files identical despite different names*

### Comparing `3ETool-0.8.2/EEETools/BlockSubClasses/valve.py` & `3ETool-0.8.3/EEETools/BlockSubClasses/valve.py`

 * *Files identical despite different names*

### Comparing `3ETool-0.8.2/EEETools/MainModules/main_module.py` & `3ETool-0.8.3/EEETools/MainModules/main_module.py`

 * *Files 1% similar despite different names*

```diff
@@ -281,20 +281,25 @@
         f = 0
         y = 0
         eta = 0
 
         c_fuel = 0
         c_dest = 0
 
+        self.calculate_exergy_analysis()
         fuel_exergy = self.exergy_analysis["fuel"]
         dest_exergy = self.exergy_analysis["distruction"]
         dest_loss_exergy = self.exergy_analysis["distruction"] + self.exergy_analysis["losses"]
 
         fuel_cost = 0.
 
+        if self.can_be_removed_in_pf_definition and self.main_class.options.calculate_on_pf_diagram:
+
+            self.output_cost = self.output_connections[0].rel_cost
+
         if self.is_dissipative:
 
             c_prod = self.dissipative_output_cost
 
         else:
 
             c_prod = self.output_cost
@@ -311,19 +316,19 @@
                 eta = 1/eta
 
             c_fuel = fuel_cost / abs(fuel_exergy)
             c_dest = c_fuel
 
         if not c_fuel == 0:
 
-            r = (self.output_cost - c_fuel) / c_fuel
+            r = (c_prod - c_fuel) / c_fuel
 
         if not (self.comp_cost + c_dest * abs(dest_loss_exergy)) == 0:
 
-            f = self.comp_cost / (self.comp_cost + c_dest * abs(dest_loss_exergy))
+            f = self.comp_cost / (self.comp_cost + c_dest * abs(dest_exergy))
 
         if not total_destruction == 0:
 
             y = dest_exergy / total_destruction
 
         self.coefficients.update({
 
@@ -522,16 +527,14 @@
                     warningString += " connection not updated"
 
                     warnings.warn(warningString)
                     return
 
             sel_block.add_connection(new_connection, is_input)
 
-        self.calculate_exergy_analysis()
-
     def remove_connection(self, deleted_conn):
 
         # This method tries to remove the connection from the input_connections List (it can do that because
         # connection class has __eq__ method implemented) if the elimination does not succeed (i.e. there is not such
         # connection in the List) it rises a warning and exit
 
         # The method search the connection to be deleted in the input_connection list and in the output_connection
@@ -1363,14 +1366,16 @@
 
             if self.options.calculate_on_pf_diagram and "PFArrayHandler" not in str(type(self)):
 
                 from EEETools.MainModules.pf_diagram_generation_module import PFArrayHandler
                 self.pf_diagram = PFArrayHandler(self)
                 self.pf_diagram.calculate()
 
+                self.calculate_coefficients()
+
             else:
 
                 i = 0
                 n_elements = self.n_block
 
                 self.matrix = np.zeros((n_elements, n_elements))
                 self.vector = np.zeros(n_elements)
@@ -1417,14 +1422,20 @@
 
         total_destruction = self.total_destruction
 
         for block in self.block_list:
 
             block.calculate_coefficients(total_destruction)
 
+    def calculate_exergy_analysis(self):
+
+        for block in self.block_list:
+
+            block.calculate_exergy_analysis()
+
     def decompose_component_output_cost(self):
 
         if self.options.calculate_component_decomposition:
 
             try:
 
                 __inverse_matrix = np.linalg.inv(self.matrix)
@@ -1448,14 +1459,15 @@
                     self.options.calculate_component_decomposition = False
 
     def prepare_system(self):
 
         # this method has to be called just before the calculation, it asks the blocks to prepare themselves for the
         # calculation
 
+        self.calculate_exergy_analysis()
         self.__update_block_list()
 
         for block in self.block_list:
             block.prepare_for_calculation()
 
         if self.there_are_dissipative_blocks:
             self.__move_skipped_element_at_the_end()
@@ -1570,20 +1582,22 @@
             self.__reset_IDs(reset_block=True)
 
             return new_block
 
     def append_connection(self, new_conn=None, from_block=None, to_block=None) -> Connection:
 
         if new_conn is None:
-            new_conn = Connection(self.n_connection)
+
+            new_conn = Connection(self.__get_empty_index())
 
         self.__try_append_connection(new_conn, from_block, is_input=False)
         self.__try_append_connection(new_conn, to_block, is_input=True)
 
         if not new_conn in self.connection_list:
+
             self.connection_list.append(new_conn)
             self.__reset_IDs(reset_block=False)
 
         return new_conn
 
     def remove_block(self, block, disconnect_block=True):
 
@@ -1900,19 +1914,20 @@
 
         self.n_block = len(self.block_list)
         self.n_connection = len(self.connection_list)
 
     def __update_block_list(self):
 
         # this method asks the blocks to generate their own support blocks (if needed) and appends them to the
-        # block list. Finally it orders the lists and reset the IDs.
+        # block list. Finally, it orders the lists and reset the IDs.
 
         for block in self.block_list:
 
             if block.has_support_block:
+
                 block_list = block.support_block
                 self.append_block(block_list)
 
         self.__reset_IDs(reset_block=True)
 
     def __move_skipped_element_at_the_end(self):
 
@@ -1920,14 +1935,29 @@
             block.move_skipped_block_at_the_end = True
 
         self.__reset_IDs(reset_block=True)
 
         for block in self.block_list:
             block.move_skipped_block_at_the_end = False
 
+    def __get_empty_index(self):
+
+        i = 0
+        j = 0
+
+        while np.power(10, i) < self.n_connection:
+
+            i += 1
+
+        while self.find_connection_by_index(int(np.power(10, i)) + j) is not None:
+
+            j += 1
+
+        return int(np.power(10, i)) + j
+
     @property
     def blocks_by_index(self):
 
         new_block_list = list()
         for block in self.block_list:
 
             inserted = False
```

### Comparing `3ETool-0.8.2/EEETools/MainModules/pf_diagram_generation_module.py` & `3ETool-0.8.3/EEETools/MainModules/pf_diagram_generation_module.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import warnings
-
 from EEETools.MainModules.main_module import Connection, ArrayHandler, Block
 from EEETools.BlockSubClasses.generic import Generic
 
 
 class ProductBlock(Generic):
 
     def __init__(self, inputID, main_class, base_block: Block):
@@ -28,14 +26,22 @@
             self.contained_connection.append(new_connection)
 
     def append_output_cost(self, defined_steam_cost):
 
         super().append_output_cost(defined_steam_cost)
         self.base_block.append_output_cost(defined_steam_cost)
 
+        for outConn in self.contained_connection:
+
+            if outConn.is_loss and self.main_class.options.loss_cost_is_zero:
+                outConn.set_cost(0.)
+
+            else:
+                outConn.set_cost(self.output_cost)
+
     def generate_output_cost_decomposition(self, inverse_matrix_row):
 
         super(ProductBlock, self).generate_output_cost_decomposition(inverse_matrix_row)
 
         for block in self.contained_blocks:
             block.output_cost_decomposition = self.output_cost_decomposition
 
@@ -57,15 +63,14 @@
             return element in self.contained_blocks
 
     def calculate_coefficients(self, total_destruction):
 
         super(ProductBlock, self).calculate_coefficients(total_destruction)
 
         self.base_block.coefficients = self.coefficients
-        self.base_block.exergy_analysis = self.exergy_analysis
 
     def __check_connection(self, conn):
 
         if conn.is_system_output:
 
             self.main_class.generate_product_connection(conn, from_product_block=self)
```

### Comparing `3ETool-0.8.2/EEETools/MainModules/support_blocks.py` & `3ETool-0.8.3/EEETools/MainModules/support_blocks.py`

 * *Files identical despite different names*

### Comparing `3ETool-0.8.2/EEETools/Tools/API/DatAPI/modules_importer.py` & `3ETool-0.8.3/EEETools/Tools/API/DatAPI/modules_importer.py`

 * *Files identical despite different names*

### Comparing `3ETool-0.8.2/EEETools/Tools/API/ExcelAPI/modules_importer.py` & `3ETool-0.8.3/EEETools/Tools/API/ExcelAPI/modules_importer.py`

 * *Files identical despite different names*

### Comparing `3ETool-0.8.2/EEETools/Tools/API/Tools/main_tools.py` & `3ETool-0.8.3/EEETools/Tools/API/Tools/main_tools.py`

 * *Files identical despite different names*

### Comparing `3ETool-0.8.2/EEETools/Tools/API/Tools/sankey_diagram_generation.py` & `3ETool-0.8.3/EEETools/Tools/API/Tools/sankey_diagram_generation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-import math
-
 from EEETools.MainModules.pf_diagram_generation_module import ArrayHandler
+import math
 
 
 class SankeyDiagramOptions:
 
     def __init__(self):
 
         self.generate_on_pf_diagram = False
@@ -200,15 +199,22 @@
 
             else:
 
                 value = conn.abs_cost
 
                 rel_cost = conn.rel_cost
                 max_rel_cost = self.__get_maximum_rel_cost()
-                perc = rel_cost / max_rel_cost * (1 - self.options.min_opacity_perc) + self.options.min_opacity_perc
+
+                if max_rel_cost == 0:
+
+                    perc = 1
+
+                else:
+
+                    perc = rel_cost / max_rel_cost * (1 - self.options.min_opacity_perc) + self.options.min_opacity_perc
 
                 color = self.options.define_color(to_block_label, is_link=True, cost_perc=perc)
 
             self.link_dict["value"].append(value)
             self.link_dict["color"].append(color)
 
     def __check_label(self, label):
```

### Comparing `3ETool-0.8.2/EEETools/Tools/API/terminal_api.py` & `3ETool-0.8.3/EEETools/Tools/API/terminal_api.py`

 * *Files 7% similar despite different names*

```diff
@@ -76,15 +76,15 @@
     display_network(array_handler)
 
 
 def plot_sankey(
 
         excel_path="", show_component_mixers=False,
         generate_on_pf_diagram=True, display_costs=False,
-        font_size=15
+        font_size=15, min_opacity_perc=0.15
 
 ):
 
     from EEETools.Tools.API.Tools.sankey_diagram_generation import SankeyDiagramGenerator, SankeyDiagramOptions
     excel_path = __find_excel_path(excel_path)
     if excel_path == "":
         return
@@ -92,14 +92,15 @@
     array_handler = import_excel_input(excel_path)
 
     options = SankeyDiagramOptions()
     options.generate_on_pf_diagram = generate_on_pf_diagram
     options.show_component_mixers = show_component_mixers
     options.display_costs = display_costs
     options.font_size = font_size
+    options.min_opacity_perc = min_opacity_perc
 
     SankeyDiagramGenerator(array_handler, options).show()
 
 
 def paste_default_excel_file():
     __import_file("Default Excel Input_eng.xlsm")
```

### Comparing `3ETool-0.8.2/EEETools/Tools/CostCorrelations/CorrelationClasses/turton_correlation.py` & `3ETool-0.8.3/EEETools/Tools/CostCorrelations/CorrelationClasses/turton_correlation.py`

 * *Files identical despite different names*

### Comparing `3ETool-0.8.2/EEETools/Tools/CostCorrelations/cost_correlation_classes.py` & `3ETool-0.8.3/EEETools/Tools/CostCorrelations/cost_correlation_classes.py`

 * *Files identical despite different names*

### Comparing `3ETool-0.8.2/EEETools/Tools/CostCorrelations/cost_correlation_gui.py` & `3ETool-0.8.3/EEETools/Tools/CostCorrelations/cost_correlation_gui.py`

 * *Files identical despite different names*

### Comparing `3ETool-0.8.2/EEETools/Tools/EESCodeGenerator/EES_checker.py` & `3ETool-0.8.3/EEETools/Tools/EESCodeGenerator/EES_checker.py`

 * *Files identical despite different names*

### Comparing `3ETool-0.8.2/EEETools/Tools/EESCodeGenerator/EES_code.py` & `3ETool-0.8.3/EEETools/Tools/EESCodeGenerator/EES_code.py`

 * *Files identical despite different names*

### Comparing `3ETool-0.8.2/EEETools/Tools/EESCodeGenerator/EES_creator_tool.py` & `3ETool-0.8.3/EEETools/Tools/EESCodeGenerator/EES_creator_tool.py`

 * *Files identical despite different names*

### Comparing `3ETool-0.8.2/EEETools/Tools/EESCodeGenerator/EES_parser.py` & `3ETool-0.8.3/EEETools/Tools/EESCodeGenerator/EES_parser.py`

 * *Files identical despite different names*

### Comparing `3ETool-0.8.2/EEETools/Tools/GUIElements/connection_and_block_check.py` & `3ETool-0.8.3/EEETools/Tools/GUIElements/connection_and_block_check.py`

 * *Files identical despite different names*

### Comparing `3ETool-0.8.2/EEETools/Tools/GUIElements/gui_base_classes.py` & `3ETool-0.8.3/EEETools/Tools/GUIElements/gui_base_classes.py`

 * *Files identical despite different names*

### Comparing `3ETool-0.8.2/EEETools/Tools/GUIElements/net_plot_modules.py` & `3ETool-0.8.3/EEETools/Tools/GUIElements/net_plot_modules.py`

 * *Files identical despite different names*

### Comparing `3ETool-0.8.2/EEETools/Tools/Other/fernet_handler.py` & `3ETool-0.8.3/EEETools/Tools/Other/fernet_handler.py`

 * *Files identical despite different names*

### Comparing `3ETool-0.8.2/EEETools/Tools/Other/google_drive_downloader.py` & `3ETool-0.8.3/EEETools/Tools/Other/google_drive_downloader.py`

 * *Files identical despite different names*

### Comparing `3ETool-0.8.2/EEETools/Tools/Other/handler.py` & `3ETool-0.8.3/EEETools/Tools/Other/handler.py`

 * *Files identical despite different names*

### Comparing `3ETool-0.8.2/EEETools/Tools/Other/matrix_analyzer.py` & `3ETool-0.8.3/EEETools/Tools/Other/matrix_analyzer.py`

 * *Files identical despite different names*

### Comparing `3ETool-0.8.2/EEETools/Tools/Other/resource_downloader.py` & `3ETool-0.8.3/EEETools/Tools/Other/resource_downloader.py`

 * *Files identical despite different names*

### Comparing `3ETool-0.8.2/EEETools/Tools/Other/unisim_connect.py` & `3ETool-0.8.3/EEETools/Tools/Other/unisim_connect.py`

 * *Files identical despite different names*

### Comparing `3ETool-0.8.2/EEETools/Tools/modules_handler.py` & `3ETool-0.8.3/EEETools/Tools/modules_handler.py`

 * *Files identical despite different names*

### Comparing `3ETool-0.8.2/EEETools/__init__.py` & `3ETool-0.8.3/EEETools/__init__.py`

 * *Files identical despite different names*

### Comparing `3ETool-0.8.2/EEETools/costants.py` & `3ETool-0.8.3/EEETools/costants.py`

 * *Files identical despite different names*

### Comparing `3ETool-0.8.2/EEETools/qrc_resources.py` & `3ETool-0.8.3/EEETools/qrc_resources.py`

 * *Files identical despite different names*

### Comparing `3ETool-0.8.2/LICENSE` & `3ETool-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `3ETool-0.8.2/PKG-INFO` & `3ETool-0.8.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: 3ETool
-Version: 0.8.2
+Version: 0.8.3
 Summary: Tools for performing exergo-economic and exergo-environmental analysis
 Home-page: https://tinyurl.com/SERG-3ETool
-Download-URL: https://github.com/SERGGroup/3ETool/archive/refs/tags/0.8.2.tar.gz
+Download-URL: https://github.com/SERGGroup/3ETool/archive/refs/tags/0.8.3.tar.gz
 Author: Pietro Ungar
 Author-email: pietro.ungar@unifi.it
 License: GNU GPLv3
 Project-URL: Documentation, https://drive.google.com/file/d/1Dzdz4_EAKyY9c8nOm2SKTIqSXfV74w2-/view?usp=sharing
 Project-URL: Source, https://github.com/SERGGroup/3ETool
 Project-URL: Tracker, https://github.com/SERGGroup/3ETool/issues
 Platform: UNKNOWN
```

### Comparing `3ETool-0.8.2/README.md` & `3ETool-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `3ETool-0.8.2/setup.py` & `3ETool-0.8.3/setup.py`

 * *Files identical despite different names*

### Comparing `3ETool-0.8.2/test/test_EES_code.py` & `3ETool-0.8.3/test/test_EES_code.py`

 * *Files identical despite different names*

### Comparing `3ETool-0.8.2/test/test_EES_generator_UI.py` & `3ETool-0.8.3/test/test_EES_generator_UI.py`

 * *Files identical despite different names*

### Comparing `3ETool-0.8.2/test/test_GUI.py` & `3ETool-0.8.3/test/test_GUI.py`

 * *Files identical despite different names*

### Comparing `3ETool-0.8.2/test/test_array_handler.py` & `3ETool-0.8.3/test/test_array_handler.py`

 * *Files identical despite different names*

### Comparing `3ETool-0.8.2/test/test_block_class.py` & `3ETool-0.8.3/test/test_block_class.py`

 * *Files identical despite different names*

### Comparing `3ETool-0.8.2/test/test_cost_correlation.py` & `3ETool-0.8.3/test/test_cost_correlation.py`

 * *Files identical despite different names*

### Comparing `3ETool-0.8.2/test/test_import_module.py` & `3ETool-0.8.3/test/test_import_module.py`

 * *Files 4% similar despite different names*

```diff
@@ -107,15 +107,21 @@
         FernetHandler()
 
         self.assertTrue(True)
 
     def test_excel_calculate(self):
 
         import EEETools
-        EEETools.calculate(calculate_on_pf_diagram=True)
+        EEETools.calculate(
+
+            calculate_on_pf_diagram=True,
+            condenser_is_dissipative=True,
+            loss_cost_is_zero=True,
+
+        )
         self.assertTrue(True)
 
     def test_excel_debug(self):
 
         import EEETools
         EEETools.export_debug_information(calculate_on_pf_diagram=True)
         self.assertTrue(True)
@@ -139,15 +145,15 @@
         connection = updated_exergy_values[0]
         array_handler = calculate_excel(excel_path, new_exergy_list=updated_exergy_values, export_solution=False)
         self.assertEqual(connection["value"], array_handler.find_connection_by_index(connection["index"]).exergy_value)
 
     def test_sankey(self):
 
         import EEETools
-        EEETools.plot_sankey(generate_on_pf_diagram=True, display_costs=True, font_size=15)
+        EEETools.plot_sankey(generate_on_pf_diagram=True, display_costs=False)
         self.assertTrue(True)
 
     def test_connection_check(self):
 
         import EEETools
         EEETools.launch_connection_debug()
         self.assertTrue(True)
```

### Comparing `3ETool-0.8.2/test/test_modules_handler.py` & `3ETool-0.8.3/test/test_modules_handler.py`

 * *Files identical despite different names*

### Comparing `3ETool-0.8.2/test/test_package.py` & `3ETool-0.8.3/test/test_package.py`

 * *Files identical despite different names*

