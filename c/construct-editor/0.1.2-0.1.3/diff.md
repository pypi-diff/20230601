# Comparing `tmp/construct-editor-0.1.2.tar.gz` & `tmp/construct-editor-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "construct-editor-0.1.2.tar", last modified: Tue May  9 11:27:00 2023, max compression
+gzip compressed data, was "construct-editor-0.1.3.tar", last modified: Thu Jun  1 07:56:59 2023, max compression
```

## Comparing `construct-editor-0.1.2.tar` & `construct-editor-0.1.3.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:27:00.623731 construct-editor-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-09 11:26:46.000000 construct-editor-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-05-09 11:27:00.623731 construct-editor-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-05-09 11:26:46.000000 construct-editor-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:27:00.619730 construct-editor-0.1.2/construct_editor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 11:26:46.000000 construct-editor-0.1.2/construct_editor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:27:00.619730 construct-editor-0.1.2/construct_editor/core/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-09 11:26:46.000000 construct-editor-0.1.2/construct_editor/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-09 11:26:46.000000 construct-editor-0.1.2/construct_editor/core/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5031 2023-05-09 11:26:46.000000 construct-editor-0.1.2/construct_editor/core/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    12727 2023-05-09 11:26:46.000000 construct-editor-0.1.2/construct_editor/core/construct_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-05-09 11:26:46.000000 construct-editor-0.1.2/construct_editor/core/context_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-05-09 11:26:46.000000 construct-editor-0.1.2/construct_editor/core/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)    62952 2023-05-09 11:26:46.000000 construct-editor-0.1.2/construct_editor/core/entries.py
--rw-r--r--   0 runner    (1001) docker     (123)     6068 2023-05-09 11:26:46.000000 construct-editor-0.1.2/construct_editor/core/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-05-09 11:26:46.000000 construct-editor-0.1.2/construct_editor/core/preprocessor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:27:00.623731 construct-editor-0.1.2/construct_editor/gallery/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-09 11:26:46.000000 construct-editor-0.1.2/construct_editor/gallery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-05-09 11:26:46.000000 construct-editor-0.1.2/construct_editor/gallery/example_cmd_resp.py
--rw-r--r--   0 runner    (1001) docker     (123)    27072 2023-05-09 11:26:46.000000 construct-editor-0.1.2/construct_editor/gallery/example_ipstack.py
--rw-r--r--   0 runner    (1001) docker     (123)     7829 2023-05-09 11:26:46.000000 construct-editor-0.1.2/construct_editor/gallery/example_pe32coff.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-09 11:26:46.000000 construct-editor-0.1.2/construct_editor/gallery/test_aligned.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-05-09 11:26:46.000000 construct-editor-0.1.2/construct_editor/gallery/test_array.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-09 11:26:46.000000 construct-editor-0.1.2/construct_editor/gallery/test_bits_swapped_bitwise.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-09 11:26:46.000000 construct-editor-0.1.2/construct_editor/gallery/test_bitwise.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-09 11:26:46.000000 construct-editor-0.1.2/construct_editor/gallery/test_bytes_greedybytes.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-09 11:26:46.000000 construct-editor-0.1.2/construct_editor/gallery/test_checksum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-05-09 11:26:46.000000 construct-editor-0.1.2/construct_editor/gallery/test_compressed.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-09 11:26:46.000000 construct-editor-0.1.2/construct_editor/gallery/test_computed.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-09 11:26:46.000000 construct-editor-0.1.2/construct_editor/gallery/test_const.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-09 11:26:46.000000 construct-editor-0.1.2/construct_editor/gallery/test_dataclass_bit_struct.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-09 11:26:46.000000 construct-editor-0.1.2/construct_editor/gallery/test_dataclass_struct.py
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-09 11:26:46.000000 construct-editor-0.1.2/construct_editor/gallery/test_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-09 11:26:46.000000 construct-editor-0.1.2/construct_editor/gallery/test_fixedsized.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-09 11:26:46.000000 construct-editor-0.1.2/construct_editor/gallery/test_flag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-05-09 11:26:46.000000 construct-editor-0.1.2/construct_editor/gallery/test_flagsenum.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-09 11:26:46.000000 construct-editor-0.1.2/construct_editor/gallery/test_focusedseq.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-09 11:26:46.000000 construct-editor-0.1.2/construct_editor/gallery/test_greedyrange.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-09 11:26:46.000000 construct-editor-0.1.2/construct_editor/gallery/test_ifthenelse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-09 11:26:46.000000 construct-editor-0.1.2/construct_editor/gallery/test_ifthenelse_nested_switch.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-09 11:26:46.000000 construct-editor-0.1.2/construct_editor/gallery/test_nullstripped.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-09 11:26:46.000000 construct-editor-0.1.2/construct_editor/gallery/test_nullterminated.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-09 11:26:46.000000 construct-editor-0.1.2/construct_editor/gallery/test_padded.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-09 11:26:46.000000 construct-editor-0.1.2/construct_editor/gallery/test_padded_string.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-09 11:26:46.000000 construct-editor-0.1.2/construct_editor/gallery/test_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-09 11:26:46.000000 construct-editor-0.1.2/construct_editor/gallery/test_pointer_peek_seek_tell.py
--rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-05-09 11:26:46.000000 construct-editor-0.1.2/construct_editor/gallery/test_renamed.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-09 11:26:46.000000 construct-editor-0.1.2/construct_editor/gallery/test_select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-05-09 11:26:46.000000 construct-editor-0.1.2/construct_editor/gallery/test_select_complex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-05-09 11:26:46.000000 construct-editor-0.1.2/construct_editor/gallery/test_stringencodded.py
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-05-09 11:26:46.000000 construct-editor-0.1.2/construct_editor/gallery/test_switch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-05-09 11:26:46.000000 construct-editor-0.1.2/construct_editor/gallery/test_switch_dataclass.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-05-09 11:26:46.000000 construct-editor-0.1.2/construct_editor/gallery/test_tenum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-05-09 11:26:46.000000 construct-editor-0.1.2/construct_editor/gallery/test_tflagsenum.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-09 11:26:46.000000 construct-editor-0.1.2/construct_editor/gallery/test_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)    20479 2023-05-09 11:26:46.000000 construct-editor-0.1.2/construct_editor/main.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 11:26:46.000000 construct-editor-0.1.2/construct_editor/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-09 11:26:46.000000 construct-editor-0.1.2/construct_editor/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:27:00.623731 construct-editor-0.1.2/construct_editor/wx_widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-09 11:26:46.000000 construct-editor-0.1.2/construct_editor/wx_widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25380 2023-05-09 11:26:46.000000 construct-editor-0.1.2/construct_editor/wx_widgets/wx_construct_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9905 2023-05-09 11:26:46.000000 construct-editor-0.1.2/construct_editor/wx_widgets/wx_construct_hex_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-05-09 11:26:46.000000 construct-editor-0.1.2/construct_editor/wx_widgets/wx_context_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-05-09 11:26:46.000000 construct-editor-0.1.2/construct_editor/wx_widgets/wx_exception_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)    44578 2023-05-09 11:26:46.000000 construct-editor-0.1.2/construct_editor/wx_widgets/wx_hex_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)    15722 2023-05-09 11:26:46.000000 construct-editor-0.1.2/construct_editor/wx_widgets/wx_obj_view.py
--rw-r--r--   0 runner    (1001) docker     (123)    20170 2023-05-09 11:26:46.000000 construct-editor-0.1.2/construct_editor/wx_widgets/wx_python_code_editor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:27:00.619730 construct-editor-0.1.2/construct_editor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-05-09 11:27:00.000000 construct-editor-0.1.2/construct_editor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-05-09 11:27:00.000000 construct-editor-0.1.2/construct_editor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 11:27:00.000000 construct-editor-0.1.2/construct_editor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-09 11:27:00.000000 construct-editor-0.1.2/construct_editor.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-09 11:27:00.000000 construct-editor-0.1.2/construct_editor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-09 11:27:00.000000 construct-editor-0.1.2/construct_editor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 11:27:00.623731 construct-editor-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-09 11:26:46.000000 construct-editor-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:56:59.008777 construct-editor-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-01 07:56:45.000000 construct-editor-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-06-01 07:56:59.008777 construct-editor-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-06-01 07:56:45.000000 construct-editor-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:56:59.000776 construct-editor-0.1.3/construct_editor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 07:56:45.000000 construct-editor-0.1.3/construct_editor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:56:59.004777 construct-editor-0.1.3/construct_editor/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-01 07:56:45.000000 construct-editor-0.1.3/construct_editor/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-01 07:56:45.000000 construct-editor-0.1.3/construct_editor/core/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5031 2023-06-01 07:56:45.000000 construct-editor-0.1.3/construct_editor/core/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12727 2023-06-01 07:56:45.000000 construct-editor-0.1.3/construct_editor/core/construct_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-06-01 07:56:45.000000 construct-editor-0.1.3/construct_editor/core/context_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-06-01 07:56:45.000000 construct-editor-0.1.3/construct_editor/core/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63127 2023-06-01 07:56:45.000000 construct-editor-0.1.3/construct_editor/core/entries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6068 2023-06-01 07:56:45.000000 construct-editor-0.1.3/construct_editor/core/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-06-01 07:56:45.000000 construct-editor-0.1.3/construct_editor/core/preprocessor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:56:59.008777 construct-editor-0.1.3/construct_editor/gallery/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-01 07:56:45.000000 construct-editor-0.1.3/construct_editor/gallery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-06-01 07:56:45.000000 construct-editor-0.1.3/construct_editor/gallery/example_cmd_resp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27072 2023-06-01 07:56:45.000000 construct-editor-0.1.3/construct_editor/gallery/example_ipstack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7829 2023-06-01 07:56:45.000000 construct-editor-0.1.3/construct_editor/gallery/example_pe32coff.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-01 07:56:45.000000 construct-editor-0.1.3/construct_editor/gallery/test_aligned.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-06-01 07:56:45.000000 construct-editor-0.1.3/construct_editor/gallery/test_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-01 07:56:45.000000 construct-editor-0.1.3/construct_editor/gallery/test_bits_swapped_bitwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-01 07:56:45.000000 construct-editor-0.1.3/construct_editor/gallery/test_bitwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-01 07:56:45.000000 construct-editor-0.1.3/construct_editor/gallery/test_bytes_greedybytes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-01 07:56:45.000000 construct-editor-0.1.3/construct_editor/gallery/test_checksum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-06-01 07:56:45.000000 construct-editor-0.1.3/construct_editor/gallery/test_compressed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-01 07:56:45.000000 construct-editor-0.1.3/construct_editor/gallery/test_computed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-01 07:56:45.000000 construct-editor-0.1.3/construct_editor/gallery/test_const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-01 07:56:45.000000 construct-editor-0.1.3/construct_editor/gallery/test_dataclass_bit_struct.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-01 07:56:45.000000 construct-editor-0.1.3/construct_editor/gallery/test_dataclass_struct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-01 07:56:45.000000 construct-editor-0.1.3/construct_editor/gallery/test_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-01 07:56:45.000000 construct-editor-0.1.3/construct_editor/gallery/test_fixedsized.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-01 07:56:45.000000 construct-editor-0.1.3/construct_editor/gallery/test_flag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-06-01 07:56:45.000000 construct-editor-0.1.3/construct_editor/gallery/test_flagsenum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-01 07:56:45.000000 construct-editor-0.1.3/construct_editor/gallery/test_focusedseq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-01 07:56:45.000000 construct-editor-0.1.3/construct_editor/gallery/test_greedyrange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-01 07:56:45.000000 construct-editor-0.1.3/construct_editor/gallery/test_ifthenelse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-01 07:56:45.000000 construct-editor-0.1.3/construct_editor/gallery/test_ifthenelse_nested_switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-01 07:56:45.000000 construct-editor-0.1.3/construct_editor/gallery/test_nullstripped.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-01 07:56:45.000000 construct-editor-0.1.3/construct_editor/gallery/test_nullterminated.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-01 07:56:45.000000 construct-editor-0.1.3/construct_editor/gallery/test_padded.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-01 07:56:45.000000 construct-editor-0.1.3/construct_editor/gallery/test_padded_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-01 07:56:45.000000 construct-editor-0.1.3/construct_editor/gallery/test_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-01 07:56:45.000000 construct-editor-0.1.3/construct_editor/gallery/test_pointer_peek_seek_tell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-06-01 07:56:45.000000 construct-editor-0.1.3/construct_editor/gallery/test_renamed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-01 07:56:45.000000 construct-editor-0.1.3/construct_editor/gallery/test_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-06-01 07:56:45.000000 construct-editor-0.1.3/construct_editor/gallery/test_select_complex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-06-01 07:56:45.000000 construct-editor-0.1.3/construct_editor/gallery/test_stringencodded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-06-01 07:56:45.000000 construct-editor-0.1.3/construct_editor/gallery/test_switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-06-01 07:56:45.000000 construct-editor-0.1.3/construct_editor/gallery/test_switch_dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-06-01 07:56:45.000000 construct-editor-0.1.3/construct_editor/gallery/test_tenum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-06-01 07:56:45.000000 construct-editor-0.1.3/construct_editor/gallery/test_tflagsenum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-01 07:56:45.000000 construct-editor-0.1.3/construct_editor/gallery/test_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20479 2023-06-01 07:56:45.000000 construct-editor-0.1.3/construct_editor/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 07:56:45.000000 construct-editor-0.1.3/construct_editor/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-01 07:56:45.000000 construct-editor-0.1.3/construct_editor/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:56:59.008777 construct-editor-0.1.3/construct_editor/wx_widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-01 07:56:45.000000 construct-editor-0.1.3/construct_editor/wx_widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25380 2023-06-01 07:56:45.000000 construct-editor-0.1.3/construct_editor/wx_widgets/wx_construct_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9905 2023-06-01 07:56:45.000000 construct-editor-0.1.3/construct_editor/wx_widgets/wx_construct_hex_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-06-01 07:56:45.000000 construct-editor-0.1.3/construct_editor/wx_widgets/wx_context_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-06-01 07:56:45.000000 construct-editor-0.1.3/construct_editor/wx_widgets/wx_exception_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44578 2023-06-01 07:56:45.000000 construct-editor-0.1.3/construct_editor/wx_widgets/wx_hex_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15722 2023-06-01 07:56:45.000000 construct-editor-0.1.3/construct_editor/wx_widgets/wx_obj_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20170 2023-06-01 07:56:45.000000 construct-editor-0.1.3/construct_editor/wx_widgets/wx_python_code_editor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:56:59.004777 construct-editor-0.1.3/construct_editor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-06-01 07:56:58.000000 construct-editor-0.1.3/construct_editor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-06-01 07:56:58.000000 construct-editor-0.1.3/construct_editor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 07:56:58.000000 construct-editor-0.1.3/construct_editor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-01 07:56:58.000000 construct-editor-0.1.3/construct_editor.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-01 07:56:58.000000 construct-editor-0.1.3/construct_editor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-01 07:56:58.000000 construct-editor-0.1.3/construct_editor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 07:56:59.008777 construct-editor-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-06-01 07:56:45.000000 construct-editor-0.1.3/setup.py
```

### Comparing `construct-editor-0.1.2/LICENSE` & `construct-editor-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.2/PKG-INFO` & `construct-editor-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: construct-editor
-Version: 0.1.2
+Version: 0.1.3
 Summary: GUI (based on wxPython) for 'construct', which is a powerful declarative and symmetrical parser and builder for binary data.
 Home-page: https://github.com/timrid/construct-editor
 Author: Tim Riddermann
 License: MIT
 Keywords: gui,wx,wxpython,widget,binary,editorconstruct,kaitai,declarative,data structure,struct,binary,symmetric,parser,builder,parsing,building,pack,unpack,packer,unpacker,bitstring,bytestring,bitstruct
 Platform: Windows
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Construct Editor
```

### Comparing `construct-editor-0.1.2/README.md` & `construct-editor-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.2/construct_editor/core/callbacks.py` & `construct-editor-0.1.3/construct_editor/core/callbacks.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.2/construct_editor/core/commands.py` & `construct-editor-0.1.3/construct_editor/core/commands.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.2/construct_editor/core/construct_editor.py` & `construct-editor-0.1.3/construct_editor/core/construct_editor.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.2/construct_editor/core/context_menu.py` & `construct-editor-0.1.3/construct_editor/core/context_menu.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.2/construct_editor/core/custom.py` & `construct-editor-0.1.3/construct_editor/core/custom.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.2/construct_editor/core/entries.py` & `construct-editor-0.1.3/construct_editor/core/entries.py`

 * *Files 2% similar despite different names*

```diff
@@ -1707,14 +1707,18 @@
                 new_obj[item.name] = True
             else:
                 new_obj[item.name] = False
         return new_obj
 
 
 # EntryTEnum ##########################################################################################################
