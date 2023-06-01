# Comparing `tmp/cqwu-0.0.8.tar.gz` & `tmp/cqwu-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cqwu-0.0.8.tar", last modified: Sat Mar 18 06:00:12 2023, max compression
+gzip compressed data, was "cqwu-0.0.9.tar", last modified: Thu Mar 23 14:27:39 2023, max compression
```

## Comparing `cqwu-0.0.8.tar` & `cqwu-0.0.9.tar`

### file list

```diff
@@ -1,56 +1,60 @@
-drwxrwxrwx   0        0        0        0 2023-03-18 06:00:12.117860 cqwu-0.0.8/
--rw-rw-rw-   0        0        0    35184 2023-03-08 07:19:04.000000 cqwu-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      460 2023-03-18 06:00:12.116862 cqwu-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       36 2023-03-08 07:19:04.000000 cqwu-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-03-18 06:00:12.050356 cqwu-0.0.8/cqwu/
--rw-rw-rw-   0        0        0       64 2023-03-08 14:43:56.000000 cqwu-0.0.8/cqwu/__init__.py
--rw-rw-rw-   0        0        0     1799 2023-03-15 09:29:44.000000 cqwu-0.0.8/cqwu/client.py
-drwxrwxrwx   0        0        0        0 2023-03-18 06:00:12.059285 cqwu-0.0.8/cqwu/enums/
--rw-rw-rw-   0        0        0        0 2023-03-08 09:44:33.000000 cqwu-0.0.8/cqwu/enums/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-18 06:00:12.066230 cqwu-0.0.8/cqwu/errors/
--rw-rw-rw-   0        0        0       63 2023-03-16 12:50:43.000000 cqwu-0.0.8/cqwu/errors/__init__.py
--rw-rw-rw-   0        0        0      383 2023-03-17 11:10:14.000000 cqwu-0.0.8/cqwu/errors/auth.py
--rw-rw-rw-   0        0        0       97 2023-03-08 07:44:11.000000 cqwu-0.0.8/cqwu/errors/base.py
--rw-rw-rw-   0        0        0      191 2023-03-16 12:50:43.000000 cqwu-0.0.8/cqwu/errors/epay.py
-drwxrwxrwx   0        0        0        0 2023-03-18 06:00:12.067271 cqwu-0.0.8/cqwu/methods/
--rw-rw-rw-   0        0        0      212 2023-03-15 09:29:44.000000 cqwu-0.0.8/cqwu/methods/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-18 06:00:12.084417 cqwu-0.0.8/cqwu/methods/auth/
--rw-rw-rw-   0        0        0      475 2023-03-08 12:20:02.000000 cqwu-0.0.8/cqwu/methods/auth/__init__.py
--rw-rw-rw-   0        0        0     1268 2023-03-08 12:20:44.000000 cqwu-0.0.8/cqwu/methods/auth/check_captcha.py
--rw-rw-rw-   0        0        0      448 2023-03-08 07:19:04.000000 cqwu-0.0.8/cqwu/methods/auth/export_cookie_to_file.py
--rw-rw-rw-   0        0        0      592 2023-03-08 11:32:25.000000 cqwu-0.0.8/cqwu/methods/auth/login.py
--rw-rw-rw-   0        0        0      798 2023-03-08 11:26:56.000000 cqwu-0.0.8/cqwu/methods/auth/login_with_cookie.py
--rw-rw-rw-   0        0        0      579 2023-03-08 11:26:56.000000 cqwu-0.0.8/cqwu/methods/auth/login_with_cookie_file.py
--rw-rw-rw-   0        0        0     3406 2023-03-17 11:10:00.000000 cqwu-0.0.8/cqwu/methods/auth/login_with_password.py
--rw-rw-rw-   0        0        0      449 2023-03-08 09:19:11.000000 cqwu-0.0.8/cqwu/methods/auth/oauth.py
-drwxrwxrwx   0        0        0        0 2023-03-18 06:00:12.091427 cqwu-0.0.8/cqwu/methods/epay/
--rw-rw-rw-   0        0        0      146 2023-03-08 09:37:42.000000 cqwu-0.0.8/cqwu/methods/epay/__init__.py
--rw-rw-rw-   0        0        0     1238 2023-03-16 12:50:43.000000 cqwu-0.0.8/cqwu/methods/epay/gen_pay_qrcode.py
--rw-rw-rw-   0        0        0      762 2023-03-08 09:14:50.000000 cqwu-0.0.8/cqwu/methods/epay/get_balance.py
-drwxrwxrwx   0        0        0        0 2023-03-18 06:00:12.094047 cqwu-0.0.8/cqwu/methods/users/
--rw-rw-rw-   0        0        0       70 2023-03-08 07:19:04.000000 cqwu-0.0.8/cqwu/methods/users/__init__.py
--rw-rw-rw-   0        0        0     1933 2023-03-08 09:10:31.000000 cqwu-0.0.8/cqwu/methods/users/get_me.py
-drwxrwxrwx   0        0        0        0 2023-03-18 06:00:12.101072 cqwu-0.0.8/cqwu/methods/webvpn/
--rw-rw-rw-   0        0        0      579 2023-03-15 09:29:44.000000 cqwu-0.0.8/cqwu/methods/webvpn/__init__.py
--rw-rw-rw-   0        0        0     5018 2023-03-18 05:48:44.000000 cqwu-0.0.8/cqwu/methods/webvpn/get_calendar.py
--rw-rw-rw-   0        0        0     3954 2023-03-15 09:29:44.000000 cqwu-0.0.8/cqwu/methods/webvpn/get_calendar_change.py
--rw-rw-rw-   0        0        0      814 2023-03-15 09:29:44.000000 cqwu-0.0.8/cqwu/methods/webvpn/login_webvpn.py
-drwxrwxrwx   0        0        0        0 2023-03-18 06:00:12.105454 cqwu-0.0.8/cqwu/methods/xg/
--rw-rw-rw-   0        0        0       77 2023-03-08 10:02:46.000000 cqwu-0.0.8/cqwu/methods/xg/__init__.py
--rw-rw-rw-   0        0        0     2526 2023-03-15 09:29:44.000000 cqwu-0.0.8/cqwu/methods/xg/get_score.py
-drwxrwxrwx   0        0        0        0 2023-03-18 06:00:12.111664 cqwu-0.0.8/cqwu/types/
--rw-rw-rw-   0        0        0       50 2023-03-08 09:56:43.000000 cqwu-0.0.8/cqwu/types/__init__.py
--rw-rw-rw-   0        0        0      539 2023-03-17 14:37:59.000000 cqwu-0.0.8/cqwu/types/calendar.py
--rw-rw-rw-   0        0        0      815 2023-03-08 09:56:29.000000 cqwu-0.0.8/cqwu/types/score.py
--rw-rw-rw-   0        0        0     1400 2023-03-08 07:19:04.000000 cqwu-0.0.8/cqwu/types/user.py
-drwxrwxrwx   0        0        0        0 2023-03-18 06:00:12.115689 cqwu-0.0.8/cqwu/utils/
--rw-rw-rw-   0        0        0       68 2023-03-08 14:54:26.000000 cqwu-0.0.8/cqwu/utils/__init__.py
--rw-rw-rw-   0        0        0    14194 2023-03-08 07:19:04.000000 cqwu-0.0.8/cqwu/utils/auth.py
-drwxrwxrwx   0        0        0        0 2023-03-18 06:00:12.058285 cqwu-0.0.8/cqwu.egg-info/
--rw-rw-rw-   0        0        0      460 2023-03-18 06:00:11.000000 cqwu-0.0.8/cqwu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1105 2023-03-18 06:00:11.000000 cqwu-0.0.8/cqwu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-18 06:00:11.000000 cqwu-0.0.8/cqwu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-03-18 06:00:11.000000 cqwu-0.0.8/cqwu.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-03-18 06:00:11.000000 cqwu-0.0.8/cqwu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-18 06:00:12.117860 cqwu-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1201 2023-03-18 05:48:44.000000 cqwu-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-23 14:27:39.257224 cqwu-0.0.9/
+-rw-rw-rw-   0        0        0    35184 2023-03-08 07:19:04.000000 cqwu-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      460 2023-03-23 14:27:39.254229 cqwu-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       36 2023-03-08 07:19:04.000000 cqwu-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-03-23 14:27:39.154969 cqwu-0.0.9/cqwu/
+-rw-rw-rw-   0        0        0       64 2023-03-08 14:43:56.000000 cqwu-0.0.9/cqwu/__init__.py
+-rw-rw-rw-   0        0        0     1842 2023-03-23 14:26:23.000000 cqwu-0.0.9/cqwu/client.py
+drwxrwxrwx   0        0        0        0 2023-03-23 14:27:39.171924 cqwu-0.0.9/cqwu/enums/
+-rw-rw-rw-   0        0        0        0 2023-03-08 09:44:33.000000 cqwu-0.0.9/cqwu/enums/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-23 14:27:39.180899 cqwu-0.0.9/cqwu/errors/
+-rw-rw-rw-   0        0        0       63 2023-03-16 12:50:43.000000 cqwu-0.0.9/cqwu/errors/__init__.py
+-rw-rw-rw-   0        0        0      383 2023-03-17 11:10:14.000000 cqwu-0.0.9/cqwu/errors/auth.py
+-rw-rw-rw-   0        0        0       97 2023-03-08 07:44:11.000000 cqwu-0.0.9/cqwu/errors/base.py
+-rw-rw-rw-   0        0        0      191 2023-03-16 12:50:43.000000 cqwu-0.0.9/cqwu/errors/epay.py
+drwxrwxrwx   0        0        0        0 2023-03-23 14:27:39.182894 cqwu-0.0.9/cqwu/methods/
+-rw-rw-rw-   0        0        0      212 2023-03-15 09:29:44.000000 cqwu-0.0.9/cqwu/methods/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-23 14:27:39.200849 cqwu-0.0.9/cqwu/methods/auth/
+-rw-rw-rw-   0        0        0      475 2023-03-08 12:20:02.000000 cqwu-0.0.9/cqwu/methods/auth/__init__.py
+-rw-rw-rw-   0        0        0     1268 2023-03-08 12:20:44.000000 cqwu-0.0.9/cqwu/methods/auth/check_captcha.py
+-rw-rw-rw-   0        0        0      448 2023-03-08 07:19:04.000000 cqwu-0.0.9/cqwu/methods/auth/export_cookie_to_file.py
+-rw-rw-rw-   0        0        0      592 2023-03-08 11:32:25.000000 cqwu-0.0.9/cqwu/methods/auth/login.py
+-rw-rw-rw-   0        0        0      798 2023-03-08 11:26:56.000000 cqwu-0.0.9/cqwu/methods/auth/login_with_cookie.py
+-rw-rw-rw-   0        0        0      579 2023-03-08 11:26:56.000000 cqwu-0.0.9/cqwu/methods/auth/login_with_cookie_file.py
+-rw-rw-rw-   0        0        0     3406 2023-03-17 11:10:00.000000 cqwu-0.0.9/cqwu/methods/auth/login_with_password.py
+-rw-rw-rw-   0        0        0      449 2023-03-08 09:19:11.000000 cqwu-0.0.9/cqwu/methods/auth/oauth.py
+drwxrwxrwx   0        0        0        0 2023-03-23 14:27:39.210823 cqwu-0.0.9/cqwu/methods/epay/
+-rw-rw-rw-   0        0        0      201 2023-03-23 14:26:23.000000 cqwu-0.0.9/cqwu/methods/epay/__init__.py
+-rw-rw-rw-   0        0        0     1238 2023-03-16 12:50:43.000000 cqwu-0.0.9/cqwu/methods/epay/gen_pay_qrcode.py
+-rw-rw-rw-   0        0        0      762 2023-03-08 09:14:50.000000 cqwu-0.0.9/cqwu/methods/epay/get_balance.py
+-rw-rw-rw-   0        0        0      782 2023-03-23 14:26:23.000000 cqwu-0.0.9/cqwu/methods/epay/get_pay_bill.py
+drwxrwxrwx   0        0        0        0 2023-03-23 14:27:39.217806 cqwu-0.0.9/cqwu/methods/users/
+-rw-rw-rw-   0        0        0       70 2023-03-08 07:19:04.000000 cqwu-0.0.9/cqwu/methods/users/__init__.py
+-rw-rw-rw-   0        0        0     1933 2023-03-08 09:10:31.000000 cqwu-0.0.9/cqwu/methods/users/get_me.py
+drwxrwxrwx   0        0        0        0 2023-03-23 14:27:39.227298 cqwu-0.0.9/cqwu/methods/webvpn/
+-rw-rw-rw-   0        0        0      579 2023-03-15 09:29:44.000000 cqwu-0.0.9/cqwu/methods/webvpn/__init__.py
+-rw-rw-rw-   0        0        0     5018 2023-03-23 14:26:18.000000 cqwu-0.0.9/cqwu/methods/webvpn/get_calendar.py
+-rw-rw-rw-   0        0        0     3954 2023-03-15 09:29:44.000000 cqwu-0.0.9/cqwu/methods/webvpn/get_calendar_change.py
+-rw-rw-rw-   0        0        0      814 2023-03-15 09:29:44.000000 cqwu-0.0.9/cqwu/methods/webvpn/login_webvpn.py
+drwxrwxrwx   0        0        0        0 2023-03-23 14:27:39.233283 cqwu-0.0.9/cqwu/methods/xg/
+-rw-rw-rw-   0        0        0      116 2023-03-23 14:26:23.000000 cqwu-0.0.9/cqwu/methods/xg/__init__.py
+-rw-rw-rw-   0        0        0     3771 2023-03-23 14:26:23.000000 cqwu-0.0.9/cqwu/methods/xg/get_cp.py
+-rw-rw-rw-   0        0        0     2526 2023-03-15 09:29:44.000000 cqwu-0.0.9/cqwu/methods/xg/get_score.py
+drwxrwxrwx   0        0        0        0 2023-03-23 14:27:39.247245 cqwu-0.0.9/cqwu/types/
+-rw-rw-rw-   0        0        0       50 2023-03-08 09:56:43.000000 cqwu-0.0.9/cqwu/types/__init__.py
+-rw-rw-rw-   0        0        0      539 2023-03-17 14:37:59.000000 cqwu-0.0.9/cqwu/types/calendar.py
+-rw-rw-rw-   0        0        0      348 2023-03-23 14:26:23.000000 cqwu-0.0.9/cqwu/types/cp.py
+-rw-rw-rw-   0        0        0      328 2023-03-23 14:26:23.000000 cqwu-0.0.9/cqwu/types/epay.py
+-rw-rw-rw-   0        0        0      815 2023-03-08 09:56:29.000000 cqwu-0.0.9/cqwu/types/score.py
+-rw-rw-rw-   0        0        0     1400 2023-03-08 07:19:04.000000 cqwu-0.0.9/cqwu/types/user.py
+drwxrwxrwx   0        0        0        0 2023-03-23 14:27:39.251236 cqwu-0.0.9/cqwu/utils/
+-rw-rw-rw-   0        0        0       68 2023-03-08 14:54:26.000000 cqwu-0.0.9/cqwu/utils/__init__.py
+-rw-rw-rw-   0        0        0    14194 2023-03-08 07:19:04.000000 cqwu-0.0.9/cqwu/utils/auth.py
+drwxrwxrwx   0        0        0        0 2023-03-23 14:27:39.168931 cqwu-0.0.9/cqwu.egg-info/
+-rw-rw-rw-   0        0        0      460 2023-03-23 14:27:38.000000 cqwu-0.0.9/cqwu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1201 2023-03-23 14:27:39.000000 cqwu-0.0.9/cqwu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-23 14:27:38.000000 cqwu-0.0.9/cqwu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2023-03-23 14:27:38.000000 cqwu-0.0.9/cqwu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-03-23 14:27:38.000000 cqwu-0.0.9/cqwu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-03-23 14:27:39.257224 cqwu-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1222 2023-03-23 14:26:23.000000 cqwu-0.0.9/setup.py
```

### Comparing `cqwu-0.0.8/LICENSE` & `cqwu-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cqwu-0.0.8/cqwu/client.py` & `cqwu-0.0.9/cqwu/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,24 +11,25 @@
 
     def __init__(
         self,
         username: int = None,
         password: str = None,
         cookie: str = None,
         cookie_file_path: str = "cookie.txt",
+        timeout: int = 10,
     ):
         self.username = username
         self.password = password
         self.cookie = cookie
         self.cookie_file_path = cookie_file_path
         self.host = "http://ehall.cqwu.edu.cn"
         self.auth_host = "http://authserver.cqwu.edu.cn"
         self.web_ehall_path = ""
         self.cookies = Cookies()
