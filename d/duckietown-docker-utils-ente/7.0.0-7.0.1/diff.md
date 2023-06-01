# Comparing `tmp/duckietown-docker-utils-ente-7.0.0.tar.gz` & `tmp/duckietown-docker-utils-ente-7.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duckietown-docker-utils-ente-7.0.0.tar", last modified: Wed Jul 28 22:49:43 2021, max compression
+gzip compressed data, was "duckietown-docker-utils-ente-7.0.1.tar", last modified: Thu Jun  1 13:49:51 2023, max compression
```

## Comparing `duckietown-docker-utils-ente-7.0.0.tar` & `duckietown-docker-utils-ente-7.0.1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2021-07-28 22:49:43.436323 duckietown-docker-utils-ente-7.0.0/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      202 2021-07-28 22:49:43.436323 duckietown-docker-utils-ente-7.0.0/PKG-INFO
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       38 2021-07-28 22:49:43.436323 duckietown-docker-utils-ente-7.0.0/setup.cfg
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      905 2021-07-28 22:46:59.000000 duckietown-docker-utils-ente-7.0.0/setup.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2021-07-28 22:49:43.436323 duckietown-docker-utils-ente-7.0.0/src/
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2021-07-28 22:49:43.436323 duckietown-docker-utils-ente-7.0.0/src/duckietown_docker_utils/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      341 2021-07-28 22:48:53.000000 duckietown-docker-utils-ente-7.0.0/src/duckietown_docker_utils/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1362 2021-07-28 22:46:20.000000 duckietown-docker-utils-ente-7.0.0/src/duckietown_docker_utils/cli.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      769 2021-07-28 22:46:20.000000 duckietown-docker-utils-ente-7.0.0/src/duckietown_docker_utils/constants.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    16543 2021-07-28 22:46:20.000000 duckietown-docker-utils-ente-7.0.0/src/duckietown_docker_utils/docker_run.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     4068 2021-07-28 22:46:20.000000 duckietown-docker-utils-ente-7.0.0/src/duckietown_docker_utils/monitoring.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1425 2021-07-28 22:46:20.000000 duckietown-docker-utils-ente-7.0.0/src/duckietown_docker_utils/terminal_size.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2021-07-28 22:49:43.436323 duckietown-docker-utils-ente-7.0.0/src/duckietown_docker_utils_ente.egg-info/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      202 2021-07-28 22:49:43.000000 duckietown-docker-utils-ente-7.0.0/src/duckietown_docker_utils_ente.egg-info/PKG-INFO
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      591 2021-07-28 22:49:43.000000 duckietown-docker-utils-ente-7.0.0/src/duckietown_docker_utils_ente.egg-info/SOURCES.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        1 2021-07-28 22:49:43.000000 duckietown-docker-utils-ente-7.0.0/src/duckietown_docker_utils_ente.egg-info/dependency_links.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       78 2021-07-28 22:49:43.000000 duckietown-docker-utils-ente-7.0.0/src/duckietown_docker_utils_ente.egg-info/entry_points.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       13 2021-07-28 22:49:43.000000 duckietown-docker-utils-ente-7.0.0/src/duckietown_docker_utils_ente.egg-info/requires.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       24 2021-07-28 22:49:43.000000 duckietown-docker-utils-ente-7.0.0/src/duckietown_docker_utils_ente.egg-info/top_level.txt
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-06-01 13:49:51.920397 duckietown-docker-utils-ente-7.0.1/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      153 2023-06-01 13:49:51.920397 duckietown-docker-utils-ente-7.0.1/PKG-INFO
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       38 2023-06-01 13:49:51.920397 duckietown-docker-utils-ente-7.0.1/setup.cfg
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      397 2023-06-01 13:49:46.000000 duckietown-docker-utils-ente-7.0.1/setup.json
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      940 2023-06-01 13:46:55.000000 duckietown-docker-utils-ente-7.0.1/setup.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-06-01 13:49:51.920397 duckietown-docker-utils-ente-7.0.1/src/
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-06-01 13:49:51.920397 duckietown-docker-utils-ente-7.0.1/src/duckietown_docker_utils/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      341 2023-06-01 13:49:46.000000 duckietown-docker-utils-ente-7.0.1/src/duckietown_docker_utils/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1362 2023-06-01 13:40:49.000000 duckietown-docker-utils-ente-7.0.1/src/duckietown_docker_utils/cli.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      772 2023-06-01 13:40:49.000000 duckietown-docker-utils-ente-7.0.1/src/duckietown_docker_utils/constants.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    16894 2023-06-01 13:40:49.000000 duckietown-docker-utils-ente-7.0.1/src/duckietown_docker_utils/docker_run.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     4148 2023-06-01 13:40:49.000000 duckietown-docker-utils-ente-7.0.1/src/duckietown_docker_utils/monitoring.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1421 2023-06-01 13:40:49.000000 duckietown-docker-utils-ente-7.0.1/src/duckietown_docker_utils/terminal_size.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-06-01 13:49:51.920397 duckietown-docker-utils-ente-7.0.1/src/duckietown_docker_utils_ente.egg-info/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      153 2023-06-01 13:49:51.000000 duckietown-docker-utils-ente-7.0.1/src/duckietown_docker_utils_ente.egg-info/PKG-INFO
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      602 2023-06-01 13:49:51.000000 duckietown-docker-utils-ente-7.0.1/src/duckietown_docker_utils_ente.egg-info/SOURCES.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        1 2023-06-01 13:49:51.000000 duckietown-docker-utils-ente-7.0.1/src/duckietown_docker_utils_ente.egg-info/dependency_links.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       78 2023-06-01 13:49:51.000000 duckietown-docker-utils-ente-7.0.1/src/duckietown_docker_utils_ente.egg-info/entry_points.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       27 2023-06-01 13:49:51.000000 duckietown-docker-utils-ente-7.0.1/src/duckietown_docker_utils_ente.egg-info/requires.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       24 2023-06-01 13:49:51.000000 duckietown-docker-utils-ente-7.0.1/src/duckietown_docker_utils_ente.egg-info/top_level.txt
```

### Comparing `duckietown-docker-utils-ente-7.0.0/setup.py` & `duckietown-docker-utils-ente-7.0.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,15 +15,19 @@
     if version is None:
         raise ValueError(filename)
     return version
 
 
 version = get_version(filename="src/duckietown_docker_utils/__init__.py")
 
