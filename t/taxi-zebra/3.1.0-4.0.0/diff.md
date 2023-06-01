# Comparing `tmp/taxi_zebra-3.1.0.tar.gz` & `tmp/taxi_zebra-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taxi_zebra-3.1.0.tar", last modified: Mon May 15 10:21:56 2023, max compression
+gzip compressed data, was "taxi_zebra-4.0.0.tar", last modified: Thu Jun  1 15:02:18 2023, max compression
```

## Comparing `taxi_zebra-3.1.0.tar` & `taxi_zebra-4.0.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:21:56.754171 taxi_zebra-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-15 10:21:37.000000 taxi_zebra-3.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-15 10:21:56.754171 taxi_zebra-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-15 10:21:37.000000 taxi_zebra-3.1.0/README.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)      252 2023-05-15 10:21:56.758171 taxi_zebra-3.1.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      950 2023-05-15 10:21:37.000000 taxi_zebra-3.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:21:56.754171 taxi_zebra-3.1.0/taxi_zebra/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-15 10:21:37.000000 taxi_zebra-3.1.0/taxi_zebra/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10302 2023-05-15 10:21:37.000000 taxi_zebra-3.1.0/taxi_zebra/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-05-15 10:21:37.000000 taxi_zebra-3.1.0/taxi_zebra/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-15 10:21:37.000000 taxi_zebra-3.1.0/taxi_zebra/roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-05-15 10:21:37.000000 taxi_zebra-3.1.0/taxi_zebra/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-15 10:21:37.000000 taxi_zebra-3.1.0/taxi_zebra/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:21:56.754171 taxi_zebra-3.1.0/taxi_zebra.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-15 10:21:56.000000 taxi_zebra-3.1.0/taxi_zebra.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-15 10:21:56.000000 taxi_zebra-3.1.0/taxi_zebra.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 10:21:56.000000 taxi_zebra-3.1.0/taxi_zebra.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-15 10:21:56.000000 taxi_zebra-3.1.0/taxi_zebra.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-15 10:21:56.000000 taxi_zebra-3.1.0/taxi_zebra.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-15 10:21:56.000000 taxi_zebra-3.1.0/taxi_zebra.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:21:56.754171 taxi_zebra-3.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9092 2023-05-15 10:21:37.000000 taxi_zebra-3.1.0/tests/test_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:02:18.967056 taxi_zebra-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-01 15:01:52.000000 taxi_zebra-4.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-01 15:02:18.967056 taxi_zebra-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-06-01 15:01:52.000000 taxi_zebra-4.0.0/README.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      252 2023-06-01 15:02:18.967056 taxi_zebra-4.0.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      937 2023-06-01 15:01:52.000000 taxi_zebra-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:02:18.967056 taxi_zebra-4.0.0/taxi_zebra/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-01 15:01:52.000000 taxi_zebra-4.0.0/taxi_zebra/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10303 2023-06-01 15:01:52.000000 taxi_zebra-4.0.0/taxi_zebra/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-06-01 15:01:52.000000 taxi_zebra-4.0.0/taxi_zebra/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-01 15:01:52.000000 taxi_zebra-4.0.0/taxi_zebra/roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-06-01 15:01:52.000000 taxi_zebra-4.0.0/taxi_zebra/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-01 15:01:52.000000 taxi_zebra-4.0.0/taxi_zebra/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:02:18.967056 taxi_zebra-4.0.0/taxi_zebra.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-01 15:02:18.000000 taxi_zebra-4.0.0/taxi_zebra.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-01 15:02:18.000000 taxi_zebra-4.0.0/taxi_zebra.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 15:02:18.000000 taxi_zebra-4.0.0/taxi_zebra.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-01 15:02:18.000000 taxi_zebra-4.0.0/taxi_zebra.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-01 15:02:18.000000 taxi_zebra-4.0.0/taxi_zebra.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-01 15:02:18.000000 taxi_zebra-4.0.0/taxi_zebra.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:02:18.967056 taxi_zebra-4.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9176 2023-06-01 15:01:52.000000 taxi_zebra-4.0.0/tests/test_backend.py
```

### Comparing `taxi_zebra-3.1.0/README.rst` & `taxi_zebra-4.0.0/README.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,25 @@
 Zebra backend for Taxi
 ======================
 
-This is the Zebra backend for `Taxi <https://github.com/sephii/taxi>`_. It
+This is the Zebra backend for `Taxi <https://github.com/liip/taxi>`_. It
 exposes the ``zebra`` protocol to push entries and fetch projects and
 activities from Zebra.
 
 Installation
 ------------
 
     taxi plugin install zebra
 
 Usage
 -----
 
 In your ``.taxirc`` file, use the ``zebra`` protocol for your backend. For example,
-if your Zebra instance is hosted at https://zebra.example.com/ you'll use the
-following configuration::
-
-    [backends]
-    my_zebra_backend = zebra://username:password@zebra.example.com
-
-If you want to use a token-based authentication, start by generating a token in
-your Zebra profile, then use the token as your username, without any password::
+if your Zebra instance is hosted at https://zebra.example.com/, after generating a
+token in your Zebra profile, you'll use the following configuration::
 
     [backends]
     my_zebra_backend = zebra://token@zebra.example.com
 
 Contributing
 ------------
