# Comparing `tmp/jipdate-0.0.1.tar.gz` & `tmp/jipdate-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jipdate-0.0.1.tar", last modified: Thu Nov 18 20:23:58 2021, max compression
+gzip compressed data, was "jipdate-2.0.1.tar", last modified: Thu Jun  1 13:23:57 2023, max compression
```

## Comparing `jipdate-0.0.1.tar` & `jipdate-2.0.1.tar`

### file list

```diff
@@ -1,23 +1,25 @@
--rw-r--r--   0        0        0       66 2021-11-18 11:13:21.829134 jipdate-0.0.1/.gitignore
--rw-r--r--   0        0        0     1063 2021-11-18 11:13:21.829134 jipdate-0.0.1/LICENSE
--rw-r--r--   0        0        0      460 2021-11-18 11:13:21.829134 jipdate-0.0.1/README.md
--rw-r--r--   0        0        0      604 2021-11-18 11:13:21.829134 jipdate-0.0.1/docs/Makefile
--rw-r--r--   0        0        0      142 2021-11-18 11:13:21.829134 jipdate-0.0.1/docs/_static/css/mystyle.css
--rw-r--r--   0        0        0      618 2021-11-18 11:13:21.829134 jipdate-0.0.1/docs/about.rst
--rw-r--r--   0        0        0     5130 2021-11-18 11:13:21.829134 jipdate-0.0.1/docs/conf.py
--rw-r--r--   0        0        0     7241 2021-11-18 11:13:21.829134 jipdate-0.0.1/docs/config.rst
--rw-r--r--   0        0        0      167 2021-11-18 11:13:21.829134 jipdate-0.0.1/docs/index.rst
--rw-r--r--   0        0        0     2086 2021-11-18 11:13:21.829134 jipdate-0.0.1/docs/install.rst
--rw-r--r--   0        0        0     5789 2021-11-18 11:13:21.829134 jipdate-0.0.1/docs/jipdate.rst
--rw-r--r--   0        0        0     2299 2021-11-18 11:13:21.829134 jipdate-0.0.1/docs/jipstatus.rst
--rw-r--r--   0        0        0     1576 2021-11-18 11:13:21.829134 jipdate-0.0.1/docs/problems.rst
--rw-r--r--   0        0        0     1465 2021-11-18 11:13:21.829134 jipdate-0.0.1/docs/run.rst
--rw-r--r--   0        0        0       57 2021-11-18 15:00:28.288808 jipdate-0.0.1/jipdate/__init__.py
--rw-r--r--   0        0        0     3410 2021-11-18 11:13:51.765435 jipdate-0.0.1/jipdate/cfg.py
--rwxr-xr-x   0        0        0    19026 2021-11-18 11:13:51.765435 jipdate-0.0.1/jipdate/jipdate.py
--rwxr-xr-x   0        0        0    19865 2021-11-18 11:13:51.765435 jipdate-0.0.1/jipdate/jipfp.py
--rwxr-xr-x   0        0        0     9694 2021-11-18 11:13:51.765435 jipdate-0.0.1/jipdate/jipstatus.py
--rw-r--r--   0        0        0     3610 2021-11-18 11:13:51.769435 jipdate-0.0.1/jipdate/jiralogin.py
--rw-r--r--   0        0        0      571 2021-11-18 14:23:34.537483 jipdate-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      771 1970-01-01 00:00:00.000000 jipdate-0.0.1/setup.py
--rw-r--r--   0        0        0      848 1970-01-01 00:00:00.000000 jipdate-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       66 2022-01-05 21:22:55.225653 jipdate-2.0.1/.gitignore
+-rw-r--r--   0        0        0     1063 2021-09-27 12:17:51.864950 jipdate-2.0.1/LICENSE
+-rw-r--r--   0        0        0      460 2022-01-05 21:22:55.225653 jipdate-2.0.1/README.md
+-rw-r--r--   0        0        0      604 2022-01-05 21:22:55.225653 jipdate-2.0.1/docs/Makefile
+-rw-r--r--   0        0        0      142 2022-01-05 21:22:55.225653 jipdate-2.0.1/docs/_static/css/mystyle.css
+-rw-r--r--   0        0        0      618 2022-01-05 21:22:55.225653 jipdate-2.0.1/docs/about.rst
+-rw-r--r--   0        0        0     5130 2022-01-05 21:22:55.225653 jipdate-2.0.1/docs/conf.py
+-rw-r--r--   0        0        0     7345 2022-01-12 10:13:55.631749 jipdate-2.0.1/docs/config.rst
+-rw-r--r--   0        0        0      181 2023-05-31 10:40:14.000989 jipdate-2.0.1/docs/index.rst
+-rw-r--r--   0        0        0     2700 2023-06-01 13:10:59.581924 jipdate-2.0.1/docs/install.rst
+-rw-r--r--   0        0        0     2195 2023-05-31 10:40:14.012989 jipdate-2.0.1/docs/jipcreate.rst
+-rw-r--r--   0        0        0     6277 2023-05-31 10:40:14.004989 jipdate-2.0.1/docs/jipdate.rst
+-rw-r--r--   0        0        0     2259 2023-05-31 10:40:14.004989 jipdate-2.0.1/docs/jipstatus.rst
+-rw-r--r--   0        0        0     1576 2022-01-05 21:22:55.225653 jipdate-2.0.1/docs/problems.rst
+-rw-r--r--   0        0        0     1461 2023-05-31 10:40:14.004989 jipdate-2.0.1/docs/run.rst
+-rw-r--r--   0        0        0       57 2023-06-01 13:23:12.698786 jipdate-2.0.1/jipdate/__init__.py
+-rw-r--r--   0        0        0     3547 2023-05-31 10:40:13.992989 jipdate-2.0.1/jipdate/cfg.py
+-rwxr-xr-x   0        0        0    10353 2023-05-31 10:40:14.016989 jipdate-2.0.1/jipdate/jipcreate.py
+-rwxr-xr-x   0        0        0    19627 2023-05-31 10:40:14.016989 jipdate-2.0.1/jipdate/jipdate.py
+-rwxr-xr-x   0        0        0    19865 2023-05-31 10:40:13.992989 jipdate-2.0.1/jipdate/jipfp.py
+-rwxr-xr-x   0        0        0     8518 2023-06-01 13:13:27.390894 jipdate-2.0.1/jipdate/jipsearch.py
+-rwxr-xr-x   0        0        0     9912 2023-05-31 10:40:13.992989 jipdate-2.0.1/jipdate/jipstatus.py
+-rw-r--r--   0        0        0     3610 2023-05-31 10:40:13.992989 jipdate-2.0.1/jipdate/jiralogin.py
+-rw-r--r--   0        0        0      664 2023-06-01 12:33:43.359601 jipdate-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0      879 1970-01-01 00:00:00.000000 jipdate-2.0.1/PKG-INFO
```

### Comparing `jipdate-0.0.1/LICENSE` & `jipdate-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jipdate-0.0.1/docs/Makefile` & `jipdate-2.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `jipdate-0.0.1/docs/about.rst` & `jipdate-2.0.1/docs/about.rst`

 * *Files identical despite different names*

