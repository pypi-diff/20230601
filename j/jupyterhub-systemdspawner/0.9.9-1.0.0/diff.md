# Comparing `tmp/jupyterhub-systemdspawner-0.9.9.tar.gz` & `tmp/jupyterhub-systemdspawner-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jupyterhub-systemdspawner-0.9.9.tar", last modified: Thu Nov  3 03:59:19 2016, max compression
+gzip compressed data, was "jupyterhub-systemdspawner-1.0.0.tar", last modified: Thu Jun  1 21:28:48 2023, max compression
```

## Comparing `jupyterhub-systemdspawner-0.9.9.tar` & `jupyterhub-systemdspawner-1.0.0.tar`

### file list

```diff
@@ -1,13 +1,22 @@
-drwxr-xr-x   0 yuvipanda  (1000) yuvipanda  (1000)        0 2016-11-03 03:59:19.000000 jupyterhub-systemdspawner-0.9.9/
-drwxr-xr-x   0 yuvipanda  (1000) yuvipanda  (1000)        0 2016-11-03 03:59:19.000000 jupyterhub-systemdspawner-0.9.9/systemdspawner/
--rw-r--r--   0 yuvipanda  (1000) yuvipanda  (1000)       85 2016-09-06 05:57:37.000000 jupyterhub-systemdspawner-0.9.9/systemdspawner/__init__.py
--rw-r--r--   0 yuvipanda  (1000) yuvipanda  (1000)     9956 2016-11-03 03:53:52.000000 jupyterhub-systemdspawner-0.9.9/systemdspawner/systemdspawner.py
--rw-r--r--   0 yuvipanda  (1000) yuvipanda  (1000)      479 2016-11-03 03:57:21.000000 jupyterhub-systemdspawner-0.9.9/setup.py
--rw-r--r--   0 yuvipanda  (1000) yuvipanda  (1000)      359 2016-11-03 03:59:19.000000 jupyterhub-systemdspawner-0.9.9/PKG-INFO
-drwxr-xr-x   0 yuvipanda  (1000) yuvipanda  (1000)        0 2016-11-03 03:59:19.000000 jupyterhub-systemdspawner-0.9.9/jupyterhub_systemdspawner.egg-info/
--rw-r--r--   0 yuvipanda  (1000) yuvipanda  (1000)       15 2016-11-03 03:59:18.000000 jupyterhub-systemdspawner-0.9.9/jupyterhub_systemdspawner.egg-info/top_level.txt
--rw-r--r--   0 yuvipanda  (1000) yuvipanda  (1000)       11 2016-11-03 03:59:18.000000 jupyterhub-systemdspawner-0.9.9/jupyterhub_systemdspawner.egg-info/requires.txt
--rw-r--r--   0 yuvipanda  (1000) yuvipanda  (1000)      359 2016-11-03 03:59:18.000000 jupyterhub-systemdspawner-0.9.9/jupyterhub_systemdspawner.egg-info/PKG-INFO
--rw-r--r--   0 yuvipanda  (1000) yuvipanda  (1000)        1 2016-11-03 03:59:18.000000 jupyterhub-systemdspawner-0.9.9/jupyterhub_systemdspawner.egg-info/dependency_links.txt
--rw-r--r--   0 yuvipanda  (1000) yuvipanda  (1000)      312 2016-11-03 03:59:19.000000 jupyterhub-systemdspawner-0.9.9/jupyterhub_systemdspawner.egg-info/SOURCES.txt
--rw-r--r--   0 yuvipanda  (1000) yuvipanda  (1000)       59 2016-11-03 03:59:19.000000 jupyterhub-systemdspawner-0.9.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:28:48.950944 jupyterhub-systemdspawner-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-06-01 21:28:36.000000 jupyterhub-systemdspawner-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-01 21:28:36.000000 jupyterhub-systemdspawner-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    15805 2023-06-01 21:28:48.950944 jupyterhub-systemdspawner-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15433 2023-06-01 21:28:36.000000 jupyterhub-systemdspawner-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:28:48.946944 jupyterhub-systemdspawner-1.0.0/jupyterhub_systemdspawner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15805 2023-06-01 21:28:48.000000 jupyterhub-systemdspawner-1.0.0/jupyterhub_systemdspawner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-01 21:28:48.000000 jupyterhub-systemdspawner-1.0.0/jupyterhub_systemdspawner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 21:28:48.000000 jupyterhub-systemdspawner-1.0.0/jupyterhub_systemdspawner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-01 21:28:48.000000 jupyterhub-systemdspawner-1.0.0/jupyterhub_systemdspawner.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-01 21:28:48.000000 jupyterhub-systemdspawner-1.0.0/jupyterhub_systemdspawner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-01 21:28:48.000000 jupyterhub-systemdspawner-1.0.0/jupyterhub_systemdspawner.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-01 21:28:36.000000 jupyterhub-systemdspawner-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 21:28:48.950944 jupyterhub-systemdspawner-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-01 21:28:36.000000 jupyterhub-systemdspawner-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:28:48.946944 jupyterhub-systemdspawner-1.0.0/systemdspawner/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-01 21:28:36.000000 jupyterhub-systemdspawner-1.0.0/systemdspawner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7319 2023-06-01 21:28:36.000000 jupyterhub-systemdspawner-1.0.0/systemdspawner/systemd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11923 2023-06-01 21:28:36.000000 jupyterhub-systemdspawner-1.0.0/systemdspawner/systemdspawner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:28:48.946944 jupyterhub-systemdspawner-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7803 2023-06-01 21:28:36.000000 jupyterhub-systemdspawner-1.0.0/tests/test_systemd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-06-01 21:28:36.000000 jupyterhub-systemdspawner-1.0.0/tests/test_systemdspawner.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `jupyterhub-systemdspawner-0.9.9/systemdspawner/systemdspawner.py` & `jupyterhub-systemdspawner-1.0.0/systemdspawner/systemdspawner.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,269 +1,356 @@
+import asyncio
 import os
 import pwd
-import time
-import subprocess
-import shlex
-from traitlets import Bool, Int, Unicode, List
-from tornado import gen
+import sys
 
 from jupyterhub.spawner import Spawner
 from jupyterhub.utils import random_port
+from traitlets import Bool, Dict, List, Unicode
+
+from systemdspawner import systemd
+
+SYSTEMD_REQUIRED_VERSION = 243
+SYSTEMD_LOWEST_RECOMMENDED_VERSION = 245
 
 
 class SystemdSpawner(Spawner):
-    mem_limit = Unicode(
+    user_workingdir = Unicode(
         None,
-        help='Memory limit for each user. Set to `None` for no limits. Uses suffixes that are recognized by Systemd (M, G, etc)',
         allow_none=True,
-    ).tag(config=True)
+        help="""
+        Path to start each notebook user on.
 
-    cpu_limit = Int(
-        None,
-        help='CPU limit for each user. 100 means 1 full CPU, 30 is 30% of 1 CPU, 200 is 2 CPUs, etc. Set to `None` (default) for no limits',
-        allow_none=True,
+        {USERNAME} and {USERID} are expanded.
+
+        Defaults to the home directory of the user.
+
+        Not respected if dynamic_users is set to True.
+        """,
     ).tag(config=True)
 
-    user_workingdir = Unicode(
-        '/home/{USERNAME}',
-        help='Path to start each notebook user on. {USERNAME} and {USERID} are expanded'
+    username_template = Unicode(
+        "{USERNAME}",
+        help="""
+        Template for unix username each user should be spawned as.
+
+        {USERNAME} and {USERID} are expanded.
+
+        This user should already exist in the system.
+
+        Not respected if dynamic_users is set to True
+        """,
     ).tag(config=True)
 
     default_shell = Unicode(
-        os.environ.get('SHELL', '/bin/bash'),
-        help='Default shell for users on the notebook terminal'
+        os.environ.get("SHELL", "/bin/bash"),
+        help="Default shell for users on the notebook terminal",
     ).tag(config=True)
 
     extra_paths = List(
         [],
-        help='Extra paths to prepend to the $PATH environment variable. {USERNAME} and {USERID} are expanded',
+        help="""
+        Extra paths to prepend to the $PATH environment variable.
+
+        {USERNAME} and {USERID} are expanded
+        """,
     ).tag(config=True)
 
     unit_name_template = Unicode(
-        'jupyter-{USERNAME}-singleuser',
-        help='Template to use to make the systemd service names. {USERNAME} and {USERID} are expanded}'
+        "jupyter-{USERNAME}-singleuser",
+        help="""
+        Template to use to make the systemd service names.
+
+        {USERNAME} and {USERID} are expanded}
+        """,
     ).tag(config=True)
 
-    # FIXME: Do not allow enabling this for systemd versions < 227,
-    # since that is when it was introduced.
     isolate_tmp = Bool(
         False,
-        help='Give each notebook user their own /tmp, isolated from the system & each other'
+        help="""
+        Give each notebook user their own /tmp, isolated from the system & each other
+        """,
     ).tag(config=True)
 
     isolate_devices = Bool(
         False,
-        help='Give each notebook user their own /dev, with a very limited set of devices mounted'
+        help="""
+        Give each notebook user their own /dev, with a very limited set of devices mounted
+        """,
     ).tag(config=True)
 
     disable_user_sudo = Bool(
-        False,
-        help='Set to true to disallow becoming root (or any other user) via sudo or other means from inside the notebook',
+        True,
+        help="""
+        Set to true to disallow becoming root (or any other user) via sudo or other means from inside the notebook
+        """,
     ).tag(config=True)
 
     readonly_paths = List(
         None,
         allow_none=True,
-        help='List of paths that should be marked readonly from the user notebook. Subpaths can be overriden by setting readwrite_paths',
+        help="""
+        List of paths that should be marked readonly from the user notebook.
+
+        Subpaths maybe be made writeable by setting readwrite_paths
+        """,
     ).tag(config=True)
 
     readwrite_paths = List(
         None,
         allow_none=True,
-        help='List of paths that should be marked read-write from the user notebook. Usually used to make a subpath of a readonly path writeable',
+        help="""
+        List of paths that should be marked read-write from the user notebook.
+
+        Used to make a subpath of a readonly path writeable
+        """,
     ).tag(config=True)
 
-    use_sudo = Bool(
+    unit_extra_properties = Dict(
+        {},
+        help="""
+        Dict of extra properties for systemd-run --property=[...].
+
+        Keys are property names, and values are either strings or
+        list of strings (for multiple entries). When values are
+        lists, ordering is guaranteed. Ordering across keys of the
+        dictionary are *not* guaranteed.
+
+        Used to add arbitrary properties for spawned Jupyter units.
+        Read `man systemd-run` for details on per-unit properties
+        available in transient units.
+        """,
+    ).tag(config=True)
+
+    dynamic_users = Bool(
         False,
         help="""
-        Use sudo to run systemd-run / systemctl commands.
+        Allocate system users dynamically for each user.
 
-        Useful if you want to run jupyterhub as a non-root user and have set up sudo rules to allow
-        it to call systemd-run / systemctl commands
-        """
+        Uses the DynamicUser= feature of Systemd to make a new system user
+        for each hub user dynamically. Their home directories are set up
+        under /var/lib/{USERNAME}, and persist over time. The system user
+        is deallocated whenever the user's server is not running.
+
+        See http://0pointer.net/blog/dynamic-users-with-systemd.html for more
+        information.
+        """,
+    ).tag(config=True)
+
+    slice = Unicode(
+        None,
+        allow_none=True,
+        help="""
+        Ensure that all users that are created are run within a given slice.
+        This allow global configuration of the maximum resources that all users
+        collectively can use by creating a a slice beforehand.
+        """,
     ).tag(config=True)
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         # All traitlets configurables are configured by now
-        self.systemctl_cmd = ['/bin/systemctl']
-        self.systemd_run_cmd = ['/usr/bin/systemd-run']
-        if self.use_sudo:
-            self.systemctl_cmd.insert(0, '/usr/bin/sudo')
-            self.systemd_run_cmd.insert(0, '/usr/bin/sudo')
-
         self.unit_name = self._expand_user_vars(self.unit_name_template)
 
-        self.log.debug('user:%s Initialized spawner with unit %s', self.user.name, self.unit_name)
+        self.log.debug(
+            "user:%s Initialized spawner with unit %s", self.user.name, self.unit_name
+        )
 
+        systemd_version = systemd.get_systemd_version()
+        if systemd_version is None:
+            self.log.warning(
+                "Failed to parse systemd version from 'systemctl --version'"
+            )
+        elif systemd_version < SYSTEMD_REQUIRED_VERSION:
+            self.log.critical(
+                f"systemd version {SYSTEMD_REQUIRED_VERSION} or higher is required, version {systemd_version} is used"
+            )
+            sys.exit(1)
+        elif systemd_version < SYSTEMD_LOWEST_RECOMMENDED_VERSION:
+            self.log.warning(
+                f"systemd version {SYSTEMD_LOWEST_RECOMMENDED_VERSION} or higher is recommended, version {systemd_version} is used"
+            )
 
     def _expand_user_vars(self, string):
         """
         Expand user related variables in a given string
 
         Currently expands:
           {USERNAME} -> Name of the user
           {USERID} -> UserID
         """
-        return string.format(
-            USERNAME=self.user.name,
-            USERID=self.user.id
-        )
+        return string.format(USERNAME=self.user.name, USERID=self.user.id)
 
     def get_state(self):
         """
         Save state required to reconstruct spawner from scratch
 
         We save the unit name, just in case the unit template was changed
         between a restart. We do not want to lost the previously launched
         events.
 
         JupyterHub before 0.7 also assumed your notebook was dead if it
         saved no state, so this helps with that too!
         """
         state = super().get_state()
-        state['unit_name'] = self.unit_name
+        state["unit_name"] = self.unit_name
         return state
 
     def load_state(self, state):
         """
-        Load state from storage required to reinstate this user's pod
+        Load state from storage required to reinstate this user's server
 
         This runs after __init__, so we can override it with saved unit name
         if needed. This is useful primarily when you change the unit name template
         between restarts.
 
         JupyterHub before 0.7 also assumed your notebook was dead if it
         saved no state, so this helps with that too!
         """
-        if 'unit_name' in state:
-            self.unit_name = state['unit_name']
+        if "unit_name" in state:
+            self.unit_name = state["unit_name"]
 
-    @gen.coroutine
-    def start(self):
+    async def start(self):
         self.port = random_port()
-        self.log.debug('user:% Using port %s to start spawning for user %s', self.user.name, self.port)
+        self.log.debug(
+            "user:%s Using port %s to start spawning user server",
+            self.user.name,
+            self.port,
+        )
+
+        # If there's a unit with this name running already. This means a bug in
+        # JupyterHub, a remnant from a previous install or a failed service start
+        # from earlier. Regardless, we kill it and start ours in its place.
+        # FIXME: Carefully look at this when doing a security sweep.
+        if await systemd.service_running(self.unit_name):
+            self.log.info(
+                "user:%s Unit %s already exists but not known to JupyterHub. Killing",
+                self.user.name,
+                self.unit_name,
+            )
+            await systemd.stop_service(self.unit_name)
+            if await systemd.service_running(self.unit_name):
+                self.log.error(
+                    "user:%s Could not stop already existing unit %s",
+                    self.user.name,
+                    self.unit_name,
+                )
+                raise Exception(
+                    f"Could not stop already existing unit {self.unit_name}"
+                )
+
+        # If there's a unit with this name already but sitting in a failed state.
+        # Does a reset of the state before trying to start it up again.
+        if await systemd.service_failed(self.unit_name):
+            self.log.info(
+                "user:%s Unit %s in a failed state. Resetting state.",
+                self.user.name,
+                self.unit_name,
+            )
+            await systemd.reset_service(self.unit_name)
 
-        # if a previous attempt to start the service for this user was made and failed,
-        # systemd keeps the service around in 'failed' state. This will prevent future
-        # services with the same name from being started. While this behavior makes sense
-        # (since if it fails & is deleted immediately, we will lose state info), in our
-        # case it is ok to reset it and move on when trying to start again.
-        try:
-            if subprocess.check_output(self.systemctl_cmd + [
-                'is-failed',
-                self.unit_name
-            ]).decode('utf-8').strip() == 'failed':
-                subprocess.check_output(self.systemctl_cmd + [
-                    'reset-failed',
-                    self.unit_name
-                ])
-                self.log.info('user:%s Unit %s in failed state, resetting', self.user.name, self.unit_name)
-        except subprocess.CalledProcessError as e:
-            # This is returned when the unit is *not* in failed state. bah!
-            pass
         env = self.get_env()
 
-        cmd = self.systemd_run_cmd[:]
+        properties = {}
 
-        cmd.extend(['--unit', self.unit_name])
-        try:
-            pwnam = pwd.getpwnam(self.user.name)
-        except KeyError:
-            self.log.exception('No user named %s found in the system' % self.user.name)
-            raise
-        cmd.extend(['--uid', str(pwnam.pw_uid), '--gid', str(pwnam.pw_gid)])
+        if self.dynamic_users:
+            properties["DynamicUser"] = "yes"
+            properties["StateDirectory"] = self._expand_user_vars("{USERNAME}")
+
+            # HOME is not set by default otherwise
+            env["HOME"] = self._expand_user_vars("/var/lib/{USERNAME}")
+            # Set working directory to $HOME too
+            working_dir = env["HOME"]
+            # Set uid, gid = None so we don't set them
+            uid = gid = None
+        else:
+            try:
+                unix_username = self._expand_user_vars(self.username_template)
+                pwnam = pwd.getpwnam(unix_username)
+            except KeyError:
+                self.log.exception(f"No user named {unix_username} found in the system")
+                raise
+            uid = pwnam.pw_uid
+            gid = pwnam.pw_gid
+            if self.user_workingdir is None:
+                working_dir = pwnam.pw_dir
+            else:
+                working_dir = self._expand_user_vars(self.user_workingdir)
 
         if self.isolate_tmp:
-            cmd.extend(['--property=PrivateTmp=yes'])
+            properties["PrivateTmp"] = "yes"
 
         if self.isolate_devices:
-            cmd.extend(['--property=PrivateDevices=yes'])
+            properties["PrivateDevices"] = "yes"
 
         if self.extra_paths:
-            env['PATH'] = '{extrapath}:{curpath}'.format(
-                curpath=env['PATH'],
-                extrapath=':'.join(
+            env["PATH"] = "{extrapath}:{curpath}".format(
+                curpath=env["PATH"],
+                extrapath=":".join(
                     [self._expand_user_vars(p) for p in self.extra_paths]
-                )
+                ),
             )
 
-        for key, value in env.items():
-            cmd.append('--setenv={key}={value}'.format(key=key, value=value))
-
-        cmd.append('--setenv=SHELL={shell}'.format(shell=self.default_shell))
+        env["SHELL"] = self.default_shell
 
         if self.mem_limit is not None:
-            # FIXME: Detect & use proper properties for v1 vs v2 cgroups
-            cmd.extend([
-                '--property=MemoryAccounting=yes',
-                '--property=MemoryLimit={mem}'.format(mem=self.mem_limit),
-            ])
+            properties["MemoryAccounting"] = "yes"
+            properties["MemoryMax"] = self.mem_limit
 
         if self.cpu_limit is not None:
-            # FIXME: Detect & use proper properties for v1 vs v2 cgroups
-            # FIXME: Make sure that the kernel supports CONFIG_CFS_BANDWIDTH
-            #        otherwise this doesn't have any effect.
-            cmd.extend([
-                '--property=CPUAccounting=yes',
-                '--property=CPUQuota={quota}%'.format(quota=self.cpu_limit)
-            ])
+            # NOTE: The linux kernel must be compiled with the configuration option
+            #       CONFIG_CFS_BANDWIDTH, otherwise CPUQuota doesn't have any
+            #       effect.
+            #
+            #       This can be checked with the check-kernel.bash script in
+            #       this git repository.
+            #
+            #       ref: https://github.com/systemd/systemd/blob/v245/README#L35
+            #
+            properties["CPUAccounting"] = "yes"
+            properties["CPUQuota"] = f"{int(self.cpu_limit * 100)}%"
 
         if self.disable_user_sudo:
-            cmd.append('--property=NoNewPrivileges=yes')
+            properties["NoNewPrivileges"] = "yes"
 
         if self.readonly_paths is not None:
-            cmd.extend([
-                self._expand_user_vars('--property=ReadOnlyDirectories=-{path}'.format(path=path))
-                for path in self.readonly_paths
-            ])
+            properties["ReadOnlyDirectories"] = [
+                self._expand_user_vars(path) for path in self.readonly_paths
+            ]
 
         if self.readwrite_paths is not None:
-            cmd.extend([
-                self._expand_user_vars('--property=ReadWriteDirectories={path}'.format(path=path))
-                for path in self.readwrite_paths
-            ])
-
-        # We unfortunately have to resort to doing cd with bash, since WorkingDirectory property
-        # of systemd units can't be set for transient units via systemd-run until systemd v227.
-        # Centos 7 has systemd 219, and will probably never upgrade - so we need to support them.
-        bash_cmd = [
-            '/bin/bash',
-            '-c',
-            "cd {wd} && exec {cmd} {args}".format(
-                wd=shlex.quote(self._expand_user_vars(self.user_workingdir)),
-                cmd=' '.join([shlex.quote(self._expand_user_vars(c)) for c in self.cmd]),
-                args=' '.join([shlex.quote(a) for a in self.get_args()])
-            )
-        ]
-        cmd.extend(bash_cmd)
-
-        self.log.debug('user:%s Running systemd-run with: %s', self.user.name, ' '.join(cmd))
-        subprocess.check_output(cmd)
+            properties["ReadWriteDirectories"] = [
+                self._expand_user_vars(path) for path in self.readwrite_paths
+            ]
+
+        for property, value in self.unit_extra_properties.items():
+            self.unit_extra_properties[property] = self._expand_user_vars(value)
+
+        properties.update(self.unit_extra_properties)
+
+        await systemd.start_transient_service(
+            self.unit_name,
+            cmd=[self._expand_user_vars(c) for c in self.cmd],
+            args=[self._expand_user_vars(a) for a in self.get_args()],
+            working_dir=working_dir,
+            environment_variables=env,
+            properties=properties,
+            uid=uid,
+            gid=gid,
+            slice=self.slice,
+        )
 
         for i in range(self.start_timeout):
-            is_up = yield self.poll()
+            is_up = await self.poll()
             if is_up is None:
-                return (self.ip or '127.0.0.1', self.port)
-            yield gen.sleep(1)
+                return (self.ip or "127.0.0.1", self.port)
+            await asyncio.sleep(1)
 
         return None
 
-    @gen.coroutine
-    def stop(self):
-        subprocess.check_output(self.systemctl_cmd + [
-            'stop',
-            self.unit_name
-        ])
-
-    @gen.coroutine
-    def poll(self):
-        try:
-            if subprocess.check_call(self.systemctl_cmd + [
-                'is-active',
-                self.unit_name
-            ], stdout=open('/dev/null', 'w'), stderr=open('/dev/null', 'w')) == 0:
-                self.log.debug('user:%s unit %s is active', self.user.name, self.unit_name)
-                return None
-        except subprocess.CalledProcessError as e:
-            self.log.debug('user:%s unit %s is not active', self.user.name, self.unit_name)
-            return e.returncode
+    async def stop(self, now=False):
+        await systemd.stop_service(self.unit_name)
+
+    async def poll(self):
+        if await systemd.service_running(self.unit_name):
+            return None
+        return 1
```