```

### Comparing `taxi_zebra-3.1.0/taxi_zebra/backend.py` & `taxi_zebra-4.0.0/taxi_zebra/backend.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,302 +1,314 @@
 import json
 import logging
 from collections import namedtuple
 from datetime import datetime
 from functools import wraps
+from urllib import parse
 
 import click
 import requests
-from urllib import parse
+
 from taxi import __version__ as taxi_version
 from taxi.aliases import aliases_database
 from taxi.backends import BaseBackend, PushEntryFailed
 from taxi.exceptions import TaxiException
 from taxi.projects import Activity, Project
 
 from .roles import INDIVIDUAL_ACTION_ID, NEVER_SAVE_ROLE_ID
-from .ui import prompt_role, format_response_messages
+from .ui import format_response_messages, prompt_role
 from .utils import get_role_id_from_alias, to_zebra_params
 
-
 logger = logging.getLogger(__name__)
 
 
-Role = namedtuple('Role', ['id', 'parent_id', 'full_name'])
+Role = namedtuple("Role", ["id", "parent_id", "full_name"])
 
 
 def get_alias_id(alias):
     return aliases_database[alias].mapping[1]
 
 
 def needs_authentication(f):
     @wraps(f)
     def wrapper(*args, **kwargs):
-        args[0].authenticate()
+        args[0].authorize_session()
         return f(*args, **kwargs)
 
     return wrapper
 
 
 class ZebraBackend(BaseBackend):
     def __init__(self, *args, **kwargs):
         super(ZebraBackend, self).__init__(*args, **kwargs)
 
+        if self.password:
+            raise TaxiException(
+                "Password was passed to ZebraBackend, only token is supported."
+            )
+        # To clarify the later code; unset username/password, set token.
+        self.token = self.username
+        del self.password
+        del self.username
+
         self.port = self.port if self.port else 443
 
-        if not self.path.startswith('/'):
-            self.path = '/' + self.path
+        if not self.path.startswith("/"):
+            self.path = "/" + self.path
 
-        if not self.path.endswith('/'):
-            self.path += '/'
+        if not self.path.endswith("/"):
+            self.path += "/"
 
-        self._authenticated = False
         self._session = requests.Session()
-        self._session.headers.update(
-            {'user-agent': 'Taxi {}'.format(taxi_version)}
-        )
+        self._session.headers.update({"user-agent": "Taxi {}".format(taxi_version)})
         self._user_info = None
 
     def get_api_url(self, url):
-        absolute_url = self.get_full_url('/api/v2{url}'.format(url=url))
-
-        if not self.password:
-            absolute_url = self.append_token(absolute_url)
-
-        return absolute_url
+        return self.get_full_url("/api/v2{url}".format(url=url))
 
     def get_full_url(self, url):
         # Remove slash at the start of the string since self.path already ends
         # with a slash
-        url = url.lstrip('/')
+        url = url.lstrip("/")
 
