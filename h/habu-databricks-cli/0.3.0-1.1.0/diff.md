# Comparing `tmp/habu_databricks_cli-0.3.0-py3-none-any.whl.zip` & `tmp/habu_databricks_cli-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,21 @@
-Zip file size: 16292 bytes, number of entries: 20
--rw-r--r--  2.0 unx     3764 b- defN 23-May-01 17:40 README.md
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-01 00:18 hdb/__init__.py
--rw-r--r--  2.0 unx     3604 b- defN 23-May-01 17:40 hdb/_token.py
--rw-r--r--  2.0 unx     6095 b- defN 23-May-01 17:40 hdb/cli.py
--rw-r--r--  2.0 unx     5088 b- defN 23-May-01 17:40 hdb/cluster.py
--rw-r--r--  2.0 unx     3567 b- defN 23-May-01 17:40 hdb/config.py
--rw-r--r--  2.0 unx     3206 b- defN 23-Apr-01 00:18 hdb/init.py
--rw-r--r--  2.0 unx     4946 b- defN 23-May-01 17:40 hdb/job.py
--rw-r--r--  2.0 unx      854 b- defN 23-Apr-13 14:16 hdb/util.py
--rw-r--r--  2.0 unx     3457 b- defN 23-May-01 17:40 hdb/cli_installer/cli-installer.sql
--rw-r--r--  2.0 unx     3721 b- defN 23-May-01 17:40 hdb/commands/cleanroom_request.sql
--rw-r--r--  2.0 unx      277 b- defN 23-Apr-10 19:59 hdb/commands/create-cleanroom.sql
--rw-r--r--  2.0 unx      912 b- defN 23-Apr-10 19:59 hdb/commands/create-dataset.sql
--rw-r--r--  2.0 unx     1883 b- defN 23-May-01 17:40 hdb/commands/new-data-connection.sql
--rw-r--r--  2.0 unx      594 b- defN 23-May-01 17:40 hdb/resource/config.yaml
--rw-r--r--  2.0 unx      388 b- defN 23-May-01 17:44 habu_databricks_cli-0.3.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-01 17:44 habu_databricks_cli-0.3.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       40 b- defN 23-May-01 17:44 habu_databricks_cli-0.3.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        4 b- defN 23-May-01 17:44 habu_databricks_cli-0.3.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1598 b- defN 23-May-01 17:44 habu_databricks_cli-0.3.0.dist-info/RECORD
-20 files, 44090 bytes uncompressed, 13696 bytes compressed:  68.9%
+Zip file size: 15249 bytes, number of entries: 19
+-rw-r--r--  2.0 unx     3764 b- defN 23-Jun-01 19:24 README.md
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 19:24 hdb/__init__.py
+-rw-r--r--  2.0 unx     5989 b- defN 23-Jun-01 19:24 hdb/cli.py
+-rw-r--r--  2.0 unx     5623 b- defN 23-Jun-01 19:24 hdb/cluster.py
+-rw-r--r--  2.0 unx     3478 b- defN 23-Jun-01 19:24 hdb/config.py
+-rw-r--r--  2.0 unx     3638 b- defN 23-Jun-01 19:24 hdb/init.py
+-rw-r--r--  2.0 unx     5348 b- defN 23-Jun-01 19:24 hdb/job.py
+-rw-r--r--  2.0 unx      854 b- defN 23-Jun-01 19:24 hdb/util.py
+-rw-r--r--  2.0 unx     3246 b- defN 23-Jun-01 19:24 hdb/cli_installer/cli-installer.sql
+-rw-r--r--  2.0 unx     3721 b- defN 23-Jun-01 19:24 hdb/commands/cleanroom-request.sql
+-rw-r--r--  2.0 unx      277 b- defN 23-Jun-01 19:24 hdb/commands/create-cleanroom.sql
+-rw-r--r--  2.0 unx      912 b- defN 23-Jun-01 19:24 hdb/commands/create-dataset.sql
+-rw-r--r--  2.0 unx     1883 b- defN 23-Jun-01 19:24 hdb/commands/new-data-connection.sql
+-rw-r--r--  2.0 unx      594 b- defN 23-Jun-01 19:24 hdb/resource/config.yaml
+-rw-r--r--  2.0 unx      388 b- defN 23-Jun-01 19:25 habu_databricks_cli-1.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-01 19:25 habu_databricks_cli-1.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       40 b- defN 23-Jun-01 19:25 habu_databricks_cli-1.1.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        4 b- defN 23-Jun-01 19:25 habu_databricks_cli-1.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1528 b- defN 23-Jun-01 19:25 habu_databricks_cli-1.1.0.dist-info/RECORD
+19 files, 41379 bytes uncompressed, 12755 bytes compressed:  69.2%
```

## zipnote {}

```diff
@@ -1,16 +1,13 @@
 Filename: README.md
 Comment: 
 
 Filename: hdb/__init__.py
 Comment: 
 
