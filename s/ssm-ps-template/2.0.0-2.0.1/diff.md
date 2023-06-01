# Comparing `tmp/ssm-ps-template-2.0.0.tar.gz` & `tmp/ssm-ps-template-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssm-ps-template-2.0.0.tar", last modified: Thu Jun  1 19:59:47 2023, max compression
+gzip compressed data, was "ssm-ps-template-2.0.1.tar", last modified: Thu Jun  1 21:28:27 2023, max compression
```

## Comparing `ssm-ps-template-2.0.0.tar` & `ssm-ps-template-2.0.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:59:47.532972 ssm-ps-template-2.0.0/
--rw-r--r--   0 root         (0) root         (0)     1495 2023-06-01 19:59:36.000000 ssm-ps-template-2.0.0/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    10526 2023-06-01 19:59:47.532972 ssm-ps-template-2.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7890 2023-06-01 19:59:36.000000 ssm-ps-template-2.0.0/README.md
--rw-r--r--   0 root         (0) root         (0)     1879 2023-06-01 19:59:36.000000 ssm-ps-template-2.0.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-01 19:59:47.532972 ssm-ps-template-2.0.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:59:47.528972 ssm-ps-template-2.0.0/ssm_ps_template/
--rw-r--r--   0 root         (0) root         (0)      165 2023-06-01 19:59:36.000000 ssm-ps-template-2.0.0/ssm_ps_template/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3214 2023-06-01 19:59:36.000000 ssm-ps-template-2.0.0/ssm_ps_template/__main__.py
--rw-r--r--   0 root         (0) root         (0)     2364 2023-06-01 19:59:36.000000 ssm-ps-template-2.0.0/ssm_ps_template/config.py
--rw-r--r--   0 root         (0) root         (0)     1825 2023-06-01 19:59:36.000000 ssm-ps-template-2.0.0/ssm_ps_template/discovery.py
--rw-r--r--   0 root         (0) root         (0)     1575 2023-06-01 19:59:36.000000 ssm-ps-template-2.0.0/ssm_ps_template/render.py
--rw-r--r--   0 root         (0) root         (0)     3352 2023-06-01 19:59:36.000000 ssm-ps-template-2.0.0/ssm_ps_template/ssm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:59:47.532972 ssm-ps-template-2.0.0/ssm_ps_template.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10526 2023-06-01 19:59:47.000000 ssm-ps-template-2.0.0/ssm_ps_template.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      535 2023-06-01 19:59:47.000000 ssm-ps-template-2.0.0/ssm_ps_template.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 19:59:47.000000 ssm-ps-template-2.0.0/ssm_ps_template.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       66 2023-06-01 19:59:47.000000 ssm-ps-template-2.0.0/ssm_ps_template.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      246 2023-06-01 19:59:47.000000 ssm-ps-template-2.0.0/ssm_ps_template.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-06-01 19:59:47.000000 ssm-ps-template-2.0.0/ssm_ps_template.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:59:47.532972 ssm-ps-template-2.0.0/tests/
--rw-r--r--   0 root         (0) root         (0)     2833 2023-06-01 19:59:36.000000 ssm-ps-template-2.0.0/tests/test_config.py
--rw-r--r--   0 root         (0) root         (0)      784 2023-06-01 19:59:36.000000 ssm-ps-template-2.0.0/tests/test_discovery.py
--rw-r--r--   0 root         (0) root         (0)     1660 2023-06-01 19:59:36.000000 ssm-ps-template-2.0.0/tests/test_main.py
--rw-r--r--   0 root         (0) root         (0)      733 2023-06-01 19:59:36.000000 ssm-ps-template-2.0.0/tests/test_render.py
--rw-r--r--   0 root         (0) root         (0)     2972 2023-06-01 19:59:36.000000 ssm-ps-template-2.0.0/tests/test_ssm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 21:28:27.425444 ssm-ps-template-2.0.1/
+-rw-r--r--   0 root         (0) root         (0)     1495 2023-06-01 21:28:14.000000 ssm-ps-template-2.0.1/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    11045 2023-06-01 21:28:27.425444 ssm-ps-template-2.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8409 2023-06-01 21:28:14.000000 ssm-ps-template-2.0.1/README.md
+-rw-r--r--   0 root         (0) root         (0)     1879 2023-06-01 21:28:14.000000 ssm-ps-template-2.0.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-01 21:28:27.425444 ssm-ps-template-2.0.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 21:28:27.421444 ssm-ps-template-2.0.1/ssm_ps_template/
+-rw-r--r--   0 root         (0) root         (0)      165 2023-06-01 21:28:14.000000 ssm-ps-template-2.0.1/ssm_ps_template/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3030 2023-06-01 21:28:14.000000 ssm-ps-template-2.0.1/ssm_ps_template/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     2364 2023-06-01 21:28:14.000000 ssm-ps-template-2.0.1/ssm_ps_template/config.py
+-rw-r--r--   0 root         (0) root         (0)     1825 2023-06-01 21:28:14.000000 ssm-ps-template-2.0.1/ssm_ps_template/discovery.py
+-rw-r--r--   0 root         (0) root         (0)     1575 2023-06-01 21:28:14.000000 ssm-ps-template-2.0.1/ssm_ps_template/render.py
+-rw-r--r--   0 root         (0) root         (0)     3388 2023-06-01 21:28:14.000000 ssm-ps-template-2.0.1/ssm_ps_template/ssm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 21:28:27.421444 ssm-ps-template-2.0.1/ssm_ps_template.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11045 2023-06-01 21:28:27.000000 ssm-ps-template-2.0.1/ssm_ps_template.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      535 2023-06-01 21:28:27.000000 ssm-ps-template-2.0.1/ssm_ps_template.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 21:28:27.000000 ssm-ps-template-2.0.1/ssm_ps_template.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       66 2023-06-01 21:28:27.000000 ssm-ps-template-2.0.1/ssm_ps_template.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      246 2023-06-01 21:28:27.000000 ssm-ps-template-2.0.1/ssm_ps_template.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-06-01 21:28:27.000000 ssm-ps-template-2.0.1/ssm_ps_template.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 21:28:27.421444 ssm-ps-template-2.0.1/tests/
+-rw-r--r--   0 root         (0) root         (0)     2833 2023-06-01 21:28:14.000000 ssm-ps-template-2.0.1/tests/test_config.py
+-rw-r--r--   0 root         (0) root         (0)      784 2023-06-01 21:28:14.000000 ssm-ps-template-2.0.1/tests/test_discovery.py
+-rw-r--r--   0 root         (0) root         (0)     1332 2023-06-01 21:28:14.000000 ssm-ps-template-2.0.1/tests/test_main.py
+-rw-r--r--   0 root         (0) root         (0)      733 2023-06-01 21:28:14.000000 ssm-ps-template-2.0.1/tests/test_render.py
+-rw-r--r--   0 root         (0) root         (0)     3119 2023-06-01 21:28:14.000000 ssm-ps-template-2.0.1/tests/test_ssm.py
```

### Comparing `ssm-ps-template-2.0.0/LICENSE.txt` & `ssm-ps-template-2.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-2.0.0/PKG-INFO` & `ssm-ps-template-2.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssm-ps-template
-Version: 2.0.0
+Version: 2.0.1
 Summary: CLI for rendering configuration templates with SSM Parameter Store as a data source
 Author-email: "Gavin M. Roy" <gavinmroy@gmail.com>
 License: Copyright (c) 2023 Gavin M. Roy
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification,
         are permitted provided that the following conditions are met:
