# Comparing `tmp/badi_users-1.0.7.tar.gz` & `tmp/badi_users-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "badi_users-1.0.7.tar", last modified: Thu Jun  1 07:35:08 2023, max compression
+gzip compressed data, was "badi_users-1.0.8.tar", last modified: Thu Jun  1 08:08:20 2023, max compression
```

## Comparing `badi_users-1.0.7.tar` & `badi_users-1.0.8.tar`

### file list

```diff
@@ -1,317 +1,322 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 07:35:08.486431 badi_users-1.0.7/
--rw-rw-rw-   0        0        0     1093 2022-09-24 06:05:13.000000 badi_users-1.0.7/LICENSE
--rw-rw-rw-   0        0        0     1066 2022-11-10 17:03:20.000000 badi_users-1.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0      419 2023-06-01 07:35:08.486431 badi_users-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      143 2022-10-02 09:04:41.000000 badi_users-1.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 07:35:08.164293 badi_users-1.0.7/badi_ticket/
--rw-rw-rw-   0        0        0        0 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_ticket/__init__.py
--rw-rw-rw-   0        0        0      143 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_ticket/admin.py
--rw-rw-rw-   0        0        0     9892 2023-04-27 05:00:29.000000 badi_users-1.0.7/badi_ticket/api.py
--rw-rw-rw-   0        0        0      129 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_ticket/apps.py
-drwxrwxrwx   0        0        0        0 2023-06-01 07:35:08.124416 badi_users-1.0.7/badi_ticket/locale/
-drwxrwxrwx   0        0        0        0 2023-06-01 07:35:08.124416 badi_users-1.0.7/badi_ticket/locale/fa/
-drwxrwxrwx   0        0        0        0 2023-06-01 07:35:08.165290 badi_users-1.0.7/badi_ticket/locale/fa/LC_MESSAGES/
--rw-rw-rw-   0        0        0     2781 2023-06-01 07:29:15.000000 badi_users-1.0.7/badi_ticket/locale/fa/LC_MESSAGES/django.mo
-drwxrwxrwx   0        0        0        0 2023-06-01 07:35:08.166287 badi_users-1.0.7/badi_ticket/migrations/
--rw-rw-rw-   0        0        0        0 2022-08-06 18:28:13.000000 badi_users-1.0.7/badi_ticket/migrations/__init__.py
--rw-rw-rw-   0        0        0     4335 2023-05-02 06:51:52.000000 badi_users-1.0.7/badi_ticket/models.py
--rw-rw-rw-   0        0        0      313 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_ticket/routers.py
--rw-rw-rw-   0        0        0     2618 2023-05-07 09:45:31.000000 badi_users-1.0.7/badi_ticket/serializers.py
-drwxrwxrwx   0        0        0        0 2023-06-01 07:35:08.125413 badi_users-1.0.7/badi_ticket/static/
-drwxrwxrwx   0        0        0        0 2023-06-01 07:35:08.125413 badi_users-1.0.7/badi_ticket/static/ticket/
-drwxrwxrwx   0        0        0        0 2023-06-01 07:35:08.167284 badi_users-1.0.7/badi_ticket/static/ticket/js/
--rw-rw-rw-   0        0        0     2448 2023-04-16 09:16:22.000000 badi_users-1.0.7/badi_ticket/static/ticket/js/chat.js
-drwxrwxrwx   0        0        0        0 2023-06-01 07:35:08.168282 badi_users-1.0.7/badi_ticket/templates/
--rw-rw-rw-   0        0        0        0 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_ticket/templates/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 07:35:08.174266 badi_users-1.0.7/badi_ticket/templates/ticket/
--rw-rw-rw-   0        0        0     6358 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_ticket/templates/ticket/admin_tickets.html
--rw-rw-rw-   0        0        0     5265 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_ticket/templates/ticket/message_list.html
--rw-rw-rw-   0        0        0     9642 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_ticket/templates/ticket/my_tickets.html
--rw-rw-rw-   0        0        0     7214 2023-04-27 04:28:28.000000 badi_users-1.0.7/badi_ticket/templates/ticket/ticket_create.html
--rw-rw-rw-   0        0        0     1639 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_ticket/templates/ticket/ticket_update.html
--rw-rw-rw-   0        0        0       63 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_ticket/tests.py
--rw-rw-rw-   0        0        0      583 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_ticket/urls.py
--rw-rw-rw-   0        0        0     2099 2023-04-27 04:25:44.000000 badi_users-1.0.7/badi_ticket/views.py
-drwxrwxrwx   0        0        0        0 2023-06-01 07:35:08.182245 badi_users-1.0.7/badi_user/
--rw-rw-rw-   0        0        0        0 2023-05-24 05:07:29.000000 badi_users-1.0.7/badi_user/__init__.py
--rw-rw-rw-   0        0        0      166 2023-05-24 05:07:29.000000 badi_users-1.0.7/badi_user/admin.py
-drwxrwxrwx   0        0        0        0 2023-06-01 07:35:08.187231 badi_users-1.0.7/badi_user/api/
--rw-rw-rw-   0        0        0        0 2023-05-24 05:07:29.000000 badi_users-1.0.7/badi_user/api/__init__.py
--rw-rw-rw-   0        0        0    29905 2023-05-24 05:07:29.000000 badi_users-1.0.7/badi_user/api/api.py
--rw-rw-rw-   0        0        0      485 2023-05-24 05:07:29.000000 badi_users-1.0.7/badi_user/api/routers.py
--rw-rw-rw-   0        0        0     5939 2023-05-24 05:07:29.000000 badi_users-1.0.7/badi_user/api/serializers.py
--rw-rw-rw-   0        0        0      183 2023-05-24 05:07:29.000000 badi_users-1.0.7/badi_user/apps.py
--rw-rw-rw-   0        0        0     3428 2023-05-24 05:07:29.000000 badi_users-1.0.7/badi_user/filter.py
-drwxrwxrwx   0        0        0        0 2023-06-01 07:35:08.134372 badi_users-1.0.7/badi_user/locale/
-drwxrwxrwx   0        0        0        0 2023-06-01 07:35:08.134372 badi_users-1.0.7/badi_user/locale/fa/
-drwxrwxrwx   0        0        0        0 2023-06-01 07:35:08.188229 badi_users-1.0.7/badi_user/locale/fa/LC_MESSAGES/
--rw-rw-rw-   0        0        0     4486 2023-06-01 07:29:16.000000 badi_users-1.0.7/badi_user/locale/fa/LC_MESSAGES/django.mo
-drwxrwxrwx   0        0        0        0 2023-06-01 07:35:08.189226 badi_users-1.0.7/badi_user/migrations/
--rw-rw-rw-   0        0        0        0 2022-08-06 18:28:13.000000 badi_users-1.0.7/badi_user/migrations/__init__.py
--rw-rw-rw-   0        0        0     6895 2023-05-24 05:07:29.000000 badi_users-1.0.7/badi_user/models.py
-drwxrwxrwx   0        0        0        0 2023-06-01 07:35:08.192218 badi_users-1.0.7/badi_user/templates/
--rw-rw-rw-   0        0        0        0 2023-05-24 05:07:29.000000 badi_users-1.0.7/badi_user/templates/__init__.py
--rw-rw-rw-   0        0        0       27 2023-05-24 05:07:29.000000 badi_users-1.0.7/badi_user/templates/badi-user-test.html
-drwxrwxrwx   0        0        0        0 2023-06-01 07:35:08.194213 badi_users-1.0.7/badi_user/templates/group/
--rw-rw-rw-   0        0        0     8558 2023-05-24 05:07:30.000000 badi_users-1.0.7/badi_user/templates/group/group_create.html
--rw-rw-rw-   0        0        0     5472 2023-05-24 05:07:30.000000 badi_users-1.0.7/badi_user/templates/group/group_update.html
-drwxrwxrwx   0        0        0        0 2023-06-01 07:35:08.195210 badi_users-1.0.7/badi_user/templates/log/
--rw-rw-rw-   0        0        0     3987 2023-05-24 05:07:30.000000 badi_users-1.0.7/badi_user/templates/log/log_list.html
-drwxrwxrwx   0        0        0        0 2023-06-01 07:35:08.196207 badi_users-1.0.7/badi_user/templates/login-theme/
--rw-rw-rw-   0        0        0     7336 2023-05-24 05:07:30.000000 badi_users-1.0.7/badi_user/templates/login-theme/login-1.html
-drwxrwxrwx   0        0        0        0 2023-06-01 07:35:08.201194 badi_users-1.0.7/badi_user/templates/member/
--rw-rw-rw-   0        0        0     6863 2023-05-24 05:07:30.000000 badi_users-1.0.7/badi_user/templates/member/member_create.html
--rw-rw-rw-   0        0        0    22635 2023-05-24 05:07:30.000000 badi_users-1.0.7/badi_user/templates/member/member_list.html
--rw-rw-rw-   0        0        0     4783 2023-05-24 05:07:30.000000 badi_users-1.0.7/badi_user/templates/member/member_self_update.html
--rw-rw-rw-   0        0        0     6525 2023-05-24 05:07:30.000000 badi_users-1.0.7/badi_user/templates/member/member_update.html
-drwxrwxrwx   0        0        0        0 2023-06-01 07:35:08.205184 badi_users-1.0.7/badi_user/templates/user/
--rw-rw-rw-   0        0        0     5056 2023-05-24 05:07:29.000000 badi_users-1.0.7/badi_user/templates/user/change_password.html
--rw-rw-rw-   0        0        0     6743 2023-05-24 05:07:29.000000 badi_users-1.0.7/badi_user/templates/user/user_create.html
--rw-rw-rw-   0        0        0     4019 2023-05-24 05:07:29.000000 badi_users-1.0.7/badi_user/templates/user/user_list.html
--rw-rw-rw-   0        0        0     5005 2023-05-24 05:07:29.000000 badi_users-1.0.7/badi_user/templates/user/user_update.html
-drwxrwxrwx   0        0        0        0 2023-06-01 07:35:08.207178 badi_users-1.0.7/badi_user/templatetags/
--rw-rw-rw-   0        0        0        0 2023-05-24 05:07:30.000000 badi_users-1.0.7/badi_user/templatetags/__init__.py
--rw-rw-rw-   0        0        0     5950 2023-05-24 05:07:30.000000 badi_users-1.0.7/badi_user/templatetags/appfilter.py
--rw-rw-rw-   0        0        0      500 2023-05-24 05:07:29.000000 badi_users-1.0.7/badi_user/tests.py
-drwxrwxrwx   0        0        0        0 2023-06-01 07:35:08.216154 badi_users-1.0.7/badi_user/ui/
--rw-rw-rw-   0        0        0        0 2023-05-24 05:07:29.000000 badi_users-1.0.7/badi_user/ui/__init__.py
--rw-rw-rw-   0        0        0     1484 2023-05-24 05:07:29.000000 badi_users-1.0.7/badi_user/ui/forms.py
--rw-rw-rw-   0        0        0      320 2023-05-24 05:07:29.000000 badi_users-1.0.7/badi_user/ui/log_views.py
--rw-rw-rw-   0        0        0     1706 2023-05-24 05:07:29.000000 badi_users-1.0.7/badi_user/ui/member_views.py
--rw-rw-rw-   0        0        0      672 2023-05-24 05:07:29.000000 badi_users-1.0.7/badi_user/ui/notification_views.py
--rw-rw-rw-   0        0        0      644 2023-05-24 05:07:29.000000 badi_users-1.0.7/badi_user/ui/roles_views.py
--rw-rw-rw-   0        0        0     1624 2023-05-24 05:07:29.000000 badi_users-1.0.7/badi_user/ui/urls.py
--rw-rw-rw-   0        0        0     2633 2023-05-24 05:07:29.000000 badi_users-1.0.7/badi_user/ui/views.py
-drwxrwxrwx   0        0        0        0 2023-06-01 07:35:08.238096 badi_users-1.0.7/badi_users.egg-info/
--rw-rw-rw-   0        0        0      419 2023-06-01 07:35:07.000000 badi_users-1.0.7/badi_users.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    10996 2023-06-01 07:35:08.000000 badi_users-1.0.7/badi_users.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 07:35:07.000000 badi_users-1.0.7/badi_users.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-06-01 07:35:07.000000 badi_users-1.0.7/badi_users.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-01 07:35:08.256048 badi_users-1.0.7/badi_utils/
--rw-rw-rw-   0        0        0        0 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/__init__.py
--rw-rw-rw-   0        0        0     6835 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/date_calc.py
--rw-rw-rw-   0        0        0    28237 2023-05-10 09:02:15.000000 badi_users-1.0.7/badi_utils/dynamic.py
--rw-rw-rw-   0        0        0    22478 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/dynamic_api.py
--rw-rw-rw-   0        0        0     3412 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/dynamic_models.py
--rw-rw-rw-   0        0        0     2990 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/email.py
--rw-rw-rw-   0        0        0      252 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/errors.py
--rw-rw-rw-   0        0        0     1509 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/logging.py
--rw-rw-rw-   0        0        0      947 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/responses.py
--rw-rw-rw-   0        0        0      904 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/rss.py
--rw-rw-rw-   0        0        0     1529 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/select2.py
--rw-rw-rw-   0        0        0     3714 2023-05-07 04:58:19.000000 badi_users-1.0.7/badi_utils/sms.py
-drwxrwxrwx   0        0        0        0 2023-06-01 07:35:08.140356 badi_users-1.0.7/badi_utils/static/
-drwxrwxrwx   0        0        0        0 2023-06-01 07:35:08.140356 badi_users-1.0.7/badi_utils/static/badi_utils/
-drwxrwxrwx   0        0        0        0 2023-06-01 07:35:08.257044 badi_users-1.0.7/badi_utils/static/badi_utils/css/
--rw-rw-rw-   0        0        0    40504 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/static/badi_utils/css/custom.css
-drwxrwxrwx   0        0        0        0 2023-06-01 07:35:08.326857 badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/
--rw-rw-rw-   0        0        0    59778 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).eot
--rw-rw-rw-   0        0        0    59532 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).ttf
--rw-rw-rw-   0        0        0    38401 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).woff
--rw-rw-rw-   0        0        0    31304 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).woff2
--rw-rw-rw-   0        0        0    59778 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_2.eot
--rw-rw-rw-   0        0        0    31992 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.eot
--rw-rw-rw-   0        0        0    57268 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.ttf
--rw-rw-rw-   0        0        0    36069 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.woff
--rw-rw-rw-   0        0        0    28856 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.woff2
--rw-rw-rw-   0        0        0    31992 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold_2.eot
--rw-rw-rw-   0        0        0    35477 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.eot
--rw-rw-rw-   0        0        0    60584 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.ttf
--rw-rw-rw-   0        0        0    39557 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.woff
--rw-rw-rw-   0        0        0    32344 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.woff2
--rw-rw-rw-   0        0        0    35477 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light_2.eot
--rw-rw-rw-   0        0        0    32043 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.eot
--rw-rw-rw-   0        0        0    58192 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.ttf
--rw-rw-rw-   0        0        0    36145 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.woff
--rw-rw-rw-   0        0        0    28912 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.woff2
--rw-rw-rw-   0        0        0    32043 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium_2.eot
--rw-rw-rw-   0        0        0    33102 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.eot
--rw-rw-rw-   0        0        0    56352 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.ttf
--rw-rw-rw-   0        0        0    36913 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.woff
--rw-rw-rw-   0        0        0    30072 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.woff2
--rw-rw-rw-   0        0        0    33102 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight_2.eot
--rw-rw-rw-   0        0        0    58886 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb.eot
--rw-rw-rw-   0        0        0    38473 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb.woff
--rw-rw-rw-   0        0        0    31320 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb.woff2
--rw-rw-rw-   0        0        0    58886 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_2.eot
--rw-rw-rw-   0        0        0    57974 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.eot
--rw-rw-rw-   0        0        0    57760 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.ttf
--rw-rw-rw-   0        0        0    36629 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.woff
--rw-rw-rw-   0        0        0    29688 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.woff2
--rw-rw-rw-   0        0        0    57974 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold_2.eot
--rw-rw-rw-   0        0        0    57974 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold_3.eot
--rw-rw-rw-   0        0        0    35458 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.eot
--rw-rw-rw-   0        0        0    59968 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.ttf
--rw-rw-rw-   0        0        0    39693 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.woff
--rw-rw-rw-   0        0        0    32420 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.woff2
--rw-rw-rw-   0        0        0    35458 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light_2.eot
--rw-rw-rw-   0        0        0    31983 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.eot
--rw-rw-rw-   0        0        0    57544 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.ttf
--rw-rw-rw-   0        0        0    36141 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.woff
--rw-rw-rw-   0        0        0    28916 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.woff2
--rw-rw-rw-   0        0        0    31983 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium_2.eot
--rw-rw-rw-   0        0        0    33044 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.eot
--rw-rw-rw-   0        0        0    55640 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.ttf
--rw-rw-rw-   0        0        0    36945 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.woff
--rw-rw-rw-   0        0        0    29840 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.woff2
--rw-rw-rw-   0        0        0    33044 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight_2.eot
--rw-rw-rw-   0        0        0    93376 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/Ray-Black.ttf
--rw-rw-rw-   0        0        0    94304 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/Ray-Bold.ttf
--rw-rw-rw-   0        0        0    94740 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/Ray.ttf
-drwxrwxrwx   0        0        0        0 2023-06-01 07:35:08.345807 badi_users-1.0.7/badi_utils/static/badi_utils/js/
--rw-rw-rw-   0        0        0   478686 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/static/badi_utils/js/apexchart.js
--rw-rw-rw-   0        0        0    19110 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/static/badi_utils/js/api-login.js
--rw-rw-rw-   0        0        0    20445 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/static/badi_utils/js/api.js
--rw-rw-rw-   0        0        0    25944 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/static/badi_utils/js/base.js
--rw-rw-rw-   0        0        0     2149 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/static/badi_utils/js/chat.js
--rw-rw-rw-   0        0        0     3167 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/static/badi_utils/js/custom-vue.js
--rw-rw-rw-   0        0        0    18429 2023-04-16 15:34:42.000000 badi_users-1.0.7/badi_utils/static/badi_utils/js/datatable.js
--rw-rw-rw-   0        0        0     2470 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/static/badi_utils/js/image-field.js
--rw-rw-rw-   0        0        0    30541 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/static/badi_utils/js/main.js
--rw-rw-rw-   0        0        0      959 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/static/badi_utils/js/notification.js
--rw-rw-rw-   0        0        0     2213 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/static/badi_utils/js/pagination-vue.js
--rw-rw-rw-   0        0        0    20317 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/static/badi_utils/js/tableexport.js
--rw-rw-rw-   0        0        0      654 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/static/badi_utils/js/transaction.js
--rw-rw-rw-   0        0        0   354110 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/static/badi_utils/js/vue.js
--rw-rw-rw-   0        0        0   268386 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/static/badi_utils/js/xlsx.mini.min.js
-drwxrwxrwx   0        0        0        0 2023-06-01 07:35:08.348800 badi_users-1.0.7/badi_utils/templates/
--rw-rw-rw-   0        0        0        0 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 07:35:08.372735 badi_users-1.0.7/badi_utils/templates/component/
--rw-rw-rw-   0        0        0     1777 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/component/createModal.html
--rw-rw-rw-   0        0        0     1645 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/component/createTitle.html
--rw-rw-rw-   0        0        0     1054 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/component/filter-form.html
--rw-rw-rw-   0        0        0      729 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/component/form-errors.html
--rw-rw-rw-   0        0        0     1340 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/component/form-progressbar-js.html
--rw-rw-rw-   0        0        0      491 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/component/form-progressbar.html
--rw-rw-rw-   0        0        0      342 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/component/form.html
--rw-rw-rw-   0        0        0     1231 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/component/image-field.html
--rw-rw-rw-   0        0        0    34439 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/component/index-menu.html
--rw-rw-rw-   0        0        0     2346 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/component/input.html
--rw-rw-rw-   0        0        0       69 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/component/loader.html
--rw-rw-rw-   0        0        0      468 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/component/menu-item.html
--rw-rw-rw-   0        0        0      362 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/component/menu-list.html
--rw-rw-rw-   0        0        0      746 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/component/messages.html
--rw-rw-rw-   0        0        0     1134 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/component/pagination-vue.html
--rw-rw-rw-   0        0        0     2491 2023-05-23 08:24:01.000000 badi_users-1.0.7/badi_utils/templates/component/pagination.html
--rw-rw-rw-   0        0        0      361 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/component/profile_item.html
--rw-rw-rw-   0        0        0      204 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/component/space-between.html
--rw-rw-rw-   0        0        0      430 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/component/svg-button-with-text.html
--rw-rw-rw-   0        0        0      428 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/component/svg-button.html
--rw-rw-rw-   0        0        0     1411 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/component/table-item.html
--rw-rw-rw-   0        0        0     2114 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/component/user-card.html
--rw-rw-rw-   0        0        0      257 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/component/yesno.html
-drwxrwxrwx   0        0        0        0 2023-06-01 07:35:08.445541 badi_users-1.0.7/badi_utils/templates/svg/
--rw-rw-rw-   0        0        0     1949 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/svg/Incoming-box.html
--rw-rw-rw-   0        0        0     1159 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/svg/add-user.html
--rw-rw-rw-   0        0        0     1092 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/svg/address-book.html
--rw-rw-rw-   0        0        0     1095 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/svg/arrow-left.html
--rw-rw-rw-   0        0        0     1081 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/svg/arrow-right.html
--rw-rw-rw-   0        0        0     2024 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/svg/bitcoin.html
--rw-rw-rw-   0        0        0      697 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/svg/box.html
--rw-rw-rw-   0        0        0     1378 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/svg/calendar-day.html
--rw-rw-rw-   0        0        0     1489 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/svg/calendar-gym.html
--rw-rw-rw-   0        0        0      925 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/svg/calendar.html
--rw-rw-rw-   0        0        0     1223 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/svg/call.html
--rw-rw-rw-   0        0        0     1385 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/svg/category.html
--rw-rw-rw-   0        0        0     1270 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/svg/chat.html
--rw-rw-rw-   0        0        0      938 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/svg/check.html
--rw-rw-rw-   0        0        0      344 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/svg/circle.html
--rw-rw-rw-   0        0        0     1686 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/svg/city.html
--rw-rw-rw-   0        0        0     1430 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/svg/clipboard-list.html
--rw-rw-rw-   0        0        0     2247 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/svg/clock.html
--rw-rw-rw-   0        0        0      645 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/svg/close.html
--rw-rw-rw-   0        0        0     2483 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/svg/collection.html
--rw-rw-rw-   0        0        0     1046 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/svg/comment.html
--rw-rw-rw-   0        0        0     1103 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/svg/dashboard.html
--rw-rw-rw-   0        0        0      893 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/svg/delete.html
--rw-rw-rw-   0        0        0     1521 2023-06-01 05:43:12.000000 badi_users-1.0.7/badi_utils/templates/svg/discount-code.html
--rw-rw-rw-   0        0        0     1505 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/svg/download.html
--rw-rw-rw-   0        0        0      901 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/svg/edit.html
--rw-rw-rw-   0        0        0     1361 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/svg/file-check.html
--rw-rw-rw-   0        0        0      988 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/svg/file.html
--rw-rw-rw-   0        0        0     2111 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/svg/film.html
--rw-rw-rw-   0        0        0      681 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/svg/fire.html
--rw-rw-rw-   0        0        0     1252 2023-06-01 05:43:38.000000 badi_users-1.0.7/badi_utils/templates/svg/gift.html
--rw-rw-rw-   0        0        0     1648 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/svg/group-chat.html
--rw-rw-rw-   0        0        0     1213 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/svg/group.html
--rw-rw-rw-   0        0        0     1394 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/svg/half_star.html
--rw-rw-rw-   0        0        0      944 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/svg/home.html
--rw-rw-rw-   0        0        0     1906 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/svg/hourse.html
--rw-rw-rw-   0        0        0      631 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/svg/image.html
--rw-rw-rw-   0        0        0      508 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/svg/info.html
--rw-rw-rw-   0        0        0     1394 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/svg/interview.html
--rw-rw-rw-   0        0        0     1389 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/svg/key.html
--rw-rw-rw-   0        0        0     2472 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/svg/logout.html
--rw-rw-rw-   0        0        0      940 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/svg/mail.html
--rw-rw-rw-   0        0        0      731 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/svg/map.html
--rw-rw-rw-   0        0        0     1601 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/svg/message.html
--rw-rw-rw-   0        0        0     1607 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/svg/messages.html
--rw-rw-rw-   0        0        0      683 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/svg/notification.html
--rw-rw-rw-   0        0        0      708 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/svg/plus.html
--rw-rw-rw-   0        0        0      753 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/svg/puzzle.html
--rw-rw-rw-   0        0        0      882 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/svg/question.html
--rw-rw-rw-   0        0        0     1174 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/svg/refresh.html
--rw-rw-rw-   0        0        0     1416 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/svg/safe.html
--rw-rw-rw-   0        0        0     1091 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/svg/search.html
--rw-rw-rw-   0        0        0     1114 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/svg/shield-protected.html
--rw-rw-rw-   0        0        0     1219 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/svg/shield-user.html
--rw-rw-rw-   0        0        0      451 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/svg/slide.html
--rw-rw-rw-   0        0        0     1587 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/svg/timer.html
--rw-rw-rw-   0        0        0     1043 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/svg/town.html
--rw-rw-rw-   0        0        0      804 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/svg/user.html
--rw-rw-rw-   0        0        0      936 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/svg/wallet.html
--rw-rw-rw-   0        0        0      933 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/svg/warning.html
--rw-rw-rw-   0        0        0       19 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templates/test.html
-drwxrwxrwx   0        0        0        0 2023-06-01 07:35:08.447535 badi_users-1.0.7/badi_utils/templatetags/
--rw-rw-rw-   0        0        0        0 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/templatetags/__init__.py
--rw-rw-rw-   0        0        0      555 2023-05-23 08:22:50.000000 badi_users-1.0.7/badi_utils/templatetags/badi_utils.py
--rw-rw-rw-   0        0        0     7102 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/utils.py
--rw-rw-rw-   0        0        0     1911 2023-04-11 07:22:40.000000 badi_users-1.0.7/badi_utils/validations.py
-drwxrwxrwx   0        0        0        0 2023-06-01 07:35:08.453519 badi_users-1.0.7/badi_visit/
--rw-rw-rw-   0        0        0        0 2022-08-14 04:14:27.000000 badi_users-1.0.7/badi_visit/__init__.py
--rw-rw-rw-   0        0        0      167 2022-11-10 16:59:20.000000 badi_users-1.0.7/badi_visit/admin.py
-drwxrwxrwx   0        0        0        0 2023-06-01 07:35:08.456510 badi_users-1.0.7/badi_visit/api/
--rw-rw-rw-   0        0        0        0 2022-10-24 15:37:24.000000 badi_users-1.0.7/badi_visit/api/__init__.py
--rw-rw-rw-   0        0        0     2871 2022-11-10 16:59:20.000000 badi_users-1.0.7/badi_visit/api/api.py
--rw-rw-rw-   0        0        0      208 2022-11-10 16:59:20.000000 badi_users-1.0.7/badi_visit/api/routers.py
--rw-rw-rw-   0        0        0      185 2022-11-10 16:59:20.000000 badi_users-1.0.7/badi_visit/apps.py
-drwxrwxrwx   0        0        0        0 2023-06-01 07:35:08.457508 badi_users-1.0.7/badi_visit/migrations/
--rw-rw-rw-   0        0        0        0 2022-08-14 04:14:27.000000 badi_users-1.0.7/badi_visit/migrations/__init__.py
--rw-rw-rw-   0        0        0     1616 2023-05-02 06:52:22.000000 badi_users-1.0.7/badi_visit/models.py
--rw-rw-rw-   0        0        0       63 2022-08-14 04:14:27.000000 badi_users-1.0.7/badi_visit/tests.py
-drwxrwxrwx   0        0        0        0 2023-06-01 07:35:08.465487 badi_users-1.0.7/badi_wallet/
--rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-1.0.7/badi_wallet/__init__.py
--rw-rw-rw-   0        0        0     8868 2023-06-01 07:03:07.000000 badi_users-1.0.7/badi_wallet/action.py
--rw-rw-rw-   0        0        0      202 2023-03-27 19:00:31.000000 badi_users-1.0.7/badi_wallet/admin.py
-drwxrwxrwx   0        0        0        0 2023-06-01 07:35:08.470474 badi_users-1.0.7/badi_wallet/api/
--rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-1.0.7/badi_wallet/api/__init__.py
--rw-rw-rw-   0        0        0      339 2023-06-01 05:47:13.000000 badi_users-1.0.7/badi_wallet/api/routers.py
--rw-rw-rw-   0        0        0      870 2023-06-01 05:27:59.000000 badi_users-1.0.7/badi_wallet/api/serializers.py
--rw-rw-rw-   0        0        0     8514 2023-06-01 07:21:31.000000 badi_users-1.0.7/badi_wallet/api/view_sets.py
--rw-rw-rw-   0        0        0      243 2023-03-27 19:00:31.000000 badi_users-1.0.7/badi_wallet/apps.py
--rw-rw-rw-   0        0        0      350 2023-03-28 19:16:55.000000 badi_users-1.0.7/badi_wallet/filter.py
-drwxrwxrwx   0        0        0        0 2023-06-01 07:35:08.145346 badi_users-1.0.7/badi_wallet/locale/
-drwxrwxrwx   0        0        0        0 2023-06-01 07:35:08.145346 badi_users-1.0.7/badi_wallet/locale/fa/
-drwxrwxrwx   0        0        0        0 2023-06-01 07:35:08.471470 badi_users-1.0.7/badi_wallet/locale/fa/LC_MESSAGES/
--rw-rw-rw-   0        0        0     2358 2023-06-01 07:32:17.000000 badi_users-1.0.7/badi_wallet/locale/fa/LC_MESSAGES/django.mo
-drwxrwxrwx   0        0        0        0 2023-06-01 07:35:08.472468 badi_users-1.0.7/badi_wallet/migrations/
--rw-rw-rw-   0        0        0        0 2022-08-06 18:28:13.000000 badi_users-1.0.7/badi_wallet/migrations/__init__.py
--rw-rw-rw-   0        0        0     5022 2023-06-01 07:28:42.000000 badi_users-1.0.7/badi_wallet/models.py
-drwxrwxrwx   0        0        0        0 2023-06-01 07:35:08.473465 badi_users-1.0.7/badi_wallet/templates/
--rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-1.0.7/badi_wallet/templates/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 07:35:08.475460 badi_users-1.0.7/badi_wallet/templates/discountcode/
--rw-rw-rw-   0        0        0     2460 2023-06-01 05:46:12.000000 badi_users-1.0.7/badi_wallet/templates/discountcode/discountcode_create.html
--rw-rw-rw-   0        0        0     1620 2023-06-01 05:37:01.000000 badi_users-1.0.7/badi_wallet/templates/discountcode/discountcode_update.html
-drwxrwxrwx   0        0        0        0 2023-06-01 07:35:08.482441 badi_users-1.0.7/badi_wallet/templates/transaction/
--rw-rw-rw-   0        0        0     6145 2023-03-29 08:22:24.000000 badi_users-1.0.7/badi_wallet/templates/transaction/all_transaction_list.html
--rw-rw-rw-   0        0        0    10786 2023-03-30 06:06:20.000000 badi_users-1.0.7/badi_wallet/templates/transaction/all_transaction_report.html
--rw-rw-rw-   0        0        0     2251 2023-03-27 19:00:31.000000 badi_users-1.0.7/badi_wallet/templates/transaction/request-transaction.html
--rw-rw-rw-   0        0        0     6203 2023-03-29 08:22:11.000000 badi_users-1.0.7/badi_wallet/templates/transaction/transaction_list.html
--rw-rw-rw-   0        0        0     3547 2023-03-27 19:00:31.000000 badi_users-1.0.7/badi_wallet/templates/transaction/transaction_result.html
--rw-rw-rw-   0        0        0       63 2023-03-27 19:00:31.000000 badi_users-1.0.7/badi_wallet/tests.py
-drwxrwxrwx   0        0        0        0 2023-06-01 07:35:08.484436 badi_users-1.0.7/badi_wallet/ui/
--rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-1.0.7/badi_wallet/ui/__init__.py
--rw-rw-rw-   0        0        0      731 2023-06-01 05:30:50.000000 badi_users-1.0.7/badi_wallet/ui/urls.py
--rw-rw-rw-   0        0        0     1721 2023-06-01 05:31:16.000000 badi_users-1.0.7/badi_wallet/ui/views.py
--rw-rw-rw-   0        0        0       42 2023-06-01 07:35:08.486431 badi_users-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0      498 2023-06-01 07:34:37.000000 badi_users-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 08:08:20.047567 badi_users-1.0.8/
+-rw-rw-rw-   0        0        0     1093 2022-09-24 06:05:13.000000 badi_users-1.0.8/LICENSE
+-rw-rw-rw-   0        0        0     1066 2022-11-10 17:03:20.000000 badi_users-1.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      419 2023-06-01 08:08:20.046569 badi_users-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      143 2022-10-02 09:04:41.000000 badi_users-1.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 08:08:19.719446 badi_users-1.0.8/badi_ticket/
+-rw-rw-rw-   0        0        0        0 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_ticket/__init__.py
+-rw-rw-rw-   0        0        0      143 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_ticket/admin.py
+-rw-rw-rw-   0        0        0     9892 2023-04-27 05:00:29.000000 badi_users-1.0.8/badi_ticket/api.py
+-rw-rw-rw-   0        0        0      129 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_ticket/apps.py
+drwxrwxrwx   0        0        0        0 2023-06-01 08:08:19.681068 badi_users-1.0.8/badi_ticket/locale/
+drwxrwxrwx   0        0        0        0 2023-06-01 08:08:19.681068 badi_users-1.0.8/badi_ticket/locale/fa/
+drwxrwxrwx   0        0        0        0 2023-06-01 08:08:19.720443 badi_users-1.0.8/badi_ticket/locale/fa/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     2781 2023-06-01 08:07:26.000000 badi_users-1.0.8/badi_ticket/locale/fa/LC_MESSAGES/django.mo
+drwxrwxrwx   0        0        0        0 2023-06-01 08:08:19.721440 badi_users-1.0.8/badi_ticket/migrations/
+-rw-rw-rw-   0        0        0        0 2022-08-06 18:28:13.000000 badi_users-1.0.8/badi_ticket/migrations/__init__.py
+-rw-rw-rw-   0        0        0     4335 2023-05-02 06:51:52.000000 badi_users-1.0.8/badi_ticket/models.py
+-rw-rw-rw-   0        0        0      313 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_ticket/routers.py
+-rw-rw-rw-   0        0        0     2618 2023-05-07 09:45:31.000000 badi_users-1.0.8/badi_ticket/serializers.py
+drwxrwxrwx   0        0        0        0 2023-06-01 08:08:19.682066 badi_users-1.0.8/badi_ticket/static/
+drwxrwxrwx   0        0        0        0 2023-06-01 08:08:19.682066 badi_users-1.0.8/badi_ticket/static/ticket/
+drwxrwxrwx   0        0        0        0 2023-06-01 08:08:19.722437 badi_users-1.0.8/badi_ticket/static/ticket/js/
+-rw-rw-rw-   0        0        0     2448 2023-04-16 09:16:22.000000 badi_users-1.0.8/badi_ticket/static/ticket/js/chat.js
+drwxrwxrwx   0        0        0        0 2023-06-01 08:08:19.723434 badi_users-1.0.8/badi_ticket/templates/
+-rw-rw-rw-   0        0        0        0 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_ticket/templates/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 08:08:19.729418 badi_users-1.0.8/badi_ticket/templates/ticket/
+-rw-rw-rw-   0        0        0     6358 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_ticket/templates/ticket/admin_tickets.html
+-rw-rw-rw-   0        0        0     5265 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_ticket/templates/ticket/message_list.html
+-rw-rw-rw-   0        0        0     9642 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_ticket/templates/ticket/my_tickets.html
+-rw-rw-rw-   0        0        0     7214 2023-04-27 04:28:28.000000 badi_users-1.0.8/badi_ticket/templates/ticket/ticket_create.html
+-rw-rw-rw-   0        0        0     1639 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_ticket/templates/ticket/ticket_update.html
+-rw-rw-rw-   0        0        0       63 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_ticket/tests.py
+-rw-rw-rw-   0        0        0      583 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_ticket/urls.py
+-rw-rw-rw-   0        0        0     2099 2023-04-27 04:25:44.000000 badi_users-1.0.8/badi_ticket/views.py
+drwxrwxrwx   0        0        0        0 2023-06-01 08:08:19.736399 badi_users-1.0.8/badi_user/
+-rw-rw-rw-   0        0        0        0 2023-05-24 05:07:29.000000 badi_users-1.0.8/badi_user/__init__.py
+-rw-rw-rw-   0        0        0      166 2023-05-24 05:07:29.000000 badi_users-1.0.8/badi_user/admin.py
+drwxrwxrwx   0        0        0        0 2023-06-01 08:08:19.740388 badi_users-1.0.8/badi_user/api/
+-rw-rw-rw-   0        0        0        0 2023-05-24 05:07:29.000000 badi_users-1.0.8/badi_user/api/__init__.py
+-rw-rw-rw-   0        0        0    29905 2023-05-24 05:07:29.000000 badi_users-1.0.8/badi_user/api/api.py
+-rw-rw-rw-   0        0        0      485 2023-05-24 05:07:29.000000 badi_users-1.0.8/badi_user/api/routers.py
+-rw-rw-rw-   0        0        0     5939 2023-05-24 05:07:29.000000 badi_users-1.0.8/badi_user/api/serializers.py
+-rw-rw-rw-   0        0        0      183 2023-05-24 05:07:29.000000 badi_users-1.0.8/badi_user/apps.py
+-rw-rw-rw-   0        0        0     3428 2023-05-24 05:07:29.000000 badi_users-1.0.8/badi_user/filter.py
+drwxrwxrwx   0        0        0        0 2023-06-01 08:08:19.690523 badi_users-1.0.8/badi_user/locale/
+drwxrwxrwx   0        0        0        0 2023-06-01 08:08:19.690523 badi_users-1.0.8/badi_user/locale/fa/
+drwxrwxrwx   0        0        0        0 2023-06-01 08:08:19.741387 badi_users-1.0.8/badi_user/locale/fa/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     4344 2023-06-01 08:07:26.000000 badi_users-1.0.8/badi_user/locale/fa/LC_MESSAGES/django.mo
+drwxrwxrwx   0        0        0        0 2023-06-01 08:08:19.742383 badi_users-1.0.8/badi_user/migrations/
+-rw-rw-rw-   0        0        0        0 2022-08-06 18:28:13.000000 badi_users-1.0.8/badi_user/migrations/__init__.py
+-rw-rw-rw-   0        0        0     6895 2023-05-24 05:07:29.000000 badi_users-1.0.8/badi_user/models.py
+drwxrwxrwx   0        0        0        0 2023-06-01 08:08:19.743380 badi_users-1.0.8/badi_user/templates/
+-rw-rw-rw-   0        0        0        0 2023-05-24 05:07:29.000000 badi_users-1.0.8/badi_user/templates/__init__.py
+-rw-rw-rw-   0        0        0       27 2023-05-24 05:07:29.000000 badi_users-1.0.8/badi_user/templates/badi-user-test.html
+drwxrwxrwx   0        0        0        0 2023-06-01 08:08:19.746372 badi_users-1.0.8/badi_user/templates/group/
+-rw-rw-rw-   0        0        0     8558 2023-05-24 05:07:30.000000 badi_users-1.0.8/badi_user/templates/group/group_create.html
+-rw-rw-rw-   0        0        0     5472 2023-05-24 05:07:30.000000 badi_users-1.0.8/badi_user/templates/group/group_update.html
+drwxrwxrwx   0        0        0        0 2023-06-01 08:08:19.747371 badi_users-1.0.8/badi_user/templates/log/
+-rw-rw-rw-   0        0        0     3987 2023-05-24 05:07:30.000000 badi_users-1.0.8/badi_user/templates/log/log_list.html
+drwxrwxrwx   0        0        0        0 2023-06-01 08:08:19.748368 badi_users-1.0.8/badi_user/templates/login-theme/
+-rw-rw-rw-   0        0        0     7336 2023-05-24 05:07:30.000000 badi_users-1.0.8/badi_user/templates/login-theme/login-1.html
+drwxrwxrwx   0        0        0        0 2023-06-01 08:08:19.752356 badi_users-1.0.8/badi_user/templates/member/
+-rw-rw-rw-   0        0        0     6863 2023-05-24 05:07:30.000000 badi_users-1.0.8/badi_user/templates/member/member_create.html
+-rw-rw-rw-   0        0        0    22635 2023-05-24 05:07:30.000000 badi_users-1.0.8/badi_user/templates/member/member_list.html
+-rw-rw-rw-   0        0        0     4783 2023-05-24 05:07:30.000000 badi_users-1.0.8/badi_user/templates/member/member_self_update.html
+-rw-rw-rw-   0        0        0     6525 2023-05-24 05:07:30.000000 badi_users-1.0.8/badi_user/templates/member/member_update.html
+drwxrwxrwx   0        0        0        0 2023-06-01 08:08:19.756345 badi_users-1.0.8/badi_user/templates/user/
+-rw-rw-rw-   0        0        0     5056 2023-05-24 05:07:29.000000 badi_users-1.0.8/badi_user/templates/user/change_password.html
+-rw-rw-rw-   0        0        0     6743 2023-05-24 05:07:29.000000 badi_users-1.0.8/badi_user/templates/user/user_create.html
+-rw-rw-rw-   0        0        0     4019 2023-05-24 05:07:29.000000 badi_users-1.0.8/badi_user/templates/user/user_list.html
+-rw-rw-rw-   0        0        0     5005 2023-05-24 05:07:29.000000 badi_users-1.0.8/badi_user/templates/user/user_update.html
+drwxrwxrwx   0        0        0        0 2023-06-01 08:08:19.758340 badi_users-1.0.8/badi_user/templatetags/
+-rw-rw-rw-   0        0        0        0 2023-05-24 05:07:30.000000 badi_users-1.0.8/badi_user/templatetags/__init__.py
+-rw-rw-rw-   0        0        0     5950 2023-05-24 05:07:30.000000 badi_users-1.0.8/badi_user/templatetags/appfilter.py
+-rw-rw-rw-   0        0        0      500 2023-05-24 05:07:29.000000 badi_users-1.0.8/badi_user/tests.py
+drwxrwxrwx   0        0        0        0 2023-06-01 08:08:19.767316 badi_users-1.0.8/badi_user/ui/
+-rw-rw-rw-   0        0        0        0 2023-05-24 05:07:29.000000 badi_users-1.0.8/badi_user/ui/__init__.py
+-rw-rw-rw-   0        0        0     1484 2023-05-24 05:07:29.000000 badi_users-1.0.8/badi_user/ui/forms.py
+-rw-rw-rw-   0        0        0      320 2023-05-24 05:07:29.000000 badi_users-1.0.8/badi_user/ui/log_views.py
+-rw-rw-rw-   0        0        0     1706 2023-05-24 05:07:29.000000 badi_users-1.0.8/badi_user/ui/member_views.py
+-rw-rw-rw-   0        0        0      672 2023-05-24 05:07:29.000000 badi_users-1.0.8/badi_user/ui/notification_views.py
+-rw-rw-rw-   0        0        0      644 2023-05-24 05:07:29.000000 badi_users-1.0.8/badi_user/ui/roles_views.py
+-rw-rw-rw-   0        0        0     1624 2023-05-24 05:07:29.000000 badi_users-1.0.8/badi_user/ui/urls.py
+-rw-rw-rw-   0        0        0     2633 2023-05-24 05:07:29.000000 badi_users-1.0.8/badi_user/ui/views.py
+drwxrwxrwx   0        0        0        0 2023-06-01 08:08:19.787263 badi_users-1.0.8/badi_users.egg-info/
+-rw-rw-rw-   0        0        0      419 2023-06-01 08:08:19.000000 badi_users-1.0.8/badi_users.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    11239 2023-06-01 08:08:19.000000 badi_users-1.0.8/badi_users.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 08:08:19.000000 badi_users-1.0.8/badi_users.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-06-01 08:08:19.000000 badi_users-1.0.8/badi_users.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-01 08:08:19.805215 badi_users-1.0.8/badi_utils/
+-rw-rw-rw-   0        0        0        0 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/__init__.py
+-rw-rw-rw-   0        0        0     6835 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/date_calc.py
+-rw-rw-rw-   0        0        0    28237 2023-05-10 09:02:15.000000 badi_users-1.0.8/badi_utils/dynamic.py
+-rw-rw-rw-   0        0        0    22478 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/dynamic_api.py
+-rw-rw-rw-   0        0        0     3412 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/dynamic_models.py
+-rw-rw-rw-   0        0        0     2990 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/email.py
+-rw-rw-rw-   0        0        0      252 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/errors.py
+-rw-rw-rw-   0        0        0     1509 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/logging.py
+-rw-rw-rw-   0        0        0      947 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/responses.py
+-rw-rw-rw-   0        0        0      904 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/rss.py
+-rw-rw-rw-   0        0        0     1529 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/select2.py
+-rw-rw-rw-   0        0        0     3714 2023-05-07 04:58:19.000000 badi_users-1.0.8/badi_utils/sms.py
+drwxrwxrwx   0        0        0        0 2023-06-01 08:08:19.696507 badi_users-1.0.8/badi_utils/static/
+drwxrwxrwx   0        0        0        0 2023-06-01 08:08:19.697503 badi_users-1.0.8/badi_utils/static/badi_utils/
+drwxrwxrwx   0        0        0        0 2023-06-01 08:08:19.806212 badi_users-1.0.8/badi_utils/static/badi_utils/css/
+-rw-rw-rw-   0        0        0    40504 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/static/badi_utils/css/custom.css
+drwxrwxrwx   0        0        0        0 2023-06-01 08:08:19.880015 badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/
+-rw-rw-rw-   0        0        0    59778 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).eot
+-rw-rw-rw-   0        0        0    59532 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).ttf
+-rw-rw-rw-   0        0        0    38401 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).woff
+-rw-rw-rw-   0        0        0    31304 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).woff2
+-rw-rw-rw-   0        0        0    59778 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_2.eot
+-rw-rw-rw-   0        0        0    31992 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.eot
+-rw-rw-rw-   0        0        0    57268 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.ttf
+-rw-rw-rw-   0        0        0    36069 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.woff
+-rw-rw-rw-   0        0        0    28856 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.woff2
+-rw-rw-rw-   0        0        0    31992 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold_2.eot
+-rw-rw-rw-   0        0        0    35477 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.eot
+-rw-rw-rw-   0        0        0    60584 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.ttf
+-rw-rw-rw-   0        0        0    39557 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.woff
+-rw-rw-rw-   0        0        0    32344 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.woff2
+-rw-rw-rw-   0        0        0    35477 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light_2.eot
+-rw-rw-rw-   0        0        0    32043 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.eot
+-rw-rw-rw-   0        0        0    58192 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.ttf
+-rw-rw-rw-   0        0        0    36145 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.woff
+-rw-rw-rw-   0        0        0    28912 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.woff2
+-rw-rw-rw-   0        0        0    32043 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium_2.eot
+-rw-rw-rw-   0        0        0    33102 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.eot
+-rw-rw-rw-   0        0        0    56352 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.ttf
+-rw-rw-rw-   0        0        0    36913 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.woff
+-rw-rw-rw-   0        0        0    30072 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.woff2
+-rw-rw-rw-   0        0        0    33102 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight_2.eot
+-rw-rw-rw-   0        0        0    58886 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb.eot
+-rw-rw-rw-   0        0        0    38473 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb.woff
+-rw-rw-rw-   0        0        0    31320 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb.woff2
+-rw-rw-rw-   0        0        0    58886 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_2.eot
+-rw-rw-rw-   0        0        0    57974 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.eot
+-rw-rw-rw-   0        0        0    57760 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.ttf
+-rw-rw-rw-   0        0        0    36629 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.woff
+-rw-rw-rw-   0        0        0    29688 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.woff2
+-rw-rw-rw-   0        0        0    57974 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold_2.eot
+-rw-rw-rw-   0        0        0    57974 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold_3.eot
+-rw-rw-rw-   0        0        0    35458 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.eot
+-rw-rw-rw-   0        0        0    59968 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.ttf
+-rw-rw-rw-   0        0        0    39693 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.woff
+-rw-rw-rw-   0        0        0    32420 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.woff2
+-rw-rw-rw-   0        0        0    35458 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light_2.eot
+-rw-rw-rw-   0        0        0    31983 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.eot
+-rw-rw-rw-   0        0        0    57544 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.ttf
+-rw-rw-rw-   0        0        0    36141 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.woff
+-rw-rw-rw-   0        0        0    28916 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.woff2
+-rw-rw-rw-   0        0        0    31983 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium_2.eot
+-rw-rw-rw-   0        0        0    33044 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.eot
+-rw-rw-rw-   0        0        0    55640 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.ttf
+-rw-rw-rw-   0        0        0    36945 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.woff
+-rw-rw-rw-   0        0        0    29840 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.woff2
+-rw-rw-rw-   0        0        0    33044 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight_2.eot
+-rw-rw-rw-   0        0        0    93376 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/Ray-Black.ttf
+-rw-rw-rw-   0        0        0    94304 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/Ray-Bold.ttf
+-rw-rw-rw-   0        0        0    94740 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/Ray.ttf
+drwxrwxrwx   0        0        0        0 2023-06-01 08:08:19.898964 badi_users-1.0.8/badi_utils/static/badi_utils/js/
+-rw-rw-rw-   0        0        0   478686 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/static/badi_utils/js/apexchart.js
+-rw-rw-rw-   0        0        0    19110 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/static/badi_utils/js/api-login.js
+-rw-rw-rw-   0        0        0    20445 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/static/badi_utils/js/api.js
+-rw-rw-rw-   0        0        0    25944 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/static/badi_utils/js/base.js
+-rw-rw-rw-   0        0        0     2149 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/static/badi_utils/js/chat.js
+-rw-rw-rw-   0        0        0     3167 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/static/badi_utils/js/custom-vue.js
+-rw-rw-rw-   0        0        0    18429 2023-04-16 15:34:42.000000 badi_users-1.0.8/badi_utils/static/badi_utils/js/datatable.js
+-rw-rw-rw-   0        0        0     2470 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/static/badi_utils/js/image-field.js
+-rw-rw-rw-   0        0        0    30541 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/static/badi_utils/js/main.js
+-rw-rw-rw-   0        0        0      959 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/static/badi_utils/js/notification.js
+-rw-rw-rw-   0        0        0     2213 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/static/badi_utils/js/pagination-vue.js
+-rw-rw-rw-   0        0        0    20317 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/static/badi_utils/js/tableexport.js
+-rw-rw-rw-   0        0        0      654 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/static/badi_utils/js/transaction.js
+-rw-rw-rw-   0        0        0   354110 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/static/badi_utils/js/vue.js
+-rw-rw-rw-   0        0        0   268386 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/static/badi_utils/js/xlsx.mini.min.js
+drwxrwxrwx   0        0        0        0 2023-06-01 08:08:19.901958 badi_users-1.0.8/badi_utils/templates/
+-rw-rw-rw-   0        0        0        0 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 08:08:19.927887 badi_users-1.0.8/badi_utils/templates/component/
+-rw-rw-rw-   0        0        0     1777 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/component/createModal.html
+-rw-rw-rw-   0        0        0     1645 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/component/createTitle.html
+-rw-rw-rw-   0        0        0     1054 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/component/filter-form.html
+-rw-rw-rw-   0        0        0      729 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/component/form-errors.html
+-rw-rw-rw-   0        0        0     1340 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/component/form-progressbar-js.html
+-rw-rw-rw-   0        0        0      491 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/component/form-progressbar.html
+-rw-rw-rw-   0        0        0      342 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/component/form.html
+-rw-rw-rw-   0        0        0     1231 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/component/image-field.html
+-rw-rw-rw-   0        0        0    34439 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/component/index-menu.html
+-rw-rw-rw-   0        0        0     2346 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/component/input.html
+-rw-rw-rw-   0        0        0       69 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/component/loader.html
+-rw-rw-rw-   0        0        0      468 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/component/menu-item.html
+-rw-rw-rw-   0        0        0      362 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/component/menu-list.html
+-rw-rw-rw-   0        0        0      746 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/component/messages.html
+-rw-rw-rw-   0        0        0     1134 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/component/pagination-vue.html
+-rw-rw-rw-   0        0        0     2491 2023-05-23 08:24:01.000000 badi_users-1.0.8/badi_utils/templates/component/pagination.html
+-rw-rw-rw-   0        0        0      361 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/component/profile_item.html
+-rw-rw-rw-   0        0        0      204 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/component/space-between.html
+-rw-rw-rw-   0        0        0      430 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/component/svg-button-with-text.html
+-rw-rw-rw-   0        0        0      428 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/component/svg-button.html
+-rw-rw-rw-   0        0        0     1411 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/component/table-item.html
+-rw-rw-rw-   0        0        0     2114 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/component/user-card.html
+-rw-rw-rw-   0        0        0      257 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/component/yesno.html
+drwxrwxrwx   0        0        0        0 2023-06-01 08:08:20.000691 badi_users-1.0.8/badi_utils/templates/svg/
+-rw-rw-rw-   0        0        0     1949 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/svg/Incoming-box.html
+-rw-rw-rw-   0        0        0     1159 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/svg/add-user.html
+-rw-rw-rw-   0        0        0     1092 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/svg/address-book.html
+-rw-rw-rw-   0        0        0     1095 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/svg/arrow-left.html
+-rw-rw-rw-   0        0        0     1081 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/svg/arrow-right.html
+-rw-rw-rw-   0        0        0     2024 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/svg/bitcoin.html
+-rw-rw-rw-   0        0        0      697 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/svg/box.html
+-rw-rw-rw-   0        0        0     1378 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/svg/calendar-day.html
+-rw-rw-rw-   0        0        0     1489 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/svg/calendar-gym.html
+-rw-rw-rw-   0        0        0      925 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/svg/calendar.html
+-rw-rw-rw-   0        0        0     1223 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/svg/call.html
+-rw-rw-rw-   0        0        0     1385 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/svg/category.html
+-rw-rw-rw-   0        0        0     1270 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/svg/chat.html
+-rw-rw-rw-   0        0        0      938 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/svg/check.html
+-rw-rw-rw-   0        0        0      344 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/svg/circle.html
+-rw-rw-rw-   0        0        0     1686 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/svg/city.html
+-rw-rw-rw-   0        0        0     1430 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/svg/clipboard-list.html
+-rw-rw-rw-   0        0        0     2247 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/svg/clock.html
+-rw-rw-rw-   0        0        0      645 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/svg/close.html
+-rw-rw-rw-   0        0        0     2483 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/svg/collection.html
+-rw-rw-rw-   0        0        0     1046 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/svg/comment.html
+-rw-rw-rw-   0        0        0     1103 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/svg/dashboard.html
+-rw-rw-rw-   0        0        0      893 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/svg/delete.html
+-rw-rw-rw-   0        0        0     1521 2023-06-01 05:43:12.000000 badi_users-1.0.8/badi_utils/templates/svg/discount-code.html
+-rw-rw-rw-   0        0        0     1505 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/svg/download.html
+-rw-rw-rw-   0        0        0      901 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/svg/edit.html
+-rw-rw-rw-   0        0        0     1361 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/svg/file-check.html
+-rw-rw-rw-   0        0        0      988 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/svg/file.html
+-rw-rw-rw-   0        0        0     2111 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/svg/film.html
+-rw-rw-rw-   0        0        0      681 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/svg/fire.html
+-rw-rw-rw-   0        0        0     1252 2023-06-01 05:43:38.000000 badi_users-1.0.8/badi_utils/templates/svg/gift.html
+-rw-rw-rw-   0        0        0     1648 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/svg/group-chat.html
+-rw-rw-rw-   0        0        0     1213 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/svg/group.html
+-rw-rw-rw-   0        0        0     1394 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/svg/half_star.html
+-rw-rw-rw-   0        0        0      944 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/svg/home.html
+-rw-rw-rw-   0        0        0     1906 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/svg/hourse.html
+-rw-rw-rw-   0        0        0      631 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/svg/image.html
+-rw-rw-rw-   0        0        0      508 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/svg/info.html
+-rw-rw-rw-   0        0        0     1394 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/svg/interview.html
+-rw-rw-rw-   0        0        0     1389 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/svg/key.html
+-rw-rw-rw-   0        0        0     2472 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/svg/logout.html
+-rw-rw-rw-   0        0        0      940 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/svg/mail.html
+-rw-rw-rw-   0        0        0      731 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/svg/map.html
+-rw-rw-rw-   0        0        0     1601 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/svg/message.html
+-rw-rw-rw-   0        0        0     1607 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/svg/messages.html
+-rw-rw-rw-   0        0        0      683 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/svg/notification.html
+-rw-rw-rw-   0        0        0      708 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/svg/plus.html
+-rw-rw-rw-   0        0        0      753 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/svg/puzzle.html
+-rw-rw-rw-   0        0        0      882 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/svg/question.html
+-rw-rw-rw-   0        0        0     1174 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/svg/refresh.html
+-rw-rw-rw-   0        0        0     1416 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/svg/safe.html
+-rw-rw-rw-   0        0        0     1091 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/svg/search.html
+-rw-rw-rw-   0        0        0     1114 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/svg/shield-protected.html
+-rw-rw-rw-   0        0        0     1219 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/svg/shield-user.html
+-rw-rw-rw-   0        0        0      451 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/svg/slide.html
+-rw-rw-rw-   0        0        0     1587 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/svg/timer.html
+-rw-rw-rw-   0        0        0     1043 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/svg/town.html
+-rw-rw-rw-   0        0        0      804 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/svg/user.html
+-rw-rw-rw-   0        0        0      936 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/svg/wallet.html
+-rw-rw-rw-   0        0        0      933 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/svg/warning.html
+-rw-rw-rw-   0        0        0       19 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templates/test.html
+drwxrwxrwx   0        0        0        0 2023-06-01 08:08:20.002687 badi_users-1.0.8/badi_utils/templatetags/
+-rw-rw-rw-   0        0        0        0 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/templatetags/__init__.py
+-rw-rw-rw-   0        0        0      555 2023-05-23 08:22:50.000000 badi_users-1.0.8/badi_utils/templatetags/badi_utils.py
+-rw-rw-rw-   0        0        0     7102 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/utils.py
+-rw-rw-rw-   0        0        0     1911 2023-04-11 07:22:40.000000 badi_users-1.0.8/badi_utils/validations.py
+drwxrwxrwx   0        0        0        0 2023-06-01 08:08:20.008670 badi_users-1.0.8/badi_visit/
+-rw-rw-rw-   0        0        0        0 2022-08-14 04:14:27.000000 badi_users-1.0.8/badi_visit/__init__.py
+-rw-rw-rw-   0        0        0      167 2022-11-10 16:59:20.000000 badi_users-1.0.8/badi_visit/admin.py
+drwxrwxrwx   0        0        0        0 2023-06-01 08:08:20.011663 badi_users-1.0.8/badi_visit/api/
+-rw-rw-rw-   0        0        0        0 2022-10-24 15:37:24.000000 badi_users-1.0.8/badi_visit/api/__init__.py
+-rw-rw-rw-   0        0        0     2871 2022-11-10 16:59:20.000000 badi_users-1.0.8/badi_visit/api/api.py
+-rw-rw-rw-   0        0        0      208 2022-11-10 16:59:20.000000 badi_users-1.0.8/badi_visit/api/routers.py
+-rw-rw-rw-   0        0        0      185 2022-11-10 16:59:20.000000 badi_users-1.0.8/badi_visit/apps.py
+drwxrwxrwx   0        0        0        0 2023-06-01 08:08:20.013657 badi_users-1.0.8/badi_visit/migrations/
+-rw-rw-rw-   0        0        0        0 2022-08-14 04:14:27.000000 badi_users-1.0.8/badi_visit/migrations/__init__.py
+-rw-rw-rw-   0        0        0     1616 2023-05-02 06:52:22.000000 badi_users-1.0.8/badi_visit/models.py
+-rw-rw-rw-   0        0        0       63 2022-08-14 04:14:27.000000 badi_users-1.0.8/badi_visit/tests.py
+drwxrwxrwx   0        0        0        0 2023-06-01 08:08:20.020639 badi_users-1.0.8/badi_wallet/
+-rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-1.0.8/badi_wallet/__init__.py
+-rw-rw-rw-   0        0        0     8873 2023-06-01 08:03:56.000000 badi_users-1.0.8/badi_wallet/action.py
+-rw-rw-rw-   0        0        0      202 2023-03-27 19:00:31.000000 badi_users-1.0.8/badi_wallet/admin.py
+drwxrwxrwx   0        0        0        0 2023-06-01 08:08:20.025628 badi_users-1.0.8/badi_wallet/api/
+-rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-1.0.8/badi_wallet/api/__init__.py
+-rw-rw-rw-   0        0        0      339 2023-06-01 05:47:13.000000 badi_users-1.0.8/badi_wallet/api/routers.py
+-rw-rw-rw-   0        0        0      870 2023-06-01 05:27:59.000000 badi_users-1.0.8/badi_wallet/api/serializers.py
+-rw-rw-rw-   0        0        0     8514 2023-06-01 07:21:31.000000 badi_users-1.0.8/badi_wallet/api/view_sets.py
+-rw-rw-rw-   0        0        0      243 2023-03-27 19:00:31.000000 badi_users-1.0.8/badi_wallet/apps.py
+-rw-rw-rw-   0        0        0      350 2023-03-28 19:16:55.000000 badi_users-1.0.8/badi_wallet/filter.py
+drwxrwxrwx   0        0        0        0 2023-06-01 08:08:19.701493 badi_users-1.0.8/badi_wallet/locale/
+drwxrwxrwx   0        0        0        0 2023-06-01 08:08:19.702489 badi_users-1.0.8/badi_wallet/locale/fa/
+drwxrwxrwx   0        0        0        0 2023-06-01 08:08:20.026623 badi_users-1.0.8/badi_wallet/locale/fa/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     2361 2023-06-01 08:07:26.000000 badi_users-1.0.8/badi_wallet/locale/fa/LC_MESSAGES/django.mo
+drwxrwxrwx   0        0        0        0 2023-06-01 08:08:20.033604 badi_users-1.0.8/badi_wallet/migrations/
+-rw-rw-rw-   0        0        0     3224 2022-10-11 07:05:24.000000 badi_users-1.0.8/badi_wallet/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      743 2022-11-10 17:00:26.000000 badi_users-1.0.8/badi_wallet/migrations/0002_auto_20221110_2030.py
+-rw-rw-rw-   0        0        0      826 2023-03-29 06:19:38.000000 badi_users-1.0.8/badi_wallet/migrations/0003_auto_20230329_0949.py
+-rw-rw-rw-   0        0        0      429 2023-03-29 09:21:40.000000 badi_users-1.0.8/badi_wallet/migrations/0004_alter_transaction_info.py
+-rw-rw-rw-   0        0        0     1002 2023-04-24 07:01:29.000000 badi_users-1.0.8/badi_wallet/migrations/0005_auto_20230424_1031.py
+-rw-rw-rw-   0        0        0        0 2022-08-06 18:28:13.000000 badi_users-1.0.8/badi_wallet/migrations/__init__.py
+-rw-rw-rw-   0        0        0     5022 2023-06-01 08:05:54.000000 badi_users-1.0.8/badi_wallet/models.py
+drwxrwxrwx   0        0        0        0 2023-06-01 08:08:20.034602 badi_users-1.0.8/badi_wallet/templates/
+-rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-1.0.8/badi_wallet/templates/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 08:08:20.036598 badi_users-1.0.8/badi_wallet/templates/discountcode/
+-rw-rw-rw-   0        0        0     2460 2023-06-01 05:46:12.000000 badi_users-1.0.8/badi_wallet/templates/discountcode/discountcode_create.html
+-rw-rw-rw-   0        0        0     1620 2023-06-01 05:37:01.000000 badi_users-1.0.8/badi_wallet/templates/discountcode/discountcode_update.html
+drwxrwxrwx   0        0        0        0 2023-06-01 08:08:20.042580 badi_users-1.0.8/badi_wallet/templates/transaction/
+-rw-rw-rw-   0        0        0     6145 2023-03-29 08:22:24.000000 badi_users-1.0.8/badi_wallet/templates/transaction/all_transaction_list.html
+-rw-rw-rw-   0        0        0    10786 2023-03-30 06:06:20.000000 badi_users-1.0.8/badi_wallet/templates/transaction/all_transaction_report.html
+-rw-rw-rw-   0        0        0     2251 2023-03-27 19:00:31.000000 badi_users-1.0.8/badi_wallet/templates/transaction/request-transaction.html
+-rw-rw-rw-   0        0        0     6430 2023-06-01 08:06:15.000000 badi_users-1.0.8/badi_wallet/templates/transaction/transaction_list.html
+-rw-rw-rw-   0        0        0     3547 2023-03-27 19:00:31.000000 badi_users-1.0.8/badi_wallet/templates/transaction/transaction_result.html
+-rw-rw-rw-   0        0        0       63 2023-03-27 19:00:31.000000 badi_users-1.0.8/badi_wallet/tests.py
+drwxrwxrwx   0        0        0        0 2023-06-01 08:08:20.045572 badi_users-1.0.8/badi_wallet/ui/
+-rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-1.0.8/badi_wallet/ui/__init__.py
+-rw-rw-rw-   0        0        0      731 2023-06-01 05:30:50.000000 badi_users-1.0.8/badi_wallet/ui/urls.py
+-rw-rw-rw-   0        0        0     1721 2023-06-01 05:31:16.000000 badi_users-1.0.8/badi_wallet/ui/views.py
+-rw-rw-rw-   0        0        0       42 2023-06-01 08:08:20.047567 badi_users-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      498 2023-06-01 08:08:00.000000 badi_users-1.0.8/setup.py
```

### Comparing `badi_users-1.0.7/LICENSE` & `badi_users-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/MANIFEST.in` & `badi_users-1.0.8/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_ticket/api.py` & `badi_users-1.0.8/badi_ticket/api.py`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_ticket/locale/fa/LC_MESSAGES/django.mo` & `badi_users-1.0.8/badi_ticket/locale/fa/LC_MESSAGES/django.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-01 10:58+0330\n"
+"POT-Creation-Date: 2023-06-01 11:36+0330\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
```