-Filename: hdb/_token.py
-Comment: 
-
 Filename: hdb/cli.py
 Comment: 
 
 Filename: hdb/cluster.py
 Comment: 
 
 Filename: hdb/config.py
@@ -24,38 +21,38 @@
 
 Filename: hdb/util.py
 Comment: 
 
 Filename: hdb/cli_installer/cli-installer.sql
 Comment: 
 
-Filename: hdb/commands/cleanroom_request.sql
+Filename: hdb/commands/cleanroom-request.sql
 Comment: 
 
 Filename: hdb/commands/create-cleanroom.sql
 Comment: 
 
 Filename: hdb/commands/create-dataset.sql
 Comment: 
 
 Filename: hdb/commands/new-data-connection.sql
 Comment: 
 
 Filename: hdb/resource/config.yaml
 Comment: 
 
-Filename: habu_databricks_cli-0.3.0.dist-info/METADATA
+Filename: habu_databricks_cli-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: habu_databricks_cli-0.3.0.dist-info/WHEEL
+Filename: habu_databricks_cli-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: habu_databricks_cli-0.3.0.dist-info/entry_points.txt
+Filename: habu_databricks_cli-1.1.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: habu_databricks_cli-0.3.0.dist-info/top_level.txt
+Filename: habu_databricks_cli-1.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: habu_databricks_cli-0.3.0.dist-info/RECORD
+Filename: habu_databricks_cli-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hdb/cli.py

