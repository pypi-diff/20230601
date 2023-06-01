# Comparing `tmp/jax-tools-1.0.8.tar.gz` & `tmp/jax-tools-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jax-tools-1.0.8.tar", last modified: Thu Jun  1 04:02:15 2023, max compression
+gzip compressed data, was "jax-tools-1.0.9.tar", last modified: Thu Jun  1 04:58:33 2023, max compression
```

## Comparing `jax-tools-1.0.8.tar` & `jax-tools-1.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 cyber.anonym   (501) staff       (20)        0 2023-06-01 04:02:15.584270 jax-tools-1.0.8/
--rw-r--r--   0 cyber.anonym   (501) staff       (20)      377 2023-06-01 04:02:15.584007 jax-tools-1.0.8/PKG-INFO
--rw-r--r--   0 cyber.anonym   (501) staff       (20)       28 2023-06-01 03:10:01.000000 jax-tools-1.0.8/README.md
-drwxr-xr-x   0 cyber.anonym   (501) staff       (20)        0 2023-06-01 04:02:15.578551 jax-tools-1.0.8/jax_tools/
--rw-r--r--   0 cyber.anonym   (501) staff       (20)      378 2023-06-01 03:54:45.000000 jax-tools-1.0.8/jax_tools/CHANGELOG.md
--rw-r--r--   0 cyber.anonym   (501) staff       (20)        0 2023-05-31 12:57:36.000000 jax-tools-1.0.8/jax_tools/__init__.py
--rw-r--r--   0 cyber.anonym   (501) staff       (20)     1919 2023-06-01 03:00:26.000000 jax-tools-1.0.8/jax_tools/logger.py
--rw-r--r--   0 cyber.anonym   (501) staff       (20)     2901 2023-06-01 02:46:34.000000 jax-tools-1.0.8/jax_tools/network_test.py
--rw-r--r--   0 cyber.anonym   (501) staff       (20)     2148 2023-06-01 02:42:28.000000 jax-tools-1.0.8/jax_tools/ssh_ops.py
-drwxr-xr-x   0 cyber.anonym   (501) staff       (20)        0 2023-06-01 04:02:15.583598 jax-tools-1.0.8/jax_tools/utils/
--rw-r--r--   0 cyber.anonym   (501) staff       (20)        0 2023-05-31 13:11:26.000000 jax-tools-1.0.8/jax_tools/utils/__init__.py
--rw-r--r--   0 cyber.anonym   (501) staff       (20)      221 2023-05-31 13:15:04.000000 jax-tools-1.0.8/jax_tools/utils/settings.py
-drwxr-xr-x   0 cyber.anonym   (501) staff       (20)        0 2023-06-01 04:02:15.582315 jax-tools-1.0.8/jax_tools.egg-info/
--rw-r--r--   0 cyber.anonym   (501) staff       (20)      377 2023-06-01 04:02:15.000000 jax-tools-1.0.8/jax_tools.egg-info/PKG-INFO
--rw-r--r--   0 cyber.anonym   (501) staff       (20)      386 2023-06-01 04:02:15.000000 jax-tools-1.0.8/jax_tools.egg-info/SOURCES.txt
--rw-r--r--   0 cyber.anonym   (501) staff       (20)        1 2023-06-01 04:02:15.000000 jax-tools-1.0.8/jax_tools.egg-info/dependency_links.txt
--rw-r--r--   0 cyber.anonym   (501) staff       (20)       51 2023-06-01 04:02:15.000000 jax-tools-1.0.8/jax_tools.egg-info/entry_points.txt
--rw-r--r--   0 cyber.anonym   (501) staff       (20)       45 2023-06-01 04:02:15.000000 jax-tools-1.0.8/jax_tools.egg-info/requires.txt
--rw-r--r--   0 cyber.anonym   (501) staff       (20)       10 2023-06-01 04:02:15.000000 jax-tools-1.0.8/jax_tools.egg-info/top_level.txt
--rw-r--r--   0 cyber.anonym   (501) staff       (20)       38 2023-06-01 04:02:15.584357 jax-tools-1.0.8/setup.cfg
--rw-r--r--   0 cyber.anonym   (501) staff       (20)     1596 2023-06-01 04:02:15.000000 jax-tools-1.0.8/setup.py
+drwxr-xr-x   0 cyber.anonym   (501) staff       (20)        0 2023-06-01 04:58:33.625723 jax-tools-1.0.9/
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)      392 2023-06-01 04:58:33.625277 jax-tools-1.0.9/PKG-INFO
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)       28 2023-06-01 03:10:01.000000 jax-tools-1.0.9/README.md
+drwxr-xr-x   0 cyber.anonym   (501) staff       (20)        0 2023-06-01 04:58:33.617631 jax-tools-1.0.9/jax_tools/
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)      378 2023-06-01 03:54:45.000000 jax-tools-1.0.9/jax_tools/CHANGELOG.md
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)        0 2023-05-31 12:57:36.000000 jax-tools-1.0.9/jax_tools/__init__.py
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)     1919 2023-06-01 03:00:26.000000 jax-tools-1.0.9/jax_tools/logger.py
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)     2901 2023-06-01 02:46:34.000000 jax-tools-1.0.9/jax_tools/network_test.py
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)     2819 2023-06-01 04:58:18.000000 jax-tools-1.0.9/jax_tools/ssh_ops.py
+drwxr-xr-x   0 cyber.anonym   (501) staff       (20)        0 2023-06-01 04:58:33.624649 jax-tools-1.0.9/jax_tools/utils/
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)        0 2023-05-31 13:11:26.000000 jax-tools-1.0.9/jax_tools/utils/__init__.py
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)      119 2023-06-01 04:28:51.000000 jax-tools-1.0.9/jax_tools/utils/settings.py
+drwxr-xr-x   0 cyber.anonym   (501) staff       (20)        0 2023-06-01 04:58:33.622707 jax-tools-1.0.9/jax_tools.egg-info/
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)      392 2023-06-01 04:58:33.000000 jax-tools-1.0.9/jax_tools.egg-info/PKG-INFO
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)      386 2023-06-01 04:58:33.000000 jax-tools-1.0.9/jax_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)        1 2023-06-01 04:58:33.000000 jax-tools-1.0.9/jax_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)       51 2023-06-01 04:58:33.000000 jax-tools-1.0.9/jax_tools.egg-info/entry_points.txt
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)       45 2023-06-01 04:58:33.000000 jax-tools-1.0.9/jax_tools.egg-info/requires.txt
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)       10 2023-06-01 04:58:33.000000 jax-tools-1.0.9/jax_tools.egg-info/top_level.txt
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)       38 2023-06-01 04:58:33.625922 jax-tools-1.0.9/setup.cfg
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)     1611 2023-06-01 04:58:18.000000 jax-tools-1.0.9/setup.py
```

### Comparing `jax-tools-1.0.8/jax_tools/logger.py` & `jax-tools-1.0.9/jax_tools/logger.py`

 * *Files identical despite different names*

### Comparing `jax-tools-1.0.8/jax_tools/network_test.py` & `jax-tools-1.0.9/jax_tools/network_test.py`

 * *Files identical despite different names*

### Comparing `jax-tools-1.0.8/jax_tools/ssh_ops.py` & `jax-tools-1.0.9/jax_tools/ssh_ops.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,83 +3,102 @@
 ssh operations
 """
 import paramiko
 import traceback
 import logging
 
 
-def get_ssh_client(host, username, password, port):
-    """
-    获取ssh连接
-    Returns:
-
-    """
-    paramiko_logger = paramiko.util.logging.getLogger()
-    paramiko_logger.setLevel(logging.WARN)
-    client = paramiko.SSHClient()
-    client.set_missing_host_key_policy(paramiko.AutoAddPolicy())
-    response = True
-    try:
-        client.connect(
-            host,
-            port,
-            username=str(username),
-            password=str(password),
-            timeout=10)
-    except paramiko.ssh_exception.AuthenticationException:
-        paramiko_logger.error('身份验证失败')
-        response = None
-    except paramiko.ssh_exception.NoValidConnectionsError:
-        paramiko_logger.error('无法连接到目标主机')
-        response = None
-    except Exception as e:
-        paramiko_logger.error(e)
-        response = None
-    if response:
-        return client
-    else:
-        return response
-
-
-def run_ssh_cmd(ssh_client, command, read_line=True, time_out=300):
-    """
-    ssh执行命令方法
-    Args:
-        ssh_client:
-        command:
-        read_line:
-        time_out
-
-    Returns:
-
-    """
-    try:
-        std_in, std_out, std_err = ssh_client.exec_command(
-            command, timeout=time_out)
-        if read_line:
-            result = std_out.readlines()
-        else:
-            result = std_out.read().decode('utf-8').rstrip()
-    except Exception as e:
-        logging.error(traceback.format_exc())
-        logging.error(e)
-        result = '用户连接登录信息可能有误'
-    return result
-
-
 class SSHConnect(object):
     """
     SSH Connector
     """
 
-    def __init__(self, host, port, username, password):
+    def __init__(self, host, port, username, password) -> None:
+        """
+        SSH Connector
+        Args:
+            host (str): host
+            port (int): port
+            username (str): username
+            password (str): password
+        """
         self.host = host
         self.username = username
         self.password = password
         self.port = port
-        self.ssh_client = get_ssh_client(host, username, password, port)
+        self.ssh_client = self.__get_ssh_client()
+        if self.ssh_client is None:
+            print('SSH connection failed')
+
+    def __get_ssh_client(self):
+        """
+        Get ssh client
+        Args:
+
+        Returns:
+            ssh client
+
+        """
+        paramiko_logger = paramiko.util.logging.getLogger()
+        paramiko_logger.setLevel(logging.WARN)
+        client = paramiko.SSHClient()
+        client.set_missing_host_key_policy(paramiko.AutoAddPolicy())
+        response = True
+        try:
+            client.connect(
+                self.host,
+                self.port,
+                username=str(self.username),
+                password=str(self.password),
+                timeout=10)
+        except paramiko.ssh_exception.AuthenticationException:
+            paramiko_logger.error('身份验证失败')
+            response = None
+        except paramiko.ssh_exception.NoValidConnectionsError:
+            paramiko_logger.error('无法连接到目标主机')
+            response = None
+        except Exception as e:
+            paramiko_logger.error(e)
+            response = None
+        if response:
+            return client
+        else:
+            return response
 
-    def run_cmd(self, cmd, read_line=True, time_out=300):
-        return run_ssh_cmd(self.ssh_client, cmd, read_line, time_out)
+    def run_cmd(self, cmd, read_line=False, time_out=300):
+        """
+        Run command on remote host
+        Args:
+            cmd (str): command to run
+            read_line (bool): True if read line by line, False if read all
+            time_out (int): timeout in seconds
+
+        Returns:
+            String if read_line is False
+
+        """
+        if self.ssh_client is None:
+            return 'SSH connection failed'
+        try:
+            std_in, std_out, std_err = self.ssh_client.exec_command(cmd, timeout=time_out)
+            if read_line:
+                result = std_out.readlines()
+            else:
+                result = std_out.read().decode('utf-8').rstrip()
+        except Exception as e:
+            logging.error(traceback.format_exc())
+            logging.error(e)
+            result = 'user login info may be wrong'
+        return result
+
+    def close(self) -> None:
+        """
+        Close ssh connection
+        Returns:
 
-    def close_connection(self):
+        """
         self.ssh_client.close()
+
+    def __del__(self):
+        if self.ssh_client:
+            self.close()
+
```

### Comparing `jax-tools-1.0.8/setup.py` & `jax-tools-1.0.9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,18 +16,18 @@
     """
     with open(file_path, 'r') as f:
         return f.read()
 
 
 setuptools.setup(
     name="jax-tools",
-    version="1.0.8",
+    version="1.0.9",
     author=u"Jax",
     author_email='alvin.wan.cn@hotmail.com',
-    description=u"Jax Tools",
+    description=u"Jax common tools library",
     platforms=['CentOS', 'Redhat', 'MacOS', 'Windows'],
     long_description='Jax Tools',
     long_description_content_type="text/markdown",
     url="https://jax-arsenals.com",
     license="MIT Licence",
     python_requires=">=3.0.0",
     # 定义要构建到包中的文件列表，这些文件会放到/usr/local下
```

