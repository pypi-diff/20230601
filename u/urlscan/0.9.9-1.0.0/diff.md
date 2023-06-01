# Comparing `tmp/urlscan-0.9.9.tar.gz` & `tmp/urlscan-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "urlscan-0.9.9.tar", last modified: Sat Jan 29 05:18:03 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `urlscan-0.9.9.tar` & `urlscan-1.0.0.tar`

### file list

```diff
@@ -1,22 +1,11 @@
-drwxr-xr-x   0 firecat53  (1000) firecat53  (1000)        0 2022-01-29 05:18:03.146722 urlscan-0.9.9/
--rw-r--r--   0 firecat53  (1000) firecat53  (1000)    17987 2021-03-19 00:20:16.000000 urlscan-0.9.9/COPYING
--rw-r--r--   0 firecat53  (1000) firecat53  (1000)       82 2021-03-19 00:20:16.000000 urlscan-0.9.9/MANIFEST.in
--rw-r--r--   0 firecat53  (1000) firecat53  (1000)     8669 2022-01-29 05:18:03.146722 urlscan-0.9.9/PKG-INFO
--rw-r--r--   0 firecat53  (1000) firecat53  (1000)     7724 2021-12-20 20:20:45.000000 urlscan-0.9.9/README.md
--rw-r--r--   0 firecat53  (1000) firecat53  (1000)       38 2022-01-29 05:18:03.146722 urlscan-0.9.9/setup.cfg
--rwxr-xr-x   0 firecat53  (1000) firecat53  (1000)     1615 2022-01-29 04:44:34.000000 urlscan-0.9.9/setup.py
-drwxr-xr-x   0 firecat53  (1000) firecat53  (1000)        0 2022-01-29 05:18:03.145722 urlscan-0.9.9/urlscan/
--rw-r--r--   0 firecat53  (1000) firecat53  (1000)       46 2021-03-19 00:20:16.000000 urlscan-0.9.9/urlscan/__init__.py
--rw-r--r--   0 firecat53  (1000) firecat53  (1000)     8010 2021-10-06 18:11:18.000000 urlscan-0.9.9/urlscan/__main__.py
-drwxr-xr-x   0 firecat53  (1000) firecat53  (1000)        0 2022-01-29 05:18:03.145722 urlscan-0.9.9/urlscan/assets/
--rw-r--r--   0 firecat53  (1000) firecat53  (1000)    10051 2021-10-13 21:33:43.000000 urlscan-0.9.9/urlscan/assets/tlds-alpha-by-domain.txt
--rw-r--r--   0 firecat53  (1000) firecat53  (1000)    36117 2021-12-20 20:20:45.000000 urlscan-0.9.9/urlscan/urlchoose.py
--rw-r--r--   0 firecat53  (1000) firecat53  (1000)    17509 2021-12-29 02:43:47.000000 urlscan-0.9.9/urlscan/urlscan.py
--rw-r--r--   0 firecat53  (1000) firecat53  (1000)     7326 2021-10-13 21:33:43.000000 urlscan-0.9.9/urlscan.1
-drwxr-xr-x   0 firecat53  (1000) firecat53  (1000)        0 2022-01-29 05:18:03.145722 urlscan-0.9.9/urlscan.egg-info/
--rw-r--r--   0 firecat53  (1000) firecat53  (1000)     8669 2022-01-29 05:18:03.000000 urlscan-0.9.9/urlscan.egg-info/PKG-INFO
--rw-r--r--   0 firecat53  (1000) firecat53  (1000)      356 2022-01-29 05:18:03.000000 urlscan-0.9.9/urlscan.egg-info/SOURCES.txt
--rw-r--r--   0 firecat53  (1000) firecat53  (1000)        1 2022-01-29 05:18:03.000000 urlscan-0.9.9/urlscan.egg-info/dependency_links.txt
--rw-r--r--   0 firecat53  (1000) firecat53  (1000)       51 2022-01-29 05:18:03.000000 urlscan-0.9.9/urlscan.egg-info/entry_points.txt
--rw-r--r--   0 firecat53  (1000) firecat53  (1000)       13 2022-01-29 05:18:03.000000 urlscan-0.9.9/urlscan.egg-info/requires.txt
--rw-r--r--   0 firecat53  (1000) firecat53  (1000)        8 2022-01-29 05:18:03.000000 urlscan-0.9.9/urlscan.egg-info/top_level.txt
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 urlscan-1.0.0/urlscan/__init__.py
+-rw-r--r--   0        0        0     8296 2020-02-02 00:00:00.000000 urlscan-1.0.0/urlscan/__main__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 urlscan-1.0.0/urlscan/_version.py
+-rw-r--r--   0        0        0    37006 2020-02-02 00:00:00.000000 urlscan-1.0.0/urlscan/urlchoose.py
+-rw-r--r--   0        0        0    17573 2020-02-02 00:00:00.000000 urlscan-1.0.0/urlscan/urlscan.py
+-rw-r--r--   0        0        0     9912 2020-02-02 00:00:00.000000 urlscan-1.0.0/urlscan/assets/tlds-alpha-by-domain.txt
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 urlscan-1.0.0/.gitignore
+-rw-r--r--   0        0        0    17987 2020-02-02 00:00:00.000000 urlscan-1.0.0/LICENSE
+-rw-r--r--   0        0        0     7902 2020-02-02 00:00:00.000000 urlscan-1.0.0/README.md
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 urlscan-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     8866 2020-02-02 00:00:00.000000 urlscan-1.0.0/PKG-INFO
```