### Comparing `badi_users-1.0.7/badi_ticket/models.py` & `badi_users-1.0.8/badi_ticket/models.py`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_ticket/serializers.py` & `badi_users-1.0.8/badi_ticket/serializers.py`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_ticket/static/ticket/js/chat.js` & `badi_users-1.0.8/badi_ticket/static/ticket/js/chat.js`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_ticket/templates/ticket/admin_tickets.html` & `badi_users-1.0.8/badi_ticket/templates/ticket/admin_tickets.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_ticket/templates/ticket/message_list.html` & `badi_users-1.0.8/badi_ticket/templates/ticket/message_list.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_ticket/templates/ticket/my_tickets.html` & `badi_users-1.0.8/badi_ticket/templates/ticket/my_tickets.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_ticket/templates/ticket/ticket_create.html` & `badi_users-1.0.8/badi_ticket/templates/ticket/ticket_create.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_ticket/templates/ticket/ticket_update.html` & `badi_users-1.0.8/badi_ticket/templates/ticket/ticket_update.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_ticket/urls.py` & `badi_users-1.0.8/badi_ticket/urls.py`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_ticket/views.py` & `badi_users-1.0.8/badi_ticket/views.py`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_user/api/api.py` & `badi_users-1.0.8/badi_user/api/api.py`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_user/api/serializers.py` & `badi_users-1.0.8/badi_user/api/serializers.py`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_user/filter.py` & `badi_users-1.0.8/badi_user/filter.py`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_user/locale/fa/LC_MESSAGES/django.mo` & `badi_users-1.0.8/badi_user/locale/fa/LC_MESSAGES/django.mo`

 * *Files 10% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-01 10:58+0330\n"