-install_requires = ["progressbar2"]
+install_requires = [
+    "progressbar2",
+    "docker",
+    "PyYAML",
+]
 
 line = "ente"
 
 setup(
     name=f"duckietown-docker-utils-{line}",
     version=version,
     keywords="",
```

### Comparing `duckietown-docker-utils-ente-7.0.0/src/duckietown_docker_utils/cli.py` & `duckietown-docker-utils-ente-7.0.1/src/duckietown_docker_utils/cli.py`

 * *Files identical despite different names*

### Comparing `duckietown-docker-utils-ente-7.0.0/src/duckietown_docker_utils/constants.py` & `duckietown-docker-utils-ente-7.0.1/src/duckietown_docker_utils/constants.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 DT1_TOKEN_CONFIG_KEY = "token_dt1"
 CONFIG_DOCKER_USERNAME = "docker_username"
 CONFIG_DOCKER_CREDENTIALS = "docker_credentials"
 CONFIG_DUCKIETOWN_VERSION = "duckietown_version"
 
 CONFIG_DOCKER_PASSWORD = "docker_password"
 
-ENV_REGISTRY = "AIDO_REGISTRY"
+ENV_REGISTRY = "DOCKER_REGISTRY"
 
 ENV_IGNORE_DIRTY = "DT_IGNORE_DIRTY"
 ENV_IGNORE_UNTAGGED = "DT_IGNORE_UNTAGGED"
 
 ENV_DT_BUILD_HOST = "DT_DOCKER_BUILD_HOST"
 
 # These are passed to the called container.
 # If the value is None, no variable is passed if one is not present.
 IMPORTANT_ENVS = {
     ENV_REGISTRY: "docker.io",
-    "PIP_INDEX_URL": "https://pypi.org/simple",
+    "PIP_INDEX_URL": "https://pypi.org/simple/",
     "DTSERVER": "https://challenges.duckietown.org/v4",
     ENV_IGNORE_UNTAGGED: None,
     ENV_IGNORE_DIRTY: None,
 }
 
 
 DEPTH_VAR = "DOCKER_DEPTH"
```

### Comparing `duckietown-docker-utils-ente-7.0.0/src/duckietown_docker_utils/docker_run.py` & `duckietown-docker-utils-ente-7.0.1/src/duckietown_docker_utils/docker_run.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,19 +38,22 @@
     "generic_docker_run",
     "get_developer_volumes",
     "replace_important_env_vars",
 ]
 
 
 def replace_important_env_vars(s: str) -> str:
+    if not isinstance(s, str):
+        raise TypeError(str(type(s)))
     for vname, vdefault in IMPORTANT_ENVS.items():
         vref = "${%s}" % vname
         if vref in s:
             value = os.environ.get(vname, vdefault)
             s = s.replace(vref, value)
+
     return s
 
 
 @dataclass
 class GenericDockerRunOutput:
     retcode: int
     message: str
@@ -71,14 +74,15 @@
     container_name: Optional[str],
     logname: str,
     docker_credentials: Dict[str, Dict[str, str]] = None,
     detach: bool = True,
     read_only: bool = True,
     working_dir: str = None,
     share_tmp: bool = True,
+    volumes_from: List[str] = None,
 ) -> GenericDockerRunOutput:
     if container_name is None:
         container_name = f"cont{random.randint(0, 1000000)}"
     image = replace_important_env_vars(image)
 
     pwd = os.getcwd()
 
@@ -94,14 +98,17 @@
         pwd_to_share = pwd
     else:
         logger.debug(f"repo_root={repo_root!r} pwd={pwd!r} pwd1={pwd1!r}")
         pwd_to_share = repo_root
 
     volumes2: Dict[str, dict] = {}
     envs = {}
