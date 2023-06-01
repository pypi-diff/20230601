# Comparing `tmp/mezcla-1.3.6.tar.gz` & `tmp/mezcla-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mezcla-1.3.6.tar", last modified: Tue Apr 25 21:57:50 2023, max compression
+gzip compressed data, was "mezcla-1.3.7.tar", last modified: Thu Jun  1 21:41:51 2023, max compression
```

## Comparing `mezcla-1.3.6.tar` & `mezcla-1.3.7.tar`

### file list

```diff
@@ -1,152 +1,152 @@
--rw-r--r--   0        0        0      542 2022-12-14 05:41:54.725724 mezcla-1.3.6/.coveragerc
--rw-r--r--   0        0        0     1660 2023-04-03 16:37:03.715727 mezcla-1.3.6/.github/workflows/tests.yml
--rw-r--r--   0        0        0     1639 2023-04-03 16:37:03.715727 mezcla-1.3.6/.gitignore
--rw-r--r--   0        0        0     7370 2022-06-03 04:33:57.175684 mezcla-1.3.6/LICENSE.txt
--rw-r--r--   0        0        0      777 2022-06-03 04:33:57.175684 mezcla-1.3.6/README.txt
--rw-r--r--   0        0        0       84 2022-10-25 19:04:34.956398 mezcla-1.3.6/TODO.txt
--rwxr-xr-x   0        0        0     1927 2023-04-25 21:52:34.589331 mezcla-1.3.6/mezcla/__init__.py
--rwxr-xr-x   0        0        0    10860 2022-06-02 23:46:45.000000 mezcla-1.3.6/mezcla/analyze_tfidf.py
--rwxr-xr-x   0        0        0    13029 2022-12-14 05:41:54.725724 mezcla-1.3.6/mezcla/audio.py
--rwxr-xr-x   0        0        0    16055 2022-06-16 07:59:25.588655 mezcla-1.3.6/mezcla/bert_multi_classification.py
--rwxr-xr-x   0        0        0    25702 2022-06-03 05:22:44.104859 mezcla-1.3.6/mezcla/bert_text_classification.py
--rwxr-xr-x   0        0        0     7625 2022-12-14 05:41:54.725724 mezcla-1.3.6/mezcla/bing_search.py
--rwxr-xr-x   0        0        0     8925 2022-02-01 06:41:33.000000 mezcla-1.3.6/mezcla/check_html_javascript.py
--rwxr-xr-x   0        0        0    14338 2022-07-16 02:12:42.988675 mezcla-1.3.6/mezcla/compute_tfidf.py
--rwxr-xr-x   0        0        0    22279 2023-04-03 16:37:03.715727 mezcla-1.3.6/mezcla/cut.py
--rwxr-xr-x   0        0        0     4279 2022-11-25 22:51:38.472697 mezcla-1.3.6/mezcla/data_utils.py
--rwxr-xr-x   0        0        0    45580 2023-04-25 17:58:45.655571 mezcla-1.3.6/mezcla/debug.py
--rw-r--r--   0        0        0    25047 2022-12-14 05:41:54.729723 mezcla-1.3.6/mezcla/docs/audio_uml.svg
--rwxr-xr-x   0        0        0        0 2022-11-11 01:58:12.573316 mezcla-1.3.6/mezcla/examples/__init__.py
--rwxr-xr-x   0        0        0    12834 2021-10-26 07:06:23.000000 mezcla-1.3.6/mezcla/examples/alt_sklearn_plot_precision_recall.py
--rwxr-xr-x   0        0        0     3608 2022-06-16 07:59:25.588655 mezcla-1.3.6/mezcla/examples/brownlee_ml_metrics.py
--rwxr-xr-x   0        0        0     2419 2022-11-01 22:06:48.768053 mezcla-1.3.6/mezcla/examples/consume_all_memory.py
--rwxr-xr-x   0        0        0     5008 2022-11-11 01:52:38.317145 mezcla-1.3.6/mezcla/examples/download_user_gist.py
--rwxr-xr-x   0        0        0     6477 2022-06-09 02:23:07.119975 mezcla-1.3.6/mezcla/examples/dump_checkpoints.py
--rw-r--r--   0        0        0     2738 2022-02-20 02:05:16.229030 mezcla-1.3.6/mezcla/examples/encoded-iris.csv
--rwxr-xr-x   0        0        0     8779 2022-02-21 09:16:29.886156 mezcla-1.3.6/mezcla/examples/feature_importance.py
--rw-r--r--   0        0        0    40044 2021-05-07 02:08:15.000000 mezcla-1.3.6/mezcla/examples/fuzzy-testing-1-2-3.wav
--rwxr-xr-x   0        0        0     3338 2023-01-27 00:16:57.067013 mezcla-1.3.6/mezcla/examples/hugging_face_speechrec.py
--rwxr-xr-x   0        0        0     3922 2023-04-03 16:37:03.715727 mezcla-1.3.6/mezcla/examples/hugging_face_translation.py
--rwxr-xr-x   0        0        0    10347 2022-09-25 01:54:34.121735 mezcla-1.3.6/mezcla/examples/inspect_checkpoint.py
--rw-r--r--   0        0        0     4607 2020-04-12 09:44:23.000000 mezcla-1.3.6/mezcla/examples/iris.csv
--rw-r--r--   0        0        0    23345 2020-05-01 07:18:00.000000 mezcla-1.3.6/mezcla/examples/pima-indians-diabetes.csv
--rwxr-xr-x   0        0        0     8279 2022-06-09 02:26:58.076477 mezcla-1.3.6/mezcla/examples/plot_forest_importances.py
--rwxr-xr-x   0        0        0    12989 2021-10-16 04:41:00.000000 mezcla-1.3.6/mezcla/examples/sklearn_plot_precision_recall.py
--rwxr-xr-x   0        0        0     1467 2023-04-03 16:37:03.715727 mezcla-1.3.6/mezcla/examples/template.py
--rwxr-xr-x   0        0        0     3155 2022-11-01 21:38:37.296840 mezcla-1.3.6/mezcla/examples/tensorflow_matrix_multiply.py
--rwxr-xr-x   0        0        0     3607 2022-10-26 21:42:12.776794 mezcla-1.3.6/mezcla/examples/tracemalloc_display.py
--rwxr-xr-x   0        0        0     4031 2023-04-03 16:37:03.719727 mezcla-1.3.6/mezcla/extract_document_text.py
--rwxr-xr-x   0        0        0     5879 2022-06-30 00:48:39.136921 mezcla-1.3.6/mezcla/file_utils.py
--rwxr-xr-x   0        0        0     3071 2022-03-01 08:46:55.000000 mezcla-1.3.6/mezcla/filter_random.py
--rwxr-xr-x   0        0        0     2998 2021-09-30 12:02:57.000000 mezcla-1.3.6/mezcla/format_profile.py
--rwxr-xr-x   0        0        0    32894 2022-06-02 07:16:58.000000 mezcla-1.3.6/mezcla/gensim_test.py
--rwxr-xr-x   0        0        0    32128 2023-04-25 17:58:45.659572 mezcla-1.3.6/mezcla/glue_helpers.py
--rwxr-xr-x   0        0        0    32492 2022-12-14 05:41:54.733723 mezcla-1.3.6/mezcla/html_utils.py
--rwxr-xr-x   0        0        0     4708 2021-09-30 12:02:57.000000 mezcla-1.3.6/mezcla/kenlm_example.py
--rwxr-xr-x   0        0        0    17916 2022-12-14 05:41:54.733723 mezcla-1.3.6/mezcla/keras_param_search.py
--rwxr-xr-x   0        0        0    41468 2023-04-03 16:37:03.719727 mezcla-1.3.6/mezcla/main.py
--rwxr-xr-x   0        0        0     9131 2022-12-14 05:03:22.477527 mezcla-1.3.6/mezcla/merge_files.py
--rwxr-xr-x   0        0        0    11717 2022-09-05 00:03:22.272746 mezcla-1.3.6/mezcla/merge_notes.py
--rwxr-xr-x   0        0        0    11640 2022-12-14 05:41:54.733723 mezcla-1.3.6/mezcla/misc_utils.py
--rwxr-xr-x   0        0        0     9507 2023-04-25 17:58:45.659572 mezcla-1.3.6/mezcla/my_regex.py
--rwxr-xr-x   0        0        0    13776 2023-04-25 18:02:39.556316 mezcla-1.3.6/mezcla/ngram_tfidf.py
--rwxr-xr-x   0        0        0      183 2022-04-08 02:22:06.000000 mezcla-1.3.6/mezcla/os_utils.py
--rwxr-xr-x   0        0        0    31436 2022-12-14 05:41:54.733723 mezcla-1.3.6/mezcla/pandas_sklearn.py
--rwxr-xr-x   0        0        0      828 2022-12-14 05:01:09.014808 mezcla-1.3.6/mezcla/plot_utils.py
--rwxr-xr-x   0        0        0     7053 2022-11-01 23:07:50.308605 mezcla-1.3.6/mezcla/randomize_lines.py
--rwxr-xr-x   0        0        0     7012 2022-11-25 22:51:38.476697 mezcla-1.3.6/mezcla/rgb_color_name.py
--rwxr-xr-x   0        0        0    40529 2022-03-01 08:46:55.000000 mezcla-1.3.6/mezcla/run_albert_classifier.py
--rwxr-xr-x   0        0        0    39613 2022-06-16 07:59:25.592656 mezcla-1.3.6/mezcla/run_bert_classifier.py
--rwxr-xr-x   0        0        0    17400 2022-10-25 19:16:24.448196 mezcla-1.3.6/mezcla/show_bert_representation.py
--rwxr-xr-x   0        0        0     1508 2021-09-30 12:02:57.000000 mezcla-1.3.6/mezcla/simple_main_example.py
--rwxr-xr-x   0        0        0    19931 2023-04-03 16:37:03.719727 mezcla-1.3.6/mezcla/spacy_nlp.py
--rwxr-xr-x   0        0        0     3011 2023-04-25 17:58:45.659572 mezcla-1.3.6/mezcla/spell.py
--rwxr-xr-x   0        0        0     2416 2021-09-30 11:10:06.000000 mezcla-1.3.6/mezcla/sys_version_info_hack.py
--rw-r--r--   0        0        0    49992 2023-04-25 17:58:45.659572 mezcla-1.3.6/mezcla/system.py
--rwxr-xr-x   0        0        0    45776 2022-07-11 18:17:58.306115 mezcla-1.3.6/mezcla/temp/simple_batspp.py
--rwxr-xr-x   0        0        0     5763 2023-04-25 17:58:45.659572 mezcla-1.3.6/mezcla/template.py
--rw-r--r--   0        0        0     7370 2022-06-03 04:33:57.199684 mezcla-1.3.6/mezcla/tests/LICENSE.txt
--rw-r--r--   0        0        0      722 2022-07-11 03:52:31.719683 mezcla-1.3.6/mezcla/tests/adhoc-tests.batspp
--rwxr-xr-x   0        0        0     3905 2022-06-03 04:33:57.199684 mezcla-1.3.6/mezcla/tests/misc_doctests.py
--rw-r--r--   0        0        0      113 2022-12-14 05:41:54.733723 mezcla-1.3.6/mezcla/tests/resources/cars-fields-2-3-4.txt
--rw-r--r--   0        0        0      810 2022-12-14 05:41:54.733723 mezcla-1.3.6/mezcla/tests/resources/cars-len-3.txt
--rw-r--r--   0        0        0      659 2022-12-14 05:41:54.733723 mezcla-1.3.6/mezcla/tests/resources/cars.csv
--rw-r--r--   0        0        0      755 2022-12-14 05:41:54.733723 mezcla-1.3.6/mezcla/tests/resources/cars.tsv
--rw-r--r--   0        0        0      603 2022-12-14 05:41:54.733723 mezcla-1.3.6/mezcla/tests/resources/example_text.txt
--rw-r--r--   0        0        0     2573 2022-12-14 05:41:54.737723 mezcla-1.3.6/mezcla/tests/resources/example_text_tags.txt
--rw-r--r--   0        0        0     2440 2022-12-14 05:41:54.737723 mezcla-1.3.6/mezcla/tests/resources/iris_output.txt
--rw-r--r--   0        0        0     1152 2022-12-14 05:41:54.737723 mezcla-1.3.6/mezcla/tests/resources/simple-window-dimensions.html
--rw-r--r--   0        0        0     5577 2022-12-14 05:41:54.737723 mezcla-1.3.6/mezcla/tests/resources/spanish-accents.docx
--rw-r--r--   0        0        0    12530 2022-12-14 05:41:54.737723 mezcla-1.3.6/mezcla/tests/resources/spanish-accents.pdf
--rw-r--r--   0        0        0      141 2022-12-14 05:41:54.737723 mezcla-1.3.6/mezcla/tests/resources/spanish-accents.txt
--rw-r--r--   0        0        0       65 2022-12-14 05:41:54.737723 mezcla-1.3.6/mezcla/tests/resources/word-POS.freq
--rw-r--r--   0        0        0      254 2023-04-25 17:58:45.675574 mezcla-1.3.6/mezcla/tests/simple-script-tests.test
--rwxr-xr-x   0        0        0     4296 2022-12-14 05:41:54.737723 mezcla-1.3.6/mezcla/tests/template.py
--rwxr-xr-x   0        0        0     4295 2022-12-14 05:41:54.737723 mezcla-1.3.6/mezcla/tests/test_audio.py
--rwxr-xr-x   0        0        0      969 2022-12-14 07:11:50.877858 mezcla-1.3.6/mezcla/tests/test_bert_multi_classification.py
--rwxr-xr-x   0        0        0      834 2022-12-14 07:11:50.877858 mezcla-1.3.6/mezcla/tests/test_bing_search.py
--rwxr-xr-x   0        0        0     1974 2022-12-14 07:11:50.877858 mezcla-1.3.6/mezcla/tests/test_compute_tfidf.py
--rwxr-xr-x   0        0        0     2932 2022-12-14 07:11:50.877858 mezcla-1.3.6/mezcla/tests/test_cut.py
--rwxr-xr-x   0        0        0     2068 2022-12-14 07:11:50.877858 mezcla-1.3.6/mezcla/tests/test_data_utils.py
--rwxr-xr-x   0        0        0    13297 2022-12-14 05:41:54.737723 mezcla-1.3.6/mezcla/tests/test_debug.py
--rwxr-xr-x   0        0        0     1030 2022-12-14 07:11:50.877858 mezcla-1.3.6/mezcla/tests/test_extract_document_text.py
--rwxr-xr-x   0        0        0     4290 2022-12-14 05:41:54.737723 mezcla-1.3.6/mezcla/tests/test_file_utils.py
--rwxr-xr-x   0        0        0     2868 2022-12-14 05:41:54.737723 mezcla-1.3.6/mezcla/tests/test_filter_random.py
--rwxr-xr-x   0        0        0     2562 2022-12-14 05:41:54.737723 mezcla-1.3.6/mezcla/tests/test_gensim_test.py
--rwxr-xr-x   0        0        0    15122 2022-12-14 05:41:54.737723 mezcla-1.3.6/mezcla/tests/test_glue_helpers.py
--rwxr-xr-x   0        0        0    13008 2022-12-14 05:41:54.737723 mezcla-1.3.6/mezcla/tests/test_html_utils.py
--rwxr-xr-x   0        0        0      892 2022-12-14 07:11:50.877858 mezcla-1.3.6/mezcla/tests/test_kenlm_example.py
--rwxr-xr-x   0        0        0     1683 2022-12-14 07:11:50.877858 mezcla-1.3.6/mezcla/tests/test_keras_param_search.py
--rwxr-xr-x   0        0        0     8809 2022-12-14 05:41:54.741723 mezcla-1.3.6/mezcla/tests/test_main.py
--rwxr-xr-x   0        0        0     2313 2022-12-14 07:11:50.877858 mezcla-1.3.6/mezcla/tests/test_merge_files.py
--rwxr-xr-x   0        0        0     1291 2022-12-14 07:11:50.881858 mezcla-1.3.6/mezcla/tests/test_merge_notes.py
--rwxr-xr-x   0        0        0     6565 2022-12-14 05:41:54.741723 mezcla-1.3.6/mezcla/tests/test_misc_utils.py
--rwxr-xr-x   0        0        0     2882 2022-12-14 05:41:54.741723 mezcla-1.3.6/mezcla/tests/test_my_regex.py
--rwxr-xr-x   0        0        0      916 2022-12-14 07:11:50.881858 mezcla-1.3.6/mezcla/tests/test_ngram_tfidf.py
--rwxr-xr-x   0        0        0      819 2022-12-14 07:11:50.881858 mezcla-1.3.6/mezcla/tests/test_os_utils.py
--rwxr-xr-x   0        0        0     8095 2022-12-14 07:11:50.881858 mezcla-1.3.6/mezcla/tests/test_pandas_sklearn.py
--rwxr-xr-x   0        0        0      829 2022-12-14 07:11:50.881858 mezcla-1.3.6/mezcla/tests/test_plot_utils.py
--rwxr-xr-x   0        0        0      854 2022-12-14 07:11:50.881858 mezcla-1.3.6/mezcla/tests/test_randomize_lines.py
--rwxr-xr-x   0        0        0     2657 2022-12-14 05:41:54.741723 mezcla-1.3.6/mezcla/tests/test_rgb_color_name.py
--rwxr-xr-x   0        0        0      895 2022-12-14 07:11:50.881858 mezcla-1.3.6/mezcla/tests/test_run_albert_classifier.py
--rwxr-xr-x   0        0        0      930 2022-12-14 07:11:50.881858 mezcla-1.3.6/mezcla/tests/test_run_bert_classifier.py
--rwxr-xr-x   0        0        0     1602 2022-12-14 07:11:50.881858 mezcla-1.3.6/mezcla/tests/test_show_bert_representation.py
--rwxr-xr-x   0        0        0      878 2022-12-14 07:11:50.881858 mezcla-1.3.6/mezcla/tests/test_simple_main_example.py
--rwxr-xr-x   0        0        0     2060 2022-12-14 07:11:50.881858 mezcla-1.3.6/mezcla/tests/test_spacy_nlp.py
--rwxr-xr-x   0        0        0      882 2022-12-14 07:11:50.881858 mezcla-1.3.6/mezcla/tests/test_sys_version_info_hack.py
--rwxr-xr-x   0        0        0    33090 2022-12-14 05:41:54.741723 mezcla-1.3.6/mezcla/tests/test_system.py
--rwxr-xr-x   0        0        0     1769 2022-12-14 05:41:54.741723 mezcla-1.3.6/mezcla/tests/test_template.py
--rwxr-xr-x   0        0        0     3651 2022-12-14 05:41:54.741723 mezcla-1.3.6/mezcla/tests/test_text_categorizer.py
--rwxr-xr-x   0        0        0     7027 2022-12-14 07:11:50.881858 mezcla-1.3.6/mezcla/tests/test_text_processing.py
--rwxr-xr-x   0        0        0     7362 2022-12-14 05:41:54.745723 mezcla-1.3.6/mezcla/tests/test_text_utils.py
--rwxr-xr-x   0        0        0    21785 2022-12-14 05:41:54.745723 mezcla-1.3.6/mezcla/tests/test_tpo_common.py
--rwxr-xr-x   0        0        0      715 2022-12-14 07:11:50.881858 mezcla-1.3.6/mezcla/tests/test_train_language_model.py
--rwxr-xr-x   0        0        0      725 2022-12-14 07:11:50.881858 mezcla-1.3.6/mezcla/tests/test_train_text_categorizer.py
--rwxr-xr-x   0        0        0      686 2022-12-14 07:11:50.881858 mezcla-1.3.6/mezcla/tests/test_transpose_data.py
--rwxr-xr-x   0        0        0     2859 2022-12-14 05:41:54.745723 mezcla-1.3.6/mezcla/tests/test_xml_utils.py
--rw-r--r--   0        0        0      676 2022-12-14 05:41:54.745723 mezcla-1.3.6/mezcla/tests/tfidf/test_corpus.py
--rw-r--r--   0        0        0      697 2022-12-14 05:41:54.745723 mezcla-1.3.6/mezcla/tests/tfidf/test_dockeyword.py
--rw-r--r--   0        0        0      688 2022-12-14 05:41:54.745723 mezcla-1.3.6/mezcla/tests/tfidf/test_document.py
--rw-r--r--   0        0        0      697 2022-12-14 05:41:54.745723 mezcla-1.3.6/mezcla/tests/tfidf/test_preprocess.py
--rwxr-xr-x   0        0        0    33807 2023-04-03 16:37:03.723726 mezcla-1.3.6/mezcla/text_categorizer.py
--rwxr-xr-x   0        0        0    23132 2022-12-14 07:12:36.328736 mezcla-1.3.6/mezcla/text_processing.py
--rwxr-xr-x   0        0        0    16223 2022-12-14 05:41:54.745723 mezcla-1.3.6/mezcla/text_utils.py
--rwxr-xr-x   0        0        0      375 2022-07-10 04:39:58.387124 mezcla-1.3.6/mezcla/tfidf/__init__.py
--rwxr-xr-x   0        0        0    18423 2022-07-16 02:20:12.481890 mezcla-1.3.6/mezcla/tfidf/corpus.py
--rwxr-xr-x   0        0        0     2282 2022-07-16 02:21:08.306400 mezcla-1.3.6/mezcla/tfidf/dockeyword.py
--rwxr-xr-x   0        0        0     7983 2022-07-16 02:23:27.003581 mezcla-1.3.6/mezcla/tfidf/document.py
-lrwxr-xr-x   0        0        0        0 2022-06-03 04:33:57.207684 mezcla-1.3.6/mezcla/tfidf/old-version -> /home/tomohara/python/tfidf
--rwxr-xr-x   0        0        0    16163 2023-04-25 18:35:58.058712 mezcla-1.3.6/mezcla/tfidf/preprocess.py
--rwxr-xr-x   0        0        0    59862 2022-12-14 05:41:54.749723 mezcla-1.3.6/mezcla/tpo_common.py
--rwxr-xr-x   0        0        0     5267 2022-04-12 04:31:30.000000 mezcla-1.3.6/mezcla/train_language_model.py
--rwxr-xr-x   0        0        0     5098 2021-10-22 05:45:54.000000 mezcla-1.3.6/mezcla/train_text_categorizer.py
--rwxr-xr-x   0        0        0     6778 2021-09-30 12:02:57.000000 mezcla-1.3.6/mezcla/transpose_data.py
--rw-r--r--   0        0        0    12934 2022-12-14 05:52:55.717367 mezcla-1.3.6/mezcla/unittest_wrapper.py
--rwxr-xr-x   0        0        0     3543 2022-04-12 04:50:46.000000 mezcla-1.3.6/mezcla/xml_utils.py
--rw-r--r--   0        0        0      958 2022-06-03 04:33:57.211684 mezcla-1.3.6/pyproject.toml
--rw-r--r--   0        0        0     1709 2023-04-03 16:37:03.723726 mezcla-1.3.6/requirements.txt
--rw-r--r--   0        0        0     1162 2023-04-25 21:52:34.589331 mezcla-1.3.6/setup.py
--rwxr-xr-x   0        0        0    45023 2022-07-16 02:44:46.791484 mezcla-1.3.6/temp/simple_batspp.py
--rwxr-xr-x   0        0        0      458 2022-12-14 05:41:54.749723 mezcla-1.3.6/tools/run_tests.bash
--rw-r--r--   0        0        0      567 2022-06-12 21:53:35.675247 mezcla-1.3.6/tox.ini
--rw-r--r--   0        0        0     1085 1970-01-01 00:00:00.000000 mezcla-1.3.6/PKG-INFO
+-rw-r--r--   0        0        0      542 2023-06-01 21:28:06.589424 mezcla-1.3.7/.coveragerc
+-rw-r--r--   0        0        0     1660 2023-06-01 21:33:21.261397 mezcla-1.3.7/.github/workflows/tests.yml
+-rw-r--r--   0        0        0     1639 2023-06-01 21:28:06.589424 mezcla-1.3.7/.gitignore
+-rw-r--r--   0        0        0     7370 2023-06-01 21:28:06.589424 mezcla-1.3.7/LICENSE.txt
+-rw-r--r--   0        0        0      777 2023-06-01 21:28:06.589424 mezcla-1.3.7/README.txt
+-rw-r--r--   0        0        0       84 2023-06-01 21:28:06.589424 mezcla-1.3.7/TODO.txt
+-rwxr-xr-x   0        0        0     1927 2023-06-01 21:35:43.501666 mezcla-1.3.7/mezcla/__init__.py
+-rwxr-xr-x   0        0        0    10860 2023-06-01 21:28:06.589424 mezcla-1.3.7/mezcla/analyze_tfidf.py
+-rwxr-xr-x   0        0        0    13029 2023-06-01 21:28:06.589424 mezcla-1.3.7/mezcla/audio.py
+-rwxr-xr-x   0        0        0    16055 2023-06-01 21:28:06.589424 mezcla-1.3.7/mezcla/bert_multi_classification.py
+-rwxr-xr-x   0        0        0    25702 2023-06-01 21:28:06.589424 mezcla-1.3.7/mezcla/bert_text_classification.py
+-rwxr-xr-x   0        0        0     7625 2023-06-01 21:28:06.593424 mezcla-1.3.7/mezcla/bing_search.py
+-rwxr-xr-x   0        0        0     8925 2023-06-01 21:28:06.593424 mezcla-1.3.7/mezcla/check_html_javascript.py
+-rwxr-xr-x   0        0        0    14338 2023-06-01 21:28:06.593424 mezcla-1.3.7/mezcla/compute_tfidf.py
+-rwxr-xr-x   0        0        0    22279 2023-06-01 21:28:06.593424 mezcla-1.3.7/mezcla/cut.py
+-rwxr-xr-x   0        0        0     4279 2023-06-01 21:33:21.261397 mezcla-1.3.7/mezcla/data_utils.py
+-rwxr-xr-x   0        0        0    45580 2023-06-01 21:28:06.593424 mezcla-1.3.7/mezcla/debug.py
+-rw-r--r--   0        0        0    25047 2023-06-01 21:28:06.593424 mezcla-1.3.7/mezcla/docs/audio_uml.svg
+-rwxr-xr-x   0        0        0        0 2023-06-01 21:28:06.593424 mezcla-1.3.7/mezcla/examples/__init__.py
+-rwxr-xr-x   0        0        0    12834 2023-06-01 21:28:06.593424 mezcla-1.3.7/mezcla/examples/alt_sklearn_plot_precision_recall.py
+-rwxr-xr-x   0        0        0     3608 2023-06-01 21:28:06.597424 mezcla-1.3.7/mezcla/examples/brownlee_ml_metrics.py
+-rwxr-xr-x   0        0        0     2419 2023-06-01 21:28:06.597424 mezcla-1.3.7/mezcla/examples/consume_all_memory.py
+-rwxr-xr-x   0        0        0     5008 2023-06-01 21:28:06.597424 mezcla-1.3.7/mezcla/examples/download_user_gist.py
+-rwxr-xr-x   0        0        0     6477 2023-06-01 21:28:06.597424 mezcla-1.3.7/mezcla/examples/dump_checkpoints.py
+-rw-r--r--   0        0        0     2738 2023-06-01 21:28:06.597424 mezcla-1.3.7/mezcla/examples/encoded-iris.csv
+-rwxr-xr-x   0        0        0     8779 2023-06-01 21:28:06.597424 mezcla-1.3.7/mezcla/examples/feature_importance.py
+-rw-r--r--   0        0        0    40044 2023-06-01 21:28:06.597424 mezcla-1.3.7/mezcla/examples/fuzzy-testing-1-2-3.wav
+-rwxr-xr-x   0        0        0     3338 2023-06-01 21:28:06.597424 mezcla-1.3.7/mezcla/examples/hugging_face_speechrec.py
+-rwxr-xr-x   0        0        0     3922 2023-06-01 21:28:06.597424 mezcla-1.3.7/mezcla/examples/hugging_face_translation.py
+-rwxr-xr-x   0        0        0    10347 2023-06-01 21:28:06.597424 mezcla-1.3.7/mezcla/examples/inspect_checkpoint.py
+-rw-r--r--   0        0        0     4607 2023-06-01 21:28:06.597424 mezcla-1.3.7/mezcla/examples/iris.csv
+-rw-r--r--   0        0        0    23345 2023-06-01 21:28:06.601424 mezcla-1.3.7/mezcla/examples/pima-indians-diabetes.csv
+-rwxr-xr-x   0        0        0     8279 2023-06-01 21:28:06.601424 mezcla-1.3.7/mezcla/examples/plot_forest_importances.py
+-rwxr-xr-x   0        0        0    12989 2023-06-01 21:28:06.601424 mezcla-1.3.7/mezcla/examples/sklearn_plot_precision_recall.py
+-rwxr-xr-x   0        0        0     1467 2023-06-01 21:28:06.601424 mezcla-1.3.7/mezcla/examples/template.py
+-rwxr-xr-x   0        0        0     3155 2023-06-01 21:28:06.601424 mezcla-1.3.7/mezcla/examples/tensorflow_matrix_multiply.py
+-rwxr-xr-x   0        0        0     3607 2023-06-01 21:28:06.601424 mezcla-1.3.7/mezcla/examples/tracemalloc_display.py
+-rwxr-xr-x   0        0        0     4031 2023-06-01 21:28:06.601424 mezcla-1.3.7/mezcla/extract_document_text.py
+-rwxr-xr-x   0        0        0     5879 2023-06-01 21:28:06.601424 mezcla-1.3.7/mezcla/file_utils.py
+-rwxr-xr-x   0        0        0     3071 2023-06-01 21:28:06.601424 mezcla-1.3.7/mezcla/filter_random.py
+-rwxr-xr-x   0        0        0     2998 2023-06-01 21:28:06.601424 mezcla-1.3.7/mezcla/format_profile.py
+-rwxr-xr-x   0        0        0    32894 2023-06-01 21:28:06.601424 mezcla-1.3.7/mezcla/gensim_test.py
+-rwxr-xr-x   0        0        0    32128 2023-06-01 21:28:06.601424 mezcla-1.3.7/mezcla/glue_helpers.py
+-rwxr-xr-x   0        0        0    32492 2023-06-01 21:28:06.605424 mezcla-1.3.7/mezcla/html_utils.py
+-rwxr-xr-x   0        0        0     4708 2023-06-01 21:28:06.605424 mezcla-1.3.7/mezcla/kenlm_example.py
+-rwxr-xr-x   0        0        0    17916 2023-06-01 21:28:06.605424 mezcla-1.3.7/mezcla/keras_param_search.py
+-rwxr-xr-x   0        0        0    41468 2023-06-01 21:33:21.261397 mezcla-1.3.7/mezcla/main.py
+-rwxr-xr-x   0        0        0     9131 2023-06-01 21:28:06.605424 mezcla-1.3.7/mezcla/merge_files.py
+-rwxr-xr-x   0        0        0    11717 2023-06-01 21:28:06.605424 mezcla-1.3.7/mezcla/merge_notes.py
+-rwxr-xr-x   0        0        0    11640 2023-06-01 21:33:21.261397 mezcla-1.3.7/mezcla/misc_utils.py
+-rwxr-xr-x   0        0        0     9507 2023-06-01 21:28:06.605424 mezcla-1.3.7/mezcla/my_regex.py
+-rwxr-xr-x   0        0        0    13776 2023-06-01 21:28:06.605424 mezcla-1.3.7/mezcla/ngram_tfidf.py
+-rwxr-xr-x   0        0        0      183 2023-06-01 21:28:06.605424 mezcla-1.3.7/mezcla/os_utils.py
+-rwxr-xr-x   0        0        0    31436 2023-06-01 21:28:06.609424 mezcla-1.3.7/mezcla/pandas_sklearn.py
+-rwxr-xr-x   0        0        0      828 2023-06-01 21:28:06.609424 mezcla-1.3.7/mezcla/plot_utils.py
+-rwxr-xr-x   0        0        0     7053 2023-06-01 21:28:06.609424 mezcla-1.3.7/mezcla/randomize_lines.py
+-rwxr-xr-x   0        0        0     7012 2023-06-01 21:28:06.609424 mezcla-1.3.7/mezcla/rgb_color_name.py
+-rwxr-xr-x   0        0        0    40529 2023-06-01 21:28:06.609424 mezcla-1.3.7/mezcla/run_albert_classifier.py
+-rwxr-xr-x   0        0        0    39613 2023-06-01 21:28:06.609424 mezcla-1.3.7/mezcla/run_bert_classifier.py
+-rwxr-xr-x   0        0        0    17400 2023-06-01 21:28:06.609424 mezcla-1.3.7/mezcla/show_bert_representation.py
+-rwxr-xr-x   0        0        0     1508 2023-06-01 21:28:06.609424 mezcla-1.3.7/mezcla/simple_main_example.py
+-rwxr-xr-x   0        0        0    19931 2023-06-01 21:28:06.609424 mezcla-1.3.7/mezcla/spacy_nlp.py
+-rwxr-xr-x   0        0        0     3011 2023-06-01 21:28:06.613424 mezcla-1.3.7/mezcla/spell.py
+-rwxr-xr-x   0        0        0     2416 2023-06-01 21:28:06.613424 mezcla-1.3.7/mezcla/sys_version_info_hack.py
+-rw-r--r--   0        0        0    50075 2023-06-01 21:33:21.265397 mezcla-1.3.7/mezcla/system.py
+-rwxr-xr-x   0        0        0    45776 2023-06-01 21:28:06.613424 mezcla-1.3.7/mezcla/temp/simple_batspp.py
+-rwxr-xr-x   0        0        0     5593 2023-06-01 21:28:06.613424 mezcla-1.3.7/mezcla/template.py
+-rw-r--r--   0        0        0     7370 2023-06-01 21:28:06.613424 mezcla-1.3.7/mezcla/tests/LICENSE.txt
+-rw-r--r--   0        0        0      722 2023-06-01 21:28:06.613424 mezcla-1.3.7/mezcla/tests/adhoc-tests.batspp
+-rwxr-xr-x   0        0        0     3905 2023-06-01 21:28:06.613424 mezcla-1.3.7/mezcla/tests/misc_doctests.py
+-rw-r--r--   0        0        0      113 2023-06-01 21:28:06.613424 mezcla-1.3.7/mezcla/tests/resources/cars-fields-2-3-4.txt
+-rw-r--r--   0        0        0      810 2023-06-01 21:33:21.265397 mezcla-1.3.7/mezcla/tests/resources/cars-len-3.txt
+-rw-r--r--   0        0        0      659 2023-06-01 21:28:06.613424 mezcla-1.3.7/mezcla/tests/resources/cars.csv
+-rw-r--r--   0        0        0      755 2023-06-01 21:33:21.265397 mezcla-1.3.7/mezcla/tests/resources/cars.tsv
+-rw-r--r--   0        0        0      603 2023-06-01 21:28:06.613424 mezcla-1.3.7/mezcla/tests/resources/example_text.txt
+-rw-r--r--   0        0        0     2573 2023-06-01 21:28:06.613424 mezcla-1.3.7/mezcla/tests/resources/example_text_tags.txt
+-rw-r--r--   0        0        0     2440 2023-06-01 21:28:06.613424 mezcla-1.3.7/mezcla/tests/resources/iris_output.txt
+-rw-r--r--   0        0        0     1152 2023-06-01 21:28:06.613424 mezcla-1.3.7/mezcla/tests/resources/simple-window-dimensions.html
+-rw-r--r--   0        0        0     5577 2023-06-01 21:28:06.617424 mezcla-1.3.7/mezcla/tests/resources/spanish-accents.docx
+-rw-r--r--   0        0        0    12530 2023-06-01 21:28:06.617424 mezcla-1.3.7/mezcla/tests/resources/spanish-accents.pdf
+-rw-r--r--   0        0        0      141 2023-06-01 21:28:06.617424 mezcla-1.3.7/mezcla/tests/resources/spanish-accents.txt
+-rw-r--r--   0        0        0       65 2023-06-01 21:28:06.617424 mezcla-1.3.7/mezcla/tests/resources/word-POS.freq
+-rw-r--r--   0        0        0      254 2023-06-01 21:28:06.617424 mezcla-1.3.7/mezcla/tests/simple-script-tests.test
+-rwxr-xr-x   0        0        0     4296 2023-06-01 21:28:06.617424 mezcla-1.3.7/mezcla/tests/template.py
+-rwxr-xr-x   0        0        0     4295 2023-06-01 21:28:06.617424 mezcla-1.3.7/mezcla/tests/test_audio.py
+-rwxr-xr-x   0        0        0      969 2023-06-01 21:28:06.617424 mezcla-1.3.7/mezcla/tests/test_bert_multi_classification.py
+-rwxr-xr-x   0        0        0      834 2023-06-01 21:28:06.617424 mezcla-1.3.7/mezcla/tests/test_bing_search.py
+-rwxr-xr-x   0        0        0     1974 2023-06-01 21:28:06.617424 mezcla-1.3.7/mezcla/tests/test_compute_tfidf.py
+-rwxr-xr-x   0        0        0     2932 2023-06-01 21:33:21.265397 mezcla-1.3.7/mezcla/tests/test_cut.py
+-rwxr-xr-x   0        0        0     2068 2023-06-01 21:33:21.265397 mezcla-1.3.7/mezcla/tests/test_data_utils.py
+-rwxr-xr-x   0        0        0    13297 2023-06-01 21:28:06.617424 mezcla-1.3.7/mezcla/tests/test_debug.py
+-rwxr-xr-x   0        0        0     1030 2023-06-01 21:28:06.617424 mezcla-1.3.7/mezcla/tests/test_extract_document_text.py
+-rwxr-xr-x   0        0        0     4290 2023-06-01 21:33:21.265397 mezcla-1.3.7/mezcla/tests/test_file_utils.py
+-rwxr-xr-x   0        0        0     2868 2023-06-01 21:28:06.617424 mezcla-1.3.7/mezcla/tests/test_filter_random.py
+-rwxr-xr-x   0        0        0     2562 2023-06-01 21:28:06.617424 mezcla-1.3.7/mezcla/tests/test_gensim_test.py
+-rwxr-xr-x   0        0        0    15122 2023-06-01 21:33:21.265397 mezcla-1.3.7/mezcla/tests/test_glue_helpers.py
+-rwxr-xr-x   0        0        0    13008 2023-06-01 21:28:06.621424 mezcla-1.3.7/mezcla/tests/test_html_utils.py
+-rwxr-xr-x   0        0        0      892 2023-06-01 21:28:06.621424 mezcla-1.3.7/mezcla/tests/test_kenlm_example.py
+-rwxr-xr-x   0        0        0     1683 2023-06-01 21:33:21.265397 mezcla-1.3.7/mezcla/tests/test_keras_param_search.py
+-rwxr-xr-x   0        0        0     8809 2023-06-01 21:33:21.265397 mezcla-1.3.7/mezcla/tests/test_main.py
+-rwxr-xr-x   0        0        0     2313 2023-06-01 21:33:21.265397 mezcla-1.3.7/mezcla/tests/test_merge_files.py
+-rwxr-xr-x   0        0        0     1291 2023-06-01 21:28:06.621424 mezcla-1.3.7/mezcla/tests/test_merge_notes.py
+-rwxr-xr-x   0        0        0     6565 2023-06-01 21:28:06.621424 mezcla-1.3.7/mezcla/tests/test_misc_utils.py
+-rwxr-xr-x   0        0        0     2882 2023-06-01 21:28:06.621424 mezcla-1.3.7/mezcla/tests/test_my_regex.py
+-rwxr-xr-x   0        0        0      916 2023-06-01 21:28:06.621424 mezcla-1.3.7/mezcla/tests/test_ngram_tfidf.py
+-rwxr-xr-x   0        0        0      819 2023-06-01 21:28:06.621424 mezcla-1.3.7/mezcla/tests/test_os_utils.py
+-rwxr-xr-x   0        0        0     8095 2023-06-01 21:33:21.265397 mezcla-1.3.7/mezcla/tests/test_pandas_sklearn.py
+-rwxr-xr-x   0        0        0      829 2023-06-01 21:28:06.621424 mezcla-1.3.7/mezcla/tests/test_plot_utils.py
+-rwxr-xr-x   0        0        0      854 2023-06-01 21:28:06.621424 mezcla-1.3.7/mezcla/tests/test_randomize_lines.py
+-rwxr-xr-x   0        0        0     2657 2023-06-01 21:33:21.265397 mezcla-1.3.7/mezcla/tests/test_rgb_color_name.py
+-rwxr-xr-x   0        0        0      895 2023-06-01 21:28:06.621424 mezcla-1.3.7/mezcla/tests/test_run_albert_classifier.py
+-rwxr-xr-x   0        0        0      930 2023-06-01 21:28:06.621424 mezcla-1.3.7/mezcla/tests/test_run_bert_classifier.py
+-rwxr-xr-x   0        0        0     1602 2023-06-01 21:28:06.621424 mezcla-1.3.7/mezcla/tests/test_show_bert_representation.py
+-rwxr-xr-x   0        0        0      878 2023-06-01 21:28:06.621424 mezcla-1.3.7/mezcla/tests/test_simple_main_example.py
+-rwxr-xr-x   0        0        0     2060 2023-06-01 21:28:06.621424 mezcla-1.3.7/mezcla/tests/test_spacy_nlp.py
+-rwxr-xr-x   0        0        0      882 2023-06-01 21:28:06.621424 mezcla-1.3.7/mezcla/tests/test_sys_version_info_hack.py
+-rwxr-xr-x   0        0        0    33090 2023-06-01 21:33:21.269397 mezcla-1.3.7/mezcla/tests/test_system.py
+-rwxr-xr-x   0        0        0     1769 2023-06-01 21:28:06.621424 mezcla-1.3.7/mezcla/tests/test_template.py
+-rwxr-xr-x   0        0        0     3651 2023-06-01 21:33:21.269397 mezcla-1.3.7/mezcla/tests/test_text_categorizer.py
+-rwxr-xr-x   0        0        0     7027 2023-06-01 21:33:21.269397 mezcla-1.3.7/mezcla/tests/test_text_processing.py
+-rwxr-xr-x   0        0        0     7362 2023-06-01 21:28:06.621424 mezcla-1.3.7/mezcla/tests/test_text_utils.py
+-rwxr-xr-x   0        0        0    21785 2023-06-01 21:28:06.625424 mezcla-1.3.7/mezcla/tests/test_tpo_common.py
+-rwxr-xr-x   0        0        0      715 2023-06-01 21:28:06.625424 mezcla-1.3.7/mezcla/tests/test_train_language_model.py
+-rwxr-xr-x   0        0        0      725 2023-06-01 21:28:06.625424 mezcla-1.3.7/mezcla/tests/test_train_text_categorizer.py
+-rwxr-xr-x   0        0        0      686 2023-06-01 21:28:06.625424 mezcla-1.3.7/mezcla/tests/test_transpose_data.py
+-rwxr-xr-x   0        0        0     2859 2023-06-01 21:28:06.625424 mezcla-1.3.7/mezcla/tests/test_xml_utils.py
+-rw-r--r--   0        0        0      676 2023-06-01 21:28:06.625424 mezcla-1.3.7/mezcla/tests/tfidf/test_corpus.py
+-rw-r--r--   0        0        0      697 2023-06-01 21:28:06.625424 mezcla-1.3.7/mezcla/tests/tfidf/test_dockeyword.py
+-rw-r--r--   0        0        0      688 2023-06-01 21:28:06.625424 mezcla-1.3.7/mezcla/tests/tfidf/test_document.py
+-rw-r--r--   0        0        0      697 2023-06-01 21:28:06.625424 mezcla-1.3.7/mezcla/tests/tfidf/test_preprocess.py
+-rwxr-xr-x   0        0        0    33807 2023-06-01 21:28:06.625424 mezcla-1.3.7/mezcla/text_categorizer.py
+-rwxr-xr-x   0        0        0    23132 2023-06-01 21:28:06.625424 mezcla-1.3.7/mezcla/text_processing.py
+-rwxr-xr-x   0        0        0    16223 2023-06-01 21:28:06.625424 mezcla-1.3.7/mezcla/text_utils.py
+-rwxr-xr-x   0        0        0      375 2023-06-01 21:28:06.625424 mezcla-1.3.7/mezcla/tfidf/__init__.py
+-rwxr-xr-x   0        0        0    18423 2023-06-01 21:28:06.625424 mezcla-1.3.7/mezcla/tfidf/corpus.py
+-rwxr-xr-x   0        0        0     2282 2023-06-01 21:28:06.625424 mezcla-1.3.7/mezcla/tfidf/dockeyword.py
+-rwxr-xr-x   0        0        0     7983 2023-06-01 21:28:06.629424 mezcla-1.3.7/mezcla/tfidf/document.py
+lrwxr-xr-x   0        0        0        0 2023-06-01 21:28:06.629424 mezcla-1.3.7/mezcla/tfidf/old-version -> /home/tomohara/python/tfidf
+-rwxr-xr-x   0        0        0    16163 2023-06-01 21:28:06.629424 mezcla-1.3.7/mezcla/tfidf/preprocess.py
+-rwxr-xr-x   0        0        0    59862 2023-06-01 21:28:06.629424 mezcla-1.3.7/mezcla/tpo_common.py
+-rwxr-xr-x   0        0        0     5267 2023-06-01 21:28:06.629424 mezcla-1.3.7/mezcla/train_language_model.py
+-rwxr-xr-x   0        0        0     5098 2023-06-01 21:28:06.629424 mezcla-1.3.7/mezcla/train_text_categorizer.py
+-rwxr-xr-x   0        0        0     6778 2023-06-01 21:28:06.629424 mezcla-1.3.7/mezcla/transpose_data.py
+-rw-r--r--   0        0        0    12934 2023-06-01 21:28:06.629424 mezcla-1.3.7/mezcla/unittest_wrapper.py
+-rwxr-xr-x   0        0        0     3543 2023-06-01 21:28:06.629424 mezcla-1.3.7/mezcla/xml_utils.py
+-rw-r--r--   0        0        0      958 2023-06-01 21:28:06.629424 mezcla-1.3.7/pyproject.toml
+-rw-r--r--   0        0        0     1709 2023-06-01 21:33:21.269397 mezcla-1.3.7/requirements.txt
+-rw-r--r--   0        0        0     1162 2023-06-01 21:35:43.501666 mezcla-1.3.7/setup.py
+-rwxr-xr-x   0        0        0    45023 2023-06-01 21:28:06.629424 mezcla-1.3.7/temp/simple_batspp.py
+-rwxr-xr-x   0        0        0      458 2023-06-01 21:33:21.269397 mezcla-1.3.7/tools/run_tests.bash
+-rw-r--r--   0        0        0      567 2023-06-01 21:28:06.629424 mezcla-1.3.7/tox.ini
+-rw-r--r--   0        0        0     1085 1970-01-01 00:00:00.000000 mezcla-1.3.7/PKG-INFO
```

### Comparing `mezcla-1.3.6/.coveragerc` & `mezcla-1.3.7/.coveragerc`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/.github/workflows/tests.yml` & `mezcla-1.3.7/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/.gitignore` & `mezcla-1.3.7/.gitignore`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/LICENSE.txt` & `mezcla-1.3.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/README.txt` & `mezcla-1.3.7/README.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/__init__.py` & `mezcla-1.3.7/mezcla/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     from mezcla import *
     debug.trace(TL.DEFAULT, "Hey")
     debug.trace(TL.DETAILED, "Joe")
 
 Tom O'Hara
 Feb 2022
 """
-__VERSION__ = '1.3.6'
+__VERSION__ = '1.3.7'
 __version__ = __VERSION__
 
 # Standard module(s)
 import sys
 
 # Note: requires python 3 or higher
 PYTHON3_PLUS = (sys.version_info[0] >= 3)
```

### Comparing `mezcla-1.3.6/mezcla/analyze_tfidf.py` & `mezcla-1.3.7/mezcla/analyze_tfidf.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/audio.py` & `mezcla-1.3.7/mezcla/audio.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/bert_multi_classification.py` & `mezcla-1.3.7/mezcla/bert_multi_classification.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/bert_text_classification.py` & `mezcla-1.3.7/mezcla/bert_text_classification.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/bing_search.py` & `mezcla-1.3.7/mezcla/bing_search.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/check_html_javascript.py` & `mezcla-1.3.7/mezcla/check_html_javascript.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/compute_tfidf.py` & `mezcla-1.3.7/mezcla/compute_tfidf.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/cut.py` & `mezcla-1.3.7/mezcla/cut.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/data_utils.py` & `mezcla-1.3.7/mezcla/data_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/debug.py` & `mezcla-1.3.7/mezcla/debug.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/docs/audio_uml.svg` & `mezcla-1.3.7/mezcla/docs/audio_uml.svg`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/examples/alt_sklearn_plot_precision_recall.py` & `mezcla-1.3.7/mezcla/examples/alt_sklearn_plot_precision_recall.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/examples/brownlee_ml_metrics.py` & `mezcla-1.3.7/mezcla/examples/brownlee_ml_metrics.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/examples/consume_all_memory.py` & `mezcla-1.3.7/mezcla/examples/consume_all_memory.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/examples/download_user_gist.py` & `mezcla-1.3.7/mezcla/examples/download_user_gist.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/examples/dump_checkpoints.py` & `mezcla-1.3.7/mezcla/examples/dump_checkpoints.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/examples/encoded-iris.csv` & `mezcla-1.3.7/mezcla/examples/encoded-iris.csv`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/examples/feature_importance.py` & `mezcla-1.3.7/mezcla/examples/feature_importance.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/examples/fuzzy-testing-1-2-3.wav` & `mezcla-1.3.7/mezcla/examples/fuzzy-testing-1-2-3.wav`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/examples/hugging_face_speechrec.py` & `mezcla-1.3.7/mezcla/examples/hugging_face_speechrec.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/examples/hugging_face_translation.py` & `mezcla-1.3.7/mezcla/examples/hugging_face_translation.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/examples/inspect_checkpoint.py` & `mezcla-1.3.7/mezcla/examples/inspect_checkpoint.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/examples/iris.csv` & `mezcla-1.3.7/mezcla/examples/iris.csv`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/examples/pima-indians-diabetes.csv` & `mezcla-1.3.7/mezcla/examples/pima-indians-diabetes.csv`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/examples/plot_forest_importances.py` & `mezcla-1.3.7/mezcla/examples/plot_forest_importances.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/examples/sklearn_plot_precision_recall.py` & `mezcla-1.3.7/mezcla/examples/sklearn_plot_precision_recall.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/examples/template.py` & `mezcla-1.3.7/mezcla/examples/template.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/examples/tensorflow_matrix_multiply.py` & `mezcla-1.3.7/mezcla/examples/tensorflow_matrix_multiply.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/examples/tracemalloc_display.py` & `mezcla-1.3.7/mezcla/examples/tracemalloc_display.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/extract_document_text.py` & `mezcla-1.3.7/mezcla/extract_document_text.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/file_utils.py` & `mezcla-1.3.7/mezcla/file_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/filter_random.py` & `mezcla-1.3.7/mezcla/filter_random.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/format_profile.py` & `mezcla-1.3.7/mezcla/format_profile.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/gensim_test.py` & `mezcla-1.3.7/mezcla/gensim_test.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/glue_helpers.py` & `mezcla-1.3.7/mezcla/glue_helpers.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/html_utils.py` & `mezcla-1.3.7/mezcla/html_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/kenlm_example.py` & `mezcla-1.3.7/mezcla/kenlm_example.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/keras_param_search.py` & `mezcla-1.3.7/mezcla/keras_param_search.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/main.py` & `mezcla-1.3.7/mezcla/main.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/merge_files.py` & `mezcla-1.3.7/mezcla/merge_files.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/merge_notes.py` & `mezcla-1.3.7/mezcla/merge_notes.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/misc_utils.py` & `mezcla-1.3.7/mezcla/misc_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/my_regex.py` & `mezcla-1.3.7/mezcla/my_regex.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/ngram_tfidf.py` & `mezcla-1.3.7/mezcla/ngram_tfidf.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/pandas_sklearn.py` & `mezcla-1.3.7/mezcla/pandas_sklearn.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/plot_utils.py` & `mezcla-1.3.7/mezcla/plot_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/randomize_lines.py` & `mezcla-1.3.7/mezcla/randomize_lines.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/rgb_color_name.py` & `mezcla-1.3.7/mezcla/rgb_color_name.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/run_albert_classifier.py` & `mezcla-1.3.7/mezcla/run_albert_classifier.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/run_bert_classifier.py` & `mezcla-1.3.7/mezcla/run_bert_classifier.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/show_bert_representation.py` & `mezcla-1.3.7/mezcla/show_bert_representation.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/simple_main_example.py` & `mezcla-1.3.7/mezcla/simple_main_example.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/spacy_nlp.py` & `mezcla-1.3.7/mezcla/spacy_nlp.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/spell.py` & `mezcla-1.3.7/mezcla/spell.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/sys_version_info_hack.py` & `mezcla-1.3.7/mezcla/sys_version_info_hack.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/system.py` & `mezcla-1.3.7/mezcla/system.py`

 * *Files 0% similar despite different names*

```diff
@@ -280,20 +280,22 @@
     print_error("Error during {t}: {exc}".
                  format(t=task, exc=get_exception()))
     if show_stack:
         print_full_stack()
     return
 
 
-def exit(message, **namespace):    # pylint: disable=redefined-builtin
+def exit(message=None, **namespace):    # pylint: disable=redefined-builtin
     """Display error MESSAGE to stderr and then exit, using optional
     NAMESPACE for format"""
+    debug.trace(6, f"system.exit{(message, namespace)})")
     if namespace:
         message = message.format(**namespace)
-    print_stderr(message)
+    if message:
+        print_stderr(message)
     return sys.exit()
 
 
 def setenv(var, value):
     """Set environment VAR to VALUE"""
     debug.trace_fmtd(5, "setenv({v}, {val})", v=var, val=value)
     os.environ[var] = value
```

### Comparing `mezcla-1.3.6/mezcla/temp/simple_batspp.py` & `mezcla-1.3.7/mezcla/temp/simple_batspp.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/template.py` & `mezcla-1.3.7/mezcla/template.py`

 * *Files 4% similar despite different names*

```diff
@@ -135,14 +135,10 @@
     debug.assertion(not any(my_re.search(r"^TODO_", m, my_re.IGNORECASE)
                             for m in dir(app)))    
     
 #-------------------------------------------------------------------------------
     
 if __name__ == '__main__':
     debug.trace_current_context(level=TL.QUITE_DETAILED)
-    ## OLD:
-    ## debug.trace_fmt(TL.USUAL, "Environment options: {eo}",
-    ##                 eo=system.formatted_environment_option_descriptions())
-    ## TODO: main => global
     debug.trace(5, f"main __doc__: {main.__doc__}")
-    debug.assertion(main.__doc__)
+    debug.assertion("TODO:" not in __doc__)
     main()
```

### Comparing `mezcla-1.3.6/mezcla/tests/LICENSE.txt` & `mezcla-1.3.7/mezcla/tests/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/tests/adhoc-tests.batspp` & `mezcla-1.3.7/mezcla/tests/adhoc-tests.batspp`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/tests/misc_doctests.py` & `mezcla-1.3.7/mezcla/tests/misc_doctests.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/tests/resources/cars-len-3.txt` & `mezcla-1.3.7/mezcla/tests/resources/cars-len-3.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/tests/resources/cars.csv` & `mezcla-1.3.7/mezcla/tests/resources/cars.csv`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/tests/resources/cars.tsv` & `mezcla-1.3.7/mezcla/tests/resources/cars.tsv`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/tests/resources/example_text.txt` & `mezcla-1.3.7/mezcla/tests/resources/example_text.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/tests/resources/example_text_tags.txt` & `mezcla-1.3.7/mezcla/tests/resources/example_text_tags.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/tests/resources/iris_output.txt` & `mezcla-1.3.7/mezcla/tests/resources/iris_output.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/tests/resources/simple-window-dimensions.html` & `mezcla-1.3.7/mezcla/tests/resources/simple-window-dimensions.html`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/tests/resources/spanish-accents.docx` & `mezcla-1.3.7/mezcla/tests/resources/spanish-accents.docx`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/tests/resources/spanish-accents.pdf` & `mezcla-1.3.7/mezcla/tests/resources/spanish-accents.pdf`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/tests/template.py` & `mezcla-1.3.7/mezcla/tests/template.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/tests/test_audio.py` & `mezcla-1.3.7/mezcla/tests/test_audio.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/tests/test_bert_multi_classification.py` & `mezcla-1.3.7/mezcla/tests/test_bert_multi_classification.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/tests/test_bing_search.py` & `mezcla-1.3.7/mezcla/tests/test_bing_search.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/tests/test_compute_tfidf.py` & `mezcla-1.3.7/mezcla/tests/test_compute_tfidf.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/tests/test_cut.py` & `mezcla-1.3.7/mezcla/tests/test_cut.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/tests/test_data_utils.py` & `mezcla-1.3.7/mezcla/tests/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/tests/test_debug.py` & `mezcla-1.3.7/mezcla/tests/test_debug.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/tests/test_extract_document_text.py` & `mezcla-1.3.7/mezcla/tests/test_extract_document_text.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/tests/test_file_utils.py` & `mezcla-1.3.7/mezcla/tests/test_file_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/tests/test_filter_random.py` & `mezcla-1.3.7/mezcla/tests/test_filter_random.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/tests/test_gensim_test.py` & `mezcla-1.3.7/mezcla/tests/test_gensim_test.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/tests/test_glue_helpers.py` & `mezcla-1.3.7/mezcla/tests/test_glue_helpers.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/tests/test_html_utils.py` & `mezcla-1.3.7/mezcla/tests/test_html_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/tests/test_kenlm_example.py` & `mezcla-1.3.7/mezcla/tests/test_kenlm_example.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/tests/test_keras_param_search.py` & `mezcla-1.3.7/mezcla/tests/test_keras_param_search.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/tests/test_main.py` & `mezcla-1.3.7/mezcla/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/tests/test_merge_files.py` & `mezcla-1.3.7/mezcla/tests/test_merge_files.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/tests/test_merge_notes.py` & `mezcla-1.3.7/mezcla/tests/test_merge_notes.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/tests/test_misc_utils.py` & `mezcla-1.3.7/mezcla/tests/test_misc_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/tests/test_my_regex.py` & `mezcla-1.3.7/mezcla/tests/test_my_regex.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/tests/test_ngram_tfidf.py` & `mezcla-1.3.7/mezcla/tests/test_ngram_tfidf.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/tests/test_os_utils.py` & `mezcla-1.3.7/mezcla/tests/test_os_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/tests/test_pandas_sklearn.py` & `mezcla-1.3.7/mezcla/tests/test_pandas_sklearn.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/tests/test_plot_utils.py` & `mezcla-1.3.7/mezcla/tests/test_plot_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/tests/test_randomize_lines.py` & `mezcla-1.3.7/mezcla/tests/test_randomize_lines.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/tests/test_rgb_color_name.py` & `mezcla-1.3.7/mezcla/tests/test_rgb_color_name.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/tests/test_run_albert_classifier.py` & `mezcla-1.3.7/mezcla/tests/test_run_albert_classifier.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/tests/test_run_bert_classifier.py` & `mezcla-1.3.7/mezcla/tests/test_run_bert_classifier.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/tests/test_show_bert_representation.py` & `mezcla-1.3.7/mezcla/tests/test_show_bert_representation.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/tests/test_simple_main_example.py` & `mezcla-1.3.7/mezcla/tests/test_simple_main_example.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/tests/test_spacy_nlp.py` & `mezcla-1.3.7/mezcla/tests/test_spacy_nlp.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/tests/test_sys_version_info_hack.py` & `mezcla-1.3.7/mezcla/tests/test_sys_version_info_hack.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/tests/test_system.py` & `mezcla-1.3.7/mezcla/tests/test_system.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/tests/test_template.py` & `mezcla-1.3.7/mezcla/tests/test_template.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/tests/test_text_categorizer.py` & `mezcla-1.3.7/mezcla/tests/test_text_categorizer.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/tests/test_text_processing.py` & `mezcla-1.3.7/mezcla/tests/test_text_processing.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/tests/test_text_utils.py` & `mezcla-1.3.7/mezcla/tests/test_text_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/tests/test_tpo_common.py` & `mezcla-1.3.7/mezcla/tests/test_tpo_common.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/tests/test_train_language_model.py` & `mezcla-1.3.7/mezcla/tests/test_train_language_model.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/tests/test_train_text_categorizer.py` & `mezcla-1.3.7/mezcla/tests/test_train_text_categorizer.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/tests/test_transpose_data.py` & `mezcla-1.3.7/mezcla/tests/test_transpose_data.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/tests/test_xml_utils.py` & `mezcla-1.3.7/mezcla/tests/test_xml_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/tests/tfidf/test_corpus.py` & `mezcla-1.3.7/mezcla/tests/tfidf/test_corpus.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/tests/tfidf/test_dockeyword.py` & `mezcla-1.3.7/mezcla/tests/tfidf/test_dockeyword.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/tests/tfidf/test_document.py` & `mezcla-1.3.7/mezcla/tests/tfidf/test_document.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/tests/tfidf/test_preprocess.py` & `mezcla-1.3.7/mezcla/tests/tfidf/test_preprocess.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/text_categorizer.py` & `mezcla-1.3.7/mezcla/text_categorizer.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/text_processing.py` & `mezcla-1.3.7/mezcla/text_processing.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/text_utils.py` & `mezcla-1.3.7/mezcla/text_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/tfidf/corpus.py` & `mezcla-1.3.7/mezcla/tfidf/corpus.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/tfidf/dockeyword.py` & `mezcla-1.3.7/mezcla/tfidf/dockeyword.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/tfidf/document.py` & `mezcla-1.3.7/mezcla/tfidf/document.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/tfidf/preprocess.py` & `mezcla-1.3.7/mezcla/tfidf/preprocess.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/tpo_common.py` & `mezcla-1.3.7/mezcla/tpo_common.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/train_language_model.py` & `mezcla-1.3.7/mezcla/train_language_model.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/train_text_categorizer.py` & `mezcla-1.3.7/mezcla/train_text_categorizer.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/transpose_data.py` & `mezcla-1.3.7/mezcla/transpose_data.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/unittest_wrapper.py` & `mezcla-1.3.7/mezcla/unittest_wrapper.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/mezcla/xml_utils.py` & `mezcla-1.3.7/mezcla/xml_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/pyproject.toml` & `mezcla-1.3.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/requirements.txt` & `mezcla-1.3.7/requirements.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/setup.py` & `mezcla-1.3.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 """Simple installer"""
 
 from distutils.core import setup
 
 setup(name='Mezcla',
       packages=['mezcla'],
       module="mezcla",
-      version='1.3.6',
+      version='1.3.7',
       description-file="README.txt",
       dist-name="Mezcla",
       ## OLD: py_modules=PYTHON_MODULE_NAMES,
       author="Tom O'Hara",
       # TODO: find out which email key is preferred
       email="tomasohara@gmail.com",
       author-email="tomasohara@gmail.com"
```

### Comparing `mezcla-1.3.6/temp/simple_batspp.py` & `mezcla-1.3.7/temp/simple_batspp.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/tox.ini` & `mezcla-1.3.7/tox.ini`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.6/PKG-INFO` & `mezcla-1.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mezcla
-Version: 1.3.6
+Version: 1.3.7
 Summary: Mezcla is Spanish for mixture, and this repository contains a variety of Python scripts.
 Home-page: https://github.com/tomasohara/mezcla
 License: LGPLv3
 Author: Tomás O'Hara
 Author-email: tomasohara@gmail.com
 Description-Content-Type: text/plain
```