-        return 'https://{host}:{port}{base_path}{url}'.format(
+        return "https://{host}:{port}{base_path}{url}".format(
             host=self.hostname, port=self.port, base_path=self.path, url=url
         )
 
     def zebra_request(self, method, url, **kwargs):
         response = self._session.request(method=method, url=url, **kwargs)
 
         if response.status_code in {401, 403}:
             raise TaxiException("Login failed, please check your credentials")
 
         return response
 
-    def append_token(self, url):
-        split_url = list(parse.urlsplit(url))
-
-        # Add the token parameter to the query string, then rebuild the URL
-        qs = parse.parse_qs(split_url[3])
-        qs['token'] = self.username
-        split_url[3] = parse.urlencode(qs, doseq=True)
-        url_with_token = parse.urlunsplit(split_url)
-
-        return url_with_token
-
-    def authenticate(self):
-        if self._authenticated or not self.password:
-            return
-
-        login_url = self.get_full_url('/login/user/%s.json' % self.username)
-        parameters_dict = {
-            'username': self.username,
-            'password': self.password,
-        }
-
-        try:
-            self.zebra_request('post', login_url, data=parameters_dict).json()
-        except ValueError:
-            raise TaxiException("Login failed, please check your credentials")
-
-        self._authenticated = True
+    def authorize_session(self):
+        """
+        Authenticate via Bearer token authorization
+
+        Starting with Zebra 14.97, that's possible for clients, and will be effective in 2023/10
+        """
+        self._session.headers.update({"Authorization": "Bearer {}".format(self.token)})
 
     @needs_authentication
     def _push_entry(self, date, entry, role_id, *args, **kwargs):
-        post_url = self.get_api_url('/timesheets/')
+        post_url = self.get_api_url("/timesheets/")
 
         mapping = aliases_database[entry.alias]
         if role_id == INDIVIDUAL_ACTION_ID:
-            kwargs['individual_action'] = True
+            kwargs["individual_action"] = True
         elif role_id:
-            kwargs['individual_action'] = False
-            kwargs['role_id'] = role_id
+            kwargs["individual_action"] = False
+            kwargs["role_id"] = role_id
 
-        parameters = dict({
-            'time': entry.hours,
-            'project_id': mapping.mapping[0],
-            'activity_id': mapping.mapping[1],
-            'date': date.strftime('%Y-%m-%d'),
-            'description': entry.description,
-        }, **kwargs)
+        parameters = dict(
+            {
+                "time": entry.hours,
+                "project_id": mapping.mapping[0],
+                "activity_id": mapping.mapping[1],
+                "date": date.strftime("%Y-%m-%d"),
+                "description": entry.description,
+            },
+            **kwargs
+        )
 
-        return self.zebra_request('post', post_url, data=to_zebra_params(parameters))
+        return self.zebra_request("post", post_url, data=to_zebra_params(parameters))
 
     @needs_authentication
     def push_entry(self, date, entry):
         user_roles = self.get_user_roles()
         alias_role_id = get_role_id_from_alias(entry.alias)
 
         if alias_role_id == NEVER_SAVE_ROLE_ID:
             alias_role_id = None
 
         response = self._push_entry(date, entry, role_id=alias_role_id)
         response_json = response.json()
 
         if not response:
-            error_code = response_json.get('errorCode')
-            if error_code in {'role_needed', 'role_invalid'}:
-                if error_code == 'role_needed':
+            error_code = response_json.get("errorCode")
+            if error_code in {"role_needed", "role_invalid"}:
+                if error_code == "role_needed":
                     prompt = "You're trying to push the following entry to an activity which doesn't have any associated role:"
-                elif error_code == 'role_invalid':
+                elif error_code == "role_invalid":
                     prompt = "You're trying to use a role you don't have (anymore):"
                 else:
                     prompt = "You can't use that role:"
 
-                click.secho("\n{}\n\n{}\n".format(
-                    prompt, self.context['view'].get_entry_status(entry)
-                ), fg='yellow')
+                click.secho(
+                    "\n{}\n\n{}\n".format(
+                        prompt, self.context["view"].get_entry_status(entry)
+                    ),
+                    fg="yellow",
+                )
 
                 default_role_id = self.get_latest_role_for_alias(entry.alias)
-                default_role = user_roles.get(default_role_id) if default_role_id else None
-                selected_role = prompt_role(entry, list(user_roles.values()), self.context, default_role=default_role)
-                selected_role_id = selected_role.id if selected_role else INDIVIDUAL_ACTION_ID
+                default_role = (
+                    user_roles.get(default_role_id) if default_role_id else None
+                )
+                selected_role = prompt_role(
+                    entry,
+                    list(user_roles.values()),
+                    self.context,
+                    default_role=default_role,
+                )
+                selected_role_id = (
+                    selected_role.id if selected_role else INDIVIDUAL_ACTION_ID
+                )
 
                 response = self._push_entry(date, entry, role_id=selected_role_id)
                 response_json = response.json()
         else:
             selected_role = user_roles.get(alias_role_id)
 
-        if not response_json['success']:
-            error = response_json.get('error', "Unknown error")
+        if not response_json["success"]:
+            error = response_json.get("error", "Unknown error")
             raise PushEntryFailed(error)
 
         if selected_role:
             self.update_latest_role_for_alias(entry.alias, selected_role.id)
 
-        additional_info = "individual action" if not selected_role else "as {}".format(selected_role.full_name)
+        additional_info = (
+            "individual action"
+            if not selected_role
+            else "as {}".format(selected_role.full_name)
+        )
         messages = format_response_messages(response_json)
 
         return ". ".join([additional_info] + messages)
 
     @needs_authentication
     def get_projects(self):
-        projects_url = self.get_api_url('/projects/')
+        projects_url = self.get_api_url("/projects/")
 
         try:
-            response = self.zebra_request('get', projects_url)
+            response = self.zebra_request("get", projects_url)
             projects = response.json()
         except ValueError:
             raise TaxiException(
                 "Unexpected response from the server (%s).  Check your "
                 "credentials" % response.content
             )
         projects_list = []
-        date_attrs = ('start_date', 'end_date')
+        date_attrs = ("start_date", "end_date")
 
-        for project in projects['data']['list'].values():
-            team = str(project['circle_id']) if project['circle_id'] else None
-            p = Project(project['id'], project['name'],
-                        Project.STATUS_ACTIVE, project['description'],
-                        project['budget'], team=team)
+        for project in projects["data"]["list"].values():
+            team = str(project["circle_id"]) if project["circle_id"] else None
+            p = Project(
+                project["id"],
+                project["name"],
+                Project.STATUS_ACTIVE,
+                project["description"],
+                project["budget"],
+                team=team,
+            )
 
             for date_attr in date_attrs:
                 try:
-                    date = datetime.strptime(project[date_attr],
-                                             '%Y-%m-%d').date()
+                    date = datetime.strptime(project[date_attr], "%Y-%m-%d").date()
                 except (ValueError, TypeError):
                     date = None
 
                 setattr(p, date_attr, date)
 
-            for activity in project['activities']:
-                a = Activity(activity['id'], activity['name'], activity['is_active'])
+            for activity in project["activities"]:
+                a = Activity(activity["id"], activity["name"], activity["is_active"])
                 p.add_activity(a)
 
-                if activity['alias']:
-                    p.aliases[activity['alias']] = activity['id']
+                if activity["alias"]:
+                    p.aliases[activity["alias"]] = activity["id"]
 
             projects_list.append(p)
 
         return projects_list
 
     @needs_authentication
     def get_user_info(self):
-        if getattr(self, '_user_info', None) is None:
-            user_info_url = self.get_api_url('/users/me')
-            data = self.zebra_request('get', user_info_url).json()['data']
+        if getattr(self, "_user_info", None) is None:
+            user_info_url = self.get_api_url("/users/me")
+            data = self.zebra_request("get", user_info_url).json()["data"]
 
             self._user_info = data
 
         return self._user_info
 
     def get_user_roles(self):
         def zebra_role_to_role(id_, role):
             if isinstance(role, dict):
                 return Role(
                     id=str(id_),
-                    parent_id=str(role['parent_id']) if role['parent_id'] else None,
-                    full_name=role['full_name']
+                    parent_id=str(role["parent_id"]) if role["parent_id"] else None,
+                    full_name=role["full_name"],
                 )
             else:
                 return Role(id=str(id_), parent_id=None, full_name=role)
 
         user_info = self.get_user_info()
         roles = {
             str(id_): zebra_role_to_role(id_, role)
-            for id_, role in user_info.get('roles', {}).items()
+            for id_, role in user_info.get("roles", {}).items()
         }
 
         return roles
 
     @needs_authentication
     def get_timesheets(self, start_date, end_date=None):
         if not end_date:
             end_date = datetime.date.today()
 
-        timesheet_url = self.get_api_url('/timesheets')
+        timesheet_url = self.get_api_url("/timesheets")
         request_params = {
-            'start_date': start_date,
-            'end_date': end_date,
+            "start_date": start_date,
+            "end_date": end_date,
         }
 
-        return self.zebra_request('get', timesheet_url, params=request_params).json()['data']['list']
+        return self.zebra_request("get", timesheet_url, params=request_params).json()[
+            "data"
+        ]["list"]
 
     def get_latest_role_for_alias(self, alias):
         try:
             alias_id = get_alias_id(alias)
         except KeyError:
             return None
 
         return self.get_activities_roles().get(alias_id)
 
     def get_activities_roles(self):
-        if getattr(self, '_activities_roles', None) is not None:
+        if getattr(self, "_activities_roles", None) is not None:
             return self._activities_roles
 
-        response = self.zebra_request('get', self.get_api_url('/latestActivityRoles'))
+        response = self.zebra_request("get", self.get_api_url("/latestActivityRoles"))
         if not response:
-            logger.warning("Could not fetch latest activity roles, got response %s", response)
+            logger.warning(
+                "Could not fetch latest activity roles, got response %s", response
+            )
             return {}
 
         try:
-            activities_roles = response.json()['data']
+            activities_roles = response.json()["data"]
         except json.JsonDecodeError as e:
-            logger.warning("Could not decode latestActivityRoles JSON response, got %s", e)
+            logger.warning(
+                "Could not decode latestActivityRoles JSON response, got %s", e
+            )
             return {}
         except KeyError:
             logger.warning("No 'data' in latestActivityRole endpoint response")
             return {}
 
-        self._activities_roles = {str(key): str(value) for key, value in activities_roles.items()}
+        self._activities_roles = {
+            str(key): str(value) for key, value in activities_roles.items()
+        }
 
         return self._activities_roles
 
     def update_latest_role_for_alias(self, alias, role_id):
         try:
             alias_id = get_alias_id(alias)
         except KeyError:
             return
 
-        if not hasattr(self, '_activities_roles'):
+        if not hasattr(self, "_activities_roles"):
             self._activities_roles = {}
 
         self._activities_roles[str(alias_id)] = str(role_id)
```

### Comparing `taxi_zebra-3.1.0/taxi_zebra/commands.py` & `taxi_zebra-4.0.0/taxi_zebra/commands.py`

 * *Files 19% similar despite different names*

```diff
@@ -26,16 +26,16 @@
     pass
 
 
 def signed_number(number, precision=2):
     """
     Return the given number as a string with a sign in front of it, ie. `+` if the number is positive, `-` otherwise.
     """
-    prefix = '' if number <= 0 else '+'
-    number_str = '{}{:.{precision}f}'.format(prefix, number, precision=precision)
+    prefix = "" if number <= 0 else "+"
+    number_str = "{}{:.{precision}f}".format(prefix, number, precision=precision)
 
     return number_str
 
 
 def get_first_dow(date):
     """
     Return the first day of the week for the given date.
@@ -57,29 +57,43 @@
     Show Zebra balance.
 
     Like the hours balance, vacation left, etc.
     """
     backend = plugins_registry.get_backends_by_class(ZebraBackend)[0]
 
     timesheet_collection = get_timesheet_collection_for_context(ctx, None)
-    hours_to_be_pushed = timesheet_collection.get_hours(pushed=False, ignored=False, unmapped=False)
+    hours_to_be_pushed = timesheet_collection.get_hours(
+        pushed=False, ignored=False, unmapped=False
+    )
 
     today = datetime.date.today()
 
     user_info = backend.get_user_info()
     timesheets_week = backend.get_timesheets(get_first_dow(today), get_last_dow(today))
     timesheets_today = backend.get_timesheets(today, today)
-    total_duration_week = sum([float(timesheet['time']) for timesheet in timesheets_week])
-    total_duration_today = sum([float(timesheet['time']) for timesheet in timesheets_today])
+    total_duration_week = sum(
+        [float(timesheet["time"]) for timesheet in timesheets_week]
+    )
+    total_duration_today = sum(
+        [float(timesheet["time"]) for timesheet in timesheets_today]
+    )
+
+    vacation_info = user_info["vacation"]
+    vacation = hours_to_days(
+        vacation_info["total_available"]
+        - vacation_info["planned"]
+        - vacation_info["used"]
+    )
+    vacation_balance = "{} days, {:.2f} hours".format(*vacation)
 
-    vacation_info = user_info['vacation']
-    vacation = hours_to_days(vacation_info['total_available'] - vacation_info['planned'] - vacation_info['used'])
-    vacation_balance = '{} days, {:.2f} hours'.format(*vacation)
-
-    hours_balance = user_info['hours']['hours']['balance']
+    hours_balance = user_info["hours"]["hours"]["balance"]
 
     click.echo("Hours balance: {}".format(signed_number(hours_balance)))
-    click.echo("Hours balance after push: {}".format(signed_number(hours_balance + hours_to_be_pushed)))
+    click.echo(
+        "Hours balance after push: {}".format(
+            signed_number(hours_balance + hours_to_be_pushed)
+        )
+    )
     click.echo("Hours done this week: {:.2f}".format(total_duration_week))
     click.echo("Hours done today: {:.2f}".format(total_duration_today))
     click.echo("Hours to be pushed: {:.2f}".format(hours_to_be_pushed))
     click.echo("Vacation left: {}".format(vacation_balance))
```

### Comparing `taxi_zebra-3.1.0/taxi_zebra/ui.py` & `taxi_zebra-4.0.0/taxi_zebra/ui.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,115 +10,132 @@
 from .utils import get_role_id_from_alias, update_alias_mapping
 
 
 class CancelInput(Exception):
     pass
 
 
-Option = namedtuple('Option', ['value', 'label', 'key', 'style'])
+Option = namedtuple("Option", ["value", "label", "key", "style"])
 Option.__new__.__defaults__ = (None, {})
 
 
 def format_response_messages(response_json):
     """
     Show all messages in the `messages` key of the given dict.
     """
     message_type_kwargs = {
-        'warning': {'fg': 'yellow'},
-        'error': {'fg': 'red'},
+        "warning": {"fg": "yellow"},
+        "error": {"fg": "red"},
     }
 
     return [
-        click.style(
-            message['text'], **message_type_kwargs.get(message['type'], {})
-        )
-        for message in response_json.get('messages', [])
+        click.style(message["text"], **message_type_kwargs.get(message["type"], {}))
+        for message in response_json.get("messages", [])
     ]
 
 
 def prompt_options(message, options, default=None):
     def get_option_key(pos, option):
         return option.key if option.key is not None else pos
 
     enumerated_options = list(enumerate(options))
-    options_by_key = [(get_option_key(i, option), option) for i, option in enumerated_options]
+    options_by_key = [
+        (get_option_key(i, option), option) for i, option in enumerated_options
+    ]
     options_by_key_dict = dict(options_by_key)
     try:
-        default_option_id = next(
-            key for key, option in options_by_key if option.value == default.value
-        ) if default else None
+        default_option_id = (
+            next(key for key, option in options_by_key if option.value == default.value)
+            if default
+            else None
+        )
     except StopIteration:
         default_option_id = None
 
     click.secho(message + "\n", bold=True)
 
     for option_key, option in options_by_key:
         if option.value is not None:
             click.echo(
-                click.style("[{}]".format(option_key), fg='yellow',
-                            **option.style)
+                click.style("[{}]".format(option_key), fg="yellow", **option.style)
                 + " "
                 + click.style(option.label, **option.style)
             )
         else:
             click.echo(option.label)
 
     click.echo()
-    prompt_message_default = " (leave empty for {})".format(click.style(default.label, bold=True)) if default else ""
+    prompt_message_default = (
+        " (leave empty for {})".format(click.style(default.label, bold=True))
+        if default
+        else ""
+    )
     prompt_message = "Select a role{}".format(prompt_message_default)
 
     while True:
-        option_id = click.prompt(
-            prompt_message,
-            default=str(default_option_id) if default_option_id is not None else None,
-            show_default=False
-        ).lstrip('[').rstrip(']')
+        option_id = (
+            click.prompt(
+                prompt_message,
+                default=str(default_option_id)
+                if default_option_id is not None
+                else None,
+                show_default=False,
+            )
+            .lstrip("[")
+            .rstrip("]")
+        )
 
         try:
             option_id = int(option_id)
         except ValueError:
             pass
 
         try:
             return options_by_key_dict[option_id][0]
         except KeyError:
-            click.secho("`{}` is not a a valid option. Please try again.".format(option_id), fg='red')
+            click.secho(
+                "`{}` is not a a valid option. Please try again.".format(option_id),
+                fg="red",
+            )
 
     return option_id
 
 
 def input_role(roles, project_team, default_role=None):
     """
     Show a list of roles to the user and ask them to select one. Return the
     selected `Role`, or `None` if individual action was chosen.
     """
+
     def role_to_option(role):
         highlight = role.parent_id and role.parent_id == project_team
 
         return Option(
-            value=role, label=role.full_name, style={'bold': True} if highlight else {}
+            value=role, label=role.full_name, style={"bold": True} if highlight else {}
         )
 
-    individual_action = 'i'
-    cancel = 'c'
+    individual_action = "i"
+    cancel = "c"
     sorted_roles = sorted(roles, key=lambda role: role.full_name)
 
-    options = [
-        role_to_option(role) for role in sorted_roles
-    ] + [
-        Option(value=None, label='-----'),
-        Option(value=individual_action, label="Individual action", key=individual_action),
+    options = [role_to_option(role) for role in sorted_roles] + [
+        Option(value=None, label="-----"),
+        Option(
+            value=individual_action, label="Individual action", key=individual_action
+        ),
         Option(value=cancel, label="Cancel, skip this entry for now", key=cancel),
     ]
 
     default_option = role_to_option(default_role) if default_role else None
 
     try:
         selected_role = prompt_options(
-            message='In which role do you want to push this entry?', options=options, default=default_option
+            message="In which role do you want to push this entry?",
+            options=options,
+            default=default_option,
         )
     except click.exceptions.Abort:
         selected_role = cancel
 
     if selected_role == cancel:
         click.echo()
         raise CancelInput()
@@ -130,55 +147,65 @@
 
 def prompt_role(entry, roles, context, default_role=None):
     """
     Ask the user to choose a role in `roles` for the given `entry` and return
     it.
     """
     mapping = aliases_database[entry.alias]
-    project = context['projects_db'].get(mapping.mapping[0], mapping.backend)
+    project = context["projects_db"].get(mapping.mapping[0], mapping.backend)
     project_team = project.team if project else None
 
     try:
         role = input_role(roles, project_team, default_role=default_role)
     except CancelInput:
         raise PushEntryFailed("Skipped")
 
     # Do not ask to save role association if user has requested to never be asked for it
     if role and get_role_id_from_alias(entry.alias) != NEVER_SAVE_ROLE_ID:
-        click.echo("You have selected the role {}".format(click.style(role.full_name, fg='yellow')))
+        click.echo(
+            "You have selected the role {}".format(
+                click.style(role.full_name, fg="yellow")
+            )
+        )
         prompt_kwargs = {
-            'prompt_suffix': ' ',
-            'type': click.Choice(['y', 'n', 'N']),
-            'default': 'y'
+            "prompt_suffix": " ",
+            "type": click.Choice(["y", "n", "N"]),
+            "default": "y",
         }
 
         # `show_choices` has been added in click 7.0. Support for click < 7 is needed for distributions
         # that only provide click 6 in their package managers
-        if 'show_choices' in inspect.signature(click.prompt).parameters:
-            prompt_kwargs['show_choices'] = False
+        if "show_choices" in inspect.signature(click.prompt).parameters:
+            prompt_kwargs["show_choices"] = False
 
         try:
             create_alias = click.prompt(
                 "Make the {} alias always use this role? ([y]es, [n]o, [N]ever)".format(
-                    click.style(entry.alias, fg='yellow')
-                ), **prompt_kwargs
+                    click.style(entry.alias, fg="yellow")
+                ),
+                **prompt_kwargs
             )
         except click.exceptions.Abort:
             click.echo()
             raise PushEntryFailed("Skipped")
 
-        if create_alias == 'y':
+        if create_alias == "y":
             update_alias_mapping(
-                context['settings'], entry.alias,
-                aliases_database[entry.alias].mapping[:2] + (str(role.id),)
+                context["settings"],
+                entry.alias,
+                aliases_database[entry.alias].mapping[:2] + (str(role.id),),
             )
 
-            click.secho("Alias {} now points to the role {}".format(
-                entry.alias, role.full_name
-            ), fg='green')
-        elif create_alias == 'N':
+            click.secho(
+                "Alias {} now points to the role {}".format(
+                    entry.alias, role.full_name
+                ),
+                fg="green",
+            )
+        elif create_alias == "N":
             update_alias_mapping(
-                context['settings'], entry.alias,
-                aliases_database[entry.alias].mapping[:2] + (NEVER_SAVE_ROLE_ID,)
+                context["settings"],
+                entry.alias,
+                aliases_database[entry.alias].mapping[:2] + (NEVER_SAVE_ROLE_ID,),
             )
 
     return role
```

### Comparing `taxi_zebra-3.1.0/taxi_zebra/utils.py` & `taxi_zebra-4.0.0/taxi_zebra/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,18 @@
     return role_id
 
 
 def to_zebra_params(params):
     """
     Transforms the given `params` dict to values that are understood by Zebra (eg. False is represented as 'false')
     """
+
     def to_zebra_value(value):
         transform_funcs = {
-            bool: lambda v: 'true' if v else 'false',
+            bool: lambda v: "true" if v else "false",
         }
 
         return transform_funcs.get(type(value), lambda v: v)(value)
 
     return {param: to_zebra_value(value) for param, value in params.items()}
```

### Comparing `taxi_zebra-3.1.0/tests/test_backend.py` & `taxi_zebra-4.0.0/tests/test_backend.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import datetime
 import json
 from unittest.mock import patch
 
 import pytest
 import responses
+
 import taxi.aliases
 from taxi.aliases import Mapping
 from taxi.backends import PushEntryFailed
+from taxi.exceptions import TaxiException
 from taxi.projects import ProjectsDb
 from taxi.timesheet.entry import Entry
 from taxi.ui.tty import TtyUi
-
 from taxi_zebra.backend import Role, ZebraBackend
 
 hostname = "zebralocal"
-username = "john.doe"
+token = "a-long-hexadecimal-token"
 base_endpoint = "https://{}:443".format(hostname)
 urls = {
     name: base_endpoint + url
     for name, url in {
-        "login": "/login/user/{}.json".format(username),
         "user_info": "/api/v2/users/me",
         "timesheets": "/api/v2/timesheets/",
-        "latestActivityRoles": "/api/v2/latestActivityRoles"
+        "latestActivityRoles": "/api/v2/latestActivityRoles",
     }.items()
 }
 
 
 @pytest.fixture
 def aliases_database():
     taxi.aliases.aliases_database.reset()
@@ -46,62 +46,77 @@
         yield r
 
 
 @pytest.fixture
 def backend(aliases_database, tmp_path):
     projects_db_path = str(tmp_path / "projects.json")
     yield ZebraBackend(
-        username=username, password="foobar", hostname=hostname, port=443,
-        path="", options={}, context={"view": TtyUi(), "projects_db": ProjectsDb(projects_db_path)}
+        username=token,
+        password="",
+        hostname=hostname,
+        port=443,
+        path="",
+        options={},
+        context={"view": TtyUi(), "projects_db": ProjectsDb(projects_db_path)},
     )
 
 
 @pytest.fixture
 def authenticated_responses(mocked_responses):
     user_info = {
         "success": True,
         "data": {
             "roles": {
                 2: {"id": 2, "parent_id": 1, "full_name": "Role"},
                 3: {"id": 3, "parent_id": 1, "full_name": "Role 2"},
             }
-        }
-    }
-    latest_activity_roles = {
-        "success": True,
-        "data": {
-            "1": 2
-        }
+        },
     }