+
+    if "DOCKER_HOST" in os.environ:
+        envs["DOCKER_HOST"] = os.environ["DOCKER_HOST"]
     for k, default in IMPORTANT_ENVS.items():
         v = os.environ.get(k, default)
         if v is not None:
             envs[k] = v
 
     def include(x: str) -> bool:
         return x.startswith("DT") or "TWINE" in x
@@ -132,31 +139,35 @@
             additional_mode = ""
 
         guest_credentials = CREDENTIALS_FILE
         volumes2[credentials] = {"bind": guest_credentials, "mode": f"ro{additional_mode}"}
 
         uid1 = os.getuid()
 
+        envs["CREDENTIALS"] = json.dumps(contents)
+
         if as_root:
             pass
         else:
             envs["USER"] = user
             envs["USERID"] = uid1
 
             # home = os.path.expanduser("~")
 
             volumes2[fake_home_host] = {"bind": FAKE_HOME_GUEST, "mode": f"rw{additional_mode}"}
             envs["HOME"] = FAKE_HOME_GUEST
 
         PWD = pwd1
-        # volumes[f'{fake_home}/.docker'] = f'{home}/.docker', False
-        volumes2[pwd_to_share] = {
-            "bind": pwd_to_share,
-            "mode": f"ro{additional_mode}" if read_only else f"rw{additional_mode}",
-        }
+
+        if not volumes_from:
+            # volumes[f'{fake_home}/.docker'] = f'{home}/.docker', False
+            volumes2[pwd_to_share] = {
+                "bind": pwd_to_share,
+                "mode": f"ro{additional_mode}" if read_only else f"rw{additional_mode}",
+            }
         on_mac = "Darwin" in platform.system()
 
         if on_mac:
             volumes2[f"/var/run/docker.sock.raw"] = {"bind": "/var/run/docker.sock", "mode": "rw"}
         else:
             volumes2[f"/var/run/docker.sock"] = {"bind": "/var/run/docker.sock", "mode": "rw"}
         if share_tmp:
@@ -262,14 +273,15 @@
             command=commands,
             tty=interactive,
             volumes=volumes2,
             environment=envs,
             network_mode="host",
             detach=detach,
             name=container_name,
+            volumes_from=volumes_from,
         )
         if entrypoint is not None:
             params["entrypoint"] = entrypoint
         if working_dir:
             params["working_dir"] = working_dir
         if development:
             logger.debug("Parameters:\n%s" % json.dumps(params, indent=4))
@@ -286,15 +298,15 @@
                 message = "Interrupted"
                 cleanup(client, container_name=container_name, prefix=prefix)
                 return GenericDockerRunOutput(retcode=0, message=message)
                 # not found; for example, CTRL-C
 
             #  {'Error': None, 'StatusCode': 32
             StatusCode = res["StatusCode"]
-            Error = res["Error"]
+            Error = res.get("Error", "n/a")
             if StatusCode and Error:
                 logger.error(f"StatusCode: {StatusCode} Error: {Error}")
             else:
                 pass
                 # logger.debug(f"StatusCode: {StatusCode} Error: {Error}")
             if Error is None:
                 Error = f"Container exited with code {StatusCode}"
```

### Comparing `duckietown-docker-utils-ente-7.0.0/src/duckietown_docker_utils/monitoring.py` & `duckietown-docker-utils-ente-7.0.1/src/duckietown_docker_utils/monitoring.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,19 @@
         # noinspection PyBroadException
         try:
 
             with open(log, "ab") as f:
                 building = b""
 
                 for c in container.logs(
-                    stdout=True, stderr=True, stream=True, follow=True, since=last_log_timestamp,
+                    stdout=True,
+                    stderr=True,
+                    stream=True,
+                    follow=True,
+                    since=last_log_timestamp,
                 ):
                     # XXX: not sure why this is needed
                     if isinstance(c, str):
                         c = c.encode()
                     f.write(c)
                     f.flush()
```

### Comparing `duckietown-docker-utils-ente-7.0.0/src/duckietown_docker_utils/terminal_size.py` & `duckietown-docker-utils-ente-7.0.1/src/duckietown_docker_utils/terminal_size.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     #         raise ValueError(msg)
 
     return max_x
 
 
 def getTerminalSize() -> Tuple[int, int]:
     """
-        columns, lines = getTerminalSize()
+    columns, lines = getTerminalSize()
     """
     cr = ioctl_GWINSZ(0) or ioctl_GWINSZ(1) or ioctl_GWINSZ(2)
     if not cr:
         # noinspection PyBroadException
         try:
             fd = os.open(os.ctermid(), os.O_RDONLY)
             cr = ioctl_GWINSZ(fd)
```

### Comparing `duckietown-docker-utils-ente-7.0.0/src/duckietown_docker_utils_ente.egg-info/SOURCES.txt` & `duckietown-docker-utils-ente-7.0.1/src/duckietown_docker_utils_ente.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+setup.json
 setup.py
 src/duckietown_docker_utils/__init__.py
 src/duckietown_docker_utils/cli.py
 src/duckietown_docker_utils/constants.py
 src/duckietown_docker_utils/docker_run.py
 src/duckietown_docker_utils/monitoring.py
 src/duckietown_docker_utils/terminal_size.py
```

