# Comparing `tmp/forevd-0.1.5.tar.gz` & `tmp/forevd-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forevd-0.1.5.tar", max compression
+gzip compressed data, was "forevd-0.1.6.tar", max compression
```

## Comparing `forevd-0.1.5.tar` & `forevd-0.1.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11357 2023-05-31 18:58:46.623227 forevd-0.1.5/LICENSE
--rw-r--r--   0        0        0     4019 2023-05-31 18:58:46.623227 forevd-0.1.5/README.md
--rw-r--r--   0        0        0        0 2023-05-31 18:58:46.627226 forevd-0.1.5/forevd/__init__.py
--rw-r--r--   0        0        0     4760 2023-05-31 18:58:46.627226 forevd-0.1.5/forevd/__main__.py
--rw-r--r--   0        0        0     1543 2023-05-31 18:58:46.627226 forevd-0.1.5/forevd/apache/__init__.py
--rw-r--r--   0        0        0     4500 2023-05-31 18:58:46.627226 forevd-0.1.5/forevd/apache/httpd.conf
--rw-r--r--   0        0        0      216 2023-05-31 18:58:46.627226 forevd-0.1.5/forevd/app.py
--rw-r--r--   0        0        0        0 2023-05-31 18:58:46.627226 forevd-0.1.5/forevd/resources/__init__.py
--rw-r--r--   0        0        0        0 2023-05-31 18:58:46.627226 forevd-0.1.5/forevd/resources/logging/__init__.py
--rw-r--r--   0        0        0      387 2023-05-31 18:58:46.627226 forevd-0.1.5/forevd/resources/logging/cli.conf
--rw-r--r--   0        0        0      884 2023-05-31 18:58:46.627226 forevd-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     4724 1970-01-01 00:00:00.000000 forevd-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-01 11:18:49.906961 forevd-0.1.6/LICENSE
+-rw-r--r--   0        0        0     4063 2023-06-01 11:18:49.906961 forevd-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2023-06-01 11:18:49.906961 forevd-0.1.6/forevd/__init__.py
+-rw-r--r--   0        0        0     5214 2023-06-01 11:18:49.906961 forevd-0.1.6/forevd/__main__.py
+-rw-r--r--   0        0        0     1543 2023-06-01 11:18:49.906961 forevd-0.1.6/forevd/apache/__init__.py
+-rw-r--r--   0        0        0     4461 2023-06-01 11:18:49.906961 forevd-0.1.6/forevd/apache/httpd.conf
+-rw-r--r--   0        0        0      216 2023-06-01 11:18:49.906961 forevd-0.1.6/forevd/app.py
+-rw-r--r--   0        0        0        0 2023-06-01 11:18:49.906961 forevd-0.1.6/forevd/resources/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-01 11:18:49.906961 forevd-0.1.6/forevd/resources/logging/__init__.py
+-rw-r--r--   0        0        0      387 2023-06-01 11:18:49.906961 forevd-0.1.6/forevd/resources/logging/cli.conf
+-rw-r--r--   0        0        0      884 2023-06-01 11:18:49.906961 forevd-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     4768 1970-01-01 00:00:00.000000 forevd-0.1.6/PKG-INFO
```

### Comparing `forevd-0.1.5/LICENSE` & `forevd-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `forevd-0.1.5/README.md` & `forevd-0.1.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 # Table of contents
 1. [Intro](#intro)
-2. [Dependencies](#deps)
-3. [Running `forevd`](#running)
-    1. [Config Files](#config)
-    2. [Mutual TLS](#mtls)
+2. [Dependencies](#dependencies)
+3. [Running `forevd`](#running-forevd)
+    1. [Config Files](#config-files)
+    2. [Mutual TLS](#mutual-tls)
 
-# <a name="intro" />Intro
+# Intro
 
 `forevd` is a forward and reverse proxy that helps deliver authentication and, optionally,
 authorization as a sidecar.
 
 This project was created to help eliminate any need to add authentication into your application
 code.
 
-# <a name="deps" />Dependencies
+# Dependencies
 
 At the moment, `forevd`, runs using Apache, so you will need to have httpd or docker image of it
 available at runtime.
 
 - Apache
 - nginx (TBD)
 
-# <a name="running" />Running `forevd`
+# Running `forevd`
 
 The following proivides some details on how to run `forevd`. The way the options work are that
 anything provided immediately on the CLI, are "global" defaults; if you then provide config
 (optionally files), via the `--locations`, `--ldap` or `--oidc` options, then those will override
 the CLI options, of, e.g. `--backend` and `--location`
 
-## <a name="config" />Config Files
+## Config Files
 
 You can optionally provide config files for more complicated setups; this section provides soem
 examples, which can be found in the `etc` directory.
 
 The config files use Jinja2 templating via environment variables, so, instead of putting values in
 directly, you can use the form `{{ ENV_VAR_NAME }}` to have the environment varibale injected at
 runtime.
@@ -101,15 +101,15 @@
 SharedCacheSize: 500000
 CacheEntries: 1024
 CacheTTL: 600
 OpCacheEntries: 1024
 OpCacheTTL: 600
 ```
 