```diff
@@ -1,12 +1,12 @@
 import logging
 
 import click
 
-from hdb import config as hdb_config, _token as token, util
+from hdb import config as hdb_config, util
 from hdb import init as init_setup, job, cluster
 from hdb.config import DATABRICKS_IID, USER
 
 RES_CONFIG: dict = hdb_config.read_resource_config('resource/config.yaml')
 
 
 @click.group()
@@ -38,34 +38,33 @@
 @cli.command()
 @click.option('--config-file', '-c', default='habu_databricks_config.yaml',
               help='File name where config will get saved (default is habu_databricks_config.yaml in current directory)')
 @click.option('--databricks-instance', '-i', prompt='Databricks instance id',
               help=' Databricks instance id (<instance-id>.cloud.databricks.com)')
 @click.option('--login', '-u', prompt="Databricks user name",
               help='Databricks user name (me@example.com)')
-@click.password_option('--password', '-p', prompt='Password',
-                       help='Enter the password')
+@click.password_option('--token', '-t', prompt='Token',
+                       help='Enter the token generated from Databricks user settings')
 @click.option('--log-level', '-l', type=click.Choice(['CRITICAL', 'ERROR', 'WARNING', 'INFO', 'DEBUG'],
                                                      case_sensitive=False), default='INFO',
               help='Select log level while running the commands, default level is set to INFO')
 @click.option('--auto-termination-mins', '-m', default=10, type=click.UNPROCESSED, callback=validate_mins,
               help='Automatically terminate the cluster after it is inactive for this time in minutes.'
                    ' If not set, the cluster will not be automatically terminated.'
                    'The threshold must be between 10 and 10000 minutes. You can also set this value to 0 '
                    'to explicitly disable automatic termination.')
-def config(config_file: str, databricks_instance: str, login: str, password: str,
-           log_level: str, auto_termination_mins: int):
+def config(config_file: str, databricks_instance: str, login: str, token: str, log_level: str, auto_termination_mins: int):
     """
     Command to generate the config for the habu databricks agent.
     The config is required to set up the habu databricks framework
     """
     setup_log(getattr(logging, log_level.upper()))
-    config_params = hdb_config.create_config(config_file, databricks_instance, login, password, auto_termination_mins)
+    config_params = hdb_config.create_config(config_file, databricks_instance, login, token, auto_termination_mins)
     if config_params is not None:
-        token.setup_token(databricks_instance, config_file, config_params, RES_CONFIG)
+        logging.info('Config file created successfully')
 
 
 @cli.command()
 @click.option('--config-file', '-c', default='habu_databricks_config.yaml',
               help='File name from where config gets read (default is habu_databricks_config.yaml in current directory)')
 @click.option('--log-level', '-l', type=click.Choice(['CRITICAL', 'ERROR', 'WARNING', 'INFO', 'DEBUG'],
                                                      case_sensitive=False), default='INFO',
@@ -74,30 +73,30 @@
     """Command to list available node types to create cluster.
     The results are the valid values that can be passed as node-type in init command"""
     setup_log(getattr(logging, log_level.upper()))
     config_params = hdb_config.read_config(config_file)
 
     if config_params is not None:
         db_instance = config_params[DATABRICKS_IID]
-        token.setup_token(db_instance, config_file, config_params, RES_CONFIG)
-        nodes = cluster.list_available_nodes(db_instance)
+        # token.setup_token(db_instance, config_file, config_params, RES_CONFIG)
+        nodes = cluster.list_available_nodes(db_instance, config_params)
         for node in nodes:
             print(node)
     else:
         logging.error(f'Failed to read config from {config_file}, use config cmd to generate config')
 
 
 @cli.command()
 @click.option('--org-id', '-o', prompt="Organization id", help='Habu Org Id')
 @click.option('--habu-sharing-id', '-s', prompt="Habu Sharing Id", help='Habu Sharing Id (aws:<region>:<id>)')
 @click.option('--orchestrator', '-oc', prompt="Orchestrator Name", help='Orchestrator name',
               default='habu-stage-orchestrator')
 @click.option('--config-file', '-c', default="./habu_databricks_config.yaml",
               help='Databricks Configuration file')
-@click.option('-node-type', '-n', prompt='cluster node type',
+@click.option('--node-type', '-n', prompt='cluster node type',
               help='Choose cluster node type (case sensitive), '
                    'use list-nodes command to find acceptable node-type values')
 @click.option('--log-level', '-l', type=click.Choice(['CRITICAL', 'ERROR', 'WARNING', 'INFO', 'DEBUG'],
                                                      case_sensitive=False), default='INFO',
               help='Select log level while running the commands, default level is set to INFO')
 def init(org_id: str, habu_sharing_id: str, orchestrator: str, config_file: str, node_type: str, log_level: str):
     """Initialize Habu Databricks framework.
@@ -106,14 +105,13 @@
     """
 
     setup_log(getattr(logging, log_level.upper()))
     config_params = hdb_config.read_config(config_file)
 
     if config_params is not None:
         db_instance = config_params[DATABRICKS_IID]
-        token.setup_token(db_instance, config_file, config_params, RES_CONFIG)
-        init_setup.setup_workspace(db_instance, config_params[USER])
+        init_setup.setup_workspace(db_instance, config_params)
         cluster_id = cluster.setup_cluster(db_instance, config_file, config_params, node_type, RES_CONFIG)
         job.setup_jobs(db_instance, org_id, habu_sharing_id, orchestrator, cluster_id,
-                       config_params[USER])
+                       config_params)
     else:
         logging.error(f'Failed to read config from {config_file}, use config cmd to generate config')
```

## hdb/cluster.py

