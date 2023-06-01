# Comparing `tmp/datagit-0.2.tar.gz` & `tmp/datagit-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datagit-0.2.tar", last modified: Tue May 23 14:59:50 2023, max compression
+gzip compressed data, was "datagit-0.3.tar", last modified: Thu Jun  1 09:44:05 2023, max compression
```

## Comparing `datagit-0.2.tar` & `datagit-0.3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-05-23 14:59:50.897602 datagit-0.2/
--rw-r--r--   0 sammyteillet   (501) staff       (20)     1167 2023-05-23 14:59:50.897419 datagit-0.2/PKG-INFO
--rw-r--r--   0 sammyteillet   (501) staff       (20)      766 2023-05-22 17:03:46.000000 datagit-0.2/README.md
-drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-05-23 14:59:50.896276 datagit-0.2/datagit/
--rw-r--r--   0 sammyteillet   (501) staff       (20)        0 2023-05-22 13:02:30.000000 datagit-0.2/datagit/__init__.py
--rw-r--r--   0 sammyteillet   (501) staff       (20)      636 2023-05-23 14:46:32.000000 datagit-0.2/datagit/dataset_helpers.py
--rw-r--r--   0 sammyteillet   (501) staff       (20)     3665 2023-05-23 14:46:32.000000 datagit-0.2/datagit/github_connector.py
--rw-r--r--   0 sammyteillet   (501) staff       (20)      721 2023-05-23 14:01:11.000000 datagit-0.2/datagit/query_builder.py
-drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-05-23 14:59:50.897068 datagit-0.2/datagit.egg-info/
--rw-r--r--   0 sammyteillet   (501) staff       (20)     1167 2023-05-23 14:59:50.000000 datagit-0.2/datagit.egg-info/PKG-INFO
--rw-r--r--   0 sammyteillet   (501) staff       (20)      242 2023-05-23 14:59:50.000000 datagit-0.2/datagit.egg-info/SOURCES.txt
--rw-r--r--   0 sammyteillet   (501) staff       (20)        1 2023-05-23 14:59:50.000000 datagit-0.2/datagit.egg-info/dependency_links.txt
--rw-r--r--   0 sammyteillet   (501) staff       (20)        8 2023-05-23 14:59:50.000000 datagit-0.2/datagit.egg-info/top_level.txt
--rw-r--r--   0 sammyteillet   (501) staff       (20)       38 2023-05-23 14:59:50.897666 datagit-0.2/setup.cfg
--rw-r--r--   0 sammyteillet   (501) staff       (20)      581 2023-05-23 14:59:49.000000 datagit-0.2/setup.py
+drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-06-01 09:44:05.697644 datagit-0.3/
+-rw-r--r--   0 sammyteillet   (501) staff       (20)     3126 2023-06-01 09:44:05.697500 datagit-0.3/PKG-INFO
+-rw-r--r--   0 sammyteillet   (501) staff       (20)     2726 2023-06-01 09:39:55.000000 datagit-0.3/README.md
+drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-06-01 09:44:05.696351 datagit-0.3/datagit/
+-rw-r--r--   0 sammyteillet   (501) staff       (20)        0 2023-05-22 13:02:30.000000 datagit-0.3/datagit/__init__.py
+-rw-r--r--   0 sammyteillet   (501) staff       (20)      635 2023-05-23 16:37:26.000000 datagit-0.3/datagit/dataset_helpers.py
+-rw-r--r--   0 sammyteillet   (501) staff       (20)     4313 2023-05-23 16:37:26.000000 datagit-0.3/datagit/github_connector.py
+-rw-r--r--   0 sammyteillet   (501) staff       (20)      721 2023-05-23 14:01:11.000000 datagit-0.3/datagit/query_builder.py
+drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-06-01 09:44:05.697256 datagit-0.3/datagit.egg-info/
+-rw-r--r--   0 sammyteillet   (501) staff       (20)     3126 2023-06-01 09:44:05.000000 datagit-0.3/datagit.egg-info/PKG-INFO
+-rw-r--r--   0 sammyteillet   (501) staff       (20)      272 2023-06-01 09:44:05.000000 datagit-0.3/datagit.egg-info/SOURCES.txt
+-rw-r--r--   0 sammyteillet   (501) staff       (20)        1 2023-06-01 09:44:05.000000 datagit-0.3/datagit.egg-info/dependency_links.txt
+-rw-r--r--   0 sammyteillet   (501) staff       (20)       16 2023-06-01 09:44:05.000000 datagit-0.3/datagit.egg-info/requires.txt
+-rw-r--r--   0 sammyteillet   (501) staff       (20)        8 2023-06-01 09:44:05.000000 datagit-0.3/datagit.egg-info/top_level.txt
+-rw-r--r--   0 sammyteillet   (501) staff       (20)       38 2023-06-01 09:44:05.697697 datagit-0.3/setup.cfg
+-rw-r--r--   0 sammyteillet   (501) staff       (20)      648 2023-06-01 09:41:42.000000 datagit-0.3/setup.py
```

### Comparing `datagit-0.2/datagit/dataset_helpers.py` & `datagit-0.3/datagit/dataset_helpers.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import pandas as pd
 
+
 def assert_dataset_has_unique_key(dataset: pd.DataFrame) -> None:
     first_column = dataset.columns[0]
 
     if first_column != "unique_key":
         raise ValueError(f"The first column is not named 'unique_key'")
 
     # Check if the first column is unique
     values = dataset[first_column].tolist()
     if len(values) != len(set(values)):
         raise ValueError(f"The {first_column} column is not unique")
 
+
 def sort_dataframe_on_first_column_and_assert_is_unique(df: pd.DataFrame) -> pd.DataFrame:
     assert_dataset_has_unique_key(df)