@@ -59,14 +59,22 @@
 pip install ssm-ps-template
 ```
 
 ## Templating
 
 The application uses [Jinja2](https://jinja.palletsprojects.com/en/3.1.x/) for the templating engine. All functionality available to Jinja2 templates by default are exposed in the application.
 
+### Using Prefixes
+
+The application has a default prefix of `/` that is prepended to parameter names that do not start with a leading slash (`/`).
+
+This functionality allows you to group your variables under a path prefix like `/my-application/settings` and then only refer to the individual key values like `password` instead of referencing the full path of `/my-application/settings/password`.
+
+If you reference a parameter name with a leading slash it will not prepend the prefix to the parameter name.
+
 ### Getting Parameter Store Values
 
 The application exposes `get_parameter(name: str, default: typing.Optional[str] = None)` in templates to access the values in SSM Parameter Store.
 
 In the following example we assume there are Parameter Store values for the keys `/my-application/foo` and `/my-application/bar` and that the application is called with a prefix of `/my-appliction`:
 
 ```yaml
@@ -78,34 +86,34 @@
 foo: bar
 baz: qux
 ```
 
 Additionally, there is another function exposed `get_parameters_by_path(path: str, default: typing.Optional[dict] = None)` which will return a dictionary for the specified path.
 
 The following example will iterate over the results:
-```
+```yaml
 {% for key, value in get_parameters_by_path('settings/', {}).items() %}
   {{ key }}: {{ value }}
 {% endfor %}
 ```
 
 Or you can use a Jinja filter to convert them to YAML:
-```
+```yaml
 {{ get_parameters_by_path('settings/') | toyaml | indent(2, first=True) }}
 ```
 
 For values in ParameterStore that are stored as `StringList`, they are automatically transformed as a list of strings. Given the following value:
 
 | Key                           | Value                            |
 |-------------------------------|----------------------------------|
 | `/my-application/connections` | `amqp://server1, amqp://server2` |
 
 And the following template:
 
-```
+```yaml
 Connections:
 {% for connection in get_parameter('/my-application/connections', []) %}
   - {{ connection }}
 ```
 
 The following would be rendered:
```

### Comparing `ssm-ps-template-2.0.0/README.md` & `ssm-ps-template-2.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,22 @@
 pip install ssm-ps-template
 ```
 
 ## Templating
 
 The application uses [Jinja2](https://jinja.palletsprojects.com/en/3.1.x/) for the templating engine. All functionality available to Jinja2 templates by default are exposed in the application.
 
+### Using Prefixes
+
+The application has a default prefix of `/` that is prepended to parameter names that do not start with a leading slash (`/`).
+
+This functionality allows you to group your variables under a path prefix like `/my-application/settings` and then only refer to the individual key values like `password` instead of referencing the full path of `/my-application/settings/password`.
+
+If you reference a parameter name with a leading slash it will not prepend the prefix to the parameter name.
+
 ### Getting Parameter Store Values
 
 The application exposes `get_parameter(name: str, default: typing.Optional[str] = None)` in templates to access the values in SSM Parameter Store.
 
 In the following example we assume there are Parameter Store values for the keys `/my-application/foo` and `/my-application/bar` and that the application is called with a prefix of `/my-appliction`:
 
 ```yaml
@@ -29,34 +37,34 @@
 foo: bar
 baz: qux
 ```
 
 Additionally, there is another function exposed `get_parameters_by_path(path: str, default: typing.Optional[dict] = None)` which will return a dictionary for the specified path.
 
 The following example will iterate over the results:
-```
+```yaml
 {% for key, value in get_parameters_by_path('settings/', {}).items() %}
   {{ key }}: {{ value }}
 {% endfor %}
 ```
 
 Or you can use a Jinja filter to convert them to YAML:
-```
+```yaml
 {{ get_parameters_by_path('settings/') | toyaml | indent(2, first=True) }}
 ```
 
 For values in ParameterStore that are stored as `StringList`, they are automatically transformed as a list of strings. Given the following value:
 
 | Key                           | Value                            |
 |-------------------------------|----------------------------------|
 | `/my-application/connections` | `amqp://server1, amqp://server2` |
 
 And the following template:
 
-```
+```yaml
 Connections:
 {% for connection in get_parameter('/my-application/connections', []) %}
   - {{ connection }}
 ```
 
 The following would be rendered:
```

### Comparing `ssm-ps-template-2.0.0/pyproject.toml` & `ssm-ps-template-2.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ssm-ps-template"
-version = "2.0.0"
+version = "2.0.1"
 description = "CLI for rendering configuration templates with SSM Parameter Store as a data source"
 authors = [
     {name = "Gavin M. Roy", email="gavinmroy@gmail.com"}
 ]
 classifiers = [
     "Topic :: Software Development",
     "License :: OSI Approved :: BSD License",
```

### Comparing `ssm-ps-template-2.0.0/ssm_ps_template/__main__.py` & `ssm-ps-template-2.0.1/ssm_ps_template/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
                         default=os.environ.get('AWS_REGION'))
     parser.add_argument('--endpoint-url', action='store',
                         help=('Specify an endpoint URL to use when contacting '
                               'SSM Parameter Store.'),
                         default=os.environ.get('SSM_ENDPOINT_URL'))
     parser.add_argument('--prefix', action='store',
                         help='Default SSM Key Prefix',
-                        default=os.environ.get('PARAMS_PREFIX', ''))
+                        default=os.environ.get('PARAMS_PREFIX', '/'))
     parser.add_argument('--replace-underscores', action='store_true',
                         help=('Replace underscores in variable names to dashes'
                               ' when looking for values in SSM'))
     parser.add_argument('--verbose', action='store_true')
     parser.add_argument('config', type=config.configuration_file, nargs=1)
     return parser.parse_args(args)
 
