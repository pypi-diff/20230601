# Comparing `tmp/omnata_cli-0.1.0.tar.gz` & `tmp/omnata_cli-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omnata_cli-0.1.0.tar", max compression
+gzip compressed data, was "omnata_cli-0.1.1.tar", max compression
```

## Comparing `omnata_cli-0.1.0.tar` & `omnata_cli-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    26526 2023-06-01 03:24:41.118557 omnata_cli-0.1.0/LICENSE
--rw-r--r--   0        0        0       49 2023-06-01 03:24:41.118557 omnata_cli-0.1.0/README.md
--rw-r--r--   0        0        0      498 2023-06-01 03:24:41.118557 omnata_cli-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1107 2023-06-01 03:24:41.118557 omnata_cli-0.1.0/src/omnata_cli/__init__.py
--rw-r--r--   0        0        0      485 1970-01-01 00:00:00.000000 omnata_cli-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    26526 2023-06-01 03:49:51.783700 omnata_cli-0.1.1/LICENSE
+-rw-r--r--   0        0        0       49 2023-06-01 03:49:51.787700 omnata_cli-0.1.1/README.md
+-rw-r--r--   0        0        0      498 2023-06-01 03:49:51.787700 omnata_cli-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1126 2023-06-01 03:49:51.787700 omnata_cli-0.1.1/src/omnata_cli/__init__.py
+-rw-r--r--   0        0        0      485 1970-01-01 00:00:00.000000 omnata_cli-0.1.1/PKG-INFO
```

### Comparing `omnata_cli-0.1.0/LICENSE` & `omnata_cli-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `omnata_cli-0.1.0/src/omnata_cli/__init__.py` & `omnata_cli-0.1.1/src/omnata_cli/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     """Open the Omnata CLI documentation in your browser."""
     typer.launch("https://docs.omnata.com")
 try:
     from omnata_plugin_devkit import cli # 
 
     # If the import is successful, we can add its commands to our application
     # Assume `external_command` is the command you want to include from the external package
-    app.command()(cli)
+    app.add_typer(cli, name="plugin_dev")
 
 except ImportError:
     @app.command()
     def plugin_dev():
         "To use the plugin-dev subcommand, run `pip install omnata_plugin_devkit`."
         print("To use the plugin-dev subcommand, run `pip install omnata_plugin_devkit`.")
         raise typer.Abort()
```