```diff
@@ -7,37 +7,44 @@
 
 CLUSTERS: str = 'clusters'
 CLUSTER_ID: str = 'cluster_id'
 CLUSTER_CONFIG: str = 'cluster_config'
 
 
 def contains_cluster(cluster_id: str, cluster_list):
+    logging.info(f'Checking if cluster {cluster_id} exists')
     if cluster_list is not None and cluster_id is not None:
         for cluster in cluster_list:
             if cluster[CLUSTER_ID] == cluster_id:
                 return True
     return False
 
 
-def list_cluster(db_instance: str):
+def list_cluster(db_instance: str, params: dict):
+    headers = {
+        'Authorization': 'Bearer {}'.format(params['token']),
+    }
     logging.info('Fetching list of available clusters')
-    response = requests.get('https://{}/api/2.0/clusters/list'.format(db_instance))
+    response = requests.get('https://{}/api/2.0/clusters/list'.format(db_instance), headers=headers)
     cluster_list = None
     if response.ok:
         cluster_list = response.json()
         return cluster_list.get(CLUSTERS)
     else:
         util.log_response(response, 'unable to fetch list of clusters!')
     response.close()
     return cluster_list
 
 
-def list_node_types(db_instance: str):
+def list_node_types(db_instance: str, params: dict):
     node_types = None
-    response = requests.get(f'https://{db_instance}/api/2.0/clusters/list-node-types')
+    headers = {
+        'Authorization': 'Bearer {}'.format(params['token']),
+    }
+    response = requests.get(f'https://{db_instance}/api/2.0/clusters/list-node-types', headers=headers)
     if response.ok:
         node_types = response.json()
     else:
         util.log_response(response, 'unable to list node types!!')
     response.close()
     return node_types
 
@@ -60,52 +67,54 @@
     logging.debug(f'num filtered : {len(filtered_nodes)}')
     if len(node_list) <= 0:
         logging.warning('Could not fetch list of supported nodes, '
                         'please make sure that the user or service principal has appropriate permissions!!')
     return filtered_nodes
 
 
-def list_available_nodes(db_instance: str):
-    return filter_node_types(list_node_types(db_instance))
+def list_available_nodes(db_instance: str, params):
+    return filter_node_types(list_node_types(db_instance, params))
 
 
-def create_cluster(db_instance: str, cluster_config: dict):
+def create_cluster(db_instance: str, cluster_config: dict, params):
     logging.info('Creating cluster')
     headers = {
         'Content-Type': 'application/x-www-form-urlencoded',
+        'Authorization': 'Bearer {}'.format(params['token']),
     }
     response = requests.post('https://{}/api/2.0/clusters/create'.format(db_instance), headers=headers,
                              data=json.dumps(cluster_config))
     cluster_id: str = ''
     if response.ok:
         cluster_id = response.json().get(CLUSTER_ID)
         logging.info(f'Cluster created, cluster_id: {cluster_id}')
     else:
         util.log_response(response, 'unable to create cluster!!')
     response.close()
     return cluster_id
 
 
-def terminate_cluster(db_instance: str, cluster_id: str):
+def terminate_cluster(db_instance: str, cluster_id: str, params: dict):
     logging.info(f'Terminating(Stopping) cluster : {cluster_id}')
     headers = {
         'Content-Type': 'application/x-www-form-urlencoded',
+        'Authorization': 'Bearer {}'.format(params['token']),
     }
     data = {
         CLUSTER_ID: cluster_id
     }
     response = requests.post('https://{}/api/2.0/clusters/delete'.format(db_instance), headers=headers,
                              data=json.dumps(data))
     if not response.ok:
         util.log_response(response, 'Unable to terminate cluster!')
     response.close()
 
 
-def validate_node_type(db_instance: str, node_type_id: str):
-    available_nodes = list_available_nodes(db_instance)
+def validate_node_type(db_instance: str, node_type_id: str, params: dict):
+    available_nodes = list_available_nodes(db_instance, params)
     if node_type_id in available_nodes:
         return True
     if len(available_nodes) > 0:
         logging.error(f'node type {node_type_id} not found!!')
         logging.info(f'Please choose from one of the following nodes : \n {available_nodes}')
     return False
 
@@ -117,25 +126,25 @@
 
     if config_params is not None:
         if node_type_id in config_params:
             cluster_id = config_params[node_type_id].get(CLUSTER_ID)
         if config.AUTO_TERMINATION_MINS in config_params:
             auto_termination_mins = config_params[config.AUTO_TERMINATION_MINS]
 
-    if validate_node_type(db_instance, node_type_id):
-        cluster_list = list_cluster(db_instance)
+    if validate_node_type(db_instance, node_type_id, config_params):
+        cluster_list = list_cluster(db_instance, config_params)
         if contains_cluster(cluster_id, cluster_list):
             return cluster_id
         else:
             logging.info('Required cluster not found')
 
             cluster_config = res_config[CLUSTER_CONFIG].copy()
             cluster_config[config.NODE_TYPE_ID] = node_type_id
             cluster_config[config.DRIVER_NODE_TYPE_ID] = node_type_id
             cluster_config[config.AUTO_TERMINATION_MINS] = auto_termination_mins
 
-            cluster_id = create_cluster(db_instance, cluster_config)
+            cluster_id = create_cluster(db_instance, cluster_config, config_params)
             cluster_info = {CLUSTER_ID: cluster_id}
             config.update_config(config_file, node_type_id, cluster_info)
-            terminate_cluster(db_instance, cluster_id)
+            terminate_cluster(db_instance, cluster_id, config_params)
 
     return cluster_id
```

