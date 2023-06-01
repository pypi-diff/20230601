# Comparing `tmp/fal_serverless-0.6.32.tar.gz` & `tmp/fal_serverless-0.6.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fal_serverless-0.6.32.tar", max compression
+gzip compressed data, was "fal_serverless-0.6.33.tar", max compression
```

## Comparing `fal_serverless-0.6.32.tar` & `fal_serverless-0.6.33.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      213 2023-05-22 22:26:27.574124 fal_serverless-0.6.32/README.md
--rw-r--r--   0        0        0      997 2023-05-22 22:27:48.446837 fal_serverless-0.6.32/pyproject.toml
--rw-r--r--   0        0        0      335 2023-05-22 22:26:27.574124 fal_serverless-0.6.32/src/fal_serverless/__init__.py
--rw-r--r--   0        0        0    17062 2023-05-22 22:26:27.574124 fal_serverless-0.6.32/src/fal_serverless/api.py
--rw-r--r--   0        0        0     2532 2023-05-22 22:26:27.574124 fal_serverless-0.6.32/src/fal_serverless/auth/__init__.py
--rw-r--r--   0        0        0     5027 2023-05-22 22:26:27.574124 fal_serverless-0.6.32/src/fal_serverless/auth/auth0.py
--rw-r--r--   0        0        0     1786 2023-05-22 22:26:27.574124 fal_serverless-0.6.32/src/fal_serverless/auth/local.py
--rw-r--r--   0        0        0    15093 2023-05-22 22:26:27.574124 fal_serverless-0.6.32/src/fal_serverless/cli.py
--rw-r--r--   0        0        0      132 2023-05-22 22:26:27.574124 fal_serverless-0.6.32/src/fal_serverless/console/__init__.py
--rw-r--r--   0        0        0      108 2023-05-22 22:26:27.574124 fal_serverless-0.6.32/src/fal_serverless/console/icons.py
--rw-r--r--   0        0        0      485 2023-05-22 22:26:27.574124 fal_serverless-0.6.32/src/fal_serverless/console/ux.py
--rw-r--r--   0        0        0      158 2023-05-22 22:26:27.574124 fal_serverless-0.6.32/src/fal_serverless/env.py
--rw-r--r--   0        0        0      938 2023-05-22 22:26:27.574124 fal_serverless-0.6.32/src/fal_serverless/exceptions/__init__.py
--rw-r--r--   0        0        0      412 2023-05-22 22:26:27.574124 fal_serverless-0.6.32/src/fal_serverless/exceptions/_base.py
--rw-r--r--   0        0        0      353 2023-05-22 22:26:27.574124 fal_serverless-0.6.32/src/fal_serverless/exceptions/auth.py
--rw-r--r--   0        0        0     1435 2023-05-22 22:26:27.574124 fal_serverless-0.6.32/src/fal_serverless/exceptions/handlers.py
--rw-r--r--   0        0        0      326 2023-05-22 22:26:27.574124 fal_serverless-0.6.32/src/fal_serverless/flags.py
--rw-r--r--   0        0        0     1649 2023-05-22 22:26:27.574124 fal_serverless-0.6.32/src/fal_serverless/logging/__init__.py
--rw-r--r--   0        0        0     2574 2023-05-22 22:26:27.574124 fal_serverless-0.6.32/src/fal_serverless/logging/datadog.py
--rw-r--r--   0        0        0     2122 2023-05-22 22:26:27.574124 fal_serverless-0.6.32/src/fal_serverless/logging/isolate.py
--rw-r--r--   0        0        0      386 2023-05-22 22:26:27.574124 fal_serverless-0.6.32/src/fal_serverless/logging/style.py
--rw-r--r--   0        0        0     1785 2023-05-22 22:26:27.574124 fal_serverless-0.6.32/src/fal_serverless/logging/trace.py
--rw-r--r--   0        0        0      643 2023-05-22 22:26:27.574124 fal_serverless-0.6.32/src/fal_serverless/logging/user.py
--rw-r--r--   0        0        0    15875 2023-05-22 22:26:27.574124 fal_serverless-0.6.32/src/fal_serverless/sdk.py
--rw-r--r--   0        0        0     5335 2023-05-22 22:26:27.574124 fal_serverless-0.6.32/src/fal_serverless/sync.py
--rw-r--r--   0        0        0     1771 1970-01-01 00:00:00.000000 fal_serverless-0.6.32/setup.py
--rw-r--r--   0        0        0     1601 1970-01-01 00:00:00.000000 fal_serverless-0.6.32/PKG-INFO
+-rw-r--r--   0        0        0      213 2023-06-01 14:31:42.566849 fal_serverless-0.6.33/README.md
+-rw-r--r--   0        0        0      998 2023-06-01 14:32:00.095054 fal_serverless-0.6.33/pyproject.toml
+-rw-r--r--   0        0        0      335 2023-06-01 14:31:42.570849 fal_serverless-0.6.33/src/fal_serverless/__init__.py
+-rw-r--r--   0        0        0    17363 2023-06-01 14:31:42.570849 fal_serverless-0.6.33/src/fal_serverless/api.py
+-rw-r--r--   0        0        0     2593 2023-06-01 14:31:42.570849 fal_serverless-0.6.33/src/fal_serverless/auth/__init__.py
+-rw-r--r--   0        0        0     5426 2023-06-01 14:31:42.570849 fal_serverless-0.6.33/src/fal_serverless/auth/auth0.py
+-rw-r--r--   0        0        0     1786 2023-06-01 14:31:42.570849 fal_serverless-0.6.33/src/fal_serverless/auth/local.py
+-rw-r--r--   0        0        0    15759 2023-06-01 14:31:42.570849 fal_serverless-0.6.33/src/fal_serverless/cli.py
+-rw-r--r--   0        0        0      132 2023-06-01 14:31:42.570849 fal_serverless-0.6.33/src/fal_serverless/console/__init__.py
+-rw-r--r--   0        0        0      108 2023-06-01 14:31:42.570849 fal_serverless-0.6.33/src/fal_serverless/console/icons.py
+-rw-r--r--   0        0        0      485 2023-06-01 14:31:42.570849 fal_serverless-0.6.33/src/fal_serverless/console/ux.py
+-rw-r--r--   0        0        0      172 2023-06-01 14:31:53.702972 fal_serverless-0.6.33/src/fal_serverless/env.py
+-rw-r--r--   0        0        0      938 2023-06-01 14:31:42.570849 fal_serverless-0.6.33/src/fal_serverless/exceptions/__init__.py
+-rw-r--r--   0        0        0      412 2023-06-01 14:31:42.570849 fal_serverless-0.6.33/src/fal_serverless/exceptions/_base.py
+-rw-r--r--   0        0        0      353 2023-06-01 14:31:42.570849 fal_serverless-0.6.33/src/fal_serverless/exceptions/auth.py
+-rw-r--r--   0        0        0     1435 2023-06-01 14:31:42.570849 fal_serverless-0.6.33/src/fal_serverless/exceptions/handlers.py
+-rw-r--r--   0        0        0      326 2023-06-01 14:31:42.570849 fal_serverless-0.6.33/src/fal_serverless/flags.py
+-rw-r--r--   0        0        0     1649 2023-06-01 14:31:42.570849 fal_serverless-0.6.33/src/fal_serverless/logging/__init__.py
+-rw-r--r--   0        0        0     2574 2023-06-01 14:31:42.570849 fal_serverless-0.6.33/src/fal_serverless/logging/datadog.py
+-rw-r--r--   0        0        0     2122 2023-06-01 14:31:42.570849 fal_serverless-0.6.33/src/fal_serverless/logging/isolate.py
+-rw-r--r--   0        0        0      386 2023-06-01 14:31:42.570849 fal_serverless-0.6.33/src/fal_serverless/logging/style.py
+-rw-r--r--   0        0        0     1785 2023-06-01 14:31:42.570849 fal_serverless-0.6.33/src/fal_serverless/logging/trace.py
+-rw-r--r--   0        0        0      643 2023-06-01 14:31:42.570849 fal_serverless-0.6.33/src/fal_serverless/logging/user.py
+-rw-r--r--   0        0        0    15875 2023-06-01 14:31:42.570849 fal_serverless-0.6.33/src/fal_serverless/sdk.py
+-rw-r--r--   0        0        0     5335 2023-06-01 14:31:42.570849 fal_serverless-0.6.33/src/fal_serverless/sync.py
+-rw-r--r--   0        0        0     1773 1970-01-01 00:00:00.000000 fal_serverless-0.6.33/setup.py
+-rw-r--r--   0        0        0     1603 1970-01-01 00:00:00.000000 fal_serverless-0.6.33/PKG-INFO
```

### Comparing `fal_serverless-0.6.32/pyproject.toml` & `fal_serverless-0.6.33/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "fal_serverless"
-version = "0.6.32"
+version = "0.6.33"
 description = "fal Serverless is an easy-to-use Serverless Python Framework"
 authors = ["Features & Labels <hello@fal.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 auth0-python = "^4.1.0"
 requests = "^2.28.1"
 isolate = {version = "0.12.0", extras = ["build"]}
 grpcio = "^1.50.0"
 dill = "0.3.5.1"
-isolate-proto = "0.0.28"
+isolate-proto = "^0.0.28"
 typing-extensions = "4.4"
 click = "^8.1.3"
 structlog = "^22.3.0"
-datadog-api-client = "^2.9.0"
+datadog-api-client = "2.12.0"
 opentelemetry-api = "^1.15.0"
 opentelemetry-sdk = "^1.15.0"
 grpc-interceptor = "^0.15.0"
 colorama = "^0.4.6"
 portalocker = "^2.7.0"
 rich = "^13.3.2"
```

### Comparing `fal_serverless-0.6.32/src/fal_serverless/api.py` & `fal_serverless-0.6.33/src/fal_serverless/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -422,16 +422,26 @@
         from flask_cors import CORS
 
         app = Flask("fal")
         cors = CORS(app, resources={r"/*": {"origins": "*"}})
 
         @app.route("/", methods=["POST"])
         def flask():
-            params = [request.get_json().get(param) for param in param_names]
-            return jsonify({"result": func(*params)})
+            try:
+                body = request.get_json()
+                if not isinstance(body, dict):
+                    raise TypeError("Body must be a JSON object")
+
+                res = func(**body)
+            except TypeError as e:
+                return jsonify({"error": str(e)}), 400
+            except Exception as e:
+                return jsonify({"error": str(e)}), 500
+
+            return jsonify({"result": res})
 
         app.run(host="0.0.0.0", port=8080)
 
     return templated_flask_wrapper
 
 
 @dataclass
```

### Comparing `fal_serverless-0.6.32/src/fal_serverless/auth/__init__.py` & `fal_serverless-0.6.33/src/fal_serverless/auth/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 from fal_serverless.auth import auth0, local
 from fal_serverless.console import console
 from fal_serverless.console.icons import CHECK_ICON
 from fal_serverless.exceptions.auth import UnauthenticatedException
 
 
 def login():
-    token_data = auth0.login()
+    refresh_token, _ = local.load_token()
+    token_data = auth0.login(bool(refresh_token))
     local.save_token(token_data["refresh_token"])
 
 
 def logout():
     refresh_token, _ = local.load_token()
     if refresh_token is None:
         raise click.ClickException(message="You're not logged in")
```

### Comparing `fal_serverless-0.6.32/src/fal_serverless/auth/auth0.py` & `fal_serverless-0.6.33/src/fal_serverless/auth/auth0.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,24 +9,46 @@
     AsymmetricSignatureVerifier,
     TokenVerifier,
 )
 from fal_serverless.console import console
 from fal_serverless.console.icons import CHECK_ICON
 from fal_serverless.console.ux import get_browser
 