+def get_enum_name(e: cst.EnumBase):
+    return f"{e.__class__.__name__}.{e.name}"
+
+
 class EntryTEnum(EntrySubconstruct):
     construct: "cst.TEnum[Any]"
 
     def __init__(
         self,
         model: "model.ConstructEditorModel",
         parent: Optional["EntryConstruct"],
@@ -1727,34 +1731,37 @@
     @property
     def typ_str(self) -> str:
         return super().typ_str + " as Enum"
 
     @property
     def obj_str(self) -> str:
         try:
-            return f"{int_to_str(self.model.integer_format, int(self.obj.value))} ({str(self.obj)})"
+            obj: cst.EnumBase = self.obj
+            return f"{int_to_str(self.model.integer_format, int(obj.value))} ({get_enum_name(obj)})"
         except Exception:
             return str(self.obj)
 
     @property
     def obj_view_settings(self) -> ObjViewSettings:
         return ObjViewSettings_Enum(self)
 
     def get_enum_items(self) -> t.List[EnumItem]:
         """Get items to show in the ComboBox"""
         items: t.List[EnumItem] = []
         enum_type: t.Type[cst.EnumBase] = self.construct.enum_type
         for e in enum_type:
-            items.append(EnumItem(name=str(e), value=e.value))
+            items.append(
+                EnumItem(name=get_enum_name(e), value=e.value)
+            )
         return items
 
     def get_enum_item_from_obj(self) -> EnumItem:
         """Get items to select in the ComboBox"""
         obj: cst.EnumBase = self.obj
-        return EnumItem(name=str(obj), value=obj.value)
+        return EnumItem(name=get_enum_name(obj), value=obj.value)
 
     def conv_str_to_obj(self, s: str) -> Any:
         """Convert string (enum name or integer value) to object"""
         enum_type: t.Type[cst.EnumBase] = self.construct.enum_type
         try:
             try:
                 new_obj = enum_type[s]
```

### Comparing `construct-editor-0.1.2/construct_editor/core/model.py` & `construct-editor-0.1.3/construct_editor/core/model.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.2/construct_editor/core/preprocessor.py` & `construct-editor-0.1.3/construct_editor/core/preprocessor.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.2/construct_editor/gallery/example_cmd_resp.py` & `construct-editor-0.1.3/construct_editor/gallery/example_cmd_resp.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.2/construct_editor/gallery/example_ipstack.py` & `construct-editor-0.1.3/construct_editor/gallery/example_ipstack.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.2/construct_editor/gallery/example_pe32coff.py` & `construct-editor-0.1.3/construct_editor/gallery/example_pe32coff.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.2/construct_editor/gallery/test_array.py` & `construct-editor-0.1.3/construct_editor/gallery/test_array.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.2/construct_editor/gallery/test_checksum.py` & `construct-editor-0.1.3/construct_editor/gallery/test_checksum.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.2/construct_editor/gallery/test_compressed.py` & `construct-editor-0.1.3/construct_editor/gallery/test_compressed.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.2/construct_editor/gallery/test_computed.py` & `construct-editor-0.1.3/construct_editor/gallery/test_computed.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.2/construct_editor/gallery/test_const.py` & `construct-editor-0.1.3/construct_editor/gallery/test_const.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.2/construct_editor/gallery/test_dataclass_bit_struct.py` & `construct-editor-0.1.3/construct_editor/gallery/test_dataclass_bit_struct.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.2/construct_editor/gallery/test_dataclass_struct.py` & `construct-editor-0.1.3/construct_editor/gallery/test_dataclass_struct.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.2/construct_editor/gallery/test_enum.py` & `construct-editor-0.1.3/construct_editor/gallery/test_enum.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.2/construct_editor/gallery/test_fixedsized.py` & `construct-editor-0.1.3/construct_editor/gallery/test_fixedsized.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.2/construct_editor/gallery/test_flagsenum.py` & `construct-editor-0.1.3/construct_editor/gallery/test_flagsenum.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.2/construct_editor/gallery/test_focusedseq.py` & `construct-editor-0.1.3/construct_editor/gallery/test_focusedseq.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.2/construct_editor/gallery/test_greedyrange.py` & `construct-editor-0.1.3/construct_editor/gallery/test_greedyrange.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.2/construct_editor/gallery/test_ifthenelse.py` & `construct-editor-0.1.3/construct_editor/gallery/test_ifthenelse.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.2/construct_editor/gallery/test_ifthenelse_nested_switch.py` & `construct-editor-0.1.3/construct_editor/gallery/test_ifthenelse_nested_switch.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.2/construct_editor/gallery/test_pointer_peek_seek_tell.py` & `construct-editor-0.1.3/construct_editor/gallery/test_pointer_peek_seek_tell.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.2/construct_editor/gallery/test_renamed.py` & `construct-editor-0.1.3/construct_editor/gallery/test_renamed.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.2/construct_editor/gallery/test_select.py` & `construct-editor-0.1.3/construct_editor/gallery/test_select.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.2/construct_editor/gallery/test_select_complex.py` & `construct-editor-0.1.3/construct_editor/gallery/test_select_complex.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.2/construct_editor/gallery/test_stringencodded.py` & `construct-editor-0.1.3/construct_editor/gallery/test_stringencodded.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.2/construct_editor/gallery/test_switch.py` & `construct-editor-0.1.3/construct_editor/gallery/test_switch.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.2/construct_editor/gallery/test_switch_dataclass.py` & `construct-editor-0.1.3/construct_editor/gallery/test_switch_dataclass.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.2/construct_editor/gallery/test_tenum.py` & `construct-editor-0.1.3/construct_editor/gallery/test_tenum.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.2/construct_editor/gallery/test_tflagsenum.py` & `construct-editor-0.1.3/construct_editor/gallery/test_tflagsenum.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.2/construct_editor/gallery/test_timestamp.py` & `construct-editor-0.1.3/construct_editor/gallery/test_timestamp.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.2/construct_editor/main.py` & `construct-editor-0.1.3/construct_editor/main.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.2/construct_editor/wx_widgets/wx_construct_editor.py` & `construct-editor-0.1.3/construct_editor/wx_widgets/wx_construct_editor.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.2/construct_editor/wx_widgets/wx_construct_hex_editor.py` & `construct-editor-0.1.3/construct_editor/wx_widgets/wx_construct_hex_editor.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.2/construct_editor/wx_widgets/wx_context_menu.py` & `construct-editor-0.1.3/construct_editor/wx_widgets/wx_context_menu.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.2/construct_editor/wx_widgets/wx_exception_dialog.py` & `construct-editor-0.1.3/construct_editor/wx_widgets/wx_exception_dialog.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.2/construct_editor/wx_widgets/wx_hex_editor.py` & `construct-editor-0.1.3/construct_editor/wx_widgets/wx_hex_editor.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.2/construct_editor/wx_widgets/wx_obj_view.py` & `construct-editor-0.1.3/construct_editor/wx_widgets/wx_obj_view.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.2/construct_editor/wx_widgets/wx_python_code_editor.py` & `construct-editor-0.1.3/construct_editor/wx_widgets/wx_python_code_editor.py`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.2/construct_editor.egg-info/PKG-INFO` & `construct-editor-0.1.3/construct_editor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: construct-editor
-Version: 0.1.2
+Version: 0.1.3
 Summary: GUI (based on wxPython) for 'construct', which is a powerful declarative and symmetrical parser and builder for binary data.
 Home-page: https://github.com/timrid/construct-editor
 Author: Tim Riddermann
 License: MIT
 Keywords: gui,wx,wxpython,widget,binary,editorconstruct,kaitai,declarative,data structure,struct,binary,symmetric,parser,builder,parsing,building,pack,unpack,packer,unpacker,bitstring,bytestring,bitstruct
 Platform: Windows
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Construct Editor
```

### Comparing `construct-editor-0.1.2/construct_editor.egg-info/SOURCES.txt` & `construct-editor-0.1.3/construct_editor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `construct-editor-0.1.2/setup.py` & `construct-editor-0.1.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,11 +65,12 @@
     classifiers=[
         "Development Status :: 3 - Alpha",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: CPython",
         "Typing :: Typed",
     ],
 )
```