## hdb/config.py

```diff
@@ -9,39 +9,35 @@
 
 DATABRICKS_IID: str = 'databricks_instance_id'
 USER: str = 'user'
 NODE_TYPE_LIST: str = 'node_type_list'
 NODE_TYPE_ID: str = 'node_type_id'
 DRIVER_NODE_TYPE_ID: str = 'driver_node_type_id'
 AUTO_TERMINATION_MINS: str = 'autotermination_minutes'
+TOKEN: str = 'token'
 
 
 def open_netrc():
     # create netrc if it doesn't exist
     file = os.path.join(os.path.expanduser('~'), '.netrc')
     if not os.path.exists(file):
         open(file, 'w').close()
     netrc = Netrc()
     return netrc
 
 
-def create_config(conf_file_name: str, databricks_instance: str, login: str, password: str, auto_termination_mins: int):
+def create_config(conf_file_name: str, databricks_instance: str, login: str, token: str, auto_termination_mins: int):
     # Add a new entry
-    netrc = open_netrc()
-    netrc[databricks_instance] = {
-        'login': login,
-        'password': password
-    }
-    netrc.save()
 
     config = None
     habu_config = {
-        USER: login,
         DATABRICKS_IID: databricks_instance,
         AUTO_TERMINATION_MINS: auto_termination_mins,
+        TOKEN: token,
+        USER: login,
     }
     try:
         with open(conf_file_name, 'w') as hdb_config:
             try:
                 hdb_config.write(yaml_dump(habu_config, indent=4))
                 hdb_config.close()
                 config = habu_config
@@ -49,15 +45,15 @@
                 logging.error('Failed to create config!', exc_info=True)
     except (FileNotFoundError, PermissionError, OSError):
         logging.error('Failed to open conf file for writing!', exc_info=True)
     return config
 
 
 def validate_critical_params(config_params: dict):
-    params = [USER, DATABRICKS_IID, AUTO_TERMINATION_MINS]
+    params = [USER, DATABRICKS_IID, AUTO_TERMINATION_MINS, TOKEN]
     for param in params:
         if config_params.get(param) is None:
             raise ValueError(f'Param {param} missing in config file, please run the config command to create config!!')
 
 
 def read_config(config_file, validate=True):
     config_params = None
```

## hdb/init.py

