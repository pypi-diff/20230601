# Comparing `tmp/ssm-ps-template-1.1.0.tar.gz` & `tmp/ssm-ps-template-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssm-ps-template-1.1.0.tar", last modified: Fri May 26 20:32:47 2023, max compression
+gzip compressed data, was "ssm-ps-template-2.0.0.tar", last modified: Thu Jun  1 19:59:47 2023, max compression
```

## Comparing `ssm-ps-template-1.1.0.tar` & `ssm-ps-template-2.0.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 20:32:47.702463 ssm-ps-template-1.1.0/
--rw-r--r--   0 root         (0) root         (0)     1495 2023-05-26 20:32:38.000000 ssm-ps-template-1.1.0/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     8651 2023-05-26 20:32:47.698462 ssm-ps-template-1.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6028 2023-05-26 20:32:38.000000 ssm-ps-template-1.1.0/README.md
--rw-r--r--   0 root         (0) root         (0)     1855 2023-05-26 20:32:38.000000 ssm-ps-template-1.1.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-26 20:32:47.702463 ssm-ps-template-1.1.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 20:32:47.698462 ssm-ps-template-1.1.0/ssm_ps_template/
--rw-r--r--   0 root         (0) root         (0)      165 2023-05-26 20:32:38.000000 ssm-ps-template-1.1.0/ssm_ps_template/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3171 2023-05-26 20:32:38.000000 ssm-ps-template-1.1.0/ssm_ps_template/__main__.py
--rw-r--r--   0 root         (0) root         (0)     2364 2023-05-26 20:32:38.000000 ssm-ps-template-1.1.0/ssm_ps_template/config.py
--rw-r--r--   0 root         (0) root         (0)     5644 2023-05-26 20:32:38.000000 ssm-ps-template-1.1.0/ssm_ps_template/discover.py
--rw-r--r--   0 root         (0) root         (0)     1558 2023-05-26 20:32:38.000000 ssm-ps-template-1.1.0/ssm_ps_template/render.py
--rw-r--r--   0 root         (0) root         (0)     3222 2023-05-26 20:32:38.000000 ssm-ps-template-1.1.0/ssm_ps_template/ssm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 20:32:47.698462 ssm-ps-template-1.1.0/ssm_ps_template.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8651 2023-05-26 20:32:47.000000 ssm-ps-template-1.1.0/ssm_ps_template.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      514 2023-05-26 20:32:47.000000 ssm-ps-template-1.1.0/ssm_ps_template.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 20:32:47.000000 ssm-ps-template-1.1.0/ssm_ps_template.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       66 2023-05-26 20:32:47.000000 ssm-ps-template-1.1.0/ssm_ps_template.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      246 2023-05-26 20:32:47.000000 ssm-ps-template-1.1.0/ssm_ps_template.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-05-26 20:32:47.000000 ssm-ps-template-1.1.0/ssm_ps_template.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 20:32:47.698462 ssm-ps-template-1.1.0/tests/
--rw-r--r--   0 root         (0) root         (0)     2324 2023-05-26 20:32:38.000000 ssm-ps-template-1.1.0/tests/test_config.py
--rw-r--r--   0 root         (0) root         (0)      405 2023-05-26 20:32:38.000000 ssm-ps-template-1.1.0/tests/test_discover.py
--rw-r--r--   0 root         (0) root         (0)     1593 2023-05-26 20:32:38.000000 ssm-ps-template-1.1.0/tests/test_render.py
--rw-r--r--   0 root         (0) root         (0)     4657 2023-05-26 20:32:38.000000 ssm-ps-template-1.1.0/tests/test_ssm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:59:47.532972 ssm-ps-template-2.0.0/
+-rw-r--r--   0 root         (0) root         (0)     1495 2023-06-01 19:59:36.000000 ssm-ps-template-2.0.0/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    10526 2023-06-01 19:59:47.532972 ssm-ps-template-2.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7890 2023-06-01 19:59:36.000000 ssm-ps-template-2.0.0/README.md
+-rw-r--r--   0 root         (0) root         (0)     1879 2023-06-01 19:59:36.000000 ssm-ps-template-2.0.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-01 19:59:47.532972 ssm-ps-template-2.0.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:59:47.528972 ssm-ps-template-2.0.0/ssm_ps_template/
+-rw-r--r--   0 root         (0) root         (0)      165 2023-06-01 19:59:36.000000 ssm-ps-template-2.0.0/ssm_ps_template/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3214 2023-06-01 19:59:36.000000 ssm-ps-template-2.0.0/ssm_ps_template/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     2364 2023-06-01 19:59:36.000000 ssm-ps-template-2.0.0/ssm_ps_template/config.py
+-rw-r--r--   0 root         (0) root         (0)     1825 2023-06-01 19:59:36.000000 ssm-ps-template-2.0.0/ssm_ps_template/discovery.py
+-rw-r--r--   0 root         (0) root         (0)     1575 2023-06-01 19:59:36.000000 ssm-ps-template-2.0.0/ssm_ps_template/render.py
+-rw-r--r--   0 root         (0) root         (0)     3352 2023-06-01 19:59:36.000000 ssm-ps-template-2.0.0/ssm_ps_template/ssm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:59:47.532972 ssm-ps-template-2.0.0/ssm_ps_template.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10526 2023-06-01 19:59:47.000000 ssm-ps-template-2.0.0/ssm_ps_template.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      535 2023-06-01 19:59:47.000000 ssm-ps-template-2.0.0/ssm_ps_template.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 19:59:47.000000 ssm-ps-template-2.0.0/ssm_ps_template.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       66 2023-06-01 19:59:47.000000 ssm-ps-template-2.0.0/ssm_ps_template.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      246 2023-06-01 19:59:47.000000 ssm-ps-template-2.0.0/ssm_ps_template.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-06-01 19:59:47.000000 ssm-ps-template-2.0.0/ssm_ps_template.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:59:47.532972 ssm-ps-template-2.0.0/tests/
+-rw-r--r--   0 root         (0) root         (0)     2833 2023-06-01 19:59:36.000000 ssm-ps-template-2.0.0/tests/test_config.py
+-rw-r--r--   0 root         (0) root         (0)      784 2023-06-01 19:59:36.000000 ssm-ps-template-2.0.0/tests/test_discovery.py
+-rw-r--r--   0 root         (0) root         (0)     1660 2023-06-01 19:59:36.000000 ssm-ps-template-2.0.0/tests/test_main.py
+-rw-r--r--   0 root         (0) root         (0)      733 2023-06-01 19:59:36.000000 ssm-ps-template-2.0.0/tests/test_render.py
+-rw-r--r--   0 root         (0) root         (0)     2972 2023-06-01 19:59:36.000000 ssm-ps-template-2.0.0/tests/test_ssm.py
```

### Comparing `ssm-ps-template-1.1.0/LICENSE.txt` & `ssm-ps-template-2.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-1.1.0/PKG-INFO` & `ssm-ps-template-2.0.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssm-ps-template
-Version: 1.1.0
+Version: 2.0.0
 Summary: CLI for rendering configuration templates with SSM Parameter Store as a data source
 Author-email: "Gavin M. Roy" <gavinmroy@gmail.com>
 License: Copyright (c) 2023 Gavin M. Roy
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification,
         are permitted provided that the following conditions are met:
@@ -31,15 +31,15 @@
         
 Project-URL: Homepage, https://github.com/gmr/ssm-ps-template
 Project-URL: Bug Tracker, https://github.com/gmr/ssm-ps-template/issues
 Keywords: aws,ssm,parameter store,templating
 Classifier: Topic :: Software Development
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Natural Language :: English
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Utilities
 Requires-Python: >=3.9
@@ -57,29 +57,86 @@
 
 ```bash
 pip install ssm-ps-template
 ```
 
 ## Templating
 
-The application uses [Jinja2](https://jinja.palletsprojects.com/en/3.1.x/) for the templating engine.
+The application uses [Jinja2](https://jinja.palletsprojects.com/en/3.1.x/) for the templating engine. All functionality available to Jinja2 templates by default are exposed in the application.
+
+### Getting Parameter Store Values
+
+The application exposes `get_parameter(name: str, default: typing.Optional[str] = None)` in templates to access the values in SSM Parameter Store.
+
+In the following example we assume there are Parameter Store values for the keys `/my-application/foo` and `/my-application/bar` and that the application is called with a prefix of `/my-appliction`:
+
+```yaml
+foo: {{ get_parameter('/my-application/foo'}}
+bar: {{ get_parameter('/my-application/bar'}}
+```
+Will render as:
+```yaml
+foo: bar
+baz: qux
+```
+
+Additionally, there is another function exposed `get_parameters_by_path(path: str, default: typing.Optional[dict] = None)` which will return a dictionary for the specified path.
+
+The following example will iterate over the results:
+```
+{% for key, value in get_parameters_by_path('settings/', {}).items() %}
+  {{ key }}: {{ value }}
+{% endfor %}
+```
+
+Or you can use a Jinja filter to convert them to YAML:
+```
+{{ get_parameters_by_path('settings/') | toyaml | indent(2, first=True) }}
+```
+
+For values in ParameterStore that are stored as `StringList`, they are automatically transformed as a list of strings. Given the following value:
+
+| Key                           | Value                            |
+|-------------------------------|----------------------------------|
+| `/my-application/connections` | `amqp://server1, amqp://server2` |
+
+And the following template:
+
+```
+Connections:
+{% for connection in get_parameter('/my-application/connections', []) %}
+  - {{ connection }}
+```
+
+The following would be rendered:
+
+```yaml
+Connections:
+  - amqp://server1
+  - amqp://server2
+```
+
+### Performance Considerations
+
+The parameter names are gathered in a pre-processing step to minimize calls to SSM Parameter Store.
 
 ## Configuration
 
 The configuration file provides the ability to specify multiple templates, override AWS configuration, and change logging levels:
 
 ### Top-Level Configuration Directives
 
-| Directive      | Description                                                                                                                      |
-|----------------|----------------------------------------------------------------------------------------------------------------------------------|
-| `templates`    | An array of template directives as detailed in the next table.                                                                   |
-| `endpoint_url` | Specify an endpoint URL to use to override the default URL used to contact SSM Parameter Store                                   |
-| `profile`      | Specify the AWS profile to use. If unspecified will default to the `AWS_DEFAULT_PROFILE` environment variable or is unspecified  |
-| `region`       | Specify the AWS region to use. If unspecified it will default to the `AWS_DEFAULT_REGION` environment variable or is unspecified |
-| `verbose`      | Turn debug logging on. Possible values are `true` and `false`                                                                    |
+| Directive             | Description                                                                                                                      |
+|-----------------------|----------------------------------------------------------------------------------------------------------------------------------|
+| `templates`           | An array of template directives as detailed in the next table.                                                                   |
+| `endpoint_url`        | Specify an endpoint URL to use to override the default URL used to contact SSM Parameter Store                                   |
+| `profile`             | Specify the AWS profile to use. If unspecified will default to the `AWS_DEFAULT_PROFILE` environment variable or is unspecified  |
+| `region`              | Specify the AWS region to use. If unspecified it will default to the `AWS_DEFAULT_REGION` environment variable or is unspecified |
+| `replace_underscores` | Replace underscores with dashes when asking for values from SSM Parameter Store                                                  |
+| `verbose`             | Turn debug logging on. Possible values are `true` and `false`                                                                    |
 
 ### Template Configuration Directives
 
 The `templates` directive in the configuration is an array of objects, defined by a `source` and `destination`.
 
 | Directive     | Description                                                                          |
 |---------------|--------------------------------------------------------------------------------------|
@@ -87,19 +144,21 @@
 | `destination` | The destination path to write the rendered template to                               |
 | `prefix`      | The prefix to prepend variables with if they do not start with a forward-slash (`/`) |
 
 ### Extended Templating Functionality
 
 In addition to the base functionality exposed by Jinja2, the following Python functions have been added:
 
-| Function   | Definition                                                                                                                                          |
-|------------|-----------------------------------------------------------------------------------------------------------------------------------------------------|
-| `urlparse` | The [`urllib.parse.urlparse`](https://docs.python.org/3/library/urllib.parse.html#urllib.parse.urlparse) function from the Python standard library. |
-| `parse_qs` | The [`urllib.parse.parse_qs`](https://docs.python.org/3/library/urllib.parse.html#urllib.parse.parse_qs) function from the Python standard library. |
-| `unquote`  | The [`urllib.parse.unquote`](https://docs.python.org/3/library/urllib.parse.html#urllib.parse.unquote) function from the Python standard library.   |
+| Function                 | Definition                                                                                                                                          |
+|--------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------|
+| `get_parameter`          | Get a string value from SSM Parameter Store                                                                                                         |
+| `get_parameters_by_path` | Get a dictionary value from SSM Parameter Store                                                                                                     |
+| `urlparse`               | The [`urllib.parse.urlparse`](https://docs.python.org/3/library/urllib.parse.html#urllib.parse.urlparse) function from the Python standard library. |
+| `parse_qs`               | The [`urllib.parse.parse_qs`](https://docs.python.org/3/library/urllib.parse.html#urllib.parse.parse_qs) function from the Python standard library. |
+| `unquote`                | The [`urllib.parse.unquote`](https://docs.python.org/3/library/urllib.parse.html#urllib.parse.unquote) function from the Python standard library.   |
 
 The following filters are added:
 
 | Filter   | Description                         |
 |----------|-------------------------------------|
 | `toyaml` | Converts a dictionary value to YAML |
 
@@ -124,37 +183,14 @@
     destination: /etc/postgresql/14/main/postgresql.conf
     prefix: /namespaced/application/postgres/
 profile: default
 region: us-east-1
 verbose: false
 ```
 
-## Path Based Dictionaries
-
-In more complex templates it's possible to need a dictionary of values from SSM instead of straight key/value usage.
-
-This is achieved by setting a variable to a key with a trailing slash (`/`).
-
-The following pattern will retrieve all keys under a path and return them as a nested dictionary with a `/` delimiter,
-and then iterate over the key/value pairs:
-
-```
-{% set values = settings/ %}
-{% for key, value in settings.items() %}
-  {{ key }}: {{ value }}
-{% endfor %}
-```
-
-Or to convert them to YAML:
-
-```
-settings: {% set values = settings/ %}
-{{ values | toyaml | indent(2, first=True) }}
-```
-
 ## Command Line Usage
 
 ```
 usage: ssm-ps-template [-h] [--aws-profile AWS_PROFILE] [--aws-region AWS_REGION] [--prefix PREFIX] [--verbose] config
 
 Templating for SSM Parameter Store
 
@@ -163,16 +199,16 @@
 
 optional arguments:
   -h, --help            show this help message and exit
   --aws-profile AWS_PROFILE
                         AWS Profile
   --aws-region AWS_REGION
                         AWS Region
-  --endpoint-url ENDPOINT_URL
+  --endpoint-url SSM_ENDPOINT_URL
                         Specify an endpoint URL to use when contacting SSM Parameter Store.
   --prefix PREFIX       Default SSM Key Prefix
   --replace-underscores
                         Replace underscores in variable names to dashes when looking for values in SSM
   --verbose
 ```
 Note that the default SSM prefix can also be set with the `PARAMS_PREFIX` environment variable and
-the endpoint URL setting cn be set with the `ENDPOINT_URL` environment variable.
+the endpoint URL setting cn be set with the `SSM_ENDPOINT_URL` environment variable.
```

### Comparing `ssm-ps-template-1.1.0/README.md` & `ssm-ps-template-2.0.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -8,29 +8,86 @@
 
 ```bash
 pip install ssm-ps-template
 ```
 
 ## Templating
 
-The application uses [Jinja2](https://jinja.palletsprojects.com/en/3.1.x/) for the templating engine.
+The application uses [Jinja2](https://jinja.palletsprojects.com/en/3.1.x/) for the templating engine. All functionality available to Jinja2 templates by default are exposed in the application.
+
+### Getting Parameter Store Values
+
+The application exposes `get_parameter(name: str, default: typing.Optional[str] = None)` in templates to access the values in SSM Parameter Store.
+
+In the following example we assume there are Parameter Store values for the keys `/my-application/foo` and `/my-application/bar` and that the application is called with a prefix of `/my-appliction`:
+
+```yaml
+foo: {{ get_parameter('/my-application/foo'}}
+bar: {{ get_parameter('/my-application/bar'}}
+```
+Will render as:
+```yaml
+foo: bar
+baz: qux
+```
+
+Additionally, there is another function exposed `get_parameters_by_path(path: str, default: typing.Optional[dict] = None)` which will return a dictionary for the specified path.
+
+The following example will iterate over the results:
+```
+{% for key, value in get_parameters_by_path('settings/', {}).items() %}
+  {{ key }}: {{ value }}
+{% endfor %}
+```
+
+Or you can use a Jinja filter to convert them to YAML:
+```
+{{ get_parameters_by_path('settings/') | toyaml | indent(2, first=True) }}
+```
+
+For values in ParameterStore that are stored as `StringList`, they are automatically transformed as a list of strings. Given the following value:
+
+| Key                           | Value                            |
+|-------------------------------|----------------------------------|
+| `/my-application/connections` | `amqp://server1, amqp://server2` |
+
+And the following template:
+
+```
+Connections:
+{% for connection in get_parameter('/my-application/connections', []) %}
+  - {{ connection }}
+```
+
+The following would be rendered:
+
+```yaml
+Connections:
+  - amqp://server1
+  - amqp://server2
+```
+
+### Performance Considerations
+
+The parameter names are gathered in a pre-processing step to minimize calls to SSM Parameter Store.
 
 ## Configuration
 
 The configuration file provides the ability to specify multiple templates, override AWS configuration, and change logging levels:
 
 ### Top-Level Configuration Directives
 
-| Directive      | Description                                                                                                                      |
-|----------------|----------------------------------------------------------------------------------------------------------------------------------|
-| `templates`    | An array of template directives as detailed in the next table.                                                                   |
-| `endpoint_url` | Specify an endpoint URL to use to override the default URL used to contact SSM Parameter Store                                   |
-| `profile`      | Specify the AWS profile to use. If unspecified will default to the `AWS_DEFAULT_PROFILE` environment variable or is unspecified  |
-| `region`       | Specify the AWS region to use. If unspecified it will default to the `AWS_DEFAULT_REGION` environment variable or is unspecified |
-| `verbose`      | Turn debug logging on. Possible values are `true` and `false`                                                                    |
+| Directive             | Description                                                                                                                      |
+|-----------------------|----------------------------------------------------------------------------------------------------------------------------------|
+| `templates`           | An array of template directives as detailed in the next table.                                                                   |
+| `endpoint_url`        | Specify an endpoint URL to use to override the default URL used to contact SSM Parameter Store                                   |
+| `profile`             | Specify the AWS profile to use. If unspecified will default to the `AWS_DEFAULT_PROFILE` environment variable or is unspecified  |
+| `region`              | Specify the AWS region to use. If unspecified it will default to the `AWS_DEFAULT_REGION` environment variable or is unspecified |
+| `replace_underscores` | Replace underscores with dashes when asking for values from SSM Parameter Store                                                  |
+| `verbose`             | Turn debug logging on. Possible values are `true` and `false`                                                                    |
 
 ### Template Configuration Directives
 
 The `templates` directive in the configuration is an array of objects, defined by a `source` and `destination`.
 
 | Directive     | Description                                                                          |
 |---------------|--------------------------------------------------------------------------------------|
@@ -38,19 +95,21 @@
 | `destination` | The destination path to write the rendered template to                               |
 | `prefix`      | The prefix to prepend variables with if they do not start with a forward-slash (`/`) |
 
 ### Extended Templating Functionality
 
 In addition to the base functionality exposed by Jinja2, the following Python functions have been added:
 
-| Function   | Definition                                                                                                                                          |
-|------------|-----------------------------------------------------------------------------------------------------------------------------------------------------|
-| `urlparse` | The [`urllib.parse.urlparse`](https://docs.python.org/3/library/urllib.parse.html#urllib.parse.urlparse) function from the Python standard library. |
-| `parse_qs` | The [`urllib.parse.parse_qs`](https://docs.python.org/3/library/urllib.parse.html#urllib.parse.parse_qs) function from the Python standard library. |
-| `unquote`  | The [`urllib.parse.unquote`](https://docs.python.org/3/library/urllib.parse.html#urllib.parse.unquote) function from the Python standard library.   |
+| Function                 | Definition                                                                                                                                          |
+|--------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------|
+| `get_parameter`          | Get a string value from SSM Parameter Store                                                                                                         |
+| `get_parameters_by_path` | Get a dictionary value from SSM Parameter Store                                                                                                     |
+| `urlparse`               | The [`urllib.parse.urlparse`](https://docs.python.org/3/library/urllib.parse.html#urllib.parse.urlparse) function from the Python standard library. |
+| `parse_qs`               | The [`urllib.parse.parse_qs`](https://docs.python.org/3/library/urllib.parse.html#urllib.parse.parse_qs) function from the Python standard library. |
+| `unquote`                | The [`urllib.parse.unquote`](https://docs.python.org/3/library/urllib.parse.html#urllib.parse.unquote) function from the Python standard library.   |
 
 The following filters are added:
 
 | Filter   | Description                         |
 |----------|-------------------------------------|
 | `toyaml` | Converts a dictionary value to YAML |
 
@@ -75,37 +134,14 @@
     destination: /etc/postgresql/14/main/postgresql.conf
     prefix: /namespaced/application/postgres/
 profile: default
 region: us-east-1
 verbose: false
 ```
 
-## Path Based Dictionaries
-
-In more complex templates it's possible to need a dictionary of values from SSM instead of straight key/value usage.
-
-This is achieved by setting a variable to a key with a trailing slash (`/`).
-
-The following pattern will retrieve all keys under a path and return them as a nested dictionary with a `/` delimiter,
-and then iterate over the key/value pairs:
-
-```
-{% set values = settings/ %}
-{% for key, value in settings.items() %}
-  {{ key }}: {{ value }}
-{% endfor %}
-```
-
-Or to convert them to YAML:
-
-```
-settings: {% set values = settings/ %}
-{{ values | toyaml | indent(2, first=True) }}
-```
-
 ## Command Line Usage
 
 ```
 usage: ssm-ps-template [-h] [--aws-profile AWS_PROFILE] [--aws-region AWS_REGION] [--prefix PREFIX] [--verbose] config
 
 Templating for SSM Parameter Store
 
@@ -114,16 +150,16 @@
 
 optional arguments:
   -h, --help            show this help message and exit
   --aws-profile AWS_PROFILE
                         AWS Profile
   --aws-region AWS_REGION
                         AWS Region
-  --endpoint-url ENDPOINT_URL
+  --endpoint-url SSM_ENDPOINT_URL
                         Specify an endpoint URL to use when contacting SSM Parameter Store.
   --prefix PREFIX       Default SSM Key Prefix
   --replace-underscores
                         Replace underscores in variable names to dashes when looking for values in SSM
   --verbose
 ```
 Note that the default SSM prefix can also be set with the `PARAMS_PREFIX` environment variable and
-the endpoint URL setting cn be set with the `ENDPOINT_URL` environment variable.
+the endpoint URL setting cn be set with the `SSM_ENDPOINT_URL` environment variable.
```

### Comparing `ssm-ps-template-1.1.0/pyproject.toml` & `ssm-ps-template-2.0.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [project]
 name = "ssm-ps-template"
-version = "1.1.0"
+version = "2.0.0"
 description = "CLI for rendering configuration templates with SSM Parameter Store as a data source"
 authors = [
     {name = "Gavin M. Roy", email="gavinmroy@gmail.com"}
 ]
 classifiers = [
     "Topic :: Software Development",
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python :: 3",
-    "Development Status :: 4 - Beta",
+    "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Intended Audience :: System Administrators",
     "Natural Language :: English",
     "Topic :: Text Processing",
     "Topic :: Utilities"
 ]
@@ -64,12 +64,12 @@
 [tool.coverage.html]
 directory = "build/coverage"
 
 [tool.coverage.xml]
 output = "build/coverage.xml"
 
 [tool.flake8]
-application-import-names = "ssm_ps_template"
+application-import-names = ["ssm_ps_template", "tests"]
 count = true
 exclude = ["bak", "build", "docs", "env"]
 import-order-style = "pycharm"
 ignore = ["RST306"]
```

### Comparing `ssm-ps-template-1.1.0/ssm_ps_template/__main__.py` & `ssm-ps-template-2.0.0/ssm_ps_template/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,80 +2,78 @@
 import logging
 import os
 import sys
 import time
 import typing
 from importlib import metadata
 
-from botocore import exceptions
-
-from ssm_ps_template import config, discover, render, ssm
+from ssm_ps_template import config, discovery, render, ssm
 
 LOGGER = logging.getLogger(__name__)
 
 
-def parse_cli_arguments() -> argparse.Namespace:
+def parse_cli_arguments(args: typing.Optional[typing.List[str]] = None) \
+        -> argparse.Namespace:
     parser = argparse.ArgumentParser(
         description='Templating for SSM Parameter Store')
-    parser.add_argument('--aws-profile', action='store', help='AWS Profile')
-    parser.add_argument('--aws-region', action='store', help='AWS Region')
+    parser.add_argument('--aws-profile', action='store', help='AWS Profile',
+                        default=os.environ.get('AWS_PROFILE'))
+    parser.add_argument('--aws-region', action='store', help='AWS Region',
+                        default=os.environ.get('AWS_REGION'))
     parser.add_argument('--endpoint-url', action='store',
                         help=('Specify an endpoint URL to use when contacting '
                               'SSM Parameter Store.'),
-                        default=os.environ.get('ENDPOINT_URL'))
+                        default=os.environ.get('SSM_ENDPOINT_URL'))
     parser.add_argument('--prefix', action='store',
                         help='Default SSM Key Prefix',
                         default=os.environ.get('PARAMS_PREFIX', ''))
     parser.add_argument('--replace-underscores', action='store_true',
                         help=('Replace underscores in variable names to dashes'
                               ' when looking for values in SSM'))
     parser.add_argument('--verbose', action='store_true')
     parser.add_argument('config', type=config.configuration_file, nargs=1)
-    return parser.parse_args()
+    return parser.parse_args(args)
 
 
 def render_templates(args: argparse.Namespace) -> typing.NoReturn:
     parameter_store = ssm.ParameterStore(
         profile=args.aws_profile or args.config[0].profile,
         region=args.aws_region or args.config[0].region,
         endpoint_url=args.endpoint_url or args.config[0].endpoint_url)
 
-    start_time = time.time()
     for template in args.config[0].templates:
         if not args.prefix and not template.prefix:
             LOGGER.error('The prefix for %s must not be empty.',
                          template.source)
             sys.exit(1)
 
-        prefix = args.prefix or template.prefix
-        if not prefix.endswith('/'):
-            prefix = f'{args.prefix}/'
+        start_time = time.time()
+
+        prefix = (args.prefix or template.prefix).rstrip('/')
 
-        variable_discovery = discover.Variables(template.source)
-        variables = sorted(variable_discovery.discover())
+        variable_discovery = discovery.VariableDiscovery(template.source)
+        variables = variable_discovery.discover()
 
         try:
             values = parameter_store.fetch_variables(
                 variables, prefix, args.replace_underscores)
-        except (exceptions.ClientError,
-                exceptions.UnauthorizedSSOTokenError) as err:
+        except ssm.SSMClientException as err:
             LOGGER.error('Error fetching parameters: %s', err)
             sys.exit(2)
 
-        renderer = render.Renderer(source=template.source, variables=variables)
+        renderer = render.Renderer(source=template.source)
         with template.destination.open('w') as handle:
             handle.write(renderer.render(values))
 
         LOGGER.info('Rendered %s in %0.2f seconds', template.destination,
                     time.time() - start_time)
 
 
-def main():
+def main():  # pragma: no cover
     args = parse_cli_arguments()
-
     verbose = args.config[0].verbose or args.verbose
     logging.basicConfig(level=logging.DEBUG if verbose else logging.INFO)
     for logger in ['boto3', 'botocore', 'urllib3']:
         logging.getLogger(logger).setLevel(logging.INFO)
 
     LOGGER.info('ssm-ps-template v%s', metadata.version('ssm-ps-template'))
     render_templates(args)
```

### Comparing `ssm-ps-template-1.1.0/ssm_ps_template/config.py` & `ssm-ps-template-2.0.0/ssm_ps_template/config.py`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-1.1.0/ssm_ps_template.egg-info/PKG-INFO` & `ssm-ps-template-2.0.0/ssm_ps_template.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssm-ps-template
-Version: 1.1.0
+Version: 2.0.0
 Summary: CLI for rendering configuration templates with SSM Parameter Store as a data source
 Author-email: "Gavin M. Roy" <gavinmroy@gmail.com>
 License: Copyright (c) 2023 Gavin M. Roy
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification,
         are permitted provided that the following conditions are met:
@@ -31,15 +31,15 @@
         
 Project-URL: Homepage, https://github.com/gmr/ssm-ps-template
 Project-URL: Bug Tracker, https://github.com/gmr/ssm-ps-template/issues
 Keywords: aws,ssm,parameter store,templating
 Classifier: Topic :: Software Development
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Natural Language :: English
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Utilities
 Requires-Python: >=3.9
@@ -57,29 +57,86 @@
 
 ```bash
 pip install ssm-ps-template
 ```
 
 ## Templating
 
-The application uses [Jinja2](https://jinja.palletsprojects.com/en/3.1.x/) for the templating engine.
+The application uses [Jinja2](https://jinja.palletsprojects.com/en/3.1.x/) for the templating engine. All functionality available to Jinja2 templates by default are exposed in the application.
+
+### Getting Parameter Store Values
+
+The application exposes `get_parameter(name: str, default: typing.Optional[str] = None)` in templates to access the values in SSM Parameter Store.
+
+In the following example we assume there are Parameter Store values for the keys `/my-application/foo` and `/my-application/bar` and that the application is called with a prefix of `/my-appliction`:
+
+```yaml
+foo: {{ get_parameter('/my-application/foo'}}
+bar: {{ get_parameter('/my-application/bar'}}
+```
+Will render as:
+```yaml
+foo: bar
+baz: qux
+```
+
+Additionally, there is another function exposed `get_parameters_by_path(path: str, default: typing.Optional[dict] = None)` which will return a dictionary for the specified path.
+
+The following example will iterate over the results:
+```
+{% for key, value in get_parameters_by_path('settings/', {}).items() %}
+  {{ key }}: {{ value }}
+{% endfor %}
+```
+
+Or you can use a Jinja filter to convert them to YAML:
+```
+{{ get_parameters_by_path('settings/') | toyaml | indent(2, first=True) }}
+```
+
+For values in ParameterStore that are stored as `StringList`, they are automatically transformed as a list of strings. Given the following value:
+
+| Key                           | Value                            |
+|-------------------------------|----------------------------------|
+| `/my-application/connections` | `amqp://server1, amqp://server2` |
+
+And the following template:
+
+```
+Connections:
+{% for connection in get_parameter('/my-application/connections', []) %}
+  - {{ connection }}
+```
+
+The following would be rendered:
+
+```yaml
+Connections:
+  - amqp://server1
+  - amqp://server2
+```
+
+### Performance Considerations
+
+The parameter names are gathered in a pre-processing step to minimize calls to SSM Parameter Store.
 
 ## Configuration
 
 The configuration file provides the ability to specify multiple templates, override AWS configuration, and change logging levels:
 
 ### Top-Level Configuration Directives
 
-| Directive      | Description                                                                                                                      |
-|----------------|----------------------------------------------------------------------------------------------------------------------------------|
-| `templates`    | An array of template directives as detailed in the next table.                                                                   |
-| `endpoint_url` | Specify an endpoint URL to use to override the default URL used to contact SSM Parameter Store                                   |
-| `profile`      | Specify the AWS profile to use. If unspecified will default to the `AWS_DEFAULT_PROFILE` environment variable or is unspecified  |
-| `region`       | Specify the AWS region to use. If unspecified it will default to the `AWS_DEFAULT_REGION` environment variable or is unspecified |
-| `verbose`      | Turn debug logging on. Possible values are `true` and `false`                                                                    |
+| Directive             | Description                                                                                                                      |
+|-----------------------|----------------------------------------------------------------------------------------------------------------------------------|
+| `templates`           | An array of template directives as detailed in the next table.                                                                   |
+| `endpoint_url`        | Specify an endpoint URL to use to override the default URL used to contact SSM Parameter Store                                   |
+| `profile`             | Specify the AWS profile to use. If unspecified will default to the `AWS_DEFAULT_PROFILE` environment variable or is unspecified  |
+| `region`              | Specify the AWS region to use. If unspecified it will default to the `AWS_DEFAULT_REGION` environment variable or is unspecified |
+| `replace_underscores` | Replace underscores with dashes when asking for values from SSM Parameter Store                                                  |
+| `verbose`             | Turn debug logging on. Possible values are `true` and `false`                                                                    |
 
 ### Template Configuration Directives
 
 The `templates` directive in the configuration is an array of objects, defined by a `source` and `destination`.
 
 | Directive     | Description                                                                          |
 |---------------|--------------------------------------------------------------------------------------|
@@ -87,19 +144,21 @@
 | `destination` | The destination path to write the rendered template to                               |
 | `prefix`      | The prefix to prepend variables with if they do not start with a forward-slash (`/`) |
 
 ### Extended Templating Functionality
 
 In addition to the base functionality exposed by Jinja2, the following Python functions have been added:
 
-| Function   | Definition                                                                                                                                          |
-|------------|-----------------------------------------------------------------------------------------------------------------------------------------------------|
-| `urlparse` | The [`urllib.parse.urlparse`](https://docs.python.org/3/library/urllib.parse.html#urllib.parse.urlparse) function from the Python standard library. |
-| `parse_qs` | The [`urllib.parse.parse_qs`](https://docs.python.org/3/library/urllib.parse.html#urllib.parse.parse_qs) function from the Python standard library. |
-| `unquote`  | The [`urllib.parse.unquote`](https://docs.python.org/3/library/urllib.parse.html#urllib.parse.unquote) function from the Python standard library.   |
+| Function                 | Definition                                                                                                                                          |
+|--------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------|
+| `get_parameter`          | Get a string value from SSM Parameter Store                                                                                                         |
+| `get_parameters_by_path` | Get a dictionary value from SSM Parameter Store                                                                                                     |
+| `urlparse`               | The [`urllib.parse.urlparse`](https://docs.python.org/3/library/urllib.parse.html#urllib.parse.urlparse) function from the Python standard library. |
+| `parse_qs`               | The [`urllib.parse.parse_qs`](https://docs.python.org/3/library/urllib.parse.html#urllib.parse.parse_qs) function from the Python standard library. |
+| `unquote`                | The [`urllib.parse.unquote`](https://docs.python.org/3/library/urllib.parse.html#urllib.parse.unquote) function from the Python standard library.   |
 
 The following filters are added:
 
 | Filter   | Description                         |
 |----------|-------------------------------------|
 | `toyaml` | Converts a dictionary value to YAML |
 
@@ -124,37 +183,14 @@
     destination: /etc/postgresql/14/main/postgresql.conf
     prefix: /namespaced/application/postgres/
 profile: default
 region: us-east-1
 verbose: false
 ```
 
-## Path Based Dictionaries
-
-In more complex templates it's possible to need a dictionary of values from SSM instead of straight key/value usage.
-
-This is achieved by setting a variable to a key with a trailing slash (`/`).
-
-The following pattern will retrieve all keys under a path and return them as a nested dictionary with a `/` delimiter,
-and then iterate over the key/value pairs:
-
-```
-{% set values = settings/ %}
-{% for key, value in settings.items() %}
-  {{ key }}: {{ value }}
-{% endfor %}
-```
-
-Or to convert them to YAML:
-
-```
-settings: {% set values = settings/ %}
-{{ values | toyaml | indent(2, first=True) }}
-```
-
 ## Command Line Usage
 
 ```
 usage: ssm-ps-template [-h] [--aws-profile AWS_PROFILE] [--aws-region AWS_REGION] [--prefix PREFIX] [--verbose] config
 
 Templating for SSM Parameter Store
 
@@ -163,16 +199,16 @@
 
 optional arguments:
   -h, --help            show this help message and exit
   --aws-profile AWS_PROFILE
                         AWS Profile
   --aws-region AWS_REGION
                         AWS Region
-  --endpoint-url ENDPOINT_URL
+  --endpoint-url SSM_ENDPOINT_URL
                         Specify an endpoint URL to use when contacting SSM Parameter Store.
   --prefix PREFIX       Default SSM Key Prefix
   --replace-underscores
                         Replace underscores in variable names to dashes when looking for values in SSM
   --verbose
 ```
 Note that the default SSM prefix can also be set with the `PARAMS_PREFIX` environment variable and
-the endpoint URL setting cn be set with the `ENDPOINT_URL` environment variable.
+the endpoint URL setting cn be set with the `SSM_ENDPOINT_URL` environment variable.
```

### Comparing `ssm-ps-template-1.1.0/ssm_ps_template.egg-info/SOURCES.txt` & `ssm-ps-template-2.0.0/ssm_ps_template.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 LICENSE.txt
 README.md
 pyproject.toml
 ssm_ps_template/__init__.py
 ssm_ps_template/__main__.py
 ssm_ps_template/config.py
-ssm_ps_template/discover.py
+ssm_ps_template/discovery.py
 ssm_ps_template/render.py
 ssm_ps_template/ssm.py
 ssm_ps_template.egg-info/PKG-INFO
 ssm_ps_template.egg-info/SOURCES.txt
 ssm_ps_template.egg-info/dependency_links.txt
 ssm_ps_template.egg-info/entry_points.txt
 ssm_ps_template.egg-info/requires.txt
 ssm_ps_template.egg-info/top_level.txt
 tests/test_config.py
-tests/test_discover.py
+tests/test_discovery.py
+tests/test_main.py
 tests/test_render.py
 tests/test_ssm.py
```

