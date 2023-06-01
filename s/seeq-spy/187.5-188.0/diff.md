# Comparing `tmp/seeq-spy-187.5.tar.gz` & `tmp/seeq-spy-188.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seeq-spy-187.5.tar", last modified: Wed May 17 17:45:36 2023, max compression
+gzip compressed data, was "dist\seeq-spy-188.0.tar", last modified: Thu Jun  1 20:00:55 2023, max compression
```

## Comparing `seeq-spy-187.5.tar` & `seeq-spy-188.0.tar`

### file list

```diff
@@ -1,151 +1,153 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 17:45:36.442211 seeq-spy-187.5/
--rw-rw-rw-   0        0        0    33551 2023-05-17 17:28:06.000000 seeq-spy-187.5/LICENSE
--rw-rw-rw-   0        0        0      207 2023-05-17 17:28:06.000000 seeq-spy-187.5/MANIFEST.in
--rw-rw-rw-   0        0        0     4606 2023-05-17 17:45:36.441209 seeq-spy-187.5/PKG-INFO
--rw-rw-rw-   0        0        0     4091 2023-05-17 17:28:06.000000 seeq-spy-187.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-17 17:45:35.109225 seeq-spy-187.5/seeq/
-drwxrwxrwx   0        0        0        0 2023-05-17 17:45:35.413213 seeq-spy-187.5/seeq/base/
--rw-rw-rw-   0        0        0       36 2023-05-17 17:45:24.000000 seeq-spy-187.5/seeq/base/__init__.py
--rw-rw-rw-   0        0        0      875 2023-05-17 17:45:24.000000 seeq-spy-187.5/seeq/base/proputil.py
--rw-rw-rw-   0        0        0    32236 2023-05-17 17:45:24.000000 seeq-spy-187.5/seeq/base/seeq_names.py
--rw-rw-rw-   0        0        0      157 2023-05-17 17:45:24.000000 seeq-spy-187.5/seeq/base/system.py
--rw-rw-rw-   0        0        0     4788 2023-05-17 17:45:24.000000 seeq-spy-187.5/seeq/base/util.py
-drwxrwxrwx   0        0        0        0 2023-05-17 17:45:35.414216 seeq-spy-187.5/seeq/scripts/
--rw-rw-rw-   0        0        0    12250 2023-05-17 17:45:24.000000 seeq-spy-187.5/seeq/scripts/create_monitoring_alerts.py
--rw-rw-rw-   0        0        0    49636 2023-05-17 17:45:24.000000 seeq-spy-187.5/seeq/scripts/create_monitoring_workbook.py
-drwxrwxrwx   0        0        0        0 2023-05-17 17:45:35.426215 seeq-spy-187.5/seeq/spy/
--rw-rw-rw-   0        0        0     1912 2023-05-17 17:45:33.000000 seeq-spy-187.5/seeq/spy/__init__.py
--rw-rw-rw-   0        0        0    30851 2023-05-17 17:45:33.000000 seeq-spy-187.5/seeq/spy/_common.py
--rw-rw-rw-   0        0        0     4687 2023-05-17 17:45:33.000000 seeq-spy-187.5/seeq/spy/_config.py
--rw-rw-rw-   0        0        0     4424 2023-05-17 17:45:33.000000 seeq-spy-187.5/seeq/spy/_datalab.py
--rw-rw-rw-   0        0        0     9686 2023-05-17 17:45:33.000000 seeq-spy-187.5/seeq/spy/_errors.py
--rw-rw-rw-   0        0        0    48955 2023-05-17 17:45:33.000000 seeq-spy-187.5/seeq/spy/_login.py
--rw-rw-rw-   0        0        0    92210 2023-05-17 17:45:33.000000 seeq-spy-187.5/seeq/spy/_metadata.py
--rw-rw-rw-   0        0        0     5822 2023-05-17 17:45:33.000000 seeq-spy-187.5/seeq/spy/_metadata_push_results.py
--rw-rw-rw-   0        0        0     2954 2023-05-17 17:45:33.000000 seeq-spy-187.5/seeq/spy/_plot.py
--rw-rw-rw-   0        0        0    55502 2023-05-17 17:45:33.000000 seeq-spy-187.5/seeq/spy/_pull.py
--rw-rw-rw-   0        0        0    68554 2023-05-17 17:45:33.000000 seeq-spy-187.5/seeq/spy/_push.py
--rw-rw-rw-   0        0        0     5155 2023-05-17 17:45:33.000000 seeq-spy-187.5/seeq/spy/_redaction.py
--rw-rw-rw-   0        0        0    41144 2023-05-17 17:45:33.000000 seeq-spy-187.5/seeq/spy/_search.py
--rw-rw-rw-   0        0        0    18978 2023-05-17 17:45:33.000000 seeq-spy-187.5/seeq/spy/_session.py
--rw-rw-rw-   0        0        0    15704 2023-05-17 17:45:33.000000 seeq-spy-187.5/seeq/spy/_status.py
--rw-rw-rw-   0        0        0     3471 2023-05-17 17:45:33.000000 seeq-spy-187.5/seeq/spy/_upgrade.py
--rw-rw-rw-   0        0        0    10707 2023-05-17 17:45:33.000000 seeq-spy-187.5/seeq/spy/_url.py
-drwxrwxrwx   0        0        0        0 2023-05-17 17:45:35.427219 seeq-spy-187.5/seeq/spy/acl/
--rw-rw-rw-   0        0        0      104 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/acl/__init__.py
--rw-rw-rw-   0        0        0    12125 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/acl/_pull.py
--rw-rw-rw-   0        0        0    11313 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/acl/_push.py
-drwxrwxrwx   0        0        0        0 2023-05-17 17:45:35.503212 seeq-spy-187.5/seeq/spy/addons/
--rw-rw-rw-   0        0        0      188 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/addons/__init__.py
--rw-rw-rw-   0        0        0    26338 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/addons/_install.py
--rw-rw-rw-   0        0        0     2408 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/addons/_permissions.py
--rw-rw-rw-   0        0        0    12099 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/addons/_search.py
--rw-rw-rw-   0        0        0     5296 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/addons/_uninstall.py
-drwxrwxrwx   0        0        0        0 2023-05-17 17:45:35.659217 seeq-spy-187.5/seeq/spy/assets/
--rw-rw-rw-   0        0        0      336 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/assets/__init__.py
--rw-rw-rw-   0        0        0     3638 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/assets/_brochure.py
--rw-rw-rw-   0        0        0    12106 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/assets/_build.py
--rw-rw-rw-   0        0        0     3133 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/assets/_context.py
--rw-rw-rw-   0        0        0    48189 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/assets/_model.py
-drwxrwxrwx   0        0        0        0 2023-05-17 17:45:35.816216 seeq-spy-187.5/seeq/spy/assets/_trees/
--rw-rw-rw-   0        0        0       69 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/assets/_trees/__init__.py
--rw-rw-rw-   0        0        0     1375 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/assets/_trees/_constants.py
--rw-rw-rw-   0        0        0     7302 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/assets/_trees/_csv.py
--rw-rw-rw-   0        0        0    22068 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/assets/_trees/_match.py
--rw-rw-rw-   0        0        0     2629 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/assets/_trees/_pandas.py
--rw-rw-rw-   0        0        0     6458 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/assets/_trees/_path.py
--rw-rw-rw-   0        0        0    23200 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/assets/_trees/_properties.py
--rw-rw-rw-   0        0        0    13341 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/assets/_trees/_pull.py
--rw-rw-rw-   0        0        0    58690 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/assets/_trees/_tree.py
--rw-rw-rw-   0        0        0     5885 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/assets/_trees/_utils.py
--rw-rw-rw-   0        0        0    25528 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/assets/_trees/_validate.py
--rw-rw-rw-   0        0        0     2538 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/assets/brochure.html
-drwxrwxrwx   0        0        0        0 2023-05-17 17:45:35.817210 seeq-spy-187.5/seeq/spy/docs/
-drwxrwxrwx   0        0        0        0 2023-05-17 17:45:35.917210 seeq-spy-187.5/seeq/spy/docs/Documentation/
-drwxrwxrwx   0        0        0        0 2023-05-17 17:45:35.919212 seeq-spy-187.5/seeq/spy/docs/Documentation/Administration/
--rw-rw-rw-   0        0        0     6702 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/docs/Documentation/Administration/User Migration.ipynb
-drwxrwxrwx   0        0        0        0 2023-05-17 17:45:36.114216 seeq-spy-187.5/seeq/spy/docs/Documentation/Advanced Scheduling/
--rw-rw-rw-   0        0        0    17428 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notification Add-on Installer.ipynb
--rw-rw-rw-   0        0        0    33412 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notification Scheduler.ipynb
--rw-rw-rw-   0        0        0    16700 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notifier.ipynb
--rw-rw-rw-   0        0        0     8406 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/docs/Documentation/Advanced Scheduling/Email Unsubscriber.ipynb
--rw-rw-rw-   0        0        0    38705 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/docs/Documentation/Advanced Scheduling/Parameterized Jobs.ipynb
--rw-rw-rw-   0        0        0      870 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/docs/Documentation/Advanced Scheduling/Seeq Data Lab.jpg
--rw-rw-rw-   0        0        0   184883 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/docs/Documentation/Asset Trees 1 - Introduction.ipynb
--rw-rw-rw-   0        0        0   222294 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/docs/Documentation/Asset Trees 2 - Templates.ipynb
--rw-rw-rw-   0        0        0   228823 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/docs/Documentation/Asset Trees 3 - Report and Dashboard Templates.ipynb
--rw-rw-rw-   0        0        0    24442 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/docs/Documentation/Asset Trees 4 - Accelerator Templates.ipynb
-drwxrwxrwx   0        0        0        0 2023-05-17 17:45:36.182202 seeq-spy-187.5/seeq/spy/docs/Documentation/Attached Images/
--rw-rw-rw-   0        0        0   135771 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot.jpg
--rw-rw-rw-   0        0        0   152116 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot2.jpg
--rw-rw-rw-   0        0        0   207271 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot3.jpg
--rw-rw-rw-   0        0        0      325 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/docs/Documentation/Attached Images/Readme.txt
--rw-rw-rw-   0        0        0   141516 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/docs/Documentation/Attached Images/ReportAndDashboardTemplates1.png
--rw-rw-rw-   0        0        0   439966 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/docs/Documentation/Attached Images/TopicTemplateScreenshot1.png
--rw-rw-rw-   0        0        0   189377 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/docs/Documentation/Attached Images/TopicTemplateScreenshot2.png
--rw-rw-rw-   0        0        0    15176 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/docs/Documentation/Command Reference.ipynb
-drwxrwxrwx   0        0        0        0 2023-05-17 17:45:36.286207 seeq-spy-187.5/seeq/spy/docs/Documentation/Support Files/
--rw-rw-rw-   0        0        0    94677 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/docs/Documentation/Support Files/Example Export.zip
--rw-rw-rw-   0        0        0   111771 2023-05-17 17:45:29.000000 seeq-spy-187.5/seeq/spy/docs/Documentation/Support Files/Report and Dashboard Templates.zip
--rw-rw-rw-   0        0        0   113084 2023-05-17 17:45:29.000000 seeq-spy-187.5/seeq/spy/docs/Documentation/Support Files/Workbook Templates.zip
--rw-rw-rw-   0        0        0  1083835 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/docs/Documentation/Support Files/csv_import_example.csv
--rw-rw-rw-   0        0        0      429 2023-05-17 17:45:29.000000 seeq-spy-187.5/seeq/spy/docs/Documentation/Support Files/spy_tree_example.csv
--rw-rw-rw-   0        0        0   673873 2023-05-17 17:45:29.000000 seeq-spy-187.5/seeq/spy/docs/Documentation/Tutorial.ipynb
--rw-rw-rw-   0        0        0    11411 2023-05-17 17:45:29.000000 seeq-spy-187.5/seeq/spy/docs/Documentation/Version Considerations.ipynb
--rw-rw-rw-   0        0        0  1556967 2023-05-17 17:45:29.000000 seeq-spy-187.5/seeq/spy/docs/Documentation/Workbook Templates.ipynb
--rw-rw-rw-   0        0        0    53885 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/docs/Documentation/spy.acl.ipynb
--rw-rw-rw-   0        0        0    11009 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/docs/Documentation/spy.jobs.ipynb
--rw-rw-rw-   0        0        0    12828 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/docs/Documentation/spy.login.ipynb
--rw-rw-rw-   0        0        0   127929 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/docs/Documentation/spy.pull.ipynb
--rw-rw-rw-   0        0        0    99356 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/docs/Documentation/spy.push.ipynb
--rw-rw-rw-   0        0        0    54441 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/docs/Documentation/spy.search.ipynb
--rw-rw-rw-   0        0        0    10645 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/docs/Documentation/spy.widgets.ipynb
--rw-rw-rw-   0        0        0    69641 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/docs/Documentation/spy.workbooks.ipynb
--rw-rw-rw-   0        0        0       60 2023-05-17 17:45:29.000000 seeq-spy-187.5/seeq/spy/docs/__init__.py
--rw-rw-rw-   0        0        0     1704 2023-05-17 17:45:29.000000 seeq-spy-187.5/seeq/spy/docs/_copy.py
-drwxrwxrwx   0        0        0        0 2023-05-17 17:45:36.292209 seeq-spy-187.5/seeq/spy/jobs/
--rw-rw-rw-   0        0        0      491 2023-05-17 17:45:29.000000 seeq-spy-187.5/seeq/spy/jobs/__init__.py
--rw-rw-rw-   0        0        0     9869 2023-05-17 17:45:29.000000 seeq-spy-187.5/seeq/spy/jobs/_execute.py
--rw-rw-rw-   0        0        0     6111 2023-05-17 17:45:29.000000 seeq-spy-187.5/seeq/spy/jobs/_pull.py
--rw-rw-rw-   0        0        0     9362 2023-05-17 17:45:29.000000 seeq-spy-187.5/seeq/spy/jobs/_push.py
--rw-rw-rw-   0        0        0    25680 2023-05-17 17:45:29.000000 seeq-spy-187.5/seeq/spy/jobs/_schedule.py
-drwxrwxrwx   0        0        0        0 2023-05-17 17:45:36.295206 seeq-spy-187.5/seeq/spy/notifications/
--rw-rw-rw-   0        0        0      153 2023-05-17 17:45:29.000000 seeq-spy-187.5/seeq/spy/notifications/__init__.py
--rw-rw-rw-   0        0        0    11926 2023-05-17 17:45:29.000000 seeq-spy-187.5/seeq/spy/notifications/_emails.py
-drwxrwxrwx   0        0        0        0 2023-05-17 17:45:36.297214 seeq-spy-187.5/seeq/spy/utils/
--rw-rw-rw-   0        0        0     1569 2023-05-17 17:45:29.000000 seeq-spy-187.5/seeq/spy/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 17:45:36.300207 seeq-spy-187.5/seeq/spy/widgets/
--rw-rw-rw-   0        0        0      200 2023-05-17 17:45:29.000000 seeq-spy-187.5/seeq/spy/widgets/__init__.py
--rw-rw-rw-   0        0        0     4158 2023-05-17 17:45:29.000000 seeq-spy-187.5/seeq/spy/widgets/_ipy_utils.py
--rw-rw-rw-   0        0        0    30480 2023-05-17 17:45:29.000000 seeq-spy-187.5/seeq/spy/widgets/_widgets.py
-drwxrwxrwx   0        0        0        0 2023-05-17 17:45:36.376205 seeq-spy-187.5/seeq/spy/workbooks/
--rw-rw-rw-   0        0        0     3012 2023-05-17 17:45:33.000000 seeq-spy-187.5/seeq/spy/workbooks/__init__.py
--rw-rw-rw-   0        0        0    43676 2023-05-17 17:45:33.000000 seeq-spy-187.5/seeq/spy/workbooks/_annotation.py
--rw-rw-rw-   0        0        0    34087 2023-05-17 17:45:33.000000 seeq-spy-187.5/seeq/spy/workbooks/_content.py
--rw-rw-rw-   0        0        0    40535 2023-05-17 17:45:33.000000 seeq-spy-187.5/seeq/spy/workbooks/_data.py
--rw-rw-rw-   0        0        0     6677 2023-05-17 17:45:33.000000 seeq-spy-187.5/seeq/spy/workbooks/_folder.py
--rw-rw-rw-   0        0        0    14959 2023-05-17 17:45:33.000000 seeq-spy-187.5/seeq/spy/workbooks/_item.py
--rw-rw-rw-   0        0        0     5448 2023-05-17 17:45:33.000000 seeq-spy-187.5/seeq/spy/workbooks/_item_map.py
--rw-rw-rw-   0        0        0     3033 2023-05-17 17:45:33.000000 seeq-spy-187.5/seeq/spy/workbooks/_load.py
--rw-rw-rw-   0        0        0     3456 2023-05-17 17:45:33.000000 seeq-spy-187.5/seeq/spy/workbooks/_mustache.py
--rw-rw-rw-   0        0        0    14137 2023-05-17 17:45:33.000000 seeq-spy-187.5/seeq/spy/workbooks/_pull.py
--rw-rw-rw-   0        0        0    23050 2023-05-17 17:45:33.000000 seeq-spy-187.5/seeq/spy/workbooks/_push.py
--rw-rw-rw-   0        0        0     6316 2023-05-17 17:45:33.000000 seeq-spy-187.5/seeq/spy/workbooks/_render.py
--rw-rw-rw-   0        0        0    27127 2023-05-17 17:45:33.000000 seeq-spy-187.5/seeq/spy/workbooks/_report_content_utilities.py
--rw-rw-rw-   0        0        0     4729 2023-05-17 17:45:33.000000 seeq-spy-187.5/seeq/spy/workbooks/_save.py
--rw-rw-rw-   0        0        0    15507 2023-05-17 17:45:33.000000 seeq-spy-187.5/seeq/spy/workbooks/_search.py
--rw-rw-rw-   0        0        0    37445 2023-05-17 17:45:33.000000 seeq-spy-187.5/seeq/spy/workbooks/_template.py
--rw-rw-rw-   0        0        0    11995 2023-05-17 17:45:33.000000 seeq-spy-187.5/seeq/spy/workbooks/_user.py
--rw-rw-rw-   0        0        0    52393 2023-05-17 17:45:33.000000 seeq-spy-187.5/seeq/spy/workbooks/_workbook.py
--rw-rw-rw-   0        0        0    48744 2023-05-17 17:45:33.000000 seeq-spy-187.5/seeq/spy/workbooks/_worksheet.py
--rw-rw-rw-   0        0        0    51518 2023-05-17 17:45:33.000000 seeq-spy-187.5/seeq/spy/workbooks/_workstep.py
--rw-rw-rw-   0        0        0   427362 2023-05-17 17:45:29.000000 seeq-spy-187.5/seeq/spy/workbooks/app.css
-drwxrwxrwx   0        0        0        0 2023-05-17 17:45:36.438218 seeq-spy-187.5/seeq_spy.egg-info/
--rw-rw-rw-   0        0        0     4606 2023-05-17 17:45:34.000000 seeq-spy-187.5/seeq_spy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4724 2023-05-17 17:45:34.000000 seeq-spy-187.5/seeq_spy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 17:45:34.000000 seeq-spy-187.5/seeq_spy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-17 17:45:34.000000 seeq-spy-187.5/seeq_spy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      311 2023-05-17 17:45:34.000000 seeq-spy-187.5/seeq_spy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-05-17 17:45:34.000000 seeq-spy-187.5/seeq_spy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-17 17:45:36.442211 seeq-spy-187.5/setup.cfg
--rw-rw-rw-   0        0        0     1677 2023-05-17 17:33:09.000000 seeq-spy-187.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 20:00:55.000000 seeq-spy-188.0/
+-rw-rw-rw-   0        0        0    33551 2023-03-17 02:53:52.000000 seeq-spy-188.0/LICENSE
+-rw-rw-rw-   0        0        0      207 2023-03-17 02:53:52.000000 seeq-spy-188.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4541 2023-06-01 20:00:55.000000 seeq-spy-188.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4026 2023-03-17 02:53:52.000000 seeq-spy-188.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 20:00:55.000000 seeq-spy-188.0/seeq/
+drwxrwxrwx   0        0        0        0 2023-06-01 20:00:55.000000 seeq-spy-188.0/seeq/base/
+-rw-rw-rw-   0        0        0       36 2023-06-01 20:00:52.000000 seeq-spy-188.0/seeq/base/__init__.py
+-rw-rw-rw-   0        0        0      875 2023-06-01 20:00:52.000000 seeq-spy-188.0/seeq/base/proputil.py
+-rw-rw-rw-   0        0        0    31475 2023-06-01 20:00:52.000000 seeq-spy-188.0/seeq/base/seeq_names.py
+-rw-rw-rw-   0        0        0    39742 2023-06-01 20:00:52.000000 seeq-spy-188.0/seeq/base/system.py
+-rw-rw-rw-   0        0        0     4788 2023-06-01 20:00:52.000000 seeq-spy-188.0/seeq/base/util.py
+drwxrwxrwx   0        0        0        0 2023-06-01 20:00:55.000000 seeq-spy-188.0/seeq/scripts/
+-rw-rw-rw-   0        0        0    12250 2023-06-01 20:00:52.000000 seeq-spy-188.0/seeq/scripts/create_monitoring_alerts.py
+-rw-rw-rw-   0        0        0    49636 2023-06-01 20:00:52.000000 seeq-spy-188.0/seeq/scripts/create_monitoring_workbook.py
+drwxrwxrwx   0        0        0        0 2023-06-01 20:00:55.000000 seeq-spy-188.0/seeq/spy/
+-rw-rw-rw-   0        0        0     1953 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/__init__.py
+-rw-rw-rw-   0        0        0    32016 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/_common.py
+-rw-rw-rw-   0        0        0     4687 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/_config.py
+-rw-rw-rw-   0        0        0     4424 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/_datalab.py
+-rw-rw-rw-   0        0        0     9686 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/_errors.py
+-rw-rw-rw-   0        0        0    48958 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/_login.py
+-rw-rw-rw-   0        0        0    92228 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/_metadata.py
+-rw-rw-rw-   0        0        0     5822 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/_metadata_push_results.py
+-rw-rw-rw-   0        0        0     2954 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/_plot.py
+-rw-rw-rw-   0        0        0    55589 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/_pull.py
+-rw-rw-rw-   0        0        0    68798 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/_push.py
+-rw-rw-rw-   0        0        0     5155 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/_redaction.py
+-rw-rw-rw-   0        0        0    44683 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/_search.py
+-rw-rw-rw-   0        0        0    20309 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/_session.py
+-rw-rw-rw-   0        0        0    15704 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/_status.py
+-rw-rw-rw-   0        0        0    20620 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/_swap.py
+-rw-rw-rw-   0        0        0     3471 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/_upgrade.py
+-rw-rw-rw-   0        0        0    10707 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/_url.py
+drwxrwxrwx   0        0        0        0 2023-06-01 20:00:55.000000 seeq-spy-188.0/seeq/spy/acl/
+-rw-rw-rw-   0        0        0      104 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/acl/__init__.py
+-rw-rw-rw-   0        0        0    12126 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/acl/_pull.py
+-rw-rw-rw-   0        0        0    11314 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/acl/_push.py
+drwxrwxrwx   0        0        0        0 2023-06-01 20:00:55.000000 seeq-spy-188.0/seeq/spy/addons/
+-rw-rw-rw-   0        0        0      188 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/addons/__init__.py
+-rw-rw-rw-   0        0        0    26339 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/addons/_install.py
+-rw-rw-rw-   0        0        0     2408 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/addons/_permissions.py
+-rw-rw-rw-   0        0        0    12100 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/addons/_search.py
+-rw-rw-rw-   0        0        0     5297 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/addons/_uninstall.py
+drwxrwxrwx   0        0        0        0 2023-06-01 20:00:55.000000 seeq-spy-188.0/seeq/spy/assets/
+-rw-rw-rw-   0        0        0      336 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/assets/__init__.py
+-rw-rw-rw-   0        0        0     3638 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/assets/_brochure.py
+-rw-rw-rw-   0        0        0    12369 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/assets/_build.py
+-rw-rw-rw-   0        0        0     3133 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/assets/_context.py
+-rw-rw-rw-   0        0        0    48189 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/assets/_model.py
+drwxrwxrwx   0        0        0        0 2023-06-01 20:00:55.000000 seeq-spy-188.0/seeq/spy/assets/_trees/
+-rw-rw-rw-   0        0        0       69 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/assets/_trees/__init__.py
+-rw-rw-rw-   0        0        0     1375 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/assets/_trees/_constants.py
+-rw-rw-rw-   0        0        0     7325 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/assets/_trees/_csv.py
+-rw-rw-rw-   0        0        0    22068 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/assets/_trees/_match.py
+-rw-rw-rw-   0        0        0     2629 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/assets/_trees/_pandas.py
+-rw-rw-rw-   0        0        0     6458 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/assets/_trees/_path.py
+-rw-rw-rw-   0        0        0    23200 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/assets/_trees/_properties.py
+-rw-rw-rw-   0        0        0    13389 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/assets/_trees/_pull.py
+-rw-rw-rw-   0        0        0    59025 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/assets/_trees/_tree.py
+-rw-rw-rw-   0        0        0     5885 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/assets/_trees/_utils.py
+-rw-rw-rw-   0        0        0    25528 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/assets/_trees/_validate.py
+-rw-rw-rw-   0        0        0     2538 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/assets/brochure.html
+drwxrwxrwx   0        0        0        0 2023-06-01 20:00:55.000000 seeq-spy-188.0/seeq/spy/docs/
+drwxrwxrwx   0        0        0        0 2023-06-01 20:00:55.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/
+drwxrwxrwx   0        0        0        0 2023-06-01 20:00:55.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/Administration/
+-rw-rw-rw-   0        0        0     6577 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/Administration/User Migration.ipynb
+drwxrwxrwx   0        0        0        0 2023-06-01 20:00:55.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/Advanced Scheduling/
+-rw-rw-rw-   0        0        0    17428 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notification Add-on Installer.ipynb
+-rw-rw-rw-   0        0        0    33412 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notification Scheduler.ipynb
+-rw-rw-rw-   0        0        0    16700 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notifier.ipynb
+-rw-rw-rw-   0        0        0     8406 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/Advanced Scheduling/Email Unsubscriber.ipynb
+-rw-rw-rw-   0        0        0    38889 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/Advanced Scheduling/Parameterized Jobs.ipynb
+-rw-rw-rw-   0        0        0      870 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/Advanced Scheduling/Seeq Data Lab.jpg
+-rw-rw-rw-   0        0        0   186560 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/Asset Trees 1 - Introduction.ipynb
+-rw-rw-rw-   0        0        0   239024 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/Asset Trees 2 - Templates.ipynb
+-rw-rw-rw-   0        0        0   229026 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/Asset Trees 3 - Report and Dashboard Templates.ipynb
+-rw-rw-rw-   0        0        0    24627 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/Asset Trees 4 - Accelerator Templates.ipynb
+drwxrwxrwx   0        0        0        0 2023-06-01 20:00:55.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/Attached Images/
+-rw-rw-rw-   0        0        0   135771 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot.jpg
+-rw-rw-rw-   0        0        0   152116 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot2.jpg
+-rw-rw-rw-   0        0        0   207271 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot3.jpg
+-rw-rw-rw-   0        0        0      325 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/Attached Images/Readme.txt
+-rw-rw-rw-   0        0        0   141516 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/Attached Images/ReportAndDashboardTemplates1.png
+-rw-rw-rw-   0        0        0   439966 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/Attached Images/TopicTemplateScreenshot1.png
+-rw-rw-rw-   0        0        0   189377 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/Attached Images/TopicTemplateScreenshot2.png
+-rw-rw-rw-   0        0        0    15177 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/Command Reference.ipynb
+drwxrwxrwx   0        0        0        0 2023-06-01 20:00:55.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/Support Files/
+-rw-rw-rw-   0        0        0    94677 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/Support Files/Example Export.zip
+-rw-rw-rw-   0        0        0   111771 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/Support Files/Report and Dashboard Templates.zip
+-rw-rw-rw-   0        0        0   113084 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/Support Files/Workbook Templates.zip
+-rw-rw-rw-   0        0        0  1083835 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/Support Files/csv_import_example.csv
+-rw-rw-rw-   0        0        0      429 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/Support Files/spy_tree_example.csv
+-rw-rw-rw-   0        0        0   674467 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/Tutorial.ipynb
+-rw-rw-rw-   0        0        0    11595 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/Version Considerations.ipynb
+-rw-rw-rw-   0        0        0  1557151 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/Workbook Templates.ipynb
+-rw-rw-rw-   0        0        0    54071 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/spy.acl.ipynb
+-rw-rw-rw-   0        0        0    11195 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/spy.jobs.ipynb
+-rw-rw-rw-   0        0        0    13015 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/spy.login.ipynb
+-rw-rw-rw-   0        0        0   128103 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/spy.pull.ipynb
+-rw-rw-rw-   0        0        0    99541 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/spy.push.ipynb
+-rw-rw-rw-   0        0        0    57289 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/spy.search.ipynb
+-rw-rw-rw-   0        0        0    95777 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/spy.swap.ipynb
+-rw-rw-rw-   0        0        0    10829 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/spy.widgets.ipynb
+-rw-rw-rw-   0        0        0    69828 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/spy.workbooks.ipynb
+-rw-rw-rw-   0        0        0       60 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/__init__.py
+-rw-rw-rw-   0        0        0     1704 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/_copy.py
+drwxrwxrwx   0        0        0        0 2023-06-01 20:00:55.000000 seeq-spy-188.0/seeq/spy/jobs/
+-rw-rw-rw-   0        0        0      491 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/jobs/__init__.py
+-rw-rw-rw-   0        0        0     9869 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/jobs/_execute.py
+-rw-rw-rw-   0        0        0     6111 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/jobs/_pull.py
+-rw-rw-rw-   0        0        0     9363 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/jobs/_push.py
+-rw-rw-rw-   0        0        0    25686 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/jobs/_schedule.py
+drwxrwxrwx   0        0        0        0 2023-06-01 20:00:55.000000 seeq-spy-188.0/seeq/spy/notifications/
+-rw-rw-rw-   0        0        0      153 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/notifications/__init__.py
+-rw-rw-rw-   0        0        0    11927 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/notifications/_emails.py
+drwxrwxrwx   0        0        0        0 2023-06-01 20:00:55.000000 seeq-spy-188.0/seeq/spy/utils/
+-rw-rw-rw-   0        0        0     1569 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 20:00:55.000000 seeq-spy-188.0/seeq/spy/widgets/
+-rw-rw-rw-   0        0        0      200 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/widgets/__init__.py
+-rw-rw-rw-   0        0        0     4158 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/widgets/_ipy_utils.py
+-rw-rw-rw-   0        0        0    30480 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/widgets/_widgets.py
+drwxrwxrwx   0        0        0        0 2023-06-01 20:00:55.000000 seeq-spy-188.0/seeq/spy/workbooks/
+-rw-rw-rw-   0        0        0     3012 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/workbooks/__init__.py
+-rw-rw-rw-   0        0        0    43729 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/workbooks/_annotation.py
+-rw-rw-rw-   0        0        0    34087 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/workbooks/_content.py
+-rw-rw-rw-   0        0        0    40974 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/workbooks/_data.py
+-rw-rw-rw-   0        0        0     6639 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/workbooks/_folder.py
+-rw-rw-rw-   0        0        0    14611 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/workbooks/_item.py
+-rw-rw-rw-   0        0        0     5448 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/workbooks/_item_map.py
+-rw-rw-rw-   0        0        0     3033 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/workbooks/_load.py
+-rw-rw-rw-   0        0        0     3456 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/workbooks/_mustache.py
+-rw-rw-rw-   0        0        0    14138 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/workbooks/_pull.py
+-rw-rw-rw-   0        0        0    23051 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/workbooks/_push.py
+-rw-rw-rw-   0        0        0     6316 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/workbooks/_render.py
+-rw-rw-rw-   0        0        0    27127 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/workbooks/_report_content_utilities.py
+-rw-rw-rw-   0        0        0     4729 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/workbooks/_save.py
+-rw-rw-rw-   0        0        0    15508 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/workbooks/_search.py
+-rw-rw-rw-   0        0        0    37445 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/workbooks/_template.py
+-rw-rw-rw-   0        0        0    11995 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/workbooks/_user.py
+-rw-rw-rw-   0        0        0    52462 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/workbooks/_workbook.py
+-rw-rw-rw-   0        0        0    48819 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/workbooks/_worksheet.py
+-rw-rw-rw-   0        0        0    51518 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/workbooks/_workstep.py
+-rw-rw-rw-   0        0        0   427362 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/workbooks/app.css
+drwxrwxrwx   0        0        0        0 2023-06-01 20:00:55.000000 seeq-spy-188.0/seeq_spy.egg-info/
+-rw-rw-rw-   0        0        0     4541 2023-06-01 20:00:55.000000 seeq-spy-188.0/seeq_spy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4785 2023-06-01 20:00:55.000000 seeq-spy-188.0/seeq_spy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 20:00:55.000000 seeq-spy-188.0/seeq_spy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-05 20:35:05.000000 seeq-spy-188.0/seeq_spy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      311 2023-06-01 20:00:55.000000 seeq-spy-188.0/seeq_spy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-01 20:00:55.000000 seeq-spy-188.0/seeq_spy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 20:00:55.000000 seeq-spy-188.0/setup.cfg
+-rw-rw-rw-   0        0        0     1677 2023-06-01 19:56:18.000000 seeq-spy-188.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `seeq-spy-187.5/LICENSE` & `seeq-spy-188.0/LICENSE`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.5/PKG-INFO` & `seeq-spy-188.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seeq-spy
-Version: 187.5
+Version: 188.0
 Summary: Easy-to-use Python interface for Seeq
 Home-page: https://www.seeq.com
 Author: Seeq Corporation
 Author-email: support@seeq.com
 Project-URL: Documentation, https://python-docs.seeq.com/
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
@@ -31,16 +31,14 @@
 - Import data in a programmatic way (when Seeq Workbench's *CSV Import* capability won't cut it)
 - Calculate new data in Python and push it into Seeq
 - Create an asset model
 - Programmatically create and manipulate Workbench Analyses or Organizer Topics
 
 **Use of the SPy module requires Python 3.7 or later.**
 
-**SPy version 187 and higher is compatible with Pandas 2.x.**
-
 To start exploring the SPy module, execute the following lines of code in Jupyter:
 
 ```
 from seeq import spy
 spy.docs.copy()
 ```
```

### Comparing `seeq-spy-187.5/README.md` & `seeq-spy-188.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,14 @@
 - Import data in a programmatic way (when Seeq Workbench's *CSV Import* capability won't cut it)
 - Calculate new data in Python and push it into Seeq
 - Create an asset model
 - Programmatically create and manipulate Workbench Analyses or Organizer Topics
 
 **Use of the SPy module requires Python 3.7 or later.**
 
-**SPy version 187 and higher is compatible with Pandas 2.x.**
-
 To start exploring the SPy module, execute the following lines of code in Jupyter:
 
 ```
 from seeq import spy
 spy.docs.copy()
 ```
```

### Comparing `seeq-spy-187.5/seeq/base/proputil.py` & `seeq-spy-188.0/seeq/base/proputil.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.5/seeq/base/seeq_names.py` & `seeq-spy-188.0/seeq/base/seeq_names.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,23 +8,16 @@
 class SeeqNames:
     class Database:
         class Schemas:
             materialized_tables = 'materialized_tables'
         
     
     class MaterializedTables:
-        datum_id_column = 'datum id'
-        item_id_column = 'item id'
-        class Rules:
-            ancestor = 'ancestor'
-            concat_columns = 'concatColumns'
-            event_property = 'eventProperty'
-            item_property = 'itemProperty'
-            path = 'path'
-        
+        datum_id_column = 'datum_id'
+        item_id_column = 'item_id'
     
     class Injection:
         everyone_user_group = 'EveryoneUserGroup'
         system_state = 'SystemState'
         system_user = 'SystemUser'
     
     class Connectors:
@@ -229,17 +222,15 @@
         content = 'Content'
         report_templates = 'ReportTemplates'
         condition_monitors = 'ConditionMonitors'
         plugins = 'Plugins'
         displays = 'Displays'
         display_templates = 'DisplayTemplates'
         notification_configurations = 'NotificationConfigurations'
-        context = 'Context'
         table_definitions = 'TableDefinitions'
-        graph_q_l = 'GraphQL'
     
     class Channels:
         agents_status = 'agents-status'
         datasources_status = 'datasources-status'
         broadcast = 'broadcast'
         live_screenshot = 'live-screenshot'
         async_response = 'async-response'
@@ -307,18 +298,15 @@
         date_ranges = '/date-ranges'
         asset_selections = '/asset-selections'
         plugins = '/plugins'
         displays = '/displays'
         display_templates = '/display-templates'
         usage = '/usage'
         notification_configurations = '/notification-configurations'
-        labels = '/labels'
-        context = '/context'
         table_definitions = '/table-definitions'
-        graph_q_l = '/graphql'
         class ErrorMessages:
             attempted_to_set_scope_on_a_globally_scoped_item = 'Attempted to set scope on a globally scoped item'
         
         class AddOnToolLinkType:
             window = 'window'
             tab = 'tab'
             none = 'none'
@@ -376,19 +364,14 @@
                 cache_capsules_read = 'Cache Capsules Read'
                 cache_in_memory_samples_read = 'Cache In-Memory Samples Read'
                 cache_in_memory_capsules_read = 'Cache In-Memory Capsules Read'
                 database_items_read = 'Database Items Read'
                 database_relationships_read = 'Database Relationships Read'
             
         
-        class Flags:
-            all_properties = '@allProperties'
-            exclude_globally_scoped = '@excludeGloballyScoped'
-            include_unsearchable = '@includeUnsearchable'
-        
     
     class UnitTest:
         timestamp1 = '1990-03-07T09:58:20.888888Z'
         timestamp2 = '1990-04-08T10:59:21.999999Z'
         non_existent_guid = '1CB64296-FC3E-4221-9A7F-947A0AB99807'
     
     class Edges:
@@ -461,15 +444,14 @@
         project_link = 'ProjectLink'
         add_on_tool = 'AddOnTool'
         base_annotation = 'BaseAnnotation'
         report = 'Report'
         report_template = 'ReportTemplate'
         journal = 'Journal'
         reply = 'Reply'
-        item_finder = 'ItemFinder'
         condition = 'Condition'
         condition_monitor = 'ConditionMonitor'
         capsule = 'Capsule'
         stored_condition = 'StoredCondition'
         calculated_condition = 'CalculatedCondition'
         scalar = 'ScalarItem'
         literal_scalar = 'LiteralScalar'
@@ -556,15 +538,14 @@
         archived_reason = 'Archived Reason'
         sync_token = 'Sync Token'
         number_format = 'Number Format'
         source_number_format = 'Source Number Format'
         string_format = 'String Format'
         source_string_format = 'Source String Format'
         storage_location = 'Storage Location'
-        executor_id = 'Executor ID'
         creator_id = 'Creator ID'
         creator_first_name = 'Creator First Name'
         creator_last_name = 'Creator Last Name'
         historical_data_version = 'Historical Data Version'
         manual_cdc = 'Manual CDC'
         scoped_to = 'Scoped To'
         asset = 'asset'
@@ -616,15 +597,15 @@
         previous_index_at = 'Previous Index At'
         sync_result = 'Sync Result'
         indexing_schedule_supported = 'Indexing Schedule Supported'
         asset_tree_search_index_needs_updating = 'Asset Tree Search Index Needs Updating'
         sync_mode = 'Sync Mode'
         items_archived_count = 'Items Archived Count'
         indexing_duration = 'Indexing Duration'
-        indexing_progress_timestamp = 'Indexing Progress Timestamp'
+        current_indexing_started_at = 'Current Indexing Started At'
         asset_progress = 'Asset Progress'
         asset_count = 'Asset Count'
         previous_asset_count = 'Previous Asset Count'
         signal_progress = 'Signal Progress'
         signal_count = 'Signal Count'
         previous_signal_count = 'Previous Signal Count'
         condition_progress = 'Condition Progress'
@@ -745,16 +726,14 @@
         summary_value = 'Summary Value'
         current_filename = 'Current Filename'
         last_result_hash = 'Last Result Hash'
         asset_path_depth = 'Asset Path Depth'
         last_run_at = 'Last Run At'
         last_run_state = 'Last Run State'
         query_range_look_ahead = 'Query Range Look Ahead'
-        finder_configurations = 'Finder Configurations'
-        last_run_warnings = 'Last Run Warnings'
         resource_size = 'Resource Size'
         project_type = 'Project Type'
         cron_schedule = 'Cron Schedule'
         background = 'Background'
         condition_formula_now = 'Condition Formula Now'
         notebook_path = 'Notebook Path'
         previous_run_time = 'Previous Run Time'
```

### Comparing `seeq-spy-187.5/seeq/base/util.py` & `seeq-spy-188.0/seeq/base/util.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.5/seeq/scripts/create_monitoring_alerts.py` & `seeq-spy-188.0/seeq/scripts/create_monitoring_alerts.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.5/seeq/scripts/create_monitoring_workbook.py` & `seeq-spy-188.0/seeq/scripts/create_monitoring_workbook.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.5/seeq/spy/__init__.py` & `seeq-spy-188.0/seeq/spy/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from seeq.spy._login import login, logout
 from seeq.spy._plot import plot
 from seeq.spy._pull import pull
 from seeq.spy._push import push
 from seeq.spy._search import search
 from seeq.spy._session import Session, Options
 from seeq.spy._status import Status
+from seeq.spy._swap import swap
 from seeq.spy._upgrade import upgrade
 
 # noinspection DuplicatedCode
 session: Session = Session(client_configuration=Configuration())
 """
 The default session used by SPy functions that interact with Seeq Server
 """
@@ -49,12 +50,12 @@
 
 server_version: Optional[str] = None
 """
 Equivalent to `spy.session.server_version`
 """
 
 __all__ = ['acl', 'addons', 'assets', 'docs', 'workbooks', 'widgets', 'login', 'logout', 'plot', 'pull', 'push',
-           'search', 'PATH_ROOT', 'DEFAULT_WORKBOOK_PATH', 'GLOBALS_ONLY', 'GLOBALS_AND_ALL_WORKBOOKS',
+           'search', 'swap', 'PATH_ROOT', 'DEFAULT_WORKBOOK_PATH', 'GLOBALS_ONLY', 'GLOBALS_AND_ALL_WORKBOOKS',
            'INHERIT_FROM_WORKBOOK', 'Session', 'Status', 'options', 'session', 'client', 'user', 'server_version',
            'jobs', 'notifications', 'upgrade', 'utils', 'errors']
 
-__version__ = '%d.%d' % (int('187'), int('5'))
+__version__ = '%d.%d' % (int('188'), int('0'))
```

### Comparing `seeq-spy-187.5/seeq/spy/_common.py` & `seeq-spy-188.0/seeq/spy/_common.py`

 * *Files 2% similar despite different names*

```diff
@@ -703,14 +703,48 @@
     return re.split(r'\s*>>\s*', path_string.strip())
 
 
 def path_list_to_string(path_list):
     return ' >> '.join(path_list)
 
 
+def resolve_old_asset_format_arg(old_asset_format_arg, df):
+    if old_asset_format_arg is None:
+        old_asset_format_arg = True
+        if hasattr(df, 'spy') and hasattr(df.spy, 'old_asset_format'):
+            old_asset_format_arg = df.spy.old_asset_format
+
+    return old_asset_format_arg
+
+
+def add_ancestors_to_definition(item_type, name, ancestors, definition, old_asset_format):
+    if item_type == 'Asset' and not old_asset_format:
+        definition['Path'] = path_list_to_string(ancestors)
+        definition['Asset'] = name
+    else:
+        if len(ancestors) > 1:
+            definition['Path'] = path_list_to_string(ancestors[0:-1])
+            definition['Asset'] = ancestors[-1]
+        elif len(ancestors) == 1:
+            definition['Path'] = None
+            definition['Asset'] = ancestors[0]
+
+
+def fqn_from_row(row):
+    parts = list()
+    if present(row, 'Path'):
+        parts.append(get(row, 'Path'))
+    if get(row, 'Type') != 'Asset' and present(row, 'Asset'):
+        parts.append(get(row, 'Asset'))
+    if present(row, 'Name'):
+        parts.append(get(row, 'Name'))
+
+    return ' >> '.join(parts)
+
+
 def sanitize_path_string(path):
     return path_list_to_string(path_string_to_list(path))
 
 
 def string_to_formula_literal(s):
     if not isinstance(s, str):
         raise ValueError('Argument must be a string')
```

### Comparing `seeq-spy-187.5/seeq/spy/_config.py` & `seeq-spy-188.0/seeq/spy/_config.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.5/seeq/spy/_datalab.py` & `seeq-spy-188.0/seeq/spy/_datalab.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.5/seeq/spy/_errors.py` & `seeq-spy-188.0/seeq/spy/_errors.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.5/seeq/spy/_login.py` & `seeq-spy-188.0/seeq/spy/_login.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
         login if already logged in. You should include a spy.login(force=False)
         cell if you are creating example notebooks that may be used in Jupyter
         environments like Anaconda, AWS SageMaker or Azure Notebooks.)
 
     quiet : bool, default False
         If True, suppresses progress output. Note that when status is
         provided, the quiet setting of the Status object that is passed
-        in takes precedent.
+        in takes precedence.
 
     status : spy.Status, optional
         If supplied, this Status object will be updated as the command
         progresses.
 
     session : spy.Session, optional
         If supplied, the Session object (and its Options) will be used to
@@ -434,15 +434,15 @@
 
     Parameters
     ----------
 
     quiet : bool, default False
         If True, suppresses progress output. Note that when status is
         provided, the quiet setting of the Status object that is passed
-        in takes precedent.
+        in takes precedence.
 
     status : spy.Status, optional
         If supplied, this Status object will be updated as the command
         progresses.
 
     session : spy.Session, optional
         The login session to use for this call. See spy.login() documentation
@@ -464,15 +464,15 @@
 
     Parameters
     ----------
 
     quiet : bool
         If True, suppresses progress output. Note that when status is
         provided, the quiet setting of the Status object that is passed
-        in takes precedent.
+        in takes precedence.
 
     status : spy.Status, optional
         If supplied, this Status object will be updated as the command
         progresses.
 
     session : spy.Session, optional
         The login session to use for this call. See spy.login() documentation
```

### Comparing `seeq-spy-187.5/seeq/spy/_metadata.py` & `seeq-spy-188.0/seeq/spy/_metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import os
 import re
 from dataclasses import dataclass
 from typing import Callable, Dict, Optional, List, Tuple, Set
 
 import numpy as np
 import pandas as pd
-
 from seeq.base.seeq_names import SeeqNames
 from seeq.sdk import *
 from seeq.spy import _common, _login
 from seeq.spy._common import EMPTY_GUID
 from seeq.spy._errors import *
 from seeq.spy._metadata_push_results import PushResults
 from seeq.spy._push import WorkbookContext
@@ -1901,15 +1900,15 @@
 
 RESERVED_SPY_COLUMN_NAMES = [
                                 'Build Path', 'Build Asset', 'Build Template',
                                 'ID', 'Type', 'Path', 'Asset', 'Object', 'Asset Object', 'Depth',
                                 'Formula Parameters', 'Capsule Is Uncertain', 'Capsule Property Units',
                                 'Override Number Format', 'Condition',
                                 'Permissions Inheritance Disabled', 'Access Control',
-                                'Roll Up Statistic', 'Roll Up Parameters',
+                                'Roll Up Statistic', 'Roll Up Parameters', 'Old Asset Format',
                                 'Template ID', 'Swap Out Asset ID', 'Swap In Asset ID', 'Source Workstep ID'
                             ] + RESERVED_SPY_STATUS_COLUMN_NAMES
 
 # Properties that will not be supplied via the "additionalProperties" field.
 # This must be kept in sync with RESERVED_ITEM_PROPERTIES in StoredItemOutput.java
 RESERVED_ITEM_PROPERTIES = [
     SeeqNames.Properties.guid,
```

### Comparing `seeq-spy-187.5/seeq/spy/_metadata_push_results.py` & `seeq-spy-188.0/seeq/spy/_metadata_push_results.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.5/seeq/spy/_plot.py` & `seeq-spy-188.0/seeq/spy/_plot.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.5/seeq/spy/_pull.py` & `seeq-spy-188.0/seeq/spy/_pull.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,25 +34,25 @@
     ----------
     items : {str, pd.DataFrame, pd.Series}
         A DataFrame or Series containing ID and Type columns that can be used
         to identify the items to pull. This is usually created via a call to
         spy.search(). Alternatively, you can supply URL of a Seeq Workbench
         worksheet as a str.
 
-    start : {str, pd.Timestamp}
+    start : {str, pd.Timestamp}, optional
         The starting time for which to pull data. This argument must be a
         string that pandas.to_datetime() can parse, or a pandas.Timestamp.
         If not provided, 'start' will default to 'end' minus 1 hour. Note
         that Seeq will potentially return one additional row that is earlier
         than this time (if it exists), as a "bounding value" for interpolation
         purposes. If both 'start' and 'end' are not provided and items
         is a str, 'start' will default to the start of the display range
         in Seeq Trend View.
 
-    end : {str, pd.Timestamp}
+    end : {str, pd.Timestamp}, optional
         The end time for which to pull data. This argument must be a string
         that pandas.to_datetime() can parse, or a pandas.Timestamp.
         If not provided, 'end' will default to now. Note that Seeq will
         potentially return one additional row that is later than this time
         (if it exists), as a "bounding value" for interpolation purposes.
         If both 'start' and 'end' are not provided and items is a str,
         'end' will default to the end of the display range in Seeq Trend View.
@@ -70,43 +70,43 @@
         If grid='auto' and the 'Estimated Sample Period' column does not exist
         in 'items', additional queries will be made to estimate the sample period
         which could potentially impact performance for large pulls. Interpolation
         is either linear or step and is set per signal at the time of the signal's
         creation. To change the interpolation type for a given signal, change the
         signal's interpolation or use the appropriate 'calculation' argument.
 
-    header : str default '__auto__'
+    header : str, default '__auto__'
         The metadata property to use as the header of each column. Common
         values would be 'ID' or 'Name'. '__auto__' concatenates Path and Name
         if they are present.
 
-    group_by : {str, list(str)}
+    group_by : {str, list(str)}, optional
         The name of a column or list of columns for which to group by. Often
         necessary when pulling data across assets: When you want header='Name',
         you typically need group_by=['Path', 'Asset']
 
     shape : {'auto', 'samples', 'capsules'}, default 'auto'
         If 'auto', returns capsules as a time series of 0 or 1 when signals are
         also present in the items argument, or returns capsules as individual
         rows if no signals are present. 'samples' or 'capsules' forces the
         output to the former or the latter, if possible.
 
-    capsule_properties : list(str)
+    capsule_properties : list(str), optional
         A list of capsule properties to retrieve when shape='capsules'.
         By default, if no signals are present in the items DataFrame, then all
         properties found on a capsule are automatically returned (because
         the nature of the query allows them to be returned "for free").
         Otherwise, you must provide a list of names of properties to retrieve.
 
-    tz_convert : {str, datetime.tzinfo}
+    tz_convert : {str, datetime.tzinfo}, optional
         The time zone in which to return all timestamps. If the time zone
         string is not recognized, the list of supported time zone strings will
         be returned in the exception text.
 
-    calculation : {str, pandas.Series, pandas.DataFrame}
+    calculation : {str, pandas.Series, pandas.DataFrame}, optional
         When applying a calculation across assets, the 'calculation' argument
         must be a one-row DataFrame (or a Series) and the 'items' argument must
         be full of assets. When applying a calculation to a signal/condition/
         scalar, calculation must be a string with a single variable in it:
         $signal, $condition or $scalar.
 
     bounding_values : bool, default False
@@ -138,15 +138,15 @@
         If 'raise', any errors encountered will cause an exception. If
         'catalog', errors will be added to a 'Result' column in the status.df
         DataFrame.
 
     quiet : bool, default False
         If True, suppresses progress output. Note that when status is
         provided, the quiet setting of the Status object that is passed
-        in takes precedent.
+        in takes precedence.
 
     status : spy.Status, optional
         If specified, the supplied Status object will be updated as the command
         progresses. It gets filled in with the same information you would see
         in Jupyter in the blue/green/red table below your code while the
         command is executed. The table itself is accessible as a DataFrame via
         the status.df property.
@@ -1095,15 +1095,15 @@
     else:
         if not item:
             item = items_api.get_item_and_all_properties(id=item_id)  # type: ItemOutputV1
 
         item_name = ''
         if header == '__auto__' and _common.present(row, 'Path'):
             item_name = _common.get(row, 'Path') + ' >> '
-            if _common.present(row, 'Asset'):
+            if item_type != 'Asset' and _common.present(row, 'Asset'):
                 item_name += _common.get(row, 'Asset') + ' >> '
 
         if header in ['__auto__', 'Name']:
             item_name += item.name
         elif header == 'Description':
             item_name += item.description
         else:
```

### Comparing `seeq-spy-187.5/seeq/spy/_push.py` & `seeq-spy-188.0/seeq/spy/_push.py`

 * *Files 0% similar despite different names*

```diff
@@ -207,15 +207,15 @@
         If 'raise', any errors encountered will cause an exception. If
         'catalog', errors will be added to a 'Result' column in the status.df
         DataFrame.
 
     quiet : bool, default False
         If True, suppresses progress output. Note that when status is
         provided, the quiet setting of the Status object that is passed
-        in takes precedent.
+        in takes precedence.
 
     status : spy.Status, optional
         If specified, the supplied Status object will be updated as the command
         progresses. It gets filled in with the same information you would see
         in Jupyter in the blue/green/red table below your code while the
         command is executed. The table itself is accessible as a DataFrame via
         the status.df property.
@@ -244,15 +244,18 @@
                             workbook.
         worksheet_id        If pushed to a specific worksheet, the ID of that
                             worksheet.
         workbook_url        If pushed to a specific workbook, the URL of that
                             workbook and the curated worksheet that this
                             command created.
         datasource          The datasource that all pushed items will fall
-                            under (as a DatasourceOutputV1 object).
+                            under (as a DatasourceOutputV1 object)
+        old_asset_format    Always False because this function requires use of
+                            the new asset format. See doc for
+                            spy.search(old_asset_format) argument.
         status              A spy.Status object with the status of the
                             spy.push call
         =================== ===================================================
     """
     input_args = _common.validate_argument_types([
         (data, 'data', pd.DataFrame),
         (metadata, 'metadata', pd.DataFrame),
@@ -590,14 +593,15 @@
     push_df_properties = types.SimpleNamespace(
         func='spy.push',
         kwargs=input_args,
         workbook_id=workbook_context.workbook_id,
         worksheet_id=workbook_context.worksheet_id,
         workbook_url=workbook_url,
         datasource=datasource_output,
+        old_asset_format=False,
         status=status)
 
     _common.put_properties_on_df(push_result_df, push_df_properties)
 
     return push_result_df
```

### Comparing `seeq-spy-187.5/seeq/spy/_redaction.py` & `seeq-spy-188.0/seeq/spy/_redaction.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.5/seeq/spy/_search.py` & `seeq-spy-188.0/seeq/spy/_search.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from __future__ import annotations
 
 import types
 from typing import List, Dict, Union, Mapping, Optional
 
-import numpy as np
 import pandas as pd
 
 from seeq import spy
 from seeq.sdk import *
-from seeq.spy import _common, _login, _metadata, _push
+from seeq.spy import _common, _login, _metadata, _push, _swap
 from seeq.spy._errors import *
 from seeq.spy._redaction import safely, request_safely
 from seeq.spy._session import Session
 from seeq.spy._status import Status
 
 RESERVED_SEARCH_COLUMN_NAMES = ['Path', 'Asset', 'Type', 'Depth', 'Estimated Sample Period', 'Formula Parameters',
                                 'Datasource Name']
 
 
 def search(query, *, all_properties=False, workbook=_common.DEFAULT_WORKBOOK_PATH, recursive=True,
-           ignore_unindexed_properties=True, include_archived=False, estimate_sample_period=None, order_by=None,
-           quiet=None, errors=None, status=None, session: Optional[Session] = None):
+           ignore_unindexed_properties=True, include_archived=False, include_swappable_assets=False,
+           estimate_sample_period=None, old_asset_format=None, order_by=None, quiet=None, errors=None, status=None,
+           session: Optional[Session] = None):
     """
     Issues a query to the Seeq Server to retrieve metadata for signals,
     conditions, scalars and assets. This metadata can then be used to retrieve
     samples, capsules for a particular time range via spy.pull().
 
     Parameters
     ----------
@@ -108,34 +108,47 @@
     ignore_unindexed_properties : bool, default True
         If False, a ValueError will be raised if any properties are supplied
         that cannot be used in the search.
 
     include_archived : bool, default False
         If True, includes trashed/archived items in the output.
 
+    include_swappable_assets : bool, default False
+        Adds a "Swappable Assets" column to the output where each cell is an
+        embedded DataFrame that includes the assets that the item refers to and
+        can theoretically be swapped for other assets using spy.swap().
+
     estimate_sample_period : dict, default None
         A dict with the keys 'Start' and 'End'. If provided, an estimated
         sample period for all signals will be included in the output. The
         values for the 'Start' and 'End' keys must be a string that
         pandas.to_datetime() can parse, or a pandas.Timestamp. The start
         and end times are used to bound the calculation of the sample period.
         If the start and end times encompass a time range that is insufficient
         to determine the sample period, a pd.NaT will be returned.
         If the value of 'Start' is set to None, it will default to the value of
         'End' minus 1 hour. Conversely, if the value of 'End' is set to None,
         it will default to now.
 
+    old_asset_format : bool, default True
+        Historically, spy.search() returned rows with a "Type" of "Asset" whereby
+        the "Asset" column was the name of the parent asset. This is inconsistent
+        with all other aspects of SPy, including spy.push(metadata). If you would
+        like Asset rows to instead be consistent with the rest of SPy (whereby
+        the "Asset" column is the name of the current asset, not the parent),
+        pass in False for this argument.
+
     order_by : {str, list}, default None
         An optional field or list of fields used to sort the search results.
         Fields on which results can be sorted are 'ID', 'Name', and 'Description'.
 
     quiet : bool, default False
         If True, suppresses progress output. Note that when status is
         provided, the quiet setting of the Status object that is passed
-        in takes precedent.
+        in takes precedence.
 
     errors : {'raise', 'catalog'}, default 'raise'
         If 'raise', any errors encountered will cause an exception. If 'catalog',
         errors will be added to a 'Result' column in the status.df DataFrame.
 
     status : spy.Status, optional
         If specified, the supplied Status object will be updated as the command
@@ -160,14 +173,16 @@
 
         =================== ===================================================
         Property            Description
         =================== ===================================================
         func                A str value of 'spy.search'
         kwargs              A dict with the values of the input parameters
                             passed to spy.search to get the output DataFrame
+        old_asset_format    True if the old Asset format was used (see doc for
+                            old_asset_format argument)
         status              A spy.Status object with the status of the
                             spy.search call
         =================== ===================================================
 
     Examples
     --------
     Search for signals with the name 'Humid' on the asset tree under
@@ -204,51 +219,60 @@
         (query, 'query', (str, dict, list, pd.DataFrame, pd.Series)),
         (all_properties, 'all_properties', bool),
         (workbook, 'workbook', str),
         (recursive, 'recursive', bool),
         (ignore_unindexed_properties, 'ignore_unindexed_properties', bool),
         (include_archived, 'include_archived', bool),
         (estimate_sample_period, 'estimate_sample_period', dict),
+        (include_swappable_assets, 'include_swappable_assets', bool),
+        (old_asset_format, 'old_asset_format', bool),
         (order_by, 'order_by', (str, list)),
         (quiet, 'quiet', bool),
         (errors, 'errors', str),
         (status, 'status', Status),
         (session, 'session', Session)
     ])
 
     status = Status.validate(status, quiet, errors)
     session = Session.validate(session)
     _login.validate_login(session, status)
 
     try:
         return _search(session, query, all_properties=all_properties, workbook=workbook, recursive=recursive,
                        ignore_unindexed_properties=ignore_unindexed_properties, include_archived=include_archived,
-                       estimate_sample_period=estimate_sample_period, order_by=order_by, status=status,
-                       input_args=input_args)
+                       estimate_sample_period=estimate_sample_period, include_swap_info=include_swappable_assets,
+                       old_asset_format=old_asset_format, order_by=order_by, status=status, input_args=input_args)
 
     except KeyboardInterrupt:
         status.update('Search canceled', Status.CANCELED)
 
 
 def _search(session: Session, query, *, all_properties, workbook, recursive, ignore_unindexed_properties,
-            include_archived, estimate_sample_period, order_by, status, input_args):
+            include_archived, estimate_sample_period, include_swap_info, old_asset_format, order_by, status,
+            input_args):
     if order_by:
         order_by = _validate_order_by(order_by)
 
     if estimate_sample_period is not None:
         if estimate_sample_period.keys() != {'Start', 'End'}:  # strict comparison, allowing only these two keys
             raise SPyValueError(f"estimate_sample_period must have 'Start' and 'End' keys but got "
                                 f"{estimate_sample_period.keys()}")
         pd_start, pd_end = _login.validate_start_and_end(session,
                                                          estimate_sample_period['Start'],
                                                          estimate_sample_period['End'])
 
     if not recursive and 'Path' not in query:
         raise SPyValueError("'Path' must be included in query when recursive=False")
 
+    old_asset_format__resolved = old_asset_format
+    if old_asset_format__resolved is None:
+        # In the future, we may wish to change this default to False, in which case we should use
+        # spy.options.compatibility and keep it True for users expecting older behavior.
+        old_asset_format__resolved = True
+
     items_api = ItemsApi(session.client)
     trees_api = TreesApi(session.client)
     formulas_api = FormulasApi(session.client)
     displays_api = DisplaysApi(session.client)
     display_templates_api = DisplayTemplatesApi(session.client)
 
     queries: List[Union[Dict, Mapping]]
@@ -292,22 +316,23 @@
             _val = _val.lower() == 'true'
         _dict[_key] = _common.none_to_nan(_val)
 
         # We want the columns to appear in a certain order (the order we added them in) for readability
         if _key not in columns:
             columns.append(_key)
 
-    def _add_ancestors_to_prop_dict(_ancestors, _prop_dict):
-        if len(_ancestors) > 1:
-            _add_to_dict(_prop_dict, 'Path',
-                         _common.path_list_to_string([_a.name for _a in _ancestors[0:-1]]))
-            _add_to_dict(_prop_dict, 'Asset', _ancestors[-1].name)
-        elif len(_ancestors) == 1:
-            _add_to_dict(_prop_dict, 'Path', np.nan)
-            _add_to_dict(_prop_dict, 'Asset', _ancestors[0].name)
+    def _add_ancestors_to_prop_dict_from_item_output(_item_output, _prop_dict):
+        _ancestors = [a.name for a in _item_output.ancestors]
+        _add_ancestors_to_prop_dict(_item_output.type, _item_output.name, _ancestors, _prop_dict)
+
+    def _add_ancestors_to_prop_dict(_type, _name, _ancestors, _prop_dict):
+        _common.add_ancestors_to_definition(_type, _name, _ancestors, _prop_dict, old_asset_format__resolved)
+        for _key in ['Path', 'Asset']:
+            if _key in _prop_dict and _key not in columns:
+                columns.append(_key)
 
     def _add_to_metadata(_prop_dict):
         if _prop_dict['ID'] not in ids:
             metadata.append(_prop_dict)
             ids.add(_prop_dict['ID'])
         else:
             nonlocal dupe_count
@@ -330,15 +355,15 @@
                 f'Could not determine the sample period for signal "{_signal_name}" {_signal_id} within the '
                 f'time period {pd_start.isoformat()} to {pd_end.isoformat()}. There might not be enough data '
                 f'in the specified time range. Modify the time period with the `estimate_start` '
                 f'and `estimate_end` arguments.'
             )
             sample_periods[_signal_id] = pd.NaT
 
-    def _add_all_properties(_id, _prop_dict, _get_tree=False):
+    def _add_all_properties(_id, _prop_dict):
 
         def _add_error_message_and_warn(msg):
             _add_to_dict(_prop_dict, 'Pull Result', msg)
             status.warn(msg)
 
         @request_safely(action_description=f'get all item properties for {_id}',
                         status=status,
@@ -374,20 +399,48 @@
                     _add_to_dict(_prop_dict, 'Swap Out Asset ID', _display_output.template.swap_source_asset_id)
 
             elif _item.type == 'DisplayTemplate':
                 _display_template_output = display_templates_api.get_display_template(id=_id)
                 _add_to_dict(_prop_dict, 'Source Workstep ID', _display_template_output.source_workstep_id)
 
         _request_item_properties()
-        if _get_tree:
-            asset_tree_output = safely(lambda: trees_api.get_tree(id=_id),
-                                       action_description=f'get asset tree ancestors for {_id}',
-                                       status=status)  # type: AssetTreeOutputV1
-            if asset_tree_output is not None:
-                _add_ancestors_to_prop_dict(asset_tree_output.item.ancestors, _prop_dict)
+        return _prop_dict
+
+    def _add_tree(_id, _prop_dict):
+        _item_output = None
+        if include_swap_info:
+            _item_dependency_output = safely(lambda: items_api.get_formula_dependencies(id=_id),
+                                             action_description=f'get dependencies for {_id}',
+                                             status=status)  # type: ItemDependencyOutputV1
+            if _item_dependency_output is not None:
+                _item_output = _item_dependency_output
+
+            _dependencies_with_relevant_assets = _swap.get_swappable_assets(_item_dependency_output)
+
+            def _swappable_asset_dict(d):
+                _leaf_asset = d.ancestors[-1]
+                return {
+                    'ID': _leaf_asset.id,
+                    'Type': _leaf_asset.type,
+                    'Path': _common.path_list_to_string([a.name for a in d.ancestors[0:-1]]),
+                    'Asset': _leaf_asset.name
+                }
+
+            _swappable_assets = pd.DataFrame([_swappable_asset_dict(d) for d in _dependencies_with_relevant_assets],
+                                             columns=['ID', 'Type', 'Path', 'Asset'])
+
+            _add_to_dict(_prop_dict, 'Swappable Assets', _swappable_assets)
+        else:
+            _asset_tree_output = safely(lambda: trees_api.get_tree(id=_id),
+                                        action_description=f'get asset tree ancestors for {_id}',
+                                        status=status)  # type: AssetTreeOutputV1
+            if _asset_tree_output is not None:
+                _item_output = _asset_tree_output.item
+        if _item_output is not None:
+            _add_ancestors_to_prop_dict_from_item_output(_item_output, _prop_dict)
         return _prop_dict
 
     workbook_id = None
     if workbook:
         if _common.is_guid(workbook):
             workbook_id = _common.sanitize_guid(workbook)
         else:
@@ -403,21 +456,22 @@
 
     for status_index in range(len(queries)):
         timer = _common.timer_start()
 
         current_query = queries[status_index]
 
         if _common.present(current_query, 'ID'):
-            # If ID is specified, short-circuit everything and just get the item directly. But since this method
-            # bypasses the search_items() route that would normally supply the asset ancestors, we specifically tell
-            # _add_all_properties() to make the trees_api call that will fetch the ancestors if the user wants all
-            # properties to be returned.
+            # If ID is specified, short-circuit everything and just get the item directly.
             _prop_dict = dict()
             current_id = current_query['ID']
-            _add_all_properties(current_id, _prop_dict, _get_tree=all_properties)
+            _add_all_properties(current_id, _prop_dict)
+
+            # Since this method bypasses the search_items() route that would normally supply the asset ancestors, we
+            # specifically call _add_tree() to make the trees_api call that will fetch the ancestors.
+            _add_tree(current_id, _prop_dict)
 
             # Still need to determine sample period for signals and have NaT for non-signal items
             if estimate_sample_period is not None:
                 if 'Signal' in current_query['Type']:
                     _estimate_sample_period(current_id, _prop_dict['Name'])
                 else:
                     sample_periods[current_query['ID']] = pd.NaT
@@ -639,29 +693,30 @@
 
         def _gather_results(_actual_path_list=None):
             def _gather_results_via_item_search(_result):
                 _item_search_preview = _result  # type: ItemSearchPreviewV1
                 __prop_dict = dict()
 
                 _add_to_dict(__prop_dict, 'ID', _item_search_preview.id)
-                _add_ancestors_to_prop_dict(_item_search_preview.ancestors, __prop_dict)
+                _add_ancestors_to_prop_dict_from_item_output(_item_search_preview, __prop_dict)
 
                 _add_to_dict(__prop_dict, 'Name', _item_search_preview.name)
                 _add_to_dict(__prop_dict, 'Description', _item_search_preview.description)
                 _add_to_dict(__prop_dict, 'Type', _item_search_preview.type)
                 _uom = _item_search_preview.value_unit_of_measure if _item_search_preview.value_unit_of_measure \
                     else _item_search_preview.source_value_unit_of_measure
                 _add_to_dict(__prop_dict, 'Value Unit Of Measure', _uom)
                 _datasource_item_preview = _item_search_preview.datasource  # type: ItemPreviewV1
                 _add_to_dict(__prop_dict, 'Datasource Name',
                              _datasource_item_preview.name if _datasource_item_preview else None)
                 _add_to_dict(__prop_dict, 'Archived', _item_search_preview.is_archived)
                 if all_properties:
                     _add_all_properties(_item_search_preview.id, __prop_dict)
-
+                if include_swap_info:
+                    _add_tree(_item_search_preview.id, __prop_dict)
                 if estimate_sample_period is not None:
                     _add_to_dict(__prop_dict, 'Estimated Sample Period', sample_periods[_item_search_preview.id])
                 _add_to_metadata(__prop_dict)
 
             def _gather_results_via_get_tree(_result):
                 _tree_item_output = _result  # type: TreeItemOutputV1
                 __prop_dict = dict()
@@ -672,30 +727,27 @@
 
                     if not _common.does_query_fragment_match(current_query[_prop],
                                                              getattr(_tree_item_output, _attr),
                                                              contains=(comparison == '~=')):
                         return
 
                 _add_to_dict(__prop_dict, 'ID', _tree_item_output.id)
-                if len(_actual_path_list) > 1:
-                    _add_to_dict(__prop_dict, 'Path', _common.path_list_to_string(_actual_path_list[0:-1]))
-                    _add_to_dict(__prop_dict, 'Asset', _actual_path_list[-1])
-                elif len(_actual_path_list) == 1:
-                    _add_to_dict(__prop_dict, 'Path', np.nan)
-                    _add_to_dict(__prop_dict, 'Asset', _actual_path_list[0])
+                _add_ancestors_to_prop_dict(
+                    _tree_item_output.type, _tree_item_output.name, _actual_path_list, __prop_dict)
 
                 _add_to_dict(__prop_dict, 'Name', _tree_item_output.name)
                 _add_to_dict(__prop_dict, 'Description', _tree_item_output.description)
                 _add_to_dict(__prop_dict, 'Type', _tree_item_output.type)
                 _add_to_dict(__prop_dict, 'Value Unit Of Measure', _tree_item_output.value_unit_of_measure)
                 _add_to_dict(__prop_dict, 'Archived', _tree_item_output.is_archived)
 
                 if all_properties:
                     _add_all_properties(_tree_item_output.id, __prop_dict)
-
+                if include_swap_info:
+                    _add_tree(_tree_item_output.id, __prop_dict)
                 if estimate_sample_period is not None:
                     _add_to_dict(__prop_dict, 'Estimated Sample Period', sample_periods[_tree_item_output.id])
                 _add_to_metadata(__prop_dict)
 
             if use_search_items_api:
                 _iterate_over_output(_do_search, 'items', _gather_results_via_item_search)
             else:
@@ -791,17 +843,27 @@
 
     if len(columns) == 0:
         columns = ['ID', 'Type']
     output_df = pd.DataFrame(data=metadata, columns=columns)
     if order_by and not output_df.empty:
         output_df.sort_values(order_by, ignore_index=True, inplace=True)
 
+    if old_asset_format is None:
+        type_column = output_df['Type']
+        if len(type_column.loc[type_column == 'Asset']) > 0:
+            status.warn('This search result includes Assets. Consider passing in "old_asset_format=False" so that the '
+                        '"Path" and "Asset" columns are populated in a way that is consistent with all other aspects '
+                        'of SPy. The default behavior without this argument emulates the (incorrect) way SPy would '
+                        'return such results historically.')
+            status.display()
+
     output_df_properties = types.SimpleNamespace(
         func='spy.search',
         kwargs=input_args,
+        old_asset_format=old_asset_format__resolved,
         status=status)
 
     _common.put_properties_on_df(output_df, output_df_properties)
 
     return output_df
```

### Comparing `seeq-spy-187.5/seeq/spy/_session.py` & `seeq-spy-188.0/seeq/spy/_session.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import textwrap
 from dataclasses import dataclass
 from typing import Optional, List
 
 import pytz
 import requests
 from dateutil.tz import tz
-
 from seeq import spy
 from seeq.sdk import *
 from seeq.sdk.configuration import ClientConfiguration
 from seeq.spy import _url, _common, _datalab, _errors
 from seeq.spy._errors import *
 
 SEEQ_SDK_RETRY_TIMEOUT_IN_SECONDS_ENV_VAR_NAME = 'SEEQ_SDK_RETRY_TIMEOUT_IN_SECONDS'
@@ -194,14 +193,21 @@
         return f'{self.private_url}/api'
 
     @property
     def options(self):
         """
         Assign a new value to the following variables if you would like to adjust them.
 
+        ``spy.options.compatibility`` (default: None)
+
+            The major version of SPy to emulate from a compatibility standpoint. This
+            is important to set if you would like to minimize the chance that your
+            script or add-on "breaks" when SPy is upgraded. Set it to the major version
+            of SPy that you have tested against. E.g.: spy.options.compatibility = 184
+
         ``spy.options.search_page_size`` (default: 1000)
 
             The number of items retrieved on each round-trip to the Seeq Server during
             a spy.search() call. If you have a fast system and fast connection, you can
             make this higher.
 
         ``spy.options.pull_page_size`` (default: 1000000)
@@ -214,14 +220,20 @@
         ``spy.options.push_page_size`` (default: 100000)
 
             The number of samples/capsules uploaded during each round-trip to the Seeq
             Server during a spy.push() call. If you have a slow system or slow
             connection, you may wish to make this lower. It is not recommended to
             exceed 1000000.
 
+        ``spy.options.metadata_push_batch_size`` (default: 1000)
+
+            The number of items uploaded during each round-trip to the Seeq
+            Server during a spy.push(metadata) call. If you have a low-memory system
+            you may wish to make this lower. It is not recommended to exceed 10000.
+
         ``spy.options.max_concurrent_requests`` (default: 8)
 
             The maximum number of simultaneous requests made to the Seeq Server during
             spy.pull() and spy.push() calls. The higher the number, the more you can
             monopolize the Seeq Server. If you keep it low, then other users are less
             likely to be impacted by your activity.
 
@@ -272,45 +284,49 @@
     _DEFAULT_PUSH_PAGE_SIZE = 100000
     _DEFAULT_METADATA_PUSH_BATCH_SIZE = 1000
     _DEFAULT_MAX_CONCURRENT_REQUESTS = 8
     _DEFAULT_CLEAR_CONTENT_CACHE_BEFORE_RENDER = False
     _DEFAULT_ALLOW_VERSION_MISMATCH = False
     _DEFAULT_FRIENDLY_EXCEPTIONS = _datalab.is_datalab()
     _DEFAULT_TIMEZONE = None
+    _DEFAULT_COMPATIBILITY = None
 
     def __init__(self, client_configuration: ClientConfiguration):
         self.client_configuration = client_configuration
         self.search_page_size = self._DEFAULT_SEARCH_PAGE_SIZE
         self.pull_page_size = self._DEFAULT_PULL_PAGE_SIZE
         self.push_page_size = self._DEFAULT_PUSH_PAGE_SIZE
         self.metadata_push_batch_size = self._DEFAULT_METADATA_PUSH_BATCH_SIZE
         self.max_concurrent_requests = self._DEFAULT_MAX_CONCURRENT_REQUESTS
         self.clear_content_cache_before_render = self._DEFAULT_CLEAR_CONTENT_CACHE_BEFORE_RENDER
         self.allow_version_mismatch = self._DEFAULT_ALLOW_VERSION_MISMATCH
         self.default_timezone = self._DEFAULT_TIMEZONE
+        self.compatibility = self._DEFAULT_COMPATIBILITY
         try:
             self.friendly_exceptions = self._DEFAULT_FRIENDLY_EXCEPTIONS
         except RuntimeError:
             pass
 
     def __str__(self):
         return '\n'.join([f"{k}: {v}" for k, v in self.__dict__.items()])
 
     def __getstate__(self):
         # We can only pickle certain members. This has to mirror __setstate__().
-        return (self.search_page_size,
+        return (self.compatibility,
+                self.search_page_size,
                 self.pull_page_size,
                 self.push_page_size,
                 self.metadata_push_batch_size,
                 self.max_concurrent_requests,
                 self.clear_content_cache_before_render,
                 self.allow_version_mismatch)
 
     def __setstate__(self, state):
-        (self.search_page_size,
+        (self.compatibility,
+         self.search_page_size,
          self.pull_page_size,
          self.push_page_size,
          self.metadata_push_batch_size,
          self.max_concurrent_requests,
          self.clear_content_cache_before_render,
          self.allow_version_mismatch) = state
 
@@ -368,14 +384,21 @@
 
             E.g.:
                spy.options.concurrent_requests = 3
 
             Available Options
             -----------------
 
+            spy.options.compatibility (default: {self._DEFAULT_COMPATIBILITY})
+
+                The major version of SPy to emulate from a compatibility standpoint. This
+                is important to set if you would like to minimize the chance that your
+                script or add-on "breaks" when SPy is upgraded. Set it to the major version
+                of SPy that you have tested against. E.g.: spy.options.compatibility = 184
+
             spy.options.search_page_size (default: {self._DEFAULT_SEARCH_PAGE_SIZE})
 
                 The number of items retrieved on each round-trip to the Seeq Server during
                 a spy.search() call. If you have a fast system and fast connection, you can
                 make this higher.
 
             spy.options.pull_page_size (default: {self._DEFAULT_PULL_PAGE_SIZE})
```

### Comparing `seeq-spy-187.5/seeq/spy/_status.py` & `seeq-spy-188.0/seeq/spy/_status.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.5/seeq/spy/_upgrade.py` & `seeq-spy-188.0/seeq/spy/_upgrade.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.5/seeq/spy/_url.py` & `seeq-spy-188.0/seeq/spy/_url.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.5/seeq/spy/acl/_pull.py` & `seeq-spy-188.0/seeq/spy/acl/_pull.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         If 'raise', any errors encountered will cause an exception. If
         'catalog', errors will be added to a 'Pull Result' column in the
         status.df DataFrame.
 
     quiet : bool, default False
         If True, suppresses progress output. Note that when status is
         provided, the quiet setting of the Status object that is passed
-        in takes precedent.
+        in takes precedence.
 
     status : spy.Status, optional
         If specified, the supplied Status object will be updated as the command
         progresses. It gets filled in with the same information you would see
         in Jupyter in the blue/green/red table below your code while the
         command is executed. The table itself is accessible as a DataFrame via
         the status.df property.
```

### Comparing `seeq-spy-187.5/seeq/spy/acl/_push.py` & `seeq-spy-188.0/seeq/spy/acl/_push.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         If 'raise', any errors encountered will cause an exception. If
         'catalog', errors will be added to a 'Push Result' column in the
         status.df DataFrame.
 
     quiet : bool, default False
         If True, suppresses progress output. Note that when status is
         provided, the quiet setting of the Status object that is passed
-        in takes precedent.
+        in takes precedence.
 
     status : spy.Status, optional
         If specified, the supplied Status object will be updated as the command
         progresses. It gets filled in with the same information you would see
         in Jupyter in the blue/green/red table below your code while the
         command is executed. The table itself is accessible as a DataFrame via
         the status.df property.
```

### Comparing `seeq-spy-187.5/seeq/spy/addons/_install.py` & `seeq-spy-188.0/seeq/spy/addons/_install.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,15 +162,15 @@
         If 'raise', any errors encountered will cause an exception. If
         'catalog', errors will be added to a 'Result' column in the status.df
         DataFrame.
 
     quiet : bool, default False
         If True, suppresses progress output. Note that when status is
         provided, the quiet setting of the Status object that is passed
-        in takes precedent.
+        in takes precedence.
 
     status : spy.Status, optional
         If specified, the supplied Status object will be updated as the command
         progresses. It gets filled in with the same information you would see
         in Jupyter in the blue/green/red table below your code while the
         command is executed. The table itself is accessible as a DataFrame via
         the status.df property.
```

### Comparing `seeq-spy-187.5/seeq/spy/addons/_permissions.py` & `seeq-spy-188.0/seeq/spy/addons/_permissions.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.5/seeq/spy/addons/_search.py` & `seeq-spy-188.0/seeq/spy/addons/_search.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         If 'raise', any errors encountered will cause an exception. If
         'catalog', errors will be added to a 'Result' column in the status.df
         DataFrame.
 
     quiet : bool, default False
         If True, suppresses progress output. Note that when status is
         provided, the quiet setting of the Status object that is passed
-        in takes precedent.
+        in takes precedence.
 
     status : spy.Status, optional
         If specified, the supplied Status object will be updated as the command
         progresses. It gets filled in with the same information you would see
         in Jupyter in the blue/green/red table below your code while the
         command is executed. The table itself is accessible as a DataFrame via
         the status.df property.
```

### Comparing `seeq-spy-187.5/seeq/spy/addons/_uninstall.py` & `seeq-spy-188.0/seeq/spy/addons/_uninstall.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         If 'raise', any errors encountered will cause an exception. If
         'catalog', errors will be added to a 'Result' column in the status.df
         DataFrame.
 
     quiet : bool
         If True, suppresses progress output. Note that when status is
         provided, the quiet setting of the Status object that is passed
-        in takes precedent.
+        in takes precedence.
 
     status : spy.Status, optional
         If specified, the supplied Status object will be updated as the command
         progresses. It gets filled in with the same information you would see
         in Jupyter in the blue/green/red table below your code while the
         command is executed. The table itself is accessible as a DataFrame via
         the status.df property.
```

### Comparing `seeq-spy-187.5/seeq/spy/assets/_brochure.py` & `seeq-spy-188.0/seeq/spy/assets/_brochure.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.5/seeq/spy/assets/_build.py` & `seeq-spy-188.0/seeq/spy/assets/_build.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import inspect
 import re
 import types
 from types import ModuleType
 from typing import List, Union, Type
 
 import pandas as pd
-
 from seeq.spy import _common
 from seeq.spy._errors import *
 from seeq.spy._status import Status
 from seeq.spy.assets._context import SPyInstanceAlreadyExists
 from seeq.spy.assets._model import _AssetBase, BuildContext, BuildPhase, SPyDependencyNotBuilt
 from seeq.spy.workbooks import Workbook
 
@@ -233,15 +232,15 @@
         templates = [model]
     else:
         raise SPyTypeError('"model" parameter must be a Python module (with Assets) or an Asset class declaration')
 
     return templates
 
 
-def prepare(metadata, *, root_asset_name=None):
+def prepare(metadata, *, root_asset_name=None, old_asset_format=None):
     """
     Modifies (in place) a metadata DataFrame that represents an existing tree,
     usually obtained by doing spy.search(recursive=True), and creates
     "Build Path" and "Build Asset" columns that are suitable for typical use of
     spy.assets.build().
 
     Parameters
@@ -251,33 +250,38 @@
         spy.search(recursive=True) on an existing tree, that will be used
         as the "ingredients" for spy.assets.build().
 
     root_asset_name : str, optional
         An optional new name to use as the root of the tree. You will typically
         want to specify this so that your new tree is differentiated from the
         existing tree.
+
+    old_asset_format : bool, optional
     """
     for column in ['Type', 'Path', 'Asset', 'Name']:
         if column not in metadata:
             raise SPyValueError(f'"{column}" is a required column')
 
+    old_asset_format = _common.resolve_old_asset_format_arg(old_asset_format, metadata)
+
     def _choose_build_asset(_row):
-        if _row['Type'] == 'Asset':
+        if _row['Type'] == 'Asset' and old_asset_format:
             return _row['Name']
         else:
             return _row['Asset']
 
     def _choose_build_path(_row):
         path = _row['Path']
-        if _row['Type'] == 'Asset':
-            if pd.isna(_row['Path']):
-                path = _row['Asset']
+
+        if _row['Type'] == 'Asset' and old_asset_format:
+            if _common.present(_row, 'Path') and _common.get(_row, 'Path') != '':
+                path = _row['Path'] + ' >> ' + _row['Asset']
             else:
-                path = f'{_row["Path"]} >> {_row["Asset"]}'
+                path = _row['Asset']
 
-        if root_asset_name:
+        if path is not None and root_asset_name:
             path = re.sub(r'^\s*.*?(\s*(>>|$))', rf'{root_asset_name}\1', path)
 
         return path
 
     metadata['Build Path'] = metadata.apply(_choose_build_path, axis=1)
     metadata['Build Asset'] = metadata.apply(_choose_build_asset, axis=1)
```

### Comparing `seeq-spy-187.5/seeq/spy/assets/_context.py` & `seeq-spy-188.0/seeq/spy/assets/_context.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.5/seeq/spy/assets/_model.py` & `seeq-spy-188.0/seeq/spy/assets/_model.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.5/seeq/spy/assets/_trees/_constants.py` & `seeq-spy-188.0/seeq/spy/assets/_trees/_constants.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.5/seeq/spy/assets/_trees/_csv.py` & `seeq-spy-188.0/seeq/spy/assets/_trees/_csv.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,15 +149,15 @@
         df_no_ids.drop(columns=['ID'], inplace=True)
 
     # which of the options the csv has:
     search_cols = [x for x in _search_options if x in df_no_ids.columns]
 
     try:
         search_res = _search.search(
-            df_no_ids[search_cols], order_by=["ID"], workbook=workbook, quiet=True
+            df_no_ids[search_cols], old_asset_format=True, order_by=["ID"], workbook=workbook, quiet=True
         )[['Name', 'ID']]
     except KeyError:
         if len(df_with_ids) == 0:
             message = f"No items were found with the specified names: {list(df_no_ids['Name'])}"
             status.exception(SPyValueError(message), throw=True)
         else:
             status.warn(f"The following names did not return search results and were "
```

### Comparing `seeq-spy-187.5/seeq/spy/assets/_trees/_match.py` & `seeq-spy-188.0/seeq/spy/assets/_trees/_match.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.5/seeq/spy/assets/_trees/_pandas.py` & `seeq-spy-188.0/seeq/spy/assets/_trees/_pandas.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.5/seeq/spy/assets/_trees/_path.py` & `seeq-spy-188.0/seeq/spy/assets/_trees/_path.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.5/seeq/spy/assets/_trees/_properties.py` & `seeq-spy-188.0/seeq/spy/assets/_trees/_properties.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.5/seeq/spy/assets/_trees/_pull.py` & `seeq-spy-188.0/seeq/spy/assets/_trees/_pull.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import re
 import types
 
 import numpy as np
 import pandas as pd
+
 from seeq.sdk import *
 from seeq.spy import _common, _search
 from seeq.spy._errors import *
 from seeq.spy._redaction import request_safely
 from seeq.spy._session import Session
 from seeq.spy._status import Status
 from seeq.spy.assets._trees import _constants, _path, _properties, _utils
@@ -86,15 +87,15 @@
     # Get all children of the requested asset
     @request_safely(
         action_description='pull children of node',
         status=status)
     def get_search_results():
         return _search.search(query={'Asset': node_id}, all_properties=True,
                               workbook=_get_search_workbook(session, node_id, workbook_id),
-                              order_by=['ID'], quiet=True, session=session)
+                              old_asset_format=True, order_by=['ID'], quiet=True, session=session)
 
     search_results = get_search_results()
     if search_results is None or len(search_results) == 0:
         return df
 
     if item_ids_to_ignore is not None:
         search_results = search_results[~search_results['ID'].isin(item_ids_to_ignore)]
@@ -242,15 +243,15 @@
             if _row_is_spy_tree_root(row, spy_tree.id, spy_tree.name):
                 if df_root_id is None:
                     df_root_id = row['ID']
                 else:
                     return None
     if df_root_id is not None:
         existing_tree_df = _search.search([{'ID': df_root_id}, {'Asset': df_root_id}], workbook=workbook_id,
-                                          order_by=['ID'], quiet=True, session=session)
+                                          old_asset_format=True, order_by=['ID'], quiet=True, session=session)
         existing_tree_df['Path'] = existing_tree_df.apply(_path.determine_path, axis=1)
         if 'Datasource Name' not in existing_tree_df.columns:
             existing_tree_df['Datasource Name'] = np.nan
         existing_tree_df = existing_tree_df[['ID', 'Path', 'Name', 'Type', 'Datasource Name']]
         return existing_tree_df
     else:
         return None
```

### Comparing `seeq-spy-187.5/seeq/spy/assets/_trees/_tree.py` & `seeq-spy-188.0/seeq/spy/assets/_trees/_tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,15 +93,15 @@
         is pushed.
 
     quiet : bool, default False
         If True, suppresses progress output. This setting will be the default for all
         operations on this Tree. This option can be changed later using
         `tree.quiet = True` or by specifying the option for individual function calls.
         Note that when status is provided, the quiet setting of the Status object
-        that is passed in takes precedent.
+        that is passed in takes precedence.
 
     errors : {'raise', 'catalog'}, default 'raise'
         If 'raise', any errors encountered will cause an exception. If 'catalog',
         errors will be added to a 'Result' column in the status.df DataFrame. The
         option chosen here will be the default for all other operations on this Tree.
         This option can be changed later using `tree.errors = 'catalog'` or by
         specifying the option for individual function calls.
@@ -319,15 +319,20 @@
             for an asset or calculation to be inserted.
 
         formula : str, optional
             The formula for a calculated item. The `formula` and `formula_parameters` are
             used in place of the `children` argument.
 
         formula_parameters : dict, optional
-            The parameters for a formula.
+            The parameters used in the specified `formula`. The following options are allowed:
+
+            1) The name of an item that is an asset sibling of this calculation.
+            2) The relative path to an item in this Tree (E.G. '.. >> Area E >> Temperature').
+            3) The absolute path to an item in this Tree (E.G. 'Example >> Cooling Tower 2 >> Area E >> Temperature').
+            4) The ID of an item (including ones not in the Tree).
 
         roll_up_statistic : str, optional
             The statistic to use when inserting a roll-up calculation. Valid options are
             Average, Maximum, Minimum, Range, Sum, Multiply, Union, Intersect, Counts,
             Count Overlaps, Combine With.
 
         roll_up_parameters : str, optional
@@ -347,15 +352,15 @@
             input will be used only for the duration of this function; it will default
             to the setting on the Tree if not specified.
 
         quiet : bool, optional
             If True, suppresses progress output. This input will be used only for the
             duration of this function; it will default to the setting on the Tree if
             not specified. Note that when status is provided, the quiet setting of
-            the Status object that is passed in takes precedent.
+            the Status object that is passed in takes precedence.
 
         status : spy.Status, optional
             If specified, the supplied Status object will be updated as the command
             progresses. It gets filled in with the same information you would see
             in Jupyter in the blue/green/red table below your code while the
             command is executed. The table itself is accessible as a DataFrame via
             the status.df property.
@@ -522,15 +527,15 @@
             input will be used only for the duration of this function; it will default
             to the setting on the Tree if not specified.
 
         quiet : bool, optional
             If True, suppresses progress output. This input will be used only for the
             duration of this function; it will default to the setting on the Tree if
             not specified. Note that when status is provided, the quiet setting of
-            the Status object that is passed in takes precedent.
+            the Status object that is passed in takes precedence.
 
         status : spy.Status, optional
             If specified, the supplied Status object will be updated as the command
             progresses. It gets filled in with the same information you would see
             in Jupyter in the blue/green/red table below your code while the
             command is executed. The table itself is accessible as a DataFrame via
             the status.df property.
@@ -593,15 +598,15 @@
             input will be used only for the duration of this function; it will default
             to the setting on the Tree if not specified.
 
         quiet : bool, optional
             If True, suppresses progress output. This input will be used only for the
             duration of this function; it will default to the setting on the Tree if
             not specified. Note that when status is provided, the quiet setting of
-            the Status object that is passed in takes precedent.
+            the Status object that is passed in takes precedence.
 
         status : spy.Status, optional
             If specified, the supplied Status object will be updated as the command
             progresses. It gets filled in with the same information you would see
             in Jupyter in the blue/green/red table below your code while the
             command is executed. The table itself is accessible as a DataFrame via
             the status.df property.
@@ -966,15 +971,15 @@
             input will be used only for the duration of this function; it will default
             to the setting on the Tree if not specified.
 
         quiet : bool, optional
             If True, suppresses progress output. This input will be used only for the
             duration of this function; it will default to the setting on the Tree if
             not specified. Note that when status is provided, the quiet setting of
-            the Status object that is passed in takes precedent.
+            the Status object that is passed in takes precedence.
 
         status : spy.Status, optional
             If specified, the supplied Status object will be updated as the command
             progresses. It gets filled in with the same information you would see
             in Jupyter in the blue/green/red table below your code while the
             command is executed. The table itself is accessible as a DataFrame via
             the status.df property.
@@ -1058,15 +1063,15 @@
             input will be used only for the duration of this function; it will default
             to the setting on the Tree if not specified.
 
         quiet : bool, optional
             If True, suppresses progress output. This input will be used only for the
             duration of this function; it will default to the setting on the Tree if
             not specified. Note that when status is provided, the quiet setting of
-            the Status object that is passed in takes precedent.
+            the Status object that is passed in takes precedence.
 
         status : spy.Status, optional
             If specified, the supplied Status object will be updated as the command
             progresses. It gets filled in with the same information you would see
             in Jupyter in the blue/green/red table below your code while the
             command is executed. The table itself is accessible as a DataFrame via
             the status.df property.
@@ -1138,17 +1143,15 @@
         Set the _workbook_id based on the workbook input. This will enable us to know whether we should set
         the `ID` or `Referenced ID` column when pulling an item.
         """
         if _common.is_guid(self._workbook):
             self._workbook_id = _common.sanitize_guid(self._workbook)
         elif self.session.client:
             search_query, _ = _push.create_analysis_search_query(self._workbook)
-            search_df = spy.workbooks.search(search_query,
-                                             status=status,
-                                             session=self.session)
+            search_df = spy.workbooks.search(search_query, status=status, session=self.session)
             self._workbook_id = search_df.iloc[0]['ID'] if len(search_df) > 0 else _constants.UNKNOWN
         else:
             self._workbook_id = _constants.UNKNOWN
 
     def validate_status(self, status: Status, quiet: Optional[bool], errors: Optional[str]):
         if status is None:
             status = Status()
```

### Comparing `seeq-spy-187.5/seeq/spy/assets/_trees/_utils.py` & `seeq-spy-188.0/seeq/spy/assets/_trees/_utils.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.5/seeq/spy/assets/_trees/_validate.py` & `seeq-spy-188.0/seeq/spy/assets/_trees/_validate.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.5/seeq/spy/assets/brochure.html` & `seeq-spy-188.0/seeq/spy/assets/brochure.html`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.5/seeq/spy/docs/Documentation/Administration/User Migration.ipynb` & `seeq-spy-188.0/seeq/spy/docs/Documentation/Administration/User Migration.ipynb`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8474713654401155%*

 * *Differences: {"'cells'": "{0: {'metadata': {replace: OrderedDict()}}, 1: {'execution_count': 1, 'source': "*

 * *            "{insert: [(4, 'from seeq import sdk, spy\\n'), (5, '\\n'), (6, '# Set the "*

 * *            'compatibility option so that you maximize the chance that SPy will remain compatible '*

 * *            "with your notebook/script\\n'), (7, 'spy.options.compatibility = 188')], delete: "*

 * *            "[4]}, 'metadata': {replace: OrderedDict()}}, 2: {'metadata': {replace: "*

 * *            "OrderedDict()}}, 3: {'metadata':  […]*

```diff
@@ -1,117 +1,102 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
                 "# User Migration\n",
                 "\n",
                 "Migrate users between datasources\n",
                 "\n",
                 "\u26a0\ufe0f Only Seeq Administrators can run this notebook\n",
                 "\n",
                 "\u26a0\ufe0f This notebook makes irreversible changes to the system. Set `dry_run = True` and review the output after making\n",
                 "any changes to the configuration or implementation of this notebook."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
-            "metadata": {
-                "collapsed": false
-            },
+            "execution_count": 1,
+            "metadata": {},
             "outputs": [],
             "source": [
                 "from collections import namedtuple\n",
                 "\n",
                 "from pandas import DataFrame\n",
                 "\n",
-                "from seeq import sdk, spy"
+                "from seeq import sdk, spy\n",
+                "\n",
+                "# Set the compatibility option so that you maximize the chance that SPy will remain compatible with your notebook/script\n",
+                "spy.options.compatibility = 188"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
                 "## Authentication\n",
                 "\n",
                 "Log into Seeq Server if you're not using Seeq Data Lab"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
                 "spy.login(url='http://localhost:34216', credentials_file='../credentials.key', force=False)"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
                 "## Configuration\n",
                 "\n",
                 "- `dry_run`: When `True` the migration details will be displayed, but the migration will NOT be executed.\n",
                 "- `criteria`: Users where ANY of these properties match between datasources will be migrated.\n",
                 "- `old_datasource_name`: The name of the datasource to migrate users from.\n",
                 "- `new_datasource_name`: The name of the datasource to migrate users to."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
                 "dry_run = True\n",
                 "criteria = ['email', 'fullname', 'username']\n",
                 "old_datasource_name = 'Old SSO Provider'\n",
                 "new_datasource_name = 'New SSO Provider'"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
                 "## Implementation"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
                 "users_api = sdk.UsersApi(spy.client)\n",
                 "NormalizedUser = namedtuple('NormalizedUser', ['id', 'email', 'fullname', 'username'])"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
                 "def normalize_str(s):\n",
                 "    return s.strip().lower() if isinstance(s, str) else s\n",
                 "\n",
                 "\n",
                 "def normalize_user(user):\n",
@@ -140,17 +125,15 @@
                 "            return users\n",
                 "        offset += limit"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
                 "old_user_map = get_user_map(old_datasource_name)\n",
                 "new_user_map = get_user_map(new_datasource_name)\n",
                 "\n",
                 "matches = sorted(dict(\n",
                 "    (old_user_map[common_key], new_user_map[common_key])\n",
@@ -172,17 +155,15 @@
                 "dfStyler = df.style.set_properties(**{'text-align': 'left', 'white-space': 'nowrap', })\n",
                 "dfStyler.set_table_styles([dict(selector='th', props=[('text-align', 'left'), ('white-space', 'nowrap')])])"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
                 "results = []\n",
                 "\n",
                 "for old, new in matches:\n",
                 "    result_args = [old.id, '->', new.id]\n",
                 "\n",
@@ -201,27 +182,27 @@
                 "dfStyler = df.style.set_properties(**{'text-align': 'left', 'white-space': 'nowrap'})\n",
                 "dfStyler.set_table_styles([dict(selector='th', props=[('text-align', 'left'), ('white-space', 'nowrap')])])"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3",
+            "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
-                "version": 2
+                "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
-            "pygments_lexer": "ipython2",
-            "version": "2.7.6"
+            "pygments_lexer": "ipython3",
+            "version": "3.8.10"
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 0
+    "nbformat_minor": 1
 }
```

### Comparing `seeq-spy-187.5/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notification Add-on Installer.ipynb` & `seeq-spy-188.0/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notification Add-on Installer.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.5/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notification Scheduler.ipynb` & `seeq-spy-188.0/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notification Scheduler.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.5/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notifier.ipynb` & `seeq-spy-188.0/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notifier.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.5/seeq/spy/docs/Documentation/Advanced Scheduling/Email Unsubscriber.ipynb` & `seeq-spy-188.0/seeq/spy/docs/Documentation/Advanced Scheduling/Email Unsubscriber.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.5/seeq/spy/docs/Documentation/Advanced Scheduling/Parameterized Jobs.ipynb` & `seeq-spy-188.0/seeq/spy/docs/Documentation/Advanced Scheduling/Parameterized Jobs.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996811224489797%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(2, 'from seeq import spy\\n'), (3, '\\n'), (4, '# Set the "*

 * *            'compatibility option so that you maximize the chance that SPy will remain compatible '*

 * *            "with your notebook/script\\n'), (5, 'spy.options.compatibility = 188')], delete: "*

 * *            '[2]}}}'}*

```diff
@@ -4,15 +4,18 @@
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import pandas as pd\n",
                 "\n",
-                "from seeq import spy"
+                "from seeq import spy\n",
+                "\n",
+                "# Set the compatibility option so that you maximize the chance that SPy will remain compatible with your notebook/script\n",
+                "spy.options.compatibility = 188"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Parameterized Jobs\n",
```

### Comparing `seeq-spy-187.5/seeq/spy/docs/Documentation/Advanced Scheduling/Seeq Data Lab.jpg` & `seeq-spy-188.0/seeq/spy/docs/Documentation/Advanced Scheduling/Seeq Data Lab.jpg`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.5/seeq/spy/docs/Documentation/Asset Trees 1 - Introduction.ipynb` & `seeq-spy-188.0/seeq/spy/docs/Documentation/Asset Trees 1 - Introduction.ipynb`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9976094483932627%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(1, 'import pandas as pd\\n'), (2, '\\n'), (3, '# Set the "*

 * *            'compatibility option so that you maximize the chance that SPy will remain compatible '*

 * *            "with your notebook/script\\n'), (4, 'spy.options.compatibility = 188')], delete: "*

 * *            "[1]}}, 19: {'outputs': {0: {'data': {'text/html': ['<div "*

 * *            'style="background-color: #EEFFEE;color:black; text-align: left;">Query '*

 * *            'successful</div><table class="tex2jax_ignore" s […]*

```diff
@@ -4,15 +4,18 @@
             "cell_type": "code",
             "execution_count": 1,
             "id": "portuguese-morris",
             "metadata": {},
             "outputs": [],
             "source": [
                 "from seeq import spy\n",
-                "import pandas as pd"
+                "import pandas as pd\n",
+                "\n",
+                "# Set the compatibility option so that you maximize the chance that SPy will remain compatible with your notebook/script\n",
+                "spy.options.compatibility = 188"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "id": "logical-skill",
             "metadata": {},
@@ -359,15 +362,15 @@
             "execution_count": 8,
             "id": "agricultural-romantic",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<div style=\"background-color: #EEFFEE;color:black; text-align: left;\">Query successful</div><table class=\"tex2jax_ignore\" style=\"color:black;\"><tr><td style=\"background-color: #EEFFEE;\"></td><td style=\"background-color: #EEFFEE; text-align: left;\">Name</td><td style=\"background-color: #EEFFEE; text-align: left;\">Datasource Name</td><td style=\"background-color: #EEFFEE; text-align: left;\">Time</td><td style=\"background-color: #EEFFEE; text-align: right;\">Count</td><td style=\"background-color: #EEFFEE; text-align: right;\">Pages</td><td style=\"background-color: #EEFFEE; text-align: left;\">Result</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">0</td><td style=\"text-align: left; vertical-align: top;\">Area A_Temperature</td><td style=\"text-align: left; vertical-align: top;\">Example Data</td><td style=\"vertical-align: top;\">00:00:00.02</td><td style=\"text-align: right; vertical-align: top;\">1</td><td style=\"text-align: right; vertical-align: top;\">1</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr></table>"
+                            "<div style=\"background-color: #EEFFEE;color:black; text-align: left;\">Query successful</div><table class=\"tex2jax_ignore\" style=\"color:black;\"><tr><td style=\"background-color: #EEFFEE;\"></td><td style=\"background-color: #EEFFEE; text-align: left;\">Name</td><td style=\"background-color: #EEFFEE; text-align: left;\">Datasource Name</td><td style=\"background-color: #EEFFEE; text-align: left;\">Time</td><td style=\"background-color: #EEFFEE; text-align: right;\">Count</td><td style=\"background-color: #EEFFEE; text-align: right;\">Pages</td><td style=\"background-color: #EEFFEE; text-align: left;\">Result</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">0</td><td style=\"text-align: left; vertical-align: top;\">Area A_Temperature</td><td style=\"text-align: left; vertical-align: top;\">Example Data</td><td style=\"vertical-align: top;\">00:00:00.03</td><td style=\"text-align: right; vertical-align: top;\">1</td><td style=\"text-align: right; vertical-align: top;\">1</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr></table>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -887,15 +890,15 @@
             "metadata": {
                 "scrolled": true
             },
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<div style=\"background-color: #EEFFEE;color:black; text-align: left;\">Pushed successfully to datasource <strong>Seeq Data Lab [Datasource ID: Seeq Data Lab]</strong> and scoped to workbook ID <strong>95BED80D-BD27-4057-B0C9-E0920E699FEE</strong><br>Click the following link to see what you pushed in Seeq:<br><a href=\"http://localhost:34216/845E2BBC-786E-47F0-8B1D-95D2DC8A9EA8/workbook/95BED80D-BD27-4057-B0C9-E0920E699FEE/worksheet/CF02358A-51F6-40FF-8E86-F2A2717D0B60\" target=\"_new\">http://localhost:34216/845E2BBC-786E-47F0-8B1D-95D2DC8A9EA8/workbook/95BED80D-BD27-4057-B0C9-E0920E699FEE/worksheet/CF02358A-51F6-40FF-8E86-F2A2717D0B60</a></div>"
+                            "<div style=\"background-color: #EEFFEE;color:black; text-align: left;\">Pushed successfully to datasource <strong>Seeq Data Lab [Datasource ID: Seeq Data Lab]</strong> and scoped to workbook ID <strong>0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8</strong><br>Click the following link to see what you pushed in Seeq:<br><a href=\"http://localhost:34216/0EDF27BC-6135-FB90-8645-7859B3D869A9/workbook/0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8/worksheet/0EDF27BC-85E0-EEE0-955F-1C59612A3AAC\" target=\"_blank\">http://localhost:34216/0EDF27BC-6135-FB90-8645-7859B3D869A9/workbook/0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8/worksheet/0EDF27BC-85E0-EEE0-955F-1C59612A3AAC</a></div>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -943,515 +946,515 @@
                             "      <th>Push Result</th>\n",
                             "      <th>Cache Enabled</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
-                            "      <td>27112E05-700D-4D37-BDE1-E58A3E5B3192</td>\n",
+                            "      <td>0EDF27BC-9A95-7390-A7E6-11E67A7C0E5E</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td></td>\n",
                             "      <td>My CSV Tree</td>\n",
                             "      <td>Asset</td>\n",
                             "      <td>1</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>...</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>95BED80D-BD27-4057-B0C9-E0920E699FEE</td>\n",
+                            "      <td>0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[95BED80D-BD27-4057-B0C9-E0920E699FEE] {Asset}...</td>\n",
+                            "      <td>[0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Asset}...</td>\n",
                             "      <td>Success</td>\n",
                             "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1</th>\n",
-                            "      <td>57AF07FD-A462-4059-823C-70CB15B2A38D</td>\n",
+                            "      <td>0EDF27BC-9A97-EAA0-83CA-0063D1483D5A</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>My CSV Tree</td>\n",
                             "      <td>Cooling Tower 1</td>\n",
                             "      <td>Asset</td>\n",
                             "      <td>2</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>...</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>95BED80D-BD27-4057-B0C9-E0920E699FEE</td>\n",
+                            "      <td>0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[95BED80D-BD27-4057-B0C9-E0920E699FEE] {Asset}...</td>\n",
+                            "      <td>[0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Asset}...</td>\n",
                             "      <td>Success</td>\n",
                             "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2</th>\n",
-                            "      <td>9CBA46E2-D056-4BF2-A838-20717F05E42E</td>\n",
+                            "      <td>0EDF27BC-9A9A-71B0-9788-8AD734BC304E</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>My CSV Tree &gt;&gt; Cooling Tower 1</td>\n",
                             "      <td>Area A</td>\n",
                             "      <td>Asset</td>\n",
                             "      <td>3</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>...</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>95BED80D-BD27-4057-B0C9-E0920E699FEE</td>\n",
+                            "      <td>0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[95BED80D-BD27-4057-B0C9-E0920E699FEE] {Asset}...</td>\n",
+                            "      <td>[0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Asset}...</td>\n",
                             "      <td>Success</td>\n",
                             "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>3</th>\n",
-                            "      <td>9E2C4E48-8C5E-4C56-987B-0C32EF55A7A1</td>\n",
+                            "      <td>0EDF27BC-9C45-75A0-9BC0-F99719E614CA</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>My CSV Tree &gt;&gt; Cooling Tower 1 &gt;&gt; Area A</td>\n",
                             "      <td>Dew Point</td>\n",
                             "      <td>CalculatedSignal</td>\n",
                             "      <td>4</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>$t - ((100 - $rh.setUnits(\"\"))/5)</td>\n",
-                            "      <td>[rh=2076B897-598A-4A5B-9226-4ACB70423073, t=63...</td>\n",
+                            "      <td>[rh=0EDF27BC-99AA-FD90-9572-383FE2C37BA9, t=0E...</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>...</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>95BED80D-BD27-4057-B0C9-E0920E699FEE</td>\n",
+                            "      <td>0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[95BED80D-BD27-4057-B0C9-E0920E699FEE] {Signal...</td>\n",
+                            "      <td>[0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Signal...</td>\n",
                             "      <td>Success</td>\n",
                             "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>4</th>\n",
-                            "      <td>2076B897-598A-4A5B-9226-4ACB70423073</td>\n",
-                            "      <td>1FF81332-426C-4D21-A98C-AAEBA2F7B8DC</td>\n",
+                            "      <td>0EDF27BC-99AA-FD90-9572-383FE2C37BA9</td>\n",
+                            "      <td>0EDF27BA-DEC0-F9E0-8E96-D0178F21E874</td>\n",
                             "      <td>My CSV Tree &gt;&gt; Cooling Tower 1 &gt;&gt; Area A</td>\n",
                             "      <td>Relative Humidity</td>\n",
                             "      <td>CalculatedSignal</td>\n",
                             "      <td>4</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>$signal</td>\n",
-                            "      <td>[signal=1FF81332-426C-4D21-A98C-AAEBA2F7B8DC]</td>\n",
+                            "      <td>[signal=0EDF27BA-DEC0-F9E0-8E96-D0178F21E874]</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>...</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>95BED80D-BD27-4057-B0C9-E0920E699FEE</td>\n",
+                            "      <td>0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[95BED80D-BD27-4057-B0C9-E0920E699FEE] {Signal...</td>\n",
+                            "      <td>[0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Signal...</td>\n",
                             "      <td>Success</td>\n",
                             "      <td>False</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>5</th>\n",
-                            "      <td>63E8C7ED-A9F3-48AF-AB3F-099F114CFF37</td>\n",
-                            "      <td>C1391A12-665B-40B0-8334-BF5F1DBADDDD</td>\n",
+                            "      <td>0EDF27BC-99D1-EE90-9B64-84989AE7FADE</td>\n",
+                            "      <td>0EDF27BA-DEA8-7340-BB28-BCB11CC252BB</td>\n",
                             "      <td>My CSV Tree &gt;&gt; Cooling Tower 1 &gt;&gt; Area A</td>\n",
                             "      <td>Temperature</td>\n",
                             "      <td>CalculatedSignal</td>\n",
                             "      <td>4</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>$signal</td>\n",
-                            "      <td>[signal=C1391A12-665B-40B0-8334-BF5F1DBADDDD]</td>\n",
+                            "      <td>[signal=0EDF27BA-DEA8-7340-BB28-BCB11CC252BB]</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>...</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>95BED80D-BD27-4057-B0C9-E0920E699FEE</td>\n",
+                            "      <td>0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[95BED80D-BD27-4057-B0C9-E0920E699FEE] {Signal...</td>\n",
+                            "      <td>[0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Signal...</td>\n",
                             "      <td>Success</td>\n",
                             "      <td>False</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>6</th>\n",
-                            "      <td>45F3ED49-CF9C-485E-9DA7-70D7CCDB9A30</td>\n",
+                            "      <td>0EDF27BC-9A9A-71B0-8CC5-C3E4117635D5</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>My CSV Tree &gt;&gt; Cooling Tower 1</td>\n",
                             "      <td>Area B</td>\n",
                             "      <td>Asset</td>\n",
                             "      <td>3</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>...</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>95BED80D-BD27-4057-B0C9-E0920E699FEE</td>\n",
+                            "      <td>0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[95BED80D-BD27-4057-B0C9-E0920E699FEE] {Asset}...</td>\n",
+                            "      <td>[0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Asset}...</td>\n",
                             "      <td>Success</td>\n",
                             "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>7</th>\n",
-                            "      <td>863C9789-5F76-4C14-9664-78261C47D737</td>\n",
+                            "      <td>0EDF27BC-9C8E-F980-A215-63EA2C3EBF52</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>My CSV Tree &gt;&gt; Cooling Tower 1 &gt;&gt; Area B</td>\n",
                             "      <td>Dew Point</td>\n",
                             "      <td>CalculatedSignal</td>\n",
                             "      <td>4</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>$t - ((100 - $rh.setUnits(\"\"))/5)</td>\n",
-                            "      <td>[rh=BDC479E9-72A9-46CA-8DAC-254376253A7E, t=D7...</td>\n",
+                            "      <td>[rh=0EDF27BC-99F4-7170-B3A5-28C54491C37E, t=0E...</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>...</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>95BED80D-BD27-4057-B0C9-E0920E699FEE</td>\n",
+                            "      <td>0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[95BED80D-BD27-4057-B0C9-E0920E699FEE] {Signal...</td>\n",
+                            "      <td>[0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Signal...</td>\n",
                             "      <td>Success</td>\n",
                             "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>8</th>\n",
-                            "      <td>BDC479E9-72A9-46CA-8DAC-254376253A7E</td>\n",
-                            "      <td>F9DAFE9A-C4FB-4C51-8A39-BEB01672EA07</td>\n",
+                            "      <td>0EDF27BC-99F4-7170-B3A5-28C54491C37E</td>\n",
+                            "      <td>0EDF27BA-DEBB-FBC0-96F3-F56E271F0439</td>\n",
                             "      <td>My CSV Tree &gt;&gt; Cooling Tower 1 &gt;&gt; Area B</td>\n",
                             "      <td>Relative Humidity</td>\n",
                             "      <td>CalculatedSignal</td>\n",
                             "      <td>4</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>$signal</td>\n",
-                            "      <td>[signal=F9DAFE9A-C4FB-4C51-8A39-BEB01672EA07]</td>\n",
+                            "      <td>[signal=0EDF27BA-DEBB-FBC0-96F3-F56E271F0439]</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>...</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>95BED80D-BD27-4057-B0C9-E0920E699FEE</td>\n",
+                            "      <td>0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[95BED80D-BD27-4057-B0C9-E0920E699FEE] {Signal...</td>\n",
+                            "      <td>[0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Signal...</td>\n",
                             "      <td>Success</td>\n",
                             "      <td>False</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>9</th>\n",
-                            "      <td>D790C465-F0DB-4C29-8240-FBAE4DB86B32</td>\n",
-                            "      <td>7088C03A-CB16-40B0-B83A-7C478F0797E0</td>\n",
+                            "      <td>0EDF27BC-9A0E-FF20-98B5-AE82FB81DB20</td>\n",
+                            "      <td>0EDF27BA-DEB4-6690-9D71-02A0E4ED00F8</td>\n",
                             "      <td>My CSV Tree &gt;&gt; Cooling Tower 1 &gt;&gt; Area B</td>\n",
                             "      <td>Temperature</td>\n",
                             "      <td>CalculatedSignal</td>\n",
                             "      <td>4</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>$signal</td>\n",
-                            "      <td>[signal=7088C03A-CB16-40B0-B83A-7C478F0797E0]</td>\n",
+                            "      <td>[signal=0EDF27BA-DEB4-6690-9D71-02A0E4ED00F8]</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>...</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>95BED80D-BD27-4057-B0C9-E0920E699FEE</td>\n",
+                            "      <td>0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[95BED80D-BD27-4057-B0C9-E0920E699FEE] {Signal...</td>\n",
+                            "      <td>[0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Signal...</td>\n",
                             "      <td>Success</td>\n",
                             "      <td>False</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>10</th>\n",
-                            "      <td>4311E85D-C597-44A2-8FA1-24DFB698B0DD</td>\n",
+                            "      <td>0EDF27BC-9A9A-71B0-9CDA-34617BD25C9D</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>My CSV Tree</td>\n",
                             "      <td>Cooling Tower 2</td>\n",
                             "      <td>Asset</td>\n",
                             "      <td>2</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>...</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>95BED80D-BD27-4057-B0C9-E0920E699FEE</td>\n",
+                            "      <td>0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[95BED80D-BD27-4057-B0C9-E0920E699FEE] {Asset}...</td>\n",
+                            "      <td>[0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Asset}...</td>\n",
                             "      <td>Success</td>\n",
                             "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>11</th>\n",
-                            "      <td>79E60A20-01A4-4A08-9AD2-6EC2A20960E8</td>\n",
+                            "      <td>0EDF27BC-9A9A-71B0-B51C-8188F141D157</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>My CSV Tree &gt;&gt; Cooling Tower 2</td>\n",
                             "      <td>Area D</td>\n",
                             "      <td>Asset</td>\n",
                             "      <td>3</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>...</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>95BED80D-BD27-4057-B0C9-E0920E699FEE</td>\n",
+                            "      <td>0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[95BED80D-BD27-4057-B0C9-E0920E699FEE] {Asset}...</td>\n",
+                            "      <td>[0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Asset}...</td>\n",
                             "      <td>Success</td>\n",
                             "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>12</th>\n",
-                            "      <td>F20738AF-67D0-46F2-A92E-AAA8B40FCA6C</td>\n",
+                            "      <td>0EDF27BC-9CCB-EA10-AD88-1B5FA8264457</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>My CSV Tree &gt;&gt; Cooling Tower 2 &gt;&gt; Area D</td>\n",
                             "      <td>Dew Point</td>\n",
                             "      <td>CalculatedSignal</td>\n",
                             "      <td>4</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>$t - ((100 - $rh.setUnits(\"\"))/5)</td>\n",
-                            "      <td>[rh=A45FF098-A765-4281-A0E2-69ABFE00364F, t=73...</td>\n",
+                            "      <td>[rh=0EDF27BC-9A2E-EAF0-A371-C607B64C3404, t=0E...</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>...</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>95BED80D-BD27-4057-B0C9-E0920E699FEE</td>\n",
+                            "      <td>0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[95BED80D-BD27-4057-B0C9-E0920E699FEE] {Signal...</td>\n",
+                            "      <td>[0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Signal...</td>\n",
                             "      <td>Success</td>\n",
                             "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>13</th>\n",
-                            "      <td>A45FF098-A765-4281-A0E2-69ABFE00364F</td>\n",
-                            "      <td>1E521D48-3D1F-4274-8A0E-23E51220967A</td>\n",
+                            "      <td>0EDF27BC-9A2E-EAF0-A371-C607B64C3404</td>\n",
+                            "      <td>0EDF27BA-DEB1-FF80-9C7D-F951BA3A75CB</td>\n",
                             "      <td>My CSV Tree &gt;&gt; Cooling Tower 2 &gt;&gt; Area D</td>\n",
                             "      <td>Relative Humidity</td>\n",
                             "      <td>CalculatedSignal</td>\n",
                             "      <td>4</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>$signal</td>\n",
-                            "      <td>[signal=1E521D48-3D1F-4274-8A0E-23E51220967A]</td>\n",
+                            "      <td>[signal=0EDF27BA-DEB1-FF80-9C7D-F951BA3A75CB]</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>...</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>95BED80D-BD27-4057-B0C9-E0920E699FEE</td>\n",
+                            "      <td>0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[95BED80D-BD27-4057-B0C9-E0920E699FEE] {Signal...</td>\n",
+                            "      <td>[0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Signal...</td>\n",
                             "      <td>Success</td>\n",
                             "      <td>False</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>14</th>\n",
-                            "      <td>734B3D00-9850-4D51-B7A1-1A522C90F0B1</td>\n",
-                            "      <td>B0C6DB27-3814-4B4A-8338-F5133C763A33</td>\n",
+                            "      <td>0EDF27BC-9A47-7190-9A77-EE93227F46C6</td>\n",
+                            "      <td>0EDF27BA-E0AD-EC80-9DEF-842FAE6B4C27</td>\n",
                             "      <td>My CSV Tree &gt;&gt; Cooling Tower 2 &gt;&gt; Area D</td>\n",
                             "      <td>Temperature</td>\n",
                             "      <td>CalculatedSignal</td>\n",
                             "      <td>4</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>$signal</td>\n",
-                            "      <td>[signal=B0C6DB27-3814-4B4A-8338-F5133C763A33]</td>\n",
+                            "      <td>[signal=0EDF27BA-E0AD-EC80-9DEF-842FAE6B4C27]</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>...</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>95BED80D-BD27-4057-B0C9-E0920E699FEE</td>\n",
+                            "      <td>0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[95BED80D-BD27-4057-B0C9-E0920E699FEE] {Signal...</td>\n",
+                            "      <td>[0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Signal...</td>\n",
                             "      <td>Success</td>\n",
                             "      <td>False</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>15</th>\n",
-                            "      <td>CF61BA32-F42E-4E3B-A0A0-356DAD1E4CE9</td>\n",
+                            "      <td>0EDF27BC-9A9A-71B0-A7C6-3A10B9EE89D9</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>My CSV Tree &gt;&gt; Cooling Tower 2</td>\n",
                             "      <td>Area E</td>\n",
                             "      <td>Asset</td>\n",
                             "      <td>3</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>...</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>95BED80D-BD27-4057-B0C9-E0920E699FEE</td>\n",
+                            "      <td>0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[95BED80D-BD27-4057-B0C9-E0920E699FEE] {Asset}...</td>\n",
+                            "      <td>[0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Asset}...</td>\n",
                             "      <td>Success</td>\n",
                             "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>16</th>\n",
-                            "      <td>AE71C1B9-F198-4C61-A128-174AA4BD9987</td>\n",
+                            "      <td>0EDF27BC-9D0B-71B0-856B-00D6368974BB</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>My CSV Tree &gt;&gt; Cooling Tower 2 &gt;&gt; Area E</td>\n",
                             "      <td>Dew Point</td>\n",
                             "      <td>CalculatedSignal</td>\n",
                             "      <td>4</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>$t - ((100 - $rh.setUnits(\"\"))/5)</td>\n",
-                            "      <td>[rh=0012B79D-E4FC-4589-A711-2D4706F38039, t=C9...</td>\n",
+                            "      <td>[rh=0EDF27BC-9A61-FF40-A7F7-5125E6DF8637, t=0E...</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>...</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>95BED80D-BD27-4057-B0C9-E0920E699FEE</td>\n",
+                            "      <td>0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[95BED80D-BD27-4057-B0C9-E0920E699FEE] {Signal...</td>\n",
+                            "      <td>[0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Signal...</td>\n",
                             "      <td>Success</td>\n",
                             "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>17</th>\n",
-                            "      <td>0012B79D-E4FC-4589-A711-2D4706F38039</td>\n",
-                            "      <td>6B68E870-1C98-4D1C-AACF-550D70540771</td>\n",
+                            "      <td>0EDF27BC-9A61-FF40-A7F7-5125E6DF8637</td>\n",
+                            "      <td>0EDF27BA-E089-6290-ABF3-D84F99D009F9</td>\n",
                             "      <td>My CSV Tree &gt;&gt; Cooling Tower 2 &gt;&gt; Area E</td>\n",
                             "      <td>Relative Humidity</td>\n",
                             "      <td>CalculatedSignal</td>\n",
                             "      <td>4</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>$signal</td>\n",
-                            "      <td>[signal=6B68E870-1C98-4D1C-AACF-550D70540771]</td>\n",
+                            "      <td>[signal=0EDF27BA-E089-6290-ABF3-D84F99D009F9]</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>...</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>95BED80D-BD27-4057-B0C9-E0920E699FEE</td>\n",
+                            "      <td>0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[95BED80D-BD27-4057-B0C9-E0920E699FEE] {Signal...</td>\n",
+                            "      <td>[0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Signal...</td>\n",
                             "      <td>Success</td>\n",
                             "      <td>False</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>18</th>\n",
-                            "      <td>C971DD89-A3F0-41E9-B491-8E3F400A10DC</td>\n",
-                            "      <td>8D80EE1E-585D-4F37-95D4-C0F31865CBBB</td>\n",
+                            "      <td>0EDF27BC-9A7A-75E0-8160-F88E06BD59E5</td>\n",
+                            "      <td>0EDF27BA-E0CD-E850-BA67-375F032E2CB9</td>\n",
                             "      <td>My CSV Tree &gt;&gt; Cooling Tower 2 &gt;&gt; Area E</td>\n",
                             "      <td>Temperature</td>\n",
                             "      <td>CalculatedSignal</td>\n",
                             "      <td>4</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>$signal</td>\n",
-                            "      <td>[signal=8D80EE1E-585D-4F37-95D4-C0F31865CBBB]</td>\n",
+                            "      <td>[signal=0EDF27BA-E0CD-E850-BA67-375F032E2CB9]</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>...</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>95BED80D-BD27-4057-B0C9-E0920E699FEE</td>\n",
+                            "      <td>0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[95BED80D-BD27-4057-B0C9-E0920E699FEE] {Signal...</td>\n",
+                            "      <td>[0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Signal...</td>\n",
                             "      <td>Success</td>\n",
                             "      <td>False</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "<p>19 rows \u00d7 29 columns</p>\n",
                             "</div>"
                         ],
                         "text/plain": [
                             "                                      ID  \\\n",
-                            "0   27112E05-700D-4D37-BDE1-E58A3E5B3192   \n",
-                            "1   57AF07FD-A462-4059-823C-70CB15B2A38D   \n",
-                            "2   9CBA46E2-D056-4BF2-A838-20717F05E42E   \n",
-                            "3   9E2C4E48-8C5E-4C56-987B-0C32EF55A7A1   \n",
-                            "4   2076B897-598A-4A5B-9226-4ACB70423073   \n",
-                            "5   63E8C7ED-A9F3-48AF-AB3F-099F114CFF37   \n",
-                            "6   45F3ED49-CF9C-485E-9DA7-70D7CCDB9A30   \n",
-                            "7   863C9789-5F76-4C14-9664-78261C47D737   \n",
-                            "8   BDC479E9-72A9-46CA-8DAC-254376253A7E   \n",
-                            "9   D790C465-F0DB-4C29-8240-FBAE4DB86B32   \n",
-                            "10  4311E85D-C597-44A2-8FA1-24DFB698B0DD   \n",
-                            "11  79E60A20-01A4-4A08-9AD2-6EC2A20960E8   \n",
-                            "12  F20738AF-67D0-46F2-A92E-AAA8B40FCA6C   \n",
-                            "13  A45FF098-A765-4281-A0E2-69ABFE00364F   \n",
-                            "14  734B3D00-9850-4D51-B7A1-1A522C90F0B1   \n",
-                            "15  CF61BA32-F42E-4E3B-A0A0-356DAD1E4CE9   \n",
-                            "16  AE71C1B9-F198-4C61-A128-174AA4BD9987   \n",
-                            "17  0012B79D-E4FC-4589-A711-2D4706F38039   \n",
-                            "18  C971DD89-A3F0-41E9-B491-8E3F400A10DC   \n",
+                            "0   0EDF27BC-9A95-7390-A7E6-11E67A7C0E5E   \n",
+                            "1   0EDF27BC-9A97-EAA0-83CA-0063D1483D5A   \n",
+                            "2   0EDF27BC-9A9A-71B0-9788-8AD734BC304E   \n",
+                            "3   0EDF27BC-9C45-75A0-9BC0-F99719E614CA   \n",
+                            "4   0EDF27BC-99AA-FD90-9572-383FE2C37BA9   \n",
+                            "5   0EDF27BC-99D1-EE90-9B64-84989AE7FADE   \n",
+                            "6   0EDF27BC-9A9A-71B0-8CC5-C3E4117635D5   \n",
+                            "7   0EDF27BC-9C8E-F980-A215-63EA2C3EBF52   \n",
+                            "8   0EDF27BC-99F4-7170-B3A5-28C54491C37E   \n",
+                            "9   0EDF27BC-9A0E-FF20-98B5-AE82FB81DB20   \n",
+                            "10  0EDF27BC-9A9A-71B0-9CDA-34617BD25C9D   \n",
+                            "11  0EDF27BC-9A9A-71B0-B51C-8188F141D157   \n",
+                            "12  0EDF27BC-9CCB-EA10-AD88-1B5FA8264457   \n",
+                            "13  0EDF27BC-9A2E-EAF0-A371-C607B64C3404   \n",
+                            "14  0EDF27BC-9A47-7190-9A77-EE93227F46C6   \n",
+                            "15  0EDF27BC-9A9A-71B0-A7C6-3A10B9EE89D9   \n",
+                            "16  0EDF27BC-9D0B-71B0-856B-00D6368974BB   \n",
+                            "17  0EDF27BC-9A61-FF40-A7F7-5125E6DF8637   \n",
+                            "18  0EDF27BC-9A7A-75E0-8160-F88E06BD59E5   \n",
                             "\n",
                             "                           Referenced ID  \\\n",
                             "0                                    NaN   \n",
                             "1                                    NaN   \n",
                             "2                                    NaN   \n",
                             "3                                    NaN   \n",
-                            "4   1FF81332-426C-4D21-A98C-AAEBA2F7B8DC   \n",
-                            "5   C1391A12-665B-40B0-8334-BF5F1DBADDDD   \n",
+                            "4   0EDF27BA-DEC0-F9E0-8E96-D0178F21E874   \n",
+                            "5   0EDF27BA-DEA8-7340-BB28-BCB11CC252BB   \n",
                             "6                                    NaN   \n",
                             "7                                    NaN   \n",
-                            "8   F9DAFE9A-C4FB-4C51-8A39-BEB01672EA07   \n",
-                            "9   7088C03A-CB16-40B0-B83A-7C478F0797E0   \n",
+                            "8   0EDF27BA-DEBB-FBC0-96F3-F56E271F0439   \n",
+                            "9   0EDF27BA-DEB4-6690-9D71-02A0E4ED00F8   \n",
                             "10                                   NaN   \n",
                             "11                                   NaN   \n",
                             "12                                   NaN   \n",
-                            "13  1E521D48-3D1F-4274-8A0E-23E51220967A   \n",
-                            "14  B0C6DB27-3814-4B4A-8338-F5133C763A33   \n",
+                            "13  0EDF27BA-DEB1-FF80-9C7D-F951BA3A75CB   \n",
+                            "14  0EDF27BA-E0AD-EC80-9DEF-842FAE6B4C27   \n",
                             "15                                   NaN   \n",
                             "16                                   NaN   \n",
-                            "17  6B68E870-1C98-4D1C-AACF-550D70540771   \n",
-                            "18  8D80EE1E-585D-4F37-95D4-C0F31865CBBB   \n",
+                            "17  0EDF27BA-E089-6290-ABF3-D84F99D009F9   \n",
+                            "18  0EDF27BA-E0CD-E850-BA67-375F032E2CB9   \n",
                             "\n",
                             "                                        Path               Name  \\\n",
                             "0                                                   My CSV Tree   \n",
                             "1                                My CSV Tree    Cooling Tower 1   \n",
                             "2             My CSV Tree >> Cooling Tower 1             Area A   \n",
                             "3   My CSV Tree >> Cooling Tower 1 >> Area A          Dew Point   \n",
                             "4   My CSV Tree >> Cooling Tower 1 >> Area A  Relative Humidity   \n",
@@ -1491,30 +1494,30 @@
                             "17  CalculatedSignal      4          NaN                            $signal   \n",
                             "18  CalculatedSignal      4          NaN                            $signal   \n",
                             "\n",
                             "                                   Formula Parameters  Roll Up Statistic  ...  \\\n",
                             "0                                                 NaN                NaN  ...   \n",
                             "1                                                 NaN                NaN  ...   \n",
                             "2                                                 NaN                NaN  ...   \n",
-                            "3   [rh=2076B897-598A-4A5B-9226-4ACB70423073, t=63...                NaN  ...   \n",
-                            "4       [signal=1FF81332-426C-4D21-A98C-AAEBA2F7B8DC]                NaN  ...   \n",
-                            "5       [signal=C1391A12-665B-40B0-8334-BF5F1DBADDDD]                NaN  ...   \n",
+                            "3   [rh=0EDF27BC-99AA-FD90-9572-383FE2C37BA9, t=0E...                NaN  ...   \n",
+                            "4       [signal=0EDF27BA-DEC0-F9E0-8E96-D0178F21E874]                NaN  ...   \n",
+                            "5       [signal=0EDF27BA-DEA8-7340-BB28-BCB11CC252BB]                NaN  ...   \n",
                             "6                                                 NaN                NaN  ...   \n",
-                            "7   [rh=BDC479E9-72A9-46CA-8DAC-254376253A7E, t=D7...                NaN  ...   \n",
-                            "8       [signal=F9DAFE9A-C4FB-4C51-8A39-BEB01672EA07]                NaN  ...   \n",
-                            "9       [signal=7088C03A-CB16-40B0-B83A-7C478F0797E0]                NaN  ...   \n",
+                            "7   [rh=0EDF27BC-99F4-7170-B3A5-28C54491C37E, t=0E...                NaN  ...   \n",
+                            "8       [signal=0EDF27BA-DEBB-FBC0-96F3-F56E271F0439]                NaN  ...   \n",
+                            "9       [signal=0EDF27BA-DEB4-6690-9D71-02A0E4ED00F8]                NaN  ...   \n",
                             "10                                                NaN                NaN  ...   \n",
                             "11                                                NaN                NaN  ...   \n",
-                            "12  [rh=A45FF098-A765-4281-A0E2-69ABFE00364F, t=73...                NaN  ...   \n",
-                            "13      [signal=1E521D48-3D1F-4274-8A0E-23E51220967A]                NaN  ...   \n",
-                            "14      [signal=B0C6DB27-3814-4B4A-8338-F5133C763A33]                NaN  ...   \n",
+                            "12  [rh=0EDF27BC-9A2E-EAF0-A371-C607B64C3404, t=0E...                NaN  ...   \n",
+                            "13      [signal=0EDF27BA-DEB1-FF80-9C7D-F951BA3A75CB]                NaN  ...   \n",
+                            "14      [signal=0EDF27BA-E0AD-EC80-9DEF-842FAE6B4C27]                NaN  ...   \n",
                             "15                                                NaN                NaN  ...   \n",
-                            "16  [rh=0012B79D-E4FC-4589-A711-2D4706F38039, t=C9...                NaN  ...   \n",
-                            "17      [signal=6B68E870-1C98-4D1C-AACF-550D70540771]                NaN  ...   \n",
-                            "18      [signal=8D80EE1E-585D-4F37-95D4-C0F31865CBBB]                NaN  ...   \n",
+                            "16  [rh=0EDF27BC-9A61-FF40-A7F7-5125E6DF8637, t=0E...                NaN  ...   \n",
+                            "17      [signal=0EDF27BA-E089-6290-ABF3-D84F99D009F9]                NaN  ...   \n",
+                            "18      [signal=0EDF27BA-E0CD-E850-BA67-375F032E2CB9]                NaN  ...   \n",
                             "\n",
                             "    Period  Process Type  Thresholds  Template ID  \\\n",
                             "0      NaN           NaN         NaN          NaN   \n",
                             "1      NaN           NaN         NaN          NaN   \n",
                             "2      NaN           NaN         NaN          NaN   \n",
                             "3      NaN           NaN         NaN          NaN   \n",
                             "4      NaN           NaN         NaN          NaN   \n",
@@ -1530,54 +1533,54 @@
                             "14     NaN           NaN         NaN          NaN   \n",
                             "15     NaN           NaN         NaN          NaN   \n",
                             "16     NaN           NaN         NaN          NaN   \n",
                             "17     NaN           NaN         NaN          NaN   \n",
                             "18     NaN           NaN         NaN          NaN   \n",
                             "\n",
                             "                               Scoped To  Datasource Class  Datasource ID  \\\n",
-                            "0   95BED80D-BD27-4057-B0C9-E0920E699FEE     Seeq Data Lab  Seeq Data Lab   \n",
-                            "1   95BED80D-BD27-4057-B0C9-E0920E699FEE     Seeq Data Lab  Seeq Data Lab   \n",
-                            "2   95BED80D-BD27-4057-B0C9-E0920E699FEE     Seeq Data Lab  Seeq Data Lab   \n",
-                            "3   95BED80D-BD27-4057-B0C9-E0920E699FEE     Seeq Data Lab  Seeq Data Lab   \n",
-                            "4   95BED80D-BD27-4057-B0C9-E0920E699FEE     Seeq Data Lab  Seeq Data Lab   \n",
-                            "5   95BED80D-BD27-4057-B0C9-E0920E699FEE     Seeq Data Lab  Seeq Data Lab   \n",
-                            "6   95BED80D-BD27-4057-B0C9-E0920E699FEE     Seeq Data Lab  Seeq Data Lab   \n",
-                            "7   95BED80D-BD27-4057-B0C9-E0920E699FEE     Seeq Data Lab  Seeq Data Lab   \n",
-                            "8   95BED80D-BD27-4057-B0C9-E0920E699FEE     Seeq Data Lab  Seeq Data Lab   \n",
-                            "9   95BED80D-BD27-4057-B0C9-E0920E699FEE     Seeq Data Lab  Seeq Data Lab   \n",
-                            "10  95BED80D-BD27-4057-B0C9-E0920E699FEE     Seeq Data Lab  Seeq Data Lab   \n",
-                            "11  95BED80D-BD27-4057-B0C9-E0920E699FEE     Seeq Data Lab  Seeq Data Lab   \n",
-                            "12  95BED80D-BD27-4057-B0C9-E0920E699FEE     Seeq Data Lab  Seeq Data Lab   \n",
-                            "13  95BED80D-BD27-4057-B0C9-E0920E699FEE     Seeq Data Lab  Seeq Data Lab   \n",
-                            "14  95BED80D-BD27-4057-B0C9-E0920E699FEE     Seeq Data Lab  Seeq Data Lab   \n",
-                            "15  95BED80D-BD27-4057-B0C9-E0920E699FEE     Seeq Data Lab  Seeq Data Lab   \n",
-                            "16  95BED80D-BD27-4057-B0C9-E0920E699FEE     Seeq Data Lab  Seeq Data Lab   \n",
-                            "17  95BED80D-BD27-4057-B0C9-E0920E699FEE     Seeq Data Lab  Seeq Data Lab   \n",
-                            "18  95BED80D-BD27-4057-B0C9-E0920E699FEE     Seeq Data Lab  Seeq Data Lab   \n",
+                            "0   0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8     Seeq Data Lab  Seeq Data Lab   \n",
+                            "1   0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8     Seeq Data Lab  Seeq Data Lab   \n",
+                            "2   0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8     Seeq Data Lab  Seeq Data Lab   \n",
+                            "3   0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8     Seeq Data Lab  Seeq Data Lab   \n",
+                            "4   0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8     Seeq Data Lab  Seeq Data Lab   \n",
+                            "5   0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8     Seeq Data Lab  Seeq Data Lab   \n",
+                            "6   0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8     Seeq Data Lab  Seeq Data Lab   \n",
+                            "7   0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8     Seeq Data Lab  Seeq Data Lab   \n",
+                            "8   0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8     Seeq Data Lab  Seeq Data Lab   \n",
+                            "9   0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8     Seeq Data Lab  Seeq Data Lab   \n",
+                            "10  0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8     Seeq Data Lab  Seeq Data Lab   \n",
+                            "11  0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8     Seeq Data Lab  Seeq Data Lab   \n",
+                            "12  0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8     Seeq Data Lab  Seeq Data Lab   \n",
+                            "13  0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8     Seeq Data Lab  Seeq Data Lab   \n",
+                            "14  0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8     Seeq Data Lab  Seeq Data Lab   \n",
+                            "15  0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8     Seeq Data Lab  Seeq Data Lab   \n",
+                            "16  0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8     Seeq Data Lab  Seeq Data Lab   \n",
+                            "17  0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8     Seeq Data Lab  Seeq Data Lab   \n",
+                            "18  0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8     Seeq Data Lab  Seeq Data Lab   \n",
                             "\n",
                             "                                              Data ID  Push Result  \\\n",
-                            "0   [95BED80D-BD27-4057-B0C9-E0920E699FEE] {Asset}...      Success   \n",
-                            "1   [95BED80D-BD27-4057-B0C9-E0920E699FEE] {Asset}...      Success   \n",
-                            "2   [95BED80D-BD27-4057-B0C9-E0920E699FEE] {Asset}...      Success   \n",
-                            "3   [95BED80D-BD27-4057-B0C9-E0920E699FEE] {Signal...      Success   \n",
-                            "4   [95BED80D-BD27-4057-B0C9-E0920E699FEE] {Signal...      Success   \n",
-                            "5   [95BED80D-BD27-4057-B0C9-E0920E699FEE] {Signal...      Success   \n",
-                            "6   [95BED80D-BD27-4057-B0C9-E0920E699FEE] {Asset}...      Success   \n",
-                            "7   [95BED80D-BD27-4057-B0C9-E0920E699FEE] {Signal...      Success   \n",
-                            "8   [95BED80D-BD27-4057-B0C9-E0920E699FEE] {Signal...      Success   \n",
-                            "9   [95BED80D-BD27-4057-B0C9-E0920E699FEE] {Signal...      Success   \n",
-                            "10  [95BED80D-BD27-4057-B0C9-E0920E699FEE] {Asset}...      Success   \n",
-                            "11  [95BED80D-BD27-4057-B0C9-E0920E699FEE] {Asset}...      Success   \n",
-                            "12  [95BED80D-BD27-4057-B0C9-E0920E699FEE] {Signal...      Success   \n",
-                            "13  [95BED80D-BD27-4057-B0C9-E0920E699FEE] {Signal...      Success   \n",
-                            "14  [95BED80D-BD27-4057-B0C9-E0920E699FEE] {Signal...      Success   \n",
-                            "15  [95BED80D-BD27-4057-B0C9-E0920E699FEE] {Asset}...      Success   \n",
-                            "16  [95BED80D-BD27-4057-B0C9-E0920E699FEE] {Signal...      Success   \n",
-                            "17  [95BED80D-BD27-4057-B0C9-E0920E699FEE] {Signal...      Success   \n",
-                            "18  [95BED80D-BD27-4057-B0C9-E0920E699FEE] {Signal...      Success   \n",
+                            "0   [0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Asset}...      Success   \n",
+                            "1   [0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Asset}...      Success   \n",
+                            "2   [0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Asset}...      Success   \n",
+                            "3   [0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Signal...      Success   \n",
+                            "4   [0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Signal...      Success   \n",
+                            "5   [0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Signal...      Success   \n",
+                            "6   [0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Asset}...      Success   \n",
+                            "7   [0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Signal...      Success   \n",
+                            "8   [0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Signal...      Success   \n",
+                            "9   [0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Signal...      Success   \n",
+                            "10  [0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Asset}...      Success   \n",
+                            "11  [0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Asset}...      Success   \n",
+                            "12  [0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Signal...      Success   \n",
+                            "13  [0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Signal...      Success   \n",
+                            "14  [0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Signal...      Success   \n",
+                            "15  [0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Asset}...      Success   \n",
+                            "16  [0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Signal...      Success   \n",
+                            "17  [0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Signal...      Success   \n",
+                            "18  [0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Signal...      Success   \n",
                             "\n",
                             "    Cache Enabled  \n",
                             "0             NaN  \n",
                             "1             NaN  \n",
                             "2             NaN  \n",
                             "3             NaN  \n",
                             "4           False  \n",
@@ -1692,36 +1695,41 @@
                         " |  description : str, optional\n",
                         " |      The description to set on the root-level asset.\n",
                         " |  \n",
                         " |  workbook : str, default 'Data Lab >> Data Lab Analysis'\n",
                         " |      The path to a workbook (in the form of 'Folder >> Path >> Workbook Name')\n",
                         " |      or an ID that all pushed items will be 'scoped to'. You can\n",
                         " |      push to the Corporate folder by using the following pattern:\n",
-                        " |      '__Corporate__ >> Folder >> Path >> Workbook Name'. A Tree currently\n",
-                        " |      may not be globally scoped. These items will not be visible/searchable\n",
-                        " |      using the data panel in other workbooks.\n",
-                        " |  \n",
-                        " |  datasource : str, optional\n",
-                        " |      The name of the datasource within which to contain all the\n",
-                        " |      pushed items. By default, all pushed items will be contained in a \"Seeq\n",
-                        " |      Data Lab\" datasource. Do not create new datasources unless you really\n",
-                        " |      want to and you have permission from your administrator.\n",
-                        " |  \n",
-                        " |      convert_displays_to_sdl : bool, default True\n",
-                        " |          If True, then if displays from a non-Seeq Data Lab datasource are found in\n",
-                        " |          a tree that is otherwise from a Seeq Data Lab datasource, then they will\n",
-                        " |          be replaced by displays from a Seeq Data Lab datasource when this tree\n",
-                        " |          is pushed.\n",
-                        " |  \n",
-                        " |      quiet : bool, default False\n",
-                        " |          If True, suppresses progress output. This setting will be the default for all\n",
-                        " |          operations on this Tree. This option can be changed later using\n",
-                        " |          `tree.quiet = True` or by specifying the option for individual function calls.\n",
-                        " |          Note that when status is provided, the quiet setting of the Status object\n",
-                        " |          that is passed in takes precedent.\n",
+                        " |      '__Corporate__ >> Folder >> Path >> Workbook Name'. Scoped items will not\n",
+                        " |      be visible/searchable using the data panel in other workbooks.\n",
+                        " |      A Tree can be globally scoped (and therefore visible across all\n",
+                        " |      workbooks) by specifying workbook=None.\n",
+                        " |  \n",
+                        " |  datasource : str, optional, default 'Seeq Data Lab'\n",
+                        " |      The name of the datasource within which to contain all the pushed items.\n",
+                        " |      Items inherit access control permissions from their datasource unless it\n",
+                        " |      has been overridden at a lower level. If you specify a datasource using\n",
+                        " |      this argument, you can later manage access control (using spy.acl functions)\n",
+                        " |      at the datasource level for all the items you have pushed.\n",
+                        " |  \n",
+                        " |      If you instead want access control for your items to be inherited from the\n",
+                        " |      workbook they are scoped to, specify `spy.INHERIT_FROM_WORKBOOK`.\n",
+                        " |  \n",
+                        " |  convert_displays_to_sdl : bool, default True\n",
+                        " |      If True, then if displays from a non-Seeq Data Lab datasource are found in\n",
+                        " |      a tree that is otherwise from a Seeq Data Lab datasource, then they will\n",
+                        " |      be replaced by displays from a Seeq Data Lab datasource when this tree\n",
+                        " |      is pushed.\n",
+                        " |  \n",
+                        " |  quiet : bool, default False\n",
+                        " |      If True, suppresses progress output. This setting will be the default for all\n",
+                        " |      operations on this Tree. This option can be changed later using\n",
+                        " |      `tree.quiet = True` or by specifying the option for individual function calls.\n",
+                        " |      Note that when status is provided, the quiet setting of the Status object\n",
+                        " |      that is passed in takes precedence.\n",
                         " |  \n",
                         " |  errors : {'raise', 'catalog'}, default 'raise'\n",
                         " |      If 'raise', any errors encountered will cause an exception. If 'catalog',\n",
                         " |      errors will be added to a 'Result' column in the status.df DataFrame. The\n",
                         " |      option chosen here will be the default for all other operations on this Tree.\n",
                         " |      This option can be changed later using `tree.errors = 'catalog'` or by\n",
                         " |      specifying the option for individual function calls.\n",
@@ -1800,15 +1808,20 @@
                         " |          for an asset or calculation to be inserted.\n",
                         " |      \n",
                         " |      formula : str, optional\n",
                         " |          The formula for a calculated item. The `formula` and `formula_parameters` are\n",
                         " |          used in place of the `children` argument.\n",
                         " |      \n",
                         " |      formula_parameters : dict, optional\n",
-                        " |          The parameters for a formula.\n",
+                        " |          The parameters used in the specified `formula`. The following options are allowed:\n",
+                        " |      \n",
+                        " |          1) The name of an item that is an asset sibling of this calculation.\n",
+                        " |          2) The relative path to an item in this Tree (E.G. '.. >> Area E >> Temperature').\n",
+                        " |          3) The absolute path to an item in this Tree (E.G. 'Example >> Cooling Tower 2 >> Area E >> Temperature').\n",
+                        " |          4) The ID of an item (including ones not in the Tree).\n",
                         " |      \n",
                         " |      roll_up_statistic : str, optional\n",
                         " |          The statistic to use when inserting a roll-up calculation. Valid options are\n",
                         " |          Average, Maximum, Minimum, Range, Sum, Multiply, Union, Intersect, Counts,\n",
                         " |          Count Overlaps, Combine With.\n",
                         " |      \n",
                         " |      roll_up_parameters : str, optional\n",
@@ -1828,15 +1841,15 @@
                         " |          input will be used only for the duration of this function; it will default\n",
                         " |          to the setting on the Tree if not specified.\n",
                         " |      \n",
                         " |      quiet : bool, optional\n",
                         " |          If True, suppresses progress output. This input will be used only for the\n",
                         " |          duration of this function; it will default to the setting on the Tree if\n",
                         " |          not specified. Note that when status is provided, the quiet setting of\n",
-                        " |          the Status object that is passed in takes precedent.\n",
+                        " |          the Status object that is passed in takes precedence.\n",
                         " |      \n",
                         " |      status : spy.Status, optional\n",
                         " |          If specified, the supplied Status object will be updated as the command\n",
                         " |          progresses. It gets filled in with the same information you would see\n",
                         " |          in Jupyter in the blue/green/red table below your code while the\n",
                         " |          command is executed. The table itself is accessible as a DataFrame via\n",
                         " |          the status.df property.\n",
@@ -1884,24 +1897,24 @@
                         " |          input will be used only for the duration of this function; it will default\n",
                         " |          to the setting on the Tree if not specified.\n",
                         " |      \n",
                         " |      quiet : bool, optional\n",
                         " |          If True, suppresses progress output. This input will be used only for the\n",
                         " |          duration of this function; it will default to the setting on the Tree if\n",
                         " |          not specified. Note that when status is provided, the quiet setting of\n",
-                        " |          the Status object that is passed in takes precedent.\n",
+                        " |          the Status object that is passed in takes precedence.\n",
                         " |      \n",
                         " |      status : spy.Status, optional\n",
                         " |          If specified, the supplied Status object will be updated as the command\n",
                         " |          progresses. It gets filled in with the same information you would see\n",
                         " |          in Jupyter in the blue/green/red table below your code while the\n",
                         " |          command is executed. The table itself is accessible as a DataFrame via\n",
                         " |          the status.df property.\n",
                         " |  \n",
-                        " |  push(self, *, metadata_state_file=None, errors=None, quiet=None, status=None)\n",
+                        " |  push(self, *, metadata_state_file: 'Optional[str]' = None, errors: 'Optional[str]' = None, quiet: 'Optional[bool]' = None, status: 'Optional[Status]' = None) -> 'pd.DataFrame'\n",
                         " |      Imports the tree into Seeq Server.\n",
                         " |      \n",
                         " |      metadata_state_file : str, optional\n",
                         " |          The file name (with full path, if desired) to a \"metadata state file\"\n",
                         " |          to use for \"incremental\" pushing, which can dramatically speed up\n",
                         " |          pushing of a large asset tree. If supplied, the metadata push\n",
                         " |          operation uses the state file to determine what changed since the\n",
@@ -1914,22 +1927,29 @@
                         " |          input will be used only for the duration of this function; it will default\n",
                         " |          to the setting on the Tree if not specified.\n",
                         " |      \n",
                         " |      quiet : bool, optional\n",
                         " |          If True, suppresses progress output. This input will be used only for the\n",
                         " |          duration of this function; it will default to the setting on the Tree if\n",
                         " |          not specified. Note that when status is provided, the quiet setting of\n",
-                        " |          the Status object that is passed in takes precedent.\n",
+                        " |          the Status object that is passed in takes precedence.\n",
                         " |      \n",
                         " |      status : spy.Status, optional\n",
                         " |          If specified, the supplied Status object will be updated as the command\n",
                         " |          progresses. It gets filled in with the same information you would see\n",
                         " |          in Jupyter in the blue/green/red table below your code while the\n",
                         " |          command is executed. The table itself is accessible as a DataFrame via\n",
                         " |          the status.df property.\n",
+                        " |      \n",
+                        " |      Returns\n",
+                        " |      -------\n",
+                        " |      pandas.DataFrame\n",
+                        " |          A DataFrame with the metadata for the items pushed, along with any\n",
+                        " |          errors and statistics about the operation. See spy.push()\n",
+                        " |          documentation for further details on this returned DataFrame.\n",
                         " |  \n",
                         " |  remove(self, elements, *, errors=None, quiet=None, status=None)\n",
                         " |      Remove the specified elements from the tree recursively.\n",
                         " |      \n",
                         " |      Parameters\n",
                         " |      ----------\n",
                         " |      elements : {pandas.DataFrame, str, int}\n",
@@ -1950,15 +1970,15 @@
                         " |          input will be used only for the duration of this function; it will default\n",
                         " |          to the setting on the Tree if not specified.\n",
                         " |      \n",
                         " |      quiet : bool, optional\n",
                         " |          If True, suppresses progress output. This input will be used only for the\n",
                         " |          duration of this function; it will default to the setting on the Tree if\n",
                         " |          not specified. Note that when status is provided, the quiet setting of\n",
-                        " |          the Status object that is passed in takes precedent.\n",
+                        " |          the Status object that is passed in takes precedence.\n",
                         " |      \n",
                         " |      status : spy.Status, optional\n",
                         " |          If specified, the supplied Status object will be updated as the command\n",
                         " |          progresses. It gets filled in with the same information you would see\n",
                         " |          in Jupyter in the blue/green/red table below your code while the\n",
                         " |          command is executed. The table itself is accessible as a DataFrame via\n",
                         " |          the status.df property.\n",
@@ -2001,15 +2021,15 @@
                         " |          input will be used only for the duration of this function; it will default\n",
                         " |          to the setting on the Tree if not specified.\n",
                         " |      \n",
                         " |      quiet : bool, optional\n",
                         " |          If True, suppresses progress output. This input will be used only for the\n",
                         " |          duration of this function; it will default to the setting on the Tree if\n",
                         " |          not specified. Note that when status is provided, the quiet setting of\n",
-                        " |          the Status object that is passed in takes precedent.\n",
+                        " |          the Status object that is passed in takes precedence.\n",
                         " |      \n",
                         " |      status : spy.Status, optional\n",
                         " |          If specified, the supplied Status object will be updated as the command\n",
                         " |          progresses. It gets filled in with the same information you would see\n",
                         " |          in Jupyter in the blue/green/red table below your code while the\n",
                         " |          command is executed. The table itself is accessible as a DataFrame via\n",
                         " |          the status.df property.\n",
@@ -2036,31 +2056,34 @@
                         " |      subtree : str, optional\n",
                         " |          Specifies an asset in the tree. Only the part of the tree below this asset\n",
                         " |          will be visualized.\n",
                         " |      print_tree: bool, optional\n",
                         " |          True (default) to print the tree visualization, False to return it as a string\n",
                         " |  \n",
                         " |  ----------------------------------------------------------------------\n",
+                        " |  Readonly properties defined here:\n",
+                        " |  \n",
+                        " |  height\n",
+                        " |      Property that gives the current height of the tree. This is the length\n",
+                        " |      of the longest item path within the tree.\n",
+                        " |  \n",
+                        " |  size\n",
+                        " |      Property that gives the number of elements currently in the tree.\n",
+                        " |  \n",
+                        " |  ----------------------------------------------------------------------\n",
                         " |  Data descriptors defined here:\n",
                         " |  \n",
                         " |  __dict__\n",
                         " |      dictionary for instance variables (if defined)\n",
                         " |  \n",
                         " |  __weakref__\n",
                         " |      list of weak references to the object (if defined)\n",
                         " |  \n",
-                        " |  height\n",
-                        " |      Property that gives the current height of the tree. This is the length\n",
-                        " |      of the longest item path within the tree.\n",
-                        " |  \n",
                         " |  name\n",
                         " |  \n",
-                        " |  size\n",
-                        " |      Property that gives the number of elements currently in the tree.\n",
-                        " |  \n",
                         " |  workbook\n",
                         " |      Property that gives the current workbook of the tree. Returns None if tree is globally scoped\n",
                         " |  \n",
                         " |  ----------------------------------------------------------------------\n",
                         " |  Data and other attributes defined here:\n",
                         " |  \n",
                         " |  __annotations__ = {'session': 'Session', 'status': 'Status'}\n",
@@ -2299,15 +2322,15 @@
             "execution_count": 24,
             "id": "guided-animation",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<div style=\"background-color: #EEFFEE;color:black; text-align: left;\">Query successful</div><table class=\"tex2jax_ignore\" style=\"color:black;\"><tr><td style=\"background-color: #EEFFEE;\"></td><td style=\"background-color: #EEFFEE; text-align: left;\">Name</td><td style=\"background-color: #EEFFEE; text-align: left;\">Datasource Name</td><td style=\"background-color: #EEFFEE; text-align: left;\">Time</td><td style=\"background-color: #EEFFEE; text-align: right;\">Count</td><td style=\"background-color: #EEFFEE; text-align: right;\">Pages</td><td style=\"background-color: #EEFFEE; text-align: left;\">Result</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">0</td><td style=\"text-align: left; vertical-align: top;\">Area ?_*</td><td style=\"text-align: left; vertical-align: top;\">Example Data</td><td style=\"vertical-align: top;\">00:00:00.06</td><td style=\"text-align: right; vertical-align: top;\">68</td><td style=\"text-align: right; vertical-align: top;\">1</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr></table>"
+                            "<div style=\"background-color: #EEFFEE;color:black; text-align: left;\">Query successful</div><table class=\"tex2jax_ignore\" style=\"color:black;\"><tr><td style=\"background-color: #EEFFEE;\"></td><td style=\"background-color: #EEFFEE; text-align: left;\">Name</td><td style=\"background-color: #EEFFEE; text-align: left;\">Datasource Name</td><td style=\"background-color: #EEFFEE; text-align: left;\">Time</td><td style=\"background-color: #EEFFEE; text-align: right;\">Count</td><td style=\"background-color: #EEFFEE; text-align: right;\">Pages</td><td style=\"background-color: #EEFFEE; text-align: left;\">Result</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">0</td><td style=\"text-align: left; vertical-align: top;\">Area ?_*</td><td style=\"text-align: left; vertical-align: top;\">Example Data</td><td style=\"vertical-align: top;\">00:00:00.08</td><td style=\"text-align: right; vertical-align: top;\">68</td><td style=\"text-align: right; vertical-align: top;\">1</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr></table>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -2341,73 +2364,73 @@
                             "      <th>Datasource Name</th>\n",
                             "      <th>Archived</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
-                            "      <td>73FC8F67-9468-44BE-85E9-3E45E44060A3</td>\n",
+                            "      <td>0EDF27BA-E0C6-7320-A878-A09581426D88</td>\n",
                             "      <td>Area A_Compressor Power</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
                             "      <td>kW</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1</th>\n",
-                            "      <td>D17ABF6D-DF08-45EB-9E4D-5D80AD736198</td>\n",
+                            "      <td>0EDF27BA-E02C-6630-B5F0-343D4E602E7D</td>\n",
                             "      <td>Area A_Compressor Stage</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
                             "      <td>string</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2</th>\n",
-                            "      <td>B695ACF4-83EF-4D8C-8D83-4F31751B1A2F</td>\n",
+                            "      <td>0EDF27BA-DEB4-6690-8D35-FCC52A615AB4</td>\n",
                             "      <td>Area A_Optimizer</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>3</th>\n",
-                            "      <td>1FF81332-426C-4D21-A98C-AAEBA2F7B8DC</td>\n",
+                            "      <td>0EDF27BA-DEC0-F9E0-8E96-D0178F21E874</td>\n",
                             "      <td>Area A_Relative Humidity</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
                             "      <td>%</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>4</th>\n",
-                            "      <td>C1391A12-665B-40B0-8334-BF5F1DBADDDD</td>\n",
+                            "      <td>0EDF27BA-DEA8-7340-BB28-BCB11CC252BB</td>\n",
                             "      <td>Area A_Temperature</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
                             "      <td>\u00b0F</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
                             "                                     ID                      Name  \\\n",
-                            "0  73FC8F67-9468-44BE-85E9-3E45E44060A3   Area A_Compressor Power   \n",
-                            "1  D17ABF6D-DF08-45EB-9E4D-5D80AD736198   Area A_Compressor Stage   \n",
-                            "2  B695ACF4-83EF-4D8C-8D83-4F31751B1A2F          Area A_Optimizer   \n",
-                            "3  1FF81332-426C-4D21-A98C-AAEBA2F7B8DC  Area A_Relative Humidity   \n",
-                            "4  C1391A12-665B-40B0-8334-BF5F1DBADDDD        Area A_Temperature   \n",
+                            "0  0EDF27BA-E0C6-7320-A878-A09581426D88   Area A_Compressor Power   \n",
+                            "1  0EDF27BA-E02C-6630-B5F0-343D4E602E7D   Area A_Compressor Stage   \n",
+                            "2  0EDF27BA-DEB4-6690-8D35-FCC52A615AB4          Area A_Optimizer   \n",
+                            "3  0EDF27BA-DEC0-F9E0-8E96-D0178F21E874  Area A_Relative Humidity   \n",
+                            "4  0EDF27BA-DEA8-7340-BB28-BCB11CC252BB        Area A_Temperature   \n",
                             "\n",
                             "   Description          Type Value Unit Of Measure Datasource Name  Archived  \n",
                             "0          NaN  StoredSignal                    kW    Example Data     False  \n",
                             "1          NaN  StoredSignal                string    Example Data     False  \n",
                             "2          NaN  StoredSignal                   NaN    Example Data     False  \n",
                             "3          NaN  StoredSignal                     %    Example Data     False  \n",
                             "4          NaN  StoredSignal                    \u00b0F    Example Data     False  "
@@ -2522,15 +2545,15 @@
             "execution_count": 26,
             "id": "ca4728b1",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<div style=\"background-color: #EEFFEE;color:black; text-align: left;\">Pushed successfully to datasource <strong>Seeq Data Lab [Datasource ID: Seeq Data Lab]</strong> and scoped to workbook ID <strong>95BED80D-BD27-4057-B0C9-E0920E699FEE</strong><br>Click the following link to see what you pushed in Seeq:<br><a href=\"http://localhost:34216/845E2BBC-786E-47F0-8B1D-95D2DC8A9EA8/workbook/95BED80D-BD27-4057-B0C9-E0920E699FEE/worksheet/CF02358A-51F6-40FF-8E86-F2A2717D0B60\" target=\"_new\">http://localhost:34216/845E2BBC-786E-47F0-8B1D-95D2DC8A9EA8/workbook/95BED80D-BD27-4057-B0C9-E0920E699FEE/worksheet/CF02358A-51F6-40FF-8E86-F2A2717D0B60</a></div>"
+                            "<div style=\"background-color: #EEFFEE;color:black; text-align: left;\">Pushed successfully to datasource <strong>Seeq Data Lab [Datasource ID: Seeq Data Lab]</strong> and scoped to workbook ID <strong>0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8</strong><br>Click the following link to see what you pushed in Seeq:<br><a href=\"http://localhost:34216/0EDF27BC-6135-FB90-8645-7859B3D869A9/workbook/0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8/worksheet/0EDF27BC-85E0-EEE0-955F-1C59612A3AAC\" target=\"_blank\">http://localhost:34216/0EDF27BC-6135-FB90-8645-7859B3D869A9/workbook/0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8/worksheet/0EDF27BC-85E0-EEE0-955F-1C59612A3AAC</a></div>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -2578,566 +2601,566 @@
                             "      <th>Push Result</th>\n",
                             "      <th>Cache Enabled</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
-                            "      <td>27112E05-700D-4D37-BDE1-E58A3E5B3192</td>\n",
+                            "      <td>0EDF27BC-9A95-7390-A7E6-11E67A7C0E5E</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td></td>\n",
                             "      <td>My CSV Tree</td>\n",
                             "      <td>Asset</td>\n",
                             "      <td>1</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>...</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>95BED80D-BD27-4057-B0C9-E0920E699FEE</td>\n",
+                            "      <td>0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[95BED80D-BD27-4057-B0C9-E0920E699FEE] {Asset}...</td>\n",
+                            "      <td>[0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Asset}...</td>\n",
                             "      <td>Success</td>\n",
                             "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1</th>\n",
-                            "      <td>57AF07FD-A462-4059-823C-70CB15B2A38D</td>\n",
+                            "      <td>0EDF27BC-9A97-EAA0-83CA-0063D1483D5A</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>My CSV Tree</td>\n",
                             "      <td>Cooling Tower 1</td>\n",
                             "      <td>Asset</td>\n",
                             "      <td>2</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>...</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>95BED80D-BD27-4057-B0C9-E0920E699FEE</td>\n",
+                            "      <td>0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[95BED80D-BD27-4057-B0C9-E0920E699FEE] {Asset}...</td>\n",
+                            "      <td>[0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Asset}...</td>\n",
                             "      <td>Success</td>\n",
                             "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2</th>\n",
-                            "      <td>9CBA46E2-D056-4BF2-A838-20717F05E42E</td>\n",
+                            "      <td>0EDF27BC-9A9A-71B0-9788-8AD734BC304E</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>My CSV Tree &gt;&gt; Cooling Tower 1</td>\n",
                             "      <td>Area A</td>\n",
                             "      <td>Asset</td>\n",
                             "      <td>3</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>...</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>95BED80D-BD27-4057-B0C9-E0920E699FEE</td>\n",
+                            "      <td>0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[95BED80D-BD27-4057-B0C9-E0920E699FEE] {Asset}...</td>\n",
+                            "      <td>[0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Asset}...</td>\n",
                             "      <td>Success</td>\n",
                             "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>3</th>\n",
-                            "      <td>9E2C4E48-8C5E-4C56-987B-0C32EF55A7A1</td>\n",
+                            "      <td>0EDF27BC-9C45-75A0-9BC0-F99719E614CA</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>My CSV Tree &gt;&gt; Cooling Tower 1 &gt;&gt; Area A</td>\n",
                             "      <td>Dew Point</td>\n",
                             "      <td>CalculatedSignal</td>\n",
                             "      <td>4</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>$t - ((100 - $rh.setUnits(\"\"))/5)</td>\n",
-                            "      <td>[rh=2076B897-598A-4A5B-9226-4ACB70423073, t=63...</td>\n",
+                            "      <td>[rh=0EDF27BC-99AA-FD90-9572-383FE2C37BA9, t=0E...</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>...</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>95BED80D-BD27-4057-B0C9-E0920E699FEE</td>\n",
+                            "      <td>0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[95BED80D-BD27-4057-B0C9-E0920E699FEE] {Signal...</td>\n",
+                            "      <td>[0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Signal...</td>\n",
                             "      <td>Success</td>\n",
                             "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>4</th>\n",
-                            "      <td>2076B897-598A-4A5B-9226-4ACB70423073</td>\n",
-                            "      <td>1FF81332-426C-4D21-A98C-AAEBA2F7B8DC</td>\n",
+                            "      <td>0EDF27BC-99AA-FD90-9572-383FE2C37BA9</td>\n",
+                            "      <td>0EDF27BA-DEC0-F9E0-8E96-D0178F21E874</td>\n",
                             "      <td>My CSV Tree &gt;&gt; Cooling Tower 1 &gt;&gt; Area A</td>\n",
                             "      <td>Relative Humidity</td>\n",
                             "      <td>CalculatedSignal</td>\n",
                             "      <td>4</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>$signal</td>\n",
-                            "      <td>[signal=1FF81332-426C-4D21-A98C-AAEBA2F7B8DC]</td>\n",
+                            "      <td>[signal=0EDF27BA-DEC0-F9E0-8E96-D0178F21E874]</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>...</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>95BED80D-BD27-4057-B0C9-E0920E699FEE</td>\n",
+                            "      <td>0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[95BED80D-BD27-4057-B0C9-E0920E699FEE] {Signal...</td>\n",
+                            "      <td>[0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Signal...</td>\n",
                             "      <td>Success</td>\n",
                             "      <td>False</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>5</th>\n",
-                            "      <td>63E8C7ED-A9F3-48AF-AB3F-099F114CFF37</td>\n",
-                            "      <td>C1391A12-665B-40B0-8334-BF5F1DBADDDD</td>\n",
+                            "      <td>0EDF27BC-99D1-EE90-9B64-84989AE7FADE</td>\n",
+                            "      <td>0EDF27BA-DEA8-7340-BB28-BCB11CC252BB</td>\n",
                             "      <td>My CSV Tree &gt;&gt; Cooling Tower 1 &gt;&gt; Area A</td>\n",
                             "      <td>Temperature</td>\n",
                             "      <td>CalculatedSignal</td>\n",
                             "      <td>4</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>$signal</td>\n",
-                            "      <td>[signal=C1391A12-665B-40B0-8334-BF5F1DBADDDD]</td>\n",
+                            "      <td>[signal=0EDF27BA-DEA8-7340-BB28-BCB11CC252BB]</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>...</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>95BED80D-BD27-4057-B0C9-E0920E699FEE</td>\n",
+                            "      <td>0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[95BED80D-BD27-4057-B0C9-E0920E699FEE] {Signal...</td>\n",
+                            "      <td>[0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Signal...</td>\n",
                             "      <td>Success</td>\n",
                             "      <td>False</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>6</th>\n",
-                            "      <td>45F3ED49-CF9C-485E-9DA7-70D7CCDB9A30</td>\n",
+                            "      <td>0EDF27BC-9A9A-71B0-8CC5-C3E4117635D5</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>My CSV Tree &gt;&gt; Cooling Tower 1</td>\n",
                             "      <td>Area B</td>\n",
                             "      <td>Asset</td>\n",
                             "      <td>3</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>...</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>95BED80D-BD27-4057-B0C9-E0920E699FEE</td>\n",
+                            "      <td>0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[95BED80D-BD27-4057-B0C9-E0920E699FEE] {Asset}...</td>\n",
+                            "      <td>[0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Asset}...</td>\n",
                             "      <td>Success</td>\n",
                             "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>7</th>\n",
-                            "      <td>863C9789-5F76-4C14-9664-78261C47D737</td>\n",
+                            "      <td>0EDF27BC-9C8E-F980-A215-63EA2C3EBF52</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>My CSV Tree &gt;&gt; Cooling Tower 1 &gt;&gt; Area B</td>\n",
                             "      <td>Dew Point</td>\n",
                             "      <td>CalculatedSignal</td>\n",
                             "      <td>4</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>$t - ((100 - $rh.setUnits(\"\"))/5)</td>\n",
-                            "      <td>[rh=BDC479E9-72A9-46CA-8DAC-254376253A7E, t=D7...</td>\n",
+                            "      <td>[rh=0EDF27BC-99F4-7170-B3A5-28C54491C37E, t=0E...</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>...</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>95BED80D-BD27-4057-B0C9-E0920E699FEE</td>\n",
+                            "      <td>0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[95BED80D-BD27-4057-B0C9-E0920E699FEE] {Signal...</td>\n",
+                            "      <td>[0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Signal...</td>\n",
                             "      <td>Success</td>\n",
                             "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>8</th>\n",
-                            "      <td>BDC479E9-72A9-46CA-8DAC-254376253A7E</td>\n",
-                            "      <td>F9DAFE9A-C4FB-4C51-8A39-BEB01672EA07</td>\n",
+                            "      <td>0EDF27BC-99F4-7170-B3A5-28C54491C37E</td>\n",
+                            "      <td>0EDF27BA-DEBB-FBC0-96F3-F56E271F0439</td>\n",
                             "      <td>My CSV Tree &gt;&gt; Cooling Tower 1 &gt;&gt; Area B</td>\n",
                             "      <td>Relative Humidity</td>\n",
                             "      <td>CalculatedSignal</td>\n",
                             "      <td>4</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>$signal</td>\n",
-                            "      <td>[signal=F9DAFE9A-C4FB-4C51-8A39-BEB01672EA07]</td>\n",
+                            "      <td>[signal=0EDF27BA-DEBB-FBC0-96F3-F56E271F0439]</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>...</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>95BED80D-BD27-4057-B0C9-E0920E699FEE</td>\n",
+                            "      <td>0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[95BED80D-BD27-4057-B0C9-E0920E699FEE] {Signal...</td>\n",
+                            "      <td>[0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Signal...</td>\n",
                             "      <td>Success</td>\n",
                             "      <td>False</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>9</th>\n",
-                            "      <td>D790C465-F0DB-4C29-8240-FBAE4DB86B32</td>\n",
-                            "      <td>7088C03A-CB16-40B0-B83A-7C478F0797E0</td>\n",
+                            "      <td>0EDF27BC-9A0E-FF20-98B5-AE82FB81DB20</td>\n",
+                            "      <td>0EDF27BA-DEB4-6690-9D71-02A0E4ED00F8</td>\n",
                             "      <td>My CSV Tree &gt;&gt; Cooling Tower 1 &gt;&gt; Area B</td>\n",
                             "      <td>Temperature</td>\n",
                             "      <td>CalculatedSignal</td>\n",
                             "      <td>4</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>$signal</td>\n",
-                            "      <td>[signal=7088C03A-CB16-40B0-B83A-7C478F0797E0]</td>\n",
+                            "      <td>[signal=0EDF27BA-DEB4-6690-9D71-02A0E4ED00F8]</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>...</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>95BED80D-BD27-4057-B0C9-E0920E699FEE</td>\n",
+                            "      <td>0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[95BED80D-BD27-4057-B0C9-E0920E699FEE] {Signal...</td>\n",
+                            "      <td>[0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Signal...</td>\n",
                             "      <td>Success</td>\n",
                             "      <td>False</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>10</th>\n",
-                            "      <td>A8C24899-30B6-44EB-A171-545204113A75</td>\n",
+                            "      <td>0EDF27BC-BBB4-73A0-B921-2B9FD6788F59</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>My CSV Tree &gt;&gt; Cooling Tower 1</td>\n",
                             "      <td>Average Temperature of All Areas</td>\n",
                             "      <td>CalculatedSignal</td>\n",
                             "      <td>3</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>average($p0, $p1)</td>\n",
-                            "      <td>[p0=63E8C7ED-A9F3-48AF-AB3F-099F114CFF37, p1=D...</td>\n",
+                            "      <td>[p0=0EDF27BC-99D1-EE90-9B64-84989AE7FADE, p1=0...</td>\n",
                             "      <td>Average</td>\n",
                             "      <td>...</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>95BED80D-BD27-4057-B0C9-E0920E699FEE</td>\n",
+                            "      <td>0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[95BED80D-BD27-4057-B0C9-E0920E699FEE] {Signal...</td>\n",
+                            "      <td>[0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Signal...</td>\n",
                             "      <td>Success</td>\n",
                             "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>11</th>\n",
-                            "      <td>4311E85D-C597-44A2-8FA1-24DFB698B0DD</td>\n",
+                            "      <td>0EDF27BC-9A9A-71B0-9CDA-34617BD25C9D</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>My CSV Tree</td>\n",
                             "      <td>Cooling Tower 2</td>\n",
                             "      <td>Asset</td>\n",
                             "      <td>2</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>...</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>95BED80D-BD27-4057-B0C9-E0920E699FEE</td>\n",
+                            "      <td>0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[95BED80D-BD27-4057-B0C9-E0920E699FEE] {Asset}...</td>\n",
+                            "      <td>[0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Asset}...</td>\n",
                             "      <td>Success</td>\n",
                             "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>12</th>\n",
-                            "      <td>79E60A20-01A4-4A08-9AD2-6EC2A20960E8</td>\n",
+                            "      <td>0EDF27BC-9A9A-71B0-B51C-8188F141D157</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>My CSV Tree &gt;&gt; Cooling Tower 2</td>\n",
                             "      <td>Area D</td>\n",
                             "      <td>Asset</td>\n",
                             "      <td>3</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>...</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>95BED80D-BD27-4057-B0C9-E0920E699FEE</td>\n",
+                            "      <td>0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[95BED80D-BD27-4057-B0C9-E0920E699FEE] {Asset}...</td>\n",
+                            "      <td>[0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Asset}...</td>\n",
                             "      <td>Success</td>\n",
                             "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>13</th>\n",
-                            "      <td>F20738AF-67D0-46F2-A92E-AAA8B40FCA6C</td>\n",
+                            "      <td>0EDF27BC-9CCB-EA10-AD88-1B5FA8264457</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>My CSV Tree &gt;&gt; Cooling Tower 2 &gt;&gt; Area D</td>\n",
                             "      <td>Dew Point</td>\n",
                             "      <td>CalculatedSignal</td>\n",
                             "      <td>4</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>$t - ((100 - $rh.setUnits(\"\"))/5)</td>\n",
-                            "      <td>[rh=A45FF098-A765-4281-A0E2-69ABFE00364F, t=73...</td>\n",
+                            "      <td>[rh=0EDF27BC-9A2E-EAF0-A371-C607B64C3404, t=0E...</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>...</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>95BED80D-BD27-4057-B0C9-E0920E699FEE</td>\n",
+                            "      <td>0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[95BED80D-BD27-4057-B0C9-E0920E699FEE] {Signal...</td>\n",
+                            "      <td>[0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Signal...</td>\n",
                             "      <td>Success</td>\n",
                             "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>14</th>\n",
-                            "      <td>A45FF098-A765-4281-A0E2-69ABFE00364F</td>\n",
-                            "      <td>1E521D48-3D1F-4274-8A0E-23E51220967A</td>\n",
+                            "      <td>0EDF27BC-9A2E-EAF0-A371-C607B64C3404</td>\n",
+                            "      <td>0EDF27BA-DEB1-FF80-9C7D-F951BA3A75CB</td>\n",
                             "      <td>My CSV Tree &gt;&gt; Cooling Tower 2 &gt;&gt; Area D</td>\n",
                             "      <td>Relative Humidity</td>\n",
                             "      <td>CalculatedSignal</td>\n",
                             "      <td>4</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>$signal</td>\n",
-                            "      <td>[signal=1E521D48-3D1F-4274-8A0E-23E51220967A]</td>\n",
+                            "      <td>[signal=0EDF27BA-DEB1-FF80-9C7D-F951BA3A75CB]</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>...</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>95BED80D-BD27-4057-B0C9-E0920E699FEE</td>\n",
+                            "      <td>0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[95BED80D-BD27-4057-B0C9-E0920E699FEE] {Signal...</td>\n",
+                            "      <td>[0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Signal...</td>\n",
                             "      <td>Success</td>\n",
                             "      <td>False</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>15</th>\n",
-                            "      <td>734B3D00-9850-4D51-B7A1-1A522C90F0B1</td>\n",
-                            "      <td>B0C6DB27-3814-4B4A-8338-F5133C763A33</td>\n",
+                            "      <td>0EDF27BC-9A47-7190-9A77-EE93227F46C6</td>\n",
+                            "      <td>0EDF27BA-E0AD-EC80-9DEF-842FAE6B4C27</td>\n",
                             "      <td>My CSV Tree &gt;&gt; Cooling Tower 2 &gt;&gt; Area D</td>\n",
                             "      <td>Temperature</td>\n",
                             "      <td>CalculatedSignal</td>\n",
                             "      <td>4</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>$signal</td>\n",
-                            "      <td>[signal=B0C6DB27-3814-4B4A-8338-F5133C763A33]</td>\n",
+                            "      <td>[signal=0EDF27BA-E0AD-EC80-9DEF-842FAE6B4C27]</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>...</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>95BED80D-BD27-4057-B0C9-E0920E699FEE</td>\n",
+                            "      <td>0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[95BED80D-BD27-4057-B0C9-E0920E699FEE] {Signal...</td>\n",
+                            "      <td>[0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Signal...</td>\n",
                             "      <td>Success</td>\n",
                             "      <td>False</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>16</th>\n",
-                            "      <td>CF61BA32-F42E-4E3B-A0A0-356DAD1E4CE9</td>\n",
+                            "      <td>0EDF27BC-9A9A-71B0-A7C6-3A10B9EE89D9</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>My CSV Tree &gt;&gt; Cooling Tower 2</td>\n",
                             "      <td>Area E</td>\n",
                             "      <td>Asset</td>\n",
                             "      <td>3</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>...</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>95BED80D-BD27-4057-B0C9-E0920E699FEE</td>\n",
+                            "      <td>0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[95BED80D-BD27-4057-B0C9-E0920E699FEE] {Asset}...</td>\n",
+                            "      <td>[0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Asset}...</td>\n",
                             "      <td>Success</td>\n",
                             "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>17</th>\n",
-                            "      <td>AE71C1B9-F198-4C61-A128-174AA4BD9987</td>\n",
+                            "      <td>0EDF27BC-9D0B-71B0-856B-00D6368974BB</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>My CSV Tree &gt;&gt; Cooling Tower 2 &gt;&gt; Area E</td>\n",
                             "      <td>Dew Point</td>\n",
                             "      <td>CalculatedSignal</td>\n",
                             "      <td>4</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>$t - ((100 - $rh.setUnits(\"\"))/5)</td>\n",
-                            "      <td>[rh=0012B79D-E4FC-4589-A711-2D4706F38039, t=C9...</td>\n",
+                            "      <td>[rh=0EDF27BC-9A61-FF40-A7F7-5125E6DF8637, t=0E...</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>...</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>95BED80D-BD27-4057-B0C9-E0920E699FEE</td>\n",
+                            "      <td>0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[95BED80D-BD27-4057-B0C9-E0920E699FEE] {Signal...</td>\n",
+                            "      <td>[0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Signal...</td>\n",
                             "      <td>Success</td>\n",
                             "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>18</th>\n",
-                            "      <td>0012B79D-E4FC-4589-A711-2D4706F38039</td>\n",
-                            "      <td>6B68E870-1C98-4D1C-AACF-550D70540771</td>\n",
+                            "      <td>0EDF27BC-9A61-FF40-A7F7-5125E6DF8637</td>\n",
+                            "      <td>0EDF27BA-E089-6290-ABF3-D84F99D009F9</td>\n",
                             "      <td>My CSV Tree &gt;&gt; Cooling Tower 2 &gt;&gt; Area E</td>\n",
                             "      <td>Relative Humidity</td>\n",
                             "      <td>CalculatedSignal</td>\n",
                             "      <td>4</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>$signal</td>\n",
-                            "      <td>[signal=6B68E870-1C98-4D1C-AACF-550D70540771]</td>\n",
+                            "      <td>[signal=0EDF27BA-E089-6290-ABF3-D84F99D009F9]</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>...</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>95BED80D-BD27-4057-B0C9-E0920E699FEE</td>\n",
+                            "      <td>0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[95BED80D-BD27-4057-B0C9-E0920E699FEE] {Signal...</td>\n",
+                            "      <td>[0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Signal...</td>\n",
                             "      <td>Success</td>\n",
                             "      <td>False</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>19</th>\n",
-                            "      <td>C971DD89-A3F0-41E9-B491-8E3F400A10DC</td>\n",
-                            "      <td>8D80EE1E-585D-4F37-95D4-C0F31865CBBB</td>\n",
+                            "      <td>0EDF27BC-9A7A-75E0-8160-F88E06BD59E5</td>\n",
+                            "      <td>0EDF27BA-E0CD-E850-BA67-375F032E2CB9</td>\n",
                             "      <td>My CSV Tree &gt;&gt; Cooling Tower 2 &gt;&gt; Area E</td>\n",
                             "      <td>Temperature</td>\n",
                             "      <td>CalculatedSignal</td>\n",
                             "      <td>4</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>$signal</td>\n",
-                            "      <td>[signal=8D80EE1E-585D-4F37-95D4-C0F31865CBBB]</td>\n",
+                            "      <td>[signal=0EDF27BA-E0CD-E850-BA67-375F032E2CB9]</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>...</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>95BED80D-BD27-4057-B0C9-E0920E699FEE</td>\n",
+                            "      <td>0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[95BED80D-BD27-4057-B0C9-E0920E699FEE] {Signal...</td>\n",
+                            "      <td>[0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Signal...</td>\n",
                             "      <td>Success</td>\n",
                             "      <td>False</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>20</th>\n",
-                            "      <td>0BC6F5F1-BC87-48B8-9548-AF02CB0B1575</td>\n",
+                            "      <td>0EDF27BC-BBE0-62C0-80A5-7D1C8A88236F</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>My CSV Tree &gt;&gt; Cooling Tower 2</td>\n",
                             "      <td>Average Temperature of All Areas</td>\n",
                             "      <td>CalculatedSignal</td>\n",
                             "      <td>3</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>average($p0, $p1)</td>\n",
-                            "      <td>[p0=734B3D00-9850-4D51-B7A1-1A522C90F0B1, p1=C...</td>\n",
+                            "      <td>[p0=0EDF27BC-9A47-7190-9A77-EE93227F46C6, p1=0...</td>\n",
                             "      <td>Average</td>\n",
                             "      <td>...</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>95BED80D-BD27-4057-B0C9-E0920E699FEE</td>\n",
+                            "      <td>0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[95BED80D-BD27-4057-B0C9-E0920E699FEE] {Signal...</td>\n",
+                            "      <td>[0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Signal...</td>\n",
                             "      <td>Success</td>\n",
                             "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "<p>21 rows \u00d7 29 columns</p>\n",
                             "</div>"
                         ],
                         "text/plain": [
                             "                                      ID  \\\n",
-                            "0   27112E05-700D-4D37-BDE1-E58A3E5B3192   \n",
-                            "1   57AF07FD-A462-4059-823C-70CB15B2A38D   \n",
-                            "2   9CBA46E2-D056-4BF2-A838-20717F05E42E   \n",
-                            "3   9E2C4E48-8C5E-4C56-987B-0C32EF55A7A1   \n",
-                            "4   2076B897-598A-4A5B-9226-4ACB70423073   \n",
-                            "5   63E8C7ED-A9F3-48AF-AB3F-099F114CFF37   \n",
-                            "6   45F3ED49-CF9C-485E-9DA7-70D7CCDB9A30   \n",
-                            "7   863C9789-5F76-4C14-9664-78261C47D737   \n",
-                            "8   BDC479E9-72A9-46CA-8DAC-254376253A7E   \n",
-                            "9   D790C465-F0DB-4C29-8240-FBAE4DB86B32   \n",
-                            "10  A8C24899-30B6-44EB-A171-545204113A75   \n",
-                            "11  4311E85D-C597-44A2-8FA1-24DFB698B0DD   \n",
-                            "12  79E60A20-01A4-4A08-9AD2-6EC2A20960E8   \n",
-                            "13  F20738AF-67D0-46F2-A92E-AAA8B40FCA6C   \n",
-                            "14  A45FF098-A765-4281-A0E2-69ABFE00364F   \n",
-                            "15  734B3D00-9850-4D51-B7A1-1A522C90F0B1   \n",
-                            "16  CF61BA32-F42E-4E3B-A0A0-356DAD1E4CE9   \n",
-                            "17  AE71C1B9-F198-4C61-A128-174AA4BD9987   \n",
-                            "18  0012B79D-E4FC-4589-A711-2D4706F38039   \n",
-                            "19  C971DD89-A3F0-41E9-B491-8E3F400A10DC   \n",
-                            "20  0BC6F5F1-BC87-48B8-9548-AF02CB0B1575   \n",
+                            "0   0EDF27BC-9A95-7390-A7E6-11E67A7C0E5E   \n",
+                            "1   0EDF27BC-9A97-EAA0-83CA-0063D1483D5A   \n",
+                            "2   0EDF27BC-9A9A-71B0-9788-8AD734BC304E   \n",
+                            "3   0EDF27BC-9C45-75A0-9BC0-F99719E614CA   \n",
+                            "4   0EDF27BC-99AA-FD90-9572-383FE2C37BA9   \n",
+                            "5   0EDF27BC-99D1-EE90-9B64-84989AE7FADE   \n",
+                            "6   0EDF27BC-9A9A-71B0-8CC5-C3E4117635D5   \n",
+                            "7   0EDF27BC-9C8E-F980-A215-63EA2C3EBF52   \n",
+                            "8   0EDF27BC-99F4-7170-B3A5-28C54491C37E   \n",
+                            "9   0EDF27BC-9A0E-FF20-98B5-AE82FB81DB20   \n",
+                            "10  0EDF27BC-BBB4-73A0-B921-2B9FD6788F59   \n",
+                            "11  0EDF27BC-9A9A-71B0-9CDA-34617BD25C9D   \n",
+                            "12  0EDF27BC-9A9A-71B0-B51C-8188F141D157   \n",
+                            "13  0EDF27BC-9CCB-EA10-AD88-1B5FA8264457   \n",
+                            "14  0EDF27BC-9A2E-EAF0-A371-C607B64C3404   \n",
+                            "15  0EDF27BC-9A47-7190-9A77-EE93227F46C6   \n",
+                            "16  0EDF27BC-9A9A-71B0-A7C6-3A10B9EE89D9   \n",
+                            "17  0EDF27BC-9D0B-71B0-856B-00D6368974BB   \n",
+                            "18  0EDF27BC-9A61-FF40-A7F7-5125E6DF8637   \n",
+                            "19  0EDF27BC-9A7A-75E0-8160-F88E06BD59E5   \n",
+                            "20  0EDF27BC-BBE0-62C0-80A5-7D1C8A88236F   \n",
                             "\n",
                             "                           Referenced ID  \\\n",
                             "0                                    NaN   \n",
                             "1                                    NaN   \n",
                             "2                                    NaN   \n",
                             "3                                    NaN   \n",
-                            "4   1FF81332-426C-4D21-A98C-AAEBA2F7B8DC   \n",
-                            "5   C1391A12-665B-40B0-8334-BF5F1DBADDDD   \n",
+                            "4   0EDF27BA-DEC0-F9E0-8E96-D0178F21E874   \n",
+                            "5   0EDF27BA-DEA8-7340-BB28-BCB11CC252BB   \n",
                             "6                                    NaN   \n",
                             "7                                    NaN   \n",
-                            "8   F9DAFE9A-C4FB-4C51-8A39-BEB01672EA07   \n",
-                            "9   7088C03A-CB16-40B0-B83A-7C478F0797E0   \n",
+                            "8   0EDF27BA-DEBB-FBC0-96F3-F56E271F0439   \n",
+                            "9   0EDF27BA-DEB4-6690-9D71-02A0E4ED00F8   \n",
                             "10                                   NaN   \n",
                             "11                                   NaN   \n",
                             "12                                   NaN   \n",
                             "13                                   NaN   \n",
-                            "14  1E521D48-3D1F-4274-8A0E-23E51220967A   \n",
-                            "15  B0C6DB27-3814-4B4A-8338-F5133C763A33   \n",
+                            "14  0EDF27BA-DEB1-FF80-9C7D-F951BA3A75CB   \n",
+                            "15  0EDF27BA-E0AD-EC80-9DEF-842FAE6B4C27   \n",
                             "16                                   NaN   \n",
                             "17                                   NaN   \n",
-                            "18  6B68E870-1C98-4D1C-AACF-550D70540771   \n",
-                            "19  8D80EE1E-585D-4F37-95D4-C0F31865CBBB   \n",
+                            "18  0EDF27BA-E089-6290-ABF3-D84F99D009F9   \n",
+                            "19  0EDF27BA-E0CD-E850-BA67-375F032E2CB9   \n",
                             "20                                   NaN   \n",
                             "\n",
                             "                                        Path  \\\n",
                             "0                                              \n",
                             "1                                My CSV Tree   \n",
                             "2             My CSV Tree >> Cooling Tower 1   \n",
                             "3   My CSV Tree >> Cooling Tower 1 >> Area A   \n",
@@ -3205,32 +3228,32 @@
                             "19                            $signal   \n",
                             "20                  average($p0, $p1)   \n",
                             "\n",
                             "                                   Formula Parameters Roll Up Statistic  ...  \\\n",
                             "0                                                 NaN               NaN  ...   \n",
                             "1                                                 NaN               NaN  ...   \n",
                             "2                                                 NaN               NaN  ...   \n",
-                            "3   [rh=2076B897-598A-4A5B-9226-4ACB70423073, t=63...               NaN  ...   \n",
-                            "4       [signal=1FF81332-426C-4D21-A98C-AAEBA2F7B8DC]               NaN  ...   \n",
-                            "5       [signal=C1391A12-665B-40B0-8334-BF5F1DBADDDD]               NaN  ...   \n",
+                            "3   [rh=0EDF27BC-99AA-FD90-9572-383FE2C37BA9, t=0E...               NaN  ...   \n",
+                            "4       [signal=0EDF27BA-DEC0-F9E0-8E96-D0178F21E874]               NaN  ...   \n",
+                            "5       [signal=0EDF27BA-DEA8-7340-BB28-BCB11CC252BB]               NaN  ...   \n",
                             "6                                                 NaN               NaN  ...   \n",
-                            "7   [rh=BDC479E9-72A9-46CA-8DAC-254376253A7E, t=D7...               NaN  ...   \n",
-                            "8       [signal=F9DAFE9A-C4FB-4C51-8A39-BEB01672EA07]               NaN  ...   \n",
-                            "9       [signal=7088C03A-CB16-40B0-B83A-7C478F0797E0]               NaN  ...   \n",
-                            "10  [p0=63E8C7ED-A9F3-48AF-AB3F-099F114CFF37, p1=D...           Average  ...   \n",
+                            "7   [rh=0EDF27BC-99F4-7170-B3A5-28C54491C37E, t=0E...               NaN  ...   \n",
+                            "8       [signal=0EDF27BA-DEBB-FBC0-96F3-F56E271F0439]               NaN  ...   \n",
+                            "9       [signal=0EDF27BA-DEB4-6690-9D71-02A0E4ED00F8]               NaN  ...   \n",
+                            "10  [p0=0EDF27BC-99D1-EE90-9B64-84989AE7FADE, p1=0...           Average  ...   \n",
                             "11                                                NaN               NaN  ...   \n",
                             "12                                                NaN               NaN  ...   \n",
-                            "13  [rh=A45FF098-A765-4281-A0E2-69ABFE00364F, t=73...               NaN  ...   \n",
-                            "14      [signal=1E521D48-3D1F-4274-8A0E-23E51220967A]               NaN  ...   \n",
-                            "15      [signal=B0C6DB27-3814-4B4A-8338-F5133C763A33]               NaN  ...   \n",
+                            "13  [rh=0EDF27BC-9A2E-EAF0-A371-C607B64C3404, t=0E...               NaN  ...   \n",
+                            "14      [signal=0EDF27BA-DEB1-FF80-9C7D-F951BA3A75CB]               NaN  ...   \n",
+                            "15      [signal=0EDF27BA-E0AD-EC80-9DEF-842FAE6B4C27]               NaN  ...   \n",
                             "16                                                NaN               NaN  ...   \n",
-                            "17  [rh=0012B79D-E4FC-4589-A711-2D4706F38039, t=C9...               NaN  ...   \n",
-                            "18      [signal=6B68E870-1C98-4D1C-AACF-550D70540771]               NaN  ...   \n",
-                            "19      [signal=8D80EE1E-585D-4F37-95D4-C0F31865CBBB]               NaN  ...   \n",
-                            "20  [p0=734B3D00-9850-4D51-B7A1-1A522C90F0B1, p1=C...           Average  ...   \n",
+                            "17  [rh=0EDF27BC-9A61-FF40-A7F7-5125E6DF8637, t=0E...               NaN  ...   \n",
+                            "18      [signal=0EDF27BA-E089-6290-ABF3-D84F99D009F9]               NaN  ...   \n",
+                            "19      [signal=0EDF27BA-E0CD-E850-BA67-375F032E2CB9]               NaN  ...   \n",
+                            "20  [p0=0EDF27BC-9A47-7190-9A77-EE93227F46C6, p1=0...           Average  ...   \n",
                             "\n",
                             "   Period  Process Type  Thresholds  Template ID  \\\n",
                             "0     NaN           NaN         NaN          NaN   \n",
                             "1     NaN           NaN         NaN          NaN   \n",
                             "2     NaN           NaN         NaN          NaN   \n",
                             "3     NaN           NaN         NaN          NaN   \n",
                             "4     NaN           NaN         NaN          NaN   \n",
@@ -3248,58 +3271,58 @@
                             "16    NaN           NaN         NaN          NaN   \n",
                             "17    NaN           NaN         NaN          NaN   \n",
                             "18    NaN           NaN         NaN          NaN   \n",
                             "19    NaN           NaN         NaN          NaN   \n",
                             "20    NaN           NaN         NaN          NaN   \n",
                             "\n",
                             "                               Scoped To  Datasource Class  Datasource ID  \\\n",
-                            "0   95BED80D-BD27-4057-B0C9-E0920E699FEE     Seeq Data Lab  Seeq Data Lab   \n",
-                            "1   95BED80D-BD27-4057-B0C9-E0920E699FEE     Seeq Data Lab  Seeq Data Lab   \n",
-                            "2   95BED80D-BD27-4057-B0C9-E0920E699FEE     Seeq Data Lab  Seeq Data Lab   \n",
-                            "3   95BED80D-BD27-4057-B0C9-E0920E699FEE     Seeq Data Lab  Seeq Data Lab   \n",
-                            "4   95BED80D-BD27-4057-B0C9-E0920E699FEE     Seeq Data Lab  Seeq Data Lab   \n",
-                            "5   95BED80D-BD27-4057-B0C9-E0920E699FEE     Seeq Data Lab  Seeq Data Lab   \n",
-                            "6   95BED80D-BD27-4057-B0C9-E0920E699FEE     Seeq Data Lab  Seeq Data Lab   \n",
-                            "7   95BED80D-BD27-4057-B0C9-E0920E699FEE     Seeq Data Lab  Seeq Data Lab   \n",
-                            "8   95BED80D-BD27-4057-B0C9-E0920E699FEE     Seeq Data Lab  Seeq Data Lab   \n",
-                            "9   95BED80D-BD27-4057-B0C9-E0920E699FEE     Seeq Data Lab  Seeq Data Lab   \n",
-                            "10  95BED80D-BD27-4057-B0C9-E0920E699FEE     Seeq Data Lab  Seeq Data Lab   \n",
-                            "11  95BED80D-BD27-4057-B0C9-E0920E699FEE     Seeq Data Lab  Seeq Data Lab   \n",
-                            "12  95BED80D-BD27-4057-B0C9-E0920E699FEE     Seeq Data Lab  Seeq Data Lab   \n",
-                            "13  95BED80D-BD27-4057-B0C9-E0920E699FEE     Seeq Data Lab  Seeq Data Lab   \n",
-                            "14  95BED80D-BD27-4057-B0C9-E0920E699FEE     Seeq Data Lab  Seeq Data Lab   \n",
-                            "15  95BED80D-BD27-4057-B0C9-E0920E699FEE     Seeq Data Lab  Seeq Data Lab   \n",
-                            "16  95BED80D-BD27-4057-B0C9-E0920E699FEE     Seeq Data Lab  Seeq Data Lab   \n",
-                            "17  95BED80D-BD27-4057-B0C9-E0920E699FEE     Seeq Data Lab  Seeq Data Lab   \n",
-                            "18  95BED80D-BD27-4057-B0C9-E0920E699FEE     Seeq Data Lab  Seeq Data Lab   \n",
-                            "19  95BED80D-BD27-4057-B0C9-E0920E699FEE     Seeq Data Lab  Seeq Data Lab   \n",
-                            "20  95BED80D-BD27-4057-B0C9-E0920E699FEE     Seeq Data Lab  Seeq Data Lab   \n",
+                            "0   0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8     Seeq Data Lab  Seeq Data Lab   \n",
+                            "1   0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8     Seeq Data Lab  Seeq Data Lab   \n",
+                            "2   0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8     Seeq Data Lab  Seeq Data Lab   \n",
+                            "3   0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8     Seeq Data Lab  Seeq Data Lab   \n",
+                            "4   0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8     Seeq Data Lab  Seeq Data Lab   \n",
+                            "5   0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8     Seeq Data Lab  Seeq Data Lab   \n",
+                            "6   0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8     Seeq Data Lab  Seeq Data Lab   \n",
+                            "7   0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8     Seeq Data Lab  Seeq Data Lab   \n",
+                            "8   0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8     Seeq Data Lab  Seeq Data Lab   \n",
+                            "9   0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8     Seeq Data Lab  Seeq Data Lab   \n",
+                            "10  0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8     Seeq Data Lab  Seeq Data Lab   \n",
+                            "11  0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8     Seeq Data Lab  Seeq Data Lab   \n",
+                            "12  0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8     Seeq Data Lab  Seeq Data Lab   \n",
+                            "13  0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8     Seeq Data Lab  Seeq Data Lab   \n",
+                            "14  0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8     Seeq Data Lab  Seeq Data Lab   \n",
+                            "15  0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8     Seeq Data Lab  Seeq Data Lab   \n",
+                            "16  0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8     Seeq Data Lab  Seeq Data Lab   \n",
+                            "17  0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8     Seeq Data Lab  Seeq Data Lab   \n",
+                            "18  0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8     Seeq Data Lab  Seeq Data Lab   \n",
+                            "19  0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8     Seeq Data Lab  Seeq Data Lab   \n",
+                            "20  0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8     Seeq Data Lab  Seeq Data Lab   \n",
                             "\n",
                             "                                              Data ID  Push Result  \\\n",
-                            "0   [95BED80D-BD27-4057-B0C9-E0920E699FEE] {Asset}...      Success   \n",
-                            "1   [95BED80D-BD27-4057-B0C9-E0920E699FEE] {Asset}...      Success   \n",
-                            "2   [95BED80D-BD27-4057-B0C9-E0920E699FEE] {Asset}...      Success   \n",
-                            "3   [95BED80D-BD27-4057-B0C9-E0920E699FEE] {Signal...      Success   \n",
-                            "4   [95BED80D-BD27-4057-B0C9-E0920E699FEE] {Signal...      Success   \n",
-                            "5   [95BED80D-BD27-4057-B0C9-E0920E699FEE] {Signal...      Success   \n",
-                            "6   [95BED80D-BD27-4057-B0C9-E0920E699FEE] {Asset}...      Success   \n",
-                            "7   [95BED80D-BD27-4057-B0C9-E0920E699FEE] {Signal...      Success   \n",
-                            "8   [95BED80D-BD27-4057-B0C9-E0920E699FEE] {Signal...      Success   \n",
-                            "9   [95BED80D-BD27-4057-B0C9-E0920E699FEE] {Signal...      Success   \n",
-                            "10  [95BED80D-BD27-4057-B0C9-E0920E699FEE] {Signal...      Success   \n",
-                            "11  [95BED80D-BD27-4057-B0C9-E0920E699FEE] {Asset}...      Success   \n",
-                            "12  [95BED80D-BD27-4057-B0C9-E0920E699FEE] {Asset}...      Success   \n",
-                            "13  [95BED80D-BD27-4057-B0C9-E0920E699FEE] {Signal...      Success   \n",
-                            "14  [95BED80D-BD27-4057-B0C9-E0920E699FEE] {Signal...      Success   \n",
-                            "15  [95BED80D-BD27-4057-B0C9-E0920E699FEE] {Signal...      Success   \n",
-                            "16  [95BED80D-BD27-4057-B0C9-E0920E699FEE] {Asset}...      Success   \n",
-                            "17  [95BED80D-BD27-4057-B0C9-E0920E699FEE] {Signal...      Success   \n",
-                            "18  [95BED80D-BD27-4057-B0C9-E0920E699FEE] {Signal...      Success   \n",
-                            "19  [95BED80D-BD27-4057-B0C9-E0920E699FEE] {Signal...      Success   \n",
-                            "20  [95BED80D-BD27-4057-B0C9-E0920E699FEE] {Signal...      Success   \n",
+                            "0   [0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Asset}...      Success   \n",
+                            "1   [0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Asset}...      Success   \n",
+                            "2   [0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Asset}...      Success   \n",
+                            "3   [0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Signal...      Success   \n",
+                            "4   [0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Signal...      Success   \n",
+                            "5   [0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Signal...      Success   \n",
+                            "6   [0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Asset}...      Success   \n",
+                            "7   [0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Signal...      Success   \n",
+                            "8   [0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Signal...      Success   \n",
+                            "9   [0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Signal...      Success   \n",
+                            "10  [0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Signal...      Success   \n",
+                            "11  [0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Asset}...      Success   \n",
+                            "12  [0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Asset}...      Success   \n",
+                            "13  [0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Signal...      Success   \n",
+                            "14  [0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Signal...      Success   \n",
+                            "15  [0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Signal...      Success   \n",
+                            "16  [0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Asset}...      Success   \n",
+                            "17  [0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Signal...      Success   \n",
+                            "18  [0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Signal...      Success   \n",
+                            "19  [0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Signal...      Success   \n",
+                            "20  [0EDF27BC-8569-64D0-B3C6-8EAEBC88BDA8] {Signal...      Success   \n",
                             "\n",
                             "    Cache Enabled  \n",
                             "0             NaN  \n",
                             "1             NaN  \n",
                             "2             NaN  \n",
                             "3             NaN  \n",
                             "4           False  \n",
@@ -3372,13 +3395,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.7.8"
+            "version": "3.8.10"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `seeq-spy-187.5/seeq/spy/docs/Documentation/Asset Trees 2 - Templates.ipynb` & `seeq-spy-188.0/seeq/spy/docs/Documentation/Asset Trees 2 - Templates.ipynb`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996221622389858%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(1, 'import pandas as pd\\n'), (2, '\\n'), (3, '# Set the "*

 * *            'compatibility option so that you maximize the chance that SPy will remain compatible '*

 * *            "with your notebook/script\\n'), (4, 'spy.options.compatibility = 188')], delete: "*

 * *            "[1]}}, 1: {'outputs': {0: {'data': {'text/html': ['<div "*

 * *            'style="background-color: #EEFFEE;color:black; text-align: left;">Logged in to '*

 * *            '<strong>http://localhost:34216</strong> s […]*

```diff
@@ -3,26 +3,29 @@
         {
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from seeq import spy\n",
-                "import pandas as pd"
+                "import pandas as pd\n",
+                "\n",
+                "# Set the compatibility option so that you maximize the chance that SPy will remain compatible with your notebook/script\n",
+                "spy.options.compatibility = 188"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<div style=\"background-color: #EEFFEE;color:black;text-align: left;\">Logged in to <strong>http://localhost:34216</strong> successfully as <strong>agent_api_key</strong>.<br>Seeq Server Version: <strong>R57.0.0-SNAPSHOT</strong><br>Seeq Python Module Version: <strong>57.0.0.182.45</strong></div>"
+                            "<div style=\"background-color: #EEFFEE;color:black; text-align: left;\">Logged in to <strong>http://localhost:34216</strong> successfully as <strong>agent_api_key</strong>.<br>Seeq Server Version: <strong>R61.0.0-SNAPSHOT</strong><br>Seeq Python Module Version: <strong>61.0.0.184.25</strong></div>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -126,15 +129,15 @@
             "cell_type": "code",
             "execution_count": 4,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<div style=\"background-color: #EEFFEE;color:black;text-align: left;\">Query successful</div><table style=\"color:black;\"><tr><td style=\"background-color: #EEFFEE;\"></td><td style=\"background-color: #EEFFEE; text-align: left;\">Name</td><td style=\"background-color: #EEFFEE; text-align: left;\">Time</td><td style=\"background-color: #EEFFEE; text-align: right;\">Count</td><td style=\"background-color: #EEFFEE; text-align: right;\">Pages</td><td style=\"background-color: #EEFFEE; text-align: left;\">Result</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">0</td><td style=\"text-align: left; vertical-align: top;\">Area ?_*</td><td style=\"vertical-align: top;\">00:00:00.06</td><td style=\"text-align: right; vertical-align: top;\">70</td><td style=\"text-align: right; vertical-align: top;\">1</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr></table>"
+                            "<div style=\"background-color: #EEFFEE;color:black; text-align: left;\">Query successful</div><table class=\"tex2jax_ignore\" style=\"color:black;\"><tr><td style=\"background-color: #EEFFEE;\"></td><td style=\"background-color: #EEFFEE; text-align: left;\">Name</td><td style=\"background-color: #EEFFEE; text-align: left;\">Time</td><td style=\"background-color: #EEFFEE; text-align: right;\">Count</td><td style=\"background-color: #EEFFEE; text-align: right;\">Pages</td><td style=\"background-color: #EEFFEE; text-align: left;\">Result</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">0</td><td style=\"text-align: left; vertical-align: top;\">Area ?_*</td><td style=\"vertical-align: top;\">00:00:00.04</td><td style=\"text-align: right; vertical-align: top;\">70</td><td style=\"text-align: right; vertical-align: top;\">1</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr></table>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -168,80 +171,80 @@
                             "      <th>Datasource Name</th>\n",
                             "      <th>Archived</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
-                            "      <td>7B7E2494-5AC5-4195-8FB6-503AB742D0A4</td>\n",
-                            "      <td>Area B_Compressor Stage_AsInt32</td>\n",
+                            "      <td>A500C388-A3DF-4033-8BEE-980DB2D1744C</td>\n",
+                            "      <td>Area I_Compressor Power</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
-                            "      <td>NaN</td>\n",
-                            "      <td>54.200.148.162</td>\n",
+                            "      <td>kW</td>\n",
+                            "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1</th>\n",
-                            "      <td>B967C513-DB58-41CA-814B-2650465466BB</td>\n",
+                            "      <td>735C9627-F777-46C4-BAF5-B5B74F4534CF</td>\n",
                             "      <td>Area B_Temperature</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
                             "      <td>\u00b0F</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2</th>\n",
-                            "      <td>861F32F0-10DC-4E09-B1FF-66802CC63191</td>\n",
-                            "      <td>Area K_Optimizer</td>\n",
+                            "      <td>E1DA8119-AF56-452C-8FC9-9073E6070D15</td>\n",
+                            "      <td>Area B_Relative Humidity</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
-                            "      <td>NaN</td>\n",
+                            "      <td>%</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>3</th>\n",
-                            "      <td>BD8EB6B0-DA92-4F58-A92C-6FEB66DC75F2</td>\n",
+                            "      <td>7F8DE82F-DEC5-400B-88C6-84BA9A7ECB72</td>\n",
                             "      <td>Area E_Compressor Power</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
                             "      <td>kW</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>4</th>\n",
-                            "      <td>1B544029-7380-4C07-833C-CB1F9BFA253C</td>\n",
-                            "      <td>Area G_Temperature</td>\n",
+                            "      <td>3E671AFE-1EBB-476E-BBD3-44691DA6F77D</td>\n",
+                            "      <td>Area B_Compressor Stage</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
-                            "      <td>\u00b0F</td>\n",
+                            "      <td>string</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
-                            "                                     ID                             Name  \\\n",
-                            "0  7B7E2494-5AC5-4195-8FB6-503AB742D0A4  Area B_Compressor Stage_AsInt32   \n",
-                            "1  B967C513-DB58-41CA-814B-2650465466BB               Area B_Temperature   \n",
-                            "2  861F32F0-10DC-4E09-B1FF-66802CC63191                 Area K_Optimizer   \n",
-                            "3  BD8EB6B0-DA92-4F58-A92C-6FEB66DC75F2          Area E_Compressor Power   \n",
-                            "4  1B544029-7380-4C07-833C-CB1F9BFA253C               Area G_Temperature   \n",
+                            "                                     ID                      Name  \\\n",
+                            "0  A500C388-A3DF-4033-8BEE-980DB2D1744C   Area I_Compressor Power   \n",
+                            "1  735C9627-F777-46C4-BAF5-B5B74F4534CF        Area B_Temperature   \n",
+                            "2  E1DA8119-AF56-452C-8FC9-9073E6070D15  Area B_Relative Humidity   \n",
+                            "3  7F8DE82F-DEC5-400B-88C6-84BA9A7ECB72   Area E_Compressor Power   \n",
+                            "4  3E671AFE-1EBB-476E-BBD3-44691DA6F77D   Area B_Compressor Stage   \n",
                             "\n",
                             "   Description          Type Value Unit Of Measure Datasource Name  Archived  \n",
-                            "0          NaN  StoredSignal                   NaN  54.200.148.162     False  \n",
+                            "0          NaN  StoredSignal                    kW    Example Data     False  \n",
                             "1          NaN  StoredSignal                    \u00b0F    Example Data     False  \n",
-                            "2          NaN  StoredSignal                   NaN    Example Data     False  \n",
+                            "2          NaN  StoredSignal                     %    Example Data     False  \n",
                             "3          NaN  StoredSignal                    kW    Example Data     False  \n",
-                            "4          NaN  StoredSignal                    \u00b0F    Example Data     False  "
+                            "4          NaN  StoredSignal                string    Example Data     False  "
                         ]
                     },
                     "execution_count": 4,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -303,70 +306,70 @@
                             "      <th>Build Asset</th>\n",
                             "      <th>Build Path</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
-                            "      <td>7B7E2494-5AC5-4195-8FB6-503AB742D0A4</td>\n",
-                            "      <td>Area B_Compressor Stage_AsInt32</td>\n",
+                            "      <td>A500C388-A3DF-4033-8BEE-980DB2D1744C</td>\n",
+                            "      <td>Area I_Compressor Power</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
-                            "      <td>NaN</td>\n",
-                            "      <td>54.200.148.162</td>\n",
+                            "      <td>kW</td>\n",
+                            "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
-                            "      <td>Area B</td>\n",
+                            "      <td>Area I</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1</th>\n",
-                            "      <td>B967C513-DB58-41CA-814B-2650465466BB</td>\n",
+                            "      <td>735C9627-F777-46C4-BAF5-B5B74F4534CF</td>\n",
                             "      <td>Area B_Temperature</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
                             "      <td>\u00b0F</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
                             "      <td>Area B</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2</th>\n",
-                            "      <td>861F32F0-10DC-4E09-B1FF-66802CC63191</td>\n",
-                            "      <td>Area K_Optimizer</td>\n",
+                            "      <td>E1DA8119-AF56-452C-8FC9-9073E6070D15</td>\n",
+                            "      <td>Area B_Relative Humidity</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
-                            "      <td>NaN</td>\n",
+                            "      <td>%</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
-                            "      <td>Area K</td>\n",
+                            "      <td>Area B</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>3</th>\n",
-                            "      <td>BD8EB6B0-DA92-4F58-A92C-6FEB66DC75F2</td>\n",
+                            "      <td>7F8DE82F-DEC5-400B-88C6-84BA9A7ECB72</td>\n",
                             "      <td>Area E_Compressor Power</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
                             "      <td>kW</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
                             "      <td>Area E</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>4</th>\n",
-                            "      <td>1B544029-7380-4C07-833C-CB1F9BFA253C</td>\n",
-                            "      <td>Area G_Temperature</td>\n",
+                            "      <td>3E671AFE-1EBB-476E-BBD3-44691DA6F77D</td>\n",
+                            "      <td>Area B_Compressor Stage</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
-                            "      <td>\u00b0F</td>\n",
+                            "      <td>string</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
-                            "      <td>Area G</td>\n",
+                            "      <td>Area B</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>...</th>\n",
                             "      <td>...</td>\n",
                             "      <td>...</td>\n",
                             "      <td>...</td>\n",
@@ -375,116 +378,116 @@
                             "      <td>...</td>\n",
                             "      <td>...</td>\n",
                             "      <td>...</td>\n",
                             "      <td>...</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>65</th>\n",
-                            "      <td>2D5AA19A-F0C4-4300-A08B-8E27EA79831E</td>\n",
-                            "      <td>Area I_Wet Bulb</td>\n",
+                            "      <td>30F8FDAF-293A-4C86-9179-A7CF7B1847B4</td>\n",
+                            "      <td>Area D_Compressor Power</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
-                            "      <td>\u00b0F</td>\n",
+                            "      <td>kW</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
-                            "      <td>Area I</td>\n",
+                            "      <td>Area D</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>66</th>\n",
-                            "      <td>EB1CC8BE-17A1-4178-B6CE-051868187C65</td>\n",
-                            "      <td>Area K_Wet Bulb</td>\n",
+                            "      <td>D211CA9C-694E-4ED0-9D4E-D31EC1F07146</td>\n",
+                            "      <td>Area J_Compressor Stage</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
-                            "      <td>\u00b0F</td>\n",
+                            "      <td>string</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
-                            "      <td>Area K</td>\n",
+                            "      <td>Area J</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>67</th>\n",
-                            "      <td>57664B69-9E1B-4DAF-82DA-F9BC42C89EC4</td>\n",
-                            "      <td>Area D_Optimizer</td>\n",
+                            "      <td>AC44D00C-D817-4CEC-BD01-3CFC3BBD940C</td>\n",
+                            "      <td>Area I_Wet Bulb</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
-                            "      <td>NaN</td>\n",
+                            "      <td>\u00b0F</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
-                            "      <td>Area D</td>\n",
+                            "      <td>Area I</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>68</th>\n",
-                            "      <td>52A57D13-5EBC-4E05-970B-5EF06CABC1BF</td>\n",
-                            "      <td>Area E_Relative Humidity</td>\n",
+                            "      <td>70CF0317-E1F6-45FA-B399-87F59AC17186</td>\n",
+                            "      <td>Area H_Relative Humidity</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
                             "      <td>%</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
-                            "      <td>Area E</td>\n",
+                            "      <td>Area H</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>69</th>\n",
-                            "      <td>E79E3573-86CA-4B47-9249-FD6E486309DF</td>\n",
-                            "      <td>Area Z_Relative Humidity</td>\n",
+                            "      <td>2543324D-0154-4896-B3E5-7EBE6448F220</td>\n",
+                            "      <td>Area A_Wet Bulb</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
-                            "      <td>%</td>\n",
+                            "      <td>\u00b0F</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
-                            "      <td>Area Z</td>\n",
+                            "      <td>Area A</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "<p>70 rows \u00d7 9 columns</p>\n",
                             "</div>"
                         ],
                         "text/plain": [
-                            "                                      ID                             Name  \\\n",
-                            "0   7B7E2494-5AC5-4195-8FB6-503AB742D0A4  Area B_Compressor Stage_AsInt32   \n",
-                            "1   B967C513-DB58-41CA-814B-2650465466BB               Area B_Temperature   \n",
-                            "2   861F32F0-10DC-4E09-B1FF-66802CC63191                 Area K_Optimizer   \n",
-                            "3   BD8EB6B0-DA92-4F58-A92C-6FEB66DC75F2          Area E_Compressor Power   \n",
-                            "4   1B544029-7380-4C07-833C-CB1F9BFA253C               Area G_Temperature   \n",
-                            "..                                   ...                              ...   \n",
-                            "65  2D5AA19A-F0C4-4300-A08B-8E27EA79831E                  Area I_Wet Bulb   \n",
-                            "66  EB1CC8BE-17A1-4178-B6CE-051868187C65                  Area K_Wet Bulb   \n",
-                            "67  57664B69-9E1B-4DAF-82DA-F9BC42C89EC4                 Area D_Optimizer   \n",
-                            "68  52A57D13-5EBC-4E05-970B-5EF06CABC1BF         Area E_Relative Humidity   \n",
-                            "69  E79E3573-86CA-4B47-9249-FD6E486309DF         Area Z_Relative Humidity   \n",
+                            "                                      ID                      Name  \\\n",
+                            "0   A500C388-A3DF-4033-8BEE-980DB2D1744C   Area I_Compressor Power   \n",
+                            "1   735C9627-F777-46C4-BAF5-B5B74F4534CF        Area B_Temperature   \n",
+                            "2   E1DA8119-AF56-452C-8FC9-9073E6070D15  Area B_Relative Humidity   \n",
+                            "3   7F8DE82F-DEC5-400B-88C6-84BA9A7ECB72   Area E_Compressor Power   \n",
+                            "4   3E671AFE-1EBB-476E-BBD3-44691DA6F77D   Area B_Compressor Stage   \n",
+                            "..                                   ...                       ...   \n",
+                            "65  30F8FDAF-293A-4C86-9179-A7CF7B1847B4   Area D_Compressor Power   \n",
+                            "66  D211CA9C-694E-4ED0-9D4E-D31EC1F07146   Area J_Compressor Stage   \n",
+                            "67  AC44D00C-D817-4CEC-BD01-3CFC3BBD940C           Area I_Wet Bulb   \n",
+                            "68  70CF0317-E1F6-45FA-B399-87F59AC17186  Area H_Relative Humidity   \n",
+                            "69  2543324D-0154-4896-B3E5-7EBE6448F220           Area A_Wet Bulb   \n",
                             "\n",
                             "    Description          Type Value Unit Of Measure Datasource Name  Archived  \\\n",
-                            "0           NaN  StoredSignal                   NaN  54.200.148.162     False   \n",
+                            "0           NaN  StoredSignal                    kW    Example Data     False   \n",
                             "1           NaN  StoredSignal                    \u00b0F    Example Data     False   \n",
-                            "2           NaN  StoredSignal                   NaN    Example Data     False   \n",
+                            "2           NaN  StoredSignal                     %    Example Data     False   \n",
                             "3           NaN  StoredSignal                    kW    Example Data     False   \n",
-                            "4           NaN  StoredSignal                    \u00b0F    Example Data     False   \n",
+                            "4           NaN  StoredSignal                string    Example Data     False   \n",
                             "..          ...           ...                   ...             ...       ...   \n",
-                            "65          NaN  StoredSignal                    \u00b0F    Example Data     False   \n",
-                            "66          NaN  StoredSignal                    \u00b0F    Example Data     False   \n",
-                            "67          NaN  StoredSignal                   NaN    Example Data     False   \n",
+                            "65          NaN  StoredSignal                    kW    Example Data     False   \n",
+                            "66          NaN  StoredSignal                string    Example Data     False   \n",
+                            "67          NaN  StoredSignal                    \u00b0F    Example Data     False   \n",
                             "68          NaN  StoredSignal                     %    Example Data     False   \n",
-                            "69          NaN  StoredSignal                     %    Example Data     False   \n",
+                            "69          NaN  StoredSignal                    \u00b0F    Example Data     False   \n",
                             "\n",
                             "   Build Asset                    Build Path  \n",
-                            "0       Area B  My HVAC Units >> Facility #1  \n",
+                            "0       Area I  My HVAC Units >> Facility #1  \n",
                             "1       Area B  My HVAC Units >> Facility #1  \n",
-                            "2       Area K  My HVAC Units >> Facility #1  \n",
+                            "2       Area B  My HVAC Units >> Facility #1  \n",
                             "3       Area E  My HVAC Units >> Facility #1  \n",
-                            "4       Area G  My HVAC Units >> Facility #1  \n",
+                            "4       Area B  My HVAC Units >> Facility #1  \n",
                             "..         ...                           ...  \n",
-                            "65      Area I  My HVAC Units >> Facility #1  \n",
-                            "66      Area K  My HVAC Units >> Facility #1  \n",
-                            "67      Area D  My HVAC Units >> Facility #1  \n",
-                            "68      Area E  My HVAC Units >> Facility #1  \n",
-                            "69      Area Z  My HVAC Units >> Facility #1  \n",
+                            "65      Area D  My HVAC Units >> Facility #1  \n",
+                            "66      Area J  My HVAC Units >> Facility #1  \n",
+                            "67      Area I  My HVAC Units >> Facility #1  \n",
+                            "68      Area H  My HVAC Units >> Facility #1  \n",
+                            "69      Area A  My HVAC Units >> Facility #1  \n",
                             "\n",
                             "[70 rows x 9 columns]"
                         ]
                     },
                     "execution_count": 5,
                     "metadata": {},
                     "output_type": "execute_result"
@@ -552,15 +555,15 @@
             "cell_type": "code",
             "execution_count": 7,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<div style=\"background-color: #FFEEEE;color:black;text-align: left;\">Errors were encountered. Look for entries in \"Build Result\" that are not \"Success\".</div><table style=\"color:black;\"><tr><td style=\"background-color: #FFEEEE;\"></td><td style=\"background-color: #FFEEEE; text-align: left;\">Build Path</td><td style=\"background-color: #FFEEEE; text-align: left;\">Build Asset</td><td style=\"background-color: #FFEEEE; text-align: left;\">Build Template</td><td style=\"background-color: #FFEEEE; text-align: left;\">Build Result</td></tr><tr style=\"background-color: #FFEEEE;\"><td style=\"vertical-align: top;\">0</td><td style=\"text-align: left; vertical-align: top;\">My HVAC Units >> Facility #1</td><td style=\"text-align: left; vertical-align: top;\">Area B</td><td style=\"text-align: left; vertical-align: top;\">HVAC</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr><tr style=\"background-color: #FFEEEE;\"><td style=\"vertical-align: top;\">1</td><td style=\"text-align: left; vertical-align: top;\">My HVAC Units >> Facility #1</td><td style=\"text-align: left; vertical-align: top;\">Area K</td><td style=\"text-align: left; vertical-align: top;\">HVAC</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr><tr style=\"background-color: #FFEEEE;\"><td style=\"vertical-align: top;\">2</td><td style=\"text-align: left; vertical-align: top;\">My HVAC Units >> Facility #1</td><td style=\"text-align: left; vertical-align: top;\">Area E</td><td style=\"text-align: left; vertical-align: top;\">HVAC</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr><tr style=\"background-color: #FFEEEE;\"><td style=\"vertical-align: top;\">3</td><td style=\"text-align: left; vertical-align: top;\">My HVAC Units >> Facility #1</td><td style=\"text-align: left; vertical-align: top;\">Area G</td><td style=\"text-align: left; vertical-align: top;\">HVAC</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr><tr style=\"background-color: #FFEEEE;\"><td style=\"vertical-align: top;\">4</td><td style=\"text-align: left; vertical-align: top;\">My HVAC Units >> Facility #1</td><td style=\"text-align: left; vertical-align: top;\">Area J</td><td style=\"text-align: left; vertical-align: top;\">HVAC</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr><tr style=\"background-color: #FFEEEE;\"><td style=\"vertical-align: top;\">5</td><td style=\"text-align: left; vertical-align: top;\">My HVAC Units >> Facility #1</td><td style=\"text-align: left; vertical-align: top;\">Area C</td><td style=\"text-align: left; vertical-align: top;\">HVAC</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr><tr style=\"background-color: #FFEEEE;\"><td style=\"vertical-align: top;\">6</td><td style=\"text-align: left; vertical-align: top;\">My HVAC Units >> Facility #1</td><td style=\"text-align: left; vertical-align: top;\">Area D</td><td style=\"text-align: left; vertical-align: top;\">HVAC</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr><tr style=\"background-color: #FFEEEE;\"><td style=\"vertical-align: top;\">7</td><td style=\"text-align: left; vertical-align: top;\">My HVAC Units >> Facility #1</td><td style=\"text-align: left; vertical-align: top;\">Area H</td><td style=\"text-align: left; vertical-align: top;\">HVAC</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr><tr style=\"background-color: #FFEEEE;\"><td style=\"vertical-align: top;\">8</td><td style=\"text-align: left; vertical-align: top;\">My HVAC Units >> Facility #1</td><td style=\"text-align: left; vertical-align: top;\">Area Z</td><td style=\"text-align: left; vertical-align: top;\">HVAC</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr><tr style=\"background-color: #FFEEEE;\"><td style=\"vertical-align: top;\">9</td><td style=\"text-align: left; vertical-align: top;\">My HVAC Units >> Facility #1</td><td style=\"text-align: left; vertical-align: top;\">Area A</td><td style=\"text-align: left; vertical-align: top;\">HVAC</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr><tr style=\"background-color: #FFEEEE;\"><td style=\"vertical-align: top;\">10</td><td style=\"text-align: left; vertical-align: top;\">My HVAC Units >> Facility #1</td><td style=\"text-align: left; vertical-align: top;\">Area I</td><td style=\"text-align: left; vertical-align: top;\">HVAC</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr><tr style=\"background-color: #FFEEEE;\"><td style=\"vertical-align: top;\">11</td><td style=\"text-align: left; vertical-align: top;\">My HVAC Units >> Facility #1</td><td style=\"text-align: left; vertical-align: top;\">Area F</td><td style=\"text-align: left; vertical-align: top;\">HVAC</td><td style=\"text-align: left; vertical-align: top;\">The following issues could not be resolved:<br>(If the cause is not immediately obvious, make sure to check for circular references.)<br>\"My HVAC Units >> Facility #1 >> Area F >> Relative_Humidity [on HVAC class]\": No matching metadata row found<br>\"My HVAC Units >> Facility #1 >> Area F >> Temperature [on HVAC class]\": No matching metadata row found</td></tr></table>"
+                            "<div style=\"background-color: #FFEEEE;color:black; text-align: left;\">Errors were encountered. Look for entries in \"Build Result\" that are not \"Success\".</div><table class=\"tex2jax_ignore\" style=\"color:black;\"><tr><td style=\"background-color: #FFEEEE;\"></td><td style=\"background-color: #FFEEEE; text-align: left;\">Build Path</td><td style=\"background-color: #FFEEEE; text-align: left;\">Build Asset</td><td style=\"background-color: #FFEEEE; text-align: left;\">Build Template</td><td style=\"background-color: #FFEEEE; text-align: left;\">Build Result</td></tr><tr style=\"background-color: #FFEEEE;\"><td style=\"vertical-align: top;\">0</td><td style=\"text-align: left; vertical-align: top;\">My HVAC Units >> Facility #1</td><td style=\"text-align: left; vertical-align: top;\">Area I</td><td style=\"text-align: left; vertical-align: top;\">HVAC</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr><tr style=\"background-color: #FFEEEE;\"><td style=\"vertical-align: top;\">1</td><td style=\"text-align: left; vertical-align: top;\">My HVAC Units >> Facility #1</td><td style=\"text-align: left; vertical-align: top;\">Area B</td><td style=\"text-align: left; vertical-align: top;\">HVAC</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr><tr style=\"background-color: #FFEEEE;\"><td style=\"vertical-align: top;\">2</td><td style=\"text-align: left; vertical-align: top;\">My HVAC Units >> Facility #1</td><td style=\"text-align: left; vertical-align: top;\">Area E</td><td style=\"text-align: left; vertical-align: top;\">HVAC</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr><tr style=\"background-color: #FFEEEE;\"><td style=\"vertical-align: top;\">3</td><td style=\"text-align: left; vertical-align: top;\">My HVAC Units >> Facility #1</td><td style=\"text-align: left; vertical-align: top;\">Area H</td><td style=\"text-align: left; vertical-align: top;\">HVAC</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr><tr style=\"background-color: #FFEEEE;\"><td style=\"vertical-align: top;\">4</td><td style=\"text-align: left; vertical-align: top;\">My HVAC Units >> Facility #1</td><td style=\"text-align: left; vertical-align: top;\">Area G</td><td style=\"text-align: left; vertical-align: top;\">HVAC</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr><tr style=\"background-color: #FFEEEE;\"><td style=\"vertical-align: top;\">5</td><td style=\"text-align: left; vertical-align: top;\">My HVAC Units >> Facility #1</td><td style=\"text-align: left; vertical-align: top;\">Area K</td><td style=\"text-align: left; vertical-align: top;\">HVAC</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr><tr style=\"background-color: #FFEEEE;\"><td style=\"vertical-align: top;\">6</td><td style=\"text-align: left; vertical-align: top;\">My HVAC Units >> Facility #1</td><td style=\"text-align: left; vertical-align: top;\">Area A</td><td style=\"text-align: left; vertical-align: top;\">HVAC</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr><tr style=\"background-color: #FFEEEE;\"><td style=\"vertical-align: top;\">7</td><td style=\"text-align: left; vertical-align: top;\">My HVAC Units >> Facility #1</td><td style=\"text-align: left; vertical-align: top;\">Area J</td><td style=\"text-align: left; vertical-align: top;\">HVAC</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr><tr style=\"background-color: #FFEEEE;\"><td style=\"vertical-align: top;\">8</td><td style=\"text-align: left; vertical-align: top;\">My HVAC Units >> Facility #1</td><td style=\"text-align: left; vertical-align: top;\">Area C</td><td style=\"text-align: left; vertical-align: top;\">HVAC</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr><tr style=\"background-color: #FFEEEE;\"><td style=\"vertical-align: top;\">9</td><td style=\"text-align: left; vertical-align: top;\">My HVAC Units >> Facility #1</td><td style=\"text-align: left; vertical-align: top;\">Area F</td><td style=\"text-align: left; vertical-align: top;\">HVAC</td><td style=\"text-align: left; vertical-align: top;\">The following issues could not be resolved:<br>(If the cause is not immediately obvious, make sure to check for circular references.)<br>\"My HVAC Units >> Facility #1 >> Area F >> Relative Humidity [on HVAC class]\": No matching metadata row found<br>\"My HVAC Units >> Facility #1 >> Area F >> Temperature [on HVAC class]\": No matching metadata row found</td></tr><tr style=\"background-color: #FFEEEE;\"><td style=\"vertical-align: top;\">10</td><td style=\"text-align: left; vertical-align: top;\">My HVAC Units >> Facility #1</td><td style=\"text-align: left; vertical-align: top;\">Area D</td><td style=\"text-align: left; vertical-align: top;\">HVAC</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr><tr style=\"background-color: #FFEEEE;\"><td style=\"vertical-align: top;\">11</td><td style=\"text-align: left; vertical-align: top;\">My HVAC Units >> Facility #1</td><td style=\"text-align: left; vertical-align: top;\">Area Z</td><td style=\"text-align: left; vertical-align: top;\">HVAC</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr></table>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -601,117 +604,117 @@
                             "      <th>Template</th>\n",
                             "      <th>Build Result</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
-                            "      <td>D9A3F0B6-09CA-425D-A737-55384D6D0CA1</td>\n",
+                            "      <td>76E93E65-B284-4722-8B34-9142B04F34AA</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
                             "      <td>%</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
-                            "      <td>Area B_Relative Humidity</td>\n",
+                            "      <td>Area I_Relative Humidity</td>\n",
                             "      <td>True</td>\n",
                             "      <td>Relative Humidity</td>\n",
-                            "      <td>Area B</td>\n",
-                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area B</td>\n",
+                            "      <td>Area I</td>\n",
+                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area I</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
                             "      <td>HVAC</td>\n",
                             "      <td>Success</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1</th>\n",
-                            "      <td>B967C513-DB58-41CA-814B-2650465466BB</td>\n",
+                            "      <td>088D7186-54DB-402C-AFD7-528B4F426DB3</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
                             "      <td>\u00b0F</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
-                            "      <td>Area B_Temperature</td>\n",
+                            "      <td>Area I_Temperature</td>\n",
                             "      <td>True</td>\n",
                             "      <td>Temperature</td>\n",
-                            "      <td>Area B</td>\n",
-                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area B</td>\n",
+                            "      <td>Area I</td>\n",
+                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area I</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
                             "      <td>HVAC</td>\n",
                             "      <td>Success</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>Asset</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>Area B</td>\n",
-                            "      <td>Area B</td>\n",
-                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area B</td>\n",
+                            "      <td>Area I</td>\n",
+                            "      <td>Area I</td>\n",
+                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area I</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
                             "      <td>HVAC</td>\n",
                             "      <td>Success</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>3</th>\n",
-                            "      <td>F6BADC7D-0D6D-43B6-9776-19199E07683C</td>\n",
+                            "      <td>E1DA8119-AF56-452C-8FC9-9073E6070D15</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
                             "      <td>%</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
-                            "      <td>Area K_Relative Humidity</td>\n",
+                            "      <td>Area B_Relative Humidity</td>\n",
                             "      <td>True</td>\n",
                             "      <td>Relative Humidity</td>\n",
-                            "      <td>Area K</td>\n",
-                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area K</td>\n",
+                            "      <td>Area B</td>\n",
+                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area B</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
                             "      <td>HVAC</td>\n",
                             "      <td>Success</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>4</th>\n",
-                            "      <td>64B266EF-2B11-4721-9E5E-A071462BC15A</td>\n",
+                            "      <td>735C9627-F777-46C4-BAF5-B5B74F4534CF</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
                             "      <td>\u00b0F</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
-                            "      <td>Area K_Temperature</td>\n",
+                            "      <td>Area B_Temperature</td>\n",
                             "      <td>True</td>\n",
                             "      <td>Temperature</td>\n",
-                            "      <td>Area K</td>\n",
-                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area K</td>\n",
+                            "      <td>Area B</td>\n",
+                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area B</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
                             "      <td>HVAC</td>\n",
                             "      <td>Success</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>5</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>Asset</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>Area K</td>\n",
-                            "      <td>Area K</td>\n",
-                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area K</td>\n",
+                            "      <td>Area B</td>\n",
+                            "      <td>Area B</td>\n",
+                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area B</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
                             "      <td>HVAC</td>\n",
                             "      <td>Success</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>6</th>\n",
-                            "      <td>52A57D13-5EBC-4E05-970B-5EF06CABC1BF</td>\n",
+                            "      <td>32E43B48-174B-4291-AED3-862C23681BB8</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
                             "      <td>%</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
                             "      <td>Area E_Relative Humidity</td>\n",
                             "      <td>True</td>\n",
@@ -720,15 +723,15 @@
                             "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area E</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
                             "      <td>HVAC</td>\n",
                             "      <td>Success</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>7</th>\n",
-                            "      <td>078E6690-63DD-443A-B1F1-535C45A74BB3</td>\n",
+                            "      <td>2A1E3E78-8F08-4601-963F-D866FB1F3523</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
                             "      <td>\u00b0F</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
                             "      <td>Area E_Temperature</td>\n",
                             "      <td>True</td>\n",
@@ -754,564 +757,585 @@
                             "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area E</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
                             "      <td>HVAC</td>\n",
                             "      <td>Success</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>9</th>\n",
-                            "      <td>965BD8D5-FEB1-4F81-B80A-6B5A4664A3E6</td>\n",
+                            "      <td>70CF0317-E1F6-45FA-B399-87F59AC17186</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
                             "      <td>%</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
-                            "      <td>Area G_Relative Humidity</td>\n",
+                            "      <td>Area H_Relative Humidity</td>\n",
                             "      <td>True</td>\n",
                             "      <td>Relative Humidity</td>\n",
-                            "      <td>Area G</td>\n",
-                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area G</td>\n",
+                            "      <td>Area H</td>\n",
+                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area H</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
                             "      <td>HVAC</td>\n",
                             "      <td>Success</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>10</th>\n",
-                            "      <td>1B544029-7380-4C07-833C-CB1F9BFA253C</td>\n",
+                            "      <td>6098E00F-32C9-47BB-A579-AB8DBF66426E</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
                             "      <td>\u00b0F</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
-                            "      <td>Area G_Temperature</td>\n",
+                            "      <td>Area H_Temperature</td>\n",
                             "      <td>True</td>\n",
                             "      <td>Temperature</td>\n",
-                            "      <td>Area G</td>\n",
-                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area G</td>\n",
+                            "      <td>Area H</td>\n",
+                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area H</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
                             "      <td>HVAC</td>\n",
                             "      <td>Success</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>11</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>Asset</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>Area G</td>\n",
-                            "      <td>Area G</td>\n",
-                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area G</td>\n",
+                            "      <td>Area H</td>\n",
+                            "      <td>Area H</td>\n",
+                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area H</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
                             "      <td>HVAC</td>\n",
                             "      <td>Success</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>12</th>\n",
-                            "      <td>AB9A0CE0-D209-4D80-85CD-100A815EB7EF</td>\n",
+                            "      <td>EC3180D2-7552-48A7-9163-469E318FC620</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
                             "      <td>%</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
-                            "      <td>Area J_Relative Humidity</td>\n",
+                            "      <td>Area G_Relative Humidity</td>\n",
                             "      <td>True</td>\n",
                             "      <td>Relative Humidity</td>\n",
-                            "      <td>Area J</td>\n",
-                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area J</td>\n",
+                            "      <td>Area G</td>\n",
+                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area G</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
                             "      <td>HVAC</td>\n",
                             "      <td>Success</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>13</th>\n",
-                            "      <td>D4A33C9B-E675-4CDA-BB18-9DCDD638E250</td>\n",
+                            "      <td>603691BF-0805-4312-B313-6B664CAA00AC</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
                             "      <td>\u00b0F</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
-                            "      <td>Area J_Temperature</td>\n",
+                            "      <td>Area G_Temperature</td>\n",
                             "      <td>True</td>\n",
                             "      <td>Temperature</td>\n",
-                            "      <td>Area J</td>\n",
-                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area J</td>\n",
+                            "      <td>Area G</td>\n",
+                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area G</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
                             "      <td>HVAC</td>\n",
                             "      <td>Success</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>14</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>Asset</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>Area J</td>\n",
-                            "      <td>Area J</td>\n",
-                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area J</td>\n",
+                            "      <td>Area G</td>\n",
+                            "      <td>Area G</td>\n",
+                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area G</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
                             "      <td>HVAC</td>\n",
                             "      <td>Success</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>15</th>\n",
-                            "      <td>5E7A4906-931D-490F-B9DE-DD12CAC1430E</td>\n",
+                            "      <td>601D5764-86B4-4FAA-BFF8-102171C0895E</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
                             "      <td>%</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
-                            "      <td>Area C_Relative Humidity</td>\n",
+                            "      <td>Area K_Relative Humidity</td>\n",
                             "      <td>True</td>\n",
                             "      <td>Relative Humidity</td>\n",
-                            "      <td>Area C</td>\n",
-                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area C</td>\n",
+                            "      <td>Area K</td>\n",
+                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area K</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
                             "      <td>HVAC</td>\n",
                             "      <td>Success</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>16</th>\n",
-                            "      <td>46E29219-3339-4F50-8137-C9C23B16DEF9</td>\n",
+                            "      <td>3D0C814D-1BBC-4931-B6F0-F5CF38D050FF</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
                             "      <td>\u00b0F</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
-                            "      <td>Area C_Temperature</td>\n",
+                            "      <td>Area K_Temperature</td>\n",
                             "      <td>True</td>\n",
                             "      <td>Temperature</td>\n",
-                            "      <td>Area C</td>\n",
-                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area C</td>\n",
+                            "      <td>Area K</td>\n",
+                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area K</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
                             "      <td>HVAC</td>\n",
                             "      <td>Success</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>17</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>Asset</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>Area C</td>\n",
-                            "      <td>Area C</td>\n",
-                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area C</td>\n",
+                            "      <td>Area K</td>\n",
+                            "      <td>Area K</td>\n",
+                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area K</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
                             "      <td>HVAC</td>\n",
                             "      <td>Success</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>18</th>\n",
-                            "      <td>AB3B81B0-8A65-4DDE-A650-DD3311900239</td>\n",
+                            "      <td>E9744446-848A-4461-A730-29CD0C97A7DC</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
                             "      <td>%</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
-                            "      <td>Area D_Relative Humidity</td>\n",
+                            "      <td>Area A_Relative Humidity</td>\n",
                             "      <td>True</td>\n",
                             "      <td>Relative Humidity</td>\n",
-                            "      <td>Area D</td>\n",
-                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area D</td>\n",
+                            "      <td>Area A</td>\n",
+                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area A</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
                             "      <td>HVAC</td>\n",
                             "      <td>Success</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>19</th>\n",
-                            "      <td>06BD8E98-DA1B-4984-B19F-367AD09340A2</td>\n",
+                            "      <td>F8B2EF0E-BAB2-441D-B031-6F920099D74A</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
                             "      <td>\u00b0F</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
-                            "      <td>Area D_Temperature</td>\n",
+                            "      <td>Area A_Temperature</td>\n",
                             "      <td>True</td>\n",
                             "      <td>Temperature</td>\n",
-                            "      <td>Area D</td>\n",
-                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area D</td>\n",
+                            "      <td>Area A</td>\n",
+                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area A</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
                             "      <td>HVAC</td>\n",
                             "      <td>Success</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>20</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>Asset</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>Area D</td>\n",
-                            "      <td>Area D</td>\n",
-                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area D</td>\n",
+                            "      <td>Area A</td>\n",
+                            "      <td>Area A</td>\n",
+                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area A</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
                             "      <td>HVAC</td>\n",
                             "      <td>Success</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>21</th>\n",
-                            "      <td>1E40325D-33DF-4C91-9B57-9CC12898BFC9</td>\n",
+                            "      <td>07EFC44C-FE26-475E-BF65-BE0AC2F890D2</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
                             "      <td>%</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
-                            "      <td>Area H_Relative Humidity</td>\n",
+                            "      <td>Area J_Relative Humidity</td>\n",
                             "      <td>True</td>\n",
                             "      <td>Relative Humidity</td>\n",
-                            "      <td>Area H</td>\n",
-                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area H</td>\n",
+                            "      <td>Area J</td>\n",
+                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area J</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
                             "      <td>HVAC</td>\n",
                             "      <td>Success</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>22</th>\n",
-                            "      <td>30E7BF71-A103-4DEE-BFFB-D99F95477615</td>\n",
+                            "      <td>74DF4A2A-C8AA-4B8D-9486-5F73E41B3283</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
                             "      <td>\u00b0F</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
-                            "      <td>Area H_Temperature</td>\n",
+                            "      <td>Area J_Temperature</td>\n",
                             "      <td>True</td>\n",
                             "      <td>Temperature</td>\n",
-                            "      <td>Area H</td>\n",
-                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area H</td>\n",
+                            "      <td>Area J</td>\n",
+                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area J</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
                             "      <td>HVAC</td>\n",
                             "      <td>Success</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>23</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>Asset</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>Area H</td>\n",
-                            "      <td>Area H</td>\n",
-                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area H</td>\n",
+                            "      <td>Area J</td>\n",
+                            "      <td>Area J</td>\n",
+                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area J</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
                             "      <td>HVAC</td>\n",
                             "      <td>Success</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>24</th>\n",
-                            "      <td>E79E3573-86CA-4B47-9249-FD6E486309DF</td>\n",
+                            "      <td>FBD71574-5153-479D-BBF2-CDA5C21C0888</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
                             "      <td>%</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
-                            "      <td>Area Z_Relative Humidity</td>\n",
+                            "      <td>Area C_Relative Humidity</td>\n",
                             "      <td>True</td>\n",
                             "      <td>Relative Humidity</td>\n",
-                            "      <td>Area Z</td>\n",
-                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area Z</td>\n",
+                            "      <td>Area C</td>\n",
+                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area C</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
                             "      <td>HVAC</td>\n",
                             "      <td>Success</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>25</th>\n",
-                            "      <td>C7790101-63F8-4567-8335-F60FB5E82F35</td>\n",
+                            "      <td>BDD6B3E7-6A62-4C43-AC60-4F6EF8525134</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
                             "      <td>\u00b0F</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
-                            "      <td>Area Z_Temperature</td>\n",
+                            "      <td>Area C_Temperature</td>\n",
                             "      <td>True</td>\n",
                             "      <td>Temperature</td>\n",
-                            "      <td>Area Z</td>\n",
-                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area Z</td>\n",
+                            "      <td>Area C</td>\n",
+                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area C</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
                             "      <td>HVAC</td>\n",
                             "      <td>Success</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>26</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>Asset</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>Area Z</td>\n",
-                            "      <td>Area Z</td>\n",
-                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area Z</td>\n",
+                            "      <td>Area C</td>\n",
+                            "      <td>Area C</td>\n",
+                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area C</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
                             "      <td>HVAC</td>\n",
                             "      <td>Success</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>27</th>\n",
-                            "      <td>44AF42F6-4041-422D-80DD-A27AA9E4A1C4</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>Asset</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>Area F</td>\n",
+                            "      <td>Area F</td>\n",
+                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area F</td>\n",
+                            "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
+                            "      <td>HVAC</td>\n",
+                            "      <td>Success</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>28</th>\n",
+                            "      <td>13DE0DEB-DD2C-4E1A-800C-13DC45B2ADAF</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
                             "      <td>%</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
-                            "      <td>Area A_Relative Humidity</td>\n",
+                            "      <td>Area D_Relative Humidity</td>\n",
                             "      <td>True</td>\n",
                             "      <td>Relative Humidity</td>\n",
-                            "      <td>Area A</td>\n",
-                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area A</td>\n",
+                            "      <td>Area D</td>\n",
+                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area D</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
                             "      <td>HVAC</td>\n",
                             "      <td>Success</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>28</th>\n",
-                            "      <td>C1F1002A-469E-47D1-83AB-99FD17650B55</td>\n",
+                            "      <th>29</th>\n",
+                            "      <td>C90CB4E9-6CF7-4F13-BA6D-5078EA33ADAB</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
                             "      <td>\u00b0F</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
-                            "      <td>Area A_Temperature</td>\n",
+                            "      <td>Area D_Temperature</td>\n",
                             "      <td>True</td>\n",
                             "      <td>Temperature</td>\n",
-                            "      <td>Area A</td>\n",
-                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area A</td>\n",
+                            "      <td>Area D</td>\n",
+                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area D</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
                             "      <td>HVAC</td>\n",
                             "      <td>Success</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>29</th>\n",
+                            "      <th>30</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>Asset</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>Area A</td>\n",
-                            "      <td>Area A</td>\n",
-                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area A</td>\n",
+                            "      <td>Area D</td>\n",
+                            "      <td>Area D</td>\n",
+                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area D</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
                             "      <td>HVAC</td>\n",
                             "      <td>Success</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>30</th>\n",
-                            "      <td>A00EE0E0-2127-4CBD-A301-1DF629D7B7FC</td>\n",
+                            "      <th>31</th>\n",
+                            "      <td>848594A9-469A-412D-8560-02A475ADA21F</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
                             "      <td>%</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
-                            "      <td>Area I_Relative Humidity</td>\n",
+                            "      <td>Area Z_Relative Humidity</td>\n",
                             "      <td>True</td>\n",
                             "      <td>Relative Humidity</td>\n",
-                            "      <td>Area I</td>\n",
-                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area I</td>\n",
+                            "      <td>Area Z</td>\n",
+                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area Z</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
                             "      <td>HVAC</td>\n",
                             "      <td>Success</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>31</th>\n",
-                            "      <td>2DE6799C-08A3-4434-9FC6-49969EE3DCBA</td>\n",
+                            "      <th>32</th>\n",
+                            "      <td>6712F9DD-49D5-4448-B370-178EF20FC283</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
                             "      <td>\u00b0F</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
-                            "      <td>Area I_Temperature</td>\n",
+                            "      <td>Area Z_Temperature</td>\n",
                             "      <td>True</td>\n",
                             "      <td>Temperature</td>\n",
-                            "      <td>Area I</td>\n",
-                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area I</td>\n",
+                            "      <td>Area Z</td>\n",
+                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area Z</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
                             "      <td>HVAC</td>\n",
                             "      <td>Success</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>32</th>\n",
+                            "      <th>33</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>Asset</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>Area I</td>\n",
-                            "      <td>Area I</td>\n",
-                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area I</td>\n",
+                            "      <td>Area Z</td>\n",
+                            "      <td>Area Z</td>\n",
+                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area Z</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
                             "      <td>HVAC</td>\n",
                             "      <td>Success</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
                             "                                      ID  Description          Type  \\\n",
-                            "0   D9A3F0B6-09CA-425D-A737-55384D6D0CA1          NaN  StoredSignal   \n",
-                            "1   B967C513-DB58-41CA-814B-2650465466BB          NaN  StoredSignal   \n",
+                            "0   76E93E65-B284-4722-8B34-9142B04F34AA          NaN  StoredSignal   \n",
+                            "1   088D7186-54DB-402C-AFD7-528B4F426DB3          NaN  StoredSignal   \n",
                             "2                                    NaN          NaN         Asset   \n",
-                            "3   F6BADC7D-0D6D-43B6-9776-19199E07683C          NaN  StoredSignal   \n",
-                            "4   64B266EF-2B11-4721-9E5E-A071462BC15A          NaN  StoredSignal   \n",
+                            "3   E1DA8119-AF56-452C-8FC9-9073E6070D15          NaN  StoredSignal   \n",
+                            "4   735C9627-F777-46C4-BAF5-B5B74F4534CF          NaN  StoredSignal   \n",
                             "5                                    NaN          NaN         Asset   \n",
-                            "6   52A57D13-5EBC-4E05-970B-5EF06CABC1BF          NaN  StoredSignal   \n",
-                            "7   078E6690-63DD-443A-B1F1-535C45A74BB3          NaN  StoredSignal   \n",
+                            "6   32E43B48-174B-4291-AED3-862C23681BB8          NaN  StoredSignal   \n",
+                            "7   2A1E3E78-8F08-4601-963F-D866FB1F3523          NaN  StoredSignal   \n",
                             "8                                    NaN          NaN         Asset   \n",
-                            "9   965BD8D5-FEB1-4F81-B80A-6B5A4664A3E6          NaN  StoredSignal   \n",
-                            "10  1B544029-7380-4C07-833C-CB1F9BFA253C          NaN  StoredSignal   \n",
+                            "9   70CF0317-E1F6-45FA-B399-87F59AC17186          NaN  StoredSignal   \n",
+                            "10  6098E00F-32C9-47BB-A579-AB8DBF66426E          NaN  StoredSignal   \n",
                             "11                                   NaN          NaN         Asset   \n",
-                            "12  AB9A0CE0-D209-4D80-85CD-100A815EB7EF          NaN  StoredSignal   \n",
-                            "13  D4A33C9B-E675-4CDA-BB18-9DCDD638E250          NaN  StoredSignal   \n",
+                            "12  EC3180D2-7552-48A7-9163-469E318FC620          NaN  StoredSignal   \n",
+                            "13  603691BF-0805-4312-B313-6B664CAA00AC          NaN  StoredSignal   \n",
                             "14                                   NaN          NaN         Asset   \n",
-                            "15  5E7A4906-931D-490F-B9DE-DD12CAC1430E          NaN  StoredSignal   \n",
-                            "16  46E29219-3339-4F50-8137-C9C23B16DEF9          NaN  StoredSignal   \n",
+                            "15  601D5764-86B4-4FAA-BFF8-102171C0895E          NaN  StoredSignal   \n",
+                            "16  3D0C814D-1BBC-4931-B6F0-F5CF38D050FF          NaN  StoredSignal   \n",
                             "17                                   NaN          NaN         Asset   \n",
-                            "18  AB3B81B0-8A65-4DDE-A650-DD3311900239          NaN  StoredSignal   \n",
-                            "19  06BD8E98-DA1B-4984-B19F-367AD09340A2          NaN  StoredSignal   \n",
+                            "18  E9744446-848A-4461-A730-29CD0C97A7DC          NaN  StoredSignal   \n",
+                            "19  F8B2EF0E-BAB2-441D-B031-6F920099D74A          NaN  StoredSignal   \n",
                             "20                                   NaN          NaN         Asset   \n",
-                            "21  1E40325D-33DF-4C91-9B57-9CC12898BFC9          NaN  StoredSignal   \n",
-                            "22  30E7BF71-A103-4DEE-BFFB-D99F95477615          NaN  StoredSignal   \n",
+                            "21  07EFC44C-FE26-475E-BF65-BE0AC2F890D2          NaN  StoredSignal   \n",
+                            "22  74DF4A2A-C8AA-4B8D-9486-5F73E41B3283          NaN  StoredSignal   \n",
                             "23                                   NaN          NaN         Asset   \n",
-                            "24  E79E3573-86CA-4B47-9249-FD6E486309DF          NaN  StoredSignal   \n",
-                            "25  C7790101-63F8-4567-8335-F60FB5E82F35          NaN  StoredSignal   \n",
+                            "24  FBD71574-5153-479D-BBF2-CDA5C21C0888          NaN  StoredSignal   \n",
+                            "25  BDD6B3E7-6A62-4C43-AC60-4F6EF8525134          NaN  StoredSignal   \n",
                             "26                                   NaN          NaN         Asset   \n",
-                            "27  44AF42F6-4041-422D-80DD-A27AA9E4A1C4          NaN  StoredSignal   \n",
-                            "28  C1F1002A-469E-47D1-83AB-99FD17650B55          NaN  StoredSignal   \n",
-                            "29                                   NaN          NaN         Asset   \n",
-                            "30  A00EE0E0-2127-4CBD-A301-1DF629D7B7FC          NaN  StoredSignal   \n",
-                            "31  2DE6799C-08A3-4434-9FC6-49969EE3DCBA          NaN  StoredSignal   \n",
-                            "32                                   NaN          NaN         Asset   \n",
+                            "27                                   NaN          NaN         Asset   \n",
+                            "28  13DE0DEB-DD2C-4E1A-800C-13DC45B2ADAF          NaN  StoredSignal   \n",
+                            "29  C90CB4E9-6CF7-4F13-BA6D-5078EA33ADAB          NaN  StoredSignal   \n",
+                            "30                                   NaN          NaN         Asset   \n",
+                            "31  848594A9-469A-412D-8560-02A475ADA21F          NaN  StoredSignal   \n",
+                            "32  6712F9DD-49D5-4448-B370-178EF20FC283          NaN  StoredSignal   \n",
+                            "33                                   NaN          NaN         Asset   \n",
                             "\n",
                             "   Value Unit Of Measure Datasource Name Archived           Referenced Name  \\\n",
-                            "0                      %    Example Data    False  Area B_Relative Humidity   \n",
-                            "1                     \u00b0F    Example Data    False        Area B_Temperature   \n",
+                            "0                      %    Example Data    False  Area I_Relative Humidity   \n",
+                            "1                     \u00b0F    Example Data    False        Area I_Temperature   \n",
                             "2                    NaN             NaN      NaN                       NaN   \n",
-                            "3                      %    Example Data    False  Area K_Relative Humidity   \n",
-                            "4                     \u00b0F    Example Data    False        Area K_Temperature   \n",
+                            "3                      %    Example Data    False  Area B_Relative Humidity   \n",
+                            "4                     \u00b0F    Example Data    False        Area B_Temperature   \n",
                             "5                    NaN             NaN      NaN                       NaN   \n",
                             "6                      %    Example Data    False  Area E_Relative Humidity   \n",
                             "7                     \u00b0F    Example Data    False        Area E_Temperature   \n",
                             "8                    NaN             NaN      NaN                       NaN   \n",
-                            "9                      %    Example Data    False  Area G_Relative Humidity   \n",
-                            "10                    \u00b0F    Example Data    False        Area G_Temperature   \n",
+                            "9                      %    Example Data    False  Area H_Relative Humidity   \n",
+                            "10                    \u00b0F    Example Data    False        Area H_Temperature   \n",
                             "11                   NaN             NaN      NaN                       NaN   \n",
-                            "12                     %    Example Data    False  Area J_Relative Humidity   \n",
-                            "13                    \u00b0F    Example Data    False        Area J_Temperature   \n",
+                            "12                     %    Example Data    False  Area G_Relative Humidity   \n",
+                            "13                    \u00b0F    Example Data    False        Area G_Temperature   \n",
                             "14                   NaN             NaN      NaN                       NaN   \n",
-                            "15                     %    Example Data    False  Area C_Relative Humidity   \n",
-                            "16                    \u00b0F    Example Data    False        Area C_Temperature   \n",
+                            "15                     %    Example Data    False  Area K_Relative Humidity   \n",
+                            "16                    \u00b0F    Example Data    False        Area K_Temperature   \n",
                             "17                   NaN             NaN      NaN                       NaN   \n",
-                            "18                     %    Example Data    False  Area D_Relative Humidity   \n",
-                            "19                    \u00b0F    Example Data    False        Area D_Temperature   \n",
+                            "18                     %    Example Data    False  Area A_Relative Humidity   \n",
+                            "19                    \u00b0F    Example Data    False        Area A_Temperature   \n",
                             "20                   NaN             NaN      NaN                       NaN   \n",
-                            "21                     %    Example Data    False  Area H_Relative Humidity   \n",
-                            "22                    \u00b0F    Example Data    False        Area H_Temperature   \n",
+                            "21                     %    Example Data    False  Area J_Relative Humidity   \n",
+                            "22                    \u00b0F    Example Data    False        Area J_Temperature   \n",
                             "23                   NaN             NaN      NaN                       NaN   \n",
-                            "24                     %    Example Data    False  Area Z_Relative Humidity   \n",
-                            "25                    \u00b0F    Example Data    False        Area Z_Temperature   \n",
+                            "24                     %    Example Data    False  Area C_Relative Humidity   \n",
+                            "25                    \u00b0F    Example Data    False        Area C_Temperature   \n",
                             "26                   NaN             NaN      NaN                       NaN   \n",
-                            "27                     %    Example Data    False  Area A_Relative Humidity   \n",
-                            "28                    \u00b0F    Example Data    False        Area A_Temperature   \n",
-                            "29                   NaN             NaN      NaN                       NaN   \n",
-                            "30                     %    Example Data    False  Area I_Relative Humidity   \n",
-                            "31                    \u00b0F    Example Data    False        Area I_Temperature   \n",
-                            "32                   NaN             NaN      NaN                       NaN   \n",
+                            "27                   NaN             NaN      NaN                       NaN   \n",
+                            "28                     %    Example Data    False  Area D_Relative Humidity   \n",
+                            "29                    \u00b0F    Example Data    False        Area D_Temperature   \n",
+                            "30                   NaN             NaN      NaN                       NaN   \n",
+                            "31                     %    Example Data    False  Area Z_Relative Humidity   \n",
+                            "32                    \u00b0F    Example Data    False        Area Z_Temperature   \n",
+                            "33                   NaN             NaN      NaN                       NaN   \n",
                             "\n",
                             "   Reference               Name   Asset  \\\n",
-                            "0       True  Relative Humidity  Area B   \n",
-                            "1       True        Temperature  Area B   \n",
-                            "2        NaN             Area B  Area B   \n",
-                            "3       True  Relative Humidity  Area K   \n",
-                            "4       True        Temperature  Area K   \n",
-                            "5        NaN             Area K  Area K   \n",
+                            "0       True  Relative Humidity  Area I   \n",
+                            "1       True        Temperature  Area I   \n",
+                            "2        NaN             Area I  Area I   \n",
+                            "3       True  Relative Humidity  Area B   \n",
+                            "4       True        Temperature  Area B   \n",
+                            "5        NaN             Area B  Area B   \n",
                             "6       True  Relative Humidity  Area E   \n",
                             "7       True        Temperature  Area E   \n",
                             "8        NaN             Area E  Area E   \n",
-                            "9       True  Relative Humidity  Area G   \n",
-                            "10      True        Temperature  Area G   \n",
-                            "11       NaN             Area G  Area G   \n",
-                            "12      True  Relative Humidity  Area J   \n",
-                            "13      True        Temperature  Area J   \n",
-                            "14       NaN             Area J  Area J   \n",
-                            "15      True  Relative Humidity  Area C   \n",
-                            "16      True        Temperature  Area C   \n",
-                            "17       NaN             Area C  Area C   \n",
-                            "18      True  Relative Humidity  Area D   \n",
-                            "19      True        Temperature  Area D   \n",
-                            "20       NaN             Area D  Area D   \n",
-                            "21      True  Relative Humidity  Area H   \n",
-                            "22      True        Temperature  Area H   \n",
-                            "23       NaN             Area H  Area H   \n",
-                            "24      True  Relative Humidity  Area Z   \n",
-                            "25      True        Temperature  Area Z   \n",
-                            "26       NaN             Area Z  Area Z   \n",
-                            "27      True  Relative Humidity  Area A   \n",
-                            "28      True        Temperature  Area A   \n",
-                            "29       NaN             Area A  Area A   \n",
-                            "30      True  Relative Humidity  Area I   \n",
-                            "31      True        Temperature  Area I   \n",
-                            "32       NaN             Area I  Area I   \n",
+                            "9       True  Relative Humidity  Area H   \n",
+                            "10      True        Temperature  Area H   \n",
+                            "11       NaN             Area H  Area H   \n",
+                            "12      True  Relative Humidity  Area G   \n",
+                            "13      True        Temperature  Area G   \n",
+                            "14       NaN             Area G  Area G   \n",
+                            "15      True  Relative Humidity  Area K   \n",
+                            "16      True        Temperature  Area K   \n",
+                            "17       NaN             Area K  Area K   \n",
+                            "18      True  Relative Humidity  Area A   \n",
+                            "19      True        Temperature  Area A   \n",
+                            "20       NaN             Area A  Area A   \n",
+                            "21      True  Relative Humidity  Area J   \n",
+                            "22      True        Temperature  Area J   \n",
+                            "23       NaN             Area J  Area J   \n",
+                            "24      True  Relative Humidity  Area C   \n",
+                            "25      True        Temperature  Area C   \n",
+                            "26       NaN             Area C  Area C   \n",
+                            "27       NaN             Area F  Area F   \n",
+                            "28      True  Relative Humidity  Area D   \n",
+                            "29      True        Temperature  Area D   \n",
+                            "30       NaN             Area D  Area D   \n",
+                            "31      True  Relative Humidity  Area Z   \n",
+                            "32      True        Temperature  Area Z   \n",
+                            "33       NaN             Area Z  Area Z   \n",
                             "\n",
                             "                              Asset Object                          Path  \\\n",
-                            "0   My HVAC Units >> Facility #1 >> Area B  My HVAC Units >> Facility #1   \n",
-                            "1   My HVAC Units >> Facility #1 >> Area B  My HVAC Units >> Facility #1   \n",
-                            "2   My HVAC Units >> Facility #1 >> Area B  My HVAC Units >> Facility #1   \n",
-                            "3   My HVAC Units >> Facility #1 >> Area K  My HVAC Units >> Facility #1   \n",
-                            "4   My HVAC Units >> Facility #1 >> Area K  My HVAC Units >> Facility #1   \n",
-                            "5   My HVAC Units >> Facility #1 >> Area K  My HVAC Units >> Facility #1   \n",
+                            "0   My HVAC Units >> Facility #1 >> Area I  My HVAC Units >> Facility #1   \n",
+                            "1   My HVAC Units >> Facility #1 >> Area I  My HVAC Units >> Facility #1   \n",
+                            "2   My HVAC Units >> Facility #1 >> Area I  My HVAC Units >> Facility #1   \n",
+                            "3   My HVAC Units >> Facility #1 >> Area B  My HVAC Units >> Facility #1   \n",
+                            "4   My HVAC Units >> Facility #1 >> Area B  My HVAC Units >> Facility #1   \n",
+                            "5   My HVAC Units >> Facility #1 >> Area B  My HVAC Units >> Facility #1   \n",
                             "6   My HVAC Units >> Facility #1 >> Area E  My HVAC Units >> Facility #1   \n",
                             "7   My HVAC Units >> Facility #1 >> Area E  My HVAC Units >> Facility #1   \n",
                             "8   My HVAC Units >> Facility #1 >> Area E  My HVAC Units >> Facility #1   \n",
-                            "9   My HVAC Units >> Facility #1 >> Area G  My HVAC Units >> Facility #1   \n",
-                            "10  My HVAC Units >> Facility #1 >> Area G  My HVAC Units >> Facility #1   \n",
-                            "11  My HVAC Units >> Facility #1 >> Area G  My HVAC Units >> Facility #1   \n",
-                            "12  My HVAC Units >> Facility #1 >> Area J  My HVAC Units >> Facility #1   \n",
-                            "13  My HVAC Units >> Facility #1 >> Area J  My HVAC Units >> Facility #1   \n",
-                            "14  My HVAC Units >> Facility #1 >> Area J  My HVAC Units >> Facility #1   \n",
-                            "15  My HVAC Units >> Facility #1 >> Area C  My HVAC Units >> Facility #1   \n",
-                            "16  My HVAC Units >> Facility #1 >> Area C  My HVAC Units >> Facility #1   \n",
-                            "17  My HVAC Units >> Facility #1 >> Area C  My HVAC Units >> Facility #1   \n",
-                            "18  My HVAC Units >> Facility #1 >> Area D  My HVAC Units >> Facility #1   \n",
-                            "19  My HVAC Units >> Facility #1 >> Area D  My HVAC Units >> Facility #1   \n",
-                            "20  My HVAC Units >> Facility #1 >> Area D  My HVAC Units >> Facility #1   \n",
-                            "21  My HVAC Units >> Facility #1 >> Area H  My HVAC Units >> Facility #1   \n",
-                            "22  My HVAC Units >> Facility #1 >> Area H  My HVAC Units >> Facility #1   \n",
-                            "23  My HVAC Units >> Facility #1 >> Area H  My HVAC Units >> Facility #1   \n",
-                            "24  My HVAC Units >> Facility #1 >> Area Z  My HVAC Units >> Facility #1   \n",
-                            "25  My HVAC Units >> Facility #1 >> Area Z  My HVAC Units >> Facility #1   \n",
-                            "26  My HVAC Units >> Facility #1 >> Area Z  My HVAC Units >> Facility #1   \n",
-                            "27  My HVAC Units >> Facility #1 >> Area A  My HVAC Units >> Facility #1   \n",
-                            "28  My HVAC Units >> Facility #1 >> Area A  My HVAC Units >> Facility #1   \n",
-                            "29  My HVAC Units >> Facility #1 >> Area A  My HVAC Units >> Facility #1   \n",
-                            "30  My HVAC Units >> Facility #1 >> Area I  My HVAC Units >> Facility #1   \n",
-                            "31  My HVAC Units >> Facility #1 >> Area I  My HVAC Units >> Facility #1   \n",
-                            "32  My HVAC Units >> Facility #1 >> Area I  My HVAC Units >> Facility #1   \n",
+                            "9   My HVAC Units >> Facility #1 >> Area H  My HVAC Units >> Facility #1   \n",
+                            "10  My HVAC Units >> Facility #1 >> Area H  My HVAC Units >> Facility #1   \n",
+                            "11  My HVAC Units >> Facility #1 >> Area H  My HVAC Units >> Facility #1   \n",
+                            "12  My HVAC Units >> Facility #1 >> Area G  My HVAC Units >> Facility #1   \n",
+                            "13  My HVAC Units >> Facility #1 >> Area G  My HVAC Units >> Facility #1   \n",
+                            "14  My HVAC Units >> Facility #1 >> Area G  My HVAC Units >> Facility #1   \n",
+                            "15  My HVAC Units >> Facility #1 >> Area K  My HVAC Units >> Facility #1   \n",
+                            "16  My HVAC Units >> Facility #1 >> Area K  My HVAC Units >> Facility #1   \n",
+                            "17  My HVAC Units >> Facility #1 >> Area K  My HVAC Units >> Facility #1   \n",
+                            "18  My HVAC Units >> Facility #1 >> Area A  My HVAC Units >> Facility #1   \n",
+                            "19  My HVAC Units >> Facility #1 >> Area A  My HVAC Units >> Facility #1   \n",
+                            "20  My HVAC Units >> Facility #1 >> Area A  My HVAC Units >> Facility #1   \n",
+                            "21  My HVAC Units >> Facility #1 >> Area J  My HVAC Units >> Facility #1   \n",
+                            "22  My HVAC Units >> Facility #1 >> Area J  My HVAC Units >> Facility #1   \n",
+                            "23  My HVAC Units >> Facility #1 >> Area J  My HVAC Units >> Facility #1   \n",
+                            "24  My HVAC Units >> Facility #1 >> Area C  My HVAC Units >> Facility #1   \n",
+                            "25  My HVAC Units >> Facility #1 >> Area C  My HVAC Units >> Facility #1   \n",
+                            "26  My HVAC Units >> Facility #1 >> Area C  My HVAC Units >> Facility #1   \n",
+                            "27  My HVAC Units >> Facility #1 >> Area F  My HVAC Units >> Facility #1   \n",
+                            "28  My HVAC Units >> Facility #1 >> Area D  My HVAC Units >> Facility #1   \n",
+                            "29  My HVAC Units >> Facility #1 >> Area D  My HVAC Units >> Facility #1   \n",
+                            "30  My HVAC Units >> Facility #1 >> Area D  My HVAC Units >> Facility #1   \n",
+                            "31  My HVAC Units >> Facility #1 >> Area Z  My HVAC Units >> Facility #1   \n",
+                            "32  My HVAC Units >> Facility #1 >> Area Z  My HVAC Units >> Facility #1   \n",
+                            "33  My HVAC Units >> Facility #1 >> Area Z  My HVAC Units >> Facility #1   \n",
                             "\n",
                             "   Template Build Result  \n",
                             "0      HVAC      Success  \n",
                             "1      HVAC      Success  \n",
                             "2      HVAC      Success  \n",
                             "3      HVAC      Success  \n",
                             "4      HVAC      Success  \n",
@@ -1338,15 +1362,16 @@
                             "25     HVAC      Success  \n",
                             "26     HVAC      Success  \n",
                             "27     HVAC      Success  \n",
                             "28     HVAC      Success  \n",
                             "29     HVAC      Success  \n",
                             "30     HVAC      Success  \n",
                             "31     HVAC      Success  \n",
-                            "32     HVAC      Success  "
+                            "32     HVAC      Success  \n",
+                            "33     HVAC      Success  "
                         ]
                     },
                     "execution_count": 7,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -1378,15 +1403,15 @@
             "cell_type": "code",
             "execution_count": 8,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<div style=\"background-color: #EEFFEE;color:black;text-align: left;\">Pushed successfully to datasource <strong>Seeq Data Lab [Datasource ID: Seeq Data Lab]</strong> and scoped to workbook ID <strong>807F13D7-C424-4840-B88B-D46F417A4966</strong><br>Click the following link to see what you pushed in Seeq:<br><a href=\"http://localhost:34216/28420AC3-152B-47A0-ACB7-6B060C3338FD/workbook/807F13D7-C424-4840-B88B-D46F417A4966/worksheet/C8375B1E-7DE2-44A6-BE3F-CA24281D6B72\" target=\"_new\">http://localhost:34216/28420AC3-152B-47A0-ACB7-6B060C3338FD/workbook/807F13D7-C424-4840-B88B-D46F417A4966/worksheet/C8375B1E-7DE2-44A6-BE3F-CA24281D6B72</a></div>"
+                            "<div style=\"background-color: #EEFFEE;color:black; text-align: left;\">Pushed successfully to datasource <strong>Seeq Data Lab [Datasource ID: Seeq Data Lab]</strong> and scoped to workbook ID <strong>90C07295-7D30-4DA6-8B5E-4DE3C7EF425C</strong><br>Click the following link to see what you pushed in Seeq:<br><a href=\"http://localhost:34216/5F85F903-0ED4-42B1-8B9E-418718482532/workbook/90C07295-7D30-4DA6-8B5E-4DE3C7EF425C/worksheet/5B3A24A6-1ABF-4403-BD0B-28669B4A60BF\" target=\"_new\">http://localhost:34216/5F85F903-0ED4-42B1-8B9E-418718482532/workbook/90C07295-7D30-4DA6-8B5E-4DE3C7EF425C/worksheet/5B3A24A6-1ABF-4403-BD0B-28669B4A60BF</a></div>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -1408,1046 +1433,1213 @@
                             "        text-align: right;\n",
                             "    }\n",
                             "</style>\n",
                             "<table border=\"1\" class=\"dataframe\">\n",
                             "  <thead>\n",
                             "    <tr style=\"text-align: right;\">\n",
                             "      <th></th>\n",
-                            "      <th>ID</th>\n",
                             "      <th>Description</th>\n",
                             "      <th>Type</th>\n",
-                            "      <th>Value Unit Of Measure</th>\n",
                             "      <th>Datasource Name</th>\n",
                             "      <th>Archived</th>\n",
                             "      <th>Referenced Name</th>\n",
                             "      <th>Reference</th>\n",
                             "      <th>Name</th>\n",
                             "      <th>Asset</th>\n",
                             "      <th>Asset Object</th>\n",
                             "      <th>Path</th>\n",
-                            "      <th>Template</th>\n",
-                            "      <th>Build Result</th>\n",
+                            "      <th>...</th>\n",
                             "      <th>Formula Parameters</th>\n",
+                            "      <th>Cache Enabled</th>\n",
+                            "      <th>Referenced ID</th>\n",
+                            "      <th>Scoped To</th>\n",
                             "      <th>Datasource Class</th>\n",
                             "      <th>Datasource ID</th>\n",
                             "      <th>Data ID</th>\n",
+                            "      <th>ID</th>\n",
                             "      <th>Push Result</th>\n",
+                            "      <th>Value Unit Of Measure</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
-                            "      <th>0</th>\n",
-                            "      <td>303B9001-49FE-4966-8664-18DF734DAFB1</td>\n",
+                            "      <th>0.0</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>CalculatedSignal</td>\n",
-                            "      <td>%</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
-                            "      <td>Area B_Relative Humidity</td>\n",
+                            "      <td>Area I_Relative Humidity</td>\n",
                             "      <td>True</td>\n",
                             "      <td>Relative Humidity</td>\n",
-                            "      <td>Area B</td>\n",
-                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area B</td>\n",
+                            "      <td>Area I</td>\n",
+                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area I</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
-                            "      <td>HVAC</td>\n",
-                            "      <td>Success</td>\n",
-                            "      <td>signal=D9A3F0B6-09CA-425D-A737-55384D6D0CA1</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>[signal=76E93E65-B284-4722-8B34-9142B04F34AA]</td>\n",
+                            "      <td>False</td>\n",
+                            "      <td>76E93E65-B284-4722-8B34-9142B04F34AA</td>\n",
+                            "      <td>90C07295-7D30-4DA6-8B5E-4DE3C7EF425C</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[807F13D7-C424-4840-B88B-D46F417A4966] {Signal} My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area B &gt;&gt; Relative Humidity</td>\n",
+                            "      <td>[90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Signal} My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area I &gt;&gt; Relative Humidity</td>\n",
+                            "      <td>C4A6B122-63DE-464F-B451-A0B4F110CEEE</td>\n",
                             "      <td>Success</td>\n",
+                            "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>1</th>\n",
-                            "      <td>E22A6AC9-209E-45BC-92C4-A1E0598B44E4</td>\n",
+                            "      <th>1.0</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>CalculatedSignal</td>\n",
-                            "      <td>\u00b0F</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
-                            "      <td>Area B_Temperature</td>\n",
+                            "      <td>Area I_Temperature</td>\n",
                             "      <td>True</td>\n",
                             "      <td>Temperature</td>\n",
-                            "      <td>Area B</td>\n",
-                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area B</td>\n",
+                            "      <td>Area I</td>\n",
+                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area I</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
-                            "      <td>HVAC</td>\n",
-                            "      <td>Success</td>\n",
-                            "      <td>[signal=B967C513-DB58-41CA-814B-2650465466BB]</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>[signal=088D7186-54DB-402C-AFD7-528B4F426DB3]</td>\n",
+                            "      <td>False</td>\n",
+                            "      <td>088D7186-54DB-402C-AFD7-528B4F426DB3</td>\n",
+                            "      <td>90C07295-7D30-4DA6-8B5E-4DE3C7EF425C</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[807F13D7-C424-4840-B88B-D46F417A4966] {Signal} My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area B &gt;&gt; Temperature</td>\n",
+                            "      <td>[90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Signal} My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area I &gt;&gt; Temperature</td>\n",
+                            "      <td>C0F59A23-AB56-424F-A79D-5EAF81AF0237</td>\n",
                             "      <td>Success</td>\n",
+                            "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>2</th>\n",
-                            "      <td>B569FED0-2BA4-48FD-89AA-E2A46F796CAF</td>\n",
+                            "      <th>2.0</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>Asset</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>NaN</td>\n",
-                            "      <td>Area B</td>\n",
-                            "      <td>Area B</td>\n",
-                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area B</td>\n",
+                            "      <td>Area I</td>\n",
+                            "      <td>Area I</td>\n",
+                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area I</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
-                            "      <td>HVAC</td>\n",
-                            "      <td>Success</td>\n",
+                            "      <td>...</td>\n",
                             "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>90C07295-7D30-4DA6-8B5E-4DE3C7EF425C</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[807F13D7-C424-4840-B88B-D46F417A4966] {Asset} My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area B</td>\n",
+                            "      <td>[90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Asset} My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area I</td>\n",
+                            "      <td>89D81BE7-91EE-4A13-B33A-CF5069D6BFF3</td>\n",
                             "      <td>Success</td>\n",
+                            "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>3</th>\n",
-                            "      <td>9589D928-22E3-4D0A-8C2F-39C85266AFF9</td>\n",
+                            "      <th>3.0</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>CalculatedSignal</td>\n",
-                            "      <td>%</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
-                            "      <td>Area K_Relative Humidity</td>\n",
+                            "      <td>Area B_Relative Humidity</td>\n",
                             "      <td>True</td>\n",
                             "      <td>Relative Humidity</td>\n",
-                            "      <td>Area K</td>\n",
-                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area K</td>\n",
+                            "      <td>Area B</td>\n",
+                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area B</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
-                            "      <td>HVAC</td>\n",
-                            "      <td>Success</td>\n",
-                            "      <td>[signal=F6BADC7D-0D6D-43B6-9776-19199E07683C]</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>[signal=E1DA8119-AF56-452C-8FC9-9073E6070D15]</td>\n",
+                            "      <td>False</td>\n",
+                            "      <td>E1DA8119-AF56-452C-8FC9-9073E6070D15</td>\n",
+                            "      <td>90C07295-7D30-4DA6-8B5E-4DE3C7EF425C</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[807F13D7-C424-4840-B88B-D46F417A4966] {Signal} My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area K &gt;&gt; Relative Humidity</td>\n",
+                            "      <td>[90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Signal} My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area B &gt;&gt; Relative Humidity</td>\n",
+                            "      <td>5AE6F6CE-3674-4AF6-8E8C-826DC8A7AF8D</td>\n",
                             "      <td>Success</td>\n",
+                            "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>4</th>\n",
-                            "      <td>43E50A16-ECA4-47F8-B98A-E110B69FBFB2</td>\n",
+                            "      <th>4.0</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>CalculatedSignal</td>\n",
-                            "      <td>\u00b0F</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
-                            "      <td>Area K_Temperature</td>\n",
+                            "      <td>Area B_Temperature</td>\n",
                             "      <td>True</td>\n",
                             "      <td>Temperature</td>\n",
-                            "      <td>Area K</td>\n",
-                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area K</td>\n",
+                            "      <td>Area B</td>\n",
+                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area B</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
-                            "      <td>HVAC</td>\n",
-                            "      <td>Success</td>\n",
-                            "      <td>[signal=64B266EF-2B11-4721-9E5E-A071462BC15A]</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>[signal=735C9627-F777-46C4-BAF5-B5B74F4534CF]</td>\n",
+                            "      <td>False</td>\n",
+                            "      <td>735C9627-F777-46C4-BAF5-B5B74F4534CF</td>\n",
+                            "      <td>90C07295-7D30-4DA6-8B5E-4DE3C7EF425C</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[807F13D7-C424-4840-B88B-D46F417A4966] {Signal} My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area K &gt;&gt; Temperature</td>\n",
+                            "      <td>[90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Signal} My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area B &gt;&gt; Temperature</td>\n",
+                            "      <td>39729CFC-7F4E-406B-A285-D07C2B63EB06</td>\n",
                             "      <td>Success</td>\n",
+                            "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>5</th>\n",
-                            "      <td>05368AE5-7A86-4B5B-BEAB-864C2B228E46</td>\n",
+                            "      <th>5.0</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>Asset</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>NaN</td>\n",
-                            "      <td>Area K</td>\n",
-                            "      <td>Area K</td>\n",
-                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area K</td>\n",
+                            "      <td>Area B</td>\n",
+                            "      <td>Area B</td>\n",
+                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area B</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
-                            "      <td>HVAC</td>\n",
-                            "      <td>Success</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
+                            "      <td>90C07295-7D30-4DA6-8B5E-4DE3C7EF425C</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[807F13D7-C424-4840-B88B-D46F417A4966] {Asset} My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area K</td>\n",
+                            "      <td>[90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Asset} My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area B</td>\n",
+                            "      <td>3F85E841-030E-483E-95FC-99A3CE6C003F</td>\n",
                             "      <td>Success</td>\n",
+                            "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>6</th>\n",
-                            "      <td>65D2AD84-EAFB-4152-82D3-F6F2C51BD38F</td>\n",
+                            "      <th>6.0</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>CalculatedSignal</td>\n",
-                            "      <td>%</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
                             "      <td>Area E_Relative Humidity</td>\n",
                             "      <td>True</td>\n",
                             "      <td>Relative Humidity</td>\n",
                             "      <td>Area E</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area E</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
-                            "      <td>HVAC</td>\n",
-                            "      <td>Success</td>\n",
-                            "      <td>[signal=52A57D13-5EBC-4E05-970B-5EF06CABC1BF]</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>[signal=32E43B48-174B-4291-AED3-862C23681BB8]</td>\n",
+                            "      <td>False</td>\n",
+                            "      <td>32E43B48-174B-4291-AED3-862C23681BB8</td>\n",
+                            "      <td>90C07295-7D30-4DA6-8B5E-4DE3C7EF425C</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[807F13D7-C424-4840-B88B-D46F417A4966] {Signal} My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area E &gt;&gt; Relative Humidity</td>\n",
+                            "      <td>[90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Signal} My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area E &gt;&gt; Relative Humidity</td>\n",
+                            "      <td>CC7DC3A2-A8A7-46C2-8C85-DE9A9E25F095</td>\n",
                             "      <td>Success</td>\n",
+                            "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>7</th>\n",
-                            "      <td>7205D9BE-5D1B-4428-B198-5D050EED14EB</td>\n",
+                            "      <th>7.0</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>CalculatedSignal</td>\n",
-                            "      <td>\u00b0F</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
                             "      <td>Area E_Temperature</td>\n",
                             "      <td>True</td>\n",
                             "      <td>Temperature</td>\n",
                             "      <td>Area E</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area E</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
-                            "      <td>HVAC</td>\n",
-                            "      <td>Success</td>\n",
-                            "      <td>[signal=078E6690-63DD-443A-B1F1-535C45A74BB3]</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>[signal=2A1E3E78-8F08-4601-963F-D866FB1F3523]</td>\n",
+                            "      <td>False</td>\n",
+                            "      <td>2A1E3E78-8F08-4601-963F-D866FB1F3523</td>\n",
+                            "      <td>90C07295-7D30-4DA6-8B5E-4DE3C7EF425C</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[807F13D7-C424-4840-B88B-D46F417A4966] {Signal} My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area E &gt;&gt; Temperature</td>\n",
+                            "      <td>[90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Signal} My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area E &gt;&gt; Temperature</td>\n",
+                            "      <td>0BA0119D-DA35-45D4-8BBC-E942736459F8</td>\n",
                             "      <td>Success</td>\n",
+                            "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>8</th>\n",
-                            "      <td>9BD7779E-2FD2-4F02-81D7-3FF2664B12B7</td>\n",
+                            "      <th>8.0</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>Asset</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>NaN</td>\n",
                             "      <td>Area E</td>\n",
                             "      <td>Area E</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area E</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
-                            "      <td>HVAC</td>\n",
-                            "      <td>Success</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
+                            "      <td>90C07295-7D30-4DA6-8B5E-4DE3C7EF425C</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[807F13D7-C424-4840-B88B-D46F417A4966] {Asset} My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area E</td>\n",
+                            "      <td>[90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Asset} My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area E</td>\n",
+                            "      <td>66EFF478-FE68-477A-ADCF-E943EA4C7156</td>\n",
                             "      <td>Success</td>\n",
+                            "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>9</th>\n",
-                            "      <td>AB19A286-8606-4AE3-838A-E7A4CC5CA8D1</td>\n",
+                            "      <th>9.0</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>CalculatedSignal</td>\n",
-                            "      <td>%</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
-                            "      <td>Area G_Relative Humidity</td>\n",
+                            "      <td>Area H_Relative Humidity</td>\n",
                             "      <td>True</td>\n",
                             "      <td>Relative Humidity</td>\n",
-                            "      <td>Area G</td>\n",
-                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area G</td>\n",
+                            "      <td>Area H</td>\n",
+                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area H</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
-                            "      <td>HVAC</td>\n",
-                            "      <td>Success</td>\n",
-                            "      <td>[signal=965BD8D5-FEB1-4F81-B80A-6B5A4664A3E6]</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>[signal=70CF0317-E1F6-45FA-B399-87F59AC17186]</td>\n",
+                            "      <td>False</td>\n",
+                            "      <td>70CF0317-E1F6-45FA-B399-87F59AC17186</td>\n",
+                            "      <td>90C07295-7D30-4DA6-8B5E-4DE3C7EF425C</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[807F13D7-C424-4840-B88B-D46F417A4966] {Signal} My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area G &gt;&gt; Relative Humidity</td>\n",
+                            "      <td>[90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Signal} My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area H &gt;&gt; Relative Humidity</td>\n",
+                            "      <td>548D8810-2484-459E-99F7-AE8EAD9E2A9D</td>\n",
                             "      <td>Success</td>\n",
+                            "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>10</th>\n",
-                            "      <td>1158EC96-5312-4B09-9B56-5B39CB13FC5C</td>\n",
+                            "      <th>10.0</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>CalculatedSignal</td>\n",
-                            "      <td>\u00b0F</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
-                            "      <td>Area G_Temperature</td>\n",
+                            "      <td>Area H_Temperature</td>\n",
                             "      <td>True</td>\n",
                             "      <td>Temperature</td>\n",
-                            "      <td>Area G</td>\n",
-                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area G</td>\n",
+                            "      <td>Area H</td>\n",
+                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area H</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
-                            "      <td>HVAC</td>\n",
-                            "      <td>Success</td>\n",
-                            "      <td>[signal=1B544029-7380-4C07-833C-CB1F9BFA253C]</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>[signal=6098E00F-32C9-47BB-A579-AB8DBF66426E]</td>\n",
+                            "      <td>False</td>\n",
+                            "      <td>6098E00F-32C9-47BB-A579-AB8DBF66426E</td>\n",
+                            "      <td>90C07295-7D30-4DA6-8B5E-4DE3C7EF425C</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[807F13D7-C424-4840-B88B-D46F417A4966] {Signal} My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area G &gt;&gt; Temperature</td>\n",
+                            "      <td>[90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Signal} My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area H &gt;&gt; Temperature</td>\n",
+                            "      <td>B0E69AF3-0237-491E-BA8D-7377FB8CDB1D</td>\n",
                             "      <td>Success</td>\n",
+                            "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>11</th>\n",
-                            "      <td>7E5CEA03-24E5-4B85-BBDB-51472E12A823</td>\n",
+                            "      <th>11.0</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>Asset</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>NaN</td>\n",
-                            "      <td>Area G</td>\n",
-                            "      <td>Area G</td>\n",
-                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area G</td>\n",
+                            "      <td>Area H</td>\n",
+                            "      <td>Area H</td>\n",
+                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area H</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
-                            "      <td>HVAC</td>\n",
-                            "      <td>Success</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
+                            "      <td>90C07295-7D30-4DA6-8B5E-4DE3C7EF425C</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[807F13D7-C424-4840-B88B-D46F417A4966] {Asset} My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area G</td>\n",
+                            "      <td>[90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Asset} My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area H</td>\n",
+                            "      <td>B533171D-6B1E-472A-BC25-3FF98ADEB26D</td>\n",
                             "      <td>Success</td>\n",
+                            "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>12</th>\n",
-                            "      <td>7CCDEDE6-EAF6-40D9-B57D-BE003A0B335D</td>\n",
+                            "      <th>12.0</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>CalculatedSignal</td>\n",
-                            "      <td>%</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
-                            "      <td>Area J_Relative Humidity</td>\n",
+                            "      <td>Area G_Relative Humidity</td>\n",
                             "      <td>True</td>\n",
                             "      <td>Relative Humidity</td>\n",
-                            "      <td>Area J</td>\n",
-                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area J</td>\n",
+                            "      <td>Area G</td>\n",
+                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area G</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
-                            "      <td>HVAC</td>\n",
-                            "      <td>Success</td>\n",
-                            "      <td>[signal=AB9A0CE0-D209-4D80-85CD-100A815EB7EF]</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>[signal=EC3180D2-7552-48A7-9163-469E318FC620]</td>\n",
+                            "      <td>False</td>\n",
+                            "      <td>EC3180D2-7552-48A7-9163-469E318FC620</td>\n",
+                            "      <td>90C07295-7D30-4DA6-8B5E-4DE3C7EF425C</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[807F13D7-C424-4840-B88B-D46F417A4966] {Signal} My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area J &gt;&gt; Relative Humidity</td>\n",
+                            "      <td>[90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Signal} My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area G &gt;&gt; Relative Humidity</td>\n",
+                            "      <td>CBE485F9-74D8-42B4-81A6-A25DF2EF0F66</td>\n",
                             "      <td>Success</td>\n",
+                            "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>13</th>\n",
-                            "      <td>F0CABBAE-9F4E-484D-912D-A81303780117</td>\n",
+                            "      <th>13.0</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>CalculatedSignal</td>\n",
-                            "      <td>\u00b0F</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
-                            "      <td>Area J_Temperature</td>\n",
+                            "      <td>Area G_Temperature</td>\n",
                             "      <td>True</td>\n",
                             "      <td>Temperature</td>\n",
-                            "      <td>Area J</td>\n",
-                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area J</td>\n",
+                            "      <td>Area G</td>\n",
+                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area G</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
-                            "      <td>HVAC</td>\n",
-                            "      <td>Success</td>\n",
-                            "      <td>[signal=D4A33C9B-E675-4CDA-BB18-9DCDD638E250]</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>[signal=603691BF-0805-4312-B313-6B664CAA00AC]</td>\n",
+                            "      <td>False</td>\n",
+                            "      <td>603691BF-0805-4312-B313-6B664CAA00AC</td>\n",
+                            "      <td>90C07295-7D30-4DA6-8B5E-4DE3C7EF425C</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[807F13D7-C424-4840-B88B-D46F417A4966] {Signal} My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area J &gt;&gt; Temperature</td>\n",
+                            "      <td>[90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Signal} My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area G &gt;&gt; Temperature</td>\n",
+                            "      <td>C2F9F5D4-9E5F-4AB5-92E1-275D3CA83F5A</td>\n",
                             "      <td>Success</td>\n",
+                            "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>14</th>\n",
-                            "      <td>9430617C-C952-4187-80A7-0E07154531B0</td>\n",
+                            "      <th>14.0</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>Asset</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>NaN</td>\n",
-                            "      <td>Area J</td>\n",
-                            "      <td>Area J</td>\n",
-                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area J</td>\n",
+                            "      <td>Area G</td>\n",
+                            "      <td>Area G</td>\n",
+                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area G</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
-                            "      <td>HVAC</td>\n",
-                            "      <td>Success</td>\n",
+                            "      <td>...</td>\n",
                             "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>90C07295-7D30-4DA6-8B5E-4DE3C7EF425C</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[807F13D7-C424-4840-B88B-D46F417A4966] {Asset} My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area J</td>\n",
+                            "      <td>[90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Asset} My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area G</td>\n",
+                            "      <td>62146015-07CD-4B83-B4B8-45058DF10BF4</td>\n",
                             "      <td>Success</td>\n",
+                            "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>15</th>\n",
-                            "      <td>74F9F4BA-559A-43F0-8AD5-E6260608A11D</td>\n",
+                            "      <th>15.0</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>CalculatedSignal</td>\n",
-                            "      <td>%</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
-                            "      <td>Area C_Relative Humidity</td>\n",
+                            "      <td>Area K_Relative Humidity</td>\n",
                             "      <td>True</td>\n",
                             "      <td>Relative Humidity</td>\n",
-                            "      <td>Area C</td>\n",
-                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area C</td>\n",
+                            "      <td>Area K</td>\n",
+                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area K</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
-                            "      <td>HVAC</td>\n",
-                            "      <td>Success</td>\n",
-                            "      <td>[signal=5E7A4906-931D-490F-B9DE-DD12CAC1430E]</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>[signal=601D5764-86B4-4FAA-BFF8-102171C0895E]</td>\n",
+                            "      <td>False</td>\n",
+                            "      <td>601D5764-86B4-4FAA-BFF8-102171C0895E</td>\n",
+                            "      <td>90C07295-7D30-4DA6-8B5E-4DE3C7EF425C</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[807F13D7-C424-4840-B88B-D46F417A4966] {Signal} My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area C &gt;&gt; Relative Humidity</td>\n",
+                            "      <td>[90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Signal} My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area K &gt;&gt; Relative Humidity</td>\n",
+                            "      <td>F00DE667-540A-4B0A-95E8-E80F4336F5DF</td>\n",
                             "      <td>Success</td>\n",
+                            "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>16</th>\n",
-                            "      <td>945944D3-8F01-4D9D-9E9D-012D2B700D28</td>\n",
+                            "      <th>16.0</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>CalculatedSignal</td>\n",
-                            "      <td>\u00b0F</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
-                            "      <td>Area C_Temperature</td>\n",
+                            "      <td>Area K_Temperature</td>\n",
                             "      <td>True</td>\n",
                             "      <td>Temperature</td>\n",
-                            "      <td>Area C</td>\n",
-                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area C</td>\n",
+                            "      <td>Area K</td>\n",
+                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area K</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
-                            "      <td>HVAC</td>\n",
-                            "      <td>Success</td>\n",
-                            "      <td>[signal=46E29219-3339-4F50-8137-C9C23B16DEF9]</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>[signal=3D0C814D-1BBC-4931-B6F0-F5CF38D050FF]</td>\n",
+                            "      <td>False</td>\n",
+                            "      <td>3D0C814D-1BBC-4931-B6F0-F5CF38D050FF</td>\n",
+                            "      <td>90C07295-7D30-4DA6-8B5E-4DE3C7EF425C</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[807F13D7-C424-4840-B88B-D46F417A4966] {Signal} My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area C &gt;&gt; Temperature</td>\n",
+                            "      <td>[90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Signal} My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area K &gt;&gt; Temperature</td>\n",
+                            "      <td>C3AD4240-F004-431D-8FB4-1644CA61948E</td>\n",
                             "      <td>Success</td>\n",
+                            "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>17</th>\n",
-                            "      <td>6B002A0B-A54C-4BF5-AB3A-588BD0984323</td>\n",
+                            "      <th>17.0</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>Asset</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>NaN</td>\n",
-                            "      <td>Area C</td>\n",
-                            "      <td>Area C</td>\n",
-                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area C</td>\n",
+                            "      <td>Area K</td>\n",
+                            "      <td>Area K</td>\n",
+                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area K</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
-                            "      <td>HVAC</td>\n",
-                            "      <td>Success</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
+                            "      <td>90C07295-7D30-4DA6-8B5E-4DE3C7EF425C</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[807F13D7-C424-4840-B88B-D46F417A4966] {Asset} My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area C</td>\n",
+                            "      <td>[90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Asset} My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area K</td>\n",
+                            "      <td>AE84756A-31C0-449C-A889-7AAAA5274265</td>\n",
                             "      <td>Success</td>\n",
+                            "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>18</th>\n",
-                            "      <td>31801747-8FA8-4FE4-B7E8-BF2318909DDE</td>\n",
+                            "      <th>18.0</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>CalculatedSignal</td>\n",
-                            "      <td>%</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
-                            "      <td>Area D_Relative Humidity</td>\n",
+                            "      <td>Area A_Relative Humidity</td>\n",
                             "      <td>True</td>\n",
                             "      <td>Relative Humidity</td>\n",
-                            "      <td>Area D</td>\n",
-                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area D</td>\n",
+                            "      <td>Area A</td>\n",
+                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area A</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
-                            "      <td>HVAC</td>\n",
-                            "      <td>Success</td>\n",
-                            "      <td>[signal=AB3B81B0-8A65-4DDE-A650-DD3311900239]</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>[signal=E9744446-848A-4461-A730-29CD0C97A7DC]</td>\n",
+                            "      <td>False</td>\n",
+                            "      <td>E9744446-848A-4461-A730-29CD0C97A7DC</td>\n",
+                            "      <td>90C07295-7D30-4DA6-8B5E-4DE3C7EF425C</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[807F13D7-C424-4840-B88B-D46F417A4966] {Signal} My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area D &gt;&gt; Relative Humidity</td>\n",
+                            "      <td>[90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Signal} My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area A &gt;&gt; Relative Humidity</td>\n",
+                            "      <td>567FBFA7-7660-4D77-91AB-43C7BFC39A84</td>\n",
                             "      <td>Success</td>\n",
+                            "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>19</th>\n",
-                            "      <td>327DDA43-DD80-4D25-A00C-197E00B597EF</td>\n",
+                            "      <th>19.0</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>CalculatedSignal</td>\n",
-                            "      <td>\u00b0F</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
-                            "      <td>Area D_Temperature</td>\n",
+                            "      <td>Area A_Temperature</td>\n",
                             "      <td>True</td>\n",
                             "      <td>Temperature</td>\n",
-                            "      <td>Area D</td>\n",
-                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area D</td>\n",
+                            "      <td>Area A</td>\n",
+                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area A</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
-                            "      <td>HVAC</td>\n",
-                            "      <td>Success</td>\n",
-                            "      <td>[signal=06BD8E98-DA1B-4984-B19F-367AD09340A2]</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>[signal=F8B2EF0E-BAB2-441D-B031-6F920099D74A]</td>\n",
+                            "      <td>False</td>\n",
+                            "      <td>F8B2EF0E-BAB2-441D-B031-6F920099D74A</td>\n",
+                            "      <td>90C07295-7D30-4DA6-8B5E-4DE3C7EF425C</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[807F13D7-C424-4840-B88B-D46F417A4966] {Signal} My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area D &gt;&gt; Temperature</td>\n",
+                            "      <td>[90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Signal} My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area A &gt;&gt; Temperature</td>\n",
+                            "      <td>DF15F6B5-BD34-4D7F-8864-7F54EFC9398F</td>\n",
                             "      <td>Success</td>\n",
+                            "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>20</th>\n",
-                            "      <td>842B2A61-FD70-483A-8386-42F858B9CD02</td>\n",
+                            "      <th>20.0</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>Asset</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>NaN</td>\n",
-                            "      <td>Area D</td>\n",
-                            "      <td>Area D</td>\n",
-                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area D</td>\n",
+                            "      <td>Area A</td>\n",
+                            "      <td>Area A</td>\n",
+                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area A</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
-                            "      <td>HVAC</td>\n",
-                            "      <td>Success</td>\n",
+                            "      <td>...</td>\n",
                             "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>90C07295-7D30-4DA6-8B5E-4DE3C7EF425C</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[807F13D7-C424-4840-B88B-D46F417A4966] {Asset} My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area D</td>\n",
+                            "      <td>[90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Asset} My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area A</td>\n",
+                            "      <td>86153257-14D6-43EA-9F11-3C4FEF7380C4</td>\n",
                             "      <td>Success</td>\n",
+                            "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>21</th>\n",
-                            "      <td>9B1F826F-8387-4F88-A3FE-4F83EF14EBAE</td>\n",
+                            "      <th>21.0</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>CalculatedSignal</td>\n",
-                            "      <td>%</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
-                            "      <td>Area H_Relative Humidity</td>\n",
+                            "      <td>Area J_Relative Humidity</td>\n",
                             "      <td>True</td>\n",
                             "      <td>Relative Humidity</td>\n",
-                            "      <td>Area H</td>\n",
-                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area H</td>\n",
+                            "      <td>Area J</td>\n",
+                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area J</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
-                            "      <td>HVAC</td>\n",
-                            "      <td>Success</td>\n",
-                            "      <td>[signal=1E40325D-33DF-4C91-9B57-9CC12898BFC9]</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>[signal=07EFC44C-FE26-475E-BF65-BE0AC2F890D2]</td>\n",
+                            "      <td>False</td>\n",
+                            "      <td>07EFC44C-FE26-475E-BF65-BE0AC2F890D2</td>\n",
+                            "      <td>90C07295-7D30-4DA6-8B5E-4DE3C7EF425C</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[807F13D7-C424-4840-B88B-D46F417A4966] {Signal} My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area H &gt;&gt; Relative Humidity</td>\n",
+                            "      <td>[90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Signal} My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area J &gt;&gt; Relative Humidity</td>\n",
+                            "      <td>26E72644-95A7-47B3-AFCB-4E0501141280</td>\n",
                             "      <td>Success</td>\n",
+                            "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>22</th>\n",
-                            "      <td>D3AD66F9-21DA-4AEE-8D50-9BC55FDD2570</td>\n",
+                            "      <th>22.0</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>CalculatedSignal</td>\n",
-                            "      <td>\u00b0F</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
-                            "      <td>Area H_Temperature</td>\n",
+                            "      <td>Area J_Temperature</td>\n",
                             "      <td>True</td>\n",
                             "      <td>Temperature</td>\n",
-                            "      <td>Area H</td>\n",
-                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area H</td>\n",
+                            "      <td>Area J</td>\n",
+                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area J</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
-                            "      <td>HVAC</td>\n",
-                            "      <td>Success</td>\n",
-                            "      <td>[signal=30E7BF71-A103-4DEE-BFFB-D99F95477615]</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>[signal=74DF4A2A-C8AA-4B8D-9486-5F73E41B3283]</td>\n",
+                            "      <td>False</td>\n",
+                            "      <td>74DF4A2A-C8AA-4B8D-9486-5F73E41B3283</td>\n",
+                            "      <td>90C07295-7D30-4DA6-8B5E-4DE3C7EF425C</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[807F13D7-C424-4840-B88B-D46F417A4966] {Signal} My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area H &gt;&gt; Temperature</td>\n",
+                            "      <td>[90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Signal} My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area J &gt;&gt; Temperature</td>\n",
+                            "      <td>94A9B21E-D41D-474F-8B43-38BB00F1F52D</td>\n",
                             "      <td>Success</td>\n",
+                            "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>23</th>\n",
-                            "      <td>68DCEBDD-DF4D-4C59-99AA-FB752EBF2AA7</td>\n",
+                            "      <th>23.0</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>Asset</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>NaN</td>\n",
-                            "      <td>Area H</td>\n",
-                            "      <td>Area H</td>\n",
-                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area H</td>\n",
+                            "      <td>Area J</td>\n",
+                            "      <td>Area J</td>\n",
+                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area J</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
-                            "      <td>HVAC</td>\n",
-                            "      <td>Success</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>90C07295-7D30-4DA6-8B5E-4DE3C7EF425C</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[807F13D7-C424-4840-B88B-D46F417A4966] {Asset} My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area H</td>\n",
+                            "      <td>[90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Asset} My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area J</td>\n",
+                            "      <td>766054C8-F386-4A3A-A8E2-7D474AF5A663</td>\n",
                             "      <td>Success</td>\n",
+                            "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>24</th>\n",
-                            "      <td>3CA298F2-9B90-4173-916D-081E10A475F2</td>\n",
+                            "      <th>24.0</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>CalculatedSignal</td>\n",
-                            "      <td>%</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
-                            "      <td>Area Z_Relative Humidity</td>\n",
+                            "      <td>Area C_Relative Humidity</td>\n",
                             "      <td>True</td>\n",
                             "      <td>Relative Humidity</td>\n",
-                            "      <td>Area Z</td>\n",
-                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area Z</td>\n",
+                            "      <td>Area C</td>\n",
+                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area C</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
-                            "      <td>HVAC</td>\n",
-                            "      <td>Success</td>\n",
-                            "      <td>[signal=E79E3573-86CA-4B47-9249-FD6E486309DF]</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>[signal=FBD71574-5153-479D-BBF2-CDA5C21C0888]</td>\n",
+                            "      <td>False</td>\n",
+                            "      <td>FBD71574-5153-479D-BBF2-CDA5C21C0888</td>\n",
+                            "      <td>90C07295-7D30-4DA6-8B5E-4DE3C7EF425C</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[807F13D7-C424-4840-B88B-D46F417A4966] {Signal} My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area Z &gt;&gt; Relative Humidity</td>\n",
+                            "      <td>[90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Signal} My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area C &gt;&gt; Relative Humidity</td>\n",
+                            "      <td>E6289352-4654-4877-B326-6E58993EFF2C</td>\n",
                             "      <td>Success</td>\n",
+                            "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>25</th>\n",
-                            "      <td>88362B6C-2DEB-4BCB-A9F7-46549A9B9519</td>\n",
+                            "      <th>25.0</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>CalculatedSignal</td>\n",
-                            "      <td>\u00b0F</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
-                            "      <td>Area Z_Temperature</td>\n",
+                            "      <td>Area C_Temperature</td>\n",
                             "      <td>True</td>\n",
                             "      <td>Temperature</td>\n",
-                            "      <td>Area Z</td>\n",
-                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area Z</td>\n",
+                            "      <td>Area C</td>\n",
+                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area C</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
-                            "      <td>HVAC</td>\n",
-                            "      <td>Success</td>\n",
-                            "      <td>[signal=C7790101-63F8-4567-8335-F60FB5E82F35]</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>[signal=BDD6B3E7-6A62-4C43-AC60-4F6EF8525134]</td>\n",
+                            "      <td>False</td>\n",
+                            "      <td>BDD6B3E7-6A62-4C43-AC60-4F6EF8525134</td>\n",
+                            "      <td>90C07295-7D30-4DA6-8B5E-4DE3C7EF425C</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[807F13D7-C424-4840-B88B-D46F417A4966] {Signal} My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area Z &gt;&gt; Temperature</td>\n",
+                            "      <td>[90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Signal} My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area C &gt;&gt; Temperature</td>\n",
+                            "      <td>3480C0A0-C9EE-467E-A4DE-947512EB0A71</td>\n",
                             "      <td>Success</td>\n",
+                            "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>26</th>\n",
-                            "      <td>34292ACB-515B-4448-AEF3-98F56493E805</td>\n",
+                            "      <th>26.0</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>Asset</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>NaN</td>\n",
-                            "      <td>Area Z</td>\n",
-                            "      <td>Area Z</td>\n",
-                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area Z</td>\n",
+                            "      <td>Area C</td>\n",
+                            "      <td>Area C</td>\n",
+                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area C</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
-                            "      <td>HVAC</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>90C07295-7D30-4DA6-8B5E-4DE3C7EF425C</td>\n",
+                            "      <td>Seeq Data Lab</td>\n",
+                            "      <td>Seeq Data Lab</td>\n",
+                            "      <td>[90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Asset} My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area C</td>\n",
+                            "      <td>B4275035-E78F-434E-835A-356076ACCA45</td>\n",
                             "      <td>Success</td>\n",
                             "      <td>NaN</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>27.0</th>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>Asset</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>Area F</td>\n",
+                            "      <td>Area F</td>\n",
+                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area F</td>\n",
+                            "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>90C07295-7D30-4DA6-8B5E-4DE3C7EF425C</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[807F13D7-C424-4840-B88B-D46F417A4966] {Asset} My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area Z</td>\n",
+                            "      <td>[90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Asset} My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area F</td>\n",
+                            "      <td>5C041D03-1011-48B3-B3A9-DF24574C81E8</td>\n",
                             "      <td>Success</td>\n",
+                            "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>27</th>\n",
-                            "      <td>1C654259-C2FC-4D7E-9A71-A76E0D994956</td>\n",
+                            "      <th>28.0</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>CalculatedSignal</td>\n",
-                            "      <td>%</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
-                            "      <td>Area A_Relative Humidity</td>\n",
+                            "      <td>Area D_Relative Humidity</td>\n",
                             "      <td>True</td>\n",
                             "      <td>Relative Humidity</td>\n",
-                            "      <td>Area A</td>\n",
-                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area A</td>\n",
+                            "      <td>Area D</td>\n",
+                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area D</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
-                            "      <td>HVAC</td>\n",
-                            "      <td>Success</td>\n",
-                            "      <td>[signal=44AF42F6-4041-422D-80DD-A27AA9E4A1C4]</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>[signal=13DE0DEB-DD2C-4E1A-800C-13DC45B2ADAF]</td>\n",
+                            "      <td>False</td>\n",
+                            "      <td>13DE0DEB-DD2C-4E1A-800C-13DC45B2ADAF</td>\n",
+                            "      <td>90C07295-7D30-4DA6-8B5E-4DE3C7EF425C</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[807F13D7-C424-4840-B88B-D46F417A4966] {Signal} My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area A &gt;&gt; Relative Humidity</td>\n",
+                            "      <td>[90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Signal} My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area D &gt;&gt; Relative Humidity</td>\n",
+                            "      <td>728D5358-289A-41D9-B44C-8E35A1F3A57E</td>\n",
                             "      <td>Success</td>\n",
+                            "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>28</th>\n",
-                            "      <td>3833B7D7-52B5-43F0-B16A-DA2C441D6D17</td>\n",
+                            "      <th>29.0</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>CalculatedSignal</td>\n",
-                            "      <td>\u00b0F</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
-                            "      <td>Area A_Temperature</td>\n",
+                            "      <td>Area D_Temperature</td>\n",
                             "      <td>True</td>\n",
                             "      <td>Temperature</td>\n",
-                            "      <td>Area A</td>\n",
-                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area A</td>\n",
+                            "      <td>Area D</td>\n",
+                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area D</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
-                            "      <td>HVAC</td>\n",
-                            "      <td>Success</td>\n",
-                            "      <td>[signal=C1F1002A-469E-47D1-83AB-99FD17650B55]</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>[signal=C90CB4E9-6CF7-4F13-BA6D-5078EA33ADAB]</td>\n",
+                            "      <td>False</td>\n",
+                            "      <td>C90CB4E9-6CF7-4F13-BA6D-5078EA33ADAB</td>\n",
+                            "      <td>90C07295-7D30-4DA6-8B5E-4DE3C7EF425C</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[807F13D7-C424-4840-B88B-D46F417A4966] {Signal} My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area A &gt;&gt; Temperature</td>\n",
+                            "      <td>[90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Signal} My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area D &gt;&gt; Temperature</td>\n",
+                            "      <td>49760019-5182-457C-A238-9CB001887A90</td>\n",
                             "      <td>Success</td>\n",
+                            "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>29</th>\n",
-                            "      <td>EE82A988-B462-4555-9827-6F6A09655400</td>\n",
+                            "      <th>30.0</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>Asset</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>NaN</td>\n",
-                            "      <td>Area A</td>\n",
-                            "      <td>Area A</td>\n",
-                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area A</td>\n",
+                            "      <td>Area D</td>\n",
+                            "      <td>Area D</td>\n",
+                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area D</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
-                            "      <td>HVAC</td>\n",
-                            "      <td>Success</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>90C07295-7D30-4DA6-8B5E-4DE3C7EF425C</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[807F13D7-C424-4840-B88B-D46F417A4966] {Asset} My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area A</td>\n",
+                            "      <td>[90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Asset} My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area D</td>\n",
+                            "      <td>F452E9EB-086E-4189-971A-7814C48B9B0B</td>\n",
                             "      <td>Success</td>\n",
+                            "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>30</th>\n",
-                            "      <td>6C0C1E9D-D719-4E61-96A9-9321D878BF34</td>\n",
+                            "      <th>31.0</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>CalculatedSignal</td>\n",
-                            "      <td>%</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
-                            "      <td>Area I_Relative Humidity</td>\n",
+                            "      <td>Area Z_Relative Humidity</td>\n",
                             "      <td>True</td>\n",
                             "      <td>Relative Humidity</td>\n",
-                            "      <td>Area I</td>\n",
-                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area I</td>\n",
+                            "      <td>Area Z</td>\n",
+                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area Z</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
-                            "      <td>HVAC</td>\n",
-                            "      <td>Success</td>\n",
-                            "      <td>[signal=A00EE0E0-2127-4CBD-A301-1DF629D7B7FC]</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>[signal=848594A9-469A-412D-8560-02A475ADA21F]</td>\n",
+                            "      <td>False</td>\n",
+                            "      <td>848594A9-469A-412D-8560-02A475ADA21F</td>\n",
+                            "      <td>90C07295-7D30-4DA6-8B5E-4DE3C7EF425C</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[807F13D7-C424-4840-B88B-D46F417A4966] {Signal} My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area I &gt;&gt; Relative Humidity</td>\n",
+                            "      <td>[90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Signal} My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area Z &gt;&gt; Relative Humidity</td>\n",
+                            "      <td>5A724793-8717-492E-9992-26A7617F3CA7</td>\n",
                             "      <td>Success</td>\n",
+                            "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>31</th>\n",
-                            "      <td>17CCBC30-5571-49D3-8364-D6A0D6E1171D</td>\n",
+                            "      <th>32.0</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>CalculatedSignal</td>\n",
-                            "      <td>\u00b0F</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
-                            "      <td>Area I_Temperature</td>\n",
+                            "      <td>Area Z_Temperature</td>\n",
                             "      <td>True</td>\n",
                             "      <td>Temperature</td>\n",
-                            "      <td>Area I</td>\n",
-                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area I</td>\n",
+                            "      <td>Area Z</td>\n",
+                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area Z</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
-                            "      <td>HVAC</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>[signal=6712F9DD-49D5-4448-B370-178EF20FC283]</td>\n",
+                            "      <td>False</td>\n",
+                            "      <td>6712F9DD-49D5-4448-B370-178EF20FC283</td>\n",
+                            "      <td>90C07295-7D30-4DA6-8B5E-4DE3C7EF425C</td>\n",
+                            "      <td>Seeq Data Lab</td>\n",
+                            "      <td>Seeq Data Lab</td>\n",
+                            "      <td>[90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Signal} My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area Z &gt;&gt; Temperature</td>\n",
+                            "      <td>17116A30-5DB7-434C-8E17-C564C884B629</td>\n",
                             "      <td>Success</td>\n",
-                            "      <td>[signal=2DE6799C-08A3-4434-9FC6-49969EE3DCBA]</td>\n",
+                            "      <td>NaN</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>33.0</th>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>Asset</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>Area Z</td>\n",
+                            "      <td>Area Z</td>\n",
+                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area Z</td>\n",
+                            "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>90C07295-7D30-4DA6-8B5E-4DE3C7EF425C</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[807F13D7-C424-4840-B88B-D46F417A4966] {Signal} My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area I &gt;&gt; Temperature</td>\n",
+                            "      <td>[90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Asset} My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area Z</td>\n",
+                            "      <td>0488E44B-D797-44E8-A8F3-3570F629FCD1</td>\n",
                             "      <td>Success</td>\n",
+                            "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>32</th>\n",
-                            "      <td>31E5CF1E-476A-4833-BFD8-D7E867E1DFB2</td>\n",
+                            "      <th>NaN</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>Asset</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
+                            "      <td>My HVAC Units</td>\n",
+                            "      <td>My HVAC Units</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>Area I</td>\n",
-                            "      <td>Area I</td>\n",
-                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area I</td>\n",
-                            "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
-                            "      <td>HVAC</td>\n",
+                            "      <td></td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>Seeq Data Lab</td>\n",
+                            "      <td>Seeq Data Lab</td>\n",
+                            "      <td>[90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Asset} My HVAC Units</td>\n",
+                            "      <td>F567A348-1877-4AAC-B6BB-A0B5A8184E6C</td>\n",
                             "      <td>Success</td>\n",
                             "      <td>NaN</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>NaN</th>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>Asset</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>Facility #1</td>\n",
+                            "      <td>Facility #1</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>My HVAC Units</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[807F13D7-C424-4840-B88B-D46F417A4966] {Asset} My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area I</td>\n",
+                            "      <td>[90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Asset} My HVAC Units &gt;&gt; Facility #1</td>\n",
+                            "      <td>8FE68DEB-AE5B-4A62-9D06-8B5BB426864C</td>\n",
                             "      <td>Success</td>\n",
+                            "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
+                            "<p>36 rows \u00d7 23 columns</p>\n",
                             "</div>"
                         ],
                         "text/plain": [
-                            "                                      ID Description              Type  \\\n",
-                            "0   303B9001-49FE-4966-8664-18DF734DAFB1         NaN  CalculatedSignal   \n",
-                            "1   E22A6AC9-209E-45BC-92C4-A1E0598B44E4         NaN  CalculatedSignal   \n",
-                            "2   B569FED0-2BA4-48FD-89AA-E2A46F796CAF         NaN             Asset   \n",
-                            "3   9589D928-22E3-4D0A-8C2F-39C85266AFF9         NaN  CalculatedSignal   \n",
-                            "4   43E50A16-ECA4-47F8-B98A-E110B69FBFB2         NaN  CalculatedSignal   \n",
-                            "5   05368AE5-7A86-4B5B-BEAB-864C2B228E46         NaN             Asset   \n",
-                            "6   65D2AD84-EAFB-4152-82D3-F6F2C51BD38F         NaN  CalculatedSignal   \n",
-                            "7   7205D9BE-5D1B-4428-B198-5D050EED14EB         NaN  CalculatedSignal   \n",
-                            "8   9BD7779E-2FD2-4F02-81D7-3FF2664B12B7         NaN             Asset   \n",
-                            "9   AB19A286-8606-4AE3-838A-E7A4CC5CA8D1         NaN  CalculatedSignal   \n",
-                            "10  1158EC96-5312-4B09-9B56-5B39CB13FC5C         NaN  CalculatedSignal   \n",
-                            "11  7E5CEA03-24E5-4B85-BBDB-51472E12A823         NaN             Asset   \n",
-                            "12  7CCDEDE6-EAF6-40D9-B57D-BE003A0B335D         NaN  CalculatedSignal   \n",
-                            "13  F0CABBAE-9F4E-484D-912D-A81303780117         NaN  CalculatedSignal   \n",
-                            "14  9430617C-C952-4187-80A7-0E07154531B0         NaN             Asset   \n",
-                            "15  74F9F4BA-559A-43F0-8AD5-E6260608A11D         NaN  CalculatedSignal   \n",
-                            "16  945944D3-8F01-4D9D-9E9D-012D2B700D28         NaN  CalculatedSignal   \n",
-                            "17  6B002A0B-A54C-4BF5-AB3A-588BD0984323         NaN             Asset   \n",
-                            "18  31801747-8FA8-4FE4-B7E8-BF2318909DDE         NaN  CalculatedSignal   \n",
-                            "19  327DDA43-DD80-4D25-A00C-197E00B597EF         NaN  CalculatedSignal   \n",
-                            "20  842B2A61-FD70-483A-8386-42F858B9CD02         NaN             Asset   \n",
-                            "21  9B1F826F-8387-4F88-A3FE-4F83EF14EBAE         NaN  CalculatedSignal   \n",
-                            "22  D3AD66F9-21DA-4AEE-8D50-9BC55FDD2570         NaN  CalculatedSignal   \n",
-                            "23  68DCEBDD-DF4D-4C59-99AA-FB752EBF2AA7         NaN             Asset   \n",
-                            "24  3CA298F2-9B90-4173-916D-081E10A475F2         NaN  CalculatedSignal   \n",
-                            "25  88362B6C-2DEB-4BCB-A9F7-46549A9B9519         NaN  CalculatedSignal   \n",
-                            "26  34292ACB-515B-4448-AEF3-98F56493E805         NaN             Asset   \n",
-                            "27  1C654259-C2FC-4D7E-9A71-A76E0D994956         NaN  CalculatedSignal   \n",
-                            "28  3833B7D7-52B5-43F0-B16A-DA2C441D6D17         NaN  CalculatedSignal   \n",
-                            "29  EE82A988-B462-4555-9827-6F6A09655400         NaN             Asset   \n",
-                            "30  6C0C1E9D-D719-4E61-96A9-9321D878BF34         NaN  CalculatedSignal   \n",
-                            "31  17CCBC30-5571-49D3-8364-D6A0D6E1171D         NaN  CalculatedSignal   \n",
-                            "32  31E5CF1E-476A-4833-BFD8-D7E867E1DFB2         NaN             Asset   \n",
+                            "      Description              Type Datasource Name Archived  \\\n",
+                            "0.0           NaN  CalculatedSignal    Example Data    False   \n",
+                            "1.0           NaN  CalculatedSignal    Example Data    False   \n",
+                            "2.0           NaN             Asset             NaN      NaN   \n",
+                            "3.0           NaN  CalculatedSignal    Example Data    False   \n",
+                            "4.0           NaN  CalculatedSignal    Example Data    False   \n",
+                            "5.0           NaN             Asset             NaN      NaN   \n",
+                            "6.0           NaN  CalculatedSignal    Example Data    False   \n",
+                            "7.0           NaN  CalculatedSignal    Example Data    False   \n",
+                            "8.0           NaN             Asset             NaN      NaN   \n",
+                            "9.0           NaN  CalculatedSignal    Example Data    False   \n",
+                            "10.0          NaN  CalculatedSignal    Example Data    False   \n",
+                            "11.0          NaN             Asset             NaN      NaN   \n",
+                            "12.0          NaN  CalculatedSignal    Example Data    False   \n",
+                            "13.0          NaN  CalculatedSignal    Example Data    False   \n",
+                            "14.0          NaN             Asset             NaN      NaN   \n",
+                            "15.0          NaN  CalculatedSignal    Example Data    False   \n",
+                            "16.0          NaN  CalculatedSignal    Example Data    False   \n",
+                            "17.0          NaN             Asset             NaN      NaN   \n",
+                            "18.0          NaN  CalculatedSignal    Example Data    False   \n",
+                            "19.0          NaN  CalculatedSignal    Example Data    False   \n",
+                            "20.0          NaN             Asset             NaN      NaN   \n",
+                            "21.0          NaN  CalculatedSignal    Example Data    False   \n",
+                            "22.0          NaN  CalculatedSignal    Example Data    False   \n",
+                            "23.0          NaN             Asset             NaN      NaN   \n",
+                            "24.0          NaN  CalculatedSignal    Example Data    False   \n",
+                            "25.0          NaN  CalculatedSignal    Example Data    False   \n",
+                            "26.0          NaN             Asset             NaN      NaN   \n",
+                            "27.0          NaN             Asset             NaN      NaN   \n",
+                            "28.0          NaN  CalculatedSignal    Example Data    False   \n",
+                            "29.0          NaN  CalculatedSignal    Example Data    False   \n",
+                            "30.0          NaN             Asset             NaN      NaN   \n",
+                            "31.0          NaN  CalculatedSignal    Example Data    False   \n",
+                            "32.0          NaN  CalculatedSignal    Example Data    False   \n",
+                            "33.0          NaN             Asset             NaN      NaN   \n",
+                            "NaN           NaN             Asset             NaN      NaN   \n",
+                            "NaN           NaN             Asset             NaN      NaN   \n",
+                            "\n",
+                            "               Referenced Name Reference               Name          Asset  \\\n",
+                            "0.0   Area I_Relative Humidity      True  Relative Humidity         Area I   \n",
+                            "1.0         Area I_Temperature      True        Temperature         Area I   \n",
+                            "2.0                        NaN       NaN             Area I         Area I   \n",
+                            "3.0   Area B_Relative Humidity      True  Relative Humidity         Area B   \n",
+                            "4.0         Area B_Temperature      True        Temperature         Area B   \n",
+                            "5.0                        NaN       NaN             Area B         Area B   \n",
+                            "6.0   Area E_Relative Humidity      True  Relative Humidity         Area E   \n",
+                            "7.0         Area E_Temperature      True        Temperature         Area E   \n",
+                            "8.0                        NaN       NaN             Area E         Area E   \n",
+                            "9.0   Area H_Relative Humidity      True  Relative Humidity         Area H   \n",
+                            "10.0        Area H_Temperature      True        Temperature         Area H   \n",
+                            "11.0                       NaN       NaN             Area H         Area H   \n",
+                            "12.0  Area G_Relative Humidity      True  Relative Humidity         Area G   \n",
+                            "13.0        Area G_Temperature      True        Temperature         Area G   \n",
+                            "14.0                       NaN       NaN             Area G         Area G   \n",
+                            "15.0  Area K_Relative Humidity      True  Relative Humidity         Area K   \n",
+                            "16.0        Area K_Temperature      True        Temperature         Area K   \n",
+                            "17.0                       NaN       NaN             Area K         Area K   \n",
+                            "18.0  Area A_Relative Humidity      True  Relative Humidity         Area A   \n",
+                            "19.0        Area A_Temperature      True        Temperature         Area A   \n",
+                            "20.0                       NaN       NaN             Area A         Area A   \n",
+                            "21.0  Area J_Relative Humidity      True  Relative Humidity         Area J   \n",
+                            "22.0        Area J_Temperature      True        Temperature         Area J   \n",
+                            "23.0                       NaN       NaN             Area J         Area J   \n",
+                            "24.0  Area C_Relative Humidity      True  Relative Humidity         Area C   \n",
+                            "25.0        Area C_Temperature      True        Temperature         Area C   \n",
+                            "26.0                       NaN       NaN             Area C         Area C   \n",
+                            "27.0                       NaN       NaN             Area F         Area F   \n",
+                            "28.0  Area D_Relative Humidity      True  Relative Humidity         Area D   \n",
+                            "29.0        Area D_Temperature      True        Temperature         Area D   \n",
+                            "30.0                       NaN       NaN             Area D         Area D   \n",
+                            "31.0  Area Z_Relative Humidity      True  Relative Humidity         Area Z   \n",
+                            "32.0        Area Z_Temperature      True        Temperature         Area Z   \n",
+                            "33.0                       NaN       NaN             Area Z         Area Z   \n",
+                            "NaN                        NaN       NaN      My HVAC Units  My HVAC Units   \n",
+                            "NaN                        NaN       NaN        Facility #1    Facility #1   \n",
+                            "\n",
+                            "                                Asset Object                          Path  \\\n",
+                            "0.0   My HVAC Units >> Facility #1 >> Area I  My HVAC Units >> Facility #1   \n",
+                            "1.0   My HVAC Units >> Facility #1 >> Area I  My HVAC Units >> Facility #1   \n",
+                            "2.0   My HVAC Units >> Facility #1 >> Area I  My HVAC Units >> Facility #1   \n",
+                            "3.0   My HVAC Units >> Facility #1 >> Area B  My HVAC Units >> Facility #1   \n",
+                            "4.0   My HVAC Units >> Facility #1 >> Area B  My HVAC Units >> Facility #1   \n",
+                            "5.0   My HVAC Units >> Facility #1 >> Area B  My HVAC Units >> Facility #1   \n",
+                            "6.0   My HVAC Units >> Facility #1 >> Area E  My HVAC Units >> Facility #1   \n",
+                            "7.0   My HVAC Units >> Facility #1 >> Area E  My HVAC Units >> Facility #1   \n",
+                            "8.0   My HVAC Units >> Facility #1 >> Area E  My HVAC Units >> Facility #1   \n",
+                            "9.0   My HVAC Units >> Facility #1 >> Area H  My HVAC Units >> Facility #1   \n",
+                            "10.0  My HVAC Units >> Facility #1 >> Area H  My HVAC Units >> Facility #1   \n",
+                            "11.0  My HVAC Units >> Facility #1 >> Area H  My HVAC Units >> Facility #1   \n",
+                            "12.0  My HVAC Units >> Facility #1 >> Area G  My HVAC Units >> Facility #1   \n",
+                            "13.0  My HVAC Units >> Facility #1 >> Area G  My HVAC Units >> Facility #1   \n",
+                            "14.0  My HVAC Units >> Facility #1 >> Area G  My HVAC Units >> Facility #1   \n",
+                            "15.0  My HVAC Units >> Facility #1 >> Area K  My HVAC Units >> Facility #1   \n",
+                            "16.0  My HVAC Units >> Facility #1 >> Area K  My HVAC Units >> Facility #1   \n",
+                            "17.0  My HVAC Units >> Facility #1 >> Area K  My HVAC Units >> Facility #1   \n",
+                            "18.0  My HVAC Units >> Facility #1 >> Area A  My HVAC Units >> Facility #1   \n",
+                            "19.0  My HVAC Units >> Facility #1 >> Area A  My HVAC Units >> Facility #1   \n",
+                            "20.0  My HVAC Units >> Facility #1 >> Area A  My HVAC Units >> Facility #1   \n",
+                            "21.0  My HVAC Units >> Facility #1 >> Area J  My HVAC Units >> Facility #1   \n",
+                            "22.0  My HVAC Units >> Facility #1 >> Area J  My HVAC Units >> Facility #1   \n",
+                            "23.0  My HVAC Units >> Facility #1 >> Area J  My HVAC Units >> Facility #1   \n",
+                            "24.0  My HVAC Units >> Facility #1 >> Area C  My HVAC Units >> Facility #1   \n",
+                            "25.0  My HVAC Units >> Facility #1 >> Area C  My HVAC Units >> Facility #1   \n",
+                            "26.0  My HVAC Units >> Facility #1 >> Area C  My HVAC Units >> Facility #1   \n",
+                            "27.0  My HVAC Units >> Facility #1 >> Area F  My HVAC Units >> Facility #1   \n",
+                            "28.0  My HVAC Units >> Facility #1 >> Area D  My HVAC Units >> Facility #1   \n",
+                            "29.0  My HVAC Units >> Facility #1 >> Area D  My HVAC Units >> Facility #1   \n",
+                            "30.0  My HVAC Units >> Facility #1 >> Area D  My HVAC Units >> Facility #1   \n",
+                            "31.0  My HVAC Units >> Facility #1 >> Area Z  My HVAC Units >> Facility #1   \n",
+                            "32.0  My HVAC Units >> Facility #1 >> Area Z  My HVAC Units >> Facility #1   \n",
+                            "33.0  My HVAC Units >> Facility #1 >> Area Z  My HVAC Units >> Facility #1   \n",
+                            "NaN                                      NaN                                 \n",
+                            "NaN                                      NaN                 My HVAC Units   \n",
+                            "\n",
+                            "      ...                             Formula Parameters Cache Enabled  \\\n",
+                            "0.0   ...  [signal=76E93E65-B284-4722-8B34-9142B04F34AA]         False   \n",
+                            "1.0   ...  [signal=088D7186-54DB-402C-AFD7-528B4F426DB3]         False   \n",
+                            "2.0   ...                                            NaN           NaN   \n",
+                            "3.0   ...  [signal=E1DA8119-AF56-452C-8FC9-9073E6070D15]         False   \n",
+                            "4.0   ...  [signal=735C9627-F777-46C4-BAF5-B5B74F4534CF]         False   \n",
+                            "5.0   ...                                            NaN           NaN   \n",
+                            "6.0   ...  [signal=32E43B48-174B-4291-AED3-862C23681BB8]         False   \n",
+                            "7.0   ...  [signal=2A1E3E78-8F08-4601-963F-D866FB1F3523]         False   \n",
+                            "8.0   ...                                            NaN           NaN   \n",
+                            "9.0   ...  [signal=70CF0317-E1F6-45FA-B399-87F59AC17186]         False   \n",
+                            "10.0  ...  [signal=6098E00F-32C9-47BB-A579-AB8DBF66426E]         False   \n",
+                            "11.0  ...                                            NaN           NaN   \n",
+                            "12.0  ...  [signal=EC3180D2-7552-48A7-9163-469E318FC620]         False   \n",
+                            "13.0  ...  [signal=603691BF-0805-4312-B313-6B664CAA00AC]         False   \n",
+                            "14.0  ...                                            NaN           NaN   \n",
+                            "15.0  ...  [signal=601D5764-86B4-4FAA-BFF8-102171C0895E]         False   \n",
+                            "16.0  ...  [signal=3D0C814D-1BBC-4931-B6F0-F5CF38D050FF]         False   \n",
+                            "17.0  ...                                            NaN           NaN   \n",
+                            "18.0  ...  [signal=E9744446-848A-4461-A730-29CD0C97A7DC]         False   \n",
+                            "19.0  ...  [signal=F8B2EF0E-BAB2-441D-B031-6F920099D74A]         False   \n",
+                            "20.0  ...                                            NaN           NaN   \n",
+                            "21.0  ...  [signal=07EFC44C-FE26-475E-BF65-BE0AC2F890D2]         False   \n",
+                            "22.0  ...  [signal=74DF4A2A-C8AA-4B8D-9486-5F73E41B3283]         False   \n",
+                            "23.0  ...                                            NaN           NaN   \n",
+                            "24.0  ...  [signal=FBD71574-5153-479D-BBF2-CDA5C21C0888]         False   \n",
+                            "25.0  ...  [signal=BDD6B3E7-6A62-4C43-AC60-4F6EF8525134]         False   \n",
+                            "26.0  ...                                            NaN           NaN   \n",
+                            "27.0  ...                                            NaN           NaN   \n",
+                            "28.0  ...  [signal=13DE0DEB-DD2C-4E1A-800C-13DC45B2ADAF]         False   \n",
+                            "29.0  ...  [signal=C90CB4E9-6CF7-4F13-BA6D-5078EA33ADAB]         False   \n",
+                            "30.0  ...                                            NaN           NaN   \n",
+                            "31.0  ...  [signal=848594A9-469A-412D-8560-02A475ADA21F]         False   \n",
+                            "32.0  ...  [signal=6712F9DD-49D5-4448-B370-178EF20FC283]         False   \n",
+                            "33.0  ...                                            NaN           NaN   \n",
+                            "NaN   ...                                            NaN           NaN   \n",
+                            "NaN   ...                                            NaN           NaN   \n",
+                            "\n",
+                            "                             Referenced ID  \\\n",
+                            "0.0   76E93E65-B284-4722-8B34-9142B04F34AA   \n",
+                            "1.0   088D7186-54DB-402C-AFD7-528B4F426DB3   \n",
+                            "2.0                                    NaN   \n",
+                            "3.0   E1DA8119-AF56-452C-8FC9-9073E6070D15   \n",
+                            "4.0   735C9627-F777-46C4-BAF5-B5B74F4534CF   \n",
+                            "5.0                                    NaN   \n",
+                            "6.0   32E43B48-174B-4291-AED3-862C23681BB8   \n",
+                            "7.0   2A1E3E78-8F08-4601-963F-D866FB1F3523   \n",
+                            "8.0                                    NaN   \n",
+                            "9.0   70CF0317-E1F6-45FA-B399-87F59AC17186   \n",
+                            "10.0  6098E00F-32C9-47BB-A579-AB8DBF66426E   \n",
+                            "11.0                                   NaN   \n",
+                            "12.0  EC3180D2-7552-48A7-9163-469E318FC620   \n",
+                            "13.0  603691BF-0805-4312-B313-6B664CAA00AC   \n",
+                            "14.0                                   NaN   \n",
+                            "15.0  601D5764-86B4-4FAA-BFF8-102171C0895E   \n",
+                            "16.0  3D0C814D-1BBC-4931-B6F0-F5CF38D050FF   \n",
+                            "17.0                                   NaN   \n",
+                            "18.0  E9744446-848A-4461-A730-29CD0C97A7DC   \n",
+                            "19.0  F8B2EF0E-BAB2-441D-B031-6F920099D74A   \n",
+                            "20.0                                   NaN   \n",
+                            "21.0  07EFC44C-FE26-475E-BF65-BE0AC2F890D2   \n",
+                            "22.0  74DF4A2A-C8AA-4B8D-9486-5F73E41B3283   \n",
+                            "23.0                                   NaN   \n",
+                            "24.0  FBD71574-5153-479D-BBF2-CDA5C21C0888   \n",
+                            "25.0  BDD6B3E7-6A62-4C43-AC60-4F6EF8525134   \n",
+                            "26.0                                   NaN   \n",
+                            "27.0                                   NaN   \n",
+                            "28.0  13DE0DEB-DD2C-4E1A-800C-13DC45B2ADAF   \n",
+                            "29.0  C90CB4E9-6CF7-4F13-BA6D-5078EA33ADAB   \n",
+                            "30.0                                   NaN   \n",
+                            "31.0  848594A9-469A-412D-8560-02A475ADA21F   \n",
+                            "32.0  6712F9DD-49D5-4448-B370-178EF20FC283   \n",
+                            "33.0                                   NaN   \n",
+                            "NaN                                    NaN   \n",
+                            "NaN                                    NaN   \n",
+                            "\n",
+                            "                                 Scoped To Datasource Class  Datasource ID  \\\n",
+                            "0.0   90C07295-7D30-4DA6-8B5E-4DE3C7EF425C    Seeq Data Lab  Seeq Data Lab   \n",
+                            "1.0   90C07295-7D30-4DA6-8B5E-4DE3C7EF425C    Seeq Data Lab  Seeq Data Lab   \n",
+                            "2.0   90C07295-7D30-4DA6-8B5E-4DE3C7EF425C    Seeq Data Lab  Seeq Data Lab   \n",
+                            "3.0   90C07295-7D30-4DA6-8B5E-4DE3C7EF425C    Seeq Data Lab  Seeq Data Lab   \n",
+                            "4.0   90C07295-7D30-4DA6-8B5E-4DE3C7EF425C    Seeq Data Lab  Seeq Data Lab   \n",
+                            "5.0   90C07295-7D30-4DA6-8B5E-4DE3C7EF425C    Seeq Data Lab  Seeq Data Lab   \n",
+                            "6.0   90C07295-7D30-4DA6-8B5E-4DE3C7EF425C    Seeq Data Lab  Seeq Data Lab   \n",
+                            "7.0   90C07295-7D30-4DA6-8B5E-4DE3C7EF425C    Seeq Data Lab  Seeq Data Lab   \n",
+                            "8.0   90C07295-7D30-4DA6-8B5E-4DE3C7EF425C    Seeq Data Lab  Seeq Data Lab   \n",
+                            "9.0   90C07295-7D30-4DA6-8B5E-4DE3C7EF425C    Seeq Data Lab  Seeq Data Lab   \n",
+                            "10.0  90C07295-7D30-4DA6-8B5E-4DE3C7EF425C    Seeq Data Lab  Seeq Data Lab   \n",
+                            "11.0  90C07295-7D30-4DA6-8B5E-4DE3C7EF425C    Seeq Data Lab  Seeq Data Lab   \n",
+                            "12.0  90C07295-7D30-4DA6-8B5E-4DE3C7EF425C    Seeq Data Lab  Seeq Data Lab   \n",
+                            "13.0  90C07295-7D30-4DA6-8B5E-4DE3C7EF425C    Seeq Data Lab  Seeq Data Lab   \n",
+                            "14.0  90C07295-7D30-4DA6-8B5E-4DE3C7EF425C    Seeq Data Lab  Seeq Data Lab   \n",
+                            "15.0  90C07295-7D30-4DA6-8B5E-4DE3C7EF425C    Seeq Data Lab  Seeq Data Lab   \n",
+                            "16.0  90C07295-7D30-4DA6-8B5E-4DE3C7EF425C    Seeq Data Lab  Seeq Data Lab   \n",
+                            "17.0  90C07295-7D30-4DA6-8B5E-4DE3C7EF425C    Seeq Data Lab  Seeq Data Lab   \n",
+                            "18.0  90C07295-7D30-4DA6-8B5E-4DE3C7EF425C    Seeq Data Lab  Seeq Data Lab   \n",
+                            "19.0  90C07295-7D30-4DA6-8B5E-4DE3C7EF425C    Seeq Data Lab  Seeq Data Lab   \n",
+                            "20.0  90C07295-7D30-4DA6-8B5E-4DE3C7EF425C    Seeq Data Lab  Seeq Data Lab   \n",
+                            "21.0  90C07295-7D30-4DA6-8B5E-4DE3C7EF425C    Seeq Data Lab  Seeq Data Lab   \n",
+                            "22.0  90C07295-7D30-4DA6-8B5E-4DE3C7EF425C    Seeq Data Lab  Seeq Data Lab   \n",
+                            "23.0  90C07295-7D30-4DA6-8B5E-4DE3C7EF425C    Seeq Data Lab  Seeq Data Lab   \n",
+                            "24.0  90C07295-7D30-4DA6-8B5E-4DE3C7EF425C    Seeq Data Lab  Seeq Data Lab   \n",
+                            "25.0  90C07295-7D30-4DA6-8B5E-4DE3C7EF425C    Seeq Data Lab  Seeq Data Lab   \n",
+                            "26.0  90C07295-7D30-4DA6-8B5E-4DE3C7EF425C    Seeq Data Lab  Seeq Data Lab   \n",
+                            "27.0  90C07295-7D30-4DA6-8B5E-4DE3C7EF425C    Seeq Data Lab  Seeq Data Lab   \n",
+                            "28.0  90C07295-7D30-4DA6-8B5E-4DE3C7EF425C    Seeq Data Lab  Seeq Data Lab   \n",
+                            "29.0  90C07295-7D30-4DA6-8B5E-4DE3C7EF425C    Seeq Data Lab  Seeq Data Lab   \n",
+                            "30.0  90C07295-7D30-4DA6-8B5E-4DE3C7EF425C    Seeq Data Lab  Seeq Data Lab   \n",
+                            "31.0  90C07295-7D30-4DA6-8B5E-4DE3C7EF425C    Seeq Data Lab  Seeq Data Lab   \n",
+                            "32.0  90C07295-7D30-4DA6-8B5E-4DE3C7EF425C    Seeq Data Lab  Seeq Data Lab   \n",
+                            "33.0  90C07295-7D30-4DA6-8B5E-4DE3C7EF425C    Seeq Data Lab  Seeq Data Lab   \n",
+                            "NaN                                    NaN    Seeq Data Lab  Seeq Data Lab   \n",
+                            "NaN                                    NaN    Seeq Data Lab  Seeq Data Lab   \n",
+                            "\n",
+                            "                                                                                                          Data ID  \\\n",
+                            "0.0   [90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Signal} My HVAC Units >> Facility #1 >> Area I >> Relative Humidity   \n",
+                            "1.0         [90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Signal} My HVAC Units >> Facility #1 >> Area I >> Temperature   \n",
+                            "2.0                         [90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Asset} My HVAC Units >> Facility #1 >> Area I   \n",
+                            "3.0   [90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Signal} My HVAC Units >> Facility #1 >> Area B >> Relative Humidity   \n",
+                            "4.0         [90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Signal} My HVAC Units >> Facility #1 >> Area B >> Temperature   \n",
+                            "5.0                         [90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Asset} My HVAC Units >> Facility #1 >> Area B   \n",
+                            "6.0   [90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Signal} My HVAC Units >> Facility #1 >> Area E >> Relative Humidity   \n",
+                            "7.0         [90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Signal} My HVAC Units >> Facility #1 >> Area E >> Temperature   \n",
+                            "8.0                         [90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Asset} My HVAC Units >> Facility #1 >> Area E   \n",
+                            "9.0   [90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Signal} My HVAC Units >> Facility #1 >> Area H >> Relative Humidity   \n",
+                            "10.0        [90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Signal} My HVAC Units >> Facility #1 >> Area H >> Temperature   \n",
+                            "11.0                        [90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Asset} My HVAC Units >> Facility #1 >> Area H   \n",
+                            "12.0  [90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Signal} My HVAC Units >> Facility #1 >> Area G >> Relative Humidity   \n",
+                            "13.0        [90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Signal} My HVAC Units >> Facility #1 >> Area G >> Temperature   \n",
+                            "14.0                        [90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Asset} My HVAC Units >> Facility #1 >> Area G   \n",
+                            "15.0  [90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Signal} My HVAC Units >> Facility #1 >> Area K >> Relative Humidity   \n",
+                            "16.0        [90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Signal} My HVAC Units >> Facility #1 >> Area K >> Temperature   \n",
+                            "17.0                        [90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Asset} My HVAC Units >> Facility #1 >> Area K   \n",
+                            "18.0  [90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Signal} My HVAC Units >> Facility #1 >> Area A >> Relative Humidity   \n",
+                            "19.0        [90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Signal} My HVAC Units >> Facility #1 >> Area A >> Temperature   \n",
+                            "20.0                        [90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Asset} My HVAC Units >> Facility #1 >> Area A   \n",
+                            "21.0  [90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Signal} My HVAC Units >> Facility #1 >> Area J >> Relative Humidity   \n",
+                            "22.0        [90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Signal} My HVAC Units >> Facility #1 >> Area J >> Temperature   \n",
+                            "23.0                        [90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Asset} My HVAC Units >> Facility #1 >> Area J   \n",
+                            "24.0  [90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Signal} My HVAC Units >> Facility #1 >> Area C >> Relative Humidity   \n",
+                            "25.0        [90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Signal} My HVAC Units >> Facility #1 >> Area C >> Temperature   \n",
+                            "26.0                        [90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Asset} My HVAC Units >> Facility #1 >> Area C   \n",
+                            "27.0                        [90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Asset} My HVAC Units >> Facility #1 >> Area F   \n",
+                            "28.0  [90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Signal} My HVAC Units >> Facility #1 >> Area D >> Relative Humidity   \n",
+                            "29.0        [90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Signal} My HVAC Units >> Facility #1 >> Area D >> Temperature   \n",
+                            "30.0                        [90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Asset} My HVAC Units >> Facility #1 >> Area D   \n",
+                            "31.0  [90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Signal} My HVAC Units >> Facility #1 >> Area Z >> Relative Humidity   \n",
+                            "32.0        [90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Signal} My HVAC Units >> Facility #1 >> Area Z >> Temperature   \n",
+                            "33.0                        [90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Asset} My HVAC Units >> Facility #1 >> Area Z   \n",
+                            "NaN                                                  [90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Asset} My HVAC Units   \n",
+                            "NaN                                   [90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Asset} My HVAC Units >> Facility #1   \n",
+                            "\n",
+                            "                                        ID Push Result Value Unit Of Measure  \n",
+                            "0.0   C4A6B122-63DE-464F-B451-A0B4F110CEEE     Success                   NaN  \n",
+                            "1.0   C0F59A23-AB56-424F-A79D-5EAF81AF0237     Success                   NaN  \n",
+                            "2.0   89D81BE7-91EE-4A13-B33A-CF5069D6BFF3     Success                   NaN  \n",
+                            "3.0   5AE6F6CE-3674-4AF6-8E8C-826DC8A7AF8D     Success                   NaN  \n",
+                            "4.0   39729CFC-7F4E-406B-A285-D07C2B63EB06     Success                   NaN  \n",
+                            "5.0   3F85E841-030E-483E-95FC-99A3CE6C003F     Success                   NaN  \n",
+                            "6.0   CC7DC3A2-A8A7-46C2-8C85-DE9A9E25F095     Success                   NaN  \n",
+                            "7.0   0BA0119D-DA35-45D4-8BBC-E942736459F8     Success                   NaN  \n",
+                            "8.0   66EFF478-FE68-477A-ADCF-E943EA4C7156     Success                   NaN  \n",
+                            "9.0   548D8810-2484-459E-99F7-AE8EAD9E2A9D     Success                   NaN  \n",
+                            "10.0  B0E69AF3-0237-491E-BA8D-7377FB8CDB1D     Success                   NaN  \n",
+                            "11.0  B533171D-6B1E-472A-BC25-3FF98ADEB26D     Success                   NaN  \n",
+                            "12.0  CBE485F9-74D8-42B4-81A6-A25DF2EF0F66     Success                   NaN  \n",
+                            "13.0  C2F9F5D4-9E5F-4AB5-92E1-275D3CA83F5A     Success                   NaN  \n",
+                            "14.0  62146015-07CD-4B83-B4B8-45058DF10BF4     Success                   NaN  \n",
+                            "15.0  F00DE667-540A-4B0A-95E8-E80F4336F5DF     Success                   NaN  \n",
+                            "16.0  C3AD4240-F004-431D-8FB4-1644CA61948E     Success                   NaN  \n",
+                            "17.0  AE84756A-31C0-449C-A889-7AAAA5274265     Success                   NaN  \n",
+                            "18.0  567FBFA7-7660-4D77-91AB-43C7BFC39A84     Success                   NaN  \n",
+                            "19.0  DF15F6B5-BD34-4D7F-8864-7F54EFC9398F     Success                   NaN  \n",
+                            "20.0  86153257-14D6-43EA-9F11-3C4FEF7380C4     Success                   NaN  \n",
+                            "21.0  26E72644-95A7-47B3-AFCB-4E0501141280     Success                   NaN  \n",
+                            "22.0  94A9B21E-D41D-474F-8B43-38BB00F1F52D     Success                   NaN  \n",
+                            "23.0  766054C8-F386-4A3A-A8E2-7D474AF5A663     Success                   NaN  \n",
+                            "24.0  E6289352-4654-4877-B326-6E58993EFF2C     Success                   NaN  \n",
+                            "25.0  3480C0A0-C9EE-467E-A4DE-947512EB0A71     Success                   NaN  \n",
+                            "26.0  B4275035-E78F-434E-835A-356076ACCA45     Success                   NaN  \n",
+                            "27.0  5C041D03-1011-48B3-B3A9-DF24574C81E8     Success                   NaN  \n",
+                            "28.0  728D5358-289A-41D9-B44C-8E35A1F3A57E     Success                   NaN  \n",
+                            "29.0  49760019-5182-457C-A238-9CB001887A90     Success                   NaN  \n",
+                            "30.0  F452E9EB-086E-4189-971A-7814C48B9B0B     Success                   NaN  \n",
+                            "31.0  5A724793-8717-492E-9992-26A7617F3CA7     Success                   NaN  \n",
+                            "32.0  17116A30-5DB7-434C-8E17-C564C884B629     Success                   NaN  \n",
+                            "33.0  0488E44B-D797-44E8-A8F3-3570F629FCD1     Success                   NaN  \n",
+                            "NaN   F567A348-1877-4AAC-B6BB-A0B5A8184E6C     Success                   NaN  \n",
+                            "NaN   8FE68DEB-AE5B-4A62-9D06-8B5BB426864C     Success                   NaN  \n",
                             "\n",
-                            "   Value Unit Of Measure Datasource Name Archived           Referenced Name  \\\n",
-                            "0                      %    Example Data    False  Area B_Relative Humidity   \n",
-                            "1                     \u00b0F    Example Data    False        Area B_Temperature   \n",
-                            "2                    NaN             NaN      NaN                       NaN   \n",
-                            "3                      %    Example Data    False  Area K_Relative Humidity   \n",
-                            "4                     \u00b0F    Example Data    False        Area K_Temperature   \n",
-                            "5                    NaN             NaN      NaN                       NaN   \n",
-                            "6                      %    Example Data    False  Area E_Relative Humidity   \n",
-                            "7                     \u00b0F    Example Data    False        Area E_Temperature   \n",
-                            "8                    NaN             NaN      NaN                       NaN   \n",
-                            "9                      %    Example Data    False  Area G_Relative Humidity   \n",
-                            "10                    \u00b0F    Example Data    False        Area G_Temperature   \n",
-                            "11                   NaN             NaN      NaN                       NaN   \n",
-                            "12                     %    Example Data    False  Area J_Relative Humidity   \n",
-                            "13                    \u00b0F    Example Data    False        Area J_Temperature   \n",
-                            "14                   NaN             NaN      NaN                       NaN   \n",
-                            "15                     %    Example Data    False  Area C_Relative Humidity   \n",
-                            "16                    \u00b0F    Example Data    False        Area C_Temperature   \n",
-                            "17                   NaN             NaN      NaN                       NaN   \n",
-                            "18                     %    Example Data    False  Area D_Relative Humidity   \n",
-                            "19                    \u00b0F    Example Data    False        Area D_Temperature   \n",
-                            "20                   NaN             NaN      NaN                       NaN   \n",
-                            "21                     %    Example Data    False  Area H_Relative Humidity   \n",
-                            "22                    \u00b0F    Example Data    False        Area H_Temperature   \n",
-                            "23                   NaN             NaN      NaN                       NaN   \n",
-                            "24                     %    Example Data    False  Area Z_Relative Humidity   \n",
-                            "25                    \u00b0F    Example Data    False        Area Z_Temperature   \n",
-                            "26                   NaN             NaN      NaN                       NaN   \n",
-                            "27                     %    Example Data    False  Area A_Relative Humidity   \n",
-                            "28                    \u00b0F    Example Data    False        Area A_Temperature   \n",
-                            "29                   NaN             NaN      NaN                       NaN   \n",
-                            "30                     %    Example Data    False  Area I_Relative Humidity   \n",
-                            "31                    \u00b0F    Example Data    False        Area I_Temperature   \n",
-                            "32                   NaN             NaN      NaN                       NaN   \n",
-                            "\n",
-                            "   Reference               Name   Asset  \\\n",
-                            "0       True  Relative Humidity  Area B   \n",
-                            "1       True        Temperature  Area B   \n",
-                            "2        NaN             Area B  Area B   \n",
-                            "3       True  Relative Humidity  Area K   \n",
-                            "4       True        Temperature  Area K   \n",
-                            "5        NaN             Area K  Area K   \n",
-                            "6       True  Relative Humidity  Area E   \n",
-                            "7       True        Temperature  Area E   \n",
-                            "8        NaN             Area E  Area E   \n",
-                            "9       True  Relative Humidity  Area G   \n",
-                            "10      True        Temperature  Area G   \n",
-                            "11       NaN             Area G  Area G   \n",
-                            "12      True  Relative Humidity  Area J   \n",
-                            "13      True        Temperature  Area J   \n",
-                            "14       NaN             Area J  Area J   \n",
-                            "15      True  Relative Humidity  Area C   \n",
-                            "16      True        Temperature  Area C   \n",
-                            "17       NaN             Area C  Area C   \n",
-                            "18      True  Relative Humidity  Area D   \n",
-                            "19      True        Temperature  Area D   \n",
-                            "20       NaN             Area D  Area D   \n",
-                            "21      True  Relative Humidity  Area H   \n",
-                            "22      True        Temperature  Area H   \n",
-                            "23       NaN             Area H  Area H   \n",
-                            "24      True  Relative Humidity  Area Z   \n",
-                            "25      True        Temperature  Area Z   \n",
-                            "26       NaN             Area Z  Area Z   \n",
-                            "27      True  Relative Humidity  Area A   \n",
-                            "28      True        Temperature  Area A   \n",
-                            "29       NaN             Area A  Area A   \n",
-                            "30      True  Relative Humidity  Area I   \n",
-                            "31      True        Temperature  Area I   \n",
-                            "32       NaN             Area I  Area I   \n",
-                            "\n",
-                            "                              Asset Object                          Path  \\\n",
-                            "0   My HVAC Units >> Facility #1 >> Area B  My HVAC Units >> Facility #1   \n",
-                            "1   My HVAC Units >> Facility #1 >> Area B  My HVAC Units >> Facility #1   \n",
-                            "2   My HVAC Units >> Facility #1 >> Area B  My HVAC Units >> Facility #1   \n",
-                            "3   My HVAC Units >> Facility #1 >> Area K  My HVAC Units >> Facility #1   \n",
-                            "4   My HVAC Units >> Facility #1 >> Area K  My HVAC Units >> Facility #1   \n",
-                            "5   My HVAC Units >> Facility #1 >> Area K  My HVAC Units >> Facility #1   \n",
-                            "6   My HVAC Units >> Facility #1 >> Area E  My HVAC Units >> Facility #1   \n",
-                            "7   My HVAC Units >> Facility #1 >> Area E  My HVAC Units >> Facility #1   \n",
-                            "8   My HVAC Units >> Facility #1 >> Area E  My HVAC Units >> Facility #1   \n",
-                            "9   My HVAC Units >> Facility #1 >> Area G  My HVAC Units >> Facility #1   \n",
-                            "10  My HVAC Units >> Facility #1 >> Area G  My HVAC Units >> Facility #1   \n",
-                            "11  My HVAC Units >> Facility #1 >> Area G  My HVAC Units >> Facility #1   \n",
-                            "12  My HVAC Units >> Facility #1 >> Area J  My HVAC Units >> Facility #1   \n",
-                            "13  My HVAC Units >> Facility #1 >> Area J  My HVAC Units >> Facility #1   \n",
-                            "14  My HVAC Units >> Facility #1 >> Area J  My HVAC Units >> Facility #1   \n",
-                            "15  My HVAC Units >> Facility #1 >> Area C  My HVAC Units >> Facility #1   \n",
-                            "16  My HVAC Units >> Facility #1 >> Area C  My HVAC Units >> Facility #1   \n",
-                            "17  My HVAC Units >> Facility #1 >> Area C  My HVAC Units >> Facility #1   \n",
-                            "18  My HVAC Units >> Facility #1 >> Area D  My HVAC Units >> Facility #1   \n",
-                            "19  My HVAC Units >> Facility #1 >> Area D  My HVAC Units >> Facility #1   \n",
-                            "20  My HVAC Units >> Facility #1 >> Area D  My HVAC Units >> Facility #1   \n",
-                            "21  My HVAC Units >> Facility #1 >> Area H  My HVAC Units >> Facility #1   \n",
-                            "22  My HVAC Units >> Facility #1 >> Area H  My HVAC Units >> Facility #1   \n",
-                            "23  My HVAC Units >> Facility #1 >> Area H  My HVAC Units >> Facility #1   \n",
-                            "24  My HVAC Units >> Facility #1 >> Area Z  My HVAC Units >> Facility #1   \n",
-                            "25  My HVAC Units >> Facility #1 >> Area Z  My HVAC Units >> Facility #1   \n",
-                            "26  My HVAC Units >> Facility #1 >> Area Z  My HVAC Units >> Facility #1   \n",
-                            "27  My HVAC Units >> Facility #1 >> Area A  My HVAC Units >> Facility #1   \n",
-                            "28  My HVAC Units >> Facility #1 >> Area A  My HVAC Units >> Facility #1   \n",
-                            "29  My HVAC Units >> Facility #1 >> Area A  My HVAC Units >> Facility #1   \n",
-                            "30  My HVAC Units >> Facility #1 >> Area I  My HVAC Units >> Facility #1   \n",
-                            "31  My HVAC Units >> Facility #1 >> Area I  My HVAC Units >> Facility #1   \n",
-                            "32  My HVAC Units >> Facility #1 >> Area I  My HVAC Units >> Facility #1   \n",
-                            "\n",
-                            "   Template Build Result                             Formula Parameters  \\\n",
-                            "0      HVAC      Success    signal=D9A3F0B6-09CA-425D-A737-55384D6D0CA1   \n",
-                            "1      HVAC      Success  [signal=B967C513-DB58-41CA-814B-2650465466BB]   \n",
-                            "2      HVAC      Success                                            NaN   \n",
-                            "3      HVAC      Success  [signal=F6BADC7D-0D6D-43B6-9776-19199E07683C]   \n",
-                            "4      HVAC      Success  [signal=64B266EF-2B11-4721-9E5E-A071462BC15A]   \n",
-                            "5      HVAC      Success                                            NaN   \n",
-                            "6      HVAC      Success  [signal=52A57D13-5EBC-4E05-970B-5EF06CABC1BF]   \n",
-                            "7      HVAC      Success  [signal=078E6690-63DD-443A-B1F1-535C45A74BB3]   \n",
-                            "8      HVAC      Success                                            NaN   \n",
-                            "9      HVAC      Success  [signal=965BD8D5-FEB1-4F81-B80A-6B5A4664A3E6]   \n",
-                            "10     HVAC      Success  [signal=1B544029-7380-4C07-833C-CB1F9BFA253C]   \n",
-                            "11     HVAC      Success                                            NaN   \n",
-                            "12     HVAC      Success  [signal=AB9A0CE0-D209-4D80-85CD-100A815EB7EF]   \n",
-                            "13     HVAC      Success  [signal=D4A33C9B-E675-4CDA-BB18-9DCDD638E250]   \n",
-                            "14     HVAC      Success                                            NaN   \n",
-                            "15     HVAC      Success  [signal=5E7A4906-931D-490F-B9DE-DD12CAC1430E]   \n",
-                            "16     HVAC      Success  [signal=46E29219-3339-4F50-8137-C9C23B16DEF9]   \n",
-                            "17     HVAC      Success                                            NaN   \n",
-                            "18     HVAC      Success  [signal=AB3B81B0-8A65-4DDE-A650-DD3311900239]   \n",
-                            "19     HVAC      Success  [signal=06BD8E98-DA1B-4984-B19F-367AD09340A2]   \n",
-                            "20     HVAC      Success                                            NaN   \n",
-                            "21     HVAC      Success  [signal=1E40325D-33DF-4C91-9B57-9CC12898BFC9]   \n",
-                            "22     HVAC      Success  [signal=30E7BF71-A103-4DEE-BFFB-D99F95477615]   \n",
-                            "23     HVAC      Success                                            NaN   \n",
-                            "24     HVAC      Success  [signal=E79E3573-86CA-4B47-9249-FD6E486309DF]   \n",
-                            "25     HVAC      Success  [signal=C7790101-63F8-4567-8335-F60FB5E82F35]   \n",
-                            "26     HVAC      Success                                            NaN   \n",
-                            "27     HVAC      Success  [signal=44AF42F6-4041-422D-80DD-A27AA9E4A1C4]   \n",
-                            "28     HVAC      Success  [signal=C1F1002A-469E-47D1-83AB-99FD17650B55]   \n",
-                            "29     HVAC      Success                                            NaN   \n",
-                            "30     HVAC      Success  [signal=A00EE0E0-2127-4CBD-A301-1DF629D7B7FC]   \n",
-                            "31     HVAC      Success  [signal=2DE6799C-08A3-4434-9FC6-49969EE3DCBA]   \n",
-                            "32     HVAC      Success                                            NaN   \n",
-                            "\n",
-                            "   Datasource Class  Datasource ID  \\\n",
-                            "0     Seeq Data Lab  Seeq Data Lab   \n",
-                            "1     Seeq Data Lab  Seeq Data Lab   \n",
-                            "2     Seeq Data Lab  Seeq Data Lab   \n",
-                            "3     Seeq Data Lab  Seeq Data Lab   \n",
-                            "4     Seeq Data Lab  Seeq Data Lab   \n",
-                            "5     Seeq Data Lab  Seeq Data Lab   \n",
-                            "6     Seeq Data Lab  Seeq Data Lab   \n",
-                            "7     Seeq Data Lab  Seeq Data Lab   \n",
-                            "8     Seeq Data Lab  Seeq Data Lab   \n",
-                            "9     Seeq Data Lab  Seeq Data Lab   \n",
-                            "10    Seeq Data Lab  Seeq Data Lab   \n",
-                            "11    Seeq Data Lab  Seeq Data Lab   \n",
-                            "12    Seeq Data Lab  Seeq Data Lab   \n",
-                            "13    Seeq Data Lab  Seeq Data Lab   \n",
-                            "14    Seeq Data Lab  Seeq Data Lab   \n",
-                            "15    Seeq Data Lab  Seeq Data Lab   \n",
-                            "16    Seeq Data Lab  Seeq Data Lab   \n",
-                            "17    Seeq Data Lab  Seeq Data Lab   \n",
-                            "18    Seeq Data Lab  Seeq Data Lab   \n",
-                            "19    Seeq Data Lab  Seeq Data Lab   \n",
-                            "20    Seeq Data Lab  Seeq Data Lab   \n",
-                            "21    Seeq Data Lab  Seeq Data Lab   \n",
-                            "22    Seeq Data Lab  Seeq Data Lab   \n",
-                            "23    Seeq Data Lab  Seeq Data Lab   \n",
-                            "24    Seeq Data Lab  Seeq Data Lab   \n",
-                            "25    Seeq Data Lab  Seeq Data Lab   \n",
-                            "26    Seeq Data Lab  Seeq Data Lab   \n",
-                            "27    Seeq Data Lab  Seeq Data Lab   \n",
-                            "28    Seeq Data Lab  Seeq Data Lab   \n",
-                            "29    Seeq Data Lab  Seeq Data Lab   \n",
-                            "30    Seeq Data Lab  Seeq Data Lab   \n",
-                            "31    Seeq Data Lab  Seeq Data Lab   \n",
-                            "32    Seeq Data Lab  Seeq Data Lab   \n",
-                            "\n",
-                            "                                                                                                        Data ID  \\\n",
-                            "0   [807F13D7-C424-4840-B88B-D46F417A4966] {Signal} My HVAC Units >> Facility #1 >> Area B >> Relative Humidity   \n",
-                            "1         [807F13D7-C424-4840-B88B-D46F417A4966] {Signal} My HVAC Units >> Facility #1 >> Area B >> Temperature   \n",
-                            "2                         [807F13D7-C424-4840-B88B-D46F417A4966] {Asset} My HVAC Units >> Facility #1 >> Area B   \n",
-                            "3   [807F13D7-C424-4840-B88B-D46F417A4966] {Signal} My HVAC Units >> Facility #1 >> Area K >> Relative Humidity   \n",
-                            "4         [807F13D7-C424-4840-B88B-D46F417A4966] {Signal} My HVAC Units >> Facility #1 >> Area K >> Temperature   \n",
-                            "5                         [807F13D7-C424-4840-B88B-D46F417A4966] {Asset} My HVAC Units >> Facility #1 >> Area K   \n",
-                            "6   [807F13D7-C424-4840-B88B-D46F417A4966] {Signal} My HVAC Units >> Facility #1 >> Area E >> Relative Humidity   \n",
-                            "7         [807F13D7-C424-4840-B88B-D46F417A4966] {Signal} My HVAC Units >> Facility #1 >> Area E >> Temperature   \n",
-                            "8                         [807F13D7-C424-4840-B88B-D46F417A4966] {Asset} My HVAC Units >> Facility #1 >> Area E   \n",
-                            "9   [807F13D7-C424-4840-B88B-D46F417A4966] {Signal} My HVAC Units >> Facility #1 >> Area G >> Relative Humidity   \n",
-                            "10        [807F13D7-C424-4840-B88B-D46F417A4966] {Signal} My HVAC Units >> Facility #1 >> Area G >> Temperature   \n",
-                            "11                        [807F13D7-C424-4840-B88B-D46F417A4966] {Asset} My HVAC Units >> Facility #1 >> Area G   \n",
-                            "12  [807F13D7-C424-4840-B88B-D46F417A4966] {Signal} My HVAC Units >> Facility #1 >> Area J >> Relative Humidity   \n",
-                            "13        [807F13D7-C424-4840-B88B-D46F417A4966] {Signal} My HVAC Units >> Facility #1 >> Area J >> Temperature   \n",
-                            "14                        [807F13D7-C424-4840-B88B-D46F417A4966] {Asset} My HVAC Units >> Facility #1 >> Area J   \n",
-                            "15  [807F13D7-C424-4840-B88B-D46F417A4966] {Signal} My HVAC Units >> Facility #1 >> Area C >> Relative Humidity   \n",
-                            "16        [807F13D7-C424-4840-B88B-D46F417A4966] {Signal} My HVAC Units >> Facility #1 >> Area C >> Temperature   \n",
-                            "17                        [807F13D7-C424-4840-B88B-D46F417A4966] {Asset} My HVAC Units >> Facility #1 >> Area C   \n",
-                            "18  [807F13D7-C424-4840-B88B-D46F417A4966] {Signal} My HVAC Units >> Facility #1 >> Area D >> Relative Humidity   \n",
-                            "19        [807F13D7-C424-4840-B88B-D46F417A4966] {Signal} My HVAC Units >> Facility #1 >> Area D >> Temperature   \n",
-                            "20                        [807F13D7-C424-4840-B88B-D46F417A4966] {Asset} My HVAC Units >> Facility #1 >> Area D   \n",
-                            "21  [807F13D7-C424-4840-B88B-D46F417A4966] {Signal} My HVAC Units >> Facility #1 >> Area H >> Relative Humidity   \n",
-                            "22        [807F13D7-C424-4840-B88B-D46F417A4966] {Signal} My HVAC Units >> Facility #1 >> Area H >> Temperature   \n",
-                            "23                        [807F13D7-C424-4840-B88B-D46F417A4966] {Asset} My HVAC Units >> Facility #1 >> Area H   \n",
-                            "24  [807F13D7-C424-4840-B88B-D46F417A4966] {Signal} My HVAC Units >> Facility #1 >> Area Z >> Relative Humidity   \n",
-                            "25        [807F13D7-C424-4840-B88B-D46F417A4966] {Signal} My HVAC Units >> Facility #1 >> Area Z >> Temperature   \n",
-                            "26                        [807F13D7-C424-4840-B88B-D46F417A4966] {Asset} My HVAC Units >> Facility #1 >> Area Z   \n",
-                            "27  [807F13D7-C424-4840-B88B-D46F417A4966] {Signal} My HVAC Units >> Facility #1 >> Area A >> Relative Humidity   \n",
-                            "28        [807F13D7-C424-4840-B88B-D46F417A4966] {Signal} My HVAC Units >> Facility #1 >> Area A >> Temperature   \n",
-                            "29                        [807F13D7-C424-4840-B88B-D46F417A4966] {Asset} My HVAC Units >> Facility #1 >> Area A   \n",
-                            "30  [807F13D7-C424-4840-B88B-D46F417A4966] {Signal} My HVAC Units >> Facility #1 >> Area I >> Relative Humidity   \n",
-                            "31        [807F13D7-C424-4840-B88B-D46F417A4966] {Signal} My HVAC Units >> Facility #1 >> Area I >> Temperature   \n",
-                            "32                        [807F13D7-C424-4840-B88B-D46F417A4966] {Asset} My HVAC Units >> Facility #1 >> Area I   \n",
-                            "\n",
-                            "   Push Result  \n",
-                            "0      Success  \n",
-                            "1      Success  \n",
-                            "2      Success  \n",
-                            "3      Success  \n",
-                            "4      Success  \n",
-                            "5      Success  \n",
-                            "6      Success  \n",
-                            "7      Success  \n",
-                            "8      Success  \n",
-                            "9      Success  \n",
-                            "10     Success  \n",
-                            "11     Success  \n",
-                            "12     Success  \n",
-                            "13     Success  \n",
-                            "14     Success  \n",
-                            "15     Success  \n",
-                            "16     Success  \n",
-                            "17     Success  \n",
-                            "18     Success  \n",
-                            "19     Success  \n",
-                            "20     Success  \n",
-                            "21     Success  \n",
-                            "22     Success  \n",
-                            "23     Success  \n",
-                            "24     Success  \n",
-                            "25     Success  \n",
-                            "26     Success  \n",
-                            "27     Success  \n",
-                            "28     Success  \n",
-                            "29     Success  \n",
-                            "30     Success  \n",
-                            "31     Success  \n",
-                            "32     Success  "
+                            "[36 rows x 23 columns]"
                         ]
                     },
                     "execution_count": 8,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -2525,15 +2717,15 @@
             "cell_type": "code",
             "execution_count": 10,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<div style=\"background-color: #EEFFEE;color:black;text-align: left;\">Pushed successfully to datasource <strong>Seeq Data Lab [Datasource ID: Seeq Data Lab]</strong> and scoped to workbook ID <strong>807F13D7-C424-4840-B88B-D46F417A4966</strong><br>Click the following link to see what you pushed in Seeq:<br><a href=\"http://localhost:34216/28420AC3-152B-47A0-ACB7-6B060C3338FD/workbook/807F13D7-C424-4840-B88B-D46F417A4966/worksheet/C8375B1E-7DE2-44A6-BE3F-CA24281D6B72\" target=\"_new\">http://localhost:34216/28420AC3-152B-47A0-ACB7-6B060C3338FD/workbook/807F13D7-C424-4840-B88B-D46F417A4966/worksheet/C8375B1E-7DE2-44A6-BE3F-CA24281D6B72</a></div>"
+                            "<div style=\"background-color: #EEFFEE;color:black; text-align: left;\">Pushed successfully to datasource <strong>Seeq Data Lab [Datasource ID: Seeq Data Lab]</strong> and scoped to workbook ID <strong>90C07295-7D30-4DA6-8B5E-4DE3C7EF425C</strong><br>Click the following link to see what you pushed in Seeq:<br><a href=\"http://localhost:34216/5F85F903-0ED4-42B1-8B9E-418718482532/workbook/90C07295-7D30-4DA6-8B5E-4DE3C7EF425C/worksheet/5B3A24A6-1ABF-4403-BD0B-28669B4A60BF\" target=\"_new\">http://localhost:34216/5F85F903-0ED4-42B1-8B9E-418718482532/workbook/90C07295-7D30-4DA6-8B5E-4DE3C7EF425C/worksheet/5B3A24A6-1ABF-4403-BD0B-28669B4A60BF</a></div>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -2565,141 +2757,147 @@
                             "      <th>Asset</th>\n",
                             "      <th>Asset Object</th>\n",
                             "      <th>Path</th>\n",
                             "      <th>Template</th>\n",
                             "      <th>Build Result</th>\n",
                             "      <th>ID</th>\n",
                             "      <th>Description</th>\n",
-                            "      <th>Value Unit Of Measure</th>\n",
-                            "      <th>Datasource Name</th>\n",
-                            "      <th>Archived</th>\n",
+                            "      <th>...</th>\n",
                             "      <th>Referenced Name</th>\n",
                             "      <th>Reference</th>\n",
                             "      <th>Formula Parameters</th>\n",
+                            "      <th>Scoped To</th>\n",
                             "      <th>Datasource Class</th>\n",
                             "      <th>Datasource ID</th>\n",
                             "      <th>Data ID</th>\n",
                             "      <th>Push Result</th>\n",
+                            "      <th>Cache Enabled</th>\n",
+                            "      <th>Referenced ID</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
-                            "      <th>0</th>\n",
+                            "      <th>0.0</th>\n",
                             "      <td>CalculatedScalar</td>\n",
                             "      <td>80F</td>\n",
                             "      <td>Hot Threshold</td>\n",
-                            "      <td>Area B</td>\n",
-                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area B</td>\n",
+                            "      <td>Area I</td>\n",
+                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area I</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
                             "      <td>HVAC With Calcs</td>\n",
                             "      <td>Success</td>\n",
-                            "      <td>73505133-BEAC-42FD-9FF1-C5962A60A9E7</td>\n",
-                            "      <td>NaN</td>\n",
-                            "      <td>NaN</td>\n",
-                            "      <td>NaN</td>\n",
-                            "      <td>NaN</td>\n",
+                            "      <td>625E9806-B59C-4C8C-857C-E958A66FFC1A</td>\n",
                             "      <td>NaN</td>\n",
+                            "      <td>...</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
+                            "      <td>[]</td>\n",
+                            "      <td>90C07295-7D30-4DA6-8B5E-4DE3C7EF425C</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[807F13D7-C424-4840-B88B-D46F417A4966] {Scalar...</td>\n",
+                            "      <td>[90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Scalar...</td>\n",
                             "      <td>Success</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>1</th>\n",
+                            "      <th>1.0</th>\n",
                             "      <td>CalculatedSignal</td>\n",
-                            "      <td>NaN</td>\n",
+                            "      <td>$signal.setUnits('%')</td>\n",
                             "      <td>Relative Humidity</td>\n",
-                            "      <td>Area B</td>\n",
-                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area B</td>\n",
+                            "      <td>Area I</td>\n",
+                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area I</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
                             "      <td>HVAC With Calcs</td>\n",
                             "      <td>Success</td>\n",
-                            "      <td>303B9001-49FE-4966-8664-18DF734DAFB1</td>\n",
+                            "      <td>C4A6B122-63DE-464F-B451-A0B4F110CEEE</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>%</td>\n",
-                            "      <td>Example Data</td>\n",
-                            "      <td>False</td>\n",
-                            "      <td>Area B_Relative Humidity</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>Area I_Relative Humidity</td>\n",
                             "      <td>True</td>\n",
-                            "      <td>[signal=D9A3F0B6-09CA-425D-A737-55384D6D0CA1]</td>\n",
+                            "      <td>[signal=76E93E65-B284-4722-8B34-9142B04F34AA]</td>\n",
+                            "      <td>90C07295-7D30-4DA6-8B5E-4DE3C7EF425C</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[807F13D7-C424-4840-B88B-D46F417A4966] {Signal...</td>\n",
+                            "      <td>[90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Signal...</td>\n",
                             "      <td>Success</td>\n",
+                            "      <td>False</td>\n",
+                            "      <td>76E93E65-B284-4722-8B34-9142B04F34AA</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>2</th>\n",
+                            "      <th>2.0</th>\n",
                             "      <td>CalculatedSignal</td>\n",
-                            "      <td>NaN</td>\n",
+                            "      <td>$signal.setUnits('\u00b0F')</td>\n",
                             "      <td>Temperature</td>\n",
-                            "      <td>Area B</td>\n",
-                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area B</td>\n",
+                            "      <td>Area I</td>\n",
+                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area I</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
                             "      <td>HVAC With Calcs</td>\n",
                             "      <td>Success</td>\n",
-                            "      <td>E22A6AC9-209E-45BC-92C4-A1E0598B44E4</td>\n",
+                            "      <td>C0F59A23-AB56-424F-A79D-5EAF81AF0237</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>\u00b0F</td>\n",
-                            "      <td>Example Data</td>\n",
-                            "      <td>False</td>\n",
-                            "      <td>Area B_Temperature</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>Area I_Temperature</td>\n",
                             "      <td>True</td>\n",
-                            "      <td>[signal=B967C513-DB58-41CA-814B-2650465466BB]</td>\n",
+                            "      <td>[signal=088D7186-54DB-402C-AFD7-528B4F426DB3]</td>\n",
+                            "      <td>90C07295-7D30-4DA6-8B5E-4DE3C7EF425C</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[807F13D7-C424-4840-B88B-D46F417A4966] {Signal...</td>\n",
+                            "      <td>[90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Signal...</td>\n",
                             "      <td>Success</td>\n",
+                            "      <td>False</td>\n",
+                            "      <td>088D7186-54DB-402C-AFD7-528B4F426DB3</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>3</th>\n",
+                            "      <th>3.0</th>\n",
                             "      <td>CalculatedSignal</td>\n",
                             "      <td>$temp.lowPassFilter(150min, 3min, 333).derivat...</td>\n",
                             "      <td>Temperature Rate Of Change</td>\n",
-                            "      <td>Area B</td>\n",
-                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area B</td>\n",
+                            "      <td>Area I</td>\n",
+                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area I</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
                             "      <td>HVAC With Calcs</td>\n",
                             "      <td>Success</td>\n",
-                            "      <td>E17F5569-66A6-4DD2-8421-BB2F4D58C68A</td>\n",
-                            "      <td>NaN</td>\n",
-                            "      <td>NaN</td>\n",
-                            "      <td>NaN</td>\n",
+                            "      <td>B3711DD3-E66A-408F-908F-74C66EA14C9C</td>\n",
                             "      <td>NaN</td>\n",
+                            "      <td>...</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>[temp=E22A6AC9-209E-45BC-92C4-A1E0598B44E4]</td>\n",
+                            "      <td>[temp=C0F59A23-AB56-424F-A79D-5EAF81AF0237]</td>\n",
+                            "      <td>90C07295-7D30-4DA6-8B5E-4DE3C7EF425C</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[807F13D7-C424-4840-B88B-D46F417A4966] {Signal...</td>\n",
+                            "      <td>[90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Signal...</td>\n",
                             "      <td>Success</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>4</th>\n",
+                            "      <th>4.0</th>\n",
                             "      <td>CalculatedCondition</td>\n",
                             "      <td>$temp.valueSearch(isGreaterThan($threshold))</td>\n",
                             "      <td>Too Hot</td>\n",
-                            "      <td>Area B</td>\n",
-                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area B</td>\n",
+                            "      <td>Area I</td>\n",
+                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area I</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
                             "      <td>HVAC With Calcs</td>\n",
                             "      <td>Success</td>\n",
-                            "      <td>396567FA-5476-4BF2-9F35-41E913FF9E2F</td>\n",
-                            "      <td>NaN</td>\n",
-                            "      <td>NaN</td>\n",
-                            "      <td>NaN</td>\n",
+                            "      <td>B789AEF8-E374-4822-8BC9-CC9C7FD975BE</td>\n",
                             "      <td>NaN</td>\n",
+                            "      <td>...</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>[temp=E22A6AC9-209E-45BC-92C4-A1E0598B44E4, th...</td>\n",
+                            "      <td>[temp=C0F59A23-AB56-424F-A79D-5EAF81AF0237, th...</td>\n",
+                            "      <td>90C07295-7D30-4DA6-8B5E-4DE3C7EF425C</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[807F13D7-C424-4840-B88B-D46F417A4966] {Condit...</td>\n",
+                            "      <td>[90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Condit...</td>\n",
                             "      <td>Success</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>...</th>\n",
                             "      <td>...</td>\n",
                             "      <td>...</td>\n",
                             "      <td>...</td>\n",
                             "      <td>...</td>\n",
@@ -2715,254 +2913,260 @@
                             "      <td>...</td>\n",
                             "      <td>...</td>\n",
                             "      <td>...</td>\n",
                             "      <td>...</td>\n",
                             "      <td>...</td>\n",
                             "      <td>...</td>\n",
                             "      <td>...</td>\n",
+                            "      <td>...</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>62</th>\n",
-                            "      <td>CalculatedSignal</td>\n",
-                            "      <td>NaN</td>\n",
-                            "      <td>Temperature</td>\n",
-                            "      <td>Area I</td>\n",
-                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area I</td>\n",
+                            "      <th>65.0</th>\n",
+                            "      <td>CalculatedCondition</td>\n",
+                            "      <td>$temp.valueSearch(isGreaterThan($threshold))</td>\n",
+                            "      <td>Too Hot</td>\n",
+                            "      <td>Area Z</td>\n",
+                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area Z</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
                             "      <td>HVAC With Calcs</td>\n",
                             "      <td>Success</td>\n",
-                            "      <td>17CCBC30-5571-49D3-8364-D6A0D6E1171D</td>\n",
+                            "      <td>8F1A572A-F689-4D84-9B76-17D85C287EDA</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>\u00b0F</td>\n",
-                            "      <td>Example Data</td>\n",
-                            "      <td>False</td>\n",
-                            "      <td>Area I_Temperature</td>\n",
-                            "      <td>True</td>\n",
-                            "      <td>[signal=2DE6799C-08A3-4434-9FC6-49969EE3DCBA]</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>[temp=17116A30-5DB7-434C-8E17-C564C884B629, th...</td>\n",
+                            "      <td>90C07295-7D30-4DA6-8B5E-4DE3C7EF425C</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[807F13D7-C424-4840-B88B-D46F417A4966] {Signal...</td>\n",
+                            "      <td>[90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Condit...</td>\n",
                             "      <td>Success</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>63</th>\n",
-                            "      <td>CalculatedSignal</td>\n",
-                            "      <td>$temp.lowPassFilter(150min, 3min, 333).derivat...</td>\n",
-                            "      <td>Temperature Rate Of Change</td>\n",
-                            "      <td>Area I</td>\n",
-                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area I</td>\n",
+                            "      <th>66.0</th>\n",
+                            "      <td>Asset</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>Area Z</td>\n",
+                            "      <td>Area Z</td>\n",
+                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area Z</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
                             "      <td>HVAC With Calcs</td>\n",
                             "      <td>Success</td>\n",
-                            "      <td>BA165F89-B98F-4FC9-9026-ABE528B79EA4</td>\n",
-                            "      <td>NaN</td>\n",
-                            "      <td>NaN</td>\n",
+                            "      <td>0488E44B-D797-44E8-A8F3-3570F629FCD1</td>\n",
                             "      <td>NaN</td>\n",
+                            "      <td>...</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>[temp=17CCBC30-5571-49D3-8364-D6A0D6E1171D]</td>\n",
+                            "      <td>90C07295-7D30-4DA6-8B5E-4DE3C7EF425C</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[807F13D7-C424-4840-B88B-D46F417A4966] {Signal...</td>\n",
+                            "      <td>[90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Asset}...</td>\n",
                             "      <td>Success</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>64</th>\n",
-                            "      <td>CalculatedCondition</td>\n",
-                            "      <td>$temp.valueSearch(isGreaterThan($threshold))</td>\n",
-                            "      <td>Too Hot</td>\n",
-                            "      <td>Area I</td>\n",
-                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area I</td>\n",
-                            "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
-                            "      <td>HVAC With Calcs</td>\n",
-                            "      <td>Success</td>\n",
-                            "      <td>E61118BE-1F07-4831-B1BF-6ED07C405D9D</td>\n",
+                            "      <th>NaN</th>\n",
+                            "      <td>Asset</td>\n",
                             "      <td>NaN</td>\n",
+                            "      <td>My HVAC Units</td>\n",
+                            "      <td>My HVAC Units</td>\n",
                             "      <td>NaN</td>\n",
+                            "      <td></td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>F567A348-1877-4AAC-B6BB-A0B5A8184E6C</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>...</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>[temp=17CCBC30-5571-49D3-8364-D6A0D6E1171D, th...</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[807F13D7-C424-4840-B88B-D46F417A4966] {Condit...</td>\n",
+                            "      <td>[90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Asset}...</td>\n",
                             "      <td>Success</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>65</th>\n",
+                            "      <th>NaN</th>\n",
                             "      <td>Asset</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>Area I</td>\n",
-                            "      <td>Area I</td>\n",
-                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area I</td>\n",
-                            "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
-                            "      <td>HVAC With Calcs</td>\n",
-                            "      <td>Success</td>\n",
-                            "      <td>31E5CF1E-476A-4833-BFD8-D7E867E1DFB2</td>\n",
+                            "      <td>Facility #1</td>\n",
+                            "      <td>Facility #1</td>\n",
                             "      <td>NaN</td>\n",
+                            "      <td>My HVAC Units</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
+                            "      <td>8FE68DEB-AE5B-4A62-9D06-8B5BB426864C</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>...</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[807F13D7-C424-4840-B88B-D46F417A4966] {Asset}...</td>\n",
+                            "      <td>[90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Asset}...</td>\n",
                             "      <td>Success</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>66</th>\n",
-                            "      <td>CalculatedScalar</td>\n",
-                            "      <td>80F</td>\n",
-                            "      <td>Hot Threshold</td>\n",
+                            "      <th>NaN</th>\n",
+                            "      <td>Asset</td>\n",
+                            "      <td>NaN</td>\n",
                             "      <td>Area F</td>\n",
-                            "      <td>My HVAC Units &gt;&gt; Facility #1 &gt;&gt; Area F</td>\n",
+                            "      <td>Area F</td>\n",
+                            "      <td>NaN</td>\n",
                             "      <td>My HVAC Units &gt;&gt; Facility #1</td>\n",
-                            "      <td>HVAC With Calcs</td>\n",
-                            "      <td>Success</td>\n",
-                            "      <td>A3486F32-A895-491E-BE10-9F8EC2F48726</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
+                            "      <td>5C041D03-1011-48B3-B3A9-DF24574C81E8</td>\n",
                             "      <td>NaN</td>\n",
+                            "      <td>...</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[807F13D7-C424-4840-B88B-D46F417A4966] {Scalar...</td>\n",
+                            "      <td>[90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Asset}...</td>\n",
                             "      <td>Success</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
-                            "<p>67 rows \u00d7 20 columns</p>\n",
+                            "<p>70 rows \u00d7 23 columns</p>\n",
                             "</div>"
                         ],
                         "text/plain": [
-                            "                   Type                                            Formula  \\\n",
-                            "0      CalculatedScalar                                                80F   \n",
-                            "1      CalculatedSignal                                                NaN   \n",
-                            "2      CalculatedSignal                                                NaN   \n",
-                            "3      CalculatedSignal  $temp.lowPassFilter(150min, 3min, 333).derivat...   \n",
-                            "4   CalculatedCondition       $temp.valueSearch(isGreaterThan($threshold))   \n",
-                            "..                  ...                                                ...   \n",
-                            "62     CalculatedSignal                                                NaN   \n",
-                            "63     CalculatedSignal  $temp.lowPassFilter(150min, 3min, 333).derivat...   \n",
-                            "64  CalculatedCondition       $temp.valueSearch(isGreaterThan($threshold))   \n",
-                            "65                Asset                                                NaN   \n",
-                            "66     CalculatedScalar                                                80F   \n",
-                            "\n",
-                            "                          Name   Asset  \\\n",
-                            "0                Hot Threshold  Area B   \n",
-                            "1            Relative Humidity  Area B   \n",
-                            "2                  Temperature  Area B   \n",
-                            "3   Temperature Rate Of Change  Area B   \n",
-                            "4                      Too Hot  Area B   \n",
-                            "..                         ...     ...   \n",
-                            "62                 Temperature  Area I   \n",
-                            "63  Temperature Rate Of Change  Area I   \n",
-                            "64                     Too Hot  Area I   \n",
-                            "65                      Area I  Area I   \n",
-                            "66               Hot Threshold  Area F   \n",
-                            "\n",
-                            "                              Asset Object                          Path  \\\n",
-                            "0   My HVAC Units >> Facility #1 >> Area B  My HVAC Units >> Facility #1   \n",
-                            "1   My HVAC Units >> Facility #1 >> Area B  My HVAC Units >> Facility #1   \n",
-                            "2   My HVAC Units >> Facility #1 >> Area B  My HVAC Units >> Facility #1   \n",
-                            "3   My HVAC Units >> Facility #1 >> Area B  My HVAC Units >> Facility #1   \n",
-                            "4   My HVAC Units >> Facility #1 >> Area B  My HVAC Units >> Facility #1   \n",
-                            "..                                     ...                           ...   \n",
-                            "62  My HVAC Units >> Facility #1 >> Area I  My HVAC Units >> Facility #1   \n",
-                            "63  My HVAC Units >> Facility #1 >> Area I  My HVAC Units >> Facility #1   \n",
-                            "64  My HVAC Units >> Facility #1 >> Area I  My HVAC Units >> Facility #1   \n",
-                            "65  My HVAC Units >> Facility #1 >> Area I  My HVAC Units >> Facility #1   \n",
-                            "66  My HVAC Units >> Facility #1 >> Area F  My HVAC Units >> Facility #1   \n",
-                            "\n",
-                            "           Template Build Result                                    ID  \\\n",
-                            "0   HVAC With Calcs      Success  73505133-BEAC-42FD-9FF1-C5962A60A9E7   \n",
-                            "1   HVAC With Calcs      Success  303B9001-49FE-4966-8664-18DF734DAFB1   \n",
-                            "2   HVAC With Calcs      Success  E22A6AC9-209E-45BC-92C4-A1E0598B44E4   \n",
-                            "3   HVAC With Calcs      Success  E17F5569-66A6-4DD2-8421-BB2F4D58C68A   \n",
-                            "4   HVAC With Calcs      Success  396567FA-5476-4BF2-9F35-41E913FF9E2F   \n",
-                            "..              ...          ...                                   ...   \n",
-                            "62  HVAC With Calcs      Success  17CCBC30-5571-49D3-8364-D6A0D6E1171D   \n",
-                            "63  HVAC With Calcs      Success  BA165F89-B98F-4FC9-9026-ABE528B79EA4   \n",
-                            "64  HVAC With Calcs      Success  E61118BE-1F07-4831-B1BF-6ED07C405D9D   \n",
-                            "65  HVAC With Calcs      Success  31E5CF1E-476A-4833-BFD8-D7E867E1DFB2   \n",
-                            "66  HVAC With Calcs      Success  A3486F32-A895-491E-BE10-9F8EC2F48726   \n",
-                            "\n",
-                            "   Description Value Unit Of Measure Datasource Name Archived  \\\n",
-                            "0          NaN                   NaN             NaN      NaN   \n",
-                            "1          NaN                     %    Example Data    False   \n",
-                            "2          NaN                    \u00b0F    Example Data    False   \n",
-                            "3          NaN                   NaN             NaN      NaN   \n",
-                            "4          NaN                   NaN             NaN      NaN   \n",
-                            "..         ...                   ...             ...      ...   \n",
-                            "62         NaN                    \u00b0F    Example Data    False   \n",
-                            "63         NaN                   NaN             NaN      NaN   \n",
-                            "64         NaN                   NaN             NaN      NaN   \n",
-                            "65         NaN                   NaN             NaN      NaN   \n",
-                            "66         NaN                   NaN             NaN      NaN   \n",
-                            "\n",
-                            "             Referenced Name Reference  \\\n",
-                            "0                        NaN       NaN   \n",
-                            "1   Area B_Relative Humidity      True   \n",
-                            "2         Area B_Temperature      True   \n",
-                            "3                        NaN       NaN   \n",
-                            "4                        NaN       NaN   \n",
-                            "..                       ...       ...   \n",
-                            "62        Area I_Temperature      True   \n",
-                            "63                       NaN       NaN   \n",
-                            "64                       NaN       NaN   \n",
-                            "65                       NaN       NaN   \n",
-                            "66                       NaN       NaN   \n",
-                            "\n",
-                            "                                   Formula Parameters Datasource Class  \\\n",
-                            "0                                                 NaN    Seeq Data Lab   \n",
-                            "1       [signal=D9A3F0B6-09CA-425D-A737-55384D6D0CA1]    Seeq Data Lab   \n",
-                            "2       [signal=B967C513-DB58-41CA-814B-2650465466BB]    Seeq Data Lab   \n",
-                            "3         [temp=E22A6AC9-209E-45BC-92C4-A1E0598B44E4]    Seeq Data Lab   \n",
-                            "4   [temp=E22A6AC9-209E-45BC-92C4-A1E0598B44E4, th...    Seeq Data Lab   \n",
-                            "..                                                ...              ...   \n",
-                            "62      [signal=2DE6799C-08A3-4434-9FC6-49969EE3DCBA]    Seeq Data Lab   \n",
-                            "63        [temp=17CCBC30-5571-49D3-8364-D6A0D6E1171D]    Seeq Data Lab   \n",
-                            "64  [temp=17CCBC30-5571-49D3-8364-D6A0D6E1171D, th...    Seeq Data Lab   \n",
-                            "65                                                NaN    Seeq Data Lab   \n",
-                            "66                                                NaN    Seeq Data Lab   \n",
-                            "\n",
-                            "    Datasource ID                                            Data ID  \\\n",
-                            "0   Seeq Data Lab  [807F13D7-C424-4840-B88B-D46F417A4966] {Scalar...   \n",
-                            "1   Seeq Data Lab  [807F13D7-C424-4840-B88B-D46F417A4966] {Signal...   \n",
-                            "2   Seeq Data Lab  [807F13D7-C424-4840-B88B-D46F417A4966] {Signal...   \n",
-                            "3   Seeq Data Lab  [807F13D7-C424-4840-B88B-D46F417A4966] {Signal...   \n",
-                            "4   Seeq Data Lab  [807F13D7-C424-4840-B88B-D46F417A4966] {Condit...   \n",
-                            "..            ...                                                ...   \n",
-                            "62  Seeq Data Lab  [807F13D7-C424-4840-B88B-D46F417A4966] {Signal...   \n",
-                            "63  Seeq Data Lab  [807F13D7-C424-4840-B88B-D46F417A4966] {Signal...   \n",
-                            "64  Seeq Data Lab  [807F13D7-C424-4840-B88B-D46F417A4966] {Condit...   \n",
-                            "65  Seeq Data Lab  [807F13D7-C424-4840-B88B-D46F417A4966] {Asset}...   \n",
-                            "66  Seeq Data Lab  [807F13D7-C424-4840-B88B-D46F417A4966] {Scalar...   \n",
-                            "\n",
-                            "   Push Result  \n",
-                            "0      Success  \n",
-                            "1      Success  \n",
-                            "2      Success  \n",
-                            "3      Success  \n",
-                            "4      Success  \n",
-                            "..         ...  \n",
-                            "62     Success  \n",
-                            "63     Success  \n",
-                            "64     Success  \n",
-                            "65     Success  \n",
-                            "66     Success  \n",
+                            "                     Type                                            Formula  \\\n",
+                            "0.0      CalculatedScalar                                                80F   \n",
+                            "1.0      CalculatedSignal                              $signal.setUnits('%')   \n",
+                            "2.0      CalculatedSignal                             $signal.setUnits('\u00b0F')   \n",
+                            "3.0      CalculatedSignal  $temp.lowPassFilter(150min, 3min, 333).derivat...   \n",
+                            "4.0   CalculatedCondition       $temp.valueSearch(isGreaterThan($threshold))   \n",
+                            "...                   ...                                                ...   \n",
+                            "65.0  CalculatedCondition       $temp.valueSearch(isGreaterThan($threshold))   \n",
+                            "66.0                Asset                                                NaN   \n",
+                            "NaN                 Asset                                                NaN   \n",
+                            "NaN                 Asset                                                NaN   \n",
+                            "NaN                 Asset                                                NaN   \n",
+                            "\n",
+                            "                            Name          Asset  \\\n",
+                            "0.0                Hot Threshold         Area I   \n",
+                            "1.0            Relative Humidity         Area I   \n",
+                            "2.0                  Temperature         Area I   \n",
+                            "3.0   Temperature Rate Of Change         Area I   \n",
+                            "4.0                      Too Hot         Area I   \n",
+                            "...                          ...            ...   \n",
+                            "65.0                     Too Hot         Area Z   \n",
+                            "66.0                      Area Z         Area Z   \n",
+                            "NaN                My HVAC Units  My HVAC Units   \n",
+                            "NaN                  Facility #1    Facility #1   \n",
+                            "NaN                       Area F         Area F   \n",
+                            "\n",
+                            "                                Asset Object                          Path  \\\n",
+                            "0.0   My HVAC Units >> Facility #1 >> Area I  My HVAC Units >> Facility #1   \n",
+                            "1.0   My HVAC Units >> Facility #1 >> Area I  My HVAC Units >> Facility #1   \n",
+                            "2.0   My HVAC Units >> Facility #1 >> Area I  My HVAC Units >> Facility #1   \n",
+                            "3.0   My HVAC Units >> Facility #1 >> Area I  My HVAC Units >> Facility #1   \n",
+                            "4.0   My HVAC Units >> Facility #1 >> Area I  My HVAC Units >> Facility #1   \n",
+                            "...                                      ...                           ...   \n",
+                            "65.0  My HVAC Units >> Facility #1 >> Area Z  My HVAC Units >> Facility #1   \n",
+                            "66.0  My HVAC Units >> Facility #1 >> Area Z  My HVAC Units >> Facility #1   \n",
+                            "NaN                                      NaN                                 \n",
+                            "NaN                                      NaN                 My HVAC Units   \n",
+                            "NaN                                      NaN  My HVAC Units >> Facility #1   \n",
+                            "\n",
+                            "             Template Build Result                                    ID  \\\n",
+                            "0.0   HVAC With Calcs      Success  625E9806-B59C-4C8C-857C-E958A66FFC1A   \n",
+                            "1.0   HVAC With Calcs      Success  C4A6B122-63DE-464F-B451-A0B4F110CEEE   \n",
+                            "2.0   HVAC With Calcs      Success  C0F59A23-AB56-424F-A79D-5EAF81AF0237   \n",
+                            "3.0   HVAC With Calcs      Success  B3711DD3-E66A-408F-908F-74C66EA14C9C   \n",
+                            "4.0   HVAC With Calcs      Success  B789AEF8-E374-4822-8BC9-CC9C7FD975BE   \n",
+                            "...               ...          ...                                   ...   \n",
+                            "65.0  HVAC With Calcs      Success  8F1A572A-F689-4D84-9B76-17D85C287EDA   \n",
+                            "66.0  HVAC With Calcs      Success  0488E44B-D797-44E8-A8F3-3570F629FCD1   \n",
+                            "NaN               NaN          NaN  F567A348-1877-4AAC-B6BB-A0B5A8184E6C   \n",
+                            "NaN               NaN          NaN  8FE68DEB-AE5B-4A62-9D06-8B5BB426864C   \n",
+                            "NaN               NaN          NaN  5C041D03-1011-48B3-B3A9-DF24574C81E8   \n",
+                            "\n",
+                            "      Description  ...           Referenced Name Reference  \\\n",
+                            "0.0           NaN  ...                       NaN       NaN   \n",
+                            "1.0           NaN  ...  Area I_Relative Humidity      True   \n",
+                            "2.0           NaN  ...        Area I_Temperature      True   \n",
+                            "3.0           NaN  ...                       NaN       NaN   \n",
+                            "4.0           NaN  ...                       NaN       NaN   \n",
+                            "...           ...  ...                       ...       ...   \n",
+                            "65.0          NaN  ...                       NaN       NaN   \n",
+                            "66.0          NaN  ...                       NaN       NaN   \n",
+                            "NaN           NaN  ...                       NaN       NaN   \n",
+                            "NaN           NaN  ...                       NaN       NaN   \n",
+                            "NaN           NaN  ...                       NaN       NaN   \n",
+                            "\n",
+                            "                                     Formula Parameters  \\\n",
+                            "0.0                                                  []   \n",
+                            "1.0       [signal=76E93E65-B284-4722-8B34-9142B04F34AA]   \n",
+                            "2.0       [signal=088D7186-54DB-402C-AFD7-528B4F426DB3]   \n",
+                            "3.0         [temp=C0F59A23-AB56-424F-A79D-5EAF81AF0237]   \n",
+                            "4.0   [temp=C0F59A23-AB56-424F-A79D-5EAF81AF0237, th...   \n",
+                            "...                                                 ...   \n",
+                            "65.0  [temp=17116A30-5DB7-434C-8E17-C564C884B629, th...   \n",
+                            "66.0                                                NaN   \n",
+                            "NaN                                                 NaN   \n",
+                            "NaN                                                 NaN   \n",
+                            "NaN                                                 NaN   \n",
+                            "\n",
+                            "                                 Scoped To Datasource Class  Datasource ID  \\\n",
+                            "0.0   90C07295-7D30-4DA6-8B5E-4DE3C7EF425C    Seeq Data Lab  Seeq Data Lab   \n",
+                            "1.0   90C07295-7D30-4DA6-8B5E-4DE3C7EF425C    Seeq Data Lab  Seeq Data Lab   \n",
+                            "2.0   90C07295-7D30-4DA6-8B5E-4DE3C7EF425C    Seeq Data Lab  Seeq Data Lab   \n",
+                            "3.0   90C07295-7D30-4DA6-8B5E-4DE3C7EF425C    Seeq Data Lab  Seeq Data Lab   \n",
+                            "4.0   90C07295-7D30-4DA6-8B5E-4DE3C7EF425C    Seeq Data Lab  Seeq Data Lab   \n",
+                            "...                                    ...              ...            ...   \n",
+                            "65.0  90C07295-7D30-4DA6-8B5E-4DE3C7EF425C    Seeq Data Lab  Seeq Data Lab   \n",
+                            "66.0  90C07295-7D30-4DA6-8B5E-4DE3C7EF425C    Seeq Data Lab  Seeq Data Lab   \n",
+                            "NaN                                    NaN    Seeq Data Lab  Seeq Data Lab   \n",
+                            "NaN                                    NaN    Seeq Data Lab  Seeq Data Lab   \n",
+                            "NaN                                    NaN    Seeq Data Lab  Seeq Data Lab   \n",
+                            "\n",
+                            "                                                Data ID Push Result  \\\n",
+                            "0.0   [90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Scalar...     Success   \n",
+                            "1.0   [90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Signal...     Success   \n",
+                            "2.0   [90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Signal...     Success   \n",
+                            "3.0   [90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Signal...     Success   \n",
+                            "4.0   [90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Condit...     Success   \n",
+                            "...                                                 ...         ...   \n",
+                            "65.0  [90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Condit...     Success   \n",
+                            "66.0  [90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Asset}...     Success   \n",
+                            "NaN   [90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Asset}...     Success   \n",
+                            "NaN   [90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Asset}...     Success   \n",
+                            "NaN   [90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Asset}...     Success   \n",
+                            "\n",
+                            "     Cache Enabled                         Referenced ID  \n",
+                            "0.0            NaN                                   NaN  \n",
+                            "1.0          False  76E93E65-B284-4722-8B34-9142B04F34AA  \n",
+                            "2.0          False  088D7186-54DB-402C-AFD7-528B4F426DB3  \n",
+                            "3.0            NaN                                   NaN  \n",
+                            "4.0            NaN                                   NaN  \n",
+                            "...            ...                                   ...  \n",
+                            "65.0           NaN                                   NaN  \n",
+                            "66.0           NaN                                   NaN  \n",
+                            "NaN            NaN                                   NaN  \n",
+                            "NaN            NaN                                   NaN  \n",
+                            "NaN            NaN                                   NaN  \n",
                             "\n",
-                            "[67 rows x 20 columns]"
+                            "[70 rows x 23 columns]"
                         ]
                     },
                     "execution_count": 10,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -2999,15 +3203,15 @@
             "cell_type": "code",
             "execution_count": 11,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<div style=\"background-color: #EEFFEE;color:black;text-align: left;\">Query successful</div><table style=\"color:black;\"><tr><td style=\"background-color: #EEFFEE;\"></td><td style=\"background-color: #EEFFEE; text-align: left;\">Name</td><td style=\"background-color: #EEFFEE; text-align: left;\">Datasource Class</td><td style=\"background-color: #EEFFEE; text-align: left;\">Time</td><td style=\"background-color: #EEFFEE; text-align: right;\">Count</td><td style=\"background-color: #EEFFEE; text-align: right;\">Pages</td><td style=\"background-color: #EEFFEE; text-align: left;\">Result</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">0</td><td style=\"text-align: left; vertical-align: top;\">/Area [A-D]_(?:Temperature|Compressor Power)/</td><td style=\"text-align: left; vertical-align: top;\">Time Series CSV Files</td><td style=\"vertical-align: top;\">00:00:00.02</td><td style=\"text-align: right; vertical-align: top;\">8</td><td style=\"text-align: right; vertical-align: top;\">1</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr></table>"
+                            "<div style=\"background-color: #EEFFEE;color:black; text-align: left;\">Query successful</div><table class=\"tex2jax_ignore\" style=\"color:black;\"><tr><td style=\"background-color: #EEFFEE;\"></td><td style=\"background-color: #EEFFEE; text-align: left;\">Name</td><td style=\"background-color: #EEFFEE; text-align: left;\">Datasource Class</td><td style=\"background-color: #EEFFEE; text-align: left;\">Time</td><td style=\"background-color: #EEFFEE; text-align: right;\">Count</td><td style=\"background-color: #EEFFEE; text-align: right;\">Pages</td><td style=\"background-color: #EEFFEE; text-align: left;\">Result</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">0</td><td style=\"text-align: left; vertical-align: top;\">/Area [A-D]_(?:Temperature|Compressor Power)/</td><td style=\"text-align: left; vertical-align: top;\">Time Series CSV Files</td><td style=\"vertical-align: top;\">00:00:00.02</td><td style=\"text-align: right; vertical-align: top;\">8</td><td style=\"text-align: right; vertical-align: top;\">1</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr></table>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -3039,100 +3243,100 @@
                             "      <th>Build Asset</th>\n",
                             "      <th>Compressor</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
-                            "      <td>B967C513-DB58-41CA-814B-2650465466BB</td>\n",
+                            "      <td>735C9627-F777-46C4-BAF5-B5B74F4534CF</td>\n",
                             "      <td>Area B_Temperature</td>\n",
                             "      <td>Refrigerator Units</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1</th>\n",
-                            "      <td>7E99DB2D-AE68-43F9-99EE-BE4095976E94</td>\n",
-                            "      <td>Area A_Compressor Power</td>\n",
+                            "      <td>F8B2EF0E-BAB2-441D-B031-6F920099D74A</td>\n",
+                            "      <td>Area A_Temperature</td>\n",
                             "      <td>Refrigerator Units</td>\n",
                             "      <td>Refrigerator 1</td>\n",
-                            "      <td>Compressor 1</td>\n",
+                            "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2</th>\n",
-                            "      <td>C1F1002A-469E-47D1-83AB-99FD17650B55</td>\n",
-                            "      <td>Area A_Temperature</td>\n",
+                            "      <td>84ED2BB0-AD0B-4C76-8233-EEA7EB358F97</td>\n",
+                            "      <td>Area B_Compressor Power</td>\n",
                             "      <td>Refrigerator Units</td>\n",
                             "      <td>Refrigerator 1</td>\n",
-                            "      <td>NaN</td>\n",
+                            "      <td>Compressor 2</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>3</th>\n",
-                            "      <td>A531B8F4-E5C6-4114-BB62-646BCFBD9DA4</td>\n",
-                            "      <td>Area C_Compressor Power</td>\n",
+                            "      <td>BDD6B3E7-6A62-4C43-AC60-4F6EF8525134</td>\n",
+                            "      <td>Area C_Temperature</td>\n",
                             "      <td>Refrigerator Units</td>\n",
                             "      <td>Refrigerator 2</td>\n",
-                            "      <td>Compressor 3</td>\n",
+                            "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>4</th>\n",
-                            "      <td>06BD8E98-DA1B-4984-B19F-367AD09340A2</td>\n",
-                            "      <td>Area D_Temperature</td>\n",
+                            "      <td>B4213340-A80E-4FF1-B277-7408E99FEDFE</td>\n",
+                            "      <td>Area A_Compressor Power</td>\n",
                             "      <td>Refrigerator Units</td>\n",
-                            "      <td>NaN</td>\n",
-                            "      <td>NaN</td>\n",
+                            "      <td>Refrigerator 1</td>\n",
+                            "      <td>Compressor 1</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>5</th>\n",
-                            "      <td>46E29219-3339-4F50-8137-C9C23B16DEF9</td>\n",
-                            "      <td>Area C_Temperature</td>\n",
+                            "      <td>C90CB4E9-6CF7-4F13-BA6D-5078EA33ADAB</td>\n",
+                            "      <td>Area D_Temperature</td>\n",
                             "      <td>Refrigerator Units</td>\n",
-                            "      <td>Refrigerator 2</td>\n",
+                            "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>6</th>\n",
-                            "      <td>87CB3E07-0568-4C53-A9A2-EDCD72CF8AC3</td>\n",
-                            "      <td>Area D_Compressor Power</td>\n",
+                            "      <td>954749C3-D3FF-4F10-9A2B-A5AF80E13E9D</td>\n",
+                            "      <td>Area C_Compressor Power</td>\n",
                             "      <td>Refrigerator Units</td>\n",
                             "      <td>Refrigerator 2</td>\n",
-                            "      <td>Compressor 4</td>\n",
+                            "      <td>Compressor 3</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>7</th>\n",
-                            "      <td>C6BC4291-2606-465A-B6AE-5427CB8540D8</td>\n",
-                            "      <td>Area B_Compressor Power</td>\n",
+                            "      <td>30F8FDAF-293A-4C86-9179-A7CF7B1847B4</td>\n",
+                            "      <td>Area D_Compressor Power</td>\n",
                             "      <td>Refrigerator Units</td>\n",
-                            "      <td>Refrigerator 1</td>\n",
-                            "      <td>Compressor 2</td>\n",
+                            "      <td>Refrigerator 2</td>\n",
+                            "      <td>Compressor 4</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
                             "                                     ID                     Name  \\\n",
-                            "0  B967C513-DB58-41CA-814B-2650465466BB       Area B_Temperature   \n",
-                            "1  7E99DB2D-AE68-43F9-99EE-BE4095976E94  Area A_Compressor Power   \n",
-                            "2  C1F1002A-469E-47D1-83AB-99FD17650B55       Area A_Temperature   \n",
-                            "3  A531B8F4-E5C6-4114-BB62-646BCFBD9DA4  Area C_Compressor Power   \n",
-                            "4  06BD8E98-DA1B-4984-B19F-367AD09340A2       Area D_Temperature   \n",
-                            "5  46E29219-3339-4F50-8137-C9C23B16DEF9       Area C_Temperature   \n",
-                            "6  87CB3E07-0568-4C53-A9A2-EDCD72CF8AC3  Area D_Compressor Power   \n",
-                            "7  C6BC4291-2606-465A-B6AE-5427CB8540D8  Area B_Compressor Power   \n",
+                            "0  735C9627-F777-46C4-BAF5-B5B74F4534CF       Area B_Temperature   \n",
+                            "1  F8B2EF0E-BAB2-441D-B031-6F920099D74A       Area A_Temperature   \n",
+                            "2  84ED2BB0-AD0B-4C76-8233-EEA7EB358F97  Area B_Compressor Power   \n",
+                            "3  BDD6B3E7-6A62-4C43-AC60-4F6EF8525134       Area C_Temperature   \n",
+                            "4  B4213340-A80E-4FF1-B277-7408E99FEDFE  Area A_Compressor Power   \n",
+                            "5  C90CB4E9-6CF7-4F13-BA6D-5078EA33ADAB       Area D_Temperature   \n",
+                            "6  954749C3-D3FF-4F10-9A2B-A5AF80E13E9D  Area C_Compressor Power   \n",
+                            "7  30F8FDAF-293A-4C86-9179-A7CF7B1847B4  Area D_Compressor Power   \n",
                             "\n",
                             "           Build Path     Build Asset    Compressor  \n",
                             "0  Refrigerator Units             NaN           NaN  \n",
-                            "1  Refrigerator Units  Refrigerator 1  Compressor 1  \n",
-                            "2  Refrigerator Units  Refrigerator 1           NaN  \n",
-                            "3  Refrigerator Units  Refrigerator 2  Compressor 3  \n",
-                            "4  Refrigerator Units             NaN           NaN  \n",
-                            "5  Refrigerator Units  Refrigerator 2           NaN  \n",
-                            "6  Refrigerator Units  Refrigerator 2  Compressor 4  \n",
-                            "7  Refrigerator Units  Refrigerator 1  Compressor 2  "
+                            "1  Refrigerator Units  Refrigerator 1           NaN  \n",
+                            "2  Refrigerator Units  Refrigerator 1  Compressor 2  \n",
+                            "3  Refrigerator Units  Refrigerator 2           NaN  \n",
+                            "4  Refrigerator Units  Refrigerator 1  Compressor 1  \n",
+                            "5  Refrigerator Units             NaN           NaN  \n",
+                            "6  Refrigerator Units  Refrigerator 2  Compressor 3  \n",
+                            "7  Refrigerator Units  Refrigerator 2  Compressor 4  "
                         ]
                     },
                     "execution_count": 11,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -3169,15 +3373,15 @@
             "cell_type": "code",
             "execution_count": 12,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<div style=\"background-color: #EEFFEE;color:black;text-align: left;\">Pushed successfully to datasource <strong>Seeq Data Lab [Datasource ID: Seeq Data Lab]</strong> and scoped to workbook ID <strong>807F13D7-C424-4840-B88B-D46F417A4966</strong><br>Click the following link to see what you pushed in Seeq:<br><a href=\"http://localhost:34216/28420AC3-152B-47A0-ACB7-6B060C3338FD/workbook/807F13D7-C424-4840-B88B-D46F417A4966/worksheet/C8375B1E-7DE2-44A6-BE3F-CA24281D6B72\" target=\"_new\">http://localhost:34216/28420AC3-152B-47A0-ACB7-6B060C3338FD/workbook/807F13D7-C424-4840-B88B-D46F417A4966/worksheet/C8375B1E-7DE2-44A6-BE3F-CA24281D6B72</a></div>"
+                            "<div style=\"background-color: #EEFFEE;color:black; text-align: left;\">Pushed successfully to datasource <strong>Seeq Data Lab [Datasource ID: Seeq Data Lab]</strong> and scoped to workbook ID <strong>90C07295-7D30-4DA6-8B5E-4DE3C7EF425C</strong><br>Click the following link to see what you pushed in Seeq:<br><a href=\"http://localhost:34216/5F85F903-0ED4-42B1-8B9E-418718482532/workbook/90C07295-7D30-4DA6-8B5E-4DE3C7EF425C/worksheet/5B3A24A6-1ABF-4403-BD0B-28669B4A60BF\" target=\"_new\">http://localhost:34216/5F85F903-0ED4-42B1-8B9E-418718482532/workbook/90C07295-7D30-4DA6-8B5E-4DE3C7EF425C/worksheet/5B3A24A6-1ABF-4403-BD0B-28669B4A60BF</a></div>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -3199,855 +3403,861 @@
                             "        text-align: right;\n",
                             "    }\n",
                             "</style>\n",
                             "<table border=\"1\" class=\"dataframe\">\n",
                             "  <thead>\n",
                             "    <tr style=\"text-align: right;\">\n",
                             "      <th></th>\n",
-                            "      <th>ID</th>\n",
                             "      <th>Description</th>\n",
                             "      <th>Type</th>\n",
-                            "      <th>Value Unit Of Measure</th>\n",
                             "      <th>Datasource Name</th>\n",
                             "      <th>Archived</th>\n",
                             "      <th>Compressor</th>\n",
                             "      <th>Referenced Name</th>\n",
                             "      <th>Reference</th>\n",
                             "      <th>Name</th>\n",
-                            "      <th>...</th>\n",
+                            "      <th>Asset</th>\n",
                             "      <th>Asset Object</th>\n",
-                            "      <th>Path</th>\n",
-                            "      <th>Template</th>\n",
-                            "      <th>Build Result</th>\n",
-                            "      <th>Formula</th>\n",
+                            "      <th>...</th>\n",
                             "      <th>Formula Parameters</th>\n",
+                            "      <th>Cache Enabled</th>\n",
+                            "      <th>Referenced ID</th>\n",
+                            "      <th>Scoped To</th>\n",
                             "      <th>Datasource Class</th>\n",
                             "      <th>Datasource ID</th>\n",
                             "      <th>Data ID</th>\n",
+                            "      <th>ID</th>\n",
                             "      <th>Push Result</th>\n",
+                            "      <th>Value Unit Of Measure</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
-                            "      <th>0</th>\n",
-                            "      <td>9196030F-C4C8-4EED-A8A3-2FE5F6EEFEB0</td>\n",
+                            "      <th>0.0</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>CalculatedSignal</td>\n",
-                            "      <td>kW</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
-                            "      <td>Compressor 1</td>\n",
-                            "      <td>Area A_Compressor Power</td>\n",
+                            "      <td>Compressor 2</td>\n",
+                            "      <td>Area B_Compressor Power</td>\n",
                             "      <td>True</td>\n",
                             "      <td>Power</td>\n",
-                            "      <td>...</td>\n",
+                            "      <td>Compressor 2</td>\n",
                             "      <td>Refrigerator Units &gt;&gt; Refrigerator 1 &gt;&gt; Compre...</td>\n",
-                            "      <td>Refrigerator Units &gt;&gt; Refrigerator 1</td>\n",
-                            "      <td>Compressor</td>\n",
-                            "      <td>Success</td>\n",
-                            "      <td>NaN</td>\n",
-                            "      <td>[signal=7E99DB2D-AE68-43F9-99EE-BE4095976E94]</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>[signal=84ED2BB0-AD0B-4C76-8233-EEA7EB358F97]</td>\n",
+                            "      <td>False</td>\n",
+                            "      <td>84ED2BB0-AD0B-4C76-8233-EEA7EB358F97</td>\n",
+                            "      <td>90C07295-7D30-4DA6-8B5E-4DE3C7EF425C</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[807F13D7-C424-4840-B88B-D46F417A4966] {Signal...</td>\n",
+                            "      <td>[90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Signal...</td>\n",
+                            "      <td>215E4C66-6AEA-490A-8506-B8A556792999</td>\n",
                             "      <td>Success</td>\n",
+                            "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>1</th>\n",
-                            "      <td>2ABA5770-D7AD-4861-8634-E31C96F9EC91</td>\n",
+                            "      <th>1.0</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>CalculatedCondition</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>NaN</td>\n",
                             "      <td>High Power</td>\n",
-                            "      <td>...</td>\n",
+                            "      <td>Compressor 2</td>\n",
                             "      <td>Refrigerator Units &gt;&gt; Refrigerator 1 &gt;&gt; Compre...</td>\n",
-                            "      <td>Refrigerator Units &gt;&gt; Refrigerator 1</td>\n",
-                            "      <td>Compressor</td>\n",
-                            "      <td>Success</td>\n",
-                            "      <td>$a.valueSearch(isGreaterThan(20kW))</td>\n",
-                            "      <td>[a=9196030F-C4C8-4EED-A8A3-2FE5F6EEFEB0]</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>[a=215E4C66-6AEA-490A-8506-B8A556792999]</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>90C07295-7D30-4DA6-8B5E-4DE3C7EF425C</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[807F13D7-C424-4840-B88B-D46F417A4966] {Condit...</td>\n",
+                            "      <td>[90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Condit...</td>\n",
+                            "      <td>5795BF85-79E1-4508-A084-ECA1B25B5990</td>\n",
                             "      <td>Success</td>\n",
+                            "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>2</th>\n",
-                            "      <td>9EFDA8AE-4BD1-4322-9096-A8C06381EB50</td>\n",
+                            "      <th>2.0</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>CalculatedCondition</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>NaN</td>\n",
                             "      <td>Other Compressors Are High Power</td>\n",
-                            "      <td>...</td>\n",
+                            "      <td>Compressor 1</td>\n",
                             "      <td>Refrigerator Units &gt;&gt; Refrigerator 1 &gt;&gt; Compre...</td>\n",
-                            "      <td>Refrigerator Units &gt;&gt; Refrigerator 1</td>\n",
-                            "      <td>Compressor</td>\n",
-                            "      <td>Success</td>\n",
-                            "      <td>$p0</td>\n",
-                            "      <td>[p0=2ABA5770-D7AD-4861-8634-E31C96F9EC91]</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>[p0=5795BF85-79E1-4508-A084-ECA1B25B5990]</td>\n",
+                            "      <td>False</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>90C07295-7D30-4DA6-8B5E-4DE3C7EF425C</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[807F13D7-C424-4840-B88B-D46F417A4966] {Condit...</td>\n",
+                            "      <td>[90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Condit...</td>\n",
+                            "      <td>C10C2EBF-092E-4232-AF25-BD2314FE1A3B</td>\n",
                             "      <td>Success</td>\n",
+                            "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>3</th>\n",
-                            "      <td>0FFCF13E-6AEB-4F3A-9958-E3D3AC1DA753</td>\n",
+                            "      <th>3.0</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>CalculatedSignal</td>\n",
-                            "      <td>kW</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
-                            "      <td>Compressor 2</td>\n",
-                            "      <td>Area B_Compressor Power</td>\n",
+                            "      <td>Compressor 1</td>\n",
+                            "      <td>Area A_Compressor Power</td>\n",
                             "      <td>True</td>\n",
                             "      <td>Power</td>\n",
-                            "      <td>...</td>\n",
+                            "      <td>Compressor 1</td>\n",
                             "      <td>Refrigerator Units &gt;&gt; Refrigerator 1 &gt;&gt; Compre...</td>\n",
-                            "      <td>Refrigerator Units &gt;&gt; Refrigerator 1</td>\n",
-                            "      <td>Compressor</td>\n",
-                            "      <td>Success</td>\n",
-                            "      <td>NaN</td>\n",
-                            "      <td>[signal=C6BC4291-2606-465A-B6AE-5427CB8540D8]</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>[signal=B4213340-A80E-4FF1-B277-7408E99FEDFE]</td>\n",
+                            "      <td>False</td>\n",
+                            "      <td>B4213340-A80E-4FF1-B277-7408E99FEDFE</td>\n",
+                            "      <td>90C07295-7D30-4DA6-8B5E-4DE3C7EF425C</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[807F13D7-C424-4840-B88B-D46F417A4966] {Signal...</td>\n",
+                            "      <td>[90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Signal...</td>\n",
+                            "      <td>85A9A341-ED97-44E3-9F0E-3D12A908F28A</td>\n",
                             "      <td>Success</td>\n",
+                            "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>4</th>\n",
-                            "      <td>3C236F11-67D1-4D69-8F02-7C382FAC809B</td>\n",
+                            "      <th>4.0</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>CalculatedCondition</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>NaN</td>\n",
                             "      <td>High Power</td>\n",
-                            "      <td>...</td>\n",
+                            "      <td>Compressor 1</td>\n",
                             "      <td>Refrigerator Units &gt;&gt; Refrigerator 1 &gt;&gt; Compre...</td>\n",
-                            "      <td>Refrigerator Units &gt;&gt; Refrigerator 1</td>\n",
-                            "      <td>Compressor</td>\n",
-                            "      <td>Success</td>\n",
-                            "      <td>$a.valueSearch(isGreaterThan(20kW))</td>\n",
-                            "      <td>[a=0FFCF13E-6AEB-4F3A-9958-E3D3AC1DA753]</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>[a=85A9A341-ED97-44E3-9F0E-3D12A908F28A]</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>90C07295-7D30-4DA6-8B5E-4DE3C7EF425C</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[807F13D7-C424-4840-B88B-D46F417A4966] {Condit...</td>\n",
+                            "      <td>[90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Condit...</td>\n",
+                            "      <td>24349142-C25B-4EE6-892C-AF6619FBD606</td>\n",
                             "      <td>Success</td>\n",
+                            "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>5</th>\n",
-                            "      <td>E99C13D0-9A89-4033-A5D8-BB55E5E98814</td>\n",
+                            "      <th>5.0</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>Asset</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>NaN</td>\n",
-                            "      <td>Compressor 2</td>\n",
-                            "      <td>...</td>\n",
+                            "      <td>Compressor 1</td>\n",
+                            "      <td>Compressor 1</td>\n",
                             "      <td>Refrigerator Units &gt;&gt; Refrigerator 1 &gt;&gt; Compre...</td>\n",
-                            "      <td>Refrigerator Units &gt;&gt; Refrigerator 1</td>\n",
-                            "      <td>Compressor</td>\n",
-                            "      <td>Success</td>\n",
+                            "      <td>...</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>90C07295-7D30-4DA6-8B5E-4DE3C7EF425C</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[807F13D7-C424-4840-B88B-D46F417A4966] {Asset}...</td>\n",
+                            "      <td>[90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Asset}...</td>\n",
+                            "      <td>FC49E623-638C-4244-B933-2F8D333215C1</td>\n",
                             "      <td>Success</td>\n",
+                            "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>6</th>\n",
-                            "      <td>8B855ED1-6962-44DA-9A92-4F4C169D93BA</td>\n",
+                            "      <th>6.0</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>CalculatedSignal</td>\n",
-                            "      <td>\u00b0F</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>Area A_Temperature</td>\n",
                             "      <td>True</td>\n",
                             "      <td>Temperature</td>\n",
-                            "      <td>...</td>\n",
+                            "      <td>Refrigerator 1</td>\n",
                             "      <td>Refrigerator Units &gt;&gt; Refrigerator 1</td>\n",
-                            "      <td>Refrigerator Units</td>\n",
-                            "      <td>Refrigerator</td>\n",
-                            "      <td>Success</td>\n",
-                            "      <td>NaN</td>\n",
-                            "      <td>[signal=C1F1002A-469E-47D1-83AB-99FD17650B55]</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>[signal=F8B2EF0E-BAB2-441D-B031-6F920099D74A]</td>\n",
+                            "      <td>False</td>\n",
+                            "      <td>F8B2EF0E-BAB2-441D-B031-6F920099D74A</td>\n",
+                            "      <td>90C07295-7D30-4DA6-8B5E-4DE3C7EF425C</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[807F13D7-C424-4840-B88B-D46F417A4966] {Signal...</td>\n",
+                            "      <td>[90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Signal...</td>\n",
+                            "      <td>AA8EDA7A-D704-477F-B67F-E4181B380326</td>\n",
                             "      <td>Success</td>\n",
+                            "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>7</th>\n",
-                            "      <td>1F6FEA1E-32CB-44B5-B673-E0AE8E1A01C9</td>\n",
+                            "      <th>7.0</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>CalculatedCondition</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>NaN</td>\n",
                             "      <td>Compressor High Power</td>\n",
-                            "      <td>...</td>\n",
+                            "      <td>Refrigerator 1</td>\n",
                             "      <td>Refrigerator Units &gt;&gt; Refrigerator 1</td>\n",
-                            "      <td>Refrigerator Units</td>\n",
-                            "      <td>Refrigerator</td>\n",
-                            "      <td>Success</td>\n",
-                            "      <td>$p0 or $p1</td>\n",
-                            "      <td>[p0=2ABA5770-D7AD-4861-8634-E31C96F9EC91, p1=3...</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>[p0=5795BF85-79E1-4508-A084-ECA1B25B5990, p1=2...</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>90C07295-7D30-4DA6-8B5E-4DE3C7EF425C</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[807F13D7-C424-4840-B88B-D46F417A4966] {Condit...</td>\n",
+                            "      <td>[90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Condit...</td>\n",
+                            "      <td>7997B9B7-5093-473B-8A5A-2A7AD1EA306E</td>\n",
                             "      <td>Success</td>\n",
+                            "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>8</th>\n",
-                            "      <td>E4A5416C-75DA-4EF4-917A-252BECA2285B</td>\n",
+                            "      <th>8.0</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>CalculatedCondition</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>NaN</td>\n",
                             "      <td>Other Compressors Are High Power</td>\n",
-                            "      <td>...</td>\n",
+                            "      <td>Compressor 2</td>\n",
                             "      <td>Refrigerator Units &gt;&gt; Refrigerator 1 &gt;&gt; Compre...</td>\n",
-                            "      <td>Refrigerator Units &gt;&gt; Refrigerator 1</td>\n",
-                            "      <td>Compressor</td>\n",
-                            "      <td>Success</td>\n",
-                            "      <td>$p0</td>\n",
-                            "      <td>[p0=3C236F11-67D1-4D69-8F02-7C382FAC809B]</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>[p0=24349142-C25B-4EE6-892C-AF6619FBD606]</td>\n",
+                            "      <td>False</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>90C07295-7D30-4DA6-8B5E-4DE3C7EF425C</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[807F13D7-C424-4840-B88B-D46F417A4966] {Condit...</td>\n",
+                            "      <td>[90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Condit...</td>\n",
+                            "      <td>E7884BC1-869A-46C4-9F23-C6324A75B979</td>\n",
                             "      <td>Success</td>\n",
+                            "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>9</th>\n",
-                            "      <td>F56061F4-661D-4EF1-A3D9-D340DD75F096</td>\n",
+                            "      <th>9.0</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>Asset</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>NaN</td>\n",
-                            "      <td>Compressor 1</td>\n",
-                            "      <td>...</td>\n",
+                            "      <td>Compressor 2</td>\n",
+                            "      <td>Compressor 2</td>\n",
                             "      <td>Refrigerator Units &gt;&gt; Refrigerator 1 &gt;&gt; Compre...</td>\n",
-                            "      <td>Refrigerator Units &gt;&gt; Refrigerator 1</td>\n",
-                            "      <td>Compressor</td>\n",
-                            "      <td>Success</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
+                            "      <td>90C07295-7D30-4DA6-8B5E-4DE3C7EF425C</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[807F13D7-C424-4840-B88B-D46F417A4966] {Asset}...</td>\n",
+                            "      <td>[90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Asset}...</td>\n",
+                            "      <td>191E9995-AC0A-49B0-B0F6-5EABF34B32E0</td>\n",
                             "      <td>Success</td>\n",
+                            "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>10</th>\n",
-                            "      <td>B09A6B45-AF14-44BC-8A51-47DEB8E5836F</td>\n",
+                            "      <th>10.0</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>CalculatedSignal</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>NaN</td>\n",
                             "      <td>Compressor Power Max</td>\n",
-                            "      <td>...</td>\n",
+                            "      <td>Refrigerator 1</td>\n",
                             "      <td>Refrigerator Units &gt;&gt; Refrigerator 1</td>\n",
-                            "      <td>Refrigerator Units</td>\n",
-                            "      <td>Refrigerator</td>\n",
-                            "      <td>Success</td>\n",
-                            "      <td>$p0.max($p1)</td>\n",
-                            "      <td>[p0=9196030F-C4C8-4EED-A8A3-2FE5F6EEFEB0, p1=0...</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>[p0=215E4C66-6AEA-490A-8506-B8A556792999, p1=8...</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>90C07295-7D30-4DA6-8B5E-4DE3C7EF425C</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[807F13D7-C424-4840-B88B-D46F417A4966] {Signal...</td>\n",
+                            "      <td>[90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Signal...</td>\n",
+                            "      <td>FEF4DC7E-7629-40F1-815A-8B4901F10711</td>\n",
                             "      <td>Success</td>\n",
+                            "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>11</th>\n",
-                            "      <td>CA5E9B99-4131-4B16-ADAE-3724F756D00E</td>\n",
+                            "      <th>11.0</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>Asset</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>NaN</td>\n",
                             "      <td>Refrigerator 1</td>\n",
-                            "      <td>...</td>\n",
+                            "      <td>Refrigerator 1</td>\n",
                             "      <td>Refrigerator Units &gt;&gt; Refrigerator 1</td>\n",
-                            "      <td>Refrigerator Units</td>\n",
-                            "      <td>Refrigerator</td>\n",
-                            "      <td>Success</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
+                            "      <td>90C07295-7D30-4DA6-8B5E-4DE3C7EF425C</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[807F13D7-C424-4840-B88B-D46F417A4966] {Asset}...</td>\n",
+                            "      <td>[90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Asset}...</td>\n",
+                            "      <td>8BD6ECFB-A7CD-40AF-9AA7-C4B4B00707E0</td>\n",
                             "      <td>Success</td>\n",
+                            "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>12</th>\n",
-                            "      <td>D665A3FF-6981-4928-A49E-ACCE530FED9C</td>\n",
+                            "      <th>12.0</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>CalculatedSignal</td>\n",
-                            "      <td>kW</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
                             "      <td>Compressor 3</td>\n",
                             "      <td>Area C_Compressor Power</td>\n",
                             "      <td>True</td>\n",
                             "      <td>Power</td>\n",
-                            "      <td>...</td>\n",
+                            "      <td>Compressor 3</td>\n",
                             "      <td>Refrigerator Units &gt;&gt; Refrigerator 2 &gt;&gt; Compre...</td>\n",
-                            "      <td>Refrigerator Units &gt;&gt; Refrigerator 2</td>\n",
-                            "      <td>Compressor</td>\n",
-                            "      <td>Success</td>\n",
-                            "      <td>NaN</td>\n",
-                            "      <td>[signal=A531B8F4-E5C6-4114-BB62-646BCFBD9DA4]</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>[signal=954749C3-D3FF-4F10-9A2B-A5AF80E13E9D]</td>\n",
+                            "      <td>False</td>\n",
+                            "      <td>954749C3-D3FF-4F10-9A2B-A5AF80E13E9D</td>\n",
+                            "      <td>90C07295-7D30-4DA6-8B5E-4DE3C7EF425C</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[807F13D7-C424-4840-B88B-D46F417A4966] {Signal...</td>\n",
+                            "      <td>[90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Signal...</td>\n",
+                            "      <td>AB5138AE-3633-4A32-B324-C6F17630E27F</td>\n",
                             "      <td>Success</td>\n",
+                            "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>13</th>\n",
-                            "      <td>9DD37884-33B6-436D-B7D5-C90E9F183131</td>\n",
+                            "      <th>13.0</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>CalculatedCondition</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>NaN</td>\n",
                             "      <td>High Power</td>\n",
-                            "      <td>...</td>\n",
+                            "      <td>Compressor 3</td>\n",
                             "      <td>Refrigerator Units &gt;&gt; Refrigerator 2 &gt;&gt; Compre...</td>\n",
-                            "      <td>Refrigerator Units &gt;&gt; Refrigerator 2</td>\n",
-                            "      <td>Compressor</td>\n",
-                            "      <td>Success</td>\n",
-                            "      <td>$a.valueSearch(isGreaterThan(20kW))</td>\n",
-                            "      <td>[a=D665A3FF-6981-4928-A49E-ACCE530FED9C]</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>[a=AB5138AE-3633-4A32-B324-C6F17630E27F]</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>90C07295-7D30-4DA6-8B5E-4DE3C7EF425C</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[807F13D7-C424-4840-B88B-D46F417A4966] {Condit...</td>\n",
+                            "      <td>[90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Condit...</td>\n",
+                            "      <td>D3694232-C913-4503-A907-3AE71F102A00</td>\n",
                             "      <td>Success</td>\n",
+                            "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>14</th>\n",
-                            "      <td>A1D48963-7E5C-4FED-99DF-E48FE9B4D207</td>\n",
+                            "      <th>14.0</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>CalculatedCondition</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>NaN</td>\n",
                             "      <td>Other Compressors Are High Power</td>\n",
-                            "      <td>...</td>\n",
+                            "      <td>Compressor 4</td>\n",
                             "      <td>Refrigerator Units &gt;&gt; Refrigerator 2 &gt;&gt; Compre...</td>\n",
-                            "      <td>Refrigerator Units &gt;&gt; Refrigerator 2</td>\n",
-                            "      <td>Compressor</td>\n",
-                            "      <td>Success</td>\n",
-                            "      <td>$p0</td>\n",
-                            "      <td>[p0=9DD37884-33B6-436D-B7D5-C90E9F183131]</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>[p0=D3694232-C913-4503-A907-3AE71F102A00]</td>\n",
+                            "      <td>False</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>90C07295-7D30-4DA6-8B5E-4DE3C7EF425C</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[807F13D7-C424-4840-B88B-D46F417A4966] {Condit...</td>\n",
+                            "      <td>[90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Condit...</td>\n",
+                            "      <td>C3B9D73B-78B1-4136-9351-B395252BEECD</td>\n",
                             "      <td>Success</td>\n",
+                            "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>15</th>\n",
-                            "      <td>CB7E51A6-CE42-4FD4-BA65-7BD19E940251</td>\n",
+                            "      <th>15.0</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>CalculatedSignal</td>\n",
-                            "      <td>kW</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
                             "      <td>Compressor 4</td>\n",
                             "      <td>Area D_Compressor Power</td>\n",
                             "      <td>True</td>\n",
                             "      <td>Power</td>\n",
-                            "      <td>...</td>\n",
+                            "      <td>Compressor 4</td>\n",
                             "      <td>Refrigerator Units &gt;&gt; Refrigerator 2 &gt;&gt; Compre...</td>\n",
-                            "      <td>Refrigerator Units &gt;&gt; Refrigerator 2</td>\n",
-                            "      <td>Compressor</td>\n",
-                            "      <td>Success</td>\n",
-                            "      <td>NaN</td>\n",
-                            "      <td>[signal=87CB3E07-0568-4C53-A9A2-EDCD72CF8AC3]</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>[signal=30F8FDAF-293A-4C86-9179-A7CF7B1847B4]</td>\n",
+                            "      <td>False</td>\n",
+                            "      <td>30F8FDAF-293A-4C86-9179-A7CF7B1847B4</td>\n",
+                            "      <td>90C07295-7D30-4DA6-8B5E-4DE3C7EF425C</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[807F13D7-C424-4840-B88B-D46F417A4966] {Signal...</td>\n",
+                            "      <td>[90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Signal...</td>\n",
+                            "      <td>A304B8D4-82DA-49BD-B383-C535CF04B3FD</td>\n",
                             "      <td>Success</td>\n",
+                            "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>16</th>\n",
-                            "      <td>2FA4345B-2B91-4F62-A72B-7C3D810BB491</td>\n",
+                            "      <th>16.0</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>CalculatedCondition</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>NaN</td>\n",
                             "      <td>High Power</td>\n",
-                            "      <td>...</td>\n",
+                            "      <td>Compressor 4</td>\n",
                             "      <td>Refrigerator Units &gt;&gt; Refrigerator 2 &gt;&gt; Compre...</td>\n",
-                            "      <td>Refrigerator Units &gt;&gt; Refrigerator 2</td>\n",
-                            "      <td>Compressor</td>\n",
-                            "      <td>Success</td>\n",
-                            "      <td>$a.valueSearch(isGreaterThan(20kW))</td>\n",
-                            "      <td>[a=CB7E51A6-CE42-4FD4-BA65-7BD19E940251]</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>[a=A304B8D4-82DA-49BD-B383-C535CF04B3FD]</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>90C07295-7D30-4DA6-8B5E-4DE3C7EF425C</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[807F13D7-C424-4840-B88B-D46F417A4966] {Condit...</td>\n",
+                            "      <td>[90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Condit...</td>\n",
+                            "      <td>1BF05DD4-C85B-44CF-8A67-39029A54A2B7</td>\n",
                             "      <td>Success</td>\n",
+                            "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>17</th>\n",
-                            "      <td>E1897406-3D7D-4CFF-8908-21D047F7E484</td>\n",
+                            "      <th>17.0</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>Asset</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>NaN</td>\n",
                             "      <td>Compressor 4</td>\n",
-                            "      <td>...</td>\n",
+                            "      <td>Compressor 4</td>\n",
                             "      <td>Refrigerator Units &gt;&gt; Refrigerator 2 &gt;&gt; Compre...</td>\n",
-                            "      <td>Refrigerator Units &gt;&gt; Refrigerator 2</td>\n",
-                            "      <td>Compressor</td>\n",
-                            "      <td>Success</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
+                            "      <td>90C07295-7D30-4DA6-8B5E-4DE3C7EF425C</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[807F13D7-C424-4840-B88B-D46F417A4966] {Asset}...</td>\n",
+                            "      <td>[90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Asset}...</td>\n",
+                            "      <td>392B154B-C3A2-40DA-8A2C-F54EB03D0EF7</td>\n",
                             "      <td>Success</td>\n",
+                            "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>18</th>\n",
-                            "      <td>EA112378-6507-481D-917F-3561F7614A60</td>\n",
+                            "      <th>18.0</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>CalculatedSignal</td>\n",
-                            "      <td>\u00b0F</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>Area C_Temperature</td>\n",
                             "      <td>True</td>\n",
                             "      <td>Temperature</td>\n",
-                            "      <td>...</td>\n",
+                            "      <td>Refrigerator 2</td>\n",
                             "      <td>Refrigerator Units &gt;&gt; Refrigerator 2</td>\n",
-                            "      <td>Refrigerator Units</td>\n",
-                            "      <td>Refrigerator</td>\n",
-                            "      <td>Success</td>\n",
-                            "      <td>NaN</td>\n",
-                            "      <td>[signal=46E29219-3339-4F50-8137-C9C23B16DEF9]</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>[signal=BDD6B3E7-6A62-4C43-AC60-4F6EF8525134]</td>\n",
+                            "      <td>False</td>\n",
+                            "      <td>BDD6B3E7-6A62-4C43-AC60-4F6EF8525134</td>\n",
+                            "      <td>90C07295-7D30-4DA6-8B5E-4DE3C7EF425C</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[807F13D7-C424-4840-B88B-D46F417A4966] {Signal...</td>\n",
+                            "      <td>[90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Signal...</td>\n",
+                            "      <td>AE1D3114-FC56-4D85-A17E-AECB3001761C</td>\n",
                             "      <td>Success</td>\n",
+                            "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>19</th>\n",
-                            "      <td>507F7690-5AF8-42DE-8261-672D0D18C8CB</td>\n",
+                            "      <th>19.0</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>CalculatedCondition</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>NaN</td>\n",
                             "      <td>Compressor High Power</td>\n",
-                            "      <td>...</td>\n",
+                            "      <td>Refrigerator 2</td>\n",
                             "      <td>Refrigerator Units &gt;&gt; Refrigerator 2</td>\n",
-                            "      <td>Refrigerator Units</td>\n",
-                            "      <td>Refrigerator</td>\n",
-                            "      <td>Success</td>\n",
-                            "      <td>$p0 or $p1</td>\n",
-                            "      <td>[p0=9DD37884-33B6-436D-B7D5-C90E9F183131, p1=2...</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>[p0=D3694232-C913-4503-A907-3AE71F102A00, p1=1...</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>90C07295-7D30-4DA6-8B5E-4DE3C7EF425C</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[807F13D7-C424-4840-B88B-D46F417A4966] {Condit...</td>\n",
+                            "      <td>[90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Condit...</td>\n",
+                            "      <td>1EBB4BD4-2778-4D86-9623-6041F17DA282</td>\n",
                             "      <td>Success</td>\n",
+                            "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>20</th>\n",
-                            "      <td>3BAA7860-6153-4C73-BFCC-D19AA4B6F7F4</td>\n",
+                            "      <th>20.0</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>CalculatedCondition</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>NaN</td>\n",
                             "      <td>Other Compressors Are High Power</td>\n",
-                            "      <td>...</td>\n",
+                            "      <td>Compressor 3</td>\n",
                             "      <td>Refrigerator Units &gt;&gt; Refrigerator 2 &gt;&gt; Compre...</td>\n",
-                            "      <td>Refrigerator Units &gt;&gt; Refrigerator 2</td>\n",
-                            "      <td>Compressor</td>\n",
-                            "      <td>Success</td>\n",
-                            "      <td>$p0</td>\n",
-                            "      <td>[p0=2FA4345B-2B91-4F62-A72B-7C3D810BB491]</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>[p0=1BF05DD4-C85B-44CF-8A67-39029A54A2B7]</td>\n",
+                            "      <td>False</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>90C07295-7D30-4DA6-8B5E-4DE3C7EF425C</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[807F13D7-C424-4840-B88B-D46F417A4966] {Condit...</td>\n",
+                            "      <td>[90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Condit...</td>\n",
+                            "      <td>17B175B4-859F-4C5C-B21F-18AA174A1EB6</td>\n",
                             "      <td>Success</td>\n",
+                            "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>21</th>\n",
-                            "      <td>CE5CB4A8-BA17-48DA-B357-1BE876CDC751</td>\n",
+                            "      <th>21.0</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>Asset</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>NaN</td>\n",
                             "      <td>Compressor 3</td>\n",
-                            "      <td>...</td>\n",
+                            "      <td>Compressor 3</td>\n",
                             "      <td>Refrigerator Units &gt;&gt; Refrigerator 2 &gt;&gt; Compre...</td>\n",
-                            "      <td>Refrigerator Units &gt;&gt; Refrigerator 2</td>\n",
-                            "      <td>Compressor</td>\n",
-                            "      <td>Success</td>\n",
+                            "      <td>...</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>90C07295-7D30-4DA6-8B5E-4DE3C7EF425C</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[807F13D7-C424-4840-B88B-D46F417A4966] {Asset}...</td>\n",
+                            "      <td>[90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Asset}...</td>\n",
+                            "      <td>99107DAE-E79D-4564-8B0A-BC1390C67F28</td>\n",
                             "      <td>Success</td>\n",
+                            "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>22</th>\n",
-                            "      <td>E5B23C51-98DE-4BB9-8E20-516C31DE2D52</td>\n",
+                            "      <th>22.0</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>CalculatedSignal</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>NaN</td>\n",
                             "      <td>Compressor Power Max</td>\n",
-                            "      <td>...</td>\n",
+                            "      <td>Refrigerator 2</td>\n",
                             "      <td>Refrigerator Units &gt;&gt; Refrigerator 2</td>\n",
-                            "      <td>Refrigerator Units</td>\n",
-                            "      <td>Refrigerator</td>\n",
-                            "      <td>Success</td>\n",
-                            "      <td>$p0.max($p1)</td>\n",
-                            "      <td>[p0=D665A3FF-6981-4928-A49E-ACCE530FED9C, p1=C...</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>[p0=AB5138AE-3633-4A32-B324-C6F17630E27F, p1=A...</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>90C07295-7D30-4DA6-8B5E-4DE3C7EF425C</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[807F13D7-C424-4840-B88B-D46F417A4966] {Signal...</td>\n",
+                            "      <td>[90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Signal...</td>\n",
+                            "      <td>7C1592C9-94AB-4E7F-A379-8A40B5A57EF6</td>\n",
                             "      <td>Success</td>\n",
+                            "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>23</th>\n",
-                            "      <td>14099FE4-0F7D-44C1-9311-088494EA3327</td>\n",
+                            "      <th>23.0</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>Asset</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>NaN</td>\n",
                             "      <td>Refrigerator 2</td>\n",
-                            "      <td>...</td>\n",
+                            "      <td>Refrigerator 2</td>\n",
                             "      <td>Refrigerator Units &gt;&gt; Refrigerator 2</td>\n",
-                            "      <td>Refrigerator Units</td>\n",
-                            "      <td>Refrigerator</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>90C07295-7D30-4DA6-8B5E-4DE3C7EF425C</td>\n",
+                            "      <td>Seeq Data Lab</td>\n",
+                            "      <td>Seeq Data Lab</td>\n",
+                            "      <td>[90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Asset}...</td>\n",
+                            "      <td>A188AAA6-4C8A-4829-962E-55AA3DCBC77D</td>\n",
                             "      <td>Success</td>\n",
                             "      <td>NaN</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>NaN</th>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>Asset</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>Refrigerator Units</td>\n",
+                            "      <td>Refrigerator Units</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[807F13D7-C424-4840-B88B-D46F417A4966] {Asset}...</td>\n",
+                            "      <td>[90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Asset}...</td>\n",
+                            "      <td>240448CA-0624-47FC-A6D1-1559F59A8FC5</td>\n",
                             "      <td>Success</td>\n",
+                            "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
-                            "<p>24 rows \u00d7 21 columns</p>\n",
+                            "<p>25 rows \u00d7 24 columns</p>\n",
                             "</div>"
                         ],
                         "text/plain": [
-                            "                                      ID Description                 Type  \\\n",
-                            "0   9196030F-C4C8-4EED-A8A3-2FE5F6EEFEB0         NaN     CalculatedSignal   \n",
-                            "1   2ABA5770-D7AD-4861-8634-E31C96F9EC91         NaN  CalculatedCondition   \n",
-                            "2   9EFDA8AE-4BD1-4322-9096-A8C06381EB50         NaN  CalculatedCondition   \n",
-                            "3   0FFCF13E-6AEB-4F3A-9958-E3D3AC1DA753         NaN     CalculatedSignal   \n",
-                            "4   3C236F11-67D1-4D69-8F02-7C382FAC809B         NaN  CalculatedCondition   \n",
-                            "5   E99C13D0-9A89-4033-A5D8-BB55E5E98814         NaN                Asset   \n",
-                            "6   8B855ED1-6962-44DA-9A92-4F4C169D93BA         NaN     CalculatedSignal   \n",
-                            "7   1F6FEA1E-32CB-44B5-B673-E0AE8E1A01C9         NaN  CalculatedCondition   \n",
-                            "8   E4A5416C-75DA-4EF4-917A-252BECA2285B         NaN  CalculatedCondition   \n",
-                            "9   F56061F4-661D-4EF1-A3D9-D340DD75F096         NaN                Asset   \n",
-                            "10  B09A6B45-AF14-44BC-8A51-47DEB8E5836F         NaN     CalculatedSignal   \n",
-                            "11  CA5E9B99-4131-4B16-ADAE-3724F756D00E         NaN                Asset   \n",
-                            "12  D665A3FF-6981-4928-A49E-ACCE530FED9C         NaN     CalculatedSignal   \n",
-                            "13  9DD37884-33B6-436D-B7D5-C90E9F183131         NaN  CalculatedCondition   \n",
-                            "14  A1D48963-7E5C-4FED-99DF-E48FE9B4D207         NaN  CalculatedCondition   \n",
-                            "15  CB7E51A6-CE42-4FD4-BA65-7BD19E940251         NaN     CalculatedSignal   \n",
-                            "16  2FA4345B-2B91-4F62-A72B-7C3D810BB491         NaN  CalculatedCondition   \n",
-                            "17  E1897406-3D7D-4CFF-8908-21D047F7E484         NaN                Asset   \n",
-                            "18  EA112378-6507-481D-917F-3561F7614A60         NaN     CalculatedSignal   \n",
-                            "19  507F7690-5AF8-42DE-8261-672D0D18C8CB         NaN  CalculatedCondition   \n",
-                            "20  3BAA7860-6153-4C73-BFCC-D19AA4B6F7F4         NaN  CalculatedCondition   \n",
-                            "21  CE5CB4A8-BA17-48DA-B357-1BE876CDC751         NaN                Asset   \n",
-                            "22  E5B23C51-98DE-4BB9-8E20-516C31DE2D52         NaN     CalculatedSignal   \n",
-                            "23  14099FE4-0F7D-44C1-9311-088494EA3327         NaN                Asset   \n",
-                            "\n",
-                            "   Value Unit Of Measure Datasource Name Archived    Compressor  \\\n",
-                            "0                     kW    Example Data    False  Compressor 1   \n",
-                            "1                    NaN             NaN      NaN           NaN   \n",
-                            "2                    NaN             NaN      NaN           NaN   \n",
-                            "3                     kW    Example Data    False  Compressor 2   \n",
-                            "4                    NaN             NaN      NaN           NaN   \n",
-                            "5                    NaN             NaN      NaN           NaN   \n",
-                            "6                     \u00b0F    Example Data    False           NaN   \n",
-                            "7                    NaN             NaN      NaN           NaN   \n",
-                            "8                    NaN             NaN      NaN           NaN   \n",
-                            "9                    NaN             NaN      NaN           NaN   \n",
-                            "10                   NaN             NaN      NaN           NaN   \n",
-                            "11                   NaN             NaN      NaN           NaN   \n",
-                            "12                    kW    Example Data    False  Compressor 3   \n",
-                            "13                   NaN             NaN      NaN           NaN   \n",
-                            "14                   NaN             NaN      NaN           NaN   \n",
-                            "15                    kW    Example Data    False  Compressor 4   \n",
-                            "16                   NaN             NaN      NaN           NaN   \n",
-                            "17                   NaN             NaN      NaN           NaN   \n",
-                            "18                    \u00b0F    Example Data    False           NaN   \n",
-                            "19                   NaN             NaN      NaN           NaN   \n",
-                            "20                   NaN             NaN      NaN           NaN   \n",
-                            "21                   NaN             NaN      NaN           NaN   \n",
-                            "22                   NaN             NaN      NaN           NaN   \n",
-                            "23                   NaN             NaN      NaN           NaN   \n",
-                            "\n",
-                            "            Referenced Name Reference                              Name  ...  \\\n",
-                            "0   Area A_Compressor Power      True                             Power  ...   \n",
-                            "1                       NaN       NaN                        High Power  ...   \n",
-                            "2                       NaN       NaN  Other Compressors Are High Power  ...   \n",
-                            "3   Area B_Compressor Power      True                             Power  ...   \n",
-                            "4                       NaN       NaN                        High Power  ...   \n",
-                            "5                       NaN       NaN                      Compressor 2  ...   \n",
-                            "6        Area A_Temperature      True                       Temperature  ...   \n",
-                            "7                       NaN       NaN             Compressor High Power  ...   \n",
-                            "8                       NaN       NaN  Other Compressors Are High Power  ...   \n",
-                            "9                       NaN       NaN                      Compressor 1  ...   \n",
-                            "10                      NaN       NaN              Compressor Power Max  ...   \n",
-                            "11                      NaN       NaN                    Refrigerator 1  ...   \n",
-                            "12  Area C_Compressor Power      True                             Power  ...   \n",
-                            "13                      NaN       NaN                        High Power  ...   \n",
-                            "14                      NaN       NaN  Other Compressors Are High Power  ...   \n",
-                            "15  Area D_Compressor Power      True                             Power  ...   \n",
-                            "16                      NaN       NaN                        High Power  ...   \n",
-                            "17                      NaN       NaN                      Compressor 4  ...   \n",
-                            "18       Area C_Temperature      True                       Temperature  ...   \n",
-                            "19                      NaN       NaN             Compressor High Power  ...   \n",
-                            "20                      NaN       NaN  Other Compressors Are High Power  ...   \n",
-                            "21                      NaN       NaN                      Compressor 3  ...   \n",
-                            "22                      NaN       NaN              Compressor Power Max  ...   \n",
-                            "23                      NaN       NaN                    Refrigerator 2  ...   \n",
-                            "\n",
-                            "                                         Asset Object  \\\n",
-                            "0   Refrigerator Units >> Refrigerator 1 >> Compre...   \n",
-                            "1   Refrigerator Units >> Refrigerator 1 >> Compre...   \n",
-                            "2   Refrigerator Units >> Refrigerator 1 >> Compre...   \n",
-                            "3   Refrigerator Units >> Refrigerator 1 >> Compre...   \n",
-                            "4   Refrigerator Units >> Refrigerator 1 >> Compre...   \n",
-                            "5   Refrigerator Units >> Refrigerator 1 >> Compre...   \n",
-                            "6                Refrigerator Units >> Refrigerator 1   \n",
-                            "7                Refrigerator Units >> Refrigerator 1   \n",
-                            "8   Refrigerator Units >> Refrigerator 1 >> Compre...   \n",
-                            "9   Refrigerator Units >> Refrigerator 1 >> Compre...   \n",
-                            "10               Refrigerator Units >> Refrigerator 1   \n",
-                            "11               Refrigerator Units >> Refrigerator 1   \n",
-                            "12  Refrigerator Units >> Refrigerator 2 >> Compre...   \n",
-                            "13  Refrigerator Units >> Refrigerator 2 >> Compre...   \n",
-                            "14  Refrigerator Units >> Refrigerator 2 >> Compre...   \n",
-                            "15  Refrigerator Units >> Refrigerator 2 >> Compre...   \n",
-                            "16  Refrigerator Units >> Refrigerator 2 >> Compre...   \n",
-                            "17  Refrigerator Units >> Refrigerator 2 >> Compre...   \n",
-                            "18               Refrigerator Units >> Refrigerator 2   \n",
-                            "19               Refrigerator Units >> Refrigerator 2   \n",
-                            "20  Refrigerator Units >> Refrigerator 2 >> Compre...   \n",
-                            "21  Refrigerator Units >> Refrigerator 2 >> Compre...   \n",
-                            "22               Refrigerator Units >> Refrigerator 2   \n",
-                            "23               Refrigerator Units >> Refrigerator 2   \n",
-                            "\n",
-                            "                                    Path      Template Build Result  \\\n",
-                            "0   Refrigerator Units >> Refrigerator 1    Compressor      Success   \n",
-                            "1   Refrigerator Units >> Refrigerator 1    Compressor      Success   \n",
-                            "2   Refrigerator Units >> Refrigerator 1    Compressor      Success   \n",
-                            "3   Refrigerator Units >> Refrigerator 1    Compressor      Success   \n",
-                            "4   Refrigerator Units >> Refrigerator 1    Compressor      Success   \n",
-                            "5   Refrigerator Units >> Refrigerator 1    Compressor      Success   \n",
-                            "6                     Refrigerator Units  Refrigerator      Success   \n",
-                            "7                     Refrigerator Units  Refrigerator      Success   \n",
-                            "8   Refrigerator Units >> Refrigerator 1    Compressor      Success   \n",
-                            "9   Refrigerator Units >> Refrigerator 1    Compressor      Success   \n",
-                            "10                    Refrigerator Units  Refrigerator      Success   \n",
-                            "11                    Refrigerator Units  Refrigerator      Success   \n",
-                            "12  Refrigerator Units >> Refrigerator 2    Compressor      Success   \n",
-                            "13  Refrigerator Units >> Refrigerator 2    Compressor      Success   \n",
-                            "14  Refrigerator Units >> Refrigerator 2    Compressor      Success   \n",
-                            "15  Refrigerator Units >> Refrigerator 2    Compressor      Success   \n",
-                            "16  Refrigerator Units >> Refrigerator 2    Compressor      Success   \n",
-                            "17  Refrigerator Units >> Refrigerator 2    Compressor      Success   \n",
-                            "18                    Refrigerator Units  Refrigerator      Success   \n",
-                            "19                    Refrigerator Units  Refrigerator      Success   \n",
-                            "20  Refrigerator Units >> Refrigerator 2    Compressor      Success   \n",
-                            "21  Refrigerator Units >> Refrigerator 2    Compressor      Success   \n",
-                            "22                    Refrigerator Units  Refrigerator      Success   \n",
-                            "23                    Refrigerator Units  Refrigerator      Success   \n",
-                            "\n",
-                            "                                Formula  \\\n",
-                            "0                                   NaN   \n",
-                            "1   $a.valueSearch(isGreaterThan(20kW))   \n",
-                            "2                                   $p0   \n",
-                            "3                                   NaN   \n",
-                            "4   $a.valueSearch(isGreaterThan(20kW))   \n",
-                            "5                                   NaN   \n",
-                            "6                                   NaN   \n",
-                            "7                            $p0 or $p1   \n",
-                            "8                                   $p0   \n",
-                            "9                                   NaN   \n",
-                            "10                         $p0.max($p1)   \n",
-                            "11                                  NaN   \n",
-                            "12                                  NaN   \n",
-                            "13  $a.valueSearch(isGreaterThan(20kW))   \n",
-                            "14                                  $p0   \n",
-                            "15                                  NaN   \n",
-                            "16  $a.valueSearch(isGreaterThan(20kW))   \n",
-                            "17                                  NaN   \n",
-                            "18                                  NaN   \n",
-                            "19                           $p0 or $p1   \n",
-                            "20                                  $p0   \n",
-                            "21                                  NaN   \n",
-                            "22                         $p0.max($p1)   \n",
-                            "23                                  NaN   \n",
-                            "\n",
-                            "                                   Formula Parameters Datasource Class  \\\n",
-                            "0       [signal=7E99DB2D-AE68-43F9-99EE-BE4095976E94]    Seeq Data Lab   \n",
-                            "1            [a=9196030F-C4C8-4EED-A8A3-2FE5F6EEFEB0]    Seeq Data Lab   \n",
-                            "2           [p0=2ABA5770-D7AD-4861-8634-E31C96F9EC91]    Seeq Data Lab   \n",
-                            "3       [signal=C6BC4291-2606-465A-B6AE-5427CB8540D8]    Seeq Data Lab   \n",
-                            "4            [a=0FFCF13E-6AEB-4F3A-9958-E3D3AC1DA753]    Seeq Data Lab   \n",
-                            "5                                                 NaN    Seeq Data Lab   \n",
-                            "6       [signal=C1F1002A-469E-47D1-83AB-99FD17650B55]    Seeq Data Lab   \n",
-                            "7   [p0=2ABA5770-D7AD-4861-8634-E31C96F9EC91, p1=3...    Seeq Data Lab   \n",
-                            "8           [p0=3C236F11-67D1-4D69-8F02-7C382FAC809B]    Seeq Data Lab   \n",
-                            "9                                                 NaN    Seeq Data Lab   \n",
-                            "10  [p0=9196030F-C4C8-4EED-A8A3-2FE5F6EEFEB0, p1=0...    Seeq Data Lab   \n",
-                            "11                                                NaN    Seeq Data Lab   \n",
-                            "12      [signal=A531B8F4-E5C6-4114-BB62-646BCFBD9DA4]    Seeq Data Lab   \n",
-                            "13           [a=D665A3FF-6981-4928-A49E-ACCE530FED9C]    Seeq Data Lab   \n",
-                            "14          [p0=9DD37884-33B6-436D-B7D5-C90E9F183131]    Seeq Data Lab   \n",
-                            "15      [signal=87CB3E07-0568-4C53-A9A2-EDCD72CF8AC3]    Seeq Data Lab   \n",
-                            "16           [a=CB7E51A6-CE42-4FD4-BA65-7BD19E940251]    Seeq Data Lab   \n",
-                            "17                                                NaN    Seeq Data Lab   \n",
-                            "18      [signal=46E29219-3339-4F50-8137-C9C23B16DEF9]    Seeq Data Lab   \n",
-                            "19  [p0=9DD37884-33B6-436D-B7D5-C90E9F183131, p1=2...    Seeq Data Lab   \n",
-                            "20          [p0=2FA4345B-2B91-4F62-A72B-7C3D810BB491]    Seeq Data Lab   \n",
-                            "21                                                NaN    Seeq Data Lab   \n",
-                            "22  [p0=D665A3FF-6981-4928-A49E-ACCE530FED9C, p1=C...    Seeq Data Lab   \n",
-                            "23                                                NaN    Seeq Data Lab   \n",
-                            "\n",
-                            "    Datasource ID                                            Data ID  \\\n",
-                            "0   Seeq Data Lab  [807F13D7-C424-4840-B88B-D46F417A4966] {Signal...   \n",
-                            "1   Seeq Data Lab  [807F13D7-C424-4840-B88B-D46F417A4966] {Condit...   \n",
-                            "2   Seeq Data Lab  [807F13D7-C424-4840-B88B-D46F417A4966] {Condit...   \n",
-                            "3   Seeq Data Lab  [807F13D7-C424-4840-B88B-D46F417A4966] {Signal...   \n",
-                            "4   Seeq Data Lab  [807F13D7-C424-4840-B88B-D46F417A4966] {Condit...   \n",
-                            "5   Seeq Data Lab  [807F13D7-C424-4840-B88B-D46F417A4966] {Asset}...   \n",
-                            "6   Seeq Data Lab  [807F13D7-C424-4840-B88B-D46F417A4966] {Signal...   \n",
-                            "7   Seeq Data Lab  [807F13D7-C424-4840-B88B-D46F417A4966] {Condit...   \n",
-                            "8   Seeq Data Lab  [807F13D7-C424-4840-B88B-D46F417A4966] {Condit...   \n",
-                            "9   Seeq Data Lab  [807F13D7-C424-4840-B88B-D46F417A4966] {Asset}...   \n",
-                            "10  Seeq Data Lab  [807F13D7-C424-4840-B88B-D46F417A4966] {Signal...   \n",
-                            "11  Seeq Data Lab  [807F13D7-C424-4840-B88B-D46F417A4966] {Asset}...   \n",
-                            "12  Seeq Data Lab  [807F13D7-C424-4840-B88B-D46F417A4966] {Signal...   \n",
-                            "13  Seeq Data Lab  [807F13D7-C424-4840-B88B-D46F417A4966] {Condit...   \n",
-                            "14  Seeq Data Lab  [807F13D7-C424-4840-B88B-D46F417A4966] {Condit...   \n",
-                            "15  Seeq Data Lab  [807F13D7-C424-4840-B88B-D46F417A4966] {Signal...   \n",
-                            "16  Seeq Data Lab  [807F13D7-C424-4840-B88B-D46F417A4966] {Condit...   \n",
-                            "17  Seeq Data Lab  [807F13D7-C424-4840-B88B-D46F417A4966] {Asset}...   \n",
-                            "18  Seeq Data Lab  [807F13D7-C424-4840-B88B-D46F417A4966] {Signal...   \n",
-                            "19  Seeq Data Lab  [807F13D7-C424-4840-B88B-D46F417A4966] {Condit...   \n",
-                            "20  Seeq Data Lab  [807F13D7-C424-4840-B88B-D46F417A4966] {Condit...   \n",
-                            "21  Seeq Data Lab  [807F13D7-C424-4840-B88B-D46F417A4966] {Asset}...   \n",
-                            "22  Seeq Data Lab  [807F13D7-C424-4840-B88B-D46F417A4966] {Signal...   \n",
-                            "23  Seeq Data Lab  [807F13D7-C424-4840-B88B-D46F417A4966] {Asset}...   \n",
-                            "\n",
-                            "   Push Result  \n",
-                            "0      Success  \n",
-                            "1      Success  \n",
-                            "2      Success  \n",
-                            "3      Success  \n",
-                            "4      Success  \n",
-                            "5      Success  \n",
-                            "6      Success  \n",
-                            "7      Success  \n",
-                            "8      Success  \n",
-                            "9      Success  \n",
-                            "10     Success  \n",
-                            "11     Success  \n",
-                            "12     Success  \n",
-                            "13     Success  \n",
-                            "14     Success  \n",
-                            "15     Success  \n",
-                            "16     Success  \n",
-                            "17     Success  \n",
-                            "18     Success  \n",
-                            "19     Success  \n",
-                            "20     Success  \n",
-                            "21     Success  \n",
-                            "22     Success  \n",
-                            "23     Success  \n",
+                            "      Description                 Type Datasource Name Archived    Compressor  \\\n",
+                            "0.0           NaN     CalculatedSignal    Example Data    False  Compressor 2   \n",
+                            "1.0           NaN  CalculatedCondition             NaN      NaN           NaN   \n",
+                            "2.0           NaN  CalculatedCondition             NaN      NaN           NaN   \n",
+                            "3.0           NaN     CalculatedSignal    Example Data    False  Compressor 1   \n",
+                            "4.0           NaN  CalculatedCondition             NaN      NaN           NaN   \n",
+                            "5.0           NaN                Asset             NaN      NaN           NaN   \n",
+                            "6.0           NaN     CalculatedSignal    Example Data    False           NaN   \n",
+                            "7.0           NaN  CalculatedCondition             NaN      NaN           NaN   \n",
+                            "8.0           NaN  CalculatedCondition             NaN      NaN           NaN   \n",
+                            "9.0           NaN                Asset             NaN      NaN           NaN   \n",
+                            "10.0          NaN     CalculatedSignal             NaN      NaN           NaN   \n",
+                            "11.0          NaN                Asset             NaN      NaN           NaN   \n",
+                            "12.0          NaN     CalculatedSignal    Example Data    False  Compressor 3   \n",
+                            "13.0          NaN  CalculatedCondition             NaN      NaN           NaN   \n",
+                            "14.0          NaN  CalculatedCondition             NaN      NaN           NaN   \n",
+                            "15.0          NaN     CalculatedSignal    Example Data    False  Compressor 4   \n",
+                            "16.0          NaN  CalculatedCondition             NaN      NaN           NaN   \n",
+                            "17.0          NaN                Asset             NaN      NaN           NaN   \n",
+                            "18.0          NaN     CalculatedSignal    Example Data    False           NaN   \n",
+                            "19.0          NaN  CalculatedCondition             NaN      NaN           NaN   \n",
+                            "20.0          NaN  CalculatedCondition             NaN      NaN           NaN   \n",
+                            "21.0          NaN                Asset             NaN      NaN           NaN   \n",
+                            "22.0          NaN     CalculatedSignal             NaN      NaN           NaN   \n",
+                            "23.0          NaN                Asset             NaN      NaN           NaN   \n",
+                            "NaN           NaN                Asset             NaN      NaN           NaN   \n",
+                            "\n",
+                            "              Referenced Name Reference                              Name  \\\n",
+                            "0.0   Area B_Compressor Power      True                             Power   \n",
+                            "1.0                       NaN       NaN                        High Power   \n",
+                            "2.0                       NaN       NaN  Other Compressors Are High Power   \n",
+                            "3.0   Area A_Compressor Power      True                             Power   \n",
+                            "4.0                       NaN       NaN                        High Power   \n",
+                            "5.0                       NaN       NaN                      Compressor 1   \n",
+                            "6.0        Area A_Temperature      True                       Temperature   \n",
+                            "7.0                       NaN       NaN             Compressor High Power   \n",
+                            "8.0                       NaN       NaN  Other Compressors Are High Power   \n",
+                            "9.0                       NaN       NaN                      Compressor 2   \n",
+                            "10.0                      NaN       NaN              Compressor Power Max   \n",
+                            "11.0                      NaN       NaN                    Refrigerator 1   \n",
+                            "12.0  Area C_Compressor Power      True                             Power   \n",
+                            "13.0                      NaN       NaN                        High Power   \n",
+                            "14.0                      NaN       NaN  Other Compressors Are High Power   \n",
+                            "15.0  Area D_Compressor Power      True                             Power   \n",
+                            "16.0                      NaN       NaN                        High Power   \n",
+                            "17.0                      NaN       NaN                      Compressor 4   \n",
+                            "18.0       Area C_Temperature      True                       Temperature   \n",
+                            "19.0                      NaN       NaN             Compressor High Power   \n",
+                            "20.0                      NaN       NaN  Other Compressors Are High Power   \n",
+                            "21.0                      NaN       NaN                      Compressor 3   \n",
+                            "22.0                      NaN       NaN              Compressor Power Max   \n",
+                            "23.0                      NaN       NaN                    Refrigerator 2   \n",
+                            "NaN                       NaN       NaN                Refrigerator Units   \n",
+                            "\n",
+                            "                   Asset                                       Asset Object  \\\n",
+                            "0.0         Compressor 2  Refrigerator Units >> Refrigerator 1 >> Compre...   \n",
+                            "1.0         Compressor 2  Refrigerator Units >> Refrigerator 1 >> Compre...   \n",
+                            "2.0         Compressor 1  Refrigerator Units >> Refrigerator 1 >> Compre...   \n",
+                            "3.0         Compressor 1  Refrigerator Units >> Refrigerator 1 >> Compre...   \n",
+                            "4.0         Compressor 1  Refrigerator Units >> Refrigerator 1 >> Compre...   \n",
+                            "5.0         Compressor 1  Refrigerator Units >> Refrigerator 1 >> Compre...   \n",
+                            "6.0       Refrigerator 1               Refrigerator Units >> Refrigerator 1   \n",
+                            "7.0       Refrigerator 1               Refrigerator Units >> Refrigerator 1   \n",
+                            "8.0         Compressor 2  Refrigerator Units >> Refrigerator 1 >> Compre...   \n",
+                            "9.0         Compressor 2  Refrigerator Units >> Refrigerator 1 >> Compre...   \n",
+                            "10.0      Refrigerator 1               Refrigerator Units >> Refrigerator 1   \n",
+                            "11.0      Refrigerator 1               Refrigerator Units >> Refrigerator 1   \n",
+                            "12.0        Compressor 3  Refrigerator Units >> Refrigerator 2 >> Compre...   \n",
+                            "13.0        Compressor 3  Refrigerator Units >> Refrigerator 2 >> Compre...   \n",
+                            "14.0        Compressor 4  Refrigerator Units >> Refrigerator 2 >> Compre...   \n",
+                            "15.0        Compressor 4  Refrigerator Units >> Refrigerator 2 >> Compre...   \n",
+                            "16.0        Compressor 4  Refrigerator Units >> Refrigerator 2 >> Compre...   \n",
+                            "17.0        Compressor 4  Refrigerator Units >> Refrigerator 2 >> Compre...   \n",
+                            "18.0      Refrigerator 2               Refrigerator Units >> Refrigerator 2   \n",
+                            "19.0      Refrigerator 2               Refrigerator Units >> Refrigerator 2   \n",
+                            "20.0        Compressor 3  Refrigerator Units >> Refrigerator 2 >> Compre...   \n",
+                            "21.0        Compressor 3  Refrigerator Units >> Refrigerator 2 >> Compre...   \n",
+                            "22.0      Refrigerator 2               Refrigerator Units >> Refrigerator 2   \n",
+                            "23.0      Refrigerator 2               Refrigerator Units >> Refrigerator 2   \n",
+                            "NaN   Refrigerator Units                                                NaN   \n",
+                            "\n",
+                            "      ...                                 Formula Parameters Cache Enabled  \\\n",
+                            "0.0   ...      [signal=84ED2BB0-AD0B-4C76-8233-EEA7EB358F97]         False   \n",
+                            "1.0   ...           [a=215E4C66-6AEA-490A-8506-B8A556792999]           NaN   \n",
+                            "2.0   ...          [p0=5795BF85-79E1-4508-A084-ECA1B25B5990]         False   \n",
+                            "3.0   ...      [signal=B4213340-A80E-4FF1-B277-7408E99FEDFE]         False   \n",
+                            "4.0   ...           [a=85A9A341-ED97-44E3-9F0E-3D12A908F28A]           NaN   \n",
+                            "5.0   ...                                                NaN           NaN   \n",
+                            "6.0   ...      [signal=F8B2EF0E-BAB2-441D-B031-6F920099D74A]         False   \n",
+                            "7.0   ...  [p0=5795BF85-79E1-4508-A084-ECA1B25B5990, p1=2...           NaN   \n",
+                            "8.0   ...          [p0=24349142-C25B-4EE6-892C-AF6619FBD606]         False   \n",
+                            "9.0   ...                                                NaN           NaN   \n",
+                            "10.0  ...  [p0=215E4C66-6AEA-490A-8506-B8A556792999, p1=8...           NaN   \n",
+                            "11.0  ...                                                NaN           NaN   \n",
+                            "12.0  ...      [signal=954749C3-D3FF-4F10-9A2B-A5AF80E13E9D]         False   \n",
+                            "13.0  ...           [a=AB5138AE-3633-4A32-B324-C6F17630E27F]           NaN   \n",
+                            "14.0  ...          [p0=D3694232-C913-4503-A907-3AE71F102A00]         False   \n",
+                            "15.0  ...      [signal=30F8FDAF-293A-4C86-9179-A7CF7B1847B4]         False   \n",
+                            "16.0  ...           [a=A304B8D4-82DA-49BD-B383-C535CF04B3FD]           NaN   \n",
+                            "17.0  ...                                                NaN           NaN   \n",
+                            "18.0  ...      [signal=BDD6B3E7-6A62-4C43-AC60-4F6EF8525134]         False   \n",
+                            "19.0  ...  [p0=D3694232-C913-4503-A907-3AE71F102A00, p1=1...           NaN   \n",
+                            "20.0  ...          [p0=1BF05DD4-C85B-44CF-8A67-39029A54A2B7]         False   \n",
+                            "21.0  ...                                                NaN           NaN   \n",
+                            "22.0  ...  [p0=AB5138AE-3633-4A32-B324-C6F17630E27F, p1=A...           NaN   \n",
+                            "23.0  ...                                                NaN           NaN   \n",
+                            "NaN   ...                                                NaN           NaN   \n",
+                            "\n",
+                            "                             Referenced ID  \\\n",
+                            "0.0   84ED2BB0-AD0B-4C76-8233-EEA7EB358F97   \n",
+                            "1.0                                    NaN   \n",
+                            "2.0                                    NaN   \n",
+                            "3.0   B4213340-A80E-4FF1-B277-7408E99FEDFE   \n",
+                            "4.0                                    NaN   \n",
+                            "5.0                                    NaN   \n",
+                            "6.0   F8B2EF0E-BAB2-441D-B031-6F920099D74A   \n",
+                            "7.0                                    NaN   \n",
+                            "8.0                                    NaN   \n",
+                            "9.0                                    NaN   \n",
+                            "10.0                                   NaN   \n",
+                            "11.0                                   NaN   \n",
+                            "12.0  954749C3-D3FF-4F10-9A2B-A5AF80E13E9D   \n",
+                            "13.0                                   NaN   \n",
+                            "14.0                                   NaN   \n",
+                            "15.0  30F8FDAF-293A-4C86-9179-A7CF7B1847B4   \n",
+                            "16.0                                   NaN   \n",
+                            "17.0                                   NaN   \n",
+                            "18.0  BDD6B3E7-6A62-4C43-AC60-4F6EF8525134   \n",
+                            "19.0                                   NaN   \n",
+                            "20.0                                   NaN   \n",
+                            "21.0                                   NaN   \n",
+                            "22.0                                   NaN   \n",
+                            "23.0                                   NaN   \n",
+                            "NaN                                    NaN   \n",
+                            "\n",
+                            "                                 Scoped To Datasource Class  Datasource ID  \\\n",
+                            "0.0   90C07295-7D30-4DA6-8B5E-4DE3C7EF425C    Seeq Data Lab  Seeq Data Lab   \n",
+                            "1.0   90C07295-7D30-4DA6-8B5E-4DE3C7EF425C    Seeq Data Lab  Seeq Data Lab   \n",
+                            "2.0   90C07295-7D30-4DA6-8B5E-4DE3C7EF425C    Seeq Data Lab  Seeq Data Lab   \n",
+                            "3.0   90C07295-7D30-4DA6-8B5E-4DE3C7EF425C    Seeq Data Lab  Seeq Data Lab   \n",
+                            "4.0   90C07295-7D30-4DA6-8B5E-4DE3C7EF425C    Seeq Data Lab  Seeq Data Lab   \n",
+                            "5.0   90C07295-7D30-4DA6-8B5E-4DE3C7EF425C    Seeq Data Lab  Seeq Data Lab   \n",
+                            "6.0   90C07295-7D30-4DA6-8B5E-4DE3C7EF425C    Seeq Data Lab  Seeq Data Lab   \n",
+                            "7.0   90C07295-7D30-4DA6-8B5E-4DE3C7EF425C    Seeq Data Lab  Seeq Data Lab   \n",
+                            "8.0   90C07295-7D30-4DA6-8B5E-4DE3C7EF425C    Seeq Data Lab  Seeq Data Lab   \n",
+                            "9.0   90C07295-7D30-4DA6-8B5E-4DE3C7EF425C    Seeq Data Lab  Seeq Data Lab   \n",
+                            "10.0  90C07295-7D30-4DA6-8B5E-4DE3C7EF425C    Seeq Data Lab  Seeq Data Lab   \n",
+                            "11.0  90C07295-7D30-4DA6-8B5E-4DE3C7EF425C    Seeq Data Lab  Seeq Data Lab   \n",
+                            "12.0  90C07295-7D30-4DA6-8B5E-4DE3C7EF425C    Seeq Data Lab  Seeq Data Lab   \n",
+                            "13.0  90C07295-7D30-4DA6-8B5E-4DE3C7EF425C    Seeq Data Lab  Seeq Data Lab   \n",
+                            "14.0  90C07295-7D30-4DA6-8B5E-4DE3C7EF425C    Seeq Data Lab  Seeq Data Lab   \n",
+                            "15.0  90C07295-7D30-4DA6-8B5E-4DE3C7EF425C    Seeq Data Lab  Seeq Data Lab   \n",
+                            "16.0  90C07295-7D30-4DA6-8B5E-4DE3C7EF425C    Seeq Data Lab  Seeq Data Lab   \n",
+                            "17.0  90C07295-7D30-4DA6-8B5E-4DE3C7EF425C    Seeq Data Lab  Seeq Data Lab   \n",
+                            "18.0  90C07295-7D30-4DA6-8B5E-4DE3C7EF425C    Seeq Data Lab  Seeq Data Lab   \n",
+                            "19.0  90C07295-7D30-4DA6-8B5E-4DE3C7EF425C    Seeq Data Lab  Seeq Data Lab   \n",
+                            "20.0  90C07295-7D30-4DA6-8B5E-4DE3C7EF425C    Seeq Data Lab  Seeq Data Lab   \n",
+                            "21.0  90C07295-7D30-4DA6-8B5E-4DE3C7EF425C    Seeq Data Lab  Seeq Data Lab   \n",
+                            "22.0  90C07295-7D30-4DA6-8B5E-4DE3C7EF425C    Seeq Data Lab  Seeq Data Lab   \n",
+                            "23.0  90C07295-7D30-4DA6-8B5E-4DE3C7EF425C    Seeq Data Lab  Seeq Data Lab   \n",
+                            "NaN                                    NaN    Seeq Data Lab  Seeq Data Lab   \n",
+                            "\n",
+                            "                                                Data ID  \\\n",
+                            "0.0   [90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Signal...   \n",
+                            "1.0   [90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Condit...   \n",
+                            "2.0   [90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Condit...   \n",
+                            "3.0   [90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Signal...   \n",
+                            "4.0   [90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Condit...   \n",
+                            "5.0   [90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Asset}...   \n",
+                            "6.0   [90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Signal...   \n",
+                            "7.0   [90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Condit...   \n",
+                            "8.0   [90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Condit...   \n",
+                            "9.0   [90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Asset}...   \n",
+                            "10.0  [90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Signal...   \n",
+                            "11.0  [90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Asset}...   \n",
+                            "12.0  [90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Signal...   \n",
+                            "13.0  [90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Condit...   \n",
+                            "14.0  [90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Condit...   \n",
+                            "15.0  [90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Signal...   \n",
+                            "16.0  [90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Condit...   \n",
+                            "17.0  [90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Asset}...   \n",
+                            "18.0  [90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Signal...   \n",
+                            "19.0  [90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Condit...   \n",
+                            "20.0  [90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Condit...   \n",
+                            "21.0  [90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Asset}...   \n",
+                            "22.0  [90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Signal...   \n",
+                            "23.0  [90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Asset}...   \n",
+                            "NaN   [90C07295-7D30-4DA6-8B5E-4DE3C7EF425C] {Asset}...   \n",
+                            "\n",
+                            "                                        ID Push Result Value Unit Of Measure  \n",
+                            "0.0   215E4C66-6AEA-490A-8506-B8A556792999     Success                   NaN  \n",
+                            "1.0   5795BF85-79E1-4508-A084-ECA1B25B5990     Success                   NaN  \n",
+                            "2.0   C10C2EBF-092E-4232-AF25-BD2314FE1A3B     Success                   NaN  \n",
+                            "3.0   85A9A341-ED97-44E3-9F0E-3D12A908F28A     Success                   NaN  \n",
+                            "4.0   24349142-C25B-4EE6-892C-AF6619FBD606     Success                   NaN  \n",
+                            "5.0   FC49E623-638C-4244-B933-2F8D333215C1     Success                   NaN  \n",
+                            "6.0   AA8EDA7A-D704-477F-B67F-E4181B380326     Success                   NaN  \n",
+                            "7.0   7997B9B7-5093-473B-8A5A-2A7AD1EA306E     Success                   NaN  \n",
+                            "8.0   E7884BC1-869A-46C4-9F23-C6324A75B979     Success                   NaN  \n",
+                            "9.0   191E9995-AC0A-49B0-B0F6-5EABF34B32E0     Success                   NaN  \n",
+                            "10.0  FEF4DC7E-7629-40F1-815A-8B4901F10711     Success                   NaN  \n",
+                            "11.0  8BD6ECFB-A7CD-40AF-9AA7-C4B4B00707E0     Success                   NaN  \n",
+                            "12.0  AB5138AE-3633-4A32-B324-C6F17630E27F     Success                   NaN  \n",
+                            "13.0  D3694232-C913-4503-A907-3AE71F102A00     Success                   NaN  \n",
+                            "14.0  C3B9D73B-78B1-4136-9351-B395252BEECD     Success                   NaN  \n",
+                            "15.0  A304B8D4-82DA-49BD-B383-C535CF04B3FD     Success                   NaN  \n",
+                            "16.0  1BF05DD4-C85B-44CF-8A67-39029A54A2B7     Success                   NaN  \n",
+                            "17.0  392B154B-C3A2-40DA-8A2C-F54EB03D0EF7     Success                   NaN  \n",
+                            "18.0  AE1D3114-FC56-4D85-A17E-AECB3001761C     Success                   NaN  \n",
+                            "19.0  1EBB4BD4-2778-4D86-9623-6041F17DA282     Success                   NaN  \n",
+                            "20.0  17B175B4-859F-4C5C-B21F-18AA174A1EB6     Success                   NaN  \n",
+                            "21.0  99107DAE-E79D-4564-8B0A-BC1390C67F28     Success                   NaN  \n",
+                            "22.0  7C1592C9-94AB-4E7F-A379-8A40B5A57EF6     Success                   NaN  \n",
+                            "23.0  A188AAA6-4C8A-4829-962E-55AA3DCBC77D     Success                   NaN  \n",
+                            "NaN   240448CA-0624-47FC-A6D1-1559F59A8FC5     Success                   NaN  \n",
                             "\n",
-                            "[24 rows x 21 columns]"
+                            "[25 rows x 24 columns]"
                         ]
                     },
                     "execution_count": 12,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -4253,15 +4463,15 @@
             "cell_type": "code",
             "execution_count": 14,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<div style=\"background-color: #EEFFEE;color:black;text-align: left;\">Pushed successfully to datasource <strong>Seeq Data Lab [Datasource ID: Seeq Data Lab]</strong> and scoped to workbook ID <strong>807F13D7-C424-4840-B88B-D46F417A4966</strong><br>Click the following link to see what you pushed in Seeq:<br><a href=\"http://localhost:34216/28420AC3-152B-47A0-ACB7-6B060C3338FD/workbook/807F13D7-C424-4840-B88B-D46F417A4966/worksheet/C8375B1E-7DE2-44A6-BE3F-CA24281D6B72\" target=\"_new\">http://localhost:34216/28420AC3-152B-47A0-ACB7-6B060C3338FD/workbook/807F13D7-C424-4840-B88B-D46F417A4966/worksheet/C8375B1E-7DE2-44A6-BE3F-CA24281D6B72</a></div>"
+                            "<div style=\"background-color: #EEFFEE;color:black; text-align: left;\">Pushed successfully to datasource <strong>Seeq Data Lab [Datasource ID: Seeq Data Lab]</strong> and scoped to workbook ID <strong>90C07295-7D30-4DA6-8B5E-4DE3C7EF425C</strong><br>Click the following link to see what you pushed in Seeq:<br><a href=\"http://localhost:34216/5F85F903-0ED4-42B1-8B9E-418718482532/workbook/90C07295-7D30-4DA6-8B5E-4DE3C7EF425C/worksheet/5B3A24A6-1ABF-4403-BD0B-28669B4A60BF\" target=\"_new\">http://localhost:34216/5F85F903-0ED4-42B1-8B9E-418718482532/workbook/90C07295-7D30-4DA6-8B5E-4DE3C7EF425C/worksheet/5B3A24A6-1ABF-4403-BD0B-28669B4A60BF</a></div>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -4301,15 +4511,15 @@
             "cell_type": "code",
             "execution_count": 15,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<div style=\"background-color: #EEFFEE;color:black;text-align: left;\">Successfully built 1 assets and 1 attributes.</div><table style=\"color:black;\"><tr><td style=\"background-color: #EEFFEE;\"></td><td style=\"background-color: #EEFFEE; text-align: left;\">Build Path</td><td style=\"background-color: #EEFFEE; text-align: left;\">Build Asset</td><td style=\"background-color: #EEFFEE; text-align: left;\">Build Template</td><td style=\"background-color: #EEFFEE; text-align: left;\">Build Result</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">0</td><td style=\"text-align: left; vertical-align: top;\">Debugging Example</td><td style=\"text-align: left; vertical-align: top;\">Debugging Area A</td><td style=\"text-align: left; vertical-align: top;\">DebuggingExample</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr></table>"
+                            "<div style=\"background-color: #EEFFEE;color:black; text-align: left;\">Successfully built 1 assets and 1 attributes.</div><table class=\"tex2jax_ignore\" style=\"color:black;\"><tr><td style=\"background-color: #EEFFEE;\"></td><td style=\"background-color: #EEFFEE; text-align: left;\">Build Path</td><td style=\"background-color: #EEFFEE; text-align: left;\">Build Asset</td><td style=\"background-color: #EEFFEE; text-align: left;\">Build Template</td><td style=\"background-color: #EEFFEE; text-align: left;\">Build Result</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">0</td><td style=\"text-align: left; vertical-align: top;\">Debugging Example</td><td style=\"text-align: left; vertical-align: top;\">Debugging Area A</td><td style=\"text-align: left; vertical-align: top;\">DebuggingExample</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr></table>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -4379,15 +4589,15 @@
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Help on function build in module seeq.spy.assets._build:\n",
                         "\n",
-                        "build(model, metadata, errors='catalog', quiet=False, status: seeq.spy._status.Status = None)\n",
+                        "build(model, metadata, *, workbooks=None, errors='catalog', quiet=None, status: 'Status' = None)\n",
                         "    Utilizes a Python Class-based asset model specification to produce a set\n",
                         "    of item definitions as a metadata DataFrame.\n",
                         "    \n",
                         "    Parameters\n",
                         "    ----------\n",
                         "    model : {ModuleType, type, List[type]}\n",
                         "        A Python module, a spy.assets.Asset or list of spy.asset.Assets to\n",
@@ -4397,20 +4607,25 @@
                         "    \n",
                         "    metadata : {pd.DataFrame}\n",
                         "        The metadata DataFrame, usually produced from calls to spy.search(),\n",
                         "        that will be used as the \"ingredients\" for the asset tree and passed\n",
                         "        into all Asset.Attribute() and Asset.Component() decorated class\n",
                         "        functions.\n",
                         "    \n",
+                        "    workbooks : {list}\n",
+                        "        The set of workbooks (usually a single AnalysisTemplate object and\n",
+                        "        one or more TopicTemplate objects) to be used in @Display and\n",
+                        "        @Document functions.\n",
+                        "    \n",
                         "    errors : {'raise', 'catalog'}, default 'catalog'\n",
                         "        If 'raise', any errors encountered will cause an exception. If\n",
                         "        'catalog', errors will be added to a 'Result' column in the status.df\n",
                         "        DataFrame.\n",
                         "    \n",
-                        "    quiet : bool\n",
+                        "    quiet : bool, default False\n",
                         "        If True, suppresses progress output.\n",
                         "    \n",
                         "    status : spy.Status, optional\n",
                         "        If specified, the supplied Status object will be updated as the command\n",
                         "        progresses. It gets filled in with the same information you would see\n",
                         "        in Jupyter in the blue/green/red table below your code while the\n",
                         "        command is executed. The table itself is accessible as a DataFrame via\n",
```

### Comparing `seeq-spy-187.5/seeq/spy/docs/Documentation/Asset Trees 3 - Report and Dashboard Templates.ipynb` & `seeq-spy-188.0/seeq/spy/docs/Documentation/Asset Trees 3 - Report and Dashboard Templates.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9993895686313607%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(1, 'from seeq import spy\\n'), (2, '\\n'), (3, '# Set the "*

 * *            'compatibility option so that you maximize the chance that SPy will remain compatible '*

 * *            "with your notebook/script\\n'), (4, 'spy.options.compatibility = 188')], delete: "*

 * *            "[1]}}, 1: {'outputs': {0: {'data': {'text/html': ['<div "*

 * *            'style="background-color: #EEFFEE;color:black; text-align: left;">Logged in to '*

 * *            '<strong>http://localhost:34216</strong>  […]*

```diff
@@ -7,30 +7,33 @@
                 "pycharm": {
                     "name": "#%%\n"
                 }
             },
             "outputs": [],
             "source": [
                 "import numpy as np\n",
-                "from seeq import spy"
+                "from seeq import spy\n",
+                "\n",
+                "# Set the compatibility option so that you maximize the chance that SPy will remain compatible with your notebook/script\n",
+                "spy.options.compatibility = 188"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {
                 "pycharm": {
                     "name": "#%%\n"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<div style=\"background-color: #EEFFEE;color:black; text-align: left;\">Logged in to <strong>http://localhost:34216</strong> successfully as <strong>agent_api_key</strong>.<br>Seeq Server Version: <strong>R59.0.0-SNAPSHOT</strong><br>Seeq Python Module Version: <strong>59.0.0.183.31</strong></div>"
+                            "<div style=\"background-color: #EEFFEE;color:black; text-align: left;\">Logged in to <strong>http://localhost:34216</strong> successfully as <strong>agent_api_key</strong>.<br>Seeq Server Version: <strong>R61.0.0-SNAPSHOT</strong><br>Seeq Python Module Version: <strong>61.0.0.184.25</strong></div>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -85,15 +88,15 @@
                     "name": "#%%\n"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<div style=\"background-color: #EEFFEE;color:black; text-align: left;\">Query successful</div><table class=\"tex2jax_ignore\" style=\"color:black;\"><tr><td style=\"background-color: #EEFFEE;\"></td><td style=\"background-color: #EEFFEE; text-align: left;\">Name</td><td style=\"background-color: #EEFFEE; text-align: left;\">Datasource Name</td><td style=\"background-color: #EEFFEE; text-align: left;\">Time</td><td style=\"background-color: #EEFFEE; text-align: right;\">Count</td><td style=\"background-color: #EEFFEE; text-align: right;\">Pages</td><td style=\"background-color: #EEFFEE; text-align: left;\">Result</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">0</td><td style=\"text-align: left; vertical-align: top;\">/Area [ABCDEG]_.*/</td><td style=\"text-align: left; vertical-align: top;\">Example Data</td><td style=\"vertical-align: top;\">00:00:00.04</td><td style=\"text-align: right; vertical-align: top;\">37</td><td style=\"text-align: right; vertical-align: top;\">1</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr></table>"
+                            "<div style=\"background-color: #EEFFEE;color:black; text-align: left;\">Query successful</div><table class=\"tex2jax_ignore\" style=\"color:black;\"><tr><td style=\"background-color: #EEFFEE;\"></td><td style=\"background-color: #EEFFEE; text-align: left;\">Name</td><td style=\"background-color: #EEFFEE; text-align: left;\">Datasource Name</td><td style=\"background-color: #EEFFEE; text-align: left;\">Time</td><td style=\"background-color: #EEFFEE; text-align: right;\">Count</td><td style=\"background-color: #EEFFEE; text-align: right;\">Pages</td><td style=\"background-color: #EEFFEE; text-align: left;\">Result</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">0</td><td style=\"text-align: left; vertical-align: top;\">/Area [ABCDEG]_.*/</td><td style=\"text-align: left; vertical-align: top;\">Example Data</td><td style=\"vertical-align: top;\">00:00:00.03</td><td style=\"text-align: right; vertical-align: top;\">37</td><td style=\"text-align: right; vertical-align: top;\">1</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr></table>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -131,71 +134,71 @@
                             "      <th>Facility</th>\n",
                             "      <th>Section</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
-                            "      <td>C99DC733-7788-4A8E-B725-8A6AB8C09C9C</td>\n",
+                            "      <td>B4213340-A80E-4FF1-B277-7408E99FEDFE</td>\n",
                             "      <td>Area A_Compressor Power</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
                             "      <td>kW</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
                             "      <td>None</td>\n",
                             "      <td>North America</td>\n",
                             "      <td>Facility 1</td>\n",
                             "      <td>Section A</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1</th>\n",
-                            "      <td>20C8D2AB-F43F-4CAD-9ACA-C76FBC02D2B2</td>\n",
+                            "      <td>DCA902F6-237D-4275-9669-1EF840ADB5D9</td>\n",
                             "      <td>Area A_Compressor Stage</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
                             "      <td>string</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
                             "      <td>None</td>\n",
                             "      <td>North America</td>\n",
                             "      <td>Facility 1</td>\n",
                             "      <td>Section A</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2</th>\n",
-                            "      <td>49881528-AB1E-4895-9596-31911B99A896</td>\n",
+                            "      <td>DC8A0F6F-12B4-4DA9-8815-0D2F6AEDA0CF</td>\n",
                             "      <td>Area A_Optimizer</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
                             "      <td>None</td>\n",
                             "      <td>North America</td>\n",
                             "      <td>Facility 1</td>\n",
                             "      <td>Section A</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>3</th>\n",
-                            "      <td>E81C6B0A-5D1A-4815-AA13-D6A2C3A73BFB</td>\n",
+                            "      <td>E9744446-848A-4461-A730-29CD0C97A7DC</td>\n",
                             "      <td>Area A_Relative Humidity</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
                             "      <td>%</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
                             "      <td>None</td>\n",
                             "      <td>North America</td>\n",
                             "      <td>Facility 1</td>\n",
                             "      <td>Section A</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>4</th>\n",
-                            "      <td>65AD165E-658B-4A7B-9582-4E0FDB5DE774</td>\n",
+                            "      <td>F8B2EF0E-BAB2-441D-B031-6F920099D74A</td>\n",
                             "      <td>Area A_Temperature</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
                             "      <td>\u00b0F</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
                             "      <td>None</td>\n",
@@ -205,19 +208,19 @@
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
                             "                                     ID                      Name  \\\n",
-                            "0  C99DC733-7788-4A8E-B725-8A6AB8C09C9C   Area A_Compressor Power   \n",
-                            "1  20C8D2AB-F43F-4CAD-9ACA-C76FBC02D2B2   Area A_Compressor Stage   \n",
-                            "2  49881528-AB1E-4895-9596-31911B99A896          Area A_Optimizer   \n",
-                            "3  E81C6B0A-5D1A-4815-AA13-D6A2C3A73BFB  Area A_Relative Humidity   \n",
-                            "4  65AD165E-658B-4A7B-9582-4E0FDB5DE774        Area A_Temperature   \n",
+                            "0  B4213340-A80E-4FF1-B277-7408E99FEDFE   Area A_Compressor Power   \n",
+                            "1  DCA902F6-237D-4275-9669-1EF840ADB5D9   Area A_Compressor Stage   \n",
+                            "2  DC8A0F6F-12B4-4DA9-8815-0D2F6AEDA0CF          Area A_Optimizer   \n",
+                            "3  E9744446-848A-4461-A730-29CD0C97A7DC  Area A_Relative Humidity   \n",
+                            "4  F8B2EF0E-BAB2-441D-B031-6F920099D74A        Area A_Temperature   \n",
                             "\n",
                             "   Description          Type Value Unit Of Measure Datasource Name  Archived  \\\n",
                             "0          NaN  StoredSignal                    kW    Example Data     False   \n",
                             "1          NaN  StoredSignal                string    Example Data     False   \n",
                             "2          NaN  StoredSignal                   NaN    Example Data     False   \n",
                             "3          NaN  StoredSignal                     %    Example Data     False   \n",
                             "4          NaN  StoredSignal                    \u00b0F    Example Data     False   \n",
@@ -403,15 +406,15 @@
                             "      <th>Template</th>\n",
                             "      <th>Build Result</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
-                            "      <td>C99DC733-7788-4A8E-B725-8A6AB8C09C9C</td>\n",
+                            "      <td>B4213340-A80E-4FF1-B277-7408E99FEDFE</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
                             "      <td>kW</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
                             "      <td>Facility 1</td>\n",
                             "      <td>Section A</td>\n",
@@ -422,15 +425,15 @@
                             "      <td>North America &gt;&gt; Facility 1 &gt;&gt; Section A</td>\n",
                             "      <td>North America &gt;&gt; Facility 1</td>\n",
                             "      <td>Section</td>\n",
                             "      <td>Success</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1</th>\n",
-                            "      <td>E81C6B0A-5D1A-4815-AA13-D6A2C3A73BFB</td>\n",
+                            "      <td>E9744446-848A-4461-A730-29CD0C97A7DC</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
                             "      <td>%</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
                             "      <td>Facility 1</td>\n",
                             "      <td>Section A</td>\n",
@@ -441,15 +444,15 @@
                             "      <td>North America &gt;&gt; Facility 1 &gt;&gt; Section A</td>\n",
                             "      <td>North America &gt;&gt; Facility 1</td>\n",
                             "      <td>Section</td>\n",
                             "      <td>Success</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2</th>\n",
-                            "      <td>65AD165E-658B-4A7B-9582-4E0FDB5DE774</td>\n",
+                            "      <td>F8B2EF0E-BAB2-441D-B031-6F920099D74A</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
                             "      <td>\u00b0F</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
                             "      <td>Facility 1</td>\n",
                             "      <td>Section A</td>\n",
@@ -479,15 +482,15 @@
                             "      <td>North America &gt;&gt; Facility 1 &gt;&gt; Section A</td>\n",
                             "      <td>North America &gt;&gt; Facility 1</td>\n",
                             "      <td>Section</td>\n",
                             "      <td>Success</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>4</th>\n",
-                            "      <td>16F15E5F-4370-4E53-9F05-C9B7C32DA4B5</td>\n",
+                            "      <td>84ED2BB0-AD0B-4C76-8233-EEA7EB358F97</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
                             "      <td>kW</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
                             "      <td>Facility 1</td>\n",
                             "      <td>Section B</td>\n",
@@ -502,19 +505,19 @@
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
                             "                                     ID  Description          Type  \\\n",
-                            "0  C99DC733-7788-4A8E-B725-8A6AB8C09C9C          NaN  StoredSignal   \n",
-                            "1  E81C6B0A-5D1A-4815-AA13-D6A2C3A73BFB          NaN  StoredSignal   \n",
-                            "2  65AD165E-658B-4A7B-9582-4E0FDB5DE774          NaN  StoredSignal   \n",
+                            "0  B4213340-A80E-4FF1-B277-7408E99FEDFE          NaN  StoredSignal   \n",
+                            "1  E9744446-848A-4461-A730-29CD0C97A7DC          NaN  StoredSignal   \n",
+                            "2  F8B2EF0E-BAB2-441D-B031-6F920099D74A          NaN  StoredSignal   \n",
                             "3                                   NaN          NaN         Asset   \n",
-                            "4  16F15E5F-4370-4E53-9F05-C9B7C32DA4B5          NaN  StoredSignal   \n",
+                            "4  84ED2BB0-AD0B-4C76-8233-EEA7EB358F97          NaN  StoredSignal   \n",
                             "\n",
                             "  Value Unit Of Measure Datasource Name Archived    Facility    Section  \\\n",
                             "0                    kW    Example Data    False  Facility 1  Section A   \n",
                             "1                     %    Example Data    False  Facility 1  Section A   \n",
                             "2                    \u00b0F    Example Data    False  Facility 1  Section A   \n",
                             "3                   NaN             NaN      NaN         NaN        NaN   \n",
                             "4                    kW    Example Data    False  Facility 1  Section B   \n",
@@ -570,15 +573,15 @@
                     "name": "#%%\n"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<div style=\"background-color: #EEFFEE;color:black; text-align: left;\">Pushed successfully to datasource <strong>Seeq Data Lab [Datasource ID: Seeq Data Lab]</strong> and scoped to workbook ID <strong>707E6B09-9100-4F37-AD0A-5256B58357A9</strong><br>Click the following link to see what you pushed in Seeq:<br><a href=\"http://localhost:34216/6E172858-A7E3-4DE8-9D83-B6BF6DA718E4/workbook/707E6B09-9100-4F37-AD0A-5256B58357A9/worksheet/A8E6BF75-F76A-4084-9833-BC53C6E5FF91\" target=\"_new\">http://localhost:34216/6E172858-A7E3-4DE8-9D83-B6BF6DA718E4/workbook/707E6B09-9100-4F37-AD0A-5256B58357A9/worksheet/A8E6BF75-F76A-4084-9833-BC53C6E5FF91</a></div>"
+                            "<div style=\"background-color: #EEFFEE;color:black; text-align: left;\">Pushed successfully to datasource <strong>Seeq Data Lab [Datasource ID: Seeq Data Lab]</strong> and scoped to workbook ID <strong>C3F1C862-FDE2-43B9-9BB6-54FE75DCC795</strong><br>Click the following link to see what you pushed in Seeq:<br><a href=\"http://localhost:34216/5F85F903-0ED4-42B1-8B9E-418718482532/workbook/C3F1C862-FDE2-43B9-9BB6-54FE75DCC795/worksheet/C0525556-6AFE-407A-B298-B0A808DADF88\" target=\"_new\">http://localhost:34216/5F85F903-0ED4-42B1-8B9E-418718482532/workbook/C3F1C862-FDE2-43B9-9BB6-54FE75DCC795/worksheet/C0525556-6AFE-407A-B298-B0A808DADF88</a></div>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -623,17 +626,17 @@
                     "output_type": "display_data"
                 },
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "worksheet.parameters = {\n",
-                        "    \"E97BBE1D-F227-4AD7-ADAC-15B54FC50DB3 [Signal] Example >> Cooling Tower 1 >> Area A >> Compressor Power\": None,\n",
                         "    \"8A4F0E26-8A0C-4127-9E11-B67E031C6049 [Signal] Example >> Cooling Tower 1 >> Area A >> Temperature\": None,\n",
-                        "    \"4B40EAFC-91ED-4AB0-8199-F21AF40A8350 [Asset] Example >> Area A\": None,\n",
+                        "    \"E97BBE1D-F227-4AD7-ADAC-15B54FC50DB3 [Signal] Example >> Cooling Tower 1 >> Area A >> Compressor Power\": None,\n",
+                        "    \"4B40EAFC-91ED-4AB0-8199-F21AF40A8350 [Asset] Example >> Cooling Tower 1 >> Area A\": None,\n",
                         "    \"B9CDE282-7A1A-4E28-A173-12E7347AB891 [Signal] Example >> Cooling Tower 1 >> Area A >> Relative Humidity\": None\n",
                         "}\n"
                     ]
                 }
             ],
             "source": [
                 "workbooks = spy.workbooks.load('./Support Files/Report and Dashboard Templates.zip',\n",
@@ -754,15 +757,15 @@
                     "name": "#%%\n"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<div style=\"background-color: #EEFFEE;color:black; text-align: left;\">Pushed successfully to datasource <strong>Seeq Data Lab [Datasource ID: Seeq Data Lab]</strong> and scoped to workbook ID <strong>707E6B09-9100-4F37-AD0A-5256B58357A9</strong><br>Click the following link to see what you pushed in Seeq:<br><a href=\"http://localhost:34216/6E172858-A7E3-4DE8-9D83-B6BF6DA718E4/workbook/707E6B09-9100-4F37-AD0A-5256B58357A9/worksheet/A8E6BF75-F76A-4084-9833-BC53C6E5FF91\" target=\"_new\">http://localhost:34216/6E172858-A7E3-4DE8-9D83-B6BF6DA718E4/workbook/707E6B09-9100-4F37-AD0A-5256B58357A9/worksheet/A8E6BF75-F76A-4084-9833-BC53C6E5FF91</a></div>"
+                            "<div style=\"background-color: #EEFFEE;color:black; text-align: left;\">Pushed successfully to datasource <strong>Seeq Data Lab [Datasource ID: Seeq Data Lab]</strong> and scoped to workbook ID <strong>C3F1C862-FDE2-43B9-9BB6-54FE75DCC795</strong><br>Click the following link to see what you pushed in Seeq:<br><a href=\"http://localhost:34216/5F85F903-0ED4-42B1-8B9E-418718482532/workbook/C3F1C862-FDE2-43B9-9BB6-54FE75DCC795/worksheet/C0525556-6AFE-407A-B298-B0A808DADF88\" target=\"_new\">http://localhost:34216/5F85F903-0ED4-42B1-8B9E-418718482532/workbook/C3F1C862-FDE2-43B9-9BB6-54FE75DCC795/worksheet/C0525556-6AFE-407A-B298-B0A808DADF88</a></div>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -868,15 +871,15 @@
                     "name": "#%%\n"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<div style=\"background-color: #EEFFEE;color:black; text-align: left;\">Push successful</div><table class=\"tex2jax_ignore\" style=\"color:black;\"><tr><td style=\"background-color: #EEFFEE;\"></td><td style=\"background-color: #EEFFEE; text-align: left;\">ID</td><td style=\"background-color: #EEFFEE; text-align: left;\">Name</td><td style=\"background-color: #EEFFEE; text-align: left;\">Type</td><td style=\"background-color: #EEFFEE; text-align: left;\">Workbook Type</td><td style=\"background-color: #EEFFEE; text-align: left;\">Count</td><td style=\"background-color: #EEFFEE; text-align: left;\">Time</td><td style=\"background-color: #EEFFEE; text-align: left;\">Result</td><td style=\"background-color: #EEFFEE; text-align: left;\">Pushed Workbook ID</td><td style=\"background-color: #EEFFEE; text-align: left;\">URL</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">0</td><td style=\"text-align: left; vertical-align: top;\">707E6B09-9100-4F37-AD0A-5256B58357A9</td><td style=\"text-align: left; vertical-align: top;\">Report and Dashboard Templates</td><td style=\"text-align: left; vertical-align: top;\">Workbook</td><td style=\"text-align: left; vertical-align: top;\">Analysis</td><td style=\"text-align: right; vertical-align: top;\">32</td><td style=\"vertical-align: top;\">00:00:01.01</td><td style=\"text-align: left; vertical-align: top;\">Success</td><td style=\"text-align: left; vertical-align: top;\">707E6B09-9100-4F37-AD0A-5256B58357A9</td><td style=\"text-align: left; vertical-align: top;\"><a target=\"_blank\" href=\"http://localhost:34216/6E172858-A7E3-4DE8-9D83-B6BF6DA718E4/workbook/707E6B09-9100-4F37-AD0A-5256B58357A9/worksheet/CA8FD71A-AEA7-454B-8480-9EF01B23C167\">link</a></td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">1</td><td style=\"text-align: left; vertical-align: top;\">14079DF9-319F-4181-AEC1-9A4D48EF310B agent_api_key Report and Dashboard Templates Example 1</td><td style=\"text-align: left; vertical-align: top;\">Report and Dashboard Templates</td><td style=\"text-align: left; vertical-align: top;\">Workbook</td><td style=\"text-align: left; vertical-align: top;\">Topic</td><td style=\"text-align: right; vertical-align: top;\">6</td><td style=\"vertical-align: top;\">00:00:00.67</td><td style=\"text-align: left; vertical-align: top;\">Success</td><td style=\"text-align: left; vertical-align: top;\">1B6ACC84-D56D-44D1-8F7E-58B864A9996E</td><td style=\"text-align: left; vertical-align: top;\"><a target=\"_blank\" href=\"http://localhost:34216/6E172858-A7E3-4DE8-9D83-B6BF6DA718E4/workbook/1B6ACC84-D56D-44D1-8F7E-58B864A9996E/worksheet/CFE7433E-0C55-487E-A54E-468654FE49E8\">link</a></td></tr></table>"
+                            "<div style=\"background-color: #EEFFEE;color:black; text-align: left;\">Push successful</div><table class=\"tex2jax_ignore\" style=\"color:black;\"><tr><td style=\"background-color: #EEFFEE;\"></td><td style=\"background-color: #EEFFEE; text-align: left;\">ID</td><td style=\"background-color: #EEFFEE; text-align: left;\">Name</td><td style=\"background-color: #EEFFEE; text-align: left;\">Type</td><td style=\"background-color: #EEFFEE; text-align: left;\">Workbook Type</td><td style=\"background-color: #EEFFEE; text-align: left;\">Count</td><td style=\"background-color: #EEFFEE; text-align: left;\">Time</td><td style=\"background-color: #EEFFEE; text-align: left;\">Result</td><td style=\"background-color: #EEFFEE; text-align: left;\">Pushed Workbook ID</td><td style=\"background-color: #EEFFEE; text-align: left;\">URL</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">0</td><td style=\"text-align: left; vertical-align: top;\">C3F1C862-FDE2-43B9-9BB6-54FE75DCC795</td><td style=\"text-align: left; vertical-align: top;\">Report and Dashboard Templates</td><td style=\"text-align: left; vertical-align: top;\">Workbook</td><td style=\"text-align: left; vertical-align: top;\">Analysis</td><td style=\"text-align: right; vertical-align: top;\">32</td><td style=\"vertical-align: top;\">00:00:01.25</td><td style=\"text-align: left; vertical-align: top;\">Success</td><td style=\"text-align: left; vertical-align: top;\">C3F1C862-FDE2-43B9-9BB6-54FE75DCC795</td><td style=\"text-align: left; vertical-align: top;\"><a target=\"_blank\" href=\"http://localhost:34216/5F85F903-0ED4-42B1-8B9E-418718482532/workbook/C3F1C862-FDE2-43B9-9BB6-54FE75DCC795/worksheet/78CB89C7-2CF1-4DC2-AA81-B50CE805DC89\">link</a></td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">1</td><td style=\"text-align: left; vertical-align: top;\">14079DF9-319F-4181-AEC1-9A4D48EF310B agent_api_key Report and Dashboard Templates Example 1</td><td style=\"text-align: left; vertical-align: top;\">Report and Dashboard Templates</td><td style=\"text-align: left; vertical-align: top;\">Workbook</td><td style=\"text-align: left; vertical-align: top;\">Topic</td><td style=\"text-align: right; vertical-align: top;\">6</td><td style=\"vertical-align: top;\">00:00:00.71</td><td style=\"text-align: left; vertical-align: top;\">Success</td><td style=\"text-align: left; vertical-align: top;\">28CAA57B-5683-494D-B464-E0E82A468FBE</td><td style=\"text-align: left; vertical-align: top;\"><a target=\"_blank\" href=\"http://localhost:34216/5F85F903-0ED4-42B1-8B9E-418718482532/workbook/28CAA57B-5683-494D-B464-E0E82A468FBE/worksheet/FCF3BFD3-6AB5-42D8-9340-C47E16940904\">link</a></td></tr></table>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
```

### Comparing `seeq-spy-187.5/seeq/spy/docs/Documentation/Asset Trees 4 - Accelerator Templates.ipynb` & `seeq-spy-188.0/seeq/spy/docs/Documentation/Asset Trees 4 - Accelerator Templates.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9973848914565826%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(3, 'import numpy as np\\n'), (4, '\\n'), (5, '# Set the "*

 * *            'compatibility option so that you maximize the chance that SPy will remain compatible '*

 * *            "with your notebook/script\\n'), (6, 'spy.options.compatibility = 188')], delete: "*

 * *            '[3]}}}',*

 * * "'metadata'": "{'language_info': {'version': '3.8.10'}}"}*

```diff
@@ -6,15 +6,18 @@
             "id": "internal-compensation",
             "metadata": {},
             "outputs": [],
             "source": [
                 "import os\n",
                 "from seeq import spy\n",
                 "import pandas as pd\n",
-                "import numpy as np"
+                "import numpy as np\n",
+                "\n",
+                "# Set the compatibility option so that you maximize the chance that SPy will remain compatible with your notebook/script\n",
+                "spy.options.compatibility = 188"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "id": "usual-insulation",
             "metadata": {},
@@ -450,13 +453,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.7.8"
+            "version": "3.8.10"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `seeq-spy-187.5/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot.jpg` & `seeq-spy-188.0/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot.jpg`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.5/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot2.jpg` & `seeq-spy-188.0/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot2.jpg`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.5/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot3.jpg` & `seeq-spy-188.0/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot3.jpg`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.5/seeq/spy/docs/Documentation/Attached Images/ReportAndDashboardTemplates1.png` & `seeq-spy-188.0/seeq/spy/docs/Documentation/Attached Images/ReportAndDashboardTemplates1.png`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.5/seeq/spy/docs/Documentation/Attached Images/TopicTemplateScreenshot1.png` & `seeq-spy-188.0/seeq/spy/docs/Documentation/Attached Images/TopicTemplateScreenshot1.png`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.5/seeq/spy/docs/Documentation/Attached Images/TopicTemplateScreenshot2.png` & `seeq-spy-188.0/seeq/spy/docs/Documentation/Attached Images/TopicTemplateScreenshot2.png`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.5/seeq/spy/docs/Documentation/Command Reference.ipynb` & `seeq-spy-188.0/seeq/spy/docs/Documentation/Command Reference.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999965790914067%*

 * *Differences: {"'cells'": "{4: {'outputs': {0: {'text': {insert: [(109, '        in takes precedence.\\n')], "*

 * *            'delete: [109]}}}}}'}*

```diff
@@ -183,15 +183,15 @@
                         "    order_by : {str, list}, default None\n",
                         "        An optional field or list of fields used to sort the search results.\n",
                         "        Fields on which results can be sorted are 'ID', 'Name', and 'Description'.\n",
                         "    \n",
                         "    quiet : bool, default False\n",
                         "        If True, suppresses progress output. Note that when status is\n",
                         "        provided, the quiet setting of the Status object that is passed\n",
-                        "        in takes precedent.\n",
+                        "        in takes precedence.\n",
                         "    \n",
                         "    status : spy.Status, optional\n",
                         "        If specified, the supplied Status object will be updated as the command\n",
                         "        progresses. It gets filled in with the same information you would see\n",
                         "        in Jupyter in the blue/green/red table below your code while the\n",
                         "        command is executed. The table itself is accessible as a DataFrame via\n",
                         "        the status.df property.\n",
```

### Comparing `seeq-spy-187.5/seeq/spy/docs/Documentation/Support Files/Example Export.zip` & `seeq-spy-188.0/seeq/spy/docs/Documentation/Support Files/Example Export.zip`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.5/seeq/spy/docs/Documentation/Support Files/Report and Dashboard Templates.zip` & `seeq-spy-188.0/seeq/spy/docs/Documentation/Support Files/Report and Dashboard Templates.zip`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.5/seeq/spy/docs/Documentation/Support Files/Workbook Templates.zip` & `seeq-spy-188.0/seeq/spy/docs/Documentation/Support Files/Workbook Templates.zip`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.5/seeq/spy/docs/Documentation/Support Files/csv_import_example.csv` & `seeq-spy-188.0/seeq/spy/docs/Documentation/Support Files/csv_import_example.csv`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.5/seeq/spy/docs/Documentation/Tutorial.ipynb` & `seeq-spy-188.0/seeq/spy/docs/Documentation/Tutorial.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9926470588235294%*

 * *Differences: {"'cells'": "{insert: [(3, OrderedDict([('cell_type', 'markdown'), ('metadata', OrderedDict()), "*

 * *            '(\'source\', ["It\'s important to set `spy.options.compatibility` in your script to '*

 * *            'the current major version of SPy so that you minimize the chance that a SPy version '*

 * *            'upgrade breaks your notebook or script code. By telling SPy what version you have '*

 * *            'been using and have tested with, it can make choices about what behavior is most '*

 * *            'likely to  […]*

```diff
@@ -32,14 +32,30 @@
                 "from seeq import spy"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
+                "It's important to set `spy.options.compatibility` in your script to the current major version of SPy so that you minimize the chance that a SPy version upgrade breaks your notebook or script code. By telling SPy what version you have been using and have tested with, it can make choices about what behavior is most likely to be compatible."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "spy.options.compatibility = 188"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
                 "You'll also want to import Pandas so that you can work with the DataFrame structures that the **spy** library consumes/produces."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {},
```

### Comparing `seeq-spy-187.5/seeq/spy/docs/Documentation/Version Considerations.ipynb` & `seeq-spy-188.0/seeq/spy/docs/Documentation/Version Considerations.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996590909090909%*

 * *Differences: {"'cells'": "{4: {'source': {insert: [(1, '\\n'), (2, '# Set the compatibility option so that you "*

 * *            "maximize the chance that SPy will remain compatible with your notebook/script\\n'), "*

 * *            "(3, 'spy.options.compatibility = 188\\n')]}}}"}*

```diff
@@ -79,14 +79,17 @@
                         "Seeq Server is at least R73.3.1? False\n"
                     ]
                 }
             ],
             "source": [
                 "from seeq import spy\n",
                 "\n",
+                "# Set the compatibility option so that you maximize the chance that SPy will remain compatible with your notebook/script\n",
+                "spy.options.compatibility = 188\n",
+                "\n",
                 "# Login so we can check the Seeq Server version\n",
                 "spy.login(url='http://localhost:34216', credentials_file='../credentials.key', force=False)\n",
                 "\n",
                 "# Check the SPy version\n",
                 "print(f'SPy is at least 184.3? {spy.utils.is_spy_module_version_at_least(184, 3)}')\n",
                 "print(f'Seeq Server is at least R73.3.1? {spy.utils.is_server_version_at_least(73, 3, 1)}')"
             ]
```

### Comparing `seeq-spy-187.5/seeq/spy/docs/Documentation/Workbook Templates.ipynb` & `seeq-spy-188.0/seeq/spy/docs/Documentation/Workbook Templates.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998027146464646%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(1, 'from seeq import spy\\n'), (2, '\\n'), (3, '# Set the "*

 * *            'compatibility option so that you maximize the chance that SPy will remain compatible '*

 * *            "with your notebook/script\\n'), (4, 'spy.options.compatibility = 188')], delete: "*

 * *            '[1]}}}'}*

```diff
@@ -8,15 +8,18 @@
                 "pycharm": {
                     "name": "#%%\n"
                 }
             },
             "outputs": [],
             "source": [
                 "import pandas as pd\n",
-                "from seeq import spy"
+                "from seeq import spy\n",
+                "\n",
+                "# Set the compatibility option so that you maximize the chance that SPy will remain compatible with your notebook/script\n",
+                "spy.options.compatibility = 188"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "id": "f4146468",
             "metadata": {
```

### Comparing `seeq-spy-187.5/seeq/spy/docs/Documentation/spy.acl.ipynb` & `seeq-spy-188.0/seeq/spy/docs/Documentation/spy.acl.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999446761557983%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(1, 'import pandas as pd\\n'), (2, '\\n'), (3, '# Set the "*

 * *            'compatibility option so that you maximize the chance that SPy will remain compatible '*

 * *            "with your notebook/script\\n'), (4, 'spy.options.compatibility = 188')], delete: "*

 * *            "[1]}}, 17: {'outputs': {0: {'text': {insert: [(51, '        in takes "*

 * *            "precedence.\\n')], delete: [51]}}}}, 18: {'outputs': {0: {'text': {insert: [(31, "*

 * *            "'        in takes precede […]*

```diff
@@ -3,15 +3,18 @@
         {
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from seeq import spy\n",
-                "import pandas as pd"
+                "import pandas as pd\n",
+                "\n",
+                "# Set the compatibility option so that you maximize the chance that SPy will remain compatible with your notebook/script\n",
+                "spy.options.compatibility = 188"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {},
             "outputs": [
@@ -1059,15 +1062,15 @@
                         "        If 'raise', any errors encountered will cause an exception. If\n",
                         "        'catalog', errors will be added to a 'Push Result' column in the\n",
                         "        status.df DataFrame.\n",
                         "    \n",
                         "    quiet : bool, default False\n",
                         "        If True, suppresses progress output. Note that when status is\n",
                         "        provided, the quiet setting of the Status object that is passed\n",
-                        "        in takes precedent.\n",
+                        "        in takes precedence.\n",
                         "    \n",
                         "    status : spy.Status, optional\n",
                         "        If specified, the supplied Status object will be updated as the command\n",
                         "        progresses. It gets filled in with the same information you would see\n",
                         "        in Jupyter in the blue/green/red table below your code while the\n",
                         "        command is executed. The table itself is accessible as a DataFrame via\n",
                         "        the status.df property.\n",
@@ -1160,15 +1163,15 @@
                         "        If 'raise', any errors encountered will cause an exception. If\n",
                         "        'catalog', errors will be added to a 'Pull Result' column in the\n",
                         "        status.df DataFrame.\n",
                         "    \n",
                         "    quiet : bool, default False\n",
                         "        If True, suppresses progress output. Note that when status is\n",
                         "        provided, the quiet setting of the Status object that is passed\n",
-                        "        in takes precedent.\n",
+                        "        in takes precedence.\n",
                         "    \n",
                         "    status : spy.Status, optional\n",
                         "        If specified, the supplied Status object will be updated as the command\n",
                         "        progresses. It gets filled in with the same information you would see\n",
                         "        in Jupyter in the blue/green/red table below your code while the\n",
                         "        command is executed. The table itself is accessible as a DataFrame via\n",
                         "        the status.df property.\n",
```

### Comparing `seeq-spy-187.5/seeq/spy/docs/Documentation/spy.jobs.ipynb` & `seeq-spy-188.0/seeq/spy/docs/Documentation/spy.jobs.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9993055555555556%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(1, 'import pandas as pd\\n'), (2, '\\n'), (3, '# Set the "*

 * *            'compatibility option so that you maximize the chance that SPy will remain compatible '*

 * *            "with your notebook/script\\n'), (4, 'spy.options.compatibility = 188')], delete: "*

 * *            '[1]}}}'}*

```diff
@@ -3,15 +3,18 @@
         {
             "cell_type": "code",
             "execution_count": 3,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from seeq import spy\n",
-                "import pandas as pd"
+                "import pandas as pd\n",
+                "\n",
+                "# Set the compatibility option so that you maximize the chance that SPy will remain compatible with your notebook/script\n",
+                "spy.options.compatibility = 188"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# spy.jobs\n",
```

### Comparing `seeq-spy-187.5/seeq/spy/docs/Documentation/spy.login.ipynb` & `seeq-spy-188.0/seeq/spy/docs/Documentation/spy.login.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9991041059280855%*

 * *Differences: {"'cells'": "{0: {'source': ['from seeq import spy\\n', '\\n', '# Set the compatibility option so "*

 * *            'that you maximize the chance that SPy will remain compatible with your '*

 * *            "notebook/script\\n', 'spy.options.compatibility = 188']}, 13: {'outputs': {0: "*

 * *            "{'text': {insert: [(67, '        in takes precedence.\\n')], delete: [67]}}}}}"}*

```diff
@@ -6,15 +6,18 @@
             "metadata": {
                 "pycharm": {
                     "is_executing": true
                 }
             },
             "outputs": [],
             "source": [
-                "from seeq import spy"
+                "from seeq import spy\n",
+                "\n",
+                "# Set the compatibility option so that you maximize the chance that SPy will remain compatible with your notebook/script\n",
+                "spy.options.compatibility = 188"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# spy.login\n",
@@ -207,15 +210,15 @@
                         "        login if already logged in. You should include a spy.login(force=False)\n",
                         "        cell if you are creating example notebooks that may be used in Jupyter\n",
                         "        environments like Anaconda, AWS SageMaker or Azure Notebooks.)\n",
                         "    \n",
                         "    quiet : bool, default False\n",
                         "        If True, suppresses progress output. Note that when status is\n",
                         "        provided, the quiet setting of the Status object that is passed\n",
-                        "        in takes precedent.\n",
+                        "        in takes precedence.\n",
                         "    \n",
                         "    status : spy.Status, optional\n",
                         "        If supplied, this Status object will be updated as the command\n",
                         "        progresses.\n",
                         "    \n",
                         "    session : spy.Session, optional\n",
                         "        If supplied, the Session object (and its Options) will be used to\n",
```

### Comparing `seeq-spy-187.5/seeq/spy/docs/Documentation/spy.pull.ipynb` & `seeq-spy-188.0/seeq/spy/docs/Documentation/spy.pull.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9983307453416149%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, 'from seeq import spy\\n'), (3, '# Set the compatibility "*

 * *            'option so that you maximize the chance that SPy will remain compatible with your '*

 * *            "notebook/script\\n'), (4, 'spy.options.compatibility = 188')], delete: [2]}}}",*

 * * "'metadata'": "{'language_info': {'version': '3.8.10'}}"}*

```diff
@@ -2,17 +2,19 @@
     "cells": [
         {
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [],
             "source": [
+                "from seeq import spy\n",
                 "import pandas as pd\n",
                 "\n",
-                "from seeq import spy"
+                "# Set the compatibility option so that you maximize the chance that SPy will remain compatible with your notebook/script\n",
+                "spy.options.compatibility = 188"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {},
             "outputs": [
@@ -2606,15 +2608,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.7.8"
+            "version": "3.8.10"
         },
         "pycharm": {
             "stem_cell": {
                 "cell_type": "raw",
                 "metadata": {
                     "collapsed": false
                 },
```

### Comparing `seeq-spy-187.5/seeq/spy/docs/Documentation/spy.push.ipynb` & `seeq-spy-188.0/seeq/spy/docs/Documentation/spy.push.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997628171247357%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(1, 'import pandas as pd\\n'), (2, '\\n'), (3, '# Set the "*

 * *            'compatibility option so that you maximize the chance that SPy will remain compatible '*

 * *            "with your notebook/script\\n'), (4, 'spy.options.compatibility = 188')], delete: "*

 * *            "[1]}}, 43: {'outputs': {0: {'text': {insert: [(174, '        in takes "*

 * *            "precedence.\\n')], delete: [174]}}}}}"}*

```diff
@@ -3,15 +3,18 @@
         {
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from seeq import spy\n",
-                "import pandas as pd"
+                "import pandas as pd\n",
+                "\n",
+                "# Set the compatibility option so that you maximize the chance that SPy will remain compatible with your notebook/script\n",
+                "spy.options.compatibility = 188"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {},
             "outputs": [
@@ -2112,15 +2115,15 @@
                         "        If 'raise', any errors encountered will cause an exception. If\n",
                         "        'catalog', errors will be added to a 'Result' column in the status.df\n",
                         "        DataFrame.\n",
                         "    \n",
                         "    quiet : bool, default False\n",
                         "        If True, suppresses progress output. Note that when status is\n",
                         "        provided, the quiet setting of the Status object that is passed\n",
-                        "        in takes precedent.\n",
+                        "        in takes precedence.\n",
                         "    \n",
                         "    status : spy.Status, optional\n",
                         "        If specified, the supplied Status object will be updated as the command\n",
                         "        progresses. It gets filled in with the same information you would see\n",
                         "        in Jupyter in the blue/green/red table below your code while the\n",
                         "        command is executed. The table itself is accessible as a DataFrame via\n",
                         "        the status.df property.\n",
```

### Comparing `seeq-spy-187.5/seeq/spy/docs/Documentation/spy.search.ipynb` & `seeq-spy-188.0/seeq/spy/docs/Documentation/spy.search.ipynb`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994449991864225%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(1, 'import pandas as pd\\n'), (2, '\\n'), (3, '# Set the "*

 * *            'compatibility option so that you maximize the chance that SPy will remain compatible '*

 * *            "with your notebook/script\\n'), (4, 'spy.options.compatibility = 188')], delete: "*

 * *            "[1]}}, 1: {'outputs': {0: {'data': {'text/html': ['<div "*

 * *            'style="background-color: #EEFFEE;color:black; text-align: left;">Logged in to '*

 * *            '<strong>http://localhost:34216</strong> s […]*

```diff
@@ -3,26 +3,29 @@
         {
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from seeq import spy\n",
-                "import pandas as pd"
+                "import pandas as pd\n",
+                "\n",
+                "# Set the compatibility option so that you maximize the chance that SPy will remain compatible with your notebook/script\n",
+                "spy.options.compatibility = 188"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<div style=\"background-color: #EEFFEE;color:black;text-align: left;\">Logged in to <strong>http://localhost:34216</strong> successfully as <strong>agent_api_key</strong>.<br>Seeq Server Version: <strong>R57.0.0-SNAPSHOT</strong><br>Seeq Python Module Version: <strong>57.0.0.182.41</strong></div>"
+                            "<div style=\"background-color: #EEFFEE;color:black; text-align: left;\">Logged in to <strong>http://localhost:34216</strong> successfully as <strong>agent_api_key</strong>.<br>Seeq Server Version: <strong>R61.0.0-SNAPSHOT</strong><br>Seeq Python Module Version: <strong>61.0.0.184.25</strong></div>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -64,15 +67,15 @@
             "cell_type": "code",
             "execution_count": 3,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<div style=\"background-color: #EEFFEE;color:black;text-align: left;\">Query successful</div><table style=\"color:black;\"><tr><td style=\"background-color: #EEFFEE;\"></td><td style=\"background-color: #EEFFEE; text-align: left;\">Name</td><td style=\"background-color: #EEFFEE; text-align: left;\">Path</td><td style=\"background-color: #EEFFEE; text-align: left;\">Time</td><td style=\"background-color: #EEFFEE; text-align: right;\">Count</td><td style=\"background-color: #EEFFEE; text-align: left;\">Result</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">0</td><td style=\"text-align: left; vertical-align: top;\">Humid</td><td style=\"text-align: left; vertical-align: top;\">Example >> Cooling Tower 1</td><td style=\"vertical-align: top;\">00:00:00.08</td><td style=\"text-align: right; vertical-align: top;\">8</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr></table>"
+                            "<div style=\"background-color: #EEFFEE;color:black; text-align: left;\">Query successful</div><table class=\"tex2jax_ignore\" style=\"color:black;\"><tr><td style=\"background-color: #EEFFEE;\"></td><td style=\"background-color: #EEFFEE; text-align: left;\">Name</td><td style=\"background-color: #EEFFEE; text-align: left;\">Path</td><td style=\"background-color: #EEFFEE; text-align: left;\">Time</td><td style=\"background-color: #EEFFEE; text-align: right;\">Count</td><td style=\"background-color: #EEFFEE; text-align: right;\">Pages</td><td style=\"background-color: #EEFFEE; text-align: left;\">Result</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">0</td><td style=\"text-align: left; vertical-align: top;\">Humid</td><td style=\"text-align: left; vertical-align: top;\">Example >> Cooling Tower 1</td><td style=\"vertical-align: top;\">00:00:00.05</td><td style=\"text-align: right; vertical-align: top;\">8</td><td style=\"text-align: right; vertical-align: top;\">1</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr></table>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -108,122 +111,122 @@
                             "      <th>Datasource Name</th>\n",
                             "      <th>Archived</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
-                            "      <td>63A50762-7393-4C48-B7CE-C8171447E2F5</td>\n",
+                            "      <td>5B43701D-A50A-4A47-A642-4918BA98C381</td>\n",
                             "      <td>Example &gt;&gt; Cooling Tower 1</td>\n",
-                            "      <td>Area B</td>\n",
+                            "      <td>Area C</td>\n",
                             "      <td>Relative Humidity</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
                             "      <td>%</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1</th>\n",
-                            "      <td>A5CBEC0A-183C-4A70-82B4-3B821E0BD075</td>\n",
+                            "      <td>8C4E0B58-E4E7-44D6-BE25-CE19FFEB4CE3</td>\n",
                             "      <td>Example &gt;&gt; Cooling Tower 1</td>\n",
-                            "      <td>Area H</td>\n",
+                            "      <td>Area A</td>\n",
                             "      <td>Relative Humidity</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
                             "      <td>%</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2</th>\n",
-                            "      <td>3810A5DB-06E5-4820-8CF7-06B381BC8355</td>\n",
+                            "      <td>99795625-0FAE-4E76-9DA6-7E03AA28603B</td>\n",
                             "      <td>Example &gt;&gt; Cooling Tower 1</td>\n",
-                            "      <td>Area I</td>\n",
+                            "      <td>Area J</td>\n",
                             "      <td>Relative Humidity</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
                             "      <td>%</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>3</th>\n",
-                            "      <td>F0381FA9-BA3D-4AB5-B5F8-44CC53B73242</td>\n",
+                            "      <td>B5510C09-F1F5-4BE8-928A-DABA83FA7BBF</td>\n",
                             "      <td>Example &gt;&gt; Cooling Tower 1</td>\n",
                             "      <td>Area K</td>\n",
                             "      <td>Relative Humidity</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
                             "      <td>%</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>4</th>\n",
-                            "      <td>9C900C56-9208-40AD-A77C-2C885175056F</td>\n",
+                            "      <td>BD9248AA-403D-4864-B6FE-6DBD7B65F5E2</td>\n",
                             "      <td>Example &gt;&gt; Cooling Tower 1</td>\n",
-                            "      <td>Area G</td>\n",
+                            "      <td>Area H</td>\n",
                             "      <td>Relative Humidity</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
                             "      <td>%</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>5</th>\n",
-                            "      <td>42DDF8F2-87EE-40EF-B013-5B1C123837F3</td>\n",
+                            "      <td>C2406578-736A-4992-8CF5-B1E29A46CE2F</td>\n",
                             "      <td>Example &gt;&gt; Cooling Tower 1</td>\n",
-                            "      <td>Area J</td>\n",
+                            "      <td>Area G</td>\n",
                             "      <td>Relative Humidity</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
                             "      <td>%</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>6</th>\n",
-                            "      <td>10DCF4CC-B1D1-46DE-B2C5-A23F5F88B617</td>\n",
+                            "      <td>D77BB5EE-E9D5-4EAD-B7ED-17593525EDA2</td>\n",
                             "      <td>Example &gt;&gt; Cooling Tower 1</td>\n",
-                            "      <td>Area C</td>\n",
+                            "      <td>Area I</td>\n",
                             "      <td>Relative Humidity</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
                             "      <td>%</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>7</th>\n",
-                            "      <td>4CD18E76-E822-447F-A2E9-76160B835CC6</td>\n",
+                            "      <td>EA2FAFEF-AEB1-4A3C-AC1E-191417EAD250</td>\n",
                             "      <td>Example &gt;&gt; Cooling Tower 1</td>\n",
-                            "      <td>Area A</td>\n",
+                            "      <td>Area B</td>\n",
                             "      <td>Relative Humidity</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
                             "      <td>%</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
                             "                                     ID                        Path   Asset  \\\n",
-                            "0  63A50762-7393-4C48-B7CE-C8171447E2F5  Example >> Cooling Tower 1  Area B   \n",
-                            "1  A5CBEC0A-183C-4A70-82B4-3B821E0BD075  Example >> Cooling Tower 1  Area H   \n",
-                            "2  3810A5DB-06E5-4820-8CF7-06B381BC8355  Example >> Cooling Tower 1  Area I   \n",
-                            "3  F0381FA9-BA3D-4AB5-B5F8-44CC53B73242  Example >> Cooling Tower 1  Area K   \n",
-                            "4  9C900C56-9208-40AD-A77C-2C885175056F  Example >> Cooling Tower 1  Area G   \n",
-                            "5  42DDF8F2-87EE-40EF-B013-5B1C123837F3  Example >> Cooling Tower 1  Area J   \n",
-                            "6  10DCF4CC-B1D1-46DE-B2C5-A23F5F88B617  Example >> Cooling Tower 1  Area C   \n",
-                            "7  4CD18E76-E822-447F-A2E9-76160B835CC6  Example >> Cooling Tower 1  Area A   \n",
+                            "0  5B43701D-A50A-4A47-A642-4918BA98C381  Example >> Cooling Tower 1  Area C   \n",
+                            "1  8C4E0B58-E4E7-44D6-BE25-CE19FFEB4CE3  Example >> Cooling Tower 1  Area A   \n",
+                            "2  99795625-0FAE-4E76-9DA6-7E03AA28603B  Example >> Cooling Tower 1  Area J   \n",
+                            "3  B5510C09-F1F5-4BE8-928A-DABA83FA7BBF  Example >> Cooling Tower 1  Area K   \n",
+                            "4  BD9248AA-403D-4864-B6FE-6DBD7B65F5E2  Example >> Cooling Tower 1  Area H   \n",
+                            "5  C2406578-736A-4992-8CF5-B1E29A46CE2F  Example >> Cooling Tower 1  Area G   \n",
+                            "6  D77BB5EE-E9D5-4EAD-B7ED-17593525EDA2  Example >> Cooling Tower 1  Area I   \n",
+                            "7  EA2FAFEF-AEB1-4A3C-AC1E-191417EAD250  Example >> Cooling Tower 1  Area B   \n",
                             "\n",
                             "                Name  Description          Type Value Unit Of Measure  \\\n",
                             "0  Relative Humidity          NaN  StoredSignal                     %   \n",
                             "1  Relative Humidity          NaN  StoredSignal                     %   \n",
                             "2  Relative Humidity          NaN  StoredSignal                     %   \n",
                             "3  Relative Humidity          NaN  StoredSignal                     %   \n",
                             "4  Relative Humidity          NaN  StoredSignal                     %   \n",
@@ -290,15 +293,15 @@
             "cell_type": "code",
             "execution_count": 4,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<div style=\"background-color: #EEFFEE;color:black;text-align: left;\">Query successful</div><table style=\"color:black;\"><tr><td style=\"background-color: #EEFFEE;\"></td><td style=\"background-color: #EEFFEE; text-align: left;\">Name</td><td style=\"background-color: #EEFFEE; text-align: left;\">Datasource Name</td><td style=\"background-color: #EEFFEE; text-align: left;\">Time</td><td style=\"background-color: #EEFFEE; text-align: right;\">Count</td><td style=\"background-color: #EEFFEE; text-align: left;\">Result</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">0</td><td style=\"text-align: left; vertical-align: top;\">Area A_*Humid*</td><td style=\"text-align: left; vertical-align: top;\">Example Data</td><td style=\"vertical-align: top;\">00:00:00.03</td><td style=\"text-align: right; vertical-align: top;\">1</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr></table>"
+                            "<div style=\"background-color: #EEFFEE;color:black; text-align: left;\">Query successful</div><table class=\"tex2jax_ignore\" style=\"color:black;\"><tr><td style=\"background-color: #EEFFEE;\"></td><td style=\"background-color: #EEFFEE; text-align: left;\">Name</td><td style=\"background-color: #EEFFEE; text-align: left;\">Datasource Name</td><td style=\"background-color: #EEFFEE; text-align: left;\">Time</td><td style=\"background-color: #EEFFEE; text-align: right;\">Count</td><td style=\"background-color: #EEFFEE; text-align: right;\">Pages</td><td style=\"background-color: #EEFFEE; text-align: left;\">Result</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">0</td><td style=\"text-align: left; vertical-align: top;\">Area A_*Humid*</td><td style=\"text-align: left; vertical-align: top;\">Example Data</td><td style=\"vertical-align: top;\">00:00:00.02</td><td style=\"text-align: right; vertical-align: top;\">1</td><td style=\"text-align: right; vertical-align: top;\">1</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr></table>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -346,61 +349,61 @@
                             "      <th>Sync Token</th>\n",
                             "      <th>Unsearchable</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
-                            "      <td>35754CAB-B2D8-441A-904E-795F412EF602</td>\n",
+                            "      <td>E9744446-848A-4461-A730-29CD0C97A7DC</td>\n",
                             "      <td>Area A_Relative Humidity</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
                             "      <td>%</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>False</td>\n",
-                            "      <td>0e40c308-109d-4816-ad7d-e94574701cb5</td>\n",
+                            "      <td>51c16b8e-a8bd-43d4-91d2-6466bc7c1e09</td>\n",
                             "      <td>...</td>\n",
                             "      <td>Time Series CSV Files</td>\n",
                             "      <td>Example Data</td>\n",
-                            "      <td>False</td>\n",
+                            "      <td>True</td>\n",
                             "      <td>Linear</td>\n",
                             "      <td>ns</td>\n",
                             "      <td>2min</td>\n",
                             "      <td>2min</td>\n",
                             "      <td>%</td>\n",
-                            "      <td>2021-12-27T01:57:07.788823900Z</td>\n",
+                            "      <td>2022-12-28T17:20:51.178990800Z</td>\n",
                             "      <td>False</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
-                            "<p>1 rows \u00d7 22 columns</p>\n",
+                            "<p>1 rows \u00d7 21 columns</p>\n",
                             "</div>"
                         ],
                         "text/plain": [
                             "                                     ID                      Name  \\\n",
-                            "0  35754CAB-B2D8-441A-904E-795F412EF602  Area A_Relative Humidity   \n",
+                            "0  E9744446-848A-4461-A730-29CD0C97A7DC  Area A_Relative Humidity   \n",
                             "\n",
                             "   Description          Type Value Unit Of Measure Datasource Name  Archived  \\\n",
                             "0          NaN  StoredSignal                     %    Example Data     False   \n",
                             "\n",
                             "   Scoped To  Cache Enabled                              Cache ID  ...  \\\n",
-                            "0        NaN          False  0e40c308-109d-4816-ad7d-e94574701cb5  ...   \n",
+                            "0        NaN          False  51c16b8e-a8bd-43d4-91d2-6466bc7c1e09  ...   \n",
                             "\n",
-                            "        Datasource Class Datasource ID Enabled Interpolation Method  \\\n",
-                            "0  Time Series CSV Files  Example Data   False               Linear   \n",
+                            "        Datasource Class Datasource ID Enabled  Interpolation Method  \\\n",
+                            "0  Time Series CSV Files  Example Data    True                Linear   \n",
                             "\n",
-                            "   Key Unit Of Measure Maximum Interpolation Source Maximum Interpolation  \\\n",
-                            "0                   ns                  2min                         2min   \n",
+                            "  Key Unit Of Measure Maximum Interpolation Source Maximum Interpolation  \\\n",
+                            "0                  ns                  2min                         2min   \n",
                             "\n",
                             "  Source Value Unit Of Measure                      Sync Token Unsearchable  \n",
-                            "0                            %  2021-12-27T01:57:07.788823900Z        False  \n",
+                            "0                            %  2022-12-28T17:20:51.178990800Z        False  \n",
                             "\n",
-                            "[1 rows x 22 columns]"
+                            "[1 rows x 21 columns]"
                         ]
                     },
                     "execution_count": 4,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -424,15 +427,15 @@
             "cell_type": "code",
             "execution_count": 5,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<div style=\"background-color: #EEFFEE;color:black;text-align: left;\">Query successful</div><table style=\"color:black;\"><tr><td style=\"background-color: #EEFFEE;\"></td><td style=\"background-color: #EEFFEE; text-align: left;\">Name</td><td style=\"background-color: #EEFFEE; text-align: left;\">Datasource Name</td><td style=\"background-color: #EEFFEE; text-align: left;\">Time</td><td style=\"background-color: #EEFFEE; text-align: right;\">Count</td><td style=\"background-color: #EEFFEE; text-align: left;\">Result</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">0</td><td style=\"text-align: left; vertical-align: top;\">Area ?_Compressor Stage</td><td style=\"text-align: left; vertical-align: top;\">Example Data</td><td style=\"vertical-align: top;\">00:00:01.87</td><td style=\"text-align: right; vertical-align: top;\">11</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr></table>"
+                            "<div style=\"background-color: #EEFFEE;color:black; text-align: left;\">Query successful</div><table class=\"tex2jax_ignore\" style=\"color:black;\"><tr><td style=\"background-color: #EEFFEE;\"></td><td style=\"background-color: #EEFFEE; text-align: left;\">Name</td><td style=\"background-color: #EEFFEE; text-align: left;\">Datasource Name</td><td style=\"background-color: #EEFFEE; text-align: left;\">Time</td><td style=\"background-color: #EEFFEE; text-align: right;\">Count</td><td style=\"background-color: #EEFFEE; text-align: right;\">Pages</td><td style=\"background-color: #EEFFEE; text-align: left;\">Result</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">0</td><td style=\"text-align: left; vertical-align: top;\">Area ?_Compressor Stage</td><td style=\"text-align: left; vertical-align: top;\">Example Data</td><td style=\"vertical-align: top;\">00:00:01.02</td><td style=\"text-align: right; vertical-align: top;\">11</td><td style=\"text-align: right; vertical-align: top;\">1</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr></table>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -467,150 +470,150 @@
                             "      <th>Archived</th>\n",
                             "      <th>Estimated Sample Period</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
-                            "      <td>CB27ACE7-8F49-4796-BB50-24C67D30D16B</td>\n",
+                            "      <td>DCA902F6-237D-4275-9669-1EF840ADB5D9</td>\n",
                             "      <td>Area A_Compressor Stage</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
                             "      <td>string</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
                             "      <td>0 days 00:02:00</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1</th>\n",
-                            "      <td>DED4CDAE-C84B-466B-B14F-0340506EED06</td>\n",
+                            "      <td>3E671AFE-1EBB-476E-BBD3-44691DA6F77D</td>\n",
                             "      <td>Area B_Compressor Stage</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
                             "      <td>string</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
                             "      <td>0 days 00:02:00</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2</th>\n",
-                            "      <td>5DF7F633-CA16-40DB-BBE8-77A2C6450673</td>\n",
+                            "      <td>9D156E8A-B19D-4BFB-BA6E-9BBF220F4CFF</td>\n",
                             "      <td>Area C_Compressor Stage</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
                             "      <td>string</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
                             "      <td>0 days 00:02:00</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>3</th>\n",
-                            "      <td>531DB08F-9BCB-4A32-A45D-5164132146D5</td>\n",
+                            "      <td>EA367096-CBC9-4B16-B219-D84FDC9AF90E</td>\n",
                             "      <td>Area D_Compressor Stage</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
                             "      <td>string</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
                             "      <td>0 days 00:02:00</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>4</th>\n",
-                            "      <td>2140C2A1-FA05-42A9-9454-601B030917BE</td>\n",
+                            "      <td>7837A0D6-361C-46CB-9E83-6AED3E9F5DBF</td>\n",
                             "      <td>Area E_Compressor Stage</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
                             "      <td>string</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
                             "      <td>0 days 00:02:00</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>5</th>\n",
-                            "      <td>6E9A92CC-0039-41AF-A9F7-21D84AA1B626</td>\n",
+                            "      <td>EAAA24BC-7A10-45DF-B9B7-741B6604FA56</td>\n",
                             "      <td>Area G_Compressor Stage</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
                             "      <td>string</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
                             "      <td>0 days 00:02:00</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>6</th>\n",
-                            "      <td>A50F60DC-F949-4895-A695-BABD39DBFDD4</td>\n",
+                            "      <td>912A4654-9A86-4FA6-AB14-1353E98634AA</td>\n",
                             "      <td>Area H_Compressor Stage</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
                             "      <td>string</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
                             "      <td>0 days 00:02:00</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>7</th>\n",
-                            "      <td>6E39F2D7-DB8C-44E9-8F3B-81F29F6BB0B8</td>\n",
+                            "      <td>D5ACE8CC-D190-420C-B68F-8944440E040B</td>\n",
                             "      <td>Area I_Compressor Stage</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
                             "      <td>string</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
                             "      <td>0 days 00:02:00</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>8</th>\n",
-                            "      <td>A47FA73B-44DE-4199-8AAA-B930888B9322</td>\n",
+                            "      <td>D211CA9C-694E-4ED0-9D4E-D31EC1F07146</td>\n",
                             "      <td>Area J_Compressor Stage</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
                             "      <td>string</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
                             "      <td>0 days 00:02:00</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>9</th>\n",
-                            "      <td>699BF5DA-B5F8-493E-A1C7-24635DD11B12</td>\n",
+                            "      <td>06168B5F-E43D-41F1-8793-23AC2AC8582A</td>\n",
                             "      <td>Area K_Compressor Stage</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
                             "      <td>string</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
                             "      <td>0 days 00:02:00</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>10</th>\n",
-                            "      <td>308BE55D-3DE6-4F00-A986-2891A1F3C1DE</td>\n",
+                            "      <td>D0D2B548-0C36-46EC-BB52-4683486706B8</td>\n",
                             "      <td>Area Z_Compressor Stage</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
                             "      <td>string</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
                             "      <td>0 days 00:00:02</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
                             "                                      ID                     Name  \\\n",
-                            "0   CB27ACE7-8F49-4796-BB50-24C67D30D16B  Area A_Compressor Stage   \n",
-                            "1   DED4CDAE-C84B-466B-B14F-0340506EED06  Area B_Compressor Stage   \n",
-                            "2   5DF7F633-CA16-40DB-BBE8-77A2C6450673  Area C_Compressor Stage   \n",
-                            "3   531DB08F-9BCB-4A32-A45D-5164132146D5  Area D_Compressor Stage   \n",
-                            "4   2140C2A1-FA05-42A9-9454-601B030917BE  Area E_Compressor Stage   \n",
-                            "5   6E9A92CC-0039-41AF-A9F7-21D84AA1B626  Area G_Compressor Stage   \n",
-                            "6   A50F60DC-F949-4895-A695-BABD39DBFDD4  Area H_Compressor Stage   \n",
-                            "7   6E39F2D7-DB8C-44E9-8F3B-81F29F6BB0B8  Area I_Compressor Stage   \n",
-                            "8   A47FA73B-44DE-4199-8AAA-B930888B9322  Area J_Compressor Stage   \n",
-                            "9   699BF5DA-B5F8-493E-A1C7-24635DD11B12  Area K_Compressor Stage   \n",
-                            "10  308BE55D-3DE6-4F00-A986-2891A1F3C1DE  Area Z_Compressor Stage   \n",
+                            "0   DCA902F6-237D-4275-9669-1EF840ADB5D9  Area A_Compressor Stage   \n",
+                            "1   3E671AFE-1EBB-476E-BBD3-44691DA6F77D  Area B_Compressor Stage   \n",
+                            "2   9D156E8A-B19D-4BFB-BA6E-9BBF220F4CFF  Area C_Compressor Stage   \n",
+                            "3   EA367096-CBC9-4B16-B219-D84FDC9AF90E  Area D_Compressor Stage   \n",
+                            "4   7837A0D6-361C-46CB-9E83-6AED3E9F5DBF  Area E_Compressor Stage   \n",
+                            "5   EAAA24BC-7A10-45DF-B9B7-741B6604FA56  Area G_Compressor Stage   \n",
+                            "6   912A4654-9A86-4FA6-AB14-1353E98634AA  Area H_Compressor Stage   \n",
+                            "7   D5ACE8CC-D190-420C-B68F-8944440E040B  Area I_Compressor Stage   \n",
+                            "8   D211CA9C-694E-4ED0-9D4E-D31EC1F07146  Area J_Compressor Stage   \n",
+                            "9   06168B5F-E43D-41F1-8793-23AC2AC8582A  Area K_Compressor Stage   \n",
+                            "10  D0D2B548-0C36-46EC-BB52-4683486706B8  Area Z_Compressor Stage   \n",
                             "\n",
                             "    Description          Type Value Unit Of Measure Datasource Name  Archived  \\\n",
                             "0           NaN  StoredSignal                string    Example Data     False   \n",
                             "1           NaN  StoredSignal                string    Example Data     False   \n",
                             "2           NaN  StoredSignal                string    Example Data     False   \n",
                             "3           NaN  StoredSignal                string    Example Data     False   \n",
                             "4           NaN  StoredSignal                string    Example Data     False   \n",
@@ -756,15 +759,15 @@
             "cell_type": "code",
             "execution_count": 7,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<div style=\"background-color: #EEFFEE;color:black;text-align: left;\">Query successful</div><table style=\"color:black;\"><tr><td style=\"background-color: #EEFFEE;\"></td><td style=\"background-color: #EEFFEE; text-align: left;\">Name</td><td style=\"background-color: #EEFFEE; text-align: left;\">Datasource Name</td><td style=\"background-color: #EEFFEE; text-align: left;\">Time</td><td style=\"background-color: #EEFFEE; text-align: right;\">Count</td><td style=\"background-color: #EEFFEE; text-align: left;\">Result</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">0</td><td style=\"text-align: left; vertical-align: top;\">Area A_Temperature</td><td style=\"text-align: left; vertical-align: top;\">Example Data</td><td style=\"vertical-align: top;\">00:00:00.03</td><td style=\"text-align: right; vertical-align: top;\">1</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">1</td><td style=\"text-align: left; vertical-align: top;\">Area B_Compressor Power</td><td style=\"text-align: left; vertical-align: top;\">Example Data</td><td style=\"vertical-align: top;\">00:00:00.01</td><td style=\"text-align: right; vertical-align: top;\">1</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">2</td><td style=\"text-align: left; vertical-align: top;\">Optimize</td><td style=\"text-align: left; vertical-align: top;\">Example Data</td><td style=\"vertical-align: top;\">00:00:00.01</td><td style=\"text-align: right; vertical-align: top;\">0</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr></table>"
+                            "<div style=\"background-color: #EEFFEE;color:black; text-align: left;\">Query successful</div><table class=\"tex2jax_ignore\" style=\"color:black;\"><tr><td style=\"background-color: #EEFFEE;\"></td><td style=\"background-color: #EEFFEE; text-align: left;\">Name</td><td style=\"background-color: #EEFFEE; text-align: left;\">Datasource Name</td><td style=\"background-color: #EEFFEE; text-align: left;\">Time</td><td style=\"background-color: #EEFFEE; text-align: right;\">Count</td><td style=\"background-color: #EEFFEE; text-align: right;\">Pages</td><td style=\"background-color: #EEFFEE; text-align: left;\">Result</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">0</td><td style=\"text-align: left; vertical-align: top;\">Area A_Temperature</td><td style=\"text-align: left; vertical-align: top;\">Example Data</td><td style=\"vertical-align: top;\">00:00:00.02</td><td style=\"text-align: right; vertical-align: top;\">1</td><td style=\"text-align: right; vertical-align: top;\">1</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">1</td><td style=\"text-align: left; vertical-align: top;\">Area B_Compressor Power</td><td style=\"text-align: left; vertical-align: top;\">Example Data</td><td style=\"vertical-align: top;\">00:00:00.01</td><td style=\"text-align: right; vertical-align: top;\">1</td><td style=\"text-align: right; vertical-align: top;\">1</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">2</td><td style=\"text-align: left; vertical-align: top;\">Optimize</td><td style=\"text-align: left; vertical-align: top;\">Example Data</td><td style=\"vertical-align: top;\">00:00:00.01</td><td style=\"text-align: right; vertical-align: top;\">0</td><td style=\"text-align: right; vertical-align: top;\">1</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr></table>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -798,40 +801,40 @@
                             "      <th>Datasource Name</th>\n",
                             "      <th>Archived</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
-                            "      <td>83432370-6220-49DF-9E40-3A8C573C51BD</td>\n",
+                            "      <td>F8B2EF0E-BAB2-441D-B031-6F920099D74A</td>\n",
                             "      <td>Area A_Temperature</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
                             "      <td>\u00b0F</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1</th>\n",
-                            "      <td>07FB0393-DD03-4541-A9FC-D995170CE87D</td>\n",
+                            "      <td>84ED2BB0-AD0B-4C76-8233-EEA7EB358F97</td>\n",
                             "      <td>Area B_Compressor Power</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
                             "      <td>kW</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
                             "                                     ID                     Name  Description  \\\n",
-                            "0  83432370-6220-49DF-9E40-3A8C573C51BD       Area A_Temperature          NaN   \n",
-                            "1  07FB0393-DD03-4541-A9FC-D995170CE87D  Area B_Compressor Power          NaN   \n",
+                            "0  F8B2EF0E-BAB2-441D-B031-6F920099D74A       Area A_Temperature          NaN   \n",
+                            "1  84ED2BB0-AD0B-4C76-8233-EEA7EB358F97  Area B_Compressor Power          NaN   \n",
                             "\n",
                             "           Type Value Unit Of Measure Datasource Name  Archived  \n",
                             "0  StoredSignal                    \u00b0F    Example Data     False  \n",
                             "1  StoredSignal                    kW    Example Data     False  "
                         ]
                     },
                     "execution_count": 7,
@@ -893,15 +896,15 @@
                     "name": "#%%\n"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<div style=\"background-color: #EEFFEE;color:black;text-align: left;\">Query successful</div><table style=\"color:black;\"><tr><td style=\"background-color: #EEFFEE;\"></td><td style=\"background-color: #EEFFEE; text-align: left;\">Name</td><td style=\"background-color: #EEFFEE; text-align: left;\">Datasource Name</td><td style=\"background-color: #EEFFEE; text-align: left;\">Time</td><td style=\"background-color: #EEFFEE; text-align: right;\">Count</td><td style=\"background-color: #EEFFEE; text-align: left;\">Result</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">0</td><td style=\"text-align: left; vertical-align: top;\">Area ?_Compressor Stage</td><td style=\"text-align: left; vertical-align: top;\">Example Data</td><td style=\"vertical-align: top;\">00:00:00.16</td><td style=\"text-align: right; vertical-align: top;\">11</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr></table>"
+                            "<div style=\"background-color: #EEFFEE;color:black; text-align: left;\">Query successful</div><table class=\"tex2jax_ignore\" style=\"color:black;\"><tr><td style=\"background-color: #EEFFEE;\"></td><td style=\"background-color: #EEFFEE; text-align: left;\">Name</td><td style=\"background-color: #EEFFEE; text-align: left;\">Datasource Name</td><td style=\"background-color: #EEFFEE; text-align: left;\">Time</td><td style=\"background-color: #EEFFEE; text-align: right;\">Count</td><td style=\"background-color: #EEFFEE; text-align: right;\">Pages</td><td style=\"background-color: #EEFFEE; text-align: left;\">Result</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">0</td><td style=\"text-align: left; vertical-align: top;\">Area ?_Compressor Stage</td><td style=\"text-align: left; vertical-align: top;\">Example Data</td><td style=\"vertical-align: top;\">00:00:00.10</td><td style=\"text-align: right; vertical-align: top;\">11</td><td style=\"text-align: right; vertical-align: top;\">1</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr></table>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -981,33 +984,38 @@
                             "  <thead>\n",
                             "    <tr style=\"text-align: right;\">\n",
                             "      <th></th>\n",
                             "      <th>Name</th>\n",
                             "      <th>Datasource Name</th>\n",
                             "      <th>Time</th>\n",
                             "      <th>Count</th>\n",
+                            "      <th>Pages</th>\n",
                             "      <th>Result</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
                             "      <td>Area ?_Compressor Stage</td>\n",
                             "      <td>Example Data</td>\n",
-                            "      <td>0:00:00.155001</td>\n",
+                            "      <td>0:00:00.104033</td>\n",
                             "      <td>11</td>\n",
+                            "      <td>1</td>\n",
                             "      <td>Success</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
-                            "                      Name Datasource Name            Time  Count   Result\n",
-                            "0  Area ?_Compressor Stage    Example Data  0:00:00.155001     11  Success"
+                            "                      Name Datasource Name            Time  Count  Pages  \\\n",
+                            "0  Area ?_Compressor Stage    Example Data  0:00:00.104033     11      1   \n",
+                            "\n",
+                            "    Result  \n",
+                            "0  Success  "
                         ]
                     },
                     "execution_count": 10,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -1035,15 +1043,15 @@
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Help on function search in module seeq.spy._search:\n",
                         "\n",
-                        "search(query, *, all_properties=False, workbook='Data Lab >> Data Lab Analysis', recursive=True, ignore_unindexed_properties=True, include_archived=False, estimate_sample_period=None, order_by=None, quiet=False, status=None, session: Union[seeq.spy._session.Session, NoneType] = None)\n",
+                        "search(query, *, all_properties=False, workbook='Data Lab >> Data Lab Analysis', recursive=True, ignore_unindexed_properties=True, include_archived=False, estimate_sample_period=None, include_swappable_assets=False, old_asset_format=None, order_by=None, quiet=None, errors=None, status=None, session: 'Optional[Session]' = None)\n",
                         "    Issues a query to the Seeq Server to retrieve metadata for signals,\n",
                         "    conditions, scalars and assets. This metadata can then be used to retrieve\n",
                         "    samples, capsules for a particular time range via spy.pull().\n",
                         "    \n",
                         "    Parameters\n",
                         "    ----------\n",
                         "    query : {str, dict, list, pd.DataFrame, pd.Series}\n",
@@ -1076,40 +1084,43 @@
                         "        Property            Description\n",
                         "        =================== ===================================================\n",
                         "        Name                Name of the item (wildcards/regex supported)\n",
                         "        Path                Asset tree path of the item (should not include the\n",
                         "                            \"leaf\" asset), using ' >> ' hierarchy delimiters\n",
                         "        Asset               Asset name (i.e., the name of the leaf asset) or ID\n",
                         "        Type                The item type. One of 'Signal', 'Condition',\n",
-                        "                              'Scalar', 'Asset', 'Chart', 'Metric', 'Workbook',\n",
-                        "                              and 'Worksheet'\n",
+                        "                            'Scalar', 'Asset', 'Chart', 'Metric', 'Workbook',\n",
+                        "                            and 'Worksheet'\n",
                         "        Description         Description of the item (wildcards/regex supported)\n",
                         "        Datasource Name     Name of the datasource\n",
                         "        Datasource ID       The datasource ID, which corresponds to the Id\n",
                         "                            field in the connector configuration\n",
                         "        Datasource Class    The datasource class (e.g. 'OSIsoft PI')\n",
                         "        Data ID             The data ID, whose format is managed by the\n",
                         "                            datasource connector\n",
                         "        Cache Enabled       True to find items where data caching is enabled\n",
                         "        Scoped To           The Seeq ID of a workbook such that results are\n",
-                        "                              limited to ONLY items scoped to that workbook.\n",
+                        "                            limited to ONLY items scoped to that workbook.\n",
                         "        =================== ===================================================\n",
                         "    \n",
-                        "    \n",
                         "    all_properties : bool, default False\n",
                         "        True if all item properties should be retrieved. This currently makes\n",
                         "        the search operation much slower as retrieval of properties for an item\n",
                         "        requires a separate call.\n",
                         "    \n",
-                        "    workbook : {str, None}\n",
+                        "    workbook : {str, None}, default 'Data Lab >> Data Lab Analysis'\n",
                         "        A path string (with ' >> ' delimiters) or an ID to indicate a workbook\n",
                         "        such that, in addition to globally-scoped items, the workbook's scoped\n",
                         "        items will also be returned in the results.\n",
                         "    \n",
-                        "        If you want all items regardless of scope, use workbook=None.\n",
+                        "        If you want all items regardless of scope, use\n",
+                        "        workbook=spy.GLOBALS_AND_ALL_WORKBOOKS\n",
+                        "    \n",
+                        "        If you want only globally-scoped items, use\n",
+                        "        workbook=spy.GLOBALS_ONLY\n",
                         "    \n",
                         "        If you don't want globally-scoped items in your results, use the\n",
                         "        'Scoped To' field in the 'query' argument instead. (See 'query'\n",
                         "        argument documentation above.)\n",
                         "    \n",
                         "        The ID for a workbook is visible in the URL of Seeq Workbench, directly\n",
                         "        after the \"workbook/\" part.\n",
@@ -1135,22 +1146,39 @@
                         "        and end times are used to bound the calculation of the sample period.\n",
                         "        If the start and end times encompass a time range that is insufficient\n",
                         "        to determine the sample period, a pd.NaT will be returned.\n",
                         "        If the value of 'Start' is set to None, it will default to the value of\n",
                         "        'End' minus 1 hour. Conversely, if the value of 'End' is set to None,\n",
                         "        it will default to now.\n",
                         "    \n",
+                        "    include_swappable_assets : bool, default False\n",
+                        "        Adds a \"Swappable Assets\" column to the output where each cell is an\n",
+                        "        embedded DataFrame that includes the assets that the item refers to and\n",
+                        "        can theoretically be swapped for other assets using spy.swap().\n",
+                        "    \n",
+                        "    old_asset_format : bool, default True\n",
+                        "        Historically, spy.search() returned rows with a \"Type\" of \"Asset\" whereby\n",
+                        "        the \"Asset\" column was the name of the parent asset. This is inconsistent\n",
+                        "        with all other aspects of SPy, including spy.push(metadata). If you would\n",
+                        "        like Asset rows to instead be consistent with the rest of SPy (whereby\n",
+                        "        the \"Asset\" column is the name of the current asset, not the parent),\n",
+                        "        pass in False for this argument.\n",
+                        "    \n",
                         "    order_by : {str, list}, default None\n",
                         "        An optional field or list of fields used to sort the search results.\n",
                         "        Fields on which results can be sorted are 'ID', 'Name', and 'Description'.\n",
                         "    \n",
                         "    quiet : bool, default False\n",
                         "        If True, suppresses progress output. Note that when status is\n",
                         "        provided, the quiet setting of the Status object that is passed\n",
-                        "        in takes precedent.\n",
+                        "        in takes precedence.\n",
+                        "    \n",
+                        "    errors : {'raise', 'catalog'}, default 'raise'\n",
+                        "        If 'raise', any errors encountered will cause an exception. If 'catalog',\n",
+                        "        errors will be added to a 'Result' column in the status.df DataFrame.\n",
                         "    \n",
                         "    status : spy.Status, optional\n",
                         "        If specified, the supplied Status object will be updated as the command\n",
                         "        progresses. It gets filled in with the same information you would see\n",
                         "        in Jupyter in the blue/green/red table below your code while the\n",
                         "        command is executed. The table itself is accessible as a DataFrame via\n",
                         "        the status.df property.\n",
@@ -1162,37 +1190,39 @@
                         "    \n",
                         "    Returns\n",
                         "    -------\n",
                         "    pandas.DataFrame\n",
                         "        A DataFrame with rows for each item found and columns for each\n",
                         "        property.\n",
                         "    \n",
-                        "        Additionally, the following properties are stored in the\n",
-                        "        output DataFrame:\n",
+                        "        Additionally, the following properties are stored on the \"spy\"\n",
+                        "        attribute of the output DataFrame:\n",
                         "    \n",
                         "        =================== ===================================================\n",
                         "        Property            Description\n",
                         "        =================== ===================================================\n",
                         "        func                A str value of 'spy.search'\n",
                         "        kwargs              A dict with the values of the input parameters\n",
                         "                            passed to spy.search to get the output DataFrame\n",
+                        "        old_asset_format    True if the old Asset format was used (see doc for\n",
+                        "                            old_asset_format argument)\n",
                         "        status              A spy.Status object with the status of the\n",
                         "                            spy.search call\n",
                         "        =================== ===================================================\n",
                         "    \n",
                         "    Examples\n",
                         "    --------\n",
                         "    Search for signals with the name 'Humid' on the asset tree under\n",
                         "    'Example >> Cooling Tower 1', retrieving all properties on the results:\n",
                         "    \n",
                         "    >>> search_results = spy.search({'Name': 'Humid', 'Path': 'Example >> Cooling Tower 1'}, all_properties=True)\n",
                         "    \n",
                         "    To access the stored properties:\n",
-                        "    >>> search_results.kwargs\n",
-                        "    >>> search_results.status\n",
+                        "    >>> search_results.spy.kwargs\n",
+                        "    >>> search_results.spy.status\n",
                         "    \n",
                         "    Search for signals that have a name that starts with 'Area' in the datasource 'Example Data' and\n",
                         "    determine the sample period of each signal during the month of January 2018\n",
                         "    \n",
                         "    >>> search_results = spy.search({\n",
                         "    >>>    'Name': 'Area ?_*',\n",
                         "    >>>    'Datasource Name': 'Example Data'\n",
```

### Comparing `seeq-spy-187.5/seeq/spy/docs/Documentation/spy.widgets.ipynb` & `seeq-spy-188.0/seeq/spy/docs/Documentation/spy.widgets.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994565217391305%*

 * *Differences: {"'cells'": "{0: {'source': ['from seeq import spy\\n', '\\n', '# Set the compatibility option so "*

 * *            'that you maximize the chance that SPy will remain compatible with your '*

 * *            "notebook/script\\n', 'spy.options.compatibility = 188']}}"}*

```diff
@@ -6,15 +6,18 @@
             "metadata": {
                 "pycharm": {
                     "is_executing": false
                 }
             },
             "outputs": [],
             "source": [
-                "from seeq import spy"
+                "from seeq import spy\n",
+                "\n",
+                "# Set the compatibility option so that you maximize the chance that SPy will remain compatible with your notebook/script\n",
+                "spy.options.compatibility = 188"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {
                 "pycharm": {
```

### Comparing `seeq-spy-187.5/seeq/spy/docs/Documentation/spy.workbooks.ipynb` & `seeq-spy-188.0/seeq/spy/docs/Documentation/spy.workbooks.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999716300233197%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(2, 'from seeq import spy\\n'), (3, '\\n'), (4, '# Set the "*

 * *            'compatibility option so that you maximize the chance that SPy will remain compatible '*

 * *            "with your notebook/script\\n'), (5, 'spy.options.compatibility = 188')], delete: "*

 * *            "[2]}}, 27: {'outputs': {0: {'text': {insert: [(57, '        in takes "*

 * *            "precedence.\\n')], delete: [57]}}}}, 28: {'outputs': {0: {'text': {insert: [(50, "*

 * *            "'        in takes preced […]*

```diff
@@ -4,15 +4,18 @@
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import os\n",
                 "import shutil\n",
-                "from seeq import spy"
+                "from seeq import spy\n",
+                "\n",
+                "# Set the compatibility option so that you maximize the chance that SPy will remain compatible with your notebook/script\n",
+                "spy.options.compatibility = 188"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {},
             "outputs": [
@@ -1071,15 +1074,15 @@
                         "    \n",
                         "    include_archived : bool, default False\n",
                         "        True if archived (aka \"trashed\") folders/workbooks should be returned.\n",
                         "    \n",
                         "    quiet : bool, default False\n",
                         "        If True, suppresses progress output. Note that when status is\n",
                         "        provided, the quiet setting of the Status object that is passed\n",
-                        "        in takes precedent.\n",
+                        "        in takes precedence.\n",
                         "    \n",
                         "    status : spy.Status, optional\n",
                         "        If specified, the supplied Status object will be updated as the command\n",
                         "        progresses. It gets filled in with the same information you would see\n",
                         "        in Jupyter in the blue/green/red table below your code while the\n",
                         "        command is executed. The table itself is accessible as a DataFrame via\n",
                         "        the status.df property.\n",
@@ -1157,15 +1160,15 @@
                         "        'catalog', errors will be added to a 'Result' column in the status.df\n",
                         "        DataFrame (errors='catalog' must be combined with\n",
                         "        status=<Status object>).\n",
                         "    \n",
                         "    quiet : bool\n",
                         "        If True, suppresses progress output. Note that when status is\n",
                         "        provided, the quiet setting of the Status object that is passed\n",
-                        "        in takes precedent.\n",
+                        "        in takes precedence.\n",
                         "    \n",
                         "    status : spy.Status, optional\n",
                         "        If specified, the supplied Status object will be updated as the command\n",
                         "        progresses. It gets filled in with the same information you would see\n",
                         "        in Jupyter in the blue/green/red table below your code while the\n",
                         "        command is executed. The table itself is accessible as a DataFrame via\n",
                         "        the status.df property.\n",
@@ -1383,15 +1386,15 @@
                         "        'catalog', errors will be added to a 'Result' column in the status.df\n",
                         "        DataFrame (errors='catalog' must be combined with\n",
                         "        status=<Status object>).\n",
                         "    \n",
                         "    quiet : bool\n",
                         "        If True, suppresses progress output. Note that when status is\n",
                         "        provided, the quiet setting of the Status object that is passed\n",
-                        "        in takes precedent.\n",
+                        "        in takes precedence.\n",
                         "    \n",
                         "    status : spy.Status, optional\n",
                         "        If specified, the supplied Status object will be updated as the command\n",
                         "        progresses. It gets filled in with the same information you would see\n",
                         "        in Jupyter in the blue/green/red table below your code while the\n",
                         "        command is executed. The table itself is accessible as a DataFrame via\n",
                         "        the status.df property.\n",
```

### Comparing `seeq-spy-187.5/seeq/spy/docs/_copy.py` & `seeq-spy-188.0/seeq/spy/docs/_copy.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.5/seeq/spy/jobs/_execute.py` & `seeq-spy-188.0/seeq/spy/jobs/_execute.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.5/seeq/spy/jobs/_pull.py` & `seeq-spy-188.0/seeq/spy/jobs/_pull.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.5/seeq/spy/jobs/_push.py` & `seeq-spy-188.0/seeq/spy/jobs/_push.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
         in scenarios where you wish to work with a notebook interactively and
         temporarily prevent job execution. Remove the argument (or change it
         to False) when you are ready to resume job execution.
 
     quiet : bool, default False
         If True, suppresses progress output. Note that when status is
         provided, the quiet setting of the Status object that is passed
-        in takes precedent.
+        in takes precedence.
 
     status : spy.Status, optional
         If specified, the supplied Status object will be updated as the command
         progresses. It gets filled in with the same information you would see
         in Jupyter in the blue/green/red table below your code while the
         command is executed. The table itself is accessible as a DataFrame via
         the status.df property.
```

### Comparing `seeq-spy-187.5/seeq/spy/jobs/_schedule.py` & `seeq-spy-188.0/seeq/spy/jobs/_schedule.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
         in scenarios where you wish to work with a notebook interactively and
         temporarily "pause" job execution. Remove the argument (or change it
         to False) when you are ready to resume job execution.
 
     quiet : bool, default False
         If True, suppresses progress output. Note that when status is
         provided, the quiet setting of the Status object that is passed
-        in takes precedent.
+        in takes precedence.
 
     status : spy.Status, optional
         If specified, the supplied Status object will be updated as the command
         progresses. It gets filled in with the same information you would see
         in Jupyter in the blue/green/red table below your code while the
         command is executed. The table itself is accessible as a DataFrame via
         the status.df property.
@@ -163,15 +163,15 @@
         A value of '*' will unschedule all jobs across all labels associated
         with the supplied notebook (or the current Notebook, if no
         datalab_notebook_url is supplied).
 
     quiet : bool, default False
         If True, suppresses progress output. Note that when status is
         provided, the quiet setting of the Status object that is passed
-        in takes precedent.
+        in takes precedence.
 
     status : spy.Status, optional
         If specified, the supplied Status object will be updated as the command
         progresses. It gets filled in with the same information you would see
         in Jupyter in the blue/green/red table below your code while the
         command is executed. The table itself is accessible as a DataFrame via
         the status.df property.
@@ -421,18 +421,18 @@
     # Add-on Mode (voila) sets env var SCRIPT_NAME to the notebook path
     if datalab_notebook_url is None and len(os.getenv('SCRIPT_NAME', '')) > 0:
         datalab_notebook_url = os.environ['SCRIPT_NAME']
 
     if datalab_notebook_url is None:
         if _datalab.is_datalab():
             return _datalab.get_data_lab_orchestrator_url(use_private_url), _datalab.get_data_lab_project_id(), \
-                   _datalab.get_notebook_path(session)
+                _datalab.get_notebook_path(session)
         if _datalab.is_executor():
             return _datalab.get_data_lab_orchestrator_url(use_private_url), _datalab.get_data_lab_project_id(), \
-                   os.environ['SEEQ_SDL_FILE_PATH']
+                os.environ['SEEQ_SDL_FILE_PATH']
         else:
             raise SPyRuntimeError('Provide a Seeq Data Lab Notebook URL for scheduling')
     else:
         data_lab_url, project_id, file_path = parse_data_lab_url_project_id_and_path(datalab_notebook_url,
                                                                                      use_private_url)
         if not data_lab_url:
             if _datalab.is_datalab() or _datalab.is_executor():
@@ -454,15 +454,16 @@
 
 def parse_data_lab_url_project_id_and_path(notebook_url, use_private_url=True):
     matches = re.search(r'^(.*/data-lab)/([0-9A-F]{8}-[0-9A-F]{4}-[0-9A-F]{4}-[0-9A-F]{4}-[0-9A-F]{12})/[\w]+/(.*)',
                         notebook_url, re.IGNORECASE)
     if not matches:
         raise SPyValueError('URL is not a valid SDL notebook')
 
-    data_lab_url = _datalab.get_data_lab_orchestrator_url(use_private_url) if matches.group(1) == '/data-lab' else matches.group(1)
+    data_lab_url = _datalab.get_data_lab_orchestrator_url(use_private_url) if matches.group(
+        1) == '/data-lab' else matches.group(1)
     project_id = matches.group(2).upper()
     file_path = unquote(matches.group(3))
     return data_lab_url, project_id, file_path
 
 
 def _spread_over_period(cron_expressions, over_period):
     over_period_delta = _common.parse_str_time_to_timedelta(over_period)
```

### Comparing `seeq-spy-187.5/seeq/spy/notifications/_emails.py` & `seeq-spy-188.0/seeq/spy/notifications/_emails.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,15 +185,15 @@
     errors : {'raise', 'catalog'}, default 'raise'
         If 'raise', any errors encountered will cause an exception. If
         'catalog', errors will be added to a 'Result' column in the status.df
         DataFrame.
 
     quiet : bool, default False
         If True, suppresses output. Note that when status is provided,
-        the quiet setting of the Status object that is passed in takes precedent.
+        the quiet setting of the Status object that is passed in takes precedence.
 
     status : spy.Status, optional
         If specified, the supplied Status object will be updated as the command
         progresses. It gets filled in with the same information you would see
         in Jupyter in the blue/green/red table below your code while the
         command is executed. The table itself is accessible as a DataFrame via
         the status.df property.
```

### Comparing `seeq-spy-187.5/seeq/spy/utils/__init__.py` & `seeq-spy-188.0/seeq/spy/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.5/seeq/spy/widgets/_ipy_utils.py` & `seeq-spy-188.0/seeq/spy/widgets/_ipy_utils.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.5/seeq/spy/widgets/_widgets.py` & `seeq-spy-188.0/seeq/spy/widgets/_widgets.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.5/seeq/spy/workbooks/__init__.py` & `seeq-spy-188.0/seeq/spy/workbooks/__init__.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.5/seeq/spy/workbooks/_annotation.py` & `seeq-spy-188.0/seeq/spy/workbooks/_annotation.py`

 * *Files 0% similar despite different names*

```diff
@@ -312,15 +312,16 @@
             if any(interest_item.id == i.interest_id for i in new_annotation.interests):
                 continue
             if isinstance(self, Report) and interest_item.id == pushed_workbook_id:
                 # Reports cannot have an interest to the workbook, see CRAB-18738
                 continue
             new_interest = AnnotationInterestInputV1()
             new_interest.interest_id = interest_item.id
-            new_interest.detail_id = interest.capsule
+            if interest.capsule is not None:
+                new_interest.detail_id = interest.capsule.id
             new_annotation.interests.append(new_interest)
 
         new_annotation.created_by_id = relevant_annotation.created_by.id
         safely(lambda: annotations_api.update_annotation(id=relevant_annotation.id, body=new_annotation),
                action_description=f'update Annotation {relevant_annotation.id}',
                status=status)
```

### Comparing `seeq-spy-187.5/seeq/spy/workbooks/_content.py` & `seeq-spy-188.0/seeq/spy/workbooks/_content.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.5/seeq/spy/workbooks/_data.py` & `seeq-spy-188.0/seeq/spy/workbooks/_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,46 +5,39 @@
 import re
 from typing import List, Dict, Union, Optional
 
 import pandas as pd
 
 from seeq.base import util
 from seeq.sdk import *
-from seeq.spy import _common, _metadata, _search
+from seeq.spy import _common, _metadata
 from seeq.spy._errors import *
 from seeq.spy._redaction import safely
 from seeq.spy._session import Session
 from seeq.spy.workbooks._item import Item, ItemMap
 
 
 class StoredOrCalculatedItem(Item):
-    def __init__(self, definition=None):
-        super().__init__(definition)
+    def __init__(self, definition=None, *, provenance=None):
+        super().__init__(definition, provenance=provenance)
 
         self.scoped_to = None
 
     def _populate_asset_and_path(self, session: Session, item_id, status):
         trees_api = TreesApi(session.client)
         asset_tree_output = safely(
             lambda: trees_api.get_tree(id=item_id),
             action_description=f'get Tree information for {item_id}',
             status=status)  # type: AssetTreeOutputV1
         if asset_tree_output is None or asset_tree_output.item is None:
             return
 
         ancestors = [a.name for a in asset_tree_output.item.ancestors]
-        if len(ancestors) >= 2:
-            self.definition['Path'] = _common.path_list_to_string(ancestors[0:-1])
-            self.definition['Asset'] = ancestors[-1]
-        elif len(ancestors) == 1:
-            self.definition['Path'] = None
-            self.definition['Asset'] = ancestors[0]
-        else:
-            self.definition['Path'] = None
-            self.definition['Asset'] = None
+
+        _common.add_ancestors_to_definition(self.type, self.name, ancestors, self.definition, old_asset_format=False)
 
     def _pull(self, session: Session, item_id, status):
         super()._pull(session, item_id, status)
 
         if 'Path' not in self.definition:
             self._populate_asset_and_path(session, item_id, status)
 
@@ -299,14 +292,15 @@
         # helps when mapping, for example, an AF tree to a Data Lab tree.
         for t in ['Signal', 'Condition', 'Scalar', 'Datasource']:
             if t in new_definition['Type']:
                 new_definition['Type'] = t
 
         if new_definition['Type'] not in ['User', 'UserGroup']:
             query_df = pd.DataFrame([new_definition])
+            from seeq.spy import _search
             if 'Path' in new_definition:
                 # If we're matching based on path, unfortunately we will not be able to match against archived items
                 # due to a limitation of the API. See CRAB-18439.
                 search_df = _search.search(query_df, workbook=pushed_workbook_id, recursive=False,
                                            ignore_unindexed_properties=False, session=session, quiet=True)
             else:
                 search_df = _search.search(query_df, workbook=pushed_workbook_id, include_archived=True,
@@ -379,15 +373,27 @@
                                                property_name='Override Maximum Interpolation',
                                                body=src_max_interp)
 
         return item
 
 
 class Asset(StoredItem):
-    pass
+    def __init__(self, definition=None, *, provenance=None):
+        super().__init__(definition, provenance=provenance)
+
+        if self.provenance == Item.LOAD:
+            if self.definition.get('Old Asset Format', True):
+                if self.type == 'Asset':
+                    if self.definition.get('Path') in [None, '']:
+                        self.definition['Path'] = self.definition['Asset']
+                    else:
+                        self.definition['Path'] += ' >> ' + self.definition['Asset']
+                        self.definition['Asset'] = self.definition['Name']
+
+        self.definition['Old Asset Format'] = False
 
 
 class Datasource(StoredItem):
     @staticmethod
     def from_datasource_output(datasource_output: Union[DatasourceOutputV1, DatasourcePreviewV1]):
         return Datasource({
             'ID': datasource_output.id,
```

### Comparing `seeq-spy-187.5/seeq/spy/workbooks/_folder.py` & `seeq-spy-188.0/seeq/spy/workbooks/_folder.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,14 @@
         folder_output = safely(lambda: folders_api.get_folder(folder_id=item_id),
                                action_description=f'get Folder {item_id}',
                                status=status)  # type: FolderOutputV1
         if folder_output is None:
             return
         self._pull_owner_and_acl(session, folder_output.owner, status)
         self._pull_ancestors(session, folder_output.ancestors)
-        self._provenance = Item.PULL
 
     def _pull_ancestors(self, session: Session, ancestors: List[ItemPreviewV1]):
         super()._pull_ancestors(session, ancestors)
         massage_ancestors(session, self)
 
     def _find_by_name(self, session: Session, folder_id, status: Status):
         folders_api = FoldersApi(session.client)
```

### Comparing `seeq-spy-187.5/seeq/spy/workbooks/_item.py` & `seeq-spy-188.0/seeq/spy/workbooks/_item.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     available_types = dict()
 
     CONSTRUCTOR = 'CONSTRUCTOR'
     PULL = 'PULL'
     LOAD = 'LOAD'
     TEMPLATE = 'TEMPLATE'
 
-    def __init__(self, definition=None):
+    def __init__(self, definition=None, *, provenance=None):
         if isinstance(definition, Item):
             definition = definition.definition_dict
 
         _common.validate_argument_types([(definition, 'definition', dict)])
 
         self._definition = definition if definition else dict()
         self._datasource = None
@@ -51,15 +51,15 @@
             if self._definition['Type'] in ['Analysis', 'Topic']:
                 self._definition['Type'] = 'Workbook'
             if 'Worksheet' in self._definition['Type']:
                 self._definition['Type'] = 'Worksheet'
             if 'Workstep' in self._definition['Type']:
                 self._definition['Type'] = 'Workstep'
 
-        self._provenance = Item.CONSTRUCTOR
+        self._provenance = Item.CONSTRUCTOR if provenance is None else provenance
 
     def __contains__(self, key):
         return _common.present(self._definition, key)
 
     def __getitem__(self, key):
         return _common.get(self._definition, key)
 
@@ -88,23 +88,15 @@
     @property
     def fqn(self):
         """
         The "fully qualified name" (FQN) of this item, which includes the Path and Asset (if present).
         For example: "Example >> Cooling Tower 1 >> Area A >> Temperature"
         :return: The fully qualified name of this item.
         """
-        parts = list()
-        if _common.present(self.definition, 'Path'):
-            parts.append(_common.get(self.definition, 'Path'))
-        if self.type != 'Asset' and _common.present(self.definition, 'Asset'):
-            parts.append(_common.get(self.definition, 'Asset'))
-        if _common.present(self.definition, 'Name'):
-            parts.append(_common.get(self.definition, 'Name'))
-
-        return ' >> '.join(parts)
+        return _common.fqn_from_row(self.definition)
 
     @property
     def id(self):
         return _common.get(self.definition, 'ID')
 
     @property
     def name(self):
@@ -279,27 +271,26 @@
         if item_output is None:
             return None
         definition = Item._dict_from_item_output(item_output)
         if allowed_types and definition['Type'] not in allowed_types:
             return None
 
         derived_class = Item._get_derived_class(definition['Type'])
-        item = derived_class(definition)  # type: Item
+        item = derived_class(definition, provenance=Item.PULL)  # type: Item
         item._pull(session, item_id, status)
         item._datasource = item_output.datasource
         return item
 
     def _pull(self, session: Session, item_id: str, status: Status):
-        self._provenance = Item.PULL
+        pass
 
     @staticmethod
     def load(definition):
         derived_class = Item._get_derived_class(definition['Type'])
-        item = derived_class(definition)
-        item._provenance = Item.LOAD
+        item = derived_class(definition, provenance=Item.LOAD)
         return item
 
     def _set_formula_based_item_properties(self, calculated_item):
         self._definition['Formula'] = Item.formula_list_from_string(self._definition['Formula'])
         self._definition['Formula Parameters'] = dict()
         for parameter in calculated_item.parameters:  # type: FormulaParameterOutputV1
             if parameter.item:
```

### Comparing `seeq-spy-187.5/seeq/spy/workbooks/_item_map.py` & `seeq-spy-188.0/seeq/spy/workbooks/_item_map.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.5/seeq/spy/workbooks/_load.py` & `seeq-spy-188.0/seeq/spy/workbooks/_load.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.5/seeq/spy/workbooks/_mustache.py` & `seeq-spy-188.0/seeq/spy/workbooks/_mustache.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.5/seeq/spy/workbooks/_pull.py` & `seeq-spy-188.0/seeq/spy/workbooks/_pull.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         'catalog', errors will be added to a 'Result' column in the status.df
         DataFrame (errors='catalog' must be combined with
         status=<Status object>).
 
     quiet : bool
         If True, suppresses progress output. Note that when status is
         provided, the quiet setting of the Status object that is passed
-        in takes precedent.
+        in takes precedence.
 
     status : spy.Status, optional
         If specified, the supplied Status object will be updated as the command
         progresses. It gets filled in with the same information you would see
         in Jupyter in the blue/green/red table below your code while the
         command is executed. The table itself is accessible as a DataFrame via
         the status.df property.
```

### Comparing `seeq-spy-187.5/seeq/spy/workbooks/_push.py` & `seeq-spy-188.0/seeq/spy/workbooks/_push.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,15 +157,15 @@
         'catalog', errors will be added to a 'Result' column in the status.df
         DataFrame (errors='catalog' must be combined with
         status=<Status object>).
 
     quiet : bool, default False
         If True, suppresses progress output. Note that when status is
         provided, the quiet setting of the Status object that is passed
-        in takes precedent.
+        in takes precedence.
 
     status : spy.Status, optional
         If specified, the supplied Status object will be updated as the command
         progresses. It gets filled in with the same information you would see
         in Jupyter in the blue/green/red table below your code while the
         command is executed. The table itself is accessible as a DataFrame via
         the status.df property.
```

### Comparing `seeq-spy-187.5/seeq/spy/workbooks/_render.py` & `seeq-spy-188.0/seeq/spy/workbooks/_render.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.5/seeq/spy/workbooks/_report_content_utilities.py` & `seeq-spy-188.0/seeq/spy/workbooks/_report_content_utilities.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.5/seeq/spy/workbooks/_save.py` & `seeq-spy-188.0/seeq/spy/workbooks/_save.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.5/seeq/spy/workbooks/_search.py` & `seeq-spy-188.0/seeq/spy/workbooks/_search.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
     errors : {'raise', 'catalog'}, default 'raise'
         If 'raise', any errors encountered will cause an exception. If 'catalog',
         errors will be added to a 'Result' column in the status.df DataFrame.
 
     quiet : bool, default False
         If True, suppresses progress output. Note that when status is
         provided, the quiet setting of the Status object that is passed
-        in takes precedent.
+        in takes precedence.
 
     status : spy.Status, optional
         If specified, the supplied Status object will be updated as the command
         progresses. It gets filled in with the same information you would see
         in Jupyter in the blue/green/red table below your code while the
         command is executed. The table itself is accessible as a DataFrame via
         the status.df property.
```

### Comparing `seeq-spy-187.5/seeq/spy/workbooks/_template.py` & `seeq-spy-188.0/seeq/spy/workbooks/_template.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.5/seeq/spy/workbooks/_user.py` & `seeq-spy-188.0/seeq/spy/workbooks/_user.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.5/seeq/spy/workbooks/_workbook.py` & `seeq-spy-188.0/seeq/spy/workbooks/_workbook.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,19 +48,19 @@
 
     def __new__(cls, *args, **kwargs):
         if cls is Workbook:
             raise SPyTypeError("Workbook may not be instantiated directly, create either Analysis or Topic")
 
         return object.__new__(cls)
 
-    def __init__(self, definition=None):
+    def __init__(self, definition=None, *, provenance=None):
         if isinstance(definition, str):
             definition = {'Name': definition}
 
-        super().__init__(definition)
+        super().__init__(definition, provenance=provenance)
 
         self.status = None
         self._item_inventory = dict()
         self.worksheets = WorksheetList(self)
         self._datasource_maps = list()
         self._scoped_items = None
         self._datasource_inventory = dict()
@@ -201,15 +201,15 @@
             self._datasource_inventory = new_item.datasource_inventory
             self._datasource_maps = new_item.datasource_maps
 
         finally:
             self.status = None
 
     @staticmethod
-    def _instantiate(definition=None):
+    def _instantiate(definition=None, *, provenance=None):
         if definition['Type'] == 'Workbook':
             if 'Workbook Type' not in definition:
                 if 'Data' not in definition or _common.get_workbook_type(definition['Data']) == 'Analysis':
                     definition['Workbook Type'] = 'Analysis'
                 else:
                     definition['Workbook Type'] = 'Topic'
         elif definition['Type'] in ['Analysis', 'Topic']:
@@ -218,31 +218,31 @@
             # property.
             definition['Workbook Type'] = definition['Type']
             definition['Type'] = 'Workbook'
         else:
             raise SPyValueError(f"Unrecognized workbook type: {definition['Type']}")
 
         if definition['Workbook Type'] == 'Analysis':
-            return Analysis(definition)
+            return Analysis(definition, provenance=provenance)
         elif definition['Workbook Type'] == 'Topic':
-            return Topic(definition)
+            return Topic(definition, provenance=provenance)
 
     @staticmethod
     def pull(item_id, *, status=None, extra_workstep_tuples=None, include_inventory=True, include_annotations=True,
              include_images=True, specific_worksheet_ids: Optional[List[str]] = None,
              session: Optional[Session] = None):
         status = Status.validate(status)
         session = Session.validate(session)
         item_output = safely(lambda: Item._get_item_output(session, item_id),
                              action_description=f'pull Workbook {item_id}',
                              status=status)
         if item_output is None:
             return
         definition = Item._dict_from_item_output(item_output)
-        workbook = Workbook._instantiate(definition)
+        workbook = Workbook._instantiate(definition, provenance=Item.PULL)
         workbook._pull(session, workbook_id=workbook.id, extra_workstep_tuples=extra_workstep_tuples,
                        include_inventory=include_inventory, include_annotations=include_annotations,
                        include_images=include_images, specific_worksheet_ids=specific_worksheet_ids, status=status)
         return workbook
 
     def pull_rendered_content(self, session: Session, status: Status):
         pass
@@ -261,16 +261,14 @@
                                      status=self.status)  # type: WorkbookOutputV1
             if workbook_output is None:
                 return
 
             self._definition['Path'] = _common.path_list_to_string([a.name for a in workbook_output.ancestors])
             self._definition['Workbook Type'] = _common.get_workbook_type(workbook_output)
 
-            self._provenance = Item.PULL
-
             self._pull_owner_and_acl(session, workbook_output.owner, self.status)
             self._pull_ancestors(session, workbook_output.ancestors)
 
             self.update_status('Pulling workbook', 1)
 
             if 'workbookState' in self._definition:
                 self._definition['workbookState'] = json.loads(self._definition['workbookState'])
@@ -763,22 +761,20 @@
         workbook_json_file = Workbook._get_workbook_json_file(workbook_folder)
         if not os.path.exists(workbook_json_file):
             raise SPyRuntimeError('Workbook JSON file "%s" does not exist' % workbook_json_file)
 
         with open(workbook_json_file, 'r', encoding='utf-8') as f:
             definition = json.load(f)
 
-        workbook = Workbook._instantiate(definition)
+        workbook = Workbook._instantiate(definition, provenance=Item.LOAD)
         workbook._load(workbook_folder)
 
         return workbook
 
     def _load(self, workbook_folder):
-        self._provenance = Item.LOAD
-
         self.worksheets = WorksheetList(self)
         for worksheet_id in self.definition['Worksheets']:
             Worksheet.load_from_workbook_folder(self, workbook_folder, worksheet_id)
 
         del self._definition['Worksheets']
 
         self._item_inventory = Workbook._load_inventory(Workbook._get_items_json_file(workbook_folder))
```

### Comparing `seeq-spy-187.5/seeq/spy/workbooks/_worksheet.py` & `seeq-spy-188.0/seeq/spy/workbooks/_worksheet.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,16 +33,16 @@
     def __new__(cls, *args, **kwargs):
         if cls is Worksheet:
             raise SPyTypeError("Worksheet may not be instantiated directly, create either AnalysisWorksheet or "
                                "TopicWorksheet")
 
         return object.__new__(cls)
 
-    def __init__(self, workbook, definition=None, add_defaults=True):
-        super().__init__(definition)
+    def __init__(self, workbook, definition=None, *, provenance=None, add_defaults=True):
+        super().__init__(definition, provenance=provenance)
 
         if workbook is None:
             raise SPyValueError("A Workbook is required to create a Worksheet")
 
         self.workbook = workbook
         self.workbook.worksheets.append(self)
 
@@ -71,19 +71,19 @@
 
     @property
     @deprecated(reason='Use either journal (for AnalysisWorksheet) or report (for TopicDocument) property instead')
     def document(self):
         return self._annotation
 
     @staticmethod
-    def _instantiate(workbook, definition=None):
+    def _instantiate(workbook, definition=None, *, provenance=None):
         if workbook['Workbook Type'] == 'Analysis':
-            return AnalysisWorksheet(workbook, definition)
+            return AnalysisWorksheet(workbook, definition, provenance=provenance)
         else:
-            return TopicDocument(workbook, definition)
+            return TopicDocument(workbook, definition, provenance=provenance)
 
     @staticmethod
     def pull(item_id, *, workbook=None, extra_workstep_tuples=None, include_annotations=True, include_images=True,
              session: Optional[Session] = None, status=None):
         session = Session.validate(session)
         status = Status.validate(status)
 
@@ -95,25 +95,23 @@
             action_description=f'get properties of worksheet {item_id}',
             status=Status(errors='catalog'))
         if definition is None:
             if status.errors == 'catalog':
                 return
             else:
                 raise SPyRuntimeError(f'Worksheet with ID "{item_id}" does not exist')
-        worksheet = Worksheet._instantiate(workbook, definition)
+        worksheet = Worksheet._instantiate(workbook, definition, provenance=Item.PULL)
         worksheet.pull_worksheet(session, item_id, extra_workstep_tuples=extra_workstep_tuples,
                                  include_annotations=include_annotations, include_images=include_images, status=status)
         return worksheet
 
     def pull_worksheet(self, session: Session, worksheet_id, extra_workstep_tuples=None, include_images=True,
                        status=None, include_annotations=True):
         status = Status.validate(status)
 
-        self._provenance = Item.PULL
-
         if include_images and not include_annotations:
             raise SPyValueError('Must specify include_images=False if you specify include_annotations=False')
 
         if include_annotations:
             self._annotation.pull(session, include_images=include_images, status=status)
 
         link_url = _url.SeeqURL.parse(session.public_url)
@@ -218,31 +216,29 @@
 
     def _load(self, workbook_folder, worksheet_id):
         worksheet_json_file = Worksheet._get_worksheet_json_file(workbook_folder, worksheet_id)
 
         with open(worksheet_json_file, 'r', encoding='utf-8') as f:
             self._definition = json.load(f)
 
-        self._provenance = Item.LOAD
-
         if self.workbook['Workbook Type'] == 'Analysis':
             self._annotation = Journal.load(self, workbook_folder)
         else:
             self._annotation = Report.load(self, workbook_folder)
 
         self.worksteps = dict()
         workstep_files = glob.glob(os.path.join(workbook_folder, 'Worksheet_%s_Workstep_*.json' % worksheet_id))
         for workstep_file in workstep_files:
             match = re.match(r'.*?Worksheet_.*?_Workstep_(.*?).json$', workstep_file)
             workstep_id = match.group(1)
             self.worksteps[workstep_id] = Workstep.load_from_workbook_folder(self, workbook_folder, workstep_id)
 
     @staticmethod
     def load_from_workbook_folder(workbook, workbook_folder, worksheet_id):
-        worksheet = Worksheet._instantiate(workbook)
+        worksheet = Worksheet._instantiate(workbook, provenance=Item.LOAD)
         worksheet._load(workbook_folder, worksheet_id)
         return worksheet
 
     @property
     def timezone(self):
         """
         The string name of the worksheet's current timezone or None if one is not set
@@ -396,15 +392,15 @@
         user interface.
 
         Parameters
         ----------
         quiet : bool, default False
             If True, suppresses progress output. Note that when status is
             provided, the quiet setting of the Status object that is passed
-            in takes precedent.
+            in takes precedence.
 
         status : spy.Status, optional
             If specified, the supplied Status object will be updated as the command
             progresses. It gets filled in with the same information you would see
             in Jupyter in the blue/green/red table below your code while the
             command is executed. The table itself is accessible as a DataFrame via
             the status.df property.
@@ -430,15 +426,15 @@
         Pushes a new workstep for the given worksheet using the current in-memory value given by current_workstep().
 
         Parameters
         ----------
         quiet : bool, default False
             If True, suppresses progress output. Note that when status is
             provided, the quiet setting of the Status object that is passed
-            in takes precedent.
+            in takes precedence.
 
         status : spy.Status, optional
             If specified, the supplied Status object will be updated as the command
             progresses. It gets filled in with the same information you would see
             in Jupyter in the blue/green/red table below your code while the
             command is executed. The table itself is accessible as a DataFrame via
             the status.df property.
```

### Comparing `seeq-spy-187.5/seeq/spy/workbooks/_workstep.py` & `seeq-spy-188.0/seeq/spy/workbooks/_workstep.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.5/seeq/spy/workbooks/app.css` & `seeq-spy-188.0/seeq/spy/workbooks/app.css`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.5/seeq_spy.egg-info/PKG-INFO` & `seeq-spy-188.0/seeq_spy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seeq-spy
-Version: 187.5
+Version: 188.0
 Summary: Easy-to-use Python interface for Seeq
 Home-page: https://www.seeq.com
 Author: Seeq Corporation
 Author-email: support@seeq.com
 Project-URL: Documentation, https://python-docs.seeq.com/
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
@@ -31,16 +31,14 @@
 - Import data in a programmatic way (when Seeq Workbench's *CSV Import* capability won't cut it)
 - Calculate new data in Python and push it into Seeq
 - Create an asset model
 - Programmatically create and manipulate Workbench Analyses or Organizer Topics
 
 **Use of the SPy module requires Python 3.7 or later.**
 
-**SPy version 187 and higher is compatible with Pandas 2.x.**
-
 To start exploring the SPy module, execute the following lines of code in Jupyter:
 
 ```
 from seeq import spy
 spy.docs.copy()
 ```
```

### Comparing `seeq-spy-187.5/seeq_spy.egg-info/SOURCES.txt` & `seeq-spy-188.0/seeq_spy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 seeq/spy/_plot.py
 seeq/spy/_pull.py
 seeq/spy/_push.py
 seeq/spy/_redaction.py
 seeq/spy/_search.py
 seeq/spy/_session.py
 seeq/spy/_status.py
+seeq/spy/_swap.py
 seeq/spy/_upgrade.py
 seeq/spy/_url.py
 seeq/spy/acl/__init__.py
 seeq/spy/acl/_pull.py
 seeq/spy/acl/_push.py
 seeq/spy/addons/__init__.py
 seeq/spy/addons/_install.py
@@ -63,14 +64,15 @@
 seeq/spy/docs/Documentation/Workbook Templates.ipynb
 seeq/spy/docs/Documentation/spy.acl.ipynb
 seeq/spy/docs/Documentation/spy.jobs.ipynb
 seeq/spy/docs/Documentation/spy.login.ipynb
 seeq/spy/docs/Documentation/spy.pull.ipynb
 seeq/spy/docs/Documentation/spy.push.ipynb
 seeq/spy/docs/Documentation/spy.search.ipynb
+seeq/spy/docs/Documentation/spy.swap.ipynb
 seeq/spy/docs/Documentation/spy.widgets.ipynb
 seeq/spy/docs/Documentation/spy.workbooks.ipynb
 seeq/spy/docs/Documentation/Administration/User Migration.ipynb
 seeq/spy/docs/Documentation/Advanced Scheduling/Email Notification Add-on Installer.ipynb
 seeq/spy/docs/Documentation/Advanced Scheduling/Email Notification Scheduler.ipynb
 seeq/spy/docs/Documentation/Advanced Scheduling/Email Notifier.ipynb
 seeq/spy/docs/Documentation/Advanced Scheduling/Email Unsubscriber.ipynb
```

### Comparing `seeq-spy-187.5/setup.py` & `seeq-spy-188.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="seeq-spy",
-    version="187.5",
+    version="188.0",
     author="Seeq Corporation",
     author_email="support@seeq.com",
     description="Easy-to-use Python interface for Seeq",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.seeq.com",
     project_urls={
```