-## <a name="mtls" />Mutual TLS
+## Mutual TLS
 
 The following command provides termination of mTLS on `/` and redirects connections to a backend at
 `http://localhost:8081`
 
 ```
 forevd --debug --listen 0.0.0.0:8080 \
     --ca-cert $PWD/../certs/ca/ca-cert.pem
@@ -118,10 +118,14 @@
     --backend http://localhost:8081
     --location /
     --mtls require
     --server-name example.com
     --var-dir /var/tmp/apache
 ```
 
-## <a name="mtls" />Authorization
+## Authorization
 
 To add authorization, it's recommended you use a config file for the `--locations` command line.
+
+There is currently support for LDAP group lookup and static user names.
+
+See [Locations Example](#example) for more detail.
```

### Comparing `forevd-0.1.5/forevd/__main__.py` & `forevd-0.1.6/forevd/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,20 +31,30 @@
 
 def _nomalize_locations(
     locations: dict, backend: str, location: str, mtls: bool, http_methods: list
 ):
     if not locations:
         locations = {}
 
-    loc_struct = locations.get(location, {})
-    loc_struct["backend"] = backend
-    loc_struct["mtls"] = mtls
-    loc_struct["http_methods"] = http_methods
+    endpoints = list(locations.keys())
+    if location:
+        endpoints.insert(0, location)
+    _LOGGER.debug(f"endpoints: {endpoints}")
+
+    for endpoint in endpoints:
+        config = locations[endpoint]
+        if "backend" not in config:
+            config["backend"] = backend
+        if "mtls" not in config:
+            config["mtls"] = mtls
+        if "http_methods" not in config:
+            config["http_methods"] = http_methods
 
-    locations[location] = loc_struct
+        locations[endpoint] = config
+    _LOGGER.debug(f"locations: {locations}")
 
     return locations
 
 
 @click.command()
 @click.option(
     "--access-log",
@@ -169,17 +179,20 @@
     oidc,
     server_name,
     var_dir,
 ):
     """forevd is a forward/reverse proxy, primarily used as a sidecar for REST or any HTTP/s apps."""
     _setup_logging(debug)
 
-    if not backend and location and not locations:
+    if (not backend or not location) and not locations:
         raise click.UsageError("You must supply a --backend and --location or --locations")
 
+    if mtls and not cert:
+        raise click.UsageError("You must provide --cert and --cert-key, for mTLS support.")
+
     config = {
         "err_log": err_log,
         "access_log": access_log,
         "ca_cert": ca_cert,
         "cert": cert,
         "cert_key": cert_key,
         "debug": debug,
```

### Comparing `forevd-0.1.5/forevd/apache/__init__.py` & `forevd-0.1.6/forevd/apache/__init__.py`

 * *Files identical despite different names*

### Comparing `forevd-0.1.5/forevd/apache/httpd.conf` & `forevd-0.1.6/forevd/apache/httpd.conf`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,14 @@
 SSLCipherSuite ALL:!EXP:!eNULL:!aNULL:!MD5:-LOW:-RC4:-SSLv2:+HIGH:+MEDIUM
 SSLVerifyDepth 5
 SSLProtocol all -TLSv1.3
 SSLSessionCache "shmcb:/usr/local/apache2/logs/ssl_scache(512000)"
 SSLSessionCacheTimeout 300
 
 SSLCACertificateFile {{ ca_cert }}
-SSLCertificateChainFile {{ ca_cert }}
 SSLCertificateFile {{ cert }}
 SSLCertificateKeyFile {{ cert_key }}
 {% endif %}
 
 {% if oidc -%}
 OIDCCryptoPassphrase {% if oidc["CryptoPassphrase"] %}{{ oidc["CryptoPassphrase"] }}{% else %}"exec:/bin/bash -c \"head /dev/urandom | tr -dc A-Za-z0-9 | head -c 32\""{% endif %}
 OIDCRedirectURI {% if oidc["RedirectURI"] %}{{ oidc["RedirectURI"] }}{% else %}https://{{ server_name }}/secure/redirect_uri{% endif %}
@@ -142,10 +141,10 @@
 
     {% if not location["http_methods"] %}
     {{ required_users }}
     {% else -%}
     <Limit {{ location["http_methods"]|join(" ") }}>
         {{ required_users }}
     </Limit>
-    {% endif -%}
+    {% endif %}
 </Location>
 {% endfor %}
```

### Comparing `forevd-0.1.5/pyproject.toml` & `forevd-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "forevd"
-version = "0.1.5"
+version = "0.1.6"
 description = "Forward and reverse proxy using nginx or apache"
 authors = ["Erick Bourgeois <erick@jeb.ca>"]
 license = "LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `forevd-0.1.5/PKG-INFO` & `forevd-0.1.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forevd
-Version: 0.1.5
+Version: 0.1.6
 Summary: Forward and reverse proxy using nginx or apache
 License: LICENSE
 Author: Erick Bourgeois
 Author-email: erick@jeb.ca
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -16,43 +16,43 @@
 Requires-Dist: firestone-lib (>=0.1.8,<0.2.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: uvicorn (>=0.22.0,<0.23.0)
 Description-Content-Type: text/markdown
 
 # Table of contents
 1. [Intro](#intro)
-2. [Dependencies](#deps)
-3. [Running `forevd`](#running)
-    1. [Config Files](#config)
-    2. [Mutual TLS](#mtls)
+2. [Dependencies](#dependencies)
+3. [Running `forevd`](#running-forevd)
+    1. [Config Files](#config-files)
+    2. [Mutual TLS](#mutual-tls)
 
-# <a name="intro" />Intro
+# Intro
 
 `forevd` is a forward and reverse proxy that helps deliver authentication and, optionally,
 authorization as a sidecar.
 
 This project was created to help eliminate any need to add authentication into your application
 code.
 
-# <a name="deps" />Dependencies
+# Dependencies
 
 At the moment, `forevd`, runs using Apache, so you will need to have httpd or docker image of it
 available at runtime.
 
 - Apache
 - nginx (TBD)
 
-# <a name="running" />Running `forevd`
+# Running `forevd`
 
 The following proivides some details on how to run `forevd`. The way the options work are that
 anything provided immediately on the CLI, are "global" defaults; if you then provide config
 (optionally files), via the `--locations`, `--ldap` or `--oidc` options, then those will override
 the CLI options, of, e.g. `--backend` and `--location`
 
-## <a name="config" />Config Files
+## Config Files
 
 You can optionally provide config files for more complicated setups; this section provides soem
 examples, which can be found in the `etc` directory.
 
 The config files use Jinja2 templating via environment variables, so, instead of putting values in
 directly, you can use the form `{{ ENV_VAR_NAME }}` to have the environment varibale injected at
 runtime.
@@ -121,15 +121,15 @@
 SharedCacheSize: 500000
 CacheEntries: 1024
 CacheTTL: 600
 OpCacheEntries: 1024
 OpCacheTTL: 600
 ```
 
-## <a name="mtls" />Mutual TLS
+## Mutual TLS
 
 The following command provides termination of mTLS on `/` and redirects connections to a backend at
 `http://localhost:8081`
 
 ```
 forevd --debug --listen 0.0.0.0:8080 \
     --ca-cert $PWD/../certs/ca/ca-cert.pem
@@ -138,11 +138,15 @@
     --backend http://localhost:8081
     --location /
     --mtls require
     --server-name example.com
     --var-dir /var/tmp/apache
 ```
 
-## <a name="mtls" />Authorization
+## Authorization
 
 To add authorization, it's recommended you use a config file for the `--locations` command line.
 
+There is currently support for LDAP group lookup and static user names.
+
+See [Locations Example](#example) for more detail.
+
```