+"POT-Creation-Date: 2023-06-01 11:36+0330\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
@@ -88,32 +88,26 @@
 
 msgid "Mobile Number"
 msgstr "شماره تماس"
 
 msgid "New Password"
 msgstr "رمز جدید"
 
-msgid "No active user found"
-msgstr "کاربر فعالی یافت نشد"
-
 msgid "Notifications"
 msgstr "اعلانات"
 
 msgid "Optional"
 msgstr "اختیاری"
 
 msgid "Password"
 msgstr "رمز عبور"
 
 msgid "Password changed successfully"
 msgstr "رمز عبور با موفقیت بروزرسانی شد"
 
-msgid "Persian"
-msgstr "فارسی"
-
 msgid "Picture"
 msgstr "تصویر پروفایل"
 
 msgid "Please try again"
 msgstr "لطفا دوباره تلاش کنید"
 
 msgid "Priority"
```

### Comparing `badi_users-1.0.7/badi_user/models.py` & `badi_users-1.0.8/badi_user/models.py`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_user/templates/group/group_create.html` & `badi_users-1.0.8/badi_user/templates/group/group_create.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_user/templates/group/group_update.html` & `badi_users-1.0.8/badi_user/templates/group/group_update.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_user/templates/log/log_list.html` & `badi_users-1.0.8/badi_user/templates/log/log_list.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_user/templates/login-theme/login-1.html` & `badi_users-1.0.8/badi_user/templates/login-theme/login-1.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_user/templates/member/member_create.html` & `badi_users-1.0.8/badi_user/templates/member/member_create.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_user/templates/member/member_list.html` & `badi_users-1.0.8/badi_user/templates/member/member_list.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_user/templates/member/member_self_update.html` & `badi_users-1.0.8/badi_user/templates/member/member_self_update.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_user/templates/member/member_update.html` & `badi_users-1.0.8/badi_user/templates/member/member_update.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_user/templates/user/change_password.html` & `badi_users-1.0.8/badi_user/templates/user/change_password.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_user/templates/user/user_create.html` & `badi_users-1.0.8/badi_user/templates/user/user_create.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_user/templates/user/user_list.html` & `badi_users-1.0.8/badi_user/templates/user/user_list.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_user/templates/user/user_update.html` & `badi_users-1.0.8/badi_user/templates/user/user_update.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_user/templatetags/appfilter.py` & `badi_users-1.0.8/badi_user/templatetags/appfilter.py`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_user/ui/forms.py` & `badi_users-1.0.8/badi_user/ui/forms.py`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_user/ui/member_views.py` & `badi_users-1.0.8/badi_user/ui/member_views.py`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_user/ui/notification_views.py` & `badi_users-1.0.8/badi_user/ui/notification_views.py`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_user/ui/roles_views.py` & `badi_users-1.0.8/badi_user/ui/roles_views.py`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_user/ui/urls.py` & `badi_users-1.0.8/badi_user/ui/urls.py`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_user/ui/views.py` & `badi_users-1.0.8/badi_user/ui/views.py`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_users.egg-info/SOURCES.txt` & `badi_users-1.0.8/badi_users.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -248,14 +248,19 @@
 badi_wallet/models.py
 badi_wallet/tests.py
 badi_wallet/api/__init__.py
 badi_wallet/api/routers.py
 badi_wallet/api/serializers.py
 badi_wallet/api/view_sets.py
 badi_wallet/locale/fa/LC_MESSAGES/django.mo