+    latest_activity_roles = {"success": True, "data": {"1": 2}}
 
-    mocked_responses.add(responses.POST,
-                         urls["login"],
-                         body="{}", status=200, content_type="application/json")
-    mocked_responses.add(responses.GET,
-                         urls["user_info"], body=json.dumps(user_info),
-                         status=200, content_type="application/json")
-    mocked_responses.add(responses.GET,
-                         urls["latestActivityRoles"], body=json.dumps(latest_activity_roles),
-                         status=200, content_type="application/json")
-    mocked_responses.add(responses.POST,
-                         urls["timesheets"], body=json.dumps({"success": True}),
-                         status=200, content_type="application/json")
+    mocked_responses.add(
+        responses.GET,
+        urls["user_info"],
+        body=json.dumps(user_info),
+        status=200,
+        content_type="application/json",
+    )
+    mocked_responses.add(
+        responses.GET,
+        urls["latestActivityRoles"],
+        body=json.dumps(latest_activity_roles),
+        status=200,
+        content_type="application/json",
+    )
+    mocked_responses.add(
+        responses.POST,
+        urls["timesheets"],
+        body=json.dumps({"success": True}),
+        status=200,
+        content_type="application/json",
+    )
 
     yield mocked_responses
 
 
 def require_role(authenticated_responses):
     authenticated_responses.remove(responses.POST, urls["timesheets"])
     authenticated_responses.add(
-        responses.POST, urls["timesheets"], body=json.dumps({"errorCode": "role_needed"}),
-        status=400, content_type="application/json"
+        responses.POST,
+        urls["timesheets"],
+        body=json.dumps({"errorCode": "role_needed"}),
+        status=400,
+        content_type="application/json",
     )
     authenticated_responses.add(
-        responses.POST, urls["timesheets"], body=json.dumps({"success": True}),
-        status=200, content_type="application/json"
+        responses.POST,
+        urls["timesheets"],
+        body=json.dumps({"success": True}),
+        status=200,
+        content_type="application/json",
     )
 
     return authenticated_responses
 
 
 def test_role_is_prompted_when_needed(authenticated_responses, backend):
     require_role(authenticated_responses)