-        self.request = AsyncClient()
+        self.request = AsyncClient(timeout=timeout)
         self.loop = asyncio.get_event_loop()
         self.me: Optional[User] = None
         self._use_password_login = False
         self.xue_nian = 2022  # 学年
         self.xue_qi = 1  # 学期 0 为第一学期， 1 为第二学期
 
     @staticmethod
```

### Comparing `cqwu-0.0.8/cqwu/methods/auth/check_captcha.py` & `cqwu-0.0.9/cqwu/methods/auth/check_captcha.py`

 * *Files identical despite different names*

### Comparing `cqwu-0.0.8/cqwu/methods/auth/login.py` & `cqwu-0.0.9/cqwu/methods/auth/login.py`

 * *Files identical despite different names*

### Comparing `cqwu-0.0.8/cqwu/methods/auth/login_with_cookie.py` & `cqwu-0.0.9/cqwu/methods/auth/login_with_cookie.py`

 * *Files identical despite different names*

### Comparing `cqwu-0.0.8/cqwu/methods/auth/login_with_cookie_file.py` & `cqwu-0.0.9/cqwu/methods/auth/login_with_cookie_file.py`

 * *Files identical despite different names*

### Comparing `cqwu-0.0.8/cqwu/methods/auth/login_with_password.py` & `cqwu-0.0.9/cqwu/methods/auth/login_with_password.py`

 * *Files identical despite different names*

### Comparing `cqwu-0.0.8/cqwu/methods/epay/gen_pay_qrcode.py` & `cqwu-0.0.9/cqwu/methods/epay/gen_pay_qrcode.py`

 * *Files identical despite different names*

### Comparing `cqwu-0.0.8/cqwu/methods/epay/get_balance.py` & `cqwu-0.0.9/cqwu/methods/epay/get_balance.py`

 * *Files identical despite different names*

### Comparing `cqwu-0.0.8/cqwu/methods/users/get_me.py` & `cqwu-0.0.9/cqwu/methods/users/get_me.py`

 * *Files identical despite different names*

### Comparing `cqwu-0.0.8/cqwu/methods/webvpn/__init__.py` & `cqwu-0.0.9/cqwu/methods/webvpn/__init__.py`

 * *Files identical despite different names*

### Comparing `cqwu-0.0.8/cqwu/methods/webvpn/get_calendar.py` & `cqwu-0.0.9/cqwu/methods/webvpn/get_calendar.py`

 * *Files identical despite different names*

### Comparing `cqwu-0.0.8/cqwu/methods/webvpn/get_calendar_change.py` & `cqwu-0.0.9/cqwu/methods/webvpn/get_calendar_change.py`

 * *Files identical despite different names*

### Comparing `cqwu-0.0.8/cqwu/methods/webvpn/login_webvpn.py` & `cqwu-0.0.9/cqwu/methods/webvpn/login_webvpn.py`

 * *Files identical despite different names*

### Comparing `cqwu-0.0.8/cqwu/methods/xg/get_score.py` & `cqwu-0.0.9/cqwu/methods/xg/get_score.py`

 * *Files identical despite different names*

### Comparing `cqwu-0.0.8/cqwu/types/calendar.py` & `cqwu-0.0.9/cqwu/types/calendar.py`

 * *Files identical despite different names*

### Comparing `cqwu-0.0.8/cqwu/types/score.py` & `cqwu-0.0.9/cqwu/types/score.py`

 * *Files identical despite different names*

### Comparing `cqwu-0.0.8/cqwu/types/user.py` & `cqwu-0.0.9/cqwu/types/user.py`

 * *Files identical despite different names*

### Comparing `cqwu-0.0.8/cqwu/utils/auth.py` & `cqwu-0.0.9/cqwu/utils/auth.py`

 * *Files identical despite different names*

### Comparing `cqwu-0.0.8/cqwu.egg-info/SOURCES.txt` & `cqwu-0.0.9/cqwu.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -21,21 +21,25 @@
 cqwu/methods/auth/login_with_cookie.py
 cqwu/methods/auth/login_with_cookie_file.py
 cqwu/methods/auth/login_with_password.py
 cqwu/methods/auth/oauth.py
 cqwu/methods/epay/__init__.py
 cqwu/methods/epay/gen_pay_qrcode.py
 cqwu/methods/epay/get_balance.py