+WEBSITE_URL = "https://fal.ai"
+
 AUTH0_DOMAIN = "auth.fal.ai"
 AUTH0_JWKS_URL = f"https://{AUTH0_DOMAIN}/.well-known/jwks.json"
 AUTH0_ALGORITHMS = ["RS256"]
 AUTH0_ISSUER = f"https://{AUTH0_DOMAIN}/"
 AUTH0_FAL_API_AUDIENCE_ID = "fal-cloud"
 AUTH0_CLIENT_ID = "TwXR51Vz8JbY8GUUMy6EyuVR0fTO7N4N"
 AUTH0_SCOPE = "openid profile email offline_access"
 
 
-def login() -> dict:
+def logout_url(return_url: str):
+    return f"https://{AUTH0_DOMAIN}/v2/logout?client_id={AUTH0_CLIENT_ID}&returnTo={return_url}"
+
+
+def _open_browser(url: str, code: str | None) -> None:
+    browser = get_browser()
+    console.print()
+
+    if browser is not None and click.confirm(
+        "Open browser automatically ('no' to show URL)?", default=True, err=True
+    ):
+        browser.open_new_tab(url)
+    else:
+        console.print(f"On your computer or mobile device navigate to: {url}")
+        if code:
+            console.print(
+                f"Confirm it shows the following code: [markdown.code]{code}[/]"
+            )
+
+
+def login(logout_first: bool) -> dict:
     """
     Runs the device authorization flow and stores the user object in memory
     """
     device_code_payload = {
         "audience": AUTH0_FAL_API_AUDIENCE_ID,
         "client_id": AUTH0_CLIENT_ID,
         "scope": AUTH0_SCOPE,
@@ -38,28 +60,20 @@
     if device_code_response.status_code != 200:
         raise click.ClickException("Error generating the device code")
 
     device_code_data = device_code_response.json()
     device_user_code = device_code_data["user_code"]
     device_confirmation_url = device_code_data["verification_uri_complete"]
 
-    browser = get_browser()
-    console.print()
-
-    if browser is not None and click.confirm(
-        "Open browser automatically ('no' to show URL)?", default=True, err=True
-    ):
-        browser.open_new_tab(device_confirmation_url)
+    if logout_first:
+        url = logout_url(device_confirmation_url)
     else:
-        console.print(
-            f"1. On your computer or mobile device navigate to: {device_confirmation_url}"
-        )
-        console.print(
-            f"2. Confirm it shows the following code: [markdown.code]{device_user_code}[/]"
-        )
+        url = device_confirmation_url
+
+    _open_browser(url, device_user_code)
 
     # This is needed to suppress the ResourceWarning emitted
     # when the process is waiting for user confirmation
     warnings.filterwarnings("ignore", category=ResourceWarning)
 
     token_payload = {
         "grant_type": "urn:ietf:params:oauth:grant-type:device_code",
@@ -122,14 +136,16 @@
         f"https://{AUTH0_DOMAIN}/oauth/revoke", data=token_payload
     )
 
     if token_response.status_code != 200:
         token_data = token_response.json()
         raise click.ClickException(token_data["error_description"])
 
+    _open_browser(logout_url(WEBSITE_URL), None)
+
 
 def get_user_info(bearer_token: str) -> dict:
     userinfo_response = requests.post(
         f"https://{AUTH0_DOMAIN}/userinfo",
         headers={"Authorization": bearer_token},
     )
```

### Comparing `fal_serverless-0.6.32/src/fal_serverless/auth/local.py` & `fal_serverless-0.6.33/src/fal_serverless/auth/local.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.32/src/fal_serverless/cli.py` & `fal_serverless-0.6.33/src/fal_serverless/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import operator
 from sys import argv
 from typing import Literal
 from uuid import uuid4
 
 import click
 import fal_serverless.auth as auth
+import grpc
 from fal_serverless import api, sdk
 from fal_serverless.console import console
 from fal_serverless.exceptions import ApplicationExceptionHandler
 from fal_serverless.logging import get_logger, set_debug_logging
 from fal_serverless.logging.isolate import IsolateLogPrinter
 from fal_serverless.logging.trace import get_tracer
 from fal_serverless.sync import list_children, parse_logs
@@ -134,14 +135,23 @@
 def auth_cli():
     pass
 
 
 @auth_cli.command(name="login")
 def auth_login():
     auth.login()
+    try:
+        client = sdk.FalServerlessClient(f"{DEFAULT_HOST}:{DEFAULT_PORT}")
+        with client.connect() as connection:
+            connection.list_worker_status()
+    except grpc.RpcError as e:
+        if "Insufficient permissions" in e.details():
+            console.print(e.details())
+        else:
+            raise e
 
 
 @auth_cli.command(name="logout")
 def auth_logout():
     auth.logout()
 
 
@@ -268,16 +278,24 @@
     import runpy
 
     module = runpy.run_path(file_path)
     isolated_function = module[function_name]
     gateway_options = isolated_function.options.gateway
     if "serve" not in gateway_options and "exposed_port" not in gateway_options:
         raise api.FalServerlessError(
-            "One of `serve` or `exposed-port` options needs to be specified in the isolated annotation to register a function"
+            "One of `serve` or `exposed_port` options needs to be specified in the isolated annotation to register a function"
+        )
+    elif (
+        "exposed_port" in gateway_options
+        and str(gateway_options.get("exposed_port")) != "8080"
+    ):
+        raise api.FalServerlessError(
+            "Must expose port 8080 for now. This will be configurable in the future."
         )
+
     id = host.register(
         func=isolated_function.func,
         options=isolated_function.options,
         application_name=alias,
         application_is_public=auth_mode == "public",
     )
     if id:
@@ -478,11 +496,12 @@
 
 cli.add_command(auth_cli, name="auth")
 cli.add_command(key_cli, name="key", aliases=["keys"])
 cli.add_command(function_cli, name="function", aliases=["fn"])
 cli.add_command(alias_cli, name="alias")
 cli.add_command(crons_cli, name="cron", aliases=["crons"])
 cli.add_command(usage_cli, name="usage")
+cli.add_command(secrets_cli, name="secret", aliases=["secrets"])
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `fal_serverless-0.6.32/src/fal_serverless/exceptions/__init__.py` & `fal_serverless-0.6.33/src/fal_serverless/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.32/src/fal_serverless/exceptions/handlers.py` & `fal_serverless-0.6.33/src/fal_serverless/exceptions/handlers.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.32/src/fal_serverless/logging/__init__.py` & `fal_serverless-0.6.33/src/fal_serverless/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.32/src/fal_serverless/logging/datadog.py` & `fal_serverless-0.6.33/src/fal_serverless/logging/datadog.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.32/src/fal_serverless/logging/isolate.py` & `fal_serverless-0.6.33/src/fal_serverless/logging/isolate.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.32/src/fal_serverless/logging/trace.py` & `fal_serverless-0.6.33/src/fal_serverless/logging/trace.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.32/src/fal_serverless/logging/user.py` & `fal_serverless-0.6.33/src/fal_serverless/logging/user.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.32/src/fal_serverless/sdk.py` & `fal_serverless-0.6.33/src/fal_serverless/sdk.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.32/src/fal_serverless/sync.py` & `fal_serverless-0.6.33/src/fal_serverless/sync.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.32/setup.py` & `fal_serverless-0.6.33/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['auth0-python>=4.1.0,<5.0.0',
  'click>=8.1.3,<9.0.0',
  'colorama>=0.4.6,<0.5.0',
- 'datadog-api-client>=2.9.0,<3.0.0',
+ 'datadog-api-client==2.12.0',
  'dill==0.3.5.1',
  'grpc-interceptor>=0.15.0,<0.16.0',
  'grpcio>=1.50.0,<2.0.0',
- 'isolate-proto==0.0.28',
+ 'isolate-proto>=0.0.28,<0.0.29',
  'isolate[build]==0.12.0',
  'opentelemetry-api>=1.15.0,<2.0.0',
  'opentelemetry-sdk>=1.15.0,<2.0.0',
  'packaging>=21.3',
  'pathspec>=0.11.1,<0.12.0',
  'portalocker>=2.7.0,<3.0.0',
  'requests>=2.28.1,<3.0.0',
@@ -38,15 +38,15 @@
 {':python_version < "3.10"': ['importlib-metadata>=4.4']}
 
 entry_points = \
 {'console_scripts': ['fal-serverless = fal_serverless.cli:cli']}
 
 setup_kwargs = {
     'name': 'fal-serverless',
-    'version': '0.6.32',
+    'version': '0.6.33',
     'description': 'fal Serverless is an easy-to-use Serverless Python Framework',
     'long_description': '# fal-serverless\n\nLibrary to run, serve or schedule your Python functions in the cloud with any machine type you may need.\n\nCheck out to the [docs](https://docs.fal.ai/fal-serverless/quickstart) for more details.\n',
     'author': 'Features & Labels',
     'author_email': 'hello@fal.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `fal_serverless-0.6.32/PKG-INFO` & `fal_serverless-0.6.33/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: fal-serverless
-Version: 0.6.32
+Version: 0.6.33
 Summary: fal Serverless is an easy-to-use Serverless Python Framework
 Author: Features & Labels
 Author-email: hello@fal.ai
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: auth0-python (>=4.1.0,<5.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
-Requires-Dist: datadog-api-client (>=2.9.0,<3.0.0)
+Requires-Dist: datadog-api-client (==2.12.0)
 Requires-Dist: dill (==0.3.5.1)
 Requires-Dist: grpc-interceptor (>=0.15.0,<0.16.0)
 Requires-Dist: grpcio (>=1.50.0,<2.0.0)
 Requires-Dist: importlib-metadata (>=4.4) ; python_version < "3.10"
-Requires-Dist: isolate-proto (==0.0.28)
+Requires-Dist: isolate-proto (>=0.0.28,<0.0.29)
 Requires-Dist: isolate[build] (==0.12.0)
 Requires-Dist: opentelemetry-api (>=1.15.0,<2.0.0)
 Requires-Dist: opentelemetry-sdk (>=1.15.0,<2.0.0)
 Requires-Dist: packaging (>=21.3)
 Requires-Dist: pathspec (>=0.11.1,<0.12.0)
 Requires-Dist: portalocker (>=2.7.0,<3.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
```