### Comparing `urlscan-0.9.9/COPYING` & `urlscan-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `urlscan-0.9.9/PKG-INFO` & `urlscan-1.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 Metadata-Version: 2.1
 Name: urlscan
-Version: 0.9.9
+Version: 1.0.0
 Summary: View/select the URLs in an email message or file
-Home-page: https://github.com/firecat53/urlscan
-Author: Scott Hansen
-Author-email: firecat4153@gmail.com
-License: GPLv2
-Download-URL: https://github.com/firecat53/urlscan/archive/0.9.9.zip
-Keywords: urlscan,urlview,email,mutt,tmux
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
+Project-URL: Homepage, https://github.com/firecat53/urlscan
+Author-email: Scott Hansen <tech@firecat53.net>
+License-Expression: GPL-2.0
+License-File: LICENSE
+Keywords: email,mutt,tmux,urlscan,urlview
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Console :: Curses
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
+Requires-Dist: urwid>=1.2.1
 Description-Content-Type: text/markdown
-License-File: COPYING
 
 # Urlscan
 
 ## Contributors
 
-Scott Hansen \<firecat4153@gmail.com\> (Author and Maintainer)
+Scott Hansen \<tech@firecat53.net\> (Author and Maintainer)
 
 Maxime Chatelle \<xakz@rxsoft.eu\> (Debian Maintainer)
 
 Daniel Burrows \<dburrows@debian.org\> (Original Author)
 
 ## Purpose and Requirements
 
@@ -90,17 +89,21 @@
 - Scan certain email headers for URLs. Currently `Link`, `Archived-At` and
   `List-*` are scanned when `--headers` is passed.
 
 - Queue multiple URLs for opening and open them all at once with `a` and `o`.
 
 ## Installation and setup
 
-To install urlscan, install from your distribution repositories (Archlinux),
-from Pypi, or do a local development install with pip -e:
+To install urlscan, install from your distribution repositories, from Pypi, or do
+a local development install with pip -e:
 
+    pipx install urlscan 
+    
+    OR
+    
     pip install --user urlscan
 
     OR
 
     cd <path/to/urlscan> && pip install --user -e .
 
 **NOTE**
@@ -214,10 +217,13 @@
 
 - The HTML message handling is a bit kludgy in general.
 
 - multipart/alternative sections are handled by descending into all the
   sub-parts, rather than just picking one, which may lead to URLs and context
   appearing twice. (Bypass this by selecting the '--dedupe' option)
 
-[1]: http://urwid.org/manual/displayattributes.html#display-attributes  "Urwid display attributes"
+## Build/development
 
+- pyproject.toml is configured for [hatch][2] for building and submitting to pypi.
 
+[1]: http://urwid.org/manual/displayattributes.html#display-attributes  "Urwid display attributes"
+[2]: https://hatch.pypa.io/latest/  "Hatch"
```

### Comparing `urlscan-0.9.9/README.md` & `urlscan-1.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Urlscan
 
 ## Contributors
 