+cqwu/methods/epay/get_pay_bill.py
 cqwu/methods/users/__init__.py
 cqwu/methods/users/get_me.py
 cqwu/methods/webvpn/__init__.py
 cqwu/methods/webvpn/get_calendar.py
 cqwu/methods/webvpn/get_calendar_change.py
 cqwu/methods/webvpn/login_webvpn.py
 cqwu/methods/xg/__init__.py
+cqwu/methods/xg/get_cp.py
 cqwu/methods/xg/get_score.py
 cqwu/types/__init__.py
 cqwu/types/calendar.py
+cqwu/types/cp.py
+cqwu/types/epay.py
 cqwu/types/score.py
 cqwu/types/user.py
 cqwu/utils/__init__.py
 cqwu/utils/auth.py
```

### Comparing `cqwu-0.0.8/setup.py` & `cqwu-0.0.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools  # 导入setuptools打包工具
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="cqwu",  # 用自己的名替换其中的YOUR_USERNAME_
-    version="0.0.8",  # 包版本号，便于维护版本
+    version="0.0.9",  # 包版本号，便于维护版本
     author="omg-xtao",  # 作者，可以写自己的姓名
     author_email="xtao@xtaolink.cn",  # 作者联系方式，可写自己的邮箱地址
     description="A cqwu ehall client.",  # 包的简述
     long_description=long_description,  # 包的详细介绍，一般在README.md文件内
     long_description_content_type="text/markdown",
     url="https://github.com/cqwu-ehall/cqwu-ehall",  # 自己项目地址，比如github的项目地址
     packages=setuptools.find_packages(),
@@ -23,9 +23,10 @@
         "httpx",
         "lxml",
         "PyExecJS2",
         "beautifulsoup4",
         "qrcode",
         "pillow",
         "pydantic",
+        "openpyxl",
     ],
 )
```