```diff
@@ -2,31 +2,33 @@
 import logging
 import os
 
 import pkg_resources
 import requests
 
 from hdb import util
+from hdb.config import USER
 
 
 def walk_resource_paths(root_dir):
     file_paths = []
     for name in pkg_resources.resource_listdir(__package__, root_dir):
         path = root_dir + f'/{name}'
         if pkg_resources.resource_isdir(__package__, path):
             file_paths = file_paths + walk_resource_paths(path)
         else:
             file_paths.append(path)
     return file_paths
 
 
-def list_dir(db_instance: str, dir_path: str):
+def list_dir(db_instance: str, dir_path: str, params):
     headers = {
         'Accept': 'application/json',
         'Content-Type': 'application/x-www-form-urlencoded',
+        'Authorization': 'Bearer {}'.format(params['token'])
     }
     data = {
         'path': dir_path
     }
     dir_list = None
     response = requests.get('https://{}/api/2.0/workspace/list'.format(db_instance), headers=headers,
                             data=json.dumps(data))
@@ -34,64 +36,69 @@
         dir_list = response.json()
     else:
         util.log_response(response, 'Workspace path does not exist!', warn=True)
     response.close()
     return dir_list
 
 
-def create_dir(db_instance, dir_path):
+def create_dir(db_instance, dir_path, params: dict):
     # habu_framework/commands/
     # habu_framework/installer/
     logging.info(f'Creating workspace dir : {dir_path}')
     headers = {
         'Accept': 'application/json',
+        'Authorization': 'Bearer {}'.format(params['token']),
     }
     data = {
         'path': dir_path
     }
     response = requests.post('https://{}/api/2.0/workspace/mkdirs'.format(db_instance), headers=headers,
                              data=json.dumps(data))
     if not response.ok:
         util.log_response(response, 'unable to create directory!')
     response.close()
 
 
-def upload_notebook(db_instance, file_path, dir_path):
+def upload_notebook(db_instance, file_path, dir_path, params):
+    headers = {
+        'Authorization': 'Bearer {}'.format(params['token'])
+    }
     logging.info(f'Setting up {file_path}')
     with open(pkg_resources.resource_filename(__package__, file_path), 'rb') as nb:
         try:
             files = {
                 'path': (None, os.path.join(dir_path, os.path.basename(file_path))),
                 'language': (None, 'SQL'),
                 'overwrite': (None, 'true'),
                 'content': nb,
             }
-            response = requests.post('https://{}/api/2.0/workspace/import'.format(db_instance), files=files)
+            response = requests.post('https://{}/api/2.0/workspace/import'.format(db_instance), files=files,
+                                     headers=headers)
             if not response.ok:
                 util.log_response(response, 'Unable to upload file')
             response.close()
             nb.close()
         except (requests.RequestException, ConnectionError):
             logging.error(f'Failed to setup {file_path}', exc_info=True)
 
 
-def setup_workspace(db_instance, user_id):
-    base_dir = '/Users/{}/habu_framework'.format(user_id)
+def setup_workspace(db_instance, config_params: dict):
+    base_dir = '/Users/{}/habu_framework'.format(config_params[USER])
 
     commands_dir_path = '{}/commands'.format(base_dir)
     installer_dir_path = '{}/installer'.format(base_dir)
 
-    dir_list = list_dir(db_instance, commands_dir_path)
+    dir_list = list_dir(db_instance, commands_dir_path, config_params)
     if dir_list is None:
-        create_dir(db_instance, commands_dir_path)
+        create_dir(db_instance, commands_dir_path, config_params)
 
-    dir_list = list_dir(db_instance, installer_dir_path)
+    dir_list = list_dir(db_instance, installer_dir_path, config_params)
     if dir_list is None:
-        create_dir(db_instance, installer_dir_path)
+        create_dir(db_instance, installer_dir_path, config_params)
 
     file_path_list = walk_resource_paths('cli_installer')
     for file_path in file_path_list:
-        upload_notebook(db_instance, file_path, installer_dir_path)
+        upload_notebook(db_instance, file_path, installer_dir_path, config_params)
 
     file_path_list = walk_resource_paths('commands')
     for file_path in file_path_list:
-        upload_notebook(db_instance, file_path, commands_dir_path)
+        upload_notebook(db_instance, file_path, commands_dir_path, config_params)
```

## hdb/job.py

