# Comparing `tmp/testmsg-0.0.5.tar.gz` & `tmp/testmsg-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testmsg-0.0.5.tar", last modified: Thu May  4 15:42:50 2023, max compression
+gzip compressed data, was "testmsg-0.0.6.tar", last modified: Thu Jun  1 14:38:48 2023, max compression
```

## Comparing `testmsg-0.0.5.tar` & `testmsg-0.0.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-05-04 15:42:50.725884 testmsg-0.0.5/
--rw-r--r--   0 xenon     (1000) xenon     (1000)     2782 2023-05-04 15:42:50.725884 testmsg-0.0.5/PKG-INFO
--rw-r--r--   0 xenon     (1000) xenon     (1000)     1933 2023-05-02 22:33:15.000000 testmsg-0.0.5/README.md
-drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-05-04 15:42:50.725884 testmsg-0.0.5/bin/
--rwxr-xr-x   0 xenon     (1000) xenon     (1000)     3086 2023-05-04 15:37:17.000000 testmsg-0.0.5/bin/testmsg
--rw-r--r--   0 xenon     (1000) xenon     (1000)       38 2023-05-04 15:42:50.725884 testmsg-0.0.5/setup.cfg
--rwxr-xr-x   0 xenon     (1000) xenon     (1000)     1242 2023-05-02 21:41:24.000000 testmsg-0.0.5/setup.py
-drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-05-04 15:42:50.725884 testmsg-0.0.5/testmsg.egg-info/
--rw-r--r--   0 xenon     (1000) xenon     (1000)     2782 2023-05-04 15:42:50.000000 testmsg-0.0.5/testmsg.egg-info/PKG-INFO
--rw-r--r--   0 xenon     (1000) xenon     (1000)      154 2023-05-04 15:42:50.000000 testmsg-0.0.5/testmsg.egg-info/SOURCES.txt
--rw-r--r--   0 xenon     (1000) xenon     (1000)        1 2023-05-04 15:42:50.000000 testmsg-0.0.5/testmsg.egg-info/dependency_links.txt
--rw-r--r--   0 xenon     (1000) xenon     (1000)        1 2023-05-04 15:42:50.000000 testmsg-0.0.5/testmsg.egg-info/top_level.txt
+drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-06-01 14:38:48.471825 testmsg-0.0.6/
+-rw-r--r--   0 xenon     (1000) xenon     (1000)     2960 2023-06-01 14:38:48.471825 testmsg-0.0.6/PKG-INFO
+-rw-r--r--   0 xenon     (1000) xenon     (1000)     2071 2023-06-01 14:38:04.000000 testmsg-0.0.6/README.md
+drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-06-01 14:38:48.471825 testmsg-0.0.6/bin/
+-rwxr-xr-x   0 xenon     (1000) xenon     (1000)     3628 2023-06-01 14:31:26.000000 testmsg-0.0.6/bin/testmsg
+-rw-r--r--   0 xenon     (1000) xenon     (1000)       38 2023-06-01 14:38:48.471825 testmsg-0.0.6/setup.cfg
+-rwxr-xr-x   0 xenon     (1000) xenon     (1000)     1242 2023-05-02 21:41:24.000000 testmsg-0.0.6/setup.py
+drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-06-01 14:38:48.471825 testmsg-0.0.6/testmsg.egg-info/
+-rw-r--r--   0 xenon     (1000) xenon     (1000)     2960 2023-06-01 14:38:48.000000 testmsg-0.0.6/testmsg.egg-info/PKG-INFO
+-rw-r--r--   0 xenon     (1000) xenon     (1000)      154 2023-06-01 14:38:48.000000 testmsg-0.0.6/testmsg.egg-info/SOURCES.txt
+-rw-r--r--   0 xenon     (1000) xenon     (1000)        1 2023-06-01 14:38:48.000000 testmsg-0.0.6/testmsg.egg-info/dependency_links.txt
+-rw-r--r--   0 xenon     (1000) xenon     (1000)        1 2023-06-01 14:38:48.000000 testmsg-0.0.6/testmsg.egg-info/top_level.txt
```

### Comparing `testmsg-0.0.5/PKG-INFO` & `testmsg-0.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testmsg
-Version: 0.0.5
+Version: 0.0.6
 Summary: UNKNOWN
 Home-page: https://github.com/yaroslaff/testmsg
 Author: Yaroslav Polyakov
 Author-email: yaroslaff@gmail.com
 License: MIT
 Description: # testmsg
         Generate RFC822 compliant e-mail messages for tests and send it over SMTP.