@@ -112,16 +127,19 @@
     with patch("taxi_zebra.backend.prompt_role") as prompt_role:
         prompt_role.return_value = role
         backend.push_entry(datetime.date.today(), entry)
 
         prompt_role.assert_called_once_with(
             entry,
             [role, Role(id="3", parent_id="1", full_name="Role 2")],
-            {"view": backend.context["view"], "projects_db": backend.context["projects_db"]},
-            default_role=Role(id="2", parent_id="1", full_name="Role")
+            {
+                "view": backend.context["view"],
+                "projects_db": backend.context["projects_db"],
+            },
+            default_role=Role(id="2", parent_id="1", full_name="Role"),
         )
 
     push_call = authenticated_responses.calls[-1]
     assert "role_id={}".format(role.id) in push_call.request.body
     assert "individual_action=false" in push_call.request.body
 
 
@@ -129,34 +147,40 @@
     entry = Entry(alias="alias1", duration=1, description="")
 
     with patch("taxi_zebra.backend.prompt_role") as prompt_role:
         backend.push_entry(datetime.date.today(), entry)
         prompt_role.assert_not_called()
 
 
-def test_role_is_not_prompted_when_alias_has_role(authenticated_responses,
-                                                  backend, aliases_database):
+def test_role_is_not_prompted_when_alias_has_role(
+    authenticated_responses, backend, aliases_database
+):
     entry = Entry(alias="alias2", duration=1, description="")
     aliases_database["alias2"] = Mapping(mapping=("1", "1", "2"), backend="local")
 
     with patch("taxi_zebra.backend.prompt_role") as prompt_role:
         backend.push_entry(datetime.date.today(), entry)
         prompt_role.assert_not_called()
 
     push_call = authenticated_responses.calls[-1]
     assert "role_id=2" in push_call.request.body
 
 
 def test_push_returns_backend_messages(authenticated_responses, backend):