-Scott Hansen \<firecat4153@gmail.com\> (Author and Maintainer)
+Scott Hansen \<tech@firecat53.net\> (Author and Maintainer)
 
 Maxime Chatelle \<xakz@rxsoft.eu\> (Debian Maintainer)
 
 Daniel Burrows \<dburrows@debian.org\> (Original Author)
 
 ## Purpose and Requirements
 
@@ -65,17 +65,21 @@
 - Scan certain email headers for URLs. Currently `Link`, `Archived-At` and
   `List-*` are scanned when `--headers` is passed.
 
 - Queue multiple URLs for opening and open them all at once with `a` and `o`.
 
 ## Installation and setup
 
-To install urlscan, install from your distribution repositories (Archlinux),
-from Pypi, or do a local development install with pip -e:
+To install urlscan, install from your distribution repositories, from Pypi, or do
+a local development install with pip -e:
 
+    pipx install urlscan 
+    
+    OR
+    
     pip install --user urlscan
 
     OR
 
     cd <path/to/urlscan> && pip install --user -e .
 
 **NOTE**
@@ -189,8 +193,13 @@
 
 - The HTML message handling is a bit kludgy in general.
 
 - multipart/alternative sections are handled by descending into all the
   sub-parts, rather than just picking one, which may lead to URLs and context
   appearing twice. (Bypass this by selecting the '--dedupe' option)
 
+## Build/development
+
+- pyproject.toml is configured for [hatch][2] for building and submitting to pypi.
+
 [1]: http://urwid.org/manual/displayattributes.html#display-attributes  "Urwid display attributes"
+[2]: https://hatch.pypa.io/latest/  "Hatch"
```

### Comparing `urlscan-0.9.9/urlscan/__main__.py` & `urlscan-1.0.0/urlscan/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 """ A simple urlview replacement that handles things like quoted-printable
 properly.
 
 """
 #
 #   Copyright (C) 2006-2007 Daniel Burrows
-#   Copyright (C) 2021 Scott Hansen
+#   Copyright (C) 2023 Scott Hansen
 #
 # This program is free software; you can redistribute it and/or
 # modify it under the terms of the GNU General Public License
 # as published by the Free Software Foundation; either version 2
 # of the License, or (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -24,14 +24,15 @@
 import argparse
 import io
 import os
 import sys
 from email import policy
 from email.parser import BytesParser
 from urlscan import urlchoose, urlscan
+from urlscan._version import version
 
 
 def parse_arguments():
     """Parse command line options.
 
     Returns: args
 
@@ -82,14 +83,17 @@
                            help='Set width to display')
     arg_parse.add_argument('--whitespace-off', '-W', dest='whitespaceoff',
                            action='store_true', default=False,
                            help="Don't display empty lines and ellipses.")
     arg_parse.add_argument('--headers', dest='headers',
                            action='store_true', default=False,
                            help='Scan certain message headers for URLs.')
+    arg_parse.add_argument('--version', '-V', dest='version',
+                           action='store_true', default=False,
+                           help='Print urlscan version')
     arg_parse.add_argument('message', nargs='?', default=sys.stdin,
                            help="Filename of the message to parse")
     return arg_parse.parse_args()
 
 
 def close_stdin():
     """This section closes out sys.stdin if necessary so as not to block curses
@@ -162,14 +166,17 @@
 
 
 def main():
     """Entrypoint function for urlscan
 
     """
     args = parse_arguments()