### Comparing `jipdate-0.0.1/docs/conf.py` & `jipdate-2.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jipdate-0.0.1/docs/config.rst` & `jipdate-2.0.1/docs/config.rst`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,18 @@
     version: 1
 
     # Jira server information
     #server:
     #  url: https://linaro.atlassian.net
     #  token: abcdefghijkl
 
+    #test_server:
+    #  url: https://<name_of_test_instance>.atlassian.net
+    #  token: abcdefghijkl
+
     # Extra comments added to each Jira issue (multiline is OK)
     comments:
         - "# No updates since last week."
 
     # Header of the file (multiline is OK). It will be followed by
     header:
         - |
```

### Comparing `jipdate-0.0.1/docs/install.rst` & `jipdate-2.0.1/docs/install.rst`

 * *Files 12% similar despite different names*

```diff
@@ -23,42 +23,68 @@
 
     Jipdate is **Python3** only! So at line 2 (*python3-pip*) and 5 (*pip3*) you
     have to adjust accordingly. I.e., if Python3 is default on your distro, then
     it might be that the package is simply ``python-pip`` (like on Arch Linux
     for example). The important message is that you **only** use Jipdate with
     Python3!
 
+Install jipdate with pip
+=============================
+.. code-block:: bash
+    :linenos:
+    :emphasize-lines: 3, 6
+
+    $ pip3 install --user jipdate
+
 Ubuntu / Debian based systems
 =============================
 .. code-block:: bash
     :linenos:
     :emphasize-lines: 3, 6
 