@@ -37,32 +37,26 @@
 def render_templates(args: argparse.Namespace) -> typing.NoReturn:
     parameter_store = ssm.ParameterStore(
         profile=args.aws_profile or args.config[0].profile,
         region=args.aws_region or args.config[0].region,
         endpoint_url=args.endpoint_url or args.config[0].endpoint_url)
 
     for template in args.config[0].templates:
-        if not args.prefix and not template.prefix:
-            LOGGER.error('The prefix for %s must not be empty.',
-                         template.source)
-            sys.exit(1)
-
         start_time = time.time()
-
         prefix = (args.prefix or template.prefix).rstrip('/')
 
         variable_discovery = discovery.VariableDiscovery(template.source)
         variables = variable_discovery.discover()
 
         try:
             values = parameter_store.fetch_variables(
                 variables, prefix, args.replace_underscores)
         except ssm.SSMClientException as err:
             LOGGER.error('Error fetching parameters: %s', err)
-            sys.exit(2)
+            sys.exit(1)
 
         renderer = render.Renderer(source=template.source)
         with template.destination.open('w') as handle:
             handle.write(renderer.render(values))
 
         LOGGER.info('Rendered %s in %0.2f seconds', template.destination,
                     time.time() - start_time)
```

### Comparing `ssm-ps-template-2.0.0/ssm_ps_template/config.py` & `ssm-ps-template-2.0.1/ssm_ps_template/config.py`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-2.0.0/ssm_ps_template/discovery.py` & `ssm-ps-template-2.0.1/ssm_ps_template/discovery.py`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-2.0.0/ssm_ps_template/render.py` & `ssm-ps-template-2.0.1/ssm_ps_template/render.py`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-2.0.0/ssm_ps_template/ssm.py` & `ssm-ps-template-2.0.1/ssm_ps_template/ssm.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
     def _build_names(variables: set,
                      prefix: str,
                      replace_underscores: bool) \
             -> typing.Tuple[typing.List[str], typing.Dict[str, str]]:
         names, name_map = [], {}
         for param in variables:
             value = param.replace('_', '-') if replace_underscores else param
-            name = f'{prefix}/{value}'
+            name = value if value.startswith('/') else f'{prefix}/{value}'
             name_map[name] = param
             names.append(name)
         return names, name_map
 
     @staticmethod
     def _parameter_value(parameter: dict) \
             -> typing.Union[str, typing.List[str]]:
```

### Comparing `ssm-ps-template-2.0.0/ssm_ps_template.egg-info/PKG-INFO` & `ssm-ps-template-2.0.1/ssm_ps_template.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssm-ps-template
-Version: 2.0.0
+Version: 2.0.1
 Summary: CLI for rendering configuration templates with SSM Parameter Store as a data source
 Author-email: "Gavin M. Roy" <gavinmroy@gmail.com>
 License: Copyright (c) 2023 Gavin M. Roy
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification,
         are permitted provided that the following conditions are met:
@@ -59,14 +59,22 @@
 pip install ssm-ps-template
 ```
 
 ## Templating
 
 The application uses [Jinja2](https://jinja.palletsprojects.com/en/3.1.x/) for the templating engine. All functionality available to Jinja2 templates by default are exposed in the application.
 
+### Using Prefixes
+
+The application has a default prefix of `/` that is prepended to parameter names that do not start with a leading slash (`/`).
+
+This functionality allows you to group your variables under a path prefix like `/my-application/settings` and then only refer to the individual key values like `password` instead of referencing the full path of `/my-application/settings/password`.
+
+If you reference a parameter name with a leading slash it will not prepend the prefix to the parameter name.
+
 ### Getting Parameter Store Values
 
 The application exposes `get_parameter(name: str, default: typing.Optional[str] = None)` in templates to access the values in SSM Parameter Store.
 
 In the following example we assume there are Parameter Store values for the keys `/my-application/foo` and `/my-application/bar` and that the application is called with a prefix of `/my-appliction`:
 
 ```yaml
