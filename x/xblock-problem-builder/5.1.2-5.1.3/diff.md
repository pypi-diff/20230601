# Comparing `tmp/xblock-problem-builder-5.1.2.tar.gz` & `tmp/xblock-problem-builder-5.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xblock-problem-builder-5.1.2.tar", last modified: Mon Mar  6 14:56:08 2023, max compression
+gzip compressed data, was "xblock-problem-builder-5.1.3.tar", last modified: Thu Jun  1 09:32:50 2023, max compression
```

## Comparing `xblock-problem-builder-5.1.2.tar` & `xblock-problem-builder-5.1.3.tar`

### file list

```diff
@@ -1,278 +1,278 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 14:56:08.097896 xblock-problem-builder-5.1.2/
--rw-r--r--   0 runner    (1001) docker     (122)      404 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (122)    35136 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     1385 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/LICENSE.MIT
--rw-r--r--   0 runner    (1001) docker     (122)      100 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    12758 2023-03-06 14:56:08.097896 xblock-problem-builder-5.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    12411 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 14:56:08.073897 xblock-problem-builder-5.1.2/problem_builder/
--rw-r--r--   0 runner    (1001) docker     (122)       22 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14172 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/answer.py
--rw-r--r--   0 runner    (1001) docker     (122)     5733 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/choice.py
--rw-r--r--   0 runner    (1001) docker     (122)     6750 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/completion.py
--rw-r--r--   0 runner    (1001) docker     (122)    22565 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (122)     3778 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/dashboard_visual.py
--rw-r--r--   0 runner    (1001) docker     (122)    11773 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/instructor_tool.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 14:56:08.073897 xblock-problem-builder-5.1.2/problem_builder/management/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 14:56:08.073897 xblock-problem-builder-5.1.2/problem_builder/management/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1617 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/management/commands/copy_deprecated_course_id.py
--rw-r--r--   0 runner    (1001) docker     (122)    10101 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/mcq.py
--rw-r--r--   0 runner    (1001) docker     (122)    43970 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/mentoring.py
--rw-r--r--   0 runner    (1001) docker     (122)     6686 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/message.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 14:56:08.077896 xblock-problem-builder-5.1.2/problem_builder/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     1010 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)     1177 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/migrations/0002_auto_20160121_1525.py
--rw-r--r--   0 runner    (1001) docker     (122)      571 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/migrations/0003_auto_20161124_0755.py
--rw-r--r--   0 runner    (1001) docker     (122)      698 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/migrations/0004_copy_course_ids.py
--rw-r--r--   0 runner    (1001) docker     (122)      570 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/migrations/0005_auto_20170112_1021.py
--rw-r--r--   0 runner    (1001) docker     (122)      486 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/migrations/0006_remove_deprecated_course_id.py
--rw-r--r--   0 runner    (1001) docker     (122)      424 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/migrations/0007_lengthen_student_id_field.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11239 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/mixins.py
--rw-r--r--   0 runner    (1001) docker     (122)     3496 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/models.py
--rw-r--r--   0 runner    (1001) docker     (122)     8909 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/mrq.py
--rw-r--r--   0 runner    (1001) docker     (122)     3126 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/platform_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (122)    17224 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 14:56:08.065896 xblock-problem-builder-5.1.2/problem_builder/public/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 14:56:08.077896 xblock-problem-builder-5.1.2/problem_builder/public/css/
--rw-r--r--   0 runner    (1001) docker     (122)      612 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/public/css/answer.css
--rw-r--r--   0 runner    (1001) docker     (122)      809 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/public/css/dashboard.css
--rw-r--r--   0 runner    (1001) docker     (122)     1647 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/public/css/instructor_tool.css
--rw-r--r--   0 runner    (1001) docker     (122)     2978 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/public/css/mentoring-table.css
--rw-r--r--   0 runner    (1001) docker     (122)       83 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/public/css/overlay.css
--rw-r--r--   0 runner    (1001) docker     (122)      382 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/public/css/plot-preview.css
--rw-r--r--   0 runner    (1001) docker     (122)      358 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/public/css/plot.css
--rw-r--r--   0 runner    (1001) docker     (122)     4079 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/public/css/problem-builder-edit.css
--rw-r--r--   0 runner    (1001) docker     (122)      302 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/public/css/problem-builder-tinymce-content.css
--rw-r--r--   0 runner    (1001) docker     (122)     6104 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/public/css/problem-builder.css
--rw-r--r--   0 runner    (1001) docker     (122)      820 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/public/css/questionnaire-edit.css
--rw-r--r--   0 runner    (1001) docker     (122)     3675 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/public/css/questionnaire.css
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 14:56:08.077896 xblock-problem-builder-5.1.2/problem_builder/public/img/
--rw-r--r--   0 runner    (1001) docker     (122)     7259 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/public/img/immunity-map-assumptions-bg.png
--rw-r--r--   0 runner    (1001) docker     (122)     4961 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/public/img/immunity-map-bg.png
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 14:56:08.077896 xblock-problem-builder-5.1.2/problem_builder/public/js/
--rw-r--r--   0 runner    (1001) docker     (122)     3685 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/public/js/answer.js
--rw-r--r--   0 runner    (1001) docker     (122)      698 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/public/js/answer_recap.js
--rw-r--r--   0 runner    (1001) docker     (122)     1092 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/public/js/completion.js
--rw-r--r--   0 runner    (1001) docker     (122)      720 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/public/js/container_edit.js
--rw-r--r--   0 runner    (1001) docker     (122)    15907 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/public/js/instructor_tool.js
--rw-r--r--   0 runner    (1001) docker     (122)     3723 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/public/js/mentoring.js
--rw-r--r--   0 runner    (1001) docker     (122)      833 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/public/js/mentoring_edit.js
--rw-r--r--   0 runner    (1001) docker     (122)     5488 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/public/js/mentoring_standard_view.js
--rw-r--r--   0 runner    (1001) docker     (122)    19686 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/public/js/mentoring_with_steps.js
--rw-r--r--   0 runner    (1001) docker     (122)     9502 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/public/js/plot.js
--rw-r--r--   0 runner    (1001) docker     (122)    11147 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/public/js/questionnaire.js
--rw-r--r--   0 runner    (1001) docker     (122)     8527 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/public/js/review_blocks.js
--rw-r--r--   0 runner    (1001) docker     (122)     1102 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/public/js/slider.js
--rw-r--r--   0 runner    (1001) docker     (122)     4451 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/public/js/step.js
--rw-r--r--   0 runner    (1001) docker     (122)     4063 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/public/js/step_util.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 14:56:08.069896 xblock-problem-builder-5.1.2/problem_builder/public/js/translations/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 14:56:08.077896 xblock-problem-builder-5.1.2/problem_builder/public/js/translations/ar/
--rw-r--r--   0 runner    (1001) docker     (122)     6618 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/public/js/translations/ar/textjs.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 14:56:08.077896 xblock-problem-builder-5.1.2/problem_builder/public/js/translations/de_DE/
--rw-r--r--   0 runner    (1001) docker     (122)     4314 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/public/js/translations/de_DE/textjs.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 14:56:08.081896 xblock-problem-builder-5.1.2/problem_builder/public/js/translations/en/
--rw-r--r--   0 runner    (1001) docker     (122)     3632 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/public/js/translations/en/textjs.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 14:56:08.081896 xblock-problem-builder-5.1.2/problem_builder/public/js/translations/eo/
--rw-r--r--   0 runner    (1001) docker     (122)     6137 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/public/js/translations/eo/textjs.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 14:56:08.081896 xblock-problem-builder-5.1.2/problem_builder/public/js/translations/es_419/
--rw-r--r--   0 runner    (1001) docker     (122)     4415 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/public/js/translations/es_419/textjs.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 14:56:08.081896 xblock-problem-builder-5.1.2/problem_builder/public/js/translations/fr/
--rw-r--r--   0 runner    (1001) docker     (122)     4418 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/public/js/translations/fr/textjs.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 14:56:08.081896 xblock-problem-builder-5.1.2/problem_builder/public/js/translations/fr_CA/
--rw-r--r--   0 runner    (1001) docker     (122)     4496 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/public/js/translations/fr_CA/textjs.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 14:56:08.081896 xblock-problem-builder-5.1.2/problem_builder/public/js/translations/ja_JP/
--rw-r--r--   0 runner    (1001) docker     (122)     4699 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/public/js/translations/ja_JP/textjs.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 14:56:08.081896 xblock-problem-builder-5.1.2/problem_builder/public/js/translations/ko_KR/
--rw-r--r--   0 runner    (1001) docker     (122)     4968 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/public/js/translations/ko_KR/textjs.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 14:56:08.081896 xblock-problem-builder-5.1.2/problem_builder/public/js/translations/pl_PL/
--rw-r--r--   0 runner    (1001) docker     (122)     4746 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/public/js/translations/pl_PL/textjs.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 14:56:08.081896 xblock-problem-builder-5.1.2/problem_builder/public/js/translations/pt_BR/
--rw-r--r--   0 runner    (1001) docker     (122)     4441 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/public/js/translations/pt_BR/textjs.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 14:56:08.081896 xblock-problem-builder-5.1.2/problem_builder/public/js/translations/zh_CN/
--rw-r--r--   0 runner    (1001) docker     (122)     4631 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/public/js/translations/zh_CN/textjs.js
--rw-r--r--   0 runner    (1001) docker     (122)     1693 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/public/js/util.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 14:56:08.081896 xblock-problem-builder-5.1.2/problem_builder/public/js/vendor/
--rw-r--r--   0 runner    (1001) docker     (122)    19414 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/public/js/vendor/backbone-min.js
--rw-r--r--   0 runner    (1001) docker     (122)    10736 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/public/js/vendor/backbone.paginator.min.js
--rw-r--r--   0 runner    (1001) docker     (122)   151143 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/public/js/vendor/d3.min.js
--rw-r--r--   0 runner    (1001) docker     (122)     5452 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/public/js/vendor/jquery-shorten.js
--rw-r--r--   0 runner    (1001) docker     (122)    13450 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/public/js/vendor/underscore-min.js
--rw-r--r--   0 runner    (1001) docker     (122)    10433 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/questionnaire.py
--rw-r--r--   0 runner    (1001) docker     (122)     2221 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/settings.py
--rw-r--r--   0 runner    (1001) docker     (122)     6653 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/slider.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 14:56:08.081896 xblock-problem-builder-5.1.2/problem_builder/south_migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     2430 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/south_migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)     2189 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/south_migrations/0002_copy_from_mentoring.py
--rw-r--r--   0 runner    (1001) docker     (122)     6717 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/south_migrations/0003_auto__add_share__add_unique_share_shared_by_shared_with_block_id.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/south_migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11660 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/step.py
--rw-r--r--   0 runner    (1001) docker     (122)    13733 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/step_review.py
--rw-r--r--   0 runner    (1001) docker     (122)     1829 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/sub_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     6284 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/swipe.py
--rw-r--r--   0 runner    (1001) docker     (122)    14475 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/table.py
--rw-r--r--   0 runner    (1001) docker     (122)     7941 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 14:56:08.069896 xblock-problem-builder-5.1.2/problem_builder/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 14:56:08.085896 xblock-problem-builder-5.1.2/problem_builder/templates/html/
--rw-r--r--   0 runner    (1001) docker     (122)      758 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/templates/html/answer_editable.html
--rw-r--r--   0 runner    (1001) docker     (122)      392 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/templates/html/answer_read_only.html
--rw-r--r--   0 runner    (1001) docker     (122)      577 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/templates/html/completion.html
--rw-r--r--   0 runner    (1001) docker     (122)     3189 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/templates/html/dashboard.html
--rw-r--r--   0 runner    (1001) docker     (122)     1029 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/templates/html/dashboard_report.html
--rw-r--r--   0 runner    (1001) docker     (122)     2964 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/templates/html/instructor_tool.html
--rw-r--r--   0 runner    (1001) docker     (122)     1502 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/templates/html/mcqblock.html
--rw-r--r--   0 runner    (1001) docker     (122)      443 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/templates/html/mentoring-column-add-button.html
--rw-r--r--   0 runner    (1001) docker     (122)      317 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/templates/html/mentoring-table-add-button.html
--rw-r--r--   0 runner    (1001) docker     (122)     2161 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/templates/html/mentoring-table-container.html
--rw-r--r--   0 runner    (1001) docker     (122)      676 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/templates/html/mentoring-table-report.html
--rw-r--r--   0 runner    (1001) docker     (122)      313 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/templates/html/mentoring-table-shared-list.html
--rw-r--r--   0 runner    (1001) docker     (122)      401 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/templates/html/mentoring-table.html
--rw-r--r--   0 runner    (1001) docker     (122)     2122 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/templates/html/mentoring.html
--rw-r--r--   0 runner    (1001) docker     (122)      227 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/templates/html/mentoring_url_name.html
--rw-r--r--   0 runner    (1001) docker     (122)     1562 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/templates/html/mentoring_with_steps.html
--rw-r--r--   0 runner    (1001) docker     (122)     1806 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/templates/html/mrqblock.html
--rw-r--r--   0 runner    (1001) docker     (122)      850 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/templates/html/overlay.html
--rw-r--r--   0 runner    (1001) docker     (122)     2269 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/templates/html/plot.html
--rw-r--r--   0 runner    (1001) docker     (122)      770 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/templates/html/plot_preview.html
--rw-r--r--   0 runner    (1001) docker     (122)      708 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/templates/html/questionnaire_add_buttons.html
--rw-r--r--   0 runner    (1001) docker     (122)      214 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/templates/html/rating_edit_footer.html
--rw-r--r--   0 runner    (1001) docker     (122)     2520 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/templates/html/ratingblock.html
--rw-r--r--   0 runner    (1001) docker     (122)      522 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/templates/html/ratingblock_edit_preview.html
--rw-r--r--   0 runner    (1001) docker     (122)      377 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/templates/html/sb-review-per-question-feedback.html
--rw-r--r--   0 runner    (1001) docker     (122)     3690 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/templates/html/sb-review-score.html
--rw-r--r--   0 runner    (1001) docker     (122)      771 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/templates/html/slider.html
--rw-r--r--   0 runner    (1001) docker     (122)      208 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/templates/html/slider_edit_footer.html
--rw-r--r--   0 runner    (1001) docker     (122)      643 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/templates/html/step.html
--rw-r--r--   0 runner    (1001) docker     (122)      166 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/templates/html/tip.html
--rw-r--r--   0 runner    (1001) docker     (122)      248 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/templates/html/tip_choice_group.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 14:56:08.085896 xblock-problem-builder-5.1.2/problem_builder/templates/xml/
--rw-r--r--   0 runner    (1001) docker     (122)     1992 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/templates/xml/mentoring_default.xml
--rw-r--r--   0 runner    (1001) docker     (122)     7014 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/templates/xml/mentoring_demo.xml
--rw-r--r--   0 runner    (1001) docker     (122)     1014 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/templates/xml/mentoring_with_only_one_step.xml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 14:56:08.069896 xblock-problem-builder-5.1.2/problem_builder/tests/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 14:56:08.089896 xblock-problem-builder-5.1.2/problem_builder/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13845 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/tests/integration/base_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     4097 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/tests/integration/test_answer.py
--rw-r--r--   0 runner    (1001) docker     (122)     3732 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/tests/integration/test_author_changes.py
--rw-r--r--   0 runner    (1001) docker     (122)     4032 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/tests/integration/test_clarifications.py
--rw-r--r--   0 runner    (1001) docker     (122)     9749 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/tests/integration/test_completion.py
--rw-r--r--   0 runner    (1001) docker     (122)    16582 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/tests/integration/test_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (122)    18042 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/tests/integration/test_instructor_tool.py
--rw-r--r--   0 runner    (1001) docker     (122)    27003 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/tests/integration/test_mentoring.py
--rw-r--r--   0 runner    (1001) docker     (122)     3782 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/tests/integration/test_messages.py
--rw-r--r--   0 runner    (1001) docker     (122)     3293 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/tests/integration/test_multiple.py
--rw-r--r--   0 runner    (1001) docker     (122)     6315 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/tests/integration/test_progression.py
--rw-r--r--   0 runner    (1001) docker     (122)    13169 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/tests/integration/test_questionnaire.py
--rw-r--r--   0 runner    (1001) docker     (122)     5789 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/tests/integration/test_slider.py
--rw-r--r--   0 runner    (1001) docker     (122)    67028 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/tests/integration/test_step_builder.py
--rw-r--r--   0 runner    (1001) docker     (122)     3244 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/tests/integration/test_table.py
--rw-r--r--   0 runner    (1001) docker     (122)     6302 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/tests/integration/test_titles.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 14:56:08.089896 xblock-problem-builder-5.1.2/problem_builder/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3902 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/tests/unit/test_answer_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)      849 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/tests/unit/test_common.py
--rw-r--r--   0 runner    (1001) docker     (122)     2111 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/tests/unit/test_dashboard_visual.py
--rw-r--r--   0 runner    (1001) docker     (122)     3366 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/tests/unit/test_instructor_tool.py
--rw-r--r--   0 runner    (1001) docker     (122)     1484 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/tests/unit/test_migration.py
--rw-r--r--   0 runner    (1001) docker     (122)    10742 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/tests/unit/test_mixins.py
--rw-r--r--   0 runner    (1001) docker     (122)     1503 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/tests/unit/test_models.py
--rw-r--r--   0 runner    (1001) docker     (122)    12299 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/tests/unit/test_problem_builder.py
--rw-r--r--   0 runner    (1001) docker     (122)     3190 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/tests/unit/test_step.py
--rw-r--r--   0 runner    (1001) docker     (122)     5842 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/tests/unit/test_step_builder.py
--rw-r--r--   0 runner    (1001) docker     (122)      572 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/tests/unit/test_swipe.py
--rw-r--r--   0 runner    (1001) docker     (122)     3009 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/tests/unit/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     5343 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/tip.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 14:56:08.089896 xblock-problem-builder-5.1.2/problem_builder/translations/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 14:56:08.069896 xblock-problem-builder-5.1.2/problem_builder/translations/ar/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 14:56:08.089896 xblock-problem-builder-5.1.2/problem_builder/translations/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     6839 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/translations/ar/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    35662 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/translations/ar/LC_MESSAGES/text.po
--rw-r--r--   0 runner    (1001) docker     (122)     2128 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/translations/ar/LC_MESSAGES/textjs.mo
--rw-r--r--   0 runner    (1001) docker     (122)     3075 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/translations/ar/LC_MESSAGES/textjs.po
--rw-r--r--   0 runner    (1001) docker     (122)      121 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/translations/babel_underscore.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      590 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/translations/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 14:56:08.069896 xblock-problem-builder-5.1.2/problem_builder/translations/de_DE/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 14:56:08.089896 xblock-problem-builder-5.1.2/problem_builder/translations/de_DE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    38290 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/translations/de_DE/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    49224 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/translations/de_DE/LC_MESSAGES/text.po
--rw-r--r--   0 runner    (1001) docker     (122)     1369 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/translations/de_DE/LC_MESSAGES/textjs.mo
--rw-r--r--   0 runner    (1001) docker     (122)     2182 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/translations/de_DE/LC_MESSAGES/textjs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 14:56:08.069896 xblock-problem-builder-5.1.2/problem_builder/translations/en/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 14:56:08.089896 xblock-problem-builder-5.1.2/problem_builder/translations/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    31356 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/translations/en/LC_MESSAGES/text.po
--rw-r--r--   0 runner    (1001) docker     (122)     2115 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/translations/en/LC_MESSAGES/textjs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 14:56:08.069896 xblock-problem-builder-5.1.2/problem_builder/translations/eo/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 14:56:08.089896 xblock-problem-builder-5.1.2/problem_builder/translations/eo/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    61722 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/translations/eo/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    71184 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/translations/eo/LC_MESSAGES/text.po
--rw-r--r--   0 runner    (1001) docker     (122)     1797 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/translations/eo/LC_MESSAGES/textjs.mo
--rw-r--r--   0 runner    (1001) docker     (122)     2558 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/translations/eo/LC_MESSAGES/textjs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 14:56:08.069896 xblock-problem-builder-5.1.2/problem_builder/translations/es_419/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 14:56:08.093896 xblock-problem-builder-5.1.2/problem_builder/translations/es_419/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    37888 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/translations/es_419/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    48896 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/translations/es_419/LC_MESSAGES/text.po
--rw-r--r--   0 runner    (1001) docker     (122)     1356 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/translations/es_419/LC_MESSAGES/textjs.mo
--rw-r--r--   0 runner    (1001) docker     (122)     2169 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/translations/es_419/LC_MESSAGES/textjs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 14:56:08.069896 xblock-problem-builder-5.1.2/problem_builder/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 14:56:08.093896 xblock-problem-builder-5.1.2/problem_builder/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    38073 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/translations/fr/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    48994 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/translations/fr/LC_MESSAGES/text.po
--rw-r--r--   0 runner    (1001) docker     (122)     1341 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/translations/fr/LC_MESSAGES/textjs.mo
--rw-r--r--   0 runner    (1001) docker     (122)     2194 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/translations/fr/LC_MESSAGES/textjs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 14:56:08.069896 xblock-problem-builder-5.1.2/problem_builder/translations/fr_CA/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 14:56:08.093896 xblock-problem-builder-5.1.2/problem_builder/translations/fr_CA/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    37716 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/translations/fr_CA/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    48281 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/translations/fr_CA/LC_MESSAGES/text.po
--rw-r--r--   0 runner    (1001) docker     (122)     1366 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/translations/fr_CA/LC_MESSAGES/textjs.mo
--rw-r--r--   0 runner    (1001) docker     (122)     2232 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/translations/fr_CA/LC_MESSAGES/textjs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 14:56:08.069896 xblock-problem-builder-5.1.2/problem_builder/translations/ja_JP/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 14:56:08.093896 xblock-problem-builder-5.1.2/problem_builder/translations/ja_JP/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    38572 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/translations/ja_JP/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    48929 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/translations/ja_JP/LC_MESSAGES/text.po
--rw-r--r--   0 runner    (1001) docker     (122)     1281 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/translations/ja_JP/LC_MESSAGES/textjs.mo
--rw-r--r--   0 runner    (1001) docker     (122)     2120 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/translations/ja_JP/LC_MESSAGES/textjs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 14:56:08.069896 xblock-problem-builder-5.1.2/problem_builder/translations/ko_KR/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 14:56:08.093896 xblock-problem-builder-5.1.2/problem_builder/translations/ko_KR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    37697 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/translations/ko_KR/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    47642 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/translations/ko_KR/LC_MESSAGES/text.po
--rw-r--r--   0 runner    (1001) docker     (122)     1716 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/translations/ko_KR/LC_MESSAGES/textjs.mo
--rw-r--r--   0 runner    (1001) docker     (122)     2505 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/translations/ko_KR/LC_MESSAGES/textjs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 14:56:08.069896 xblock-problem-builder-5.1.2/problem_builder/translations/pl_PL/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 14:56:08.093896 xblock-problem-builder-5.1.2/problem_builder/translations/pl_PL/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    37861 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/translations/pl_PL/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    48470 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/translations/pl_PL/LC_MESSAGES/text.po
--rw-r--r--   0 runner    (1001) docker     (122)     1710 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/translations/pl_PL/LC_MESSAGES/textjs.mo
--rw-r--r--   0 runner    (1001) docker     (122)     2565 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/translations/pl_PL/LC_MESSAGES/textjs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 14:56:08.069896 xblock-problem-builder-5.1.2/problem_builder/translations/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 14:56:08.093896 xblock-problem-builder-5.1.2/problem_builder/translations/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    36987 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/translations/pt_BR/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    48328 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/translations/pt_BR/LC_MESSAGES/text.po
--rw-r--r--   0 runner    (1001) docker     (122)     1330 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/translations/pt_BR/LC_MESSAGES/textjs.mo
--rw-r--r--   0 runner    (1001) docker     (122)     2173 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/translations/pt_BR/LC_MESSAGES/textjs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 14:56:08.069896 xblock-problem-builder-5.1.2/problem_builder/translations/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 14:56:08.097896 xblock-problem-builder-5.1.2/problem_builder/translations/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    32948 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/translations/zh_CN/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    43463 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/translations/zh_CN/LC_MESSAGES/text.po
--rw-r--r--   0 runner    (1001) docker     (122)     1331 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/translations/zh_CN/LC_MESSAGES/textjs.mo
--rw-r--r--   0 runner    (1001) docker     (122)     2177 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/translations/zh_CN/LC_MESSAGES/textjs.po
--rw-r--r--   0 runner    (1001) docker     (122)      749 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 14:56:08.097896 xblock-problem-builder-5.1.2/problem_builder/v1/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4633 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/v1/studio_xml_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     9556 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/v1/upgrade.py
--rw-r--r--   0 runner    (1001) docker     (122)    12550 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/problem_builder/v1/xml_changes.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 14:56:08.097896 xblock-problem-builder-5.1.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      103 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      578 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      112 2023-03-06 14:56:08.097896 xblock-problem-builder-5.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     7536 2023-03-06 14:56:05.000000 xblock-problem-builder-5.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 14:56:08.097896 xblock-problem-builder-5.1.2/xblock_problem_builder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    12758 2023-03-06 14:56:08.000000 xblock-problem-builder-5.1.2/xblock_problem_builder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    10177 2023-03-06 14:56:08.000000 xblock-problem-builder-5.1.2/xblock_problem_builder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-06 14:56:08.000000 xblock-problem-builder-5.1.2/xblock_problem_builder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1405 2023-03-06 14:56:08.000000 xblock-problem-builder-5.1.2/xblock_problem_builder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       36 2023-03-06 14:56:08.000000 xblock-problem-builder-5.1.2/xblock_problem_builder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-03-06 14:56:08.000000 xblock-problem-builder-5.1.2/xblock_problem_builder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 09:32:50.460601 xblock-problem-builder-5.1.3/
+-rw-r--r--   0 runner    (1001) docker     (122)      404 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (122)    35136 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     1385 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/LICENSE.MIT
+-rw-r--r--   0 runner    (1001) docker     (122)      100 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    12758 2023-06-01 09:32:50.460601 xblock-problem-builder-5.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    12411 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 09:32:50.436601 xblock-problem-builder-5.1.3/problem_builder/
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14172 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/answer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5733 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/choice.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6750 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/completion.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22565 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3778 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/dashboard_visual.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11773 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/instructor_tool.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 09:32:50.436601 xblock-problem-builder-5.1.3/problem_builder/management/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 09:32:50.436601 xblock-problem-builder-5.1.3/problem_builder/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1617 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/management/commands/copy_deprecated_course_id.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10101 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/mcq.py
+-rw-r--r--   0 runner    (1001) docker     (122)    43970 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/mentoring.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6686 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/message.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 09:32:50.436601 xblock-problem-builder-5.1.3/problem_builder/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     1010 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1177 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/migrations/0002_auto_20160121_1525.py
+-rw-r--r--   0 runner    (1001) docker     (122)      571 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/migrations/0003_auto_20161124_0755.py
+-rw-r--r--   0 runner    (1001) docker     (122)      698 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/migrations/0004_copy_course_ids.py
+-rw-r--r--   0 runner    (1001) docker     (122)      570 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/migrations/0005_auto_20170112_1021.py
+-rw-r--r--   0 runner    (1001) docker     (122)      486 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/migrations/0006_remove_deprecated_course_id.py
+-rw-r--r--   0 runner    (1001) docker     (122)      424 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/migrations/0007_lengthen_student_id_field.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11248 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3496 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8909 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/mrq.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3126 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/platform_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17224 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 09:32:50.412600 xblock-problem-builder-5.1.3/problem_builder/public/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 09:32:50.440601 xblock-problem-builder-5.1.3/problem_builder/public/css/
+-rw-r--r--   0 runner    (1001) docker     (122)      612 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/public/css/answer.css
+-rw-r--r--   0 runner    (1001) docker     (122)      809 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/public/css/dashboard.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1647 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/public/css/instructor_tool.css
+-rw-r--r--   0 runner    (1001) docker     (122)     2978 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/public/css/mentoring-table.css
+-rw-r--r--   0 runner    (1001) docker     (122)       83 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/public/css/overlay.css
+-rw-r--r--   0 runner    (1001) docker     (122)      382 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/public/css/plot-preview.css
+-rw-r--r--   0 runner    (1001) docker     (122)      358 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/public/css/plot.css
+-rw-r--r--   0 runner    (1001) docker     (122)     4079 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/public/css/problem-builder-edit.css
+-rw-r--r--   0 runner    (1001) docker     (122)      302 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/public/css/problem-builder-tinymce-content.css
+-rw-r--r--   0 runner    (1001) docker     (122)     6104 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/public/css/problem-builder.css
+-rw-r--r--   0 runner    (1001) docker     (122)      820 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/public/css/questionnaire-edit.css
+-rw-r--r--   0 runner    (1001) docker     (122)     3675 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/public/css/questionnaire.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 09:32:50.440601 xblock-problem-builder-5.1.3/problem_builder/public/img/
+-rw-r--r--   0 runner    (1001) docker     (122)     7259 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/public/img/immunity-map-assumptions-bg.png
+-rw-r--r--   0 runner    (1001) docker     (122)     4961 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/public/img/immunity-map-bg.png
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 09:32:50.440601 xblock-problem-builder-5.1.3/problem_builder/public/js/
+-rw-r--r--   0 runner    (1001) docker     (122)     3685 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/public/js/answer.js
+-rw-r--r--   0 runner    (1001) docker     (122)      698 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/public/js/answer_recap.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1092 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/public/js/completion.js
+-rw-r--r--   0 runner    (1001) docker     (122)      720 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/public/js/container_edit.js
+-rw-r--r--   0 runner    (1001) docker     (122)    15907 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/public/js/instructor_tool.js
+-rw-r--r--   0 runner    (1001) docker     (122)     3723 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/public/js/mentoring.js
+-rw-r--r--   0 runner    (1001) docker     (122)      833 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/public/js/mentoring_edit.js
+-rw-r--r--   0 runner    (1001) docker     (122)     5488 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/public/js/mentoring_standard_view.js
+-rw-r--r--   0 runner    (1001) docker     (122)    19686 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/public/js/mentoring_with_steps.js
+-rw-r--r--   0 runner    (1001) docker     (122)     9502 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/public/js/plot.js
+-rw-r--r--   0 runner    (1001) docker     (122)    11147 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/public/js/questionnaire.js
+-rw-r--r--   0 runner    (1001) docker     (122)     8527 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/public/js/review_blocks.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1102 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/public/js/slider.js
+-rw-r--r--   0 runner    (1001) docker     (122)     4451 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/public/js/step.js
+-rw-r--r--   0 runner    (1001) docker     (122)     4063 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/public/js/step_util.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 09:32:50.416601 xblock-problem-builder-5.1.3/problem_builder/public/js/translations/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 09:32:50.440601 xblock-problem-builder-5.1.3/problem_builder/public/js/translations/ar/
+-rw-r--r--   0 runner    (1001) docker     (122)     6618 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/public/js/translations/ar/textjs.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 09:32:50.440601 xblock-problem-builder-5.1.3/problem_builder/public/js/translations/de_DE/
+-rw-r--r--   0 runner    (1001) docker     (122)     4314 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/public/js/translations/de_DE/textjs.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 09:32:50.440601 xblock-problem-builder-5.1.3/problem_builder/public/js/translations/en/
+-rw-r--r--   0 runner    (1001) docker     (122)     3632 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/public/js/translations/en/textjs.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 09:32:50.440601 xblock-problem-builder-5.1.3/problem_builder/public/js/translations/eo/
+-rw-r--r--   0 runner    (1001) docker     (122)     6137 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/public/js/translations/eo/textjs.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 09:32:50.440601 xblock-problem-builder-5.1.3/problem_builder/public/js/translations/es_419/
+-rw-r--r--   0 runner    (1001) docker     (122)     4415 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/public/js/translations/es_419/textjs.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 09:32:50.444601 xblock-problem-builder-5.1.3/problem_builder/public/js/translations/fr/
+-rw-r--r--   0 runner    (1001) docker     (122)     4418 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/public/js/translations/fr/textjs.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 09:32:50.444601 xblock-problem-builder-5.1.3/problem_builder/public/js/translations/fr_CA/
+-rw-r--r--   0 runner    (1001) docker     (122)     4496 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/public/js/translations/fr_CA/textjs.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 09:32:50.444601 xblock-problem-builder-5.1.3/problem_builder/public/js/translations/ja_JP/
+-rw-r--r--   0 runner    (1001) docker     (122)     4699 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/public/js/translations/ja_JP/textjs.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 09:32:50.444601 xblock-problem-builder-5.1.3/problem_builder/public/js/translations/ko_KR/
+-rw-r--r--   0 runner    (1001) docker     (122)     4968 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/public/js/translations/ko_KR/textjs.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 09:32:50.444601 xblock-problem-builder-5.1.3/problem_builder/public/js/translations/pl_PL/
+-rw-r--r--   0 runner    (1001) docker     (122)     4746 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/public/js/translations/pl_PL/textjs.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 09:32:50.444601 xblock-problem-builder-5.1.3/problem_builder/public/js/translations/pt_BR/
+-rw-r--r--   0 runner    (1001) docker     (122)     4441 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/public/js/translations/pt_BR/textjs.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 09:32:50.444601 xblock-problem-builder-5.1.3/problem_builder/public/js/translations/zh_CN/
+-rw-r--r--   0 runner    (1001) docker     (122)     4631 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/public/js/translations/zh_CN/textjs.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1693 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/public/js/util.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 09:32:50.444601 xblock-problem-builder-5.1.3/problem_builder/public/js/vendor/
+-rw-r--r--   0 runner    (1001) docker     (122)    19414 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/public/js/vendor/backbone-min.js
+-rw-r--r--   0 runner    (1001) docker     (122)    10736 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/public/js/vendor/backbone.paginator.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)   151143 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/public/js/vendor/d3.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)     5452 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/public/js/vendor/jquery-shorten.js
+-rw-r--r--   0 runner    (1001) docker     (122)    13450 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/public/js/vendor/underscore-min.js
+-rw-r--r--   0 runner    (1001) docker     (122)    10433 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/questionnaire.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2221 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6653 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/slider.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 09:32:50.444601 xblock-problem-builder-5.1.3/problem_builder/south_migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     2430 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/south_migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2189 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/south_migrations/0002_copy_from_mentoring.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6717 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/south_migrations/0003_auto__add_share__add_unique_share_shared_by_shared_with_block_id.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/south_migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11660 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/step.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13733 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/step_review.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1829 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/sub_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6284 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/swipe.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14475 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/table.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7941 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 09:32:50.416601 xblock-problem-builder-5.1.3/problem_builder/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 09:32:50.448601 xblock-problem-builder-5.1.3/problem_builder/templates/html/
+-rw-r--r--   0 runner    (1001) docker     (122)      758 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/templates/html/answer_editable.html
+-rw-r--r--   0 runner    (1001) docker     (122)      392 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/templates/html/answer_read_only.html
+-rw-r--r--   0 runner    (1001) docker     (122)      577 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/templates/html/completion.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3189 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/templates/html/dashboard.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1029 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/templates/html/dashboard_report.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2964 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/templates/html/instructor_tool.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1502 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/templates/html/mcqblock.html
+-rw-r--r--   0 runner    (1001) docker     (122)      443 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/templates/html/mentoring-column-add-button.html
+-rw-r--r--   0 runner    (1001) docker     (122)      317 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/templates/html/mentoring-table-add-button.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2161 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/templates/html/mentoring-table-container.html
+-rw-r--r--   0 runner    (1001) docker     (122)      676 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/templates/html/mentoring-table-report.html
+-rw-r--r--   0 runner    (1001) docker     (122)      313 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/templates/html/mentoring-table-shared-list.html
+-rw-r--r--   0 runner    (1001) docker     (122)      401 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/templates/html/mentoring-table.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2122 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/templates/html/mentoring.html
+-rw-r--r--   0 runner    (1001) docker     (122)      227 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/templates/html/mentoring_url_name.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1562 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/templates/html/mentoring_with_steps.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1806 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/templates/html/mrqblock.html
+-rw-r--r--   0 runner    (1001) docker     (122)      850 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/templates/html/overlay.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2269 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/templates/html/plot.html
+-rw-r--r--   0 runner    (1001) docker     (122)      770 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/templates/html/plot_preview.html
+-rw-r--r--   0 runner    (1001) docker     (122)      708 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/templates/html/questionnaire_add_buttons.html
+-rw-r--r--   0 runner    (1001) docker     (122)      214 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/templates/html/rating_edit_footer.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2520 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/templates/html/ratingblock.html
+-rw-r--r--   0 runner    (1001) docker     (122)      522 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/templates/html/ratingblock_edit_preview.html
+-rw-r--r--   0 runner    (1001) docker     (122)      377 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/templates/html/sb-review-per-question-feedback.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3690 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/templates/html/sb-review-score.html
+-rw-r--r--   0 runner    (1001) docker     (122)      771 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/templates/html/slider.html
+-rw-r--r--   0 runner    (1001) docker     (122)      208 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/templates/html/slider_edit_footer.html
+-rw-r--r--   0 runner    (1001) docker     (122)      643 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/templates/html/step.html
+-rw-r--r--   0 runner    (1001) docker     (122)      166 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/templates/html/tip.html
+-rw-r--r--   0 runner    (1001) docker     (122)      248 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/templates/html/tip_choice_group.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 09:32:50.448601 xblock-problem-builder-5.1.3/problem_builder/templates/xml/
+-rw-r--r--   0 runner    (1001) docker     (122)     1992 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/templates/xml/mentoring_default.xml
+-rw-r--r--   0 runner    (1001) docker     (122)     7014 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/templates/xml/mentoring_demo.xml
+-rw-r--r--   0 runner    (1001) docker     (122)     1014 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/templates/xml/mentoring_with_only_one_step.xml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 09:32:50.420601 xblock-problem-builder-5.1.3/problem_builder/tests/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 09:32:50.452601 xblock-problem-builder-5.1.3/problem_builder/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13845 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/tests/integration/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4097 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/tests/integration/test_answer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3732 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/tests/integration/test_author_changes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4032 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/tests/integration/test_clarifications.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9749 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/tests/integration/test_completion.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16582 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/tests/integration/test_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18042 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/tests/integration/test_instructor_tool.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27003 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/tests/integration/test_mentoring.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3782 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/tests/integration/test_messages.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3293 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/tests/integration/test_multiple.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6315 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/tests/integration/test_progression.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13169 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/tests/integration/test_questionnaire.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5789 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/tests/integration/test_slider.py
+-rw-r--r--   0 runner    (1001) docker     (122)    67028 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/tests/integration/test_step_builder.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3244 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/tests/integration/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6302 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/tests/integration/test_titles.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 09:32:50.452601 xblock-problem-builder-5.1.3/problem_builder/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3902 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/tests/unit/test_answer_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)      849 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/tests/unit/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2111 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/tests/unit/test_dashboard_visual.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3366 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/tests/unit/test_instructor_tool.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1484 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/tests/unit/test_migration.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10742 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/tests/unit/test_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1503 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/tests/unit/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12299 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/tests/unit/test_problem_builder.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3190 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/tests/unit/test_step.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5842 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/tests/unit/test_step_builder.py
+-rw-r--r--   0 runner    (1001) docker     (122)      572 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/tests/unit/test_swipe.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3009 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/tests/unit/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5343 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/tip.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 09:32:50.452601 xblock-problem-builder-5.1.3/problem_builder/translations/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 09:32:50.420601 xblock-problem-builder-5.1.3/problem_builder/translations/ar/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 09:32:50.452601 xblock-problem-builder-5.1.3/problem_builder/translations/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     6839 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/translations/ar/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    35662 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/translations/ar/LC_MESSAGES/text.po
+-rw-r--r--   0 runner    (1001) docker     (122)     2128 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/translations/ar/LC_MESSAGES/textjs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     3075 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/translations/ar/LC_MESSAGES/textjs.po
+-rw-r--r--   0 runner    (1001) docker     (122)      121 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/translations/babel_underscore.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      590 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/translations/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 09:32:50.420601 xblock-problem-builder-5.1.3/problem_builder/translations/de_DE/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 09:32:50.452601 xblock-problem-builder-5.1.3/problem_builder/translations/de_DE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    38290 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/translations/de_DE/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    49224 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/translations/de_DE/LC_MESSAGES/text.po
+-rw-r--r--   0 runner    (1001) docker     (122)     1369 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/translations/de_DE/LC_MESSAGES/textjs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     2182 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/translations/de_DE/LC_MESSAGES/textjs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 09:32:50.420601 xblock-problem-builder-5.1.3/problem_builder/translations/en/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 09:32:50.456601 xblock-problem-builder-5.1.3/problem_builder/translations/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    31356 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/translations/en/LC_MESSAGES/text.po
+-rw-r--r--   0 runner    (1001) docker     (122)     2115 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/translations/en/LC_MESSAGES/textjs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 09:32:50.420601 xblock-problem-builder-5.1.3/problem_builder/translations/eo/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 09:32:50.456601 xblock-problem-builder-5.1.3/problem_builder/translations/eo/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    61722 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/translations/eo/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    71184 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/translations/eo/LC_MESSAGES/text.po
+-rw-r--r--   0 runner    (1001) docker     (122)     1797 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/translations/eo/LC_MESSAGES/textjs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     2558 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/translations/eo/LC_MESSAGES/textjs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 09:32:50.420601 xblock-problem-builder-5.1.3/problem_builder/translations/es_419/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 09:32:50.456601 xblock-problem-builder-5.1.3/problem_builder/translations/es_419/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    37888 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/translations/es_419/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    48896 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/translations/es_419/LC_MESSAGES/text.po
+-rw-r--r--   0 runner    (1001) docker     (122)     1356 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/translations/es_419/LC_MESSAGES/textjs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     2169 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/translations/es_419/LC_MESSAGES/textjs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 09:32:50.420601 xblock-problem-builder-5.1.3/problem_builder/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 09:32:50.456601 xblock-problem-builder-5.1.3/problem_builder/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    38073 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/translations/fr/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    48994 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/translations/fr/LC_MESSAGES/text.po
+-rw-r--r--   0 runner    (1001) docker     (122)     1341 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/translations/fr/LC_MESSAGES/textjs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     2194 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/translations/fr/LC_MESSAGES/textjs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 09:32:50.424601 xblock-problem-builder-5.1.3/problem_builder/translations/fr_CA/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 09:32:50.456601 xblock-problem-builder-5.1.3/problem_builder/translations/fr_CA/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    37716 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/translations/fr_CA/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    48281 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/translations/fr_CA/LC_MESSAGES/text.po
+-rw-r--r--   0 runner    (1001) docker     (122)     1366 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/translations/fr_CA/LC_MESSAGES/textjs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     2232 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/translations/fr_CA/LC_MESSAGES/textjs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 09:32:50.424601 xblock-problem-builder-5.1.3/problem_builder/translations/ja_JP/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 09:32:50.456601 xblock-problem-builder-5.1.3/problem_builder/translations/ja_JP/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    38572 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/translations/ja_JP/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    48929 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/translations/ja_JP/LC_MESSAGES/text.po
+-rw-r--r--   0 runner    (1001) docker     (122)     1281 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/translations/ja_JP/LC_MESSAGES/textjs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     2120 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/translations/ja_JP/LC_MESSAGES/textjs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 09:32:50.424601 xblock-problem-builder-5.1.3/problem_builder/translations/ko_KR/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 09:32:50.456601 xblock-problem-builder-5.1.3/problem_builder/translations/ko_KR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    37697 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/translations/ko_KR/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    47642 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/translations/ko_KR/LC_MESSAGES/text.po
+-rw-r--r--   0 runner    (1001) docker     (122)     1716 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/translations/ko_KR/LC_MESSAGES/textjs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     2505 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/translations/ko_KR/LC_MESSAGES/textjs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 09:32:50.424601 xblock-problem-builder-5.1.3/problem_builder/translations/pl_PL/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 09:32:50.460601 xblock-problem-builder-5.1.3/problem_builder/translations/pl_PL/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    37861 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/translations/pl_PL/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    48470 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/translations/pl_PL/LC_MESSAGES/text.po
+-rw-r--r--   0 runner    (1001) docker     (122)     1710 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/translations/pl_PL/LC_MESSAGES/textjs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     2565 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/translations/pl_PL/LC_MESSAGES/textjs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 09:32:50.424601 xblock-problem-builder-5.1.3/problem_builder/translations/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 09:32:50.460601 xblock-problem-builder-5.1.3/problem_builder/translations/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    36987 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/translations/pt_BR/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    48328 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/translations/pt_BR/LC_MESSAGES/text.po
+-rw-r--r--   0 runner    (1001) docker     (122)     1330 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/translations/pt_BR/LC_MESSAGES/textjs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     2173 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/translations/pt_BR/LC_MESSAGES/textjs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 09:32:50.424601 xblock-problem-builder-5.1.3/problem_builder/translations/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 09:32:50.460601 xblock-problem-builder-5.1.3/problem_builder/translations/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    32948 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/translations/zh_CN/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    43463 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/translations/zh_CN/LC_MESSAGES/text.po
+-rw-r--r--   0 runner    (1001) docker     (122)     1331 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/translations/zh_CN/LC_MESSAGES/textjs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     2177 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/translations/zh_CN/LC_MESSAGES/textjs.po
+-rw-r--r--   0 runner    (1001) docker     (122)      749 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 09:32:50.460601 xblock-problem-builder-5.1.3/problem_builder/v1/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4633 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/v1/studio_xml_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9556 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/v1/upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12550 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/problem_builder/v1/xml_changes.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 09:32:50.460601 xblock-problem-builder-5.1.3/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      578 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      112 2023-06-01 09:32:50.460601 xblock-problem-builder-5.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     7536 2023-06-01 09:32:44.000000 xblock-problem-builder-5.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 09:32:50.460601 xblock-problem-builder-5.1.3/xblock_problem_builder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    12758 2023-06-01 09:32:50.000000 xblock-problem-builder-5.1.3/xblock_problem_builder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    10177 2023-06-01 09:32:50.000000 xblock-problem-builder-5.1.3/xblock_problem_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-01 09:32:50.000000 xblock-problem-builder-5.1.3/xblock_problem_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1405 2023-06-01 09:32:50.000000 xblock-problem-builder-5.1.3/xblock_problem_builder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       36 2023-06-01 09:32:50.000000 xblock-problem-builder-5.1.3/xblock_problem_builder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-06-01 09:32:50.000000 xblock-problem-builder-5.1.3/xblock_problem_builder.egg-info/top_level.txt
```

### Comparing `xblock-problem-builder-5.1.2/LICENSE` & `xblock-problem-builder-5.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/LICENSE.MIT` & `xblock-problem-builder-5.1.3/LICENSE.MIT`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/PKG-INFO` & `xblock-problem-builder-5.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xblock-problem-builder
-Version: 5.1.2
+Version: 5.1.3
 Summary: XBlock - Problem Builder
 Home-page: https://github.com/open-craft/problem-builder
 Author: OpenCraft
 License: AGPL v3
 Keywords: Python edx
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `xblock-problem-builder-5.1.2/README.md` & `xblock-problem-builder-5.1.3/README.md`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/answer.py` & `xblock-problem-builder-5.1.3/problem_builder/answer.py`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/choice.py` & `xblock-problem-builder-5.1.3/problem_builder/choice.py`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/completion.py` & `xblock-problem-builder-5.1.3/problem_builder/completion.py`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/dashboard.py` & `xblock-problem-builder-5.1.3/problem_builder/dashboard.py`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/dashboard_visual.py` & `xblock-problem-builder-5.1.3/problem_builder/dashboard_visual.py`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/instructor_tool.py` & `xblock-problem-builder-5.1.3/problem_builder/instructor_tool.py`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/management/commands/copy_deprecated_course_id.py` & `xblock-problem-builder-5.1.3/problem_builder/management/commands/copy_deprecated_course_id.py`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/mcq.py` & `xblock-problem-builder-5.1.3/problem_builder/mcq.py`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/mentoring.py` & `xblock-problem-builder-5.1.3/problem_builder/mentoring.py`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/message.py` & `xblock-problem-builder-5.1.3/problem_builder/message.py`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/migrations/0001_initial.py` & `xblock-problem-builder-5.1.3/problem_builder/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/migrations/0002_auto_20160121_1525.py` & `xblock-problem-builder-5.1.3/problem_builder/migrations/0002_auto_20160121_1525.py`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/migrations/0003_auto_20161124_0755.py` & `xblock-problem-builder-5.1.3/problem_builder/migrations/0003_auto_20161124_0755.py`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/migrations/0004_copy_course_ids.py` & `xblock-problem-builder-5.1.3/problem_builder/migrations/0004_copy_course_ids.py`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/migrations/0005_auto_20170112_1021.py` & `xblock-problem-builder-5.1.3/problem_builder/migrations/0005_auto_20170112_1021.py`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/mixins.py` & `xblock-problem-builder-5.1.3/problem_builder/mixins.py`

 * *Files 1% similar despite different names*