-    success_response = {"success": True, "messages": [{"text": "Hello world",
-                                                       "type": "warning"}]}
+    success_response = {
+        "success": True,
+        "messages": [{"text": "Hello world", "type": "warning"}],
+    }
 
     authenticated_responses.replace(
-        responses.POST, urls["timesheets"], body=json.dumps(success_response),
-        status=200, content_type="application/json"
+        responses.POST,
+        urls["timesheets"],
+        body=json.dumps(success_response),
+        status=200,
+        content_type="application/json",
     )
     entry = Entry(alias="alias1", duration=1, description="")
     additional_info = backend.push_entry(datetime.date.today(), entry)
 
     assert "Hello world" in additional_info
 
 
@@ -191,52 +215,75 @@
         patched_input.side_effect = ["", "n"]
         backend.push_entry(datetime.date.today(), entry)
 
     push_call = authenticated_responses.calls[-1]
     assert "role_id=2" in push_call.request.body
 
 
-def test_latest_role_is_not_proposed_when_not_available(authenticated_responses, backend, capsys):
+def test_latest_role_is_not_proposed_when_not_available(
+    authenticated_responses, backend, capsys
+):
     require_role(authenticated_responses)
-    authenticated_responses.replace(responses.GET,
-                                    urls["latestActivityRoles"],
-                                    body=json.dumps({"success": True, "data": {1: "999"}}),
-                                    status=200, content_type="application/json")
+    authenticated_responses.replace(
+        responses.GET,
+        urls["latestActivityRoles"],
+        body=json.dumps({"success": True, "data": {1: "999"}}),
+        status=200,
+        content_type="application/json",
+    )
     entry = Entry(alias="alias1", duration=1, description="")
 
     with patch("click.termui.visible_prompt_func") as patched_input:
         patched_input.return_value = "c"
         with pytest.raises(PushEntryFailed):
             backend.push_entry(datetime.date.today(), entry)
 
     assert "Select a role:" in capsys.readouterr().out
 
 