-    $ sudo apt update 
-    $ sudo apt upgrade
     $ sudo apt install python3-pip git
     $ git clone https://github.com/Linaro/jipdate.git
     $ cd jipdate
-    $ pip3 install --user -r requirements.txt 
+    $ pip3 install --user flit
+    $ flit build
+    $ flit install --symlink
 
 Fedora / Red Hat based systems
 ==============================
 .. code-block:: bash
     :linenos:
     :emphasize-lines: 2, 4
 
     $ sudo dnf -y install python3-pyyaml python3-jira
     $ git clone https://github.com/Linaro/jipdate.git
     $ cd jipdate
-    $ pip3 install --user -r requirements.txt
+    $ pip3 install --user flit
+    $ flit build
+    $ flit install --symlink
 
 Arch Linux
 ==========
 .. code-block:: bash
     :linenos:
     :emphasize-lines: 2, 5
 
     $ sudo pacman -Syu
     $ sudo pacman -S extra/git extra/python extra/python-pip
     $ git clone https://github.com/Linaro/jipdate.git
     $ cd jipdate
-    $ pip3 install --user -r requirements.txt 
+    $ pip3 install --user flit
+    $ flit build
+    $ flit install --symlink
+
+Mac OS (v12 Monterey or later)
+==============================
+.. code-block:: bash
+    :linenos:   
+    :emphasize-lines: 1, 3, 5
+    
+    $ /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
+    $ brew install python git
+    $ git clone https://github.com/Linaro/jipdate.git
+    $ cd jipdate
+    $ pip3 install --user flit
+    $ flit build
+    $ flit install --symlink
```

### Comparing `jipdate-0.0.1/docs/jipdate.rst` & `jipdate-2.0.1/docs/jipdate.rst`

 * *Files 9% similar despite different names*

```diff
@@ -19,62 +19,62 @@
 ------------------------------
 .. todo::
 
     Video: 
 
 .. code-block:: bash
 
-    $ ./jipdate.py -q -e
+    $ jipdate -q -e
 
 
 I want to update my Initiatives and Epics
 -----------------------------------------
 .. todo::
 
     Video: 
 
 .. code-block:: bash
 
-    $ ./jipdate.py -q
+    $ jipdate -q
 
 
 I want to update all my tickets (Initiatives, Epics, Stories, Sub tasks)
 ------------------------------------------------------------------------
 .. todo::
 
     Video: 
 
 .. code-block:: bash
 
-    $ ./jipdate.py -q --all
+    $ jipdate -q --all
 
 
 I want to update only my Epics and reuse my previous comment(s)
 ---------------------------------------------------------------
 .. todo::
 
     Video: 
 
 .. code-block:: bash
 
-    $ ./jipdate.py -q -e -l
+    $ jipdate -q -e -l
 
 Here it's the ``-l`` that makes the difference and Jipdate will pull the last
 comment from the ticket(s) and include that in each section for each and every
 Jira ticket assigned to you.
 
 I want to update my Initiatives and Epics and reuse my previous comment(s)
 --------------------------------------------------------------------------
 .. todo::
 
     Video: 
 
 .. code-block:: bash
 
-    $ ./jipdate.py -q -l
+    $ jipdate -q -l
 
 Here it's the ``-l`` that makes the difference and Jipdate will pull the last
 comment from the ticket(s) and include that in each section for each and every
 Jira ticket assigned to you.
 
 I want to change state of my card
 ---------------------------------
@@ -83,15 +83,15 @@
     Video:
 
 Run Jipdate with any parameter that suits your needs. Here we're getting
 everything.
 
 .. code-block:: bash
 