```diff
@@ -1,13 +1,14 @@
 import json
 import logging
 
 import requests
 
 from hdb import util
+from hdb.config import USER
 
 
 def get_job_config(org_id: str, habu_sharing_id: str, orchestrator: str, cluster_id: str, user: str,
                    job_name: str, task_key: str, notebook: str, schedule_config: dict = None):
     job_config = {
         'name': job_name,
         'email_notifications': {
@@ -39,34 +40,36 @@
 
     if schedule_config is not None:
         job_config['schedule'] = schedule_config
 
     return job_config
 
 
-def create_job(db_instance: str, job_config: dict, job_name: str):
+def create_job(db_instance: str, job_config: dict, job_name: str, params: dict):
     logging.info(f'Creating job : {job_name}')
     headers = {
         'Content-Type': 'application/x-www-form-urlencoded',
+        'Authorization': 'Bearer {}'.format(params['token']),
     }
     response = requests.post('https://{}/api/2.1/jobs/create'.format(db_instance),
                              headers=headers, data=json.dumps(job_config))
     job = None
     if response.ok:
         job = response.json()
     else:
         util.log_response(response, f'Failed to create job : {job_name}')
     response.close()
     return job
 
 
-def update_job(db_instance: str, job_config: dict, job_id: str, job_name: str):
+def update_job(db_instance: str, job_config: dict, job_id: str, job_name: str, params: dict):
     logging.info(f'Updating job : {job_name}')
     headers = {
         'Content-Type': 'application/x-www-form-urlencoded',
+        'Authorization': 'Bearer {}'.format(params['token']),
     }
     update_config = {
         'job_id': job_id,
         'new_settings': job_config
     }
     response = requests.post('https://{}/api/2.1/jobs/update'.format(db_instance),
                              headers=headers, data=json.dumps(update_config))
@@ -80,32 +83,34 @@
     if job_list is not None:
         for job in job_list:
             if job['creator_user_name'] == user and job['settings']['name'] == job_name:
                 return job['job_id']
     return None
 
 
-def list_jobs(db_instance: str):
+def list_jobs(db_instance: str, params: dict):
     logging.info('fetching existing jobs')
     headers = {
         'Content-Type': 'application/x-www-form-urlencoded',
+        'Authorization': 'Bearer {}'.format(params['token']),
     }
     job_list = None
     response = requests.get('https://{}/api/2.1/jobs/list'.format(db_instance),
                             headers=headers)
     if response.ok:
         job_list = response.json()
     else:
         util.log_response(response, 'unable to fetch list of jobs!')
     response.close()
     return job_list
 
 
 def setup_jobs(db_instance: str, org_id: str, habu_sharing_id: str, orchestrator_name: str,
-               cluster_id: str, user: str):
+               cluster_id: str, config_params: dict):
+    user = config_params[USER]
     if len(cluster_id) <= 0:
         logging.error(f'Failed to create job, cluster is not setup cluster_id: {cluster_id}')
         return False
 
     cli_installer = 'cli-installer'
     cleanroom_request = 'cleanroom-request'
 
@@ -118,23 +123,23 @@
         'pause_status': 'PAUSED'
     }
 
     cr_request_config = get_job_config(org_id, habu_sharing_id, orchestrator_name, cluster_id, user,
                                        cleanroom_request, cleanroom_request, 'commands/cleanroom-request.sql',
                                        cron_config)
 
-    job_list = list_jobs(db_instance)
+    job_list = list_jobs(db_instance, config_params)
     if job_list is not None:
         job_id = job_exists(job_list, user, cli_installer)
         if job_id is not None:
-            update_job(db_instance, cli_job_config, job_id, cli_installer)
+            update_job(db_instance, cli_job_config, job_id, cli_installer, config_params)
         else:
-            create_job(db_instance, cli_job_config, cli_installer)
+            create_job(db_instance, cli_job_config, cli_installer, config_params)
 
         job_id = job_exists(job_list, user, cleanroom_request)
         if job_id is not None:
-            update_job(db_instance, cr_request_config, job_id, cleanroom_request)
+            update_job(db_instance, cr_request_config, job_id, cleanroom_request, config_params)
         else:
-            create_job(db_instance, cr_request_config, cleanroom_request)
+            create_job(db_instance, cr_request_config, cleanroom_request, config_params)
     else:
-        create_job(db_instance, cli_job_config, cli_installer)
-        create_job(db_instance, cr_request_config, cleanroom_request)
+        create_job(db_instance, cli_job_config, cli_installer, config_params)
+        create_job(db_instance, cr_request_config, cleanroom_request, config_params)
```

## hdb/cli_installer/cli-installer.sql

```diff
@@ -1,14 +1,7 @@
--- Databricks notebook source
--- MAGIC %python
--- MAGIC 
--- MAGIC org_id_sanitized = dbutils.widgets.get("org_id").replace("-", "")
--- MAGIC 
--- MAGIC dbutils.widgets.text("org_id_sanitized", org_id_sanitized)
-
 -- COMMAND ----------
 
 create catalog if not exists habu_org_${org_id_sanitized}_share_db USING SHARE ${orchestrator_name}.habu_org_${org_id_sanitized}_share;
 
 -- COMMAND ----------
 
 create catalog if not exists HABU_CLEAN_ROOM_COMMON;
@@ -69,8 +62,8 @@
 
 -- COMMAND ----------
 
 GRANT SELECT ON SHARE habu_clean_room_common_share_${org_id_sanitized} TO RECIPIENT habu_orchestrator;
 
 -- COMMAND ----------
 
-insert into habu_clean_room_common.clean_room.app_metadata select uuid(), 'latest_version', '2', current_timestamp, null;
+insert into habu_clean_room_common.clean_room.app_metadata select uuid(), 'latest_version', '1', current_timestamp, null;
```

## Comparing `hdb/commands/cleanroom_request.sql` & `hdb/commands/cleanroom-request.sql`

 * *Files identical despite different names*

## Comparing `habu_databricks_cli-0.3.0.dist-info/RECORD` & `habu_databricks_cli-1.1.0.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 README.md,sha256=fqeBg96AMadrv9ff8Z8Z1W3ea3K-b3A6gWbRVDPMbbI,3764
 hdb/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-hdb/_token.py,sha256=JGOTD7E0yB4z5XFLeW28EV0dz5vOr2-_lI83g5x3RS8,3604