@@ -38,23 +38,28 @@
         Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore =
         eu fugiat nulla pariatur.
         Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia des=
         erunt mollit anim id est laborum.
         ~~~
         
         ## Options
+        
+        ### Sending  message
         To actually send message via SMTP server add `--send localhost` or (if you need really powerful SMTP client features) pipe to msmtp:
         ~~~
         testmsg --lorem --to you@gmail.com --from you@example.net | msmtp --host mail.example.net -v --tls=on --tls-starttls=on --auth=on --user=you@example.com --passwordeval "echo YourPass" -f you@example.net you@gmail.com
         ~~~ 
         
+        ### Customize message
         Use `--from`, `--to` and `--subject` to override basic properties of message, use `--add HEADER VALUE` to add custom header(s).
         
-        Default message text is empty, use `--text "blah blah blah"` or `--lorem` or `--file PATH` or `--file -` .(to read from stdin). Add `--time` to add current time as an prefix to text.
+        Default message text is empty, use `--text "blah blah blah"` or `--lorem` or `--msg PATH` or `--msg -` .(to read from stdin). Add `--time` to add current time as an prefix to text.
         
+        ### Add attachments
+        Use `--attachment` (or `--att`) to add attachments: `--att FILE1 FILE2 ...`
         
         
         
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `testmsg-0.0.5/README.md` & `testmsg-0.0.6/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -30,18 +30,23 @@
 Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore =
 eu fugiat nulla pariatur.
 Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia des=
 erunt mollit anim id est laborum.
 ~~~
 
 ## Options
+
+### Sending  message
 To actually send message via SMTP server add `--send localhost` or (if you need really powerful SMTP client features) pipe to msmtp:
 ~~~
 testmsg --lorem --to you@gmail.com --from you@example.net | msmtp --host mail.example.net -v --tls=on --tls-starttls=on --auth=on --user=you@example.com --passwordeval "echo YourPass" -f you@example.net you@gmail.com
 ~~~ 
 
+### Customize message
 Use `--from`, `--to` and `--subject` to override basic properties of message, use `--add HEADER VALUE` to add custom header(s).
 
-Default message text is empty, use `--text "blah blah blah"` or `--lorem` or `--file PATH` or `--file -` .(to read from stdin). Add `--time` to add current time as an prefix to text.
+Default message text is empty, use `--text "blah blah blah"` or `--lorem` or `--msg PATH` or `--msg -` .(to read from stdin). Add `--time` to add current time as an prefix to text.
 
+### Add attachments
+Use `--attachment` (or `--att`) to add attachments: `--att FILE1 FILE2 ...`
```

### Comparing `testmsg-0.0.5/bin/testmsg` & `testmsg-0.0.6/bin/testmsg`

 * *Files 18% similar despite different names*