+badi_wallet/migrations/0001_initial.py
+badi_wallet/migrations/0002_auto_20221110_2030.py
+badi_wallet/migrations/0003_auto_20230329_0949.py
+badi_wallet/migrations/0004_alter_transaction_info.py
+badi_wallet/migrations/0005_auto_20230424_1031.py
 badi_wallet/migrations/__init__.py
 badi_wallet/templates/__init__.py
 badi_wallet/templates/discountcode/discountcode_create.html
 badi_wallet/templates/discountcode/discountcode_update.html
 badi_wallet/templates/transaction/all_transaction_list.html
 badi_wallet/templates/transaction/all_transaction_report.html
 badi_wallet/templates/transaction/request-transaction.html
```

### Comparing `badi_users-1.0.7/badi_utils/date_calc.py` & `badi_users-1.0.8/badi_utils/date_calc.py`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/dynamic.py` & `badi_users-1.0.8/badi_utils/dynamic.py`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/dynamic_api.py` & `badi_users-1.0.8/badi_utils/dynamic_api.py`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/dynamic_models.py` & `badi_users-1.0.8/badi_utils/dynamic_models.py`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/email.py` & `badi_users-1.0.8/badi_utils/email.py`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/logging.py` & `badi_users-1.0.8/badi_utils/logging.py`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/responses.py` & `badi_users-1.0.8/badi_utils/responses.py`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/rss.py` & `badi_users-1.0.8/badi_utils/rss.py`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/select2.py` & `badi_users-1.0.8/badi_utils/select2.py`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/sms.py` & `badi_users-1.0.8/badi_utils/sms.py`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/static/badi_utils/css/custom.css` & `badi_users-1.0.8/badi_utils/static/badi_utils/css/custom.css`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).eot` & `badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).eot`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).ttf` & `badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).ttf`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).woff` & `badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).woff`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).woff2` & `badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).woff2`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_2.eot` & `badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_2.eot`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.eot` & `badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.eot`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.ttf` & `badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.ttf`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.woff` & `badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.woff`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.woff2` & `badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.woff2`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold_2.eot` & `badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold_2.eot`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.eot` & `badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.eot`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.ttf` & `badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.ttf`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.woff` & `badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.woff`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.woff2` & `badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.woff2`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light_2.eot` & `badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light_2.eot`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.eot` & `badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.eot`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.ttf` & `badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.ttf`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.woff` & `badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.woff`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.woff2` & `badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.woff2`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium_2.eot` & `badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium_2.eot`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.eot` & `badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.eot`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.ttf` & `badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.ttf`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.woff` & `badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.woff`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.woff2` & `badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.woff2`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight_2.eot` & `badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight_2.eot`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb.eot` & `badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb.eot`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb.woff` & `badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb.woff`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb.woff2` & `badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb.woff2`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_2.eot` & `badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_2.eot`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.eot` & `badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.eot`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.ttf` & `badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.ttf`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.woff` & `badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.woff`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.woff2` & `badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.woff2`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold_2.eot` & `badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold_2.eot`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold_3.eot` & `badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold_3.eot`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.eot` & `badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.eot`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.ttf` & `badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.ttf`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.woff` & `badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.woff`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.woff2` & `badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.woff2`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light_2.eot` & `badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light_2.eot`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.eot` & `badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.eot`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.ttf` & `badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.ttf`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.woff` & `badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.woff`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.woff2` & `badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.woff2`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium_2.eot` & `badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium_2.eot`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.eot` & `badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.eot`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.ttf` & `badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.ttf`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.woff` & `badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.woff`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.woff2` & `badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.woff2`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight_2.eot` & `badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight_2.eot`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/Ray-Black.ttf` & `badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/Ray-Black.ttf`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/Ray-Bold.ttf` & `badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/Ray-Bold.ttf`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/static/badi_utils/css/fonts/Ray.ttf` & `badi_users-1.0.8/badi_utils/static/badi_utils/css/fonts/Ray.ttf`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/static/badi_utils/js/apexchart.js` & `badi_users-1.0.8/badi_utils/static/badi_utils/js/apexchart.js`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/static/badi_utils/js/api-login.js` & `badi_users-1.0.8/badi_utils/static/badi_utils/js/api-login.js`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/static/badi_utils/js/api.js` & `badi_users-1.0.8/badi_utils/static/badi_utils/js/api.js`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/static/badi_utils/js/base.js` & `badi_users-1.0.8/badi_utils/static/badi_utils/js/base.js`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/static/badi_utils/js/chat.js` & `badi_users-1.0.8/badi_utils/static/badi_utils/js/chat.js`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/static/badi_utils/js/custom-vue.js` & `badi_users-1.0.8/badi_utils/static/badi_utils/js/custom-vue.js`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/static/badi_utils/js/datatable.js` & `badi_users-1.0.8/badi_utils/static/badi_utils/js/datatable.js`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/static/badi_utils/js/image-field.js` & `badi_users-1.0.8/badi_utils/static/badi_utils/js/image-field.js`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/static/badi_utils/js/main.js` & `badi_users-1.0.8/badi_utils/static/badi_utils/js/main.js`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/static/badi_utils/js/notification.js` & `badi_users-1.0.8/badi_utils/static/badi_utils/js/notification.js`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/static/badi_utils/js/pagination-vue.js` & `badi_users-1.0.8/badi_utils/static/badi_utils/js/pagination-vue.js`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/static/badi_utils/js/tableexport.js` & `badi_users-1.0.8/badi_utils/static/badi_utils/js/tableexport.js`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/static/badi_utils/js/transaction.js` & `badi_users-1.0.8/badi_utils/static/badi_utils/js/transaction.js`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/static/badi_utils/js/vue.js` & `badi_users-1.0.8/badi_utils/static/badi_utils/js/vue.js`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/static/badi_utils/js/xlsx.mini.min.js` & `badi_users-1.0.8/badi_utils/static/badi_utils/js/xlsx.mini.min.js`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/templates/component/createModal.html` & `badi_users-1.0.8/badi_utils/templates/component/createModal.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/templates/component/createTitle.html` & `badi_users-1.0.8/badi_utils/templates/component/createTitle.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/templates/component/filter-form.html` & `badi_users-1.0.8/badi_utils/templates/component/filter-form.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/templates/component/form-errors.html` & `badi_users-1.0.8/badi_utils/templates/component/form-errors.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/templates/component/form-progressbar-js.html` & `badi_users-1.0.8/badi_utils/templates/component/form-progressbar-js.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/templates/component/image-field.html` & `badi_users-1.0.8/badi_utils/templates/component/image-field.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/templates/component/index-menu.html` & `badi_users-1.0.8/badi_utils/templates/component/index-menu.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/templates/component/input.html` & `badi_users-1.0.8/badi_utils/templates/component/input.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/templates/component/messages.html` & `badi_users-1.0.8/badi_utils/templates/component/messages.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/templates/component/pagination-vue.html` & `badi_users-1.0.8/badi_utils/templates/component/pagination-vue.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/templates/component/pagination.html` & `badi_users-1.0.8/badi_utils/templates/component/pagination.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/templates/component/table-item.html` & `badi_users-1.0.8/badi_utils/templates/component/table-item.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/templates/component/user-card.html` & `badi_users-1.0.8/badi_utils/templates/component/user-card.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/templates/svg/Incoming-box.html` & `badi_users-1.0.8/badi_utils/templates/svg/Incoming-box.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/templates/svg/add-user.html` & `badi_users-1.0.8/badi_utils/templates/svg/add-user.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/templates/svg/address-book.html` & `badi_users-1.0.8/badi_utils/templates/svg/address-book.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/templates/svg/arrow-left.html` & `badi_users-1.0.8/badi_utils/templates/svg/arrow-left.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/templates/svg/arrow-right.html` & `badi_users-1.0.8/badi_utils/templates/svg/arrow-right.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/templates/svg/bitcoin.html` & `badi_users-1.0.8/badi_utils/templates/svg/bitcoin.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/templates/svg/box.html` & `badi_users-1.0.8/badi_utils/templates/svg/box.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/templates/svg/calendar-day.html` & `badi_users-1.0.8/badi_utils/templates/svg/calendar-day.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/templates/svg/calendar-gym.html` & `badi_users-1.0.8/badi_utils/templates/svg/calendar-gym.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/templates/svg/calendar.html` & `badi_users-1.0.8/badi_utils/templates/svg/calendar.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/templates/svg/call.html` & `badi_users-1.0.8/badi_utils/templates/svg/call.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/templates/svg/category.html` & `badi_users-1.0.8/badi_utils/templates/svg/category.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/templates/svg/chat.html` & `badi_users-1.0.8/badi_utils/templates/svg/chat.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/templates/svg/check.html` & `badi_users-1.0.8/badi_utils/templates/svg/check.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/templates/svg/city.html` & `badi_users-1.0.8/badi_utils/templates/svg/city.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/templates/svg/clipboard-list.html` & `badi_users-1.0.8/badi_utils/templates/svg/clipboard-list.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/templates/svg/clock.html` & `badi_users-1.0.8/badi_utils/templates/svg/clock.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/templates/svg/close.html` & `badi_users-1.0.8/badi_utils/templates/svg/close.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/templates/svg/collection.html` & `badi_users-1.0.8/badi_utils/templates/svg/collection.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/templates/svg/comment.html` & `badi_users-1.0.8/badi_utils/templates/svg/comment.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/templates/svg/dashboard.html` & `badi_users-1.0.8/badi_utils/templates/svg/dashboard.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/templates/svg/delete.html` & `badi_users-1.0.8/badi_utils/templates/svg/delete.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/templates/svg/discount-code.html` & `badi_users-1.0.8/badi_utils/templates/svg/discount-code.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/templates/svg/download.html` & `badi_users-1.0.8/badi_utils/templates/svg/download.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/templates/svg/edit.html` & `badi_users-1.0.8/badi_utils/templates/svg/edit.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/templates/svg/file-check.html` & `badi_users-1.0.8/badi_utils/templates/svg/file-check.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/templates/svg/file.html` & `badi_users-1.0.8/badi_utils/templates/svg/file.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/templates/svg/film.html` & `badi_users-1.0.8/badi_utils/templates/svg/film.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/templates/svg/fire.html` & `badi_users-1.0.8/badi_utils/templates/svg/fire.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/templates/svg/gift.html` & `badi_users-1.0.8/badi_utils/templates/svg/gift.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/templates/svg/group-chat.html` & `badi_users-1.0.8/badi_utils/templates/svg/group-chat.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/templates/svg/group.html` & `badi_users-1.0.8/badi_utils/templates/svg/group.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/templates/svg/half_star.html` & `badi_users-1.0.8/badi_utils/templates/svg/half_star.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/templates/svg/home.html` & `badi_users-1.0.8/badi_utils/templates/svg/home.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/templates/svg/hourse.html` & `badi_users-1.0.8/badi_utils/templates/svg/hourse.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/templates/svg/image.html` & `badi_users-1.0.8/badi_utils/templates/svg/image.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/templates/svg/interview.html` & `badi_users-1.0.8/badi_utils/templates/svg/interview.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/templates/svg/key.html` & `badi_users-1.0.8/badi_utils/templates/svg/key.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/templates/svg/logout.html` & `badi_users-1.0.8/badi_utils/templates/svg/logout.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/templates/svg/mail.html` & `badi_users-1.0.8/badi_utils/templates/svg/mail.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/templates/svg/map.html` & `badi_users-1.0.8/badi_utils/templates/svg/map.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/templates/svg/message.html` & `badi_users-1.0.8/badi_utils/templates/svg/message.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/templates/svg/messages.html` & `badi_users-1.0.8/badi_utils/templates/svg/messages.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/templates/svg/notification.html` & `badi_users-1.0.8/badi_utils/templates/svg/notification.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/templates/svg/plus.html` & `badi_users-1.0.8/badi_utils/templates/svg/plus.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/templates/svg/puzzle.html` & `badi_users-1.0.8/badi_utils/templates/svg/puzzle.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/templates/svg/question.html` & `badi_users-1.0.8/badi_utils/templates/svg/question.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/templates/svg/refresh.html` & `badi_users-1.0.8/badi_utils/templates/svg/refresh.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/templates/svg/safe.html` & `badi_users-1.0.8/badi_utils/templates/svg/safe.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/templates/svg/search.html` & `badi_users-1.0.8/badi_utils/templates/svg/search.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/templates/svg/shield-protected.html` & `badi_users-1.0.8/badi_utils/templates/svg/shield-protected.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/templates/svg/shield-user.html` & `badi_users-1.0.8/badi_utils/templates/svg/shield-user.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/templates/svg/timer.html` & `badi_users-1.0.8/badi_utils/templates/svg/timer.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/templates/svg/town.html` & `badi_users-1.0.8/badi_utils/templates/svg/town.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/templates/svg/user.html` & `badi_users-1.0.8/badi_utils/templates/svg/user.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/templates/svg/wallet.html` & `badi_users-1.0.8/badi_utils/templates/svg/wallet.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/templates/svg/warning.html` & `badi_users-1.0.8/badi_utils/templates/svg/warning.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/templatetags/badi_utils.py` & `badi_users-1.0.8/badi_utils/templatetags/badi_utils.py`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/utils.py` & `badi_users-1.0.8/badi_utils/utils.py`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_utils/validations.py` & `badi_users-1.0.8/badi_utils/validations.py`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_visit/api/api.py` & `badi_users-1.0.8/badi_visit/api/api.py`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_visit/models.py` & `badi_users-1.0.8/badi_visit/models.py`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_wallet/action.py` & `badi_users-1.0.8/badi_wallet/action.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,15 +141,15 @@
                 if t_status == 100:
                     trans.is_verified = True
                     trans.ref_id = req.json()['data']['ref_id']
                     trans.save()
                     if not Transaction.objects.filter(bank_transaction=trans).first():
                         transAction = Transaction(
                             user=trans.user,
-                            amount=trans.amount,
+                            amount=trans.amount / 10,
                             type='+',
                             subject=_("Charge"),
                             bank_transaction=trans,
                         )
                         transAction.save()
                         trans.user.success_transaction(trans, req.json())
                         trans.card_hash = req.json()['data']['card_pan']
