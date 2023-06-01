# Comparing `tmp/dktotoolkit-0.0.1a0.tar.gz` & `tmp/dktotoolkit-1.0.0a12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dktotoolkit-0.0.1a0.tar", last modified: Wed May 31 20:10:57 2023, max compression
+gzip compressed data, was "dktotoolkit-1.0.0a12.tar", last modified: Thu Jun  1 12:58:17 2023, max compression
```

## Comparing `dktotoolkit-0.0.1a0.tar` & `dktotoolkit-1.0.0a12.tar`

### file list

```diff
@@ -1,19 +1,24 @@
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-05-31 20:10:57.609572 dktotoolkit-0.0.1a0/
--rw-r--r--   0 pierre    (1000) pierre    (1000)     7426 2023-05-31 20:10:57.609572 dktotoolkit-0.0.1a0/PKG-INFO
--rw-r--r--   0 pierre    (1000) pierre    (1000)     6239 2023-05-31 19:59:17.000000 dktotoolkit-0.0.1a0/README.md
--rw-r--r--   0 pierre    (1000) pierre    (1000)      607 2023-05-31 20:10:57.609572 dktotoolkit-0.0.1a0/setup.cfg
--rw-r--r--   0 pierre    (1000) pierre    (1000)      347 2023-05-31 19:59:17.000000 dktotoolkit-0.0.1a0/setup.py
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-05-31 20:10:57.589572 dktotoolkit-0.0.1a0/src/
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-05-31 20:10:57.597572 dktotoolkit-0.0.1a0/src/dktotoolkit/
--rw-r--r--   0 pierre    (1000) pierre    (1000)      931 2023-05-31 19:59:17.000000 dktotoolkit-0.0.1a0/src/dktotoolkit/__init__.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     3162 2023-05-31 19:59:17.000000 dktotoolkit-0.0.1a0/src/dktotoolkit/_loadenv.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)      571 2023-05-31 19:59:17.000000 dktotoolkit-0.0.1a0/src/dktotoolkit/dict2obj.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2035 2023-05-31 19:59:17.000000 dktotoolkit-0.0.1a0/src/dktotoolkit/dotenv2clock.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2889 2023-05-31 19:59:17.000000 dktotoolkit-0.0.1a0/src/dktotoolkit/loadenv.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     4752 2023-05-31 20:10:39.000000 dktotoolkit-0.0.1a0/src/dktotoolkit/parse_dates.py
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-05-31 20:10:57.609572 dktotoolkit-0.0.1a0/src/dktotoolkit.egg-info/
--rw-r--r--   0 pierre    (1000) pierre    (1000)     7426 2023-05-31 20:10:57.000000 dktotoolkit-0.0.1a0/src/dktotoolkit.egg-info/PKG-INFO
--rw-r--r--   0 pierre    (1000) pierre    (1000)      396 2023-05-31 20:10:57.000000 dktotoolkit-0.0.1a0/src/dktotoolkit.egg-info/SOURCES.txt
--rw-r--r--   0 pierre    (1000) pierre    (1000)        1 2023-05-31 20:10:57.000000 dktotoolkit-0.0.1a0/src/dktotoolkit.egg-info/dependency_links.txt
--rw-r--r--   0 pierre    (1000) pierre    (1000)       80 2023-05-31 20:10:57.000000 dktotoolkit-0.0.1a0/src/dktotoolkit.egg-info/requires.txt
--rw-r--r--   0 pierre    (1000) pierre    (1000)       12 2023-05-31 20:10:57.000000 dktotoolkit-0.0.1a0/src/dktotoolkit.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 12:58:17.272873 dktotoolkit-1.0.0a12/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-01 12:58:04.000000 dktotoolkit-1.0.0a12/LICENCE.txt
+-rw-r--r--   0 root         (0) root         (0)     6669 2023-06-01 12:58:17.272873 dktotoolkit-1.0.0a12/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6239 2023-06-01 12:31:22.000000 dktotoolkit-1.0.0a12/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      632 2023-06-01 12:58:17.272873 dktotoolkit-1.0.0a12/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      347 2023-06-01 12:31:22.000000 dktotoolkit-1.0.0a12/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 12:58:17.268872 dktotoolkit-1.0.0a12/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 12:58:17.268872 dktotoolkit-1.0.0a12/src/dktotoolkit/
+-rw-rw-rw-   0 root         (0) root         (0)     1602 2023-06-01 12:31:22.000000 dktotoolkit-1.0.0a12/src/dktotoolkit/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3162 2023-06-01 12:31:22.000000 dktotoolkit-1.0.0a12/src/dktotoolkit/_loadenv.py
+-rw-rw-rw-   0 root         (0) root         (0)      971 2023-06-01 12:31:22.000000 dktotoolkit-1.0.0a12/src/dktotoolkit/_replace_with_mask.py
+-rw-rw-rw-   0 root         (0) root         (0)      571 2023-06-01 12:31:22.000000 dktotoolkit-1.0.0a12/src/dktotoolkit/dict2obj.py
+-rw-rw-rw-   0 root         (0) root         (0)     2035 2023-06-01 12:31:22.000000 dktotoolkit-1.0.0a12/src/dktotoolkit/dotenv2clock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 12:58:17.272873 dktotoolkit-1.0.0a12/src/dktotoolkit/function/
+-rw-rw-rw-   0 root         (0) root         (0)      428 2023-06-01 12:31:22.000000 dktotoolkit-1.0.0a12/src/dktotoolkit/function/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      715 2023-06-01 12:31:22.000000 dktotoolkit-1.0.0a12/src/dktotoolkit/function/_compatMode.py
+-rw-rw-rw-   0 root         (0) root         (0)     2889 2023-06-01 12:31:22.000000 dktotoolkit-1.0.0a12/src/dktotoolkit/loadenv.py
+-rw-rw-rw-   0 root         (0) root         (0)     4752 2023-06-01 12:31:22.000000 dktotoolkit-1.0.0a12/src/dktotoolkit/parse_dates.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 12:58:17.272873 dktotoolkit-1.0.0a12/src/dktotoolkit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6669 2023-06-01 12:58:17.000000 dktotoolkit-1.0.0a12/src/dktotoolkit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      523 2023-06-01 12:58:17.000000 dktotoolkit-1.0.0a12/src/dktotoolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 12:58:17.000000 dktotoolkit-1.0.0a12/src/dktotoolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       80 2023-06-01 12:58:17.000000 dktotoolkit-1.0.0a12/src/dktotoolkit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-06-01 12:58:17.000000 dktotoolkit-1.0.0a12/src/dktotoolkit.egg-info/top_level.txt
```

### Comparing `dktotoolkit-0.0.1a0/PKG-INFO` & `dktotoolkit-1.0.0a12/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,107 +1,106 @@
 Metadata-Version: 2.1
 Name: dktotoolkit