+    if args.version is True:
+        print(version)
+        return
     if args.genconf is True:
         urlchoose.URLChooser([], genconf=True)
         return
     msg = process_input(args.message)
     if args.nobrowser is False:
         tui = urlchoose.URLChooser(urlscan.msgurls(msg, regex=args.regex, headers=args.headers),
                                    compact=args.compact,
```

### Comparing `urlscan-0.9.9/urlscan/assets/tlds-alpha-by-domain.txt` & `urlscan-1.0.0/urlscan/assets/tlds-alpha-by-domain.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Version 2021100600, Last Updated Wed Oct  6 07:07:01 2021 UTC
+# Version 2023060100, Last Updated Thu Jun  1 07:07:01 2023 UTC
 AAA
 AARP
 ABARTH
 ABB
 ABBOTT
 ABBVIE
 ABC
@@ -13,23 +13,21 @@
 ACADEMY
 ACCENTURE
 ACCOUNTANT
 ACCOUNTANTS
 ACO
 ACTOR
 AD
-ADAC
 ADS
 ADULT
 AE
 AEG
 AERO
 AETNA
 AF
-AFAMILYCOMPANY
 AFL
 AFRICA
 AG
 AGAKHAN
 AGENCY
 AI
 AIG
@@ -173,16 +171,14 @@
 BRIDGESTONE
 BROADWAY
 BROKER
 BROTHER
 BRUSSELS
 BS
 BT
-BUDAPEST
-BUGATTI
 BUILD
 BUILDERS
 BUSINESS
 BUY
 BUZZ
 BV
 BW
@@ -194,15 +190,14 @@
 CAFE
 CAL
 CALL
 CALVINKLEIN
 CAM
 CAMERA
 CAMP
-CANCERRESEARCH
 CANON
 CAPETOWN
 CAPITAL
 CAPITALONE
 CAR
 CARAVAN
 CARDS
@@ -297,15 +292,14 @@
 CREDITCARD
 CREDITUNION
 CRICKET
 CROWN
 CRS
 CRUISE
 CRUISES
-CSC
 CU
 CUISINELLA
 CV
 CW
 CX
 CY
 CYMRU
@@ -356,15 +350,14 @@
 DOG
 DOMAINS
 DOT
 DOWNLOAD
 DRIVE
 DTV
 DUBAI
-DUCK
 DUNLOP
 DUPONT
 DURBAN
 DVAG
 DVR
 DZ
 EARTH
@@ -490,15 +483,14 @@
 GH
 GI
 GIFT
 GIFTS
 GIVES
 GIVING
 GL
-GLADE
 GLASS
 GLE
 GLOBAL
 GLOBO
 GM
 GMAIL
 GMBH
@@ -654,14 +646,15 @@
 KERRYLOGISTICS
 KERRYPROPERTIES
 KFH
 KG
 KH
 KI
 KIA
+KIDS
 KIM
 KINDER
 KINDLE
 KITCHEN
 KIWI
 KM
 KN
@@ -711,28 +704,25 @@
 LIFESTYLE
 LIGHTING
 LIKE
 LILLY
 LIMITED
 LIMO
 LINCOLN
-LINDE
 LINK
 LIPSY
 LIVE
 LIVING
-LIXIL
 LK
 LLC
 LLP
 LOAN
 LOANS
 LOCKER
 LOCUS
-LOFT
 LOL
 LONDON
 LOTTE
 LOTTO
 LOVE
 LPL
 LPLFINANCIAL
@@ -744,15 +734,14 @@
 LU
 LUNDBECK
 LUXE
 LUXURY
 LV
 LY
 MA
-MACYS
 MADRID
 MAIF
 MAISON
 MAKEUP
 MAN
 MANAGEMENT
 MANGO
@@ -817,14 +806,15 @@
 MS
 MSD
 MT
 MTN
 MTR
 MU
 MUSEUM
+MUSIC
 MUTUAL
 MV
 MW
 MX
 MY
 MZ
 NA
@@ -873,15 +863,14 @@
 NRW
 NTT
 NU
 NYC
 NZ
 OBI
 OBSERVER
-OFF
 OFFICE
 OKINAWA
 OLAYAN
 OLAYANGROUP
 OLDNAVY
 OLLO
 OM
@@ -972,18 +961,16 @@
 PW
 PWC
 PY
 QA
 QPON
 QUEBEC
 QUEST
-QVC
 RACING
 RADIO
-RAID
 RE
 READ
 REALESTATE
 REALTOR
 REALTY
 RECIPES
 RED
@@ -1052,27 +1039,25 @@
 SCHAEFFLER
 SCHMIDT
 SCHOLARSHIPS
 SCHOOL
 SCHULE
 SCHWARZ
 SCIENCE
-SCJOHNSON
 SCOT
 SD
 SE
 SEARCH
 SEAT
 SECURE
 SECURITY
 SEEK
 SELECT
 SENER
 SERVICES
-SES
 SEVEN
 SEW
 SEX
 SEXY
 SFR
 SG
 SH
@@ -1323,15 +1308,14 @@
 XN--1QQW23A
 XN--2SCRJ9C
 XN--30RR7Y
 XN--3BST00M
 XN--3DS443G
 XN--3E0B707E
 XN--3HCRJ9C
-XN--3OQ18VL8PN36A
 XN--3PXU8K
 XN--42C2D9A
 XN--45BR5CYL
 XN--45BRJ9C
 XN--45Q11C
 XN--4DBRK0CE
 XN--4GBRIM
@@ -1392,15 +1376,14 @@
 XN--I1B6B1A6A2E
 XN--IMR513N
 XN--IO0A7I
 XN--J1AEF
 XN--J1AMH
 XN--J6W193G
 XN--JLQ480N2RG
-XN--JLQ61U9W7B
 XN--JVR189M
 XN--KCRX77D1X4A
 XN--KPRW13D
 XN--KPRY57D
 XN--KPUT3I
 XN--L1ACC
 XN--LGBBAT1AD8J
```

### Comparing `urlscan-0.9.9/urlscan/urlchoose.py` & `urlscan-1.0.0/urlscan/urlchoose.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #   Copyright (C) 2006-2007 Daniel Burrows
-#   Copyright (C) 2021 Scott Hansen
+#   Copyright (C) 2023 Scott Hansen
 #
 # This program is free software; you can redistribute it and/or
 # modify it under the terms of the GNU General Public License
 # as published by the Free Software Foundation; either version 2
 # of the License, or (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -14,14 +14,15 @@
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301, USA
 
 """An urwid listview-based widget that lets you choose a URL from a list of
 URLs."""
 
+import contextlib
 import json
 import os
 from os.path import dirname, exists, expanduser
 import re
 import shlex
 import subprocess
 import sys
@@ -206,25 +207,25 @@
         self.width = min(self.term_width, width or self.term_width)
         self.whitespaceoff = whitespaceoff
         self.activate_keys = [i for i, j in urwid.Button._command_map._command.items()
                               if j == 'activate']
         self.items, self.urls = self.process_urls(extractedurls,
                                                   dedupe=dedupe,
                                                   shorten=self.shorten)
+        # Original version of all items
+        self.items_orig = self.items
+        # Store items grouped into sections
+        self.items_org = grp_list(self.items)
         # Store 'compact' mode items
         self.items_com = [i for i in self.items if
                           isinstance(i, urwid.Columns) is True]
         if self.compact is True:
             self.items, self.items_com = self.items_com, self.items
         self.urls_unesc = [i.replace('\\', '') for i in self.urls]
         self.unesc = False
-        # Original version of all items
-        self.items_orig = self.items
-        # Store items grouped into sections
-        self.items_org = grp_list(self.items)
         listbox = urwid.ListBox(self.items)
         self.header = (":: F1 - help/keybindings :: "
                        "q - quit :: "
                        "/ - search :: "
                        "URL opening mode - {} :: "
                        "Queue - {}")
         self.link_open_modes = ["Web Browser", "Xdg-Open"] if self.xdg is True else ["Web Browser"]
@@ -349,15 +350,15 @@
             else f"Executing: {self.run or self.runsafe}"
         if os.environ.get('BROWSER') not in ['elinks', 'links', 'w3m', 'lynx']:
             self._footer_display(load_text, 5)
 
     def _background_queue(self, mode):
         """Open URLs in background"""
         for url in self.queue:
-            self.mkbrowseto(url, thread=True, mode=mode)()
+            self.mkbrowseto(url, mode=mode)()
         self.draw_screen()
 
     def _queue(self, mode=2):
         """Open all URLs in queue
 
             Args: mode - 2 for new tab, 1 for new window
 
@@ -394,27 +395,33 @@
         if self.compact is False and fpo <= 1:
             return
         self.queue.append(self.urls[url_idx])
         self.queue = list(set(self.queue))
         self.headerwid = urwid.AttrMap(urwid.Text(
             self.header.format(self.link_open_modes[0], len(self.queue))), 'header')
         self.top.base_widget.header = self.headerwid
+        label = self.items[fpo][1].label
+        if not label.startswith("* "):
+            self.items[fpo][1].set_label(f"* {label}")
 
     def _del_url(self):
         """d"""
         fpo = self.top.base_widget.body.focus_position
         url_idx = len([i for i in self.items[:fpo + 1]
                        if isinstance(i, urwid.Columns)]) - 1
         if self.compact is False and fpo <= 1:
             return
         try:
             self.queue.remove(self.urls[url_idx])
             self.headerwid = urwid.AttrMap(urwid.Text(
                 self.header.format(self.link_open_modes[0], len(self.queue))), 'header')
             self.top.base_widget.header = self.headerwid
+            label = self.items[fpo][1].label
+            if label.startswith("* "):
+                self.items[fpo][1].set_label(label.lstrip("* "))
         except ValueError:
             pass
 
     def _help_menu(self):
         """F1"""
         if self.help_menu is False:
             self.focus_pos_saved = self.top.base_widget.body.focus_position
@@ -459,16 +466,15 @@
         self.help_menu = not self.help_menu
 
     def _search_key(self):
         """ / """
         if self.urls:
             self.search = True
             if self.compact is True:
-                self.compact = False
-                self.items, self.items_com = self.items_com, self.items
+                self._context()
         else:
             return
         self.no_matches = False
         self.search_string = ""
         # Reset the search highlighting
         self._search()
         footerwid = urwid.AttrMap(urwid.Text("Search: "), 'footer')
@@ -740,56 +746,49 @@
         mode = self.link_open_modes.pop()
         self.link_open_modes.insert(0, mode)
         if self.nohelp is False:
             self.headerwid = urwid.AttrMap(urwid.Text(
                 self.header.format(self.link_open_modes[0], len(self.queue))), 'header')
             self.top.base_widget.header = self.headerwid
 
-    def mkbrowseto(self, url, thread=False, mode=0):
+    def mkbrowseto(self, url, mode=0):
         """Create the urwid callback function to open the web browser or call
         another function with the URL.
 
         """
         def browse(*args):  # pylint: disable=unused-argument
-            # These 3 lines prevent any stderr messages from webbrowser or xdg
-            savout = os.dup(2)
-            os.close(2)
-            os.open(os.devnull, os.O_RDWR)
             # double ()() to ensure self.search evaluated at runtime, not when
             # browse() is _created_. [0] is self.search, [1] is self.enter
             # self.enter prevents opening URL when in search mode
-            if self._get_search()[0]() is True:
-                if self._get_search()[1]() is True:
-                    self.search = False
-                    self.enter = False
-            elif self.link_open_modes[0] == "Web Browser":
-                webbrowser.open(url, new=mode)
-            elif self.link_open_modes[0] == "Xdg-Open":
-                subprocess.run(shlex.split(f'xdg-open "{url}"'), check=False)
-            elif self.link_open_modes[0] == self.runsafe:
-                if self.pipe:
-                    subprocess.run(shlex.split(self.runsafe),
+            with redirect_output():
+                if self._get_search()[0]() is True:
+                    if self._get_search()[1]() is True:
+                        self.search = False
+                        self.enter = False
+                elif self.link_open_modes[0] == "Web Browser":
+                    webbrowser.open(url, new=mode)
+                elif self.link_open_modes[0] == "Xdg-Open":
+                    subprocess.run(shlex.split(f'xdg-open "{url}"'), check=False)
+                elif self.link_open_modes[0] == self.runsafe:
+                    if self.pipe:
+                        subprocess.run(shlex.split(self.runsafe),
+                                       check=False,
+                                       input=url.encode(sys.getdefaultencoding()))
+                    else:
+                        cmd = [i.format(url) for i in shlex.split(self.runsafe)]
+                        subprocess.run(cmd, check=False)
+                elif self.link_open_modes[0] == self.run and self.pipe:
+                    subprocess.run(shlex.split(self.run),
                                    check=False,
                                    input=url.encode(sys.getdefaultencoding()))
                 else:
-                    cmd = [i.format(url) for i in shlex.split(self.runsafe)]
-                    subprocess.run(cmd, check=False)
-            elif self.link_open_modes[0] == self.run and self.pipe:
-                subprocess.run(shlex.split(self.run),
-                               check=False,
-                               input=url.encode(sys.getdefaultencoding()))
-            else:
-                subprocess.run(self.run.format(url), check=False, shell=True)
+                    subprocess.run(self.run.format(url), check=False, shell=True)
 
-            if self.single is True:
-                self._quit()
-            # Restore normal stderr
-            os.dup2(savout, 2)
-            if thread is False:
-                self.draw_screen()
+                if self.single is True:
+                    self._quit()
         return browse
 
     def process_urls(self, extractedurls, dedupe, shorten):
         """Process the 'extractedurls' and ready them for either the curses browser
         or non-interactive output
 
         Args: extractedurls
@@ -816,25 +815,27 @@
                 i = 0
                 while i < len(chunks):
                     chunk = chunks[i]
                     i += 1
                     if chunk.url is None:
                         markup.append(('msgtext', chunk.markup))
                     else:
+                        chunk.url = chunk.url.strip()
                         if (dedupe is True and chunk.url not in urls) \
                                 or dedupe is False:
                             urls.append(chunk.url)
                             groupurls.append(chunk.url)
                         # Collect all immediately adjacent
                         # chunks with the same URL.
                         tmpmarkup = []
                         if chunk.markup:
                             tmpmarkup.append(('msgtext', chunk.markup))
                         while i < len(chunks) and \
-                                chunks[i].url == chunk.url:
+                                (chunks[i].url if chunks[i].url is None
+                                    else chunks[i].url.strip()) == chunk.url:
                             if chunks[i].markup:
                                 tmpmarkup.append(chunks[i].markup)
                             i += 1
                         url_idx = urls.index(chunk.url) + 1 if dedupe is True else len(urls)
                         markup += [tmpmarkup or '<URL>',
                                    ('urlref:number:braces', ' ['),
                                    ('urlref:number', repr(url_idx)),
@@ -857,7 +858,33 @@
                                                                  shorten),
                                                      self.mkbrowseto(url),
                                                      user_data=url),
                                         'urlref:url', 'url:sel')]
                 items.append(urwid.Columns(markup))
 
         return items, urls