-hdb/cli.py,sha256=k4JdTxN6GU7lfStiqlrt5m78TLHDbS5vPbJyasladOU,6095
-hdb/cluster.py,sha256=uyfeodBtYNOZ_ZFuhaKg4uN1sioS8oC4IlHCAD8Mg4M,5088
-hdb/config.py,sha256=J-I__GzVqMvgQq2MojzI_PkZ1ZQq_Rbj32JbYyS67Us,3567
-hdb/init.py,sha256=xKbDpGHCSF6r58ZcwCXoMm35HuK6Eb5BhlG0b6dICL0,3206
-hdb/job.py,sha256=lTYhFbsw3KV3VX25j320FSsVei-pYViJ-PHOdvPbKL8,4946
+hdb/cli.py,sha256=hWIvHAmNCN19_051NPf-xTlpd3VHn3Nvkb6b8y1qdqk,5989
+hdb/cluster.py,sha256=XvXK-gzvvw0QyNull4-4ZyS0iIFS-kGFvaFjnZARZi4,5623
+hdb/config.py,sha256=nAlDhoqb5mftGeBYB28ujeRMtHKd3dC4TkvMcz3QYTI,3478
+hdb/init.py,sha256=0IW_u9BvG0UMeS7UG4ph6jIS25BD2f4cZpIMUY-sc4k,3638
+hdb/job.py,sha256=FJvs3PCQ_wM5yjzYmBoy9HBhiuCcZnUsaYgitUcNNkk,5348
 hdb/util.py,sha256=tYfGJp_NA8kBfO0LqoA11JObYOPzsuxrKCjqpDFvFEU,854
-hdb/cli_installer/cli-installer.sql,sha256=qmPSrOG-AIWYD5JRKmYaQOweFDMFe8fi5Azx_5y7Kf0,3457
-hdb/commands/cleanroom_request.sql,sha256=iyUZ5OW2VZYfbU60dszHTsdme5HycZZoT7gMHd41Zio,3721
+hdb/cli_installer/cli-installer.sql,sha256=qSuja0hew3YoyS8grN9eZKFtEtSvKqgjB7qxbozAuHo,3246
+hdb/commands/cleanroom-request.sql,sha256=iyUZ5OW2VZYfbU60dszHTsdme5HycZZoT7gMHd41Zio,3721
 hdb/commands/create-cleanroom.sql,sha256=NcadqD1wEGejr8G2Wqd7ajukzVbdZn588JA8JbU2Lps,277
 hdb/commands/create-dataset.sql,sha256=DgtagXn7eLCQkJxgGdUKo36tvTHVJi_6HZRQ-EHwzZM,912
 hdb/commands/new-data-connection.sql,sha256=SlV8qwK7cIfMBE07bOw-q-3AhJxlIV9676zRYDpY0As,1883
 hdb/resource/config.yaml,sha256=8CMoKN7sqljcw0oWI15U6yb2hCn8u1ItftVgdk9rBPY,594
-habu_databricks_cli-0.3.0.dist-info/METADATA,sha256=FHYCa2D3vM_ohsNkPaAt5O5PwjCWoC7MBszR-TXTCeA,388
-habu_databricks_cli-0.3.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-habu_databricks_cli-0.3.0.dist-info/entry_points.txt,sha256=ncoJOHelyx6usEFcFZ-lmQC5N0TCmPdFQ0jodLc2Z3E,40
-habu_databricks_cli-0.3.0.dist-info/top_level.txt,sha256=G1s1EaggMBt7hVcx2WCCSPJFZ4_mpLsMEENCmnDbE34,4
-habu_databricks_cli-0.3.0.dist-info/RECORD,,
+habu_databricks_cli-1.1.0.dist-info/METADATA,sha256=Pu3mci7kuTRG2qagZK73yeaqO9KzkiQgEDVt5oaRiEg,388
+habu_databricks_cli-1.1.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+habu_databricks_cli-1.1.0.dist-info/entry_points.txt,sha256=ncoJOHelyx6usEFcFZ-lmQC5N0TCmPdFQ0jodLc2Z3E,40
+habu_databricks_cli-1.1.0.dist-info/top_level.txt,sha256=G1s1EaggMBt7hVcx2WCCSPJFZ4_mpLsMEENCmnDbE34,4
+habu_databricks_cli-1.1.0.dist-info/RECORD,,
```