-Version: 0.0.1a0
+Version: 1.0.0a12
 Summary: A little toolkit with fancy functions
 Home-page: https://discord-catho.frama.io/module_toolkit
 Author: Pierre
-License: UNKNOWN
 Project-URL: Source Code, https://framagit.org/discord-catho/module_toolkit
-Description: # Module load dotenv
-        
-        
-        
-        ## Getting started
-        
-        To make it easy for you to get started with GitLab, here's a list of recommended next steps.
-        
-        Already a pro? Just edit this README.md and make it your own. Want to make it easy? [Use the template at the bottom](#editing-this-readme)!
-        
-        ## Add your files
-        
-        - [ ] [Create](https://docs.gitlab.com/ee/user/project/repository/web_editor.html#create-a-file) or [upload](https://docs.gitlab.com/ee/user/project/repository/web_editor.html#upload-a-file) files
-        - [ ] [Add files using the command line](https://docs.gitlab.com/ee/gitlab-basics/add-file.html#add-a-file-using-the-command-line) or push an existing Git repository with the following command:
-        
-        ```
-        cd existing_repo
-        git remote add origin https://framagit.org/discord-catho/module-load-dotenv.git
-        git branch -M main
-        git push -uf origin main
-        ```
-        
-        ## Integrate with your tools
-        
-        - [ ] [Set up project integrations](https://framagit.org/discord-catho/module-load-dotenv/-/settings/integrations)
-        
-        ## Collaborate with your team
-        
-        - [ ] [Invite team members and collaborators](https://docs.gitlab.com/ee/user/project/members/)
-        - [ ] [Create a new merge request](https://docs.gitlab.com/ee/user/project/merge_requests/creating_merge_requests.html)
-        - [ ] [Automatically close issues from merge requests](https://docs.gitlab.com/ee/user/project/issues/managing_issues.html#closing-issues-automatically)
-        - [ ] [Enable merge request approvals](https://docs.gitlab.com/ee/user/project/merge_requests/approvals/)
-        - [ ] [Automatically merge when pipeline succeeds](https://docs.gitlab.com/ee/user/project/merge_requests/merge_when_pipeline_succeeds.html)
-        
-        ## Test and Deploy
-        
-        Use the built-in continuous integration in GitLab.
-        
-        - [ ] [Get started with GitLab CI/CD](https://docs.gitlab.com/ee/ci/quick_start/index.html)
-        - [ ] [Analyze your code for known vulnerabilities with Static Application Security Testing(SAST)](https://docs.gitlab.com/ee/user/application_security/sast/)
-        - [ ] [Deploy to Kubernetes, Amazon EC2, or Amazon ECS using Auto Deploy](https://docs.gitlab.com/ee/topics/autodevops/requirements.html)
-        - [ ] [Use pull-based deployments for improved Kubernetes management](https://docs.gitlab.com/ee/user/clusters/agent/)
-        - [ ] [Set up protected environments](https://docs.gitlab.com/ee/ci/environments/protected_environments.html)
-        
-        ***
-        
-        # Editing this README
-        
-        When you're ready to make this README your own, just edit this file and use the handy template below (or feel free to structure it however you want - this is just a starting point!). Thank you to [makeareadme.com](https://www.makeareadme.com/) for this template.
-        
-        ## Suggestions for a good README
-        Every project is different, so consider which of these sections apply to yours. The sections used in the template are suggestions for most open source projects. Also keep in mind that while a README can be too long and detailed, too long is better than too short. If you think your README is too long, consider utilizing another form of documentation rather than cutting out information.
-        
-        ## Name
-        Choose a self-explaining name for your project.
-        
-        ## Description
-        Let people know what your project can do specifically. Provide context and add a link to any reference visitors might be unfamiliar with. A list of Features or a Background subsection can also be added here. If there are alternatives to your project, this is a good place to list differentiating factors.
-        
-        ## Badges
-        On some READMEs, you may see small images that convey metadata, such as whether or not all the tests are passing for the project. You can use Shields to add some to your README. Many services also have instructions for adding a badge.
-        
-        ## Visuals
-        Depending on what you are making, it can be a good idea to include screenshots or even a video (you'll frequently see GIFs rather than actual videos). Tools like ttygif can help, but check out Asciinema for a more sophisticated method.
-        
-        ## Installation
-        Within a particular ecosystem, there may be a common way of installing things, such as using Yarn, NuGet, or Homebrew. However, consider the possibility that whoever is reading your README is a novice and would like more guidance. Listing specific steps helps remove ambiguity and gets people to using your project as quickly as possible. If it only runs in a specific context like a particular programming language version or operating system or has dependencies that have to be installed manually, also add a Requirements subsection.
-        
-        ## Usage
-        Use examples liberally, and show the expected output if you can. It's helpful to have inline the smallest example of usage that you can demonstrate, while providing links to more sophisticated examples if they are too long to reasonably include in the README.
-        
-        ## Support
-        Tell people where they can go to for help. It can be any combination of an issue tracker, a chat room, an email address, etc.
-        
-        ## Roadmap
-        If you have ideas for releases in the future, it is a good idea to list them in the README.
-        
-        ## Contributing
-        State if you are open to contributions and what your requirements are for accepting them.
-        
-        For people who want to make changes to your project, it's helpful to have some documentation on how to get started. Perhaps there is a script that they should run or some environment variables that they need to set. Make these steps explicit. These instructions could also be useful to your future self.
-        
-        You can also document commands to lint the code or run tests. These steps help to ensure high code quality and reduce the likelihood that the changes inadvertently break something. Having instructions for running tests is especially helpful if it requires external setup, such as starting a Selenium server for testing in a browser.
-        
-        ## Authors and acknowledgment
-        Show your appreciation to those who have contributed to the project.
-        
-        ## License
-        For open source projects, say how it is licensed.
-        
-        ## Project status
-        If you have run out of energy or time for your project, put a note at the top of the README saying that development has slowed down or stopped completely. Someone may choose to fork your project or volunteer to step in as a maintainer or owner, allowing your project to keep going. You can also make an explicit request for maintainers.
-        
 Keywords: dotenv,.env,toolkit,parse dates
-Platform: UNKNOWN
 Requires-Python: <4,>=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: doc
 Provides-Extra: tests
+License-File: LICENCE.txt
+
+# Module load dotenv
+
+
+
+## Getting started
+
+To make it easy for you to get started with GitLab, here's a list of recommended next steps.
+
+Already a pro? Just edit this README.md and make it your own. Want to make it easy? [Use the template at the bottom](#editing-this-readme)!
+
+## Add your files
+
+- [ ] [Create](https://docs.gitlab.com/ee/user/project/repository/web_editor.html#create-a-file) or [upload](https://docs.gitlab.com/ee/user/project/repository/web_editor.html#upload-a-file) files
+- [ ] [Add files using the command line](https://docs.gitlab.com/ee/gitlab-basics/add-file.html#add-a-file-using-the-command-line) or push an existing Git repository with the following command:
+
+```
+cd existing_repo
+git remote add origin https://framagit.org/discord-catho/module-load-dotenv.git
+git branch -M main
+git push -uf origin main
+```
+
+## Integrate with your tools
+
+- [ ] [Set up project integrations](https://framagit.org/discord-catho/module-load-dotenv/-/settings/integrations)
+
+## Collaborate with your team
+
+- [ ] [Invite team members and collaborators](https://docs.gitlab.com/ee/user/project/members/)
+- [ ] [Create a new merge request](https://docs.gitlab.com/ee/user/project/merge_requests/creating_merge_requests.html)
+- [ ] [Automatically close issues from merge requests](https://docs.gitlab.com/ee/user/project/issues/managing_issues.html#closing-issues-automatically)
+- [ ] [Enable merge request approvals](https://docs.gitlab.com/ee/user/project/merge_requests/approvals/)
+- [ ] [Automatically merge when pipeline succeeds](https://docs.gitlab.com/ee/user/project/merge_requests/merge_when_pipeline_succeeds.html)
+
+## Test and Deploy
+
+Use the built-in continuous integration in GitLab.
+
+- [ ] [Get started with GitLab CI/CD](https://docs.gitlab.com/ee/ci/quick_start/index.html)
+- [ ] [Analyze your code for known vulnerabilities with Static Application Security Testing(SAST)](https://docs.gitlab.com/ee/user/application_security/sast/)
+- [ ] [Deploy to Kubernetes, Amazon EC2, or Amazon ECS using Auto Deploy](https://docs.gitlab.com/ee/topics/autodevops/requirements.html)
+- [ ] [Use pull-based deployments for improved Kubernetes management](https://docs.gitlab.com/ee/user/clusters/agent/)
+- [ ] [Set up protected environments](https://docs.gitlab.com/ee/ci/environments/protected_environments.html)
+
+***
+
+# Editing this README
+
+When you're ready to make this README your own, just edit this file and use the handy template below (or feel free to structure it however you want - this is just a starting point!). Thank you to [makeareadme.com](https://www.makeareadme.com/) for this template.
+
+## Suggestions for a good README
+Every project is different, so consider which of these sections apply to yours. The sections used in the template are suggestions for most open source projects. Also keep in mind that while a README can be too long and detailed, too long is better than too short. If you think your README is too long, consider utilizing another form of documentation rather than cutting out information.
+
+## Name
+Choose a self-explaining name for your project.
+
+## Description
+Let people know what your project can do specifically. Provide context and add a link to any reference visitors might be unfamiliar with. A list of Features or a Background subsection can also be added here. If there are alternatives to your project, this is a good place to list differentiating factors.
+
+## Badges
+On some READMEs, you may see small images that convey metadata, such as whether or not all the tests are passing for the project. You can use Shields to add some to your README. Many services also have instructions for adding a badge.
+
+## Visuals
+Depending on what you are making, it can be a good idea to include screenshots or even a video (you'll frequently see GIFs rather than actual videos). Tools like ttygif can help, but check out Asciinema for a more sophisticated method.
+
+## Installation
+Within a particular ecosystem, there may be a common way of installing things, such as using Yarn, NuGet, or Homebrew. However, consider the possibility that whoever is reading your README is a novice and would like more guidance. Listing specific steps helps remove ambiguity and gets people to using your project as quickly as possible. If it only runs in a specific context like a particular programming language version or operating system or has dependencies that have to be installed manually, also add a Requirements subsection.
+
+## Usage
+Use examples liberally, and show the expected output if you can. It's helpful to have inline the smallest example of usage that you can demonstrate, while providing links to more sophisticated examples if they are too long to reasonably include in the README.
+
+## Support
+Tell people where they can go to for help. It can be any combination of an issue tracker, a chat room, an email address, etc.
+
+## Roadmap
+If you have ideas for releases in the future, it is a good idea to list them in the README.
+
+## Contributing
+State if you are open to contributions and what your requirements are for accepting them.
+
+For people who want to make changes to your project, it's helpful to have some documentation on how to get started. Perhaps there is a script that they should run or some environment variables that they need to set. Make these steps explicit. These instructions could also be useful to your future self.
+
+You can also document commands to lint the code or run tests. These steps help to ensure high code quality and reduce the likelihood that the changes inadvertently break something. Having instructions for running tests is especially helpful if it requires external setup, such as starting a Selenium server for testing in a browser.
+
+## Authors and acknowledgment
+Show your appreciation to those who have contributed to the project.
+
+## License
+For open source projects, say how it is licensed.
+
+## Project status
+If you have run out of energy or time for your project, put a note at the top of the README saying that development has slowed down or stopped completely. Someone may choose to fork your project or volunteer to step in as a maintainer or owner, allowing your project to keep going. You can also make an explicit request for maintainers.
```

### Comparing `dktotoolkit-0.0.1a0/README.md` & `dktotoolkit-1.0.0a12/README.md`

 * *Files identical despite different names*

### Comparing `dktotoolkit-0.0.1a0/setup.cfg` & `dktotoolkit-1.0.0a12/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 [metadata]
 name = dktotoolkit
-version = 0.0.1a0
+version = 1.0.0a12
 author = Pierre
 description = A little toolkit with fancy functions
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://discord-catho.frama.io/module_toolkit
 project_urls = 
 	Source Code = https://framagit.org/discord-catho/module_toolkit
 keywords = dotenv, .env, toolkit, parse dates
 
 [options]
 python_requires = >=3.9, <4
 package_dir = 
 	=src
-packages = dktotoolkit
+packages = 
+	dktotoolkit
+	dktotoolkit.function
 
 [options.extras_require]
 doc = 
 	sphinx==6.2.1
 	sphinx-rtd-theme==1.2.1
 	myst-parser==1.0.0
 tests =
```

### Comparing `dktotoolkit-0.0.1a0/src/dktotoolkit/_loadenv.py` & `dktotoolkit-1.0.0a12/src/dktotoolkit/_loadenv.py`

 * *Files identical despite different names*

### Comparing `dktotoolkit-0.0.1a0/src/dktotoolkit/dict2obj.py` & `dktotoolkit-1.0.0a12/src/dktotoolkit/dict2obj.py`

 * *Files identical despite different names*

### Comparing `dktotoolkit-0.0.1a0/src/dktotoolkit/dotenv2clock.py` & `dktotoolkit-1.0.0a12/src/dktotoolkit/dotenv2clock.py`

 * *Files identical despite different names*

### Comparing `dktotoolkit-0.0.1a0/src/dktotoolkit/loadenv.py` & `dktotoolkit-1.0.0a12/src/dktotoolkit/loadenv.py`

 * *Files identical despite different names*

### Comparing `dktotoolkit-0.0.1a0/src/dktotoolkit/parse_dates.py` & `dktotoolkit-1.0.0a12/src/dktotoolkit/parse_dates.py`

 * *Files identical despite different names*

### Comparing `dktotoolkit-0.0.1a0/src/dktotoolkit.egg-info/PKG-INFO` & `dktotoolkit-1.0.0a12/src/dktotoolkit.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,107 +1,106 @@
 Metadata-Version: 2.1
 Name: dktotoolkit
-Version: 0.0.1a0
+Version: 1.0.0a12
 Summary: A little toolkit with fancy functions
 Home-page: https://discord-catho.frama.io/module_toolkit
 Author: Pierre
-License: UNKNOWN
 Project-URL: Source Code, https://framagit.org/discord-catho/module_toolkit
-Description: # Module load dotenv
-        
-        
-        
-        ## Getting started
-        
-        To make it easy for you to get started with GitLab, here's a list of recommended next steps.
-        
-        Already a pro? Just edit this README.md and make it your own. Want to make it easy? [Use the template at the bottom](#editing-this-readme)!
-        
-        ## Add your files
-        
-        - [ ] [Create](https://docs.gitlab.com/ee/user/project/repository/web_editor.html#create-a-file) or [upload](https://docs.gitlab.com/ee/user/project/repository/web_editor.html#upload-a-file) files
-        - [ ] [Add files using the command line](https://docs.gitlab.com/ee/gitlab-basics/add-file.html#add-a-file-using-the-command-line) or push an existing Git repository with the following command:
-        
-        ```
-        cd existing_repo
-        git remote add origin https://framagit.org/discord-catho/module-load-dotenv.git
-        git branch -M main
-        git push -uf origin main
-        ```
-        
-        ## Integrate with your tools
-        
-        - [ ] [Set up project integrations](https://framagit.org/discord-catho/module-load-dotenv/-/settings/integrations)
-        
-        ## Collaborate with your team
-        
-        - [ ] [Invite team members and collaborators](https://docs.gitlab.com/ee/user/project/members/)
-        - [ ] [Create a new merge request](https://docs.gitlab.com/ee/user/project/merge_requests/creating_merge_requests.html)
-        - [ ] [Automatically close issues from merge requests](https://docs.gitlab.com/ee/user/project/issues/managing_issues.html#closing-issues-automatically)
-        - [ ] [Enable merge request approvals](https://docs.gitlab.com/ee/user/project/merge_requests/approvals/)
-        - [ ] [Automatically merge when pipeline succeeds](https://docs.gitlab.com/ee/user/project/merge_requests/merge_when_pipeline_succeeds.html)
-        
-        ## Test and Deploy
-        
-        Use the built-in continuous integration in GitLab.
-        
-        - [ ] [Get started with GitLab CI/CD](https://docs.gitlab.com/ee/ci/quick_start/index.html)
-        - [ ] [Analyze your code for known vulnerabilities with Static Application Security Testing(SAST)](https://docs.gitlab.com/ee/user/application_security/sast/)
-        - [ ] [Deploy to Kubernetes, Amazon EC2, or Amazon ECS using Auto Deploy](https://docs.gitlab.com/ee/topics/autodevops/requirements.html)
-        - [ ] [Use pull-based deployments for improved Kubernetes management](https://docs.gitlab.com/ee/user/clusters/agent/)
-        - [ ] [Set up protected environments](https://docs.gitlab.com/ee/ci/environments/protected_environments.html)
-        
-        ***
-        
-        # Editing this README
-        
-        When you're ready to make this README your own, just edit this file and use the handy template below (or feel free to structure it however you want - this is just a starting point!). Thank you to [makeareadme.com](https://www.makeareadme.com/) for this template.
-        
-        ## Suggestions for a good README
-        Every project is different, so consider which of these sections apply to yours. The sections used in the template are suggestions for most open source projects. Also keep in mind that while a README can be too long and detailed, too long is better than too short. If you think your README is too long, consider utilizing another form of documentation rather than cutting out information.
-        
-        ## Name
-        Choose a self-explaining name for your project.
-        
-        ## Description
-        Let people know what your project can do specifically. Provide context and add a link to any reference visitors might be unfamiliar with. A list of Features or a Background subsection can also be added here. If there are alternatives to your project, this is a good place to list differentiating factors.
-        
-        ## Badges
-        On some READMEs, you may see small images that convey metadata, such as whether or not all the tests are passing for the project. You can use Shields to add some to your README. Many services also have instructions for adding a badge.
-        
-        ## Visuals
-        Depending on what you are making, it can be a good idea to include screenshots or even a video (you'll frequently see GIFs rather than actual videos). Tools like ttygif can help, but check out Asciinema for a more sophisticated method.
-        
-        ## Installation
-        Within a particular ecosystem, there may be a common way of installing things, such as using Yarn, NuGet, or Homebrew. However, consider the possibility that whoever is reading your README is a novice and would like more guidance. Listing specific steps helps remove ambiguity and gets people to using your project as quickly as possible. If it only runs in a specific context like a particular programming language version or operating system or has dependencies that have to be installed manually, also add a Requirements subsection.
-        
-        ## Usage
-        Use examples liberally, and show the expected output if you can. It's helpful to have inline the smallest example of usage that you can demonstrate, while providing links to more sophisticated examples if they are too long to reasonably include in the README.
-        
-        ## Support
-        Tell people where they can go to for help. It can be any combination of an issue tracker, a chat room, an email address, etc.
-        
-        ## Roadmap
-        If you have ideas for releases in the future, it is a good idea to list them in the README.
-        
-        ## Contributing
-        State if you are open to contributions and what your requirements are for accepting them.
-        
-        For people who want to make changes to your project, it's helpful to have some documentation on how to get started. Perhaps there is a script that they should run or some environment variables that they need to set. Make these steps explicit. These instructions could also be useful to your future self.
-        
-        You can also document commands to lint the code or run tests. These steps help to ensure high code quality and reduce the likelihood that the changes inadvertently break something. Having instructions for running tests is especially helpful if it requires external setup, such as starting a Selenium server for testing in a browser.
-        
-        ## Authors and acknowledgment
-        Show your appreciation to those who have contributed to the project.
-        
-        ## License
-        For open source projects, say how it is licensed.
-        
-        ## Project status
-        If you have run out of energy or time for your project, put a note at the top of the README saying that development has slowed down or stopped completely. Someone may choose to fork your project or volunteer to step in as a maintainer or owner, allowing your project to keep going. You can also make an explicit request for maintainers.
-        
 Keywords: dotenv,.env,toolkit,parse dates
-Platform: UNKNOWN
 Requires-Python: <4,>=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: doc
 Provides-Extra: tests
+License-File: LICENCE.txt
+
+# Module load dotenv
+
+
+
+## Getting started
+
+To make it easy for you to get started with GitLab, here's a list of recommended next steps.
+
+Already a pro? Just edit this README.md and make it your own. Want to make it easy? [Use the template at the bottom](#editing-this-readme)!
+
+## Add your files
+
+- [ ] [Create](https://docs.gitlab.com/ee/user/project/repository/web_editor.html#create-a-file) or [upload](https://docs.gitlab.com/ee/user/project/repository/web_editor.html#upload-a-file) files
+- [ ] [Add files using the command line](https://docs.gitlab.com/ee/gitlab-basics/add-file.html#add-a-file-using-the-command-line) or push an existing Git repository with the following command:
+
+```
+cd existing_repo
+git remote add origin https://framagit.org/discord-catho/module-load-dotenv.git
+git branch -M main
+git push -uf origin main
+```
+
+## Integrate with your tools
+
+- [ ] [Set up project integrations](https://framagit.org/discord-catho/module-load-dotenv/-/settings/integrations)
+
+## Collaborate with your team
+
+- [ ] [Invite team members and collaborators](https://docs.gitlab.com/ee/user/project/members/)
+- [ ] [Create a new merge request](https://docs.gitlab.com/ee/user/project/merge_requests/creating_merge_requests.html)
+- [ ] [Automatically close issues from merge requests](https://docs.gitlab.com/ee/user/project/issues/managing_issues.html#closing-issues-automatically)
+- [ ] [Enable merge request approvals](https://docs.gitlab.com/ee/user/project/merge_requests/approvals/)
+- [ ] [Automatically merge when pipeline succeeds](https://docs.gitlab.com/ee/user/project/merge_requests/merge_when_pipeline_succeeds.html)
+
+## Test and Deploy
+
+Use the built-in continuous integration in GitLab.
+
+- [ ] [Get started with GitLab CI/CD](https://docs.gitlab.com/ee/ci/quick_start/index.html)
+- [ ] [Analyze your code for known vulnerabilities with Static Application Security Testing(SAST)](https://docs.gitlab.com/ee/user/application_security/sast/)
+- [ ] [Deploy to Kubernetes, Amazon EC2, or Amazon ECS using Auto Deploy](https://docs.gitlab.com/ee/topics/autodevops/requirements.html)
+- [ ] [Use pull-based deployments for improved Kubernetes management](https://docs.gitlab.com/ee/user/clusters/agent/)
+- [ ] [Set up protected environments](https://docs.gitlab.com/ee/ci/environments/protected_environments.html)
+
+***
+
+# Editing this README
+
+When you're ready to make this README your own, just edit this file and use the handy template below (or feel free to structure it however you want - this is just a starting point!). Thank you to [makeareadme.com](https://www.makeareadme.com/) for this template.
+
+## Suggestions for a good README
+Every project is different, so consider which of these sections apply to yours. The sections used in the template are suggestions for most open source projects. Also keep in mind that while a README can be too long and detailed, too long is better than too short. If you think your README is too long, consider utilizing another form of documentation rather than cutting out information.
+
+## Name
+Choose a self-explaining name for your project.
+
+## Description
+Let people know what your project can do specifically. Provide context and add a link to any reference visitors might be unfamiliar with. A list of Features or a Background subsection can also be added here. If there are alternatives to your project, this is a good place to list differentiating factors.
+
+## Badges
+On some READMEs, you may see small images that convey metadata, such as whether or not all the tests are passing for the project. You can use Shields to add some to your README. Many services also have instructions for adding a badge.
+
+## Visuals
+Depending on what you are making, it can be a good idea to include screenshots or even a video (you'll frequently see GIFs rather than actual videos). Tools like ttygif can help, but check out Asciinema for a more sophisticated method.
+
+## Installation
+Within a particular ecosystem, there may be a common way of installing things, such as using Yarn, NuGet, or Homebrew. However, consider the possibility that whoever is reading your README is a novice and would like more guidance. Listing specific steps helps remove ambiguity and gets people to using your project as quickly as possible. If it only runs in a specific context like a particular programming language version or operating system or has dependencies that have to be installed manually, also add a Requirements subsection.
+
+## Usage
+Use examples liberally, and show the expected output if you can. It's helpful to have inline the smallest example of usage that you can demonstrate, while providing links to more sophisticated examples if they are too long to reasonably include in the README.
+
+## Support
+Tell people where they can go to for help. It can be any combination of an issue tracker, a chat room, an email address, etc.
+
+## Roadmap
+If you have ideas for releases in the future, it is a good idea to list them in the README.
+
+## Contributing
+State if you are open to contributions and what your requirements are for accepting them.
+
+For people who want to make changes to your project, it's helpful to have some documentation on how to get started. Perhaps there is a script that they should run or some environment variables that they need to set. Make these steps explicit. These instructions could also be useful to your future self.
+
+You can also document commands to lint the code or run tests. These steps help to ensure high code quality and reduce the likelihood that the changes inadvertently break something. Having instructions for running tests is especially helpful if it requires external setup, such as starting a Selenium server for testing in a browser.
+
+## Authors and acknowledgment
+Show your appreciation to those who have contributed to the project.
+
+## License
+For open source projects, say how it is licensed.
+
+## Project status
+If you have run out of energy or time for your project, put a note at the top of the README saying that development has slowed down or stopped completely. Someone may choose to fork your project or volunteer to step in as a maintainer or owner, allowing your project to keep going. You can also make an explicit request for maintainers.
```