```diff
@@ -291,16 +291,16 @@
         only portable URL format for static files that works across export/import and reruns).
         This method is unfortunately a bit hackish since XBlock does not provide a low-level API
         for this.
         """
         if not text:
             return text
 
-        if hasattr(self.runtime, 'replace_urls'):
-            text = self.runtime.replace_urls(text)
+        if replace_urls := getattr(self.runtime, 'replace_urls', None):
+            text = replace_urls(text)
         elif hasattr(self.runtime, 'course_id'):
             # edX Studio uses a different runtime for 'studio_view' than 'student_view',
             # and the 'studio_view' runtime doesn't provide the replace_urls API.
             from .platform_dependencies import replace_static_urls
             if replace_static_urls:
                 text = replace_static_urls(text, course_id=self.runtime.course_id)
         return text
```

### Comparing `xblock-problem-builder-5.1.2/problem_builder/models.py` & `xblock-problem-builder-5.1.3/problem_builder/models.py`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/mrq.py` & `xblock-problem-builder-5.1.3/problem_builder/mrq.py`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/platform_dependencies.py` & `xblock-problem-builder-5.1.3/problem_builder/platform_dependencies.py`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/plot.py` & `xblock-problem-builder-5.1.3/problem_builder/plot.py`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/public/css/answer.css` & `xblock-problem-builder-5.1.3/problem_builder/public/css/answer.css`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/public/css/dashboard.css` & `xblock-problem-builder-5.1.3/problem_builder/public/css/dashboard.css`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/public/css/instructor_tool.css` & `xblock-problem-builder-5.1.3/problem_builder/public/css/instructor_tool.css`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/public/css/mentoring-table.css` & `xblock-problem-builder-5.1.3/problem_builder/public/css/mentoring-table.css`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/public/css/problem-builder-edit.css` & `xblock-problem-builder-5.1.3/problem_builder/public/css/problem-builder-edit.css`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/public/css/problem-builder.css` & `xblock-problem-builder-5.1.3/problem_builder/public/css/problem-builder.css`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/public/css/questionnaire-edit.css` & `xblock-problem-builder-5.1.3/problem_builder/public/css/questionnaire-edit.css`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/public/css/questionnaire.css` & `xblock-problem-builder-5.1.3/problem_builder/public/css/questionnaire.css`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/public/img/immunity-map-assumptions-bg.png` & `xblock-problem-builder-5.1.3/problem_builder/public/img/immunity-map-assumptions-bg.png`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/public/img/immunity-map-bg.png` & `xblock-problem-builder-5.1.3/problem_builder/public/img/immunity-map-bg.png`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/public/js/answer.js` & `xblock-problem-builder-5.1.3/problem_builder/public/js/answer.js`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/public/js/answer_recap.js` & `xblock-problem-builder-5.1.3/problem_builder/public/js/answer_recap.js`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/public/js/completion.js` & `xblock-problem-builder-5.1.3/problem_builder/public/js/completion.js`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/public/js/container_edit.js` & `xblock-problem-builder-5.1.3/problem_builder/public/js/container_edit.js`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/public/js/instructor_tool.js` & `xblock-problem-builder-5.1.3/problem_builder/public/js/instructor_tool.js`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/public/js/mentoring.js` & `xblock-problem-builder-5.1.3/problem_builder/public/js/mentoring.js`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/public/js/mentoring_edit.js` & `xblock-problem-builder-5.1.3/problem_builder/public/js/mentoring_edit.js`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/public/js/mentoring_standard_view.js` & `xblock-problem-builder-5.1.3/problem_builder/public/js/mentoring_standard_view.js`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/public/js/mentoring_with_steps.js` & `xblock-problem-builder-5.1.3/problem_builder/public/js/mentoring_with_steps.js`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/public/js/plot.js` & `xblock-problem-builder-5.1.3/problem_builder/public/js/plot.js`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/public/js/questionnaire.js` & `xblock-problem-builder-5.1.3/problem_builder/public/js/questionnaire.js`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/public/js/review_blocks.js` & `xblock-problem-builder-5.1.3/problem_builder/public/js/review_blocks.js`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/public/js/slider.js` & `xblock-problem-builder-5.1.3/problem_builder/public/js/slider.js`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/public/js/step.js` & `xblock-problem-builder-5.1.3/problem_builder/public/js/step.js`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/public/js/step_util.js` & `xblock-problem-builder-5.1.3/problem_builder/public/js/step_util.js`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/public/js/translations/ar/textjs.js` & `xblock-problem-builder-5.1.3/problem_builder/public/js/translations/ar/textjs.js`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/public/js/translations/de_DE/textjs.js` & `xblock-problem-builder-5.1.3/problem_builder/public/js/translations/de_DE/textjs.js`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/public/js/translations/en/textjs.js` & `xblock-problem-builder-5.1.3/problem_builder/public/js/translations/en/textjs.js`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/public/js/translations/eo/textjs.js` & `xblock-problem-builder-5.1.3/problem_builder/public/js/translations/eo/textjs.js`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/public/js/translations/es_419/textjs.js` & `xblock-problem-builder-5.1.3/problem_builder/public/js/translations/es_419/textjs.js`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/public/js/translations/fr/textjs.js` & `xblock-problem-builder-5.1.3/problem_builder/public/js/translations/fr/textjs.js`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/public/js/translations/fr_CA/textjs.js` & `xblock-problem-builder-5.1.3/problem_builder/public/js/translations/fr_CA/textjs.js`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/public/js/translations/ja_JP/textjs.js` & `xblock-problem-builder-5.1.3/problem_builder/public/js/translations/ja_JP/textjs.js`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/public/js/translations/ko_KR/textjs.js` & `xblock-problem-builder-5.1.3/problem_builder/public/js/translations/ko_KR/textjs.js`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/public/js/translations/pl_PL/textjs.js` & `xblock-problem-builder-5.1.3/problem_builder/public/js/translations/pl_PL/textjs.js`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/public/js/translations/pt_BR/textjs.js` & `xblock-problem-builder-5.1.3/problem_builder/public/js/translations/pt_BR/textjs.js`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/public/js/translations/zh_CN/textjs.js` & `xblock-problem-builder-5.1.3/problem_builder/public/js/translations/zh_CN/textjs.js`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/public/js/util.js` & `xblock-problem-builder-5.1.3/problem_builder/public/js/util.js`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/public/js/vendor/backbone-min.js` & `xblock-problem-builder-5.1.3/problem_builder/public/js/vendor/backbone-min.js`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/public/js/vendor/backbone.paginator.min.js` & `xblock-problem-builder-5.1.3/problem_builder/public/js/vendor/backbone.paginator.min.js`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/public/js/vendor/d3.min.js` & `xblock-problem-builder-5.1.3/problem_builder/public/js/vendor/d3.min.js`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/public/js/vendor/jquery-shorten.js` & `xblock-problem-builder-5.1.3/problem_builder/public/js/vendor/jquery-shorten.js`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/public/js/vendor/underscore-min.js` & `xblock-problem-builder-5.1.3/problem_builder/public/js/vendor/underscore-min.js`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/questionnaire.py` & `xblock-problem-builder-5.1.3/problem_builder/questionnaire.py`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/settings.py` & `xblock-problem-builder-5.1.3/problem_builder/settings.py`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/slider.py` & `xblock-problem-builder-5.1.3/problem_builder/slider.py`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/south_migrations/0001_initial.py` & `xblock-problem-builder-5.1.3/problem_builder/south_migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/south_migrations/0002_copy_from_mentoring.py` & `xblock-problem-builder-5.1.3/problem_builder/south_migrations/0002_copy_from_mentoring.py`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/south_migrations/0003_auto__add_share__add_unique_share_shared_by_shared_with_block_id.py` & `xblock-problem-builder-5.1.3/problem_builder/south_migrations/0003_auto__add_share__add_unique_share_shared_by_shared_with_block_id.py`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/step.py` & `xblock-problem-builder-5.1.3/problem_builder/step.py`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/step_review.py` & `xblock-problem-builder-5.1.3/problem_builder/step_review.py`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/sub_api.py` & `xblock-problem-builder-5.1.3/problem_builder/sub_api.py`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/swipe.py` & `xblock-problem-builder-5.1.3/problem_builder/swipe.py`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/table.py` & `xblock-problem-builder-5.1.3/problem_builder/table.py`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/tasks.py` & `xblock-problem-builder-5.1.3/problem_builder/tasks.py`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/templates/html/answer_editable.html` & `xblock-problem-builder-5.1.3/problem_builder/templates/html/answer_editable.html`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/templates/html/completion.html` & `xblock-problem-builder-5.1.3/problem_builder/templates/html/completion.html`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/templates/html/dashboard.html` & `xblock-problem-builder-5.1.3/problem_builder/templates/html/dashboard.html`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/templates/html/dashboard_report.html` & `xblock-problem-builder-5.1.3/problem_builder/templates/html/dashboard_report.html`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/templates/html/instructor_tool.html` & `xblock-problem-builder-5.1.3/problem_builder/templates/html/instructor_tool.html`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/templates/html/mcqblock.html` & `xblock-problem-builder-5.1.3/problem_builder/templates/html/mcqblock.html`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/templates/html/mentoring-table-container.html` & `xblock-problem-builder-5.1.3/problem_builder/templates/html/mentoring-table-container.html`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/templates/html/mentoring-table-report.html` & `xblock-problem-builder-5.1.3/problem_builder/templates/html/mentoring-table-report.html`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/templates/html/mentoring.html` & `xblock-problem-builder-5.1.3/problem_builder/templates/html/mentoring.html`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/templates/html/mentoring_with_steps.html` & `xblock-problem-builder-5.1.3/problem_builder/templates/html/mentoring_with_steps.html`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/templates/html/mrqblock.html` & `xblock-problem-builder-5.1.3/problem_builder/templates/html/mrqblock.html`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/templates/html/overlay.html` & `xblock-problem-builder-5.1.3/problem_builder/templates/html/overlay.html`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/templates/html/plot.html` & `xblock-problem-builder-5.1.3/problem_builder/templates/html/plot.html`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/templates/html/plot_preview.html` & `xblock-problem-builder-5.1.3/problem_builder/templates/html/plot_preview.html`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/templates/html/questionnaire_add_buttons.html` & `xblock-problem-builder-5.1.3/problem_builder/templates/html/questionnaire_add_buttons.html`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/templates/html/ratingblock.html` & `xblock-problem-builder-5.1.3/problem_builder/templates/html/ratingblock.html`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/templates/html/ratingblock_edit_preview.html` & `xblock-problem-builder-5.1.3/problem_builder/templates/html/ratingblock_edit_preview.html`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/templates/html/sb-review-score.html` & `xblock-problem-builder-5.1.3/problem_builder/templates/html/sb-review-score.html`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/templates/html/slider.html` & `xblock-problem-builder-5.1.3/problem_builder/templates/html/slider.html`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/templates/html/step.html` & `xblock-problem-builder-5.1.3/problem_builder/templates/html/step.html`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/templates/xml/mentoring_default.xml` & `xblock-problem-builder-5.1.3/problem_builder/templates/xml/mentoring_default.xml`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/templates/xml/mentoring_demo.xml` & `xblock-problem-builder-5.1.3/problem_builder/templates/xml/mentoring_demo.xml`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/templates/xml/mentoring_with_only_one_step.xml` & `xblock-problem-builder-5.1.3/problem_builder/templates/xml/mentoring_with_only_one_step.xml`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/tests/integration/base_test.py` & `xblock-problem-builder-5.1.3/problem_builder/tests/integration/base_test.py`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/tests/integration/test_answer.py` & `xblock-problem-builder-5.1.3/problem_builder/tests/integration/test_answer.py`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/tests/integration/test_author_changes.py` & `xblock-problem-builder-5.1.3/problem_builder/tests/integration/test_author_changes.py`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/tests/integration/test_clarifications.py` & `xblock-problem-builder-5.1.3/problem_builder/tests/integration/test_clarifications.py`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/tests/integration/test_completion.py` & `xblock-problem-builder-5.1.3/problem_builder/tests/integration/test_completion.py`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/tests/integration/test_dashboard.py` & `xblock-problem-builder-5.1.3/problem_builder/tests/integration/test_dashboard.py`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/tests/integration/test_instructor_tool.py` & `xblock-problem-builder-5.1.3/problem_builder/tests/integration/test_instructor_tool.py`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/tests/integration/test_mentoring.py` & `xblock-problem-builder-5.1.3/problem_builder/tests/integration/test_mentoring.py`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/tests/integration/test_messages.py` & `xblock-problem-builder-5.1.3/problem_builder/tests/integration/test_messages.py`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/tests/integration/test_multiple.py` & `xblock-problem-builder-5.1.3/problem_builder/tests/integration/test_multiple.py`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/tests/integration/test_progression.py` & `xblock-problem-builder-5.1.3/problem_builder/tests/integration/test_progression.py`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/tests/integration/test_questionnaire.py` & `xblock-problem-builder-5.1.3/problem_builder/tests/integration/test_questionnaire.py`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/tests/integration/test_slider.py` & `xblock-problem-builder-5.1.3/problem_builder/tests/integration/test_slider.py`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/tests/integration/test_step_builder.py` & `xblock-problem-builder-5.1.3/problem_builder/tests/integration/test_step_builder.py`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/tests/integration/test_table.py` & `xblock-problem-builder-5.1.3/problem_builder/tests/integration/test_table.py`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/tests/integration/test_titles.py` & `xblock-problem-builder-5.1.3/problem_builder/tests/integration/test_titles.py`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/tests/unit/test_answer_mixin.py` & `xblock-problem-builder-5.1.3/problem_builder/tests/unit/test_answer_mixin.py`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/tests/unit/test_common.py` & `xblock-problem-builder-5.1.3/problem_builder/tests/unit/test_common.py`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/tests/unit/test_dashboard_visual.py` & `xblock-problem-builder-5.1.3/problem_builder/tests/unit/test_dashboard_visual.py`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/tests/unit/test_instructor_tool.py` & `xblock-problem-builder-5.1.3/problem_builder/tests/unit/test_instructor_tool.py`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/tests/unit/test_migration.py` & `xblock-problem-builder-5.1.3/problem_builder/tests/unit/test_migration.py`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/tests/unit/test_mixins.py` & `xblock-problem-builder-5.1.3/problem_builder/tests/unit/test_mixins.py`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/tests/unit/test_models.py` & `xblock-problem-builder-5.1.3/problem_builder/tests/unit/test_models.py`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/tests/unit/test_problem_builder.py` & `xblock-problem-builder-5.1.3/problem_builder/tests/unit/test_problem_builder.py`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/tests/unit/test_step.py` & `xblock-problem-builder-5.1.3/problem_builder/tests/unit/test_step.py`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/tests/unit/test_step_builder.py` & `xblock-problem-builder-5.1.3/problem_builder/tests/unit/test_step_builder.py`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/tests/unit/test_swipe.py` & `xblock-problem-builder-5.1.3/problem_builder/tests/unit/test_swipe.py`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/tests/unit/utils.py` & `xblock-problem-builder-5.1.3/problem_builder/tests/unit/utils.py`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/tip.py` & `xblock-problem-builder-5.1.3/problem_builder/tip.py`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/translations/ar/LC_MESSAGES/text.mo` & `xblock-problem-builder-5.1.3/problem_builder/translations/ar/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/translations/ar/LC_MESSAGES/text.po` & `xblock-problem-builder-5.1.3/problem_builder/translations/ar/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/translations/ar/LC_MESSAGES/textjs.mo` & `xblock-problem-builder-5.1.3/problem_builder/translations/ar/LC_MESSAGES/textjs.mo`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/translations/ar/LC_MESSAGES/textjs.po` & `xblock-problem-builder-5.1.3/problem_builder/translations/ar/LC_MESSAGES/textjs.po`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/translations/config.yaml` & `xblock-problem-builder-5.1.3/problem_builder/translations/config.yaml`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/translations/de_DE/LC_MESSAGES/text.mo` & `xblock-problem-builder-5.1.3/problem_builder/translations/de_DE/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/translations/de_DE/LC_MESSAGES/text.po` & `xblock-problem-builder-5.1.3/problem_builder/translations/de_DE/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/translations/de_DE/LC_MESSAGES/textjs.mo` & `xblock-problem-builder-5.1.3/problem_builder/translations/de_DE/LC_MESSAGES/textjs.mo`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/translations/de_DE/LC_MESSAGES/textjs.po` & `xblock-problem-builder-5.1.3/problem_builder/translations/de_DE/LC_MESSAGES/textjs.po`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/translations/en/LC_MESSAGES/text.po` & `xblock-problem-builder-5.1.3/problem_builder/translations/en/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/translations/en/LC_MESSAGES/textjs.po` & `xblock-problem-builder-5.1.3/problem_builder/translations/en/LC_MESSAGES/textjs.po`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/translations/eo/LC_MESSAGES/text.mo` & `xblock-problem-builder-5.1.3/problem_builder/translations/eo/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/translations/eo/LC_MESSAGES/text.po` & `xblock-problem-builder-5.1.3/problem_builder/translations/eo/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/translations/eo/LC_MESSAGES/textjs.mo` & `xblock-problem-builder-5.1.3/problem_builder/translations/eo/LC_MESSAGES/textjs.mo`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/translations/eo/LC_MESSAGES/textjs.po` & `xblock-problem-builder-5.1.3/problem_builder/translations/eo/LC_MESSAGES/textjs.po`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/translations/es_419/LC_MESSAGES/text.mo` & `xblock-problem-builder-5.1.3/problem_builder/translations/es_419/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/translations/es_419/LC_MESSAGES/text.po` & `xblock-problem-builder-5.1.3/problem_builder/translations/es_419/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/translations/es_419/LC_MESSAGES/textjs.mo` & `xblock-problem-builder-5.1.3/problem_builder/translations/es_419/LC_MESSAGES/textjs.mo`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/translations/es_419/LC_MESSAGES/textjs.po` & `xblock-problem-builder-5.1.3/problem_builder/translations/es_419/LC_MESSAGES/textjs.po`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/translations/fr/LC_MESSAGES/text.mo` & `xblock-problem-builder-5.1.3/problem_builder/translations/fr/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/translations/fr/LC_MESSAGES/text.po` & `xblock-problem-builder-5.1.3/problem_builder/translations/fr/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/translations/fr/LC_MESSAGES/textjs.mo` & `xblock-problem-builder-5.1.3/problem_builder/translations/fr/LC_MESSAGES/textjs.mo`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/translations/fr/LC_MESSAGES/textjs.po` & `xblock-problem-builder-5.1.3/problem_builder/translations/fr/LC_MESSAGES/textjs.po`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/translations/fr_CA/LC_MESSAGES/text.mo` & `xblock-problem-builder-5.1.3/problem_builder/translations/fr_CA/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/translations/fr_CA/LC_MESSAGES/text.po` & `xblock-problem-builder-5.1.3/problem_builder/translations/fr_CA/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/translations/fr_CA/LC_MESSAGES/textjs.mo` & `xblock-problem-builder-5.1.3/problem_builder/translations/fr_CA/LC_MESSAGES/textjs.mo`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/translations/fr_CA/LC_MESSAGES/textjs.po` & `xblock-problem-builder-5.1.3/problem_builder/translations/fr_CA/LC_MESSAGES/textjs.po`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/translations/ja_JP/LC_MESSAGES/text.mo` & `xblock-problem-builder-5.1.3/problem_builder/translations/ja_JP/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/translations/ja_JP/LC_MESSAGES/text.po` & `xblock-problem-builder-5.1.3/problem_builder/translations/ja_JP/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/translations/ja_JP/LC_MESSAGES/textjs.mo` & `xblock-problem-builder-5.1.3/problem_builder/translations/ja_JP/LC_MESSAGES/textjs.mo`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/translations/ja_JP/LC_MESSAGES/textjs.po` & `xblock-problem-builder-5.1.3/problem_builder/translations/ja_JP/LC_MESSAGES/textjs.po`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/translations/ko_KR/LC_MESSAGES/text.mo` & `xblock-problem-builder-5.1.3/problem_builder/translations/ko_KR/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/translations/ko_KR/LC_MESSAGES/text.po` & `xblock-problem-builder-5.1.3/problem_builder/translations/ko_KR/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/translations/ko_KR/LC_MESSAGES/textjs.mo` & `xblock-problem-builder-5.1.3/problem_builder/translations/ko_KR/LC_MESSAGES/textjs.mo`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/translations/ko_KR/LC_MESSAGES/textjs.po` & `xblock-problem-builder-5.1.3/problem_builder/translations/ko_KR/LC_MESSAGES/textjs.po`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/translations/pl_PL/LC_MESSAGES/text.mo` & `xblock-problem-builder-5.1.3/problem_builder/translations/pl_PL/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/translations/pl_PL/LC_MESSAGES/text.po` & `xblock-problem-builder-5.1.3/problem_builder/translations/pl_PL/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/translations/pl_PL/LC_MESSAGES/textjs.mo` & `xblock-problem-builder-5.1.3/problem_builder/translations/pl_PL/LC_MESSAGES/textjs.mo`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/translations/pl_PL/LC_MESSAGES/textjs.po` & `xblock-problem-builder-5.1.3/problem_builder/translations/pl_PL/LC_MESSAGES/textjs.po`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/translations/pt_BR/LC_MESSAGES/text.mo` & `xblock-problem-builder-5.1.3/problem_builder/translations/pt_BR/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/translations/pt_BR/LC_MESSAGES/text.po` & `xblock-problem-builder-5.1.3/problem_builder/translations/pt_BR/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/translations/pt_BR/LC_MESSAGES/textjs.mo` & `xblock-problem-builder-5.1.3/problem_builder/translations/pt_BR/LC_MESSAGES/textjs.mo`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/translations/pt_BR/LC_MESSAGES/textjs.po` & `xblock-problem-builder-5.1.3/problem_builder/translations/pt_BR/LC_MESSAGES/textjs.po`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/translations/zh_CN/LC_MESSAGES/text.mo` & `xblock-problem-builder-5.1.3/problem_builder/translations/zh_CN/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/translations/zh_CN/LC_MESSAGES/text.po` & `xblock-problem-builder-5.1.3/problem_builder/translations/zh_CN/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/translations/zh_CN/LC_MESSAGES/textjs.mo` & `xblock-problem-builder-5.1.3/problem_builder/translations/zh_CN/LC_MESSAGES/textjs.mo`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/translations/zh_CN/LC_MESSAGES/textjs.po` & `xblock-problem-builder-5.1.3/problem_builder/translations/zh_CN/LC_MESSAGES/textjs.po`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/utils.py` & `xblock-problem-builder-5.1.3/problem_builder/utils.py`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/v1/studio_xml_utils.py` & `xblock-problem-builder-5.1.3/problem_builder/v1/studio_xml_utils.py`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/v1/upgrade.py` & `xblock-problem-builder-5.1.3/problem_builder/v1/upgrade.py`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/problem_builder/v1/xml_changes.py` & `xblock-problem-builder-5.1.3/problem_builder/v1/xml_changes.py`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/requirements/constraints.txt` & `xblock-problem-builder-5.1.3/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/setup.py` & `xblock-problem-builder-5.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/xblock_problem_builder.egg-info/PKG-INFO` & `xblock-problem-builder-5.1.3/xblock_problem_builder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xblock-problem-builder
-Version: 5.1.2
+Version: 5.1.3
 Summary: XBlock - Problem Builder
 Home-page: https://github.com/open-craft/problem-builder
 Author: OpenCraft
 License: AGPL v3
 Keywords: Python edx
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `xblock-problem-builder-5.1.2/xblock_problem_builder.egg-info/SOURCES.txt` & `xblock-problem-builder-5.1.3/xblock_problem_builder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `xblock-problem-builder-5.1.2/xblock_problem_builder.egg-info/entry_points.txt` & `xblock-problem-builder-5.1.3/xblock_problem_builder.egg-info/entry_points.txt`

 * *Files identical despite different names*