```diff
@@ -1,74 +1,94 @@
 #!/usr/bin/env python3
 import smtplib
 import argparse
 import datetime
 import sys
+import mimetypes
 from email.message import EmailMessage
 
 lorem = "Lorem ipsum dolor sit amet, consectetur adipiscing elit, " \
     "sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.\n" \
     "Ut enim ad minim veniam," \
     "quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.\n" \
     "Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.\n" \
     "Excepteur sint occaecat cupidatat non proident, " \
     "sunt in culpa qui officia deserunt mollit anim id est laborum.\n"
 
-version='0.0.5'
+version='0.0.6'
+
+
+def attach(msg: EmailMessage, path: str):
+
+    ctype, _ = mimetypes.guess_type(path)
+    maintype, subtype = ctype.split('/', 1)
+
+    with open(path, 'rb') as fp:
+        msg.add_attachment(fp.read(),
+                            maintype=maintype,
+                            subtype=subtype,
+                            filename=path)
+
 
 def get_args():
     parser = argparse.ArgumentParser(description=f'Generate/Send valid RFC822 email messages for testing {version}')
     parser.add_argument('-f', '--from', dest='_from', default='from@example.com', metavar='EMAIL')
     parser.add_argument('-t', '--to', default='to@example.net', metavar='EMAIL')
     parser.add_argument('-s', '--subject', metavar='Subject', default='Sent with github.com/yaroslaff/testmsg')
     parser.add_argument('-a', '--add', nargs=2, action='append', dest='headers', metavar=('HEADER', 'VALUE'), help='add header')
 
 
     g = parser.add_argument_group('Message body')
     g.add_argument('--text')
     g.add_argument('--lorem', default=False, action='store_true', help='Use lorem ipsum...')
-    g.add_argument('--file', help='read message body from file (or "-" to read from stdin)')
+    g.add_argument('--msg', metavar='FILE', help='read message body from file (or "-" to read from stdin)')
     g.add_argument('--time', default=False, action='store_true', help='add timestamp to text')
 
+    g.add_argument('--attach', nargs='+', metavar='FILE', help='add attachment')
 
     g = parser.add_argument_group('Sending (optional)')
     g.add_argument('--send', metavar='HOST')
     g.add_argument('-v', '--verbose', default=False, action='store_true', help='Verbose SMTP')
 
 
     return parser.parse_args()
 
 def main():
 
     args = get_args()
+
     text = ''
 
     # generate text
     if args.text:
         text = args.text
     elif args.lorem:
         text = lorem
-    elif args.file:
-        if args.file == '-':
+    elif args.msg:
+        if args.msg == '-':
             for line in sys.stdin:
                 text += line;
         else:
-            with open(args.file) as fh:
+            with open(args.msg) as fh:
                 text = fh.read()
 
     if args.time:
         text = datetime.datetime.now().strftime('%D %H:%M:%S') + '\n' + text
 
     msg = EmailMessage()
     msg.set_content(text)
 
     if args.headers:
         for h in args.headers:
             msg.add_header(h[0], h[1])
 
+    if args.attach:
+        for att_file in args.attach:
+            attach(msg, att_file)
+
     # me == the sender's email address
     # you == the recipient's email address
     msg['Subject'] = args.subject
     msg['From'] = args._from or None
     msg['To'] = args.to
 
     # Send the message via our own SMTP server.
```

### Comparing `testmsg-0.0.5/setup.py` & `testmsg-0.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `testmsg-0.0.5/testmsg.egg-info/PKG-INFO` & `testmsg-0.0.6/testmsg.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testmsg
-Version: 0.0.5
+Version: 0.0.6
 Summary: UNKNOWN
 Home-page: https://github.com/yaroslaff/testmsg
 Author: Yaroslav Polyakov
 Author-email: yaroslaff@gmail.com
 License: MIT
 Description: # testmsg
         Generate RFC822 compliant e-mail messages for tests and send it over SMTP.
@@ -38,23 +38,28 @@
         Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore =
         eu fugiat nulla pariatur.
         Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia des=
         erunt mollit anim id est laborum.
         ~~~
         
         ## Options
+        
+        ### Sending  message
         To actually send message via SMTP server add `--send localhost` or (if you need really powerful SMTP client features) pipe to msmtp:
         ~~~
         testmsg --lorem --to you@gmail.com --from you@example.net | msmtp --host mail.example.net -v --tls=on --tls-starttls=on --auth=on --user=you@example.com --passwordeval "echo YourPass" -f you@example.net you@gmail.com
         ~~~ 
         
+        ### Customize message
         Use `--from`, `--to` and `--subject` to override basic properties of message, use `--add HEADER VALUE` to add custom header(s).
         
-        Default message text is empty, use `--text "blah blah blah"` or `--lorem` or `--file PATH` or `--file -` .(to read from stdin). Add `--time` to add current time as an prefix to text.
+        Default message text is empty, use `--text "blah blah blah"` or `--lorem` or `--msg PATH` or `--msg -` .(to read from stdin). Add `--time` to add current time as an prefix to text.
         
+        ### Add attachments
+        Use `--attachment` (or `--att`) to add attachments: `--att FILE1 FILE2 ...`
         
         
         
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