@@ -78,34 +86,34 @@
 foo: bar
 baz: qux
 ```
 
 Additionally, there is another function exposed `get_parameters_by_path(path: str, default: typing.Optional[dict] = None)` which will return a dictionary for the specified path.
 
 The following example will iterate over the results:
-```
+```yaml
 {% for key, value in get_parameters_by_path('settings/', {}).items() %}
   {{ key }}: {{ value }}
 {% endfor %}
 ```
 
 Or you can use a Jinja filter to convert them to YAML:
-```
+```yaml
 {{ get_parameters_by_path('settings/') | toyaml | indent(2, first=True) }}
 ```
 
 For values in ParameterStore that are stored as `StringList`, they are automatically transformed as a list of strings. Given the following value:
 
 | Key                           | Value                            |
 |-------------------------------|----------------------------------|
 | `/my-application/connections` | `amqp://server1, amqp://server2` |
 
 And the following template:
 
-```
+```yaml
 Connections:
 {% for connection in get_parameter('/my-application/connections', []) %}
   - {{ connection }}
 ```
 
 The following would be rendered:
```

### Comparing `ssm-ps-template-2.0.0/ssm_ps_template.egg-info/SOURCES.txt` & `ssm-ps-template-2.0.1/ssm_ps_template.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-2.0.0/tests/test_config.py` & `ssm-ps-template-2.0.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-2.0.0/tests/test_discovery.py` & `ssm-ps-template-2.0.1/tests/test_discovery.py`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-2.0.0/tests/test_main.py` & `ssm-ps-template-2.0.1/tests/test_main.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,25 +23,18 @@
             result = handle.read()
 
         with (utils.TEST_DATA_PATH / 'main/expectation.yaml').open() as handle:
             expectation = handle.read()
 
         self.assertEqual(result.strip(), expectation.strip())
 
-    def test_render_templates_exists_without_prefix(self):
-        args = __main__.parse_cli_arguments([
-            str(utils.TEST_DATA_PATH / 'main/config.toml')])
-        with self.assertRaises(SystemExit) as system_exit:
-            __main__.render_templates(args)
-        self.assertEqual(str(system_exit.exception), '1')
-
     def test_ssm_error_exits(self):
         args = __main__.parse_cli_arguments([
             '--prefix', '/my-application',
             str(utils.TEST_DATA_PATH / 'main/config.toml')])
 
         with mock.patch(
                 'ssm_ps_template.ssm.ParameterStore.fetch_variables') as func:
             func.side_effect = ssm.SSMClientException('Mock Error')
             with self.assertRaises(SystemExit) as system_exit:
                 __main__.render_templates(args)
-            self.assertEqual(str(system_exit.exception), '2')
+            self.assertEqual(str(system_exit.exception), '1')
```

### Comparing `ssm-ps-template-2.0.0/tests/test_render.py` & `ssm-ps-template-2.0.1/tests/test_render.py`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-2.0.0/tests/test_ssm.py` & `ssm-ps-template-2.0.1/tests/test_ssm.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,26 +46,28 @@
             dataclasses.asdict(result), dataclasses.asdict(expectation))
 
     def test_fetch_variables_with_dashes(self):
         values = {
             '/foo/bar/baz': str(uuid.uuid4()),
             '/foo/bar/corgie-qux': str(uuid.uuid4()),
             '/foo/bar/app-settings/value1': str(uuid.uuid4()),
-            '/foo/bar/app-settings/value2': str(uuid.uuid4())
+            '/foo/bar/app-settings/value2': str(uuid.uuid4()),
+            '/other-prefix/value': str(uuid.uuid4())
         }
         self.put_parameters(values)
 
         variables = discovery.Variables(
-            {'baz', 'corgie_qux'}, {'app_settings/'})
+            {'baz', 'corgie_qux', '/other-prefix/value'}, {'app_settings/'})
         result = self.ssm.fetch_variables(variables, '/foo/bar', True)
 
         expectation = ssm.Values(
             {
                 'baz': values['/foo/bar/baz'],
-                'corgie_qux': values['/foo/bar/corgie-qux']
+                'corgie_qux': values['/foo/bar/corgie-qux'],
+                '/other-prefix/value': values['/other-prefix/value']
             },
             {
                 'app_settings/': {
                     'value1': values['/foo/bar/app-settings/value1'],
                     'value2': values['/foo/bar/app-settings/value2']
                 }
             })
```