+
+
+@contextlib.contextmanager
+def redirect_output():
+    """
+    A context manager to temporarily redirect stderr and stdout to devnull
+
+    Usage:
+        with redirect_output():
+            webbrowser.open('https://google.com')
+
+    """
+    try:
+        err = os.dup(sys.stderr.fileno())
+        out = os.dup(sys.stdout.fileno())
+        dest_file = open(os.devnull, 'w')
+        os.dup2(dest_file.fileno(), sys.stderr.fileno())
+        os.dup2(dest_file.fileno(), sys.stdout.fileno())
+        yield
+    finally:
+        if err is not None:
+            os.dup2(err, sys.stderr.fileno())
+        if out is not None:
+            os.dup2(out, sys.stdout.fileno())
+        if dest_file is not None:
+            dest_file.close()
```

### Comparing `urlscan-0.9.9/urlscan/urlscan.py` & `urlscan-1.0.0/urlscan/urlscan.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #   Copyright (C) 2006-2007 Daniel Burrows
-#   Copyright (C) 2021 Scott Hansen
+#   Copyright (C) 2023 Scott Hansen
 #
 # This program is free software; you can redistribute it and/or
 # modify it under the terms of the GNU General Public License
 # as published by the Free Software Foundation; either version 2
 # of the License, or (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -241,15 +241,15 @@
             self.handle_data(HTMLChunker.entities[name])
         else:
             # If you see a reference, it needs to be
             # added above.
             self.handle_data(f"&{name};")
 
 
-URLINTERNALPATTERN = r'[{}()@\w/\\\-%?!&.=:;+,#~]'
+URLINTERNALPATTERN = r'[\[\]{}()@\w/\\\-%?!&.=:;+,#~*]'
 URLTRAILINGPATTERN = r'[{}(@\w/\-%&=+#$]'
 HTTPURLPATTERN = (r'(?:(https?|file|ftps?)://' + URLINTERNALPATTERN +
                   r'*' + URLTRAILINGPATTERN + r')')
 # Used to guess that blah.blah.blah.TLD is a URL.
 
 
 def load_tlds():
@@ -287,14 +287,15 @@
 assert not URLRE.match('blah..org')
 assert URLRE.match('http://www.testurl.zw')
 assert URLRE.match('http://www.testurl.smile')
 assert URLRE.match('testurl.smile.smile')
 assert URLRE.match('testurl.biz.smile.zw')
 assert not URLRE.match('example..biz')
 assert not URLRE.match('blah.baz.obviouslynotarealdomain')
+assert URLRE.match('http://[2a07:3500:11a0:320::22]:8080')
 
 
 def parse_text_urls(mesg, regex=None):
     """Parse a block of text, splitting it into its url and non-url
     components."""
 
     rval = []
```