-def test_no_default_role_proposed_when_alias_never_used(authenticated_responses, backend, capsys):
+def test_no_default_role_proposed_when_alias_never_used(
+    authenticated_responses, backend, capsys
+):
     require_role(authenticated_responses)
-    authenticated_responses.replace(responses.GET,
-                                    urls["latestActivityRoles"],
-                                    body=json.dumps({"success": True, "data": {}}),
-                                    status=200, content_type="application/json")
+    authenticated_responses.replace(
+        responses.GET,
+        urls["latestActivityRoles"],
+        body=json.dumps({"success": True, "data": {}}),
+        status=200,
+        content_type="application/json",
+    )
     entry = Entry(alias="alias1", duration=1, description="")
 
     with patch("click.termui.visible_prompt_func") as patched_input:
         patched_input.return_value = "c"
         with pytest.raises(PushEntryFailed):
             backend.push_entry(datetime.date.today(), entry)
 
     assert "Select a role:" in capsys.readouterr().out
 
 
 def test_default_role_updates_between_entries(authenticated_responses, backend, capsys):
     entries = [
         Entry(alias="alias1", duration=1, description="foo"),
-        Entry(alias="alias1", duration=1, description="bar")
+        Entry(alias="alias1", duration=1, description="bar"),
     ]
 
     with patch("click.termui.visible_prompt_func") as patched_input:
         patched_input.side_effect = ["1", "n", "", "n"]
         for entry in entries:
             require_role(authenticated_responses)
             backend.push_entry(datetime.date.today(), entry)
 
     assert "Select a role (leave empty for Role 2):" in capsys.readouterr().out
+
+
+def test_zebra_backend_doesnt_accept_password():
+    with pytest.raises(TaxiException):
+        ZebraBackend(
+            username="very-old-liiper",
+            password="has-an-imap-password",
+            hostname=hostname,
+            port=443,
+            path="",
+            options={},
+            context={},
+        )
```