```

### Comparing `badi_users-1.0.7/badi_wallet/api/serializers.py` & `badi_users-1.0.8/badi_wallet/api/serializers.py`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_wallet/api/view_sets.py` & `badi_users-1.0.8/badi_wallet/api/view_sets.py`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_wallet/locale/fa/LC_MESSAGES/django.mo` & `badi_users-1.0.8/badi_wallet/locale/fa/LC_MESSAGES/django.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-01 10:58+0330\n"
+"POT-Creation-Date: 2023-06-01 11:36+0330\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
@@ -85,16 +85,16 @@
 
 msgid "Percent"
 msgstr "درصد"
 
 msgid "RefID"
 msgstr "کد رهگیری"
 
-msgid "Return"
-msgstr "بازگشت"
+msgid "Refund"
+msgstr "عودت وجه"
 
 msgid "Time"
 msgstr "زمان"
 
 msgid "Transaction"
 msgstr "تراکنش"
```

### Comparing `badi_users-1.0.7/badi_wallet/models.py` & `badi_users-1.0.8/badi_wallet/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
             ('can_transaction', _("Manage") + ' ' + verbose_name_plural),
         )
 
     TYPES = (
         ('1', _("Buy")),
         ('+', _("Charge")),
         ('m', _("Charge by Management")),
-        ('-', _("Return")),
+        ('-', _("Refund")),
     )
 
     user = models.ForeignKey(User, related_name='transactions', on_delete=models.PROTECT, verbose_name=_("User"))
     amount = models.BigIntegerField(default=0, verbose_name=_("Amount"))
     type = models.CharField(max_length=2, choices=TYPES, verbose_name=_("Type"))
     info = models.TextField(blank=True, verbose_name=_("Info"))
     date_time = models.DateTimeField(auto_now_add=True, blank=True, verbose_name=_("Time"))