-    $ ./jipdate.py -q --all
+    $ jipdate -q --all
 
 In your Editor you will see a section for each Jira ticket (based on your given
 parameters to Jipdate). It could look like this:
 
 .. code-block:: bash
 
     ...
@@ -103,42 +103,58 @@
     ...
 
 Here you can see it in the ``Open`` state (``# Status Open``). If you want to
 change this to another state, then simply uncomment the line and write another
 state for it, i.e., change like we've done at line 4 here.
 
 .. code-block:: bash
-    :linenos:
-    :emphasize-lines: 4
 
     [SWG-368]
     # Header: Demo / Test issue three
     # Type: Epic
     Status: To do
     # No updates since last week.
 
 .. note::
 
     Upper/lower case doesn't matter for the status change, nor does spaces
     before or after matter. But it needs to be written as in Jira otherwise. If
     you get it wrong, Jipdate will return an error and also show the possible
     combinations. Example. ``todo`` is wrong, but ``to do`` is correct!
 
+.. code-block:: bash
+
+    ...
+    [SWG-368]
+    # Header: Demo / Test issue three
+    # Type: Epic
+    Status: In progress
+    Time spent: 4h
+    Updates since last week.
+    ...
+
+Here you can see ``Status`` in ``In progress``, and ``Time spent`` on this issue is ste to 4 hours. There are also some updates, and these updates ``Updates since last week.`` will be updated under ``Comments`` and under ``Work log`` in that ticket.
+
+.. note::
+
+    ``Time spent`` can be written in the formats: ``5m``, ``5h``, ``5d`` and ``5w``,
+    and that means ``m (minutes), h (hours), d (days), w (weeks)``.
+
 Updates with status reports
 ===========================
 
 I want to update my Epics and create a status report
 ----------------------------------------------------
 .. todo::
 
     Video: 
 
 .. code-block:: bash
 
-    $ ./jipdate.py -q -e -f status_report_week_xy.txt
+    $ jipdate -q -e -f status_report_week_xy.txt
 
 When the script has finished running you will have a file
 ``status_report_week_xy.txt`` in the folder with your entire status update ready
 to be sent out via email, for archiving or copy/pasted into a combined status
 document.
 
 .. note::
@@ -151,15 +167,15 @@
 ------------------------------------------------------
 .. todo::
 
     Video: 
 
 .. code-block:: bash
 
-    $ ./jipdate.py -f my_status.txt
+    $ jipdate -f my_status.txt
 
 The use case here is that you have a Jipdate status file stored locally that you
 update on regular basis and you basically never query Jira itself.
 
 
 Special use cases
 =================
@@ -168,15 +184,15 @@
 ---------------------------------------------------------------------
 .. todo::
 
     Video: 
 
 .. code-block:: bash
 
-    $ ./jipdate.py -q -u john.doe
+    $ jipdate -q -u john.doe
 
 .. note::
 
     For this you still need to enter your own password even though you make a
     query about another user.
 
 
@@ -184,15 +200,15 @@
 ------------------------------------------------------------------------
 .. todo::
 
     Video: 
 
 .. code-block:: bash
 
-    $ ./jipdate.py -q -u john.doe -l
+    $ jipdate -q -u john.doe -l
 
 .. note::
 
     For this you still need to enter your own password even though you make a
     query about another user.
 
 
@@ -200,43 +216,43 @@
 ----------------------------------------
 .. todo::
 
     Video: 
 
 .. code-block:: bash
 
-    $ ./jipdate.py -q -p
+    $ jipdate -q -p
 
 This can be combined with other flags (e.g. ``--all``, ``-e`` etc).
 
 Testing / development
 =====================
 
 
 I want to use a test-server / sandbox
 -------------------------------------
 .. code-block:: bash
 
-    $ ./jipdate.py -t -q
+    $ jipdate -t -q
 
 Here we provide ``-t`` which will use Linaro's `test server`_ instead of the
 real Jira instance. This is totally safe to use when playing around and testing
 Jipdate. You can of course combine this with all other parameters.
 
 
 I want to do a dry-run
 ----------------------
 .. code-block:: bash
 
-    $ ./jipdate.py -q --dry-run
+    $ jipdate -q --dry-run
 
 With ``--dry-run`` you can query the real Jira instance without risking to make
 any updates. I.e., this can be used as a complement to query the `test server`_.
 
 I want to see more debugging text from Jipdate
 ----------------------------------------------
 .. code-block:: bash
 
-    $ ./jipdate.py -q -v
+    $ jipdate -q -v
 
 
 .. _test server: https://dev-projects.linaro.org
```

### Comparing `jipdate-0.0.1/docs/jipstatus.rst` & `jipdate-2.0.1/docs/jipstatus.rst`

 * *Files 21% similar despite different names*

```diff
@@ -19,72 +19,72 @@
 
 The default behavior for `jipstatus` when no specific arguments are used is to
 query the Jira server for all the updates for the current user in the last
 week.
 
 .. code-block:: bash
 
-    $ ./jipstatus.py
+    $ jipstatus
 
 The `--days` argument can be used to query for any arbitrary duration (in days):
 
 .. code-block:: bash
 
-    $ ./jipstatus.py --days 30
+    $ jipstatus --days 30
 
 I want to generate an HTML output
 ---------------------------------
 
 The argument `--html` can be used to generate a report in HTML format. By
 default `jipstatus` will create the file `status.html`, which can be changed by
 the user:
 
 .. code-block:: bash
 
-    $ ./jipstatus.py --html [file.html]
+    $ jipstatus --html [file.html]
 
 Retrieve updates for a specific Jira project
 ============================================
 
 Instead of querying Jira for a specific user, `--project` can be used to request
 updates to all tickets from a specific project.
 
 .. code-block:: bash
 
-    $ ./jipstatus.py --project <PJT_KEY>
+    $ jipstatus --project <PJT_KEY>
 
 Several arguments can be combined together:
 
 .. code-block:: bash
 
-    $ ./jipstatus.py --project <PJT_KEY> --days 30 --html
+    $ jipstatus --project <PJT_KEY> --days 30 --html
 
 Retrieve updates for a specific Jira team
 =========================================
 
 The `--team` argument can be used to retrieve updates from all users who belong
 to a specific Jira team (or group):
 
 .. code-block:: bash
 
-    $ ./jipstatus.py --team linaro --days 30 --html
+    $ jipstatus --team linaro --days 30 --html
 
 
 Retrieve updates for a specific Jira user
 =========================================
 
 The `--user` argument can be used to retrieve update from a specific user, it
 can be the user email address, or the short form firstname.lastname.
 
 .. code-block:: bash
 
-    $ ./jipstatus.py --user jane.doe --days 30 --html
+    $ jipstatus --user jane.doe --days 30 --html
 
 
 I want to see more debugging text from Jipstatus
 ================================================
 
 You can use `-v` to request verbose output.
 
 .. code-block:: bash
 
-    $ ./jipstatus.py -v
+    $ jipstatus -v
```

### Comparing `jipdate-0.0.1/docs/problems.rst` & `jipdate-2.0.1/docs/problems.rst`

 * *Files identical despite different names*

### Comparing `jipdate-0.0.1/docs/run.rst` & `jipdate-2.0.1/docs/run.rst`

 * *Files 1% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 #########################
 Run Jipdate
 #########################
 The most straight forward way is to simply run the script
 
 .. code-block:: bash
 
-    $ ./jipdate
+    $ jipdate
 
 Running it without any parameters (or with ``-h``) will give you a list of all
 parameters. If you want to see examples of how to combine flags/parameters, then
 head over to :ref:`jipdate_examples`.
 
 #########################
 Run Jipstatus
 #########################
 The most straight forward way is to simply run the script
 
 .. code-block:: bash
 
-    $ ./jipstatus
+    $ jipstatus
 
 Running it without any parameters will show all tickets updates for the current
 user in the last 7 days, including newly created tickets, state transitions, and
 all updates.
 
 Running with ``-h`` will give you a list of all parameters. If you want to see
 examples of how to combine flags/parameters, then head over to
```

### Comparing `jipdate-0.0.1/jipdate/cfg.py` & `jipdate-2.0.1/jipdate/cfg.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,14 +38,18 @@
 version: 1
 
 # Jira server information
 #server:
 #  url: https://linaro.atlassian.net
 #  token: abcdefghijkl
 
+#test_server:
+#  url: https://<name_of_test_instance>.atlassian.net
+#  token: abcdefghijkl
+
 # Extra comments added to each Jira issue (multiline is OK)
 comments:
         - "# No updates since last week."
 
 # Header of the file (multiline is OK). It will be followed by JIRA_USERNAME
 header:
         - |
@@ -88,17 +92,18 @@
     # If nothing was found, then return the default file
     return config_path + "/" + config_filename
 
 
 def get_server(use_test_server=False):
     # Get Jira Server details. Check first if using the test server
     # then try user config file, then default from cfg.py
-    server = TEST_SERVER
     if use_test_server is False:
         server = yml_config.get('server', PRODUCTION_SERVER)
+    else:
+        server = yml_config.get('test_server', TEST_SERVER)
 
     return server
 
 
 def initiate_config():
     """ Reads the config file (yaml format) and returns the sets the global
     instance.
```

### Comparing `jipdate-0.0.1/jipdate/jipdate.py` & `jipdate-2.0.1/jipdate/jipdate.py`

 * *Files 5% similar despite different names*

```diff
@@ -134,15 +134,15 @@
             help='Do not make any changes to JIRA')
 
     return parser
 
 ################################################################################
 # Jira functions
 ################################################################################
-def update_jira(jira, i, c, t):
+def update_jira(jira, i, c, t, ts=None):
     """
     This is the function that do the actual updates to Jira and in this case it
     is adding comments to a certain issue.
     """
     if t['transition']:
         if t['resolution']:
             log.debug("Updating Jira issue: %s with transition: %s (%s)" %
@@ -154,14 +154,16 @@
 
     if c != "":
         log.debug("Updating Jira issue: %s with comment:" % i)
         log.debug("-- 8< --------------------------------------------------------------------------")
         log.debug("%s" % c)
         log.debug("-- >8 --------------------------------------------------------------------------\n\n")
         jira.add_comment(i, c)
+        if ts:
+            jira.add_worklog(i, timeSpent=ts, comment=c)
 
 
 def write_last_jira_comment(f, jira, issue):
     """ Pulls the last comment from Jira from an issue and writes it to the file
     object.
     """
     c = jira.comments(issue)
@@ -282,14 +284,18 @@
     # Regexp to match for a status update, this will remove 'Status' from the
     # match:
     regex_status = r'(?:^Status:) *(.+)\n$'
 
     # Contains the status text, it could be a file or a status email
     status = ""
 
+    # Regexp to match for a time spent update, this will remove 'Time spent:'
+    # from the match:
+    regex_timespent = r'(^Time spent:) \d+\w\n$'
+
     # List of resolutions (when doing a transition to Resolved). Query once globally.
     resolution_map = dict([(t.name.title(), t.id) for t in jira.resolutions()])
 
     with open(filename) as f:
         status = f.readlines()
 
     myissue = "";
@@ -310,65 +316,69 @@
             myissue = match.group(1)
             validissue = True
 
             # if we ran a query, we might already have fetched the issue
             # let's try to find the issue there first, otherwise ask Jira
             try:
                 issue = [x for x in issues if str(x) == myissue][0]
-                issue_comments.append((issue, "", ""))
+                issue_comments.append((issue, "", "", None))
 
             # IndexError: we had fetched already, but issue is not found
             # TypeError: issues is None, we haven't queried Jira yet, at all
             except (IndexError, TypeError) as e:
                 try:
                     issue = jira.issue(myissue)
-                    issue_comments.append((issue, "", ""))
+                    issue_comments.append((issue, "", "", None))
                 except  Exception as e:
                     if 'Issue Does Not Exist' in e.text:
                         print('[{}] :  {}'.format(myissue, e.text))
                         validissue = False
 
         # Stop parsing entirely.  This needs to be placed before regex_stop
         # or the .* will match and [FIN] won't be processed
         elif re.search(regex_fin, line):
             break
         # If we have non-JIRA issue tags, stop parsing until we find a valid tag
         elif re.search(regex_stop, line):
-                validissue = False
+            validissue = False
         elif transition and validissue:
             # If we have a match, then the new status should be first in the
             # group. Jira always expect the name of the state transitions to be
             # word capitalized, hence the call to the title() function. This
             # means that it doesn't matter if the user enter all lower case,
             # mixed or all upper case. All of them will work.
             new_status = transition.groups()[0].title()
-            (i,c,_) = issue_comments[-1]
-            issue_comments[-1] = (i, c, new_status)
+            (i,c,_,ts) = issue_comments[-1]
+            issue_comments[-1] = (i, c, new_status, ts)
+        elif re.search(regex_timespent, line, re.IGNORECASE):
+            timespent = line.split(':')[1].strip()
+            (i,c,t,_) = issue_comments[-1]
+            issue_comments[-1] = (i, c, t, timespent)
         else:
             # Don't add lines with comments
             if (line[0] != "#" and issue_comments and validissue):
-                (i,c,t) = issue_comments[-1]
-                issue_comments[-1] = (i, c + line, t)
+                (i,c,t,ts) = issue_comments[-1]
+                issue_comments[-1] = (i, c + line, t, ts)
 
     issue_upload = []
     print("These JIRA cards will be updated as follows:\n")
     for (idx,t) in enumerate(issue_comments):
-        (issue,comment,transition) = issue_comments[idx]
+        (issue,comment,transition,timespent) = issue_comments[idx]
 
         # Strip beginning  and trailing blank lines
         comment = comment.strip('\n')
 
         # initialize here to avoid unassigned variables and useless code complexity
         resolution_id = transition_id = None
         resolution = transition_summary = ""
 
         if transition != "" and transition != str(issue.fields.status):
             # An optional 'resolution' attribute can be set when doing a transition
             # to Resolved, using the following pattern: Resolved / <resolution>
-            if transition.startswith('Resolved') and '/' in transition:
+            if (transition.startswith('Resolved') or transition.startswith('Closed')) and '/' in transition:
                 (transition, resolution) = map(str.strip, transition.split('/'))
                 if not resolution in resolution_map:
                     print("Invalid resolution \"{}\" for issue {}".format(resolution, issue))
                     print("Possible resolution: {}".format([t for t in resolution_map]))
                     sys.exit(1)
                 resolution_id = resolution_map[resolution]
 
@@ -385,31 +395,32 @@
                 transition_summary = " %s => %s" % (issue.fields.status, transition)
 
         if comment == "" and not transition_id:
             log.debug("Issue [%s] has no comment or transitions, not updating the issue" % (issue))
             continue
 
         issue_upload.append((issue, comment,
-                             {'transition': transition_id, 'resolution': resolution_id}))
+                             {'transition': transition_id, 'resolution': resolution_id}, timespent))
         print("[%s]%s\n  %s" % (issue, transition_summary, "\n  ".join(comment.splitlines())))
+        if timespent: print(" Time spent: %s" % timespent)
     print("")
 
     issue_comments = issue_upload
     if issue_comments == [] or cfg.args.dry_run or should_update() == "n":
         if issue_comments == []:
             print("No change, Jira was not updated!\n")
         else:
             print("Comments will not be written to Jira!\n")
         if not cfg.args.s:
             print_status(status)
         sys.exit()
 
     # if we found something, let's update jira
-    for (issue,comment,transition) in issue_comments:
-        update_jira(jira, issue, comment, transition)
+    for (issue,comment,transition,timespent) in issue_comments:
+        update_jira(jira, issue, comment, transition, timespent)
 
     print("Successfully updated your Jira tickets!\n")
     if not cfg.args.s:
         print_status(status)
 
 def print_status_file(filename):
     with open(filename, 'r') as f:
```

### Comparing `jipdate-0.0.1/jipdate/jipfp.py` & `jipdate-2.0.1/jipdate/jipfp.py`

 * *Files identical despite different names*

### Comparing `jipdate-0.0.1/jipdate/jipstatus.py` & `jipdate-2.0.1/jipdate/jipstatus.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,26 +26,29 @@
     it is already included.
     """
     if '@' not in user:
         user = user + "@linaro.org"
     return user
 
 def default_jql():
-    user = cfg.args.user
     project = cfg.args.project
     team = cfg.args.team
 
     if team and project:
         jql = "(project = %s or assignee in membersOf('%s')) " % (project, team)
     elif team:
         jql = "assignee in membersOf('%s') " % team
     elif project:
         jql = "project =  '%s' " % project
     else:
-        jql = "assignee = '%s' " % add_domain(user)
+        # cfg.args.user is a list with 1 or more users
+        # we construct the query as:
+        # (assignee = 'user1' or assignee = 'user2' )
+        users = list(map(add_domain, cfg.args.user))
+        jql = '(' + ' or '.join(map(lambda str: 'assignee = \'' + str + '\'' , users)) + ')'
 
     return jql
 
 def enumerate_updates(jira):
     since = datetime.datetime.now() - datetime.timedelta(days=int(cfg.args.days))
 
     jql = default_jql()
@@ -130,15 +133,15 @@
     """ Takes care of script argument parsing. """
     parser = ArgumentParser(description='Script used to update comments in Jira')
 
     parser.add_argument('--test', required=False, action="store_true", \
             default=False, \
             help='Use the test server')
 
-    parser.add_argument('-u', '--user', required=False, action="store", \
+    parser.add_argument('-u', '--user', required=False, action="append", \
             default=None, \
             help='Query Jira with another Jira username \
             (first.last or first.last@linaro.org)')
 
     parser.add_argument('-p', '--project', required=False, action="store", \
             default=None, \
             type = str.upper, \
@@ -258,15 +261,15 @@
     # This initiates the global yml configuration instance so it will be
     # accessible everywhere after this call.
     cfg.initiate_config()
 
     jira, username = jiralogin.get_jira_instance(cfg.args.test)
 
     if cfg.args.user is None:
-        cfg.args.user = username
+        cfg.args.user = [username]
 
     updates = list(enumerate_updates(jira))
     pendings = list(enumerate_pending(jira))
 
     assignees = sorted(set([u['assignee'] for u in updates]) | set([p['assignee'] for p in pendings]))
     # Move "Unassigned" issues to the end
     assignees.sort(key='Unassigned'.__eq__)
```

### Comparing `jipdate-0.0.1/jipdate/jiralogin.py` & `jipdate-2.0.1/jipdate/jiralogin.py`

 * *Files identical despite different names*

### Comparing `jipdate-0.0.1/pyproject.toml` & `jipdate-2.0.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -8,17 +8,20 @@
 readme = "README.md"
 classifiers = ["License :: OSI Approved :: MIT License"]
 requires-python = ">=3.6"
 dependencies = [
     "jinja2",
     "jira",
     "PyYAML",
+    "python-dateutil",
 ]
 dynamic = ["version", "description"]
 
 [project.urls]
 Documentation = "https://jipdate.readthedocs.io/en/latest/"
 
 [project.scripts]
+jipcreate="jipdate.jipcreate:main"
 jipdate="jipdate.jipdate:main"
 jipfp="jipdate.jipfp:main"
+jipsearch="jipdate.jipsearch:main"
 jipstatus="jipdate.jipstatus:main"
```

### Comparing `jipdate-0.0.1/PKG-INFO` & `jipdate-2.0.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: jipdate
-Version: 0.0.1
+Version: 2.0.1
 Summary: Command line tool for Jira
 Author-email: Joakim Bech <joakim.bech@linaro.org>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: jinja2
 Requires-Dist: jira
 Requires-Dist: PyYAML
+Requires-Dist: python-dateutil
 Project-URL: Documentation, https://jipdate.readthedocs.io/en/latest/
 
 # Jipdate - Jira comment and status update tool
 
 Jipdate is a tool used at Linaro that makes it possible in one go to:
 
 * Update all tickets belonging to a certain user using command line and your
```