-    
+
     sorted_df = df.sort_values(by=['unique_key'])
-    return sorted_df
+    return sorted_df
```

### Comparing `datagit-0.2/datagit/github_connector.py` & `datagit-0.3/datagit/github_connector.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,89 +1,97 @@
 from typing import Optional, List
 import pandas as pd
 from github import Github, Repository, ContentFile, GithubException
 from datagit.dataset_helpers import sort_dataframe_on_first_column_and_assert_is_unique
 
 
-def store_metric(ghClient: Github, dataframe: pd.DataFrame, filepath: str, assignees: List[str] = [], branch: str = "production"):
+def store_metric(ghClient: Github, dataframe: pd.DataFrame, filepath: str, assignees: List[str] = [], branch: str = "production", store_json: bool = True) -> None:
     repo_orga, repo_name, file_path = filepath.split('/', 2)
 
     repo = ghClient.get_repo(repo_orga + "/" + repo_name)
     assert_branch_exist(repo, branch)
-    contents = assert_file_exists(repo,file_path, ref=branch)
+    contents = assert_file_exists(repo, file_path, ref=branch)
     dataframe = sort_dataframe_on_first_column_and_assert_is_unique(dataframe)
     if contents is None:
-        create_file_with_pull_request(file_path, repo, branch, dataframe, assignees)
+        create_file_with_pull_request(
+            file_path, repo, branch, dataframe, assignees, store_json)
         pass
     else:
-        new_contents = dataframe.to_csv()
+        new_contents = dataframe.to_csv(index=False, header=True)
         if contents.decoded_content.decode('utf-8') != new_contents:
             push_new_content_with_pull_request(
-                file_path, repo, branch, contents, dataframe, assignees)
+                file_path, repo, branch, contents, dataframe, assignees, store_json)
     pass
 
 
 def assert_file_exists(repo: Repository.Repository, file_path: str, ref: str) -> Optional[ContentFile.ContentFile]:
     try:
         contents = repo.get_contents(file_path, ref=ref)
-        assert not isinstance(contents, list), "pathfile returned multiple contents"
+        assert not isinstance(
+            contents, list), "pathfile returned multiple contents"
         return contents
     except GithubException as e:
         if e.status == 404:
             return None
         else:
             raise e
 
 
-def push_new_content_with_pull_request(file_path: str, repo: Repository.Repository, branch: str, contents: ContentFile.ContentFile, dataframe: pd.DataFrame, assignees: List[str]):
+def push_new_content_with_pull_request(file_path: str, repo: Repository.Repository, branch: str, contents: ContentFile.ContentFile, dataframe: pd.DataFrame, assignees: List[str], store_json: bool):
     commit_message = "Update metric :" + file_path
-    new_contents = dataframe.to_csv()
     repo.update_file(contents.path, commit_message,
-                     new_contents, contents.sha, branch)
+                     dataframe.to_csv(index=False, header=True), contents.sha, branch)
 
     create_pullrequest(repo, branch, assignees)
+    if store_json:
+        json_file_path = contents.path.replace(".csv", ".json")
+        repo.update_file(json_file_path, "Update metric :" + json_file_path,
+                         dataframe.to_json(orient="records", lines=True, date_format="iso"), contents.sha, branch)
 
 
-
-def create_file_with_pull_request(file_path: str, repo: Repository.Repository, branch: str, dataframe: pd.DataFrame, assignees: List[str]):
-    encoded_content = dataframe.to_csv()
-    repo.create_file(file_path, "New Metric "+file_path, encoded_content, branch)
+def create_file_with_pull_request(file_path: str, repo: Repository.Repository, branch: str, dataframe: pd.DataFrame, assignees: List[str], store_json: bool):
+    repo.create_file(file_path, "New Metric " +
+                     file_path, dataframe.to_csv(index=False, header=True), branch)
     create_pullrequest(repo, branch, assignees)
-
+    if store_json:
+        json_file_path = file_path.replace(".csv", ".json")
+        repo.create_file(json_file_path, "New Metric " +
+                         file_path, dataframe.to_json(orient="records", lines=True, date_format="iso"), branch)
 
 
 def create_pullrequest(repo: Repository.Repository, branch: str, assignees: List[str]):
     try:
-        pullrequest = repo.create_pull(title="New data", body="New data available",
-                         head=branch, base=repo.default_branch)
+        pullrequest = repo.create_pull(
+            title="New data", body="New data available", head=branch, base=repo.default_branch)
         print("Pull request created: " + pullrequest.html_url)
         if len(assignees) > 0:
             existing_assignees = assert_assignees_exists(repo, assignees)
             pullrequest.add_to_assignees(*existing_assignees)
     except GithubException as e:
         if e.status == 422:
             print("Pull request already exists, skipping...")
         else:
             raise e
-        
+
 
 def assert_branch_exist(repo: Repository.Repository, branch_name: str) -> None:
     try:
         branch = repo.get_branch(branch_name)
     except:
         branch = None
 
     # If the branch doesn't exist, create it
     if not branch:
         print(f"Branch {branch_name} doesn't exist, creating it...")
         master_ref = repo.get_git_ref("heads/main")
         repo.create_git_ref(f"refs/heads/{branch_name}", master_ref.object.sha)
 
+
 def assert_assignees_exists(repo: Repository.Repository, assignees: List[str]) -> List[str]:
     members = [collaborator.login for collaborator in repo.get_collaborators()]
     exising_assignees = []
     for assignee in assignees:
         if assignee not in members:
             print(f"Assignee {assignee} does not exist")
         else:
             exising_assignees.append(assignee)
-    return exising_assignees
+    return exising_assignees
```

### Comparing `datagit-0.2/datagit/query_builder.py` & `datagit-0.3/datagit/query_builder.py`

 * *Files identical despite different names*