```

### Comparing `badi_users-1.0.7/badi_wallet/templates/discountcode/discountcode_create.html` & `badi_users-1.0.8/badi_wallet/templates/discountcode/discountcode_create.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_wallet/templates/discountcode/discountcode_update.html` & `badi_users-1.0.8/badi_wallet/templates/discountcode/discountcode_update.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_wallet/templates/transaction/all_transaction_list.html` & `badi_users-1.0.8/badi_wallet/templates/transaction/all_transaction_list.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_wallet/templates/transaction/all_transaction_report.html` & `badi_users-1.0.8/badi_wallet/templates/transaction/all_transaction_report.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_wallet/templates/transaction/request-transaction.html` & `badi_users-1.0.8/badi_wallet/templates/transaction/request-transaction.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_wallet/templates/transaction/transaction_list.html` & `badi_users-1.0.8/badi_wallet/templates/transaction/transaction_list.html`

 * *Files 2% similar despite different names*

```diff
@@ -146,15 +146,21 @@
         const table = datatable_simple_show({
             api_url: '{{ api_url }}',
             real_cols: {{cols|length}},
             datable_id: '#table',
         }, {
             rowCallback: function (row, data) {
                 defaultDrawCallBack(row, data);
-                boldCol(0, row, formatNumber(data[1]) + ' ' + badiConfig["price_text"] + ' ', data[2] === 'شارژ' ? 'primary' : 'danger')
+                const colors = {
+                    'شارژ': 'success',
+                    'خرید': 'danger',
+                    'عودت وجه': 'warning',
+                    'شارژ توسط مدیریت': 'primary',
+                }
+                boldCol(0, row, formatNumber(data[1]) + ' ' + badiConfig["price_text"] + ' ', colors[data[2]])
                 $(`td:last`, row).html(`
 <button type="button" onclick="showTransactionDetail(${data[0]})" data-skin="dark" data-toggle="tooltip" data-placement="top" title="" data-original-title="edit" class="btn btn-sm btn-light-primary btn-hover-text-primary btn-icon mx-2"><span class="svg-icon svg-icon-md">{% include 'svg/info.html' %}</span></button>
 				`)
             }
         });
 	</script>
 {% endblock %}
```

### Comparing `badi_users-1.0.7/badi_wallet/templates/transaction/transaction_result.html` & `badi_users-1.0.8/badi_wallet/templates/transaction/transaction_result.html`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_wallet/ui/urls.py` & `badi_users-1.0.8/badi_wallet/ui/urls.py`

 * *Files identical despite different names*

### Comparing `badi_users-1.0.7/badi_wallet/ui/views.py` & `badi_users-1.0.8/badi_wallet/ui/views.py`

 * *Files identical despite different names*

