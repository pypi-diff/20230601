# Comparing `tmp/iga-1.0.3.tar.gz` & `tmp/iga-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iga-1.0.3.tar", last modified: Wed May 24 21:09:36 2023, max compression
+gzip compressed data, was "iga-1.1.0.tar", last modified: Wed May 31 23:12:01 2023, max compression
```

## Comparing `iga-1.0.3.tar` & `iga-1.1.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-05-24 21:09:36.324432 iga-1.0.3/
--rw-r--r--   0 mhucka     (503) staff       (20)     1527 2023-05-23 15:45:07.000000 iga-1.0.3/LICENSE
--rw-r--r--   0 mhucka     (503) staff       (20)    38059 2023-05-24 21:09:36.324552 iga-1.0.3/PKG-INFO
--rw-r--r--   0 mhucka     (503) staff       (20)    37153 2023-05-24 21:02:11.000000 iga-1.0.3/README.md
-drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-05-24 21:09:36.321238 iga-1.0.3/iga/
--rw-r--r--   0 mhucka     (503) staff       (20)     1458 2023-05-24 21:02:11.000000 iga-1.0.3/iga/__init__.py
--rw-r--r--   0 mhucka     (503) staff       (20)      905 2023-05-23 15:45:07.000000 iga-1.0.3/iga/__main__.py
--rw-r--r--   0 mhucka     (503) staff       (20)    34712 2023-05-23 15:45:07.000000 iga-1.0.3/iga/cli.py
--rw-r--r--   0 mhucka     (503) staff       (20)     3317 2023-05-23 15:45:07.000000 iga-1.0.3/iga/data_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)     2859 2023-05-23 15:45:07.000000 iga-1.0.3/iga/doi.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1252 2023-05-23 15:45:07.000000 iga-1.0.3/iga/exceptions.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1514 2023-05-23 15:45:07.000000 iga-1.0.3/iga/exit_codes.py
--rw-r--r--   0 mhucka     (503) staff       (20)    15499 2023-05-23 15:45:07.000000 iga-1.0.3/iga/github.py
--rw-r--r--   0 mhucka     (503) staff       (20)     4901 2023-05-23 15:45:07.000000 iga-1.0.3/iga/id_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)    18504 2023-05-23 15:45:07.000000 iga-1.0.3/iga/invenio.py
--rw-r--r--   0 mhucka     (503) staff       (20)     2064 2023-05-24 21:02:11.000000 iga-1.0.3/iga/json_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)   242887 2023-05-23 15:45:07.000000 iga-1.0.3/iga/licenses.py
--rw-r--r--   0 mhucka     (503) staff       (20)    70404 2023-05-23 15:45:07.000000 iga-1.0.3/iga/metadata.py
--rw-r--r--   0 mhucka     (503) staff       (20)    14593 2023-05-24 19:21:29.000000 iga-1.0.3/iga/name_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)     5273 2023-05-23 15:45:07.000000 iga-1.0.3/iga/orcid.py
--rw-r--r--   0 mhucka     (503) staff       (20)     5147 2023-05-23 15:45:07.000000 iga-1.0.3/iga/reference.py
--rw-r--r--   0 mhucka     (503) staff       (20)     3969 2023-05-23 15:45:07.000000 iga-1.0.3/iga/ror.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1624 2023-05-23 15:45:07.000000 iga-1.0.3/iga/text_utils.py
-drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-05-24 21:09:36.322023 iga-1.0.3/iga.egg-info/
--rw-r--r--   0 mhucka     (503) staff       (20)    38059 2023-05-24 21:09:36.000000 iga-1.0.3/iga.egg-info/PKG-INFO
--rw-r--r--   0 mhucka     (503) staff       (20)      930 2023-05-24 21:09:36.000000 iga-1.0.3/iga.egg-info/SOURCES.txt
--rw-r--r--   0 mhucka     (503) staff       (20)        1 2023-05-24 21:09:36.000000 iga-1.0.3/iga.egg-info/dependency_links.txt
--rw-r--r--   0 mhucka     (503) staff       (20)       58 2023-05-24 21:09:36.000000 iga-1.0.3/iga.egg-info/entry_points.txt
--rw-r--r--   0 mhucka     (503) staff       (20)        1 2023-05-24 21:09:36.000000 iga-1.0.3/iga.egg-info/not-zip-safe
--rw-r--r--   0 mhucka     (503) staff       (20)      657 2023-05-24 21:09:36.000000 iga-1.0.3/iga.egg-info/requires.txt
--rw-r--r--   0 mhucka     (503) staff       (20)        4 2023-05-24 21:09:36.000000 iga-1.0.3/iga.egg-info/top_level.txt
--rw-r--r--   0 mhucka     (503) staff       (20)     1095 2023-05-24 21:09:36.324861 iga-1.0.3/setup.cfg
--rwxr-xr-x   0 mhucka     (503) staff       (20)     1708 2023-05-23 15:45:07.000000 iga-1.0.3/setup.py
-drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-05-24 21:09:36.324320 iga-1.0.3/tests/
--rw-r--r--   0 mhucka     (503) staff       (20)     6117 2023-05-23 15:45:07.000000 iga-1.0.3/tests/test_cli.py
--rw-r--r--   0 mhucka     (503) staff       (20)     4481 2023-05-23 15:45:07.000000 iga-1.0.3/tests/test_data_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1417 2023-05-23 15:45:07.000000 iga-1.0.3/tests/test_doi.py
--rw-r--r--   0 mhucka     (503) staff       (20)      686 2023-05-23 15:45:07.000000 iga-1.0.3/tests/test_exceptions.py
--rw-r--r--   0 mhucka     (503) staff       (20)      177 2023-05-23 15:45:07.000000 iga-1.0.3/tests/test_exit_codes.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1446 2023-05-23 15:45:07.000000 iga-1.0.3/tests/test_github.py
--rw-r--r--   0 mhucka     (503) staff       (20)     3015 2023-05-23 15:45:07.000000 iga-1.0.3/tests/test_github_mocks.py
--rw-r--r--   0 mhucka     (503) staff       (20)     3666 2023-05-23 15:45:07.000000 iga-1.0.3/tests/test_id_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)      641 2023-05-23 15:45:07.000000 iga-1.0.3/tests/test_init.py
--rw-r--r--   0 mhucka     (503) staff       (20)    49214 2023-05-23 15:45:07.000000 iga-1.0.3/tests/test_is_person.py
--rw-r--r--   0 mhucka     (503) staff       (20)      912 2023-05-23 15:45:07.000000 iga-1.0.3/tests/test_licenses.py
--rw-r--r--   0 mhucka     (503) staff       (20)     4408 2023-05-23 15:45:07.000000 iga-1.0.3/tests/test_name_splitting.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1829 2023-05-23 15:45:07.000000 iga-1.0.3/tests/test_name_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1054 2023-05-23 15:45:07.000000 iga-1.0.3/tests/test_orcid.py
--rw-r--r--   0 mhucka     (503) staff       (20)     5997 2023-05-23 15:45:07.000000 iga-1.0.3/tests/test_record_from_codemeta.py
--rw-r--r--   0 mhucka     (503) staff       (20)     6026 2023-05-23 15:45:07.000000 iga-1.0.3/tests/test_reference.py
--rw-r--r--   0 mhucka     (503) staff       (20)      947 2023-05-23 15:45:07.000000 iga-1.0.3/tests/test_ror.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1375 2023-05-23 15:45:07.000000 iga-1.0.3/tests/test_text_utils.py
+drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-05-31 23:12:01.483243 iga-1.1.0/
+-rw-r--r--   0 mhucka     (503) staff       (20)     1527 2023-05-31 23:10:37.000000 iga-1.1.0/LICENSE
+-rw-r--r--   0 mhucka     (503) staff       (20)    39913 2023-05-31 23:12:01.483344 iga-1.1.0/PKG-INFO
+-rw-r--r--   0 mhucka     (503) staff       (20)    39007 2023-05-31 23:10:37.000000 iga-1.1.0/README.md
+drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-05-31 23:12:01.480025 iga-1.1.0/iga/
+-rw-r--r--   0 mhucka     (503) staff       (20)     1458 2023-05-31 23:11:02.000000 iga-1.1.0/iga/__init__.py
+-rw-r--r--   0 mhucka     (503) staff       (20)      905 2023-05-31 23:10:37.000000 iga-1.1.0/iga/__main__.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    35365 2023-05-31 23:10:37.000000 iga-1.1.0/iga/cli.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     3317 2023-05-31 23:10:37.000000 iga-1.1.0/iga/data_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     2859 2023-05-31 23:10:37.000000 iga-1.1.0/iga/doi.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1252 2023-05-31 23:10:37.000000 iga-1.1.0/iga/exceptions.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1514 2023-05-31 23:10:37.000000 iga-1.1.0/iga/exit_codes.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    15499 2023-05-31 23:10:37.000000 iga-1.1.0/iga/github.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     4901 2023-05-31 23:10:37.000000 iga-1.1.0/iga/id_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    18747 2023-05-31 23:10:37.000000 iga-1.1.0/iga/invenio.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     2064 2023-05-31 23:10:37.000000 iga-1.1.0/iga/json_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)   242887 2023-05-31 23:10:37.000000 iga-1.1.0/iga/licenses.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    70404 2023-05-31 23:10:37.000000 iga-1.1.0/iga/metadata.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    14563 2023-05-31 23:10:37.000000 iga-1.1.0/iga/name_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     5273 2023-05-31 23:10:37.000000 iga-1.1.0/iga/orcid.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     5147 2023-05-31 23:10:37.000000 iga-1.1.0/iga/reference.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     3969 2023-05-31 23:10:37.000000 iga-1.1.0/iga/ror.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1624 2023-05-31 23:10:37.000000 iga-1.1.0/iga/text_utils.py
+drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-05-31 23:12:01.480886 iga-1.1.0/iga.egg-info/
+-rw-r--r--   0 mhucka     (503) staff       (20)    39913 2023-05-31 23:12:01.000000 iga-1.1.0/iga.egg-info/PKG-INFO
+-rw-r--r--   0 mhucka     (503) staff       (20)      930 2023-05-31 23:12:01.000000 iga-1.1.0/iga.egg-info/SOURCES.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)        1 2023-05-31 23:12:01.000000 iga-1.1.0/iga.egg-info/dependency_links.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)       58 2023-05-31 23:12:01.000000 iga-1.1.0/iga.egg-info/entry_points.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)        1 2023-05-31 23:12:01.000000 iga-1.1.0/iga.egg-info/not-zip-safe
+-rw-r--r--   0 mhucka     (503) staff       (20)      659 2023-05-31 23:12:01.000000 iga-1.1.0/iga.egg-info/requires.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)        4 2023-05-31 23:12:01.000000 iga-1.1.0/iga.egg-info/top_level.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)     1095 2023-05-31 23:12:01.483691 iga-1.1.0/setup.cfg
+-rwxr-xr-x   0 mhucka     (503) staff       (20)     1708 2023-05-31 23:10:37.000000 iga-1.1.0/setup.py
+drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-05-31 23:12:01.483131 iga-1.1.0/tests/
+-rw-r--r--   0 mhucka     (503) staff       (20)     6117 2023-05-31 23:10:37.000000 iga-1.1.0/tests/test_cli.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     4481 2023-05-31 23:10:37.000000 iga-1.1.0/tests/test_data_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1417 2023-05-31 23:10:37.000000 iga-1.1.0/tests/test_doi.py
+-rw-r--r--   0 mhucka     (503) staff       (20)      686 2023-05-31 23:10:37.000000 iga-1.1.0/tests/test_exceptions.py
+-rw-r--r--   0 mhucka     (503) staff       (20)      177 2023-05-31 23:10:37.000000 iga-1.1.0/tests/test_exit_codes.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1446 2023-05-31 23:10:37.000000 iga-1.1.0/tests/test_github.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     3015 2023-05-31 23:10:37.000000 iga-1.1.0/tests/test_github_mocks.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     3666 2023-05-31 23:10:37.000000 iga-1.1.0/tests/test_id_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)      641 2023-05-31 23:10:37.000000 iga-1.1.0/tests/test_init.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    49214 2023-05-31 23:10:37.000000 iga-1.1.0/tests/test_is_person.py
+-rw-r--r--   0 mhucka     (503) staff       (20)      912 2023-05-31 23:10:37.000000 iga-1.1.0/tests/test_licenses.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     4408 2023-05-31 23:10:37.000000 iga-1.1.0/tests/test_name_splitting.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1829 2023-05-31 23:10:37.000000 iga-1.1.0/tests/test_name_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1054 2023-05-31 23:10:37.000000 iga-1.1.0/tests/test_orcid.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     5997 2023-05-31 23:10:37.000000 iga-1.1.0/tests/test_record_from_codemeta.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     6026 2023-05-31 23:10:37.000000 iga-1.1.0/tests/test_reference.py
+-rw-r--r--   0 mhucka     (503) staff       (20)      947 2023-05-31 23:10:37.000000 iga-1.1.0/tests/test_ror.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1375 2023-05-31 23:10:37.000000 iga-1.1.0/tests/test_text_utils.py
```

### Comparing `iga-1.0.3/LICENSE` & `iga-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `iga-1.0.3/PKG-INFO` & `iga-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iga
-Version: 1.0.3
+Version: 1.1.0
 Summary: InvenioRDM GitHub Archiver
 Home-page: https://github.com/caltechlibrary/iga
 Author: Michael Hucka
 Author-email: helpdesk@library.caltech.edu
 License: https://github.com/caltechlibrary/iga/blob/main/LICENSE
 Project-URL: Source Code, https://github.com/caltechlibrary/iga
 Project-URL: Bug Tracker, https://github.com/caltechlibrary/iga/issues
@@ -77,20 +77,23 @@
 
 ### IGA as a standalone program
 
 Please choose an approach that suits your situation and preferences.
 
 <details><summary><h4><i>Alternative 1: using <code>pipx</code></i></h4></summary>
 
-[Pipx](https://pypa.github.io/pipx/) lets you install Python programs in a way that isolates Python dependencies, and yet the resulting `iga` command can be run from any shell and directory &ndash; like any normal program on your computer. If you use `pipx` on your system, you can install IGA with the following command:
+[Pipx](https://pypa.github.io/pipx/) lets you install Python programs in a way that isolates Python dependencies from other Python programs on your system, and yet the resulting `iga` command can be run from any shell and directory &ndash; like any normal program on your computer. If you use `pipx` on your system, you can install IGA with the following command:
 ```sh
 pipx install iga
 ```
 
-Pipx can also let you run IGA directly using `pipx run iga`, although in that case, you must always prefix every IGA command with `pipx run`.  Consult the [documentation for `pipx run`](https://github.com/pypa/pipx#walkthrough-running-an-application-in-a-temporary-virtual-environment) for more information.
+After installation, a program named `iga` should end up in a location where other command-line programs are installed on your computer.  Test it by running the following command in a shell:
+```shell
+iga --help
+```
 </details>
 
 <details><summary><h4><i>Alternative 2: using <code>pip</code></i></h4></summary>
 
 IGA is available from the [Python package repository PyPI](https://pypi.org) and can be installed using [`pip`](https://pip.pypa.io/en/stable/installing/):
 ```sh
 python3 -m pip install iga
@@ -98,14 +101,19 @@
 
 As an alternative to getting it from [PyPI](https://pypi.org), you can install `iga` directly from GitHub:
 ```sh
 python3 -m pip install git+https://github.com/caltechlibrary/iga.git
 ```
 
 _If you already installed IGA once before_, and want to update to the latest version, add `--upgrade` to the end of either command line above.
+
+After installation, a program named `iga` should end up in a location where other command-line programs are installed on your computer.  Test it by running the following command in a shell:
+```shell
+iga --help
+```
 </details>
 
 <details><summary><h4><i>Alternative 3: from sources</i></h4></summary>
 
 If  you prefer to install IGA directly from the source code, first obtain a copy by either downloading the source archive from the [IGA releases page on GitHub](https://github.com/caltechlibrary/iga/releases), or by using `git` to clone the repository to a location on your computer. For example,
 ```sh
 git clone https://github.com/caltechlibrary/iga
@@ -114,19 +122,14 @@
 Next, after getting a copy of the files,  run `setup.py` inside the code directory:
 ```sh
 cd iga
 python3 setup.py install
 ```
 </details>
 
-After installation, a program named `iga` should end up in a location where other command-line programs are installed on your computer.  Test it by running the following command in a shell:
-```shell
-iga --help
-```
-
 
 ### IGA as a GitHub Actions workflow
 
 A [GitHub Actions](https://docs.github.com/en/actions) workflow is an automated process that runs on GitHub's servers under control of a file in your repository. Follow these steps to create the IGA workflow file:
 
 1. In the main branch of your GitHub repository, create a `.github/workflows` directory
 2. In the `.github/workflows` directory, create a file named (e.g.) `iga.yml` and copy the [following contents](https://raw.githubusercontent.com/caltechlibrary/iga/main/sample-workflow.yml) into it:
@@ -278,15 +281,15 @@
 
 A personal access token (PAT) for making API calls to the InvenioRDM server must be also supplied when invoking IGA. The preferred method is to set the value of the environment variable `INVENIO_TOKEN`. Alternatively, you can use the option `--invenio-token` to pass the token on the command line, but **you are strongly advised to avoid this practice because it is insecure**.
 
 To obtain a PAT from an InvenioRDM server, first log in to the server, then visit the page at `/account/settings/applications` and use the interface there to create a token. The token will be a long string of alphanumeric characters such as `OH0KYf4PGYQGnCM4b53ejSGicOC4s4YnonRVzGJbWxY`; set the value of the variable `INVENIO_TOKEN` to this string.
 
 ### Providing a GitHub access token
 
-It _may_ be possible to run IGA without providing a GitHub access token. GitHub allows up to 60 API calls per minute when running without credentials, and though IGA makes several API calls to GitHub each time it runs, for some repositories IGA will not hit the limit. However, if you run IGA multiple times in a row or your repository has many contributors, then you may need to supply a GitHub access token. The preferred way of doing that is to set the value of the environment variable `GITHUB_TOKEN`. Alternatively, you can use the option `--github-token` to pass the token on the command line, but **you are strongly advised to avoid this practice because it is insecure**.  To obtain a PAT from GitHub, visit https://docs.github.com/en/authentication and follow the instructions for creating a "classic" personal access token.
+It _may_ be possible to run IGA without providing a GitHub access token. GitHub allows up to 60 API calls per minute when running without credentials, and though IGA makes several API calls to GitHub each time it runs, for some public repositories IGA will not hit the limit. However, if you are archiving a private repository, run IGA multiple times in a row, or the repository has many contributors, then you will need to supply a GitHub access token. The preferred way of doing that is to set the value of the environment variable `GITHUB_TOKEN`. Alternatively, you can use the option `--github-token` to pass the token on the command line, but **you are strongly advised to avoid this practice because it is insecure**.  To obtain a PAT from GitHub, visit https://docs.github.com/en/authentication and follow the instructions for creating a "classic" personal access token.
 
 Note that when you run IGA as a GitHub Actions workflow, you do not need to create or set a GitHub token because it is obtained automatically by the GitHub Actions workflow.
 
 ### Specifying a GitHub release
 
 A GitHub release can be specified to IGA in one of two mutually-exclusive ways:
  1. The full URL of the web page on GitHub of a tagged release. In this case,
@@ -352,14 +355,16 @@
 
 Running IGA with the option `--save-metadata` will make it create a metadata record, but instead of uploading the record (and any assets) to the InvenioRDM server, IGA will write the result to the given destination. This can be useful not only for debugging but also for creating a starting point for a custom metadata record: first run IGA with `--save-metadata` to save a record to a file, edit the result, then finally run IGA with the `--read-metadata` option to use the modified record to create a release in the InvenioRDM server.
 
 The `--mode` option can be used to change the run mode. Four run modes are available: `quiet`, `normal`, `verbose`, and `debug`. The default mode is `normal`, in which IGA prints a few messages while it's working. The mode `quiet` will make it avoid printing anything unless an error occurs, the mode `verbose` will make it print a detailed trace of what it is doing, and the mode `debug` will make IGA even more verbose. In addition, in `debug` mode, IGA will drop into the `pdb` debugger if it encounters an exception during execution. On Linux and macOS, debug mode also installs a signal handler on signal USR1 that causes IGA to drop into the `pdb` debugger if the signal USR1 is received. (Use `kill -USR1 NNN`, where NNN is the IGA process id.)
 
 By default, informational output is sent to the standard output (normally the terminal console). The option `--log-dest` can be used to send the output to the given destination instead. The value can be `-` (i.e., a dash) to indicate console output, or it can be a file path to send the output to the file. A special exception is that even if a log destination is given, IGA will still print the final record URL to stdout.  This makes it possible to invoke IGA from scripts that capture the record URL while still saving diagnostic output in case debugging is needed.
 
+By default, IGA prints only the record URL when done. The option `--print-doi` will make it also print the DOI of the record. (Note that this only works when publishing records; if options `--draft` or `--community` are used, then there will be no DOI. In those case, only the URL will be printed.)
+
 Reading and writing large files may take a long time; on the other hand, IGA should not wait forever on network operations before reporting an error if a server or network becomes unresponsive. To balance these conflicting needs, IGA automatically scales its network timeout based on file sizes. To override its adaptive algorithm and set an explicit timeout value, use the option `--timeout` with a value in seconds.
 
 If given the `--version` option, this program will print its version and other information, and exit without doing anything else.
 
 Running IGA with the option `--help` will make it print help text and exit without doing anything else.
 
 ### Summary of command-line options
@@ -380,14 +385,15 @@
 | `--invenio-server` _S_ | `-s` _S_ | Send record to InvenioRDM server at address _S_ | Use value in env. var. `INVENIO_SERVER` | | 
 | `--invenio-token` _K_  | `-k` _K_ | Use InvenioRDM access token _K_ | Use value in env. var. `INVENIO_TOKEN` | | 
 | `--list-communities`   | `-L`     | List communities available for use with `--community` | | |
 | `--log-dest` _L_       | `-l` _L_ | Write log output to destination _L_ | Write to terminal | ⚐ |
 | `--mode` _M_           | `-m` _M_ | Run in mode `quiet`, `normal`, `verbose`, or `debug` | `normal` | |
 | `--open`               | `-o`     | Open record's web page in a browser when done | Do nothing when done | |
 | `--parent-record` _N_  | `-p` _N_ | Make this a new version of existing record _N_ | New record is unrelated to other records | ❖ |
+| `--print-doi`          | `-i`     | Print both the DOI & record URL when done | Print only the record URL | |
 | `--read-metadata` _R_  | `-R` _R_ | Read metadata record from file _R_; don\'t build one | Build metadata record | |
 | `--save-metadata` _D_  | `-S` _D_ | Save metadata record to file _D_; don\'t upload it | Upload to InvenioRDM server | |
 | `--timeout` _X_        | `-T` _X_ | Wait on network operations a max of _X_ seconds | Auto-adjusted based on file size | |
 | `--version`            | `-V`     | Print program version info and exit | | |
 
 ⚑ &nbsp; Can repeat the option to specify multiple files.<br>
 ⚐ &nbsp; To write to the console, use the character `-` as the value of _OUT_; otherwise, _OUT_ must be the name of a file where the output should be written.<br>
@@ -410,15 +416,17 @@
 | 7    | an exception or fatal error occurred                     |
 
 
 ## Known issues and limitations
 
 The following are known issues and limitations.
 * As of mid-2023, InvenioRDM requires names of record creators and other contributors to be split into given (first) and family (surname). This is problematic for multiple reasons. The first is that mononyms are common in many countries: a person's name may legitimately be only a single word which is not conceptually a "given" or "family" name.  To compound the difficulty for IGA, names are stored as single fields in GitHub account metadata, so unless a repository has a `codemeta.json` or `CITATION.cff` file (which allow authors more control over how they want their names represented), IGA is forced to try to split the single GitHub name string into two parts. _A foolproof algorithm for doing this does not exist_, so IGA will sometimes get it wrong. (That said, IGA goes to extraordinary lengths to try to do a good job.)
-* Some accounts on GitHub are software automation or "bot" accounts but are not labeled as such. These accounts are generally indistinguishable from human accounts on GitHub. If such an account is the creator of a release in GitHub, and IGA has to use its name-splitting algorithm on the name of the account, it may produce a nonsensical result. For example, it might turn "Travis CI" into an entry with a first name of "Travis" and last name of "CI". 
+* InvenioRDM requires that identities (creators, contributors, etc.) to be labeled as personal or organizational. The nature of identities is usually made clear in `codemeta.json` and `CITATION.cff` files. GitHub also provides a flag that is meant to be used to label organizational accounts, but sometimes people don't set the GitHub account information correctly. Consequently, if IGA has to use GitHub data to get (e.g.) the list of contributors on a project, it may mislabel identities in the InvenioRDM record it produces.
+* Some accounts on GitHub are software automation or "bot" accounts, but are not labeled as such. These accounts are generally indistinguishable from human accounts on GitHub, so if they're not labeled as bot or organizational accounts in GitHub, IGA can't recognize that they're humans. If such an account is the creator of a release in GitHub, and IGA tries to use its name-splitting algorithm on the name of the account, it may produce a nonsensical result. For example, it might turn "Travis CI" into an entry with a first name of "Travis" and last name of "CI".
+* Funder and funding information can only be specified in `codemeta.json` files; neither GitHub nor `CITATION.cff` have provisions to store this kind of metadata. The CodeMeta specification defines two fields for this purpose: `funder` and `funding`. Unfortunately, these map imperfectly to the requirements of InvenioRDM's metadata format. In addition, people don't always follow the CodeMeta guidelines, and sometimes they write funding information as text strings (instead of structured objects), the interpretation of which would require software that can recognize grant and funding agency information from free-text descriptions. This combination of factors means IGA often can't fill in the funding metadata in InvenioRDM records even if there is some funding information in the `codemeta.json` file.
 
 
 ## Getting help
 
 If you find an issue, please submit it in [the GitHub issue tracker](https://github.com/caltechlibrary/iga/issues) for this repository.
```

### Comparing `iga-1.0.3/README.md` & `iga-1.1.0/iga.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,31 @@
+Metadata-Version: 2.1
+Name: iga
+Version: 1.1.0
+Summary: InvenioRDM GitHub Archiver
+Home-page: https://github.com/caltechlibrary/iga
+Author: Michael Hucka
+Author-email: helpdesk@library.caltech.edu
+License: https://github.com/caltechlibrary/iga/blob/main/LICENSE
+Project-URL: Source Code, https://github.com/caltechlibrary/iga
+Project-URL: Bug Tracker, https://github.com/caltechlibrary/iga/issues
+Keywords: Python,applications
+Classifier: Development Status :: 3 - Alpha
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Science/Research
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: Unix
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # IGA<img width="12%" align="right" src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/cloud-upload.png">
 
 IGA is the _InvenioRDM GitHub Archiver_, a standalone program as well as a [GitHub Actions](https://github.com/marketplace/actions/iga) workflow that lets you automatically archive GitHub software releases in an [InvenioRDM](https://inveniosoftware.org/products/rdm/) repository.
 
 [![Latest release](https://img.shields.io/github/v/release/caltechlibrary/iga.svg?style=flat-square&color=b44e88&label=Latest%20release)](https://github.com/caltechlibrary/iga/releases)
 [![License](https://img.shields.io/badge/License-BSD--like-lightgrey.svg?style=flat-square)](https://github.com/caltechlibrary/iga/LICENSE)
 [![Python](https://img.shields.io/badge/Python-3.9+-brightgreen.svg?style=flat-square)](https://www.python.org/downloads/release/python-390/)
@@ -53,20 +77,23 @@
 
 ### IGA as a standalone program
 
 Please choose an approach that suits your situation and preferences.
 
 <details><summary><h4><i>Alternative 1: using <code>pipx</code></i></h4></summary>
 
-[Pipx](https://pypa.github.io/pipx/) lets you install Python programs in a way that isolates Python dependencies, and yet the resulting `iga` command can be run from any shell and directory &ndash; like any normal program on your computer. If you use `pipx` on your system, you can install IGA with the following command:
+[Pipx](https://pypa.github.io/pipx/) lets you install Python programs in a way that isolates Python dependencies from other Python programs on your system, and yet the resulting `iga` command can be run from any shell and directory &ndash; like any normal program on your computer. If you use `pipx` on your system, you can install IGA with the following command:
 ```sh
 pipx install iga
 ```
 
-Pipx can also let you run IGA directly using `pipx run iga`, although in that case, you must always prefix every IGA command with `pipx run`.  Consult the [documentation for `pipx run`](https://github.com/pypa/pipx#walkthrough-running-an-application-in-a-temporary-virtual-environment) for more information.
+After installation, a program named `iga` should end up in a location where other command-line programs are installed on your computer.  Test it by running the following command in a shell:
+```shell
+iga --help
+```
 </details>
 
 <details><summary><h4><i>Alternative 2: using <code>pip</code></i></h4></summary>
 
 IGA is available from the [Python package repository PyPI](https://pypi.org) and can be installed using [`pip`](https://pip.pypa.io/en/stable/installing/):
 ```sh
 python3 -m pip install iga
@@ -74,14 +101,19 @@
 
 As an alternative to getting it from [PyPI](https://pypi.org), you can install `iga` directly from GitHub:
 ```sh
 python3 -m pip install git+https://github.com/caltechlibrary/iga.git
 ```
 
 _If you already installed IGA once before_, and want to update to the latest version, add `--upgrade` to the end of either command line above.
+
+After installation, a program named `iga` should end up in a location where other command-line programs are installed on your computer.  Test it by running the following command in a shell:
+```shell
+iga --help
+```
 </details>
 
 <details><summary><h4><i>Alternative 3: from sources</i></h4></summary>
 
 If  you prefer to install IGA directly from the source code, first obtain a copy by either downloading the source archive from the [IGA releases page on GitHub](https://github.com/caltechlibrary/iga/releases), or by using `git` to clone the repository to a location on your computer. For example,
 ```sh
 git clone https://github.com/caltechlibrary/iga
@@ -90,19 +122,14 @@
 Next, after getting a copy of the files,  run `setup.py` inside the code directory:
 ```sh
 cd iga
 python3 setup.py install
 ```
 </details>
 
-After installation, a program named `iga` should end up in a location where other command-line programs are installed on your computer.  Test it by running the following command in a shell:
-```shell
-iga --help
-```
-
 
 ### IGA as a GitHub Actions workflow
 
 A [GitHub Actions](https://docs.github.com/en/actions) workflow is an automated process that runs on GitHub's servers under control of a file in your repository. Follow these steps to create the IGA workflow file:
 
 1. In the main branch of your GitHub repository, create a `.github/workflows` directory
 2. In the `.github/workflows` directory, create a file named (e.g.) `iga.yml` and copy the [following contents](https://raw.githubusercontent.com/caltechlibrary/iga/main/sample-workflow.yml) into it:
@@ -254,15 +281,15 @@
 
 A personal access token (PAT) for making API calls to the InvenioRDM server must be also supplied when invoking IGA. The preferred method is to set the value of the environment variable `INVENIO_TOKEN`. Alternatively, you can use the option `--invenio-token` to pass the token on the command line, but **you are strongly advised to avoid this practice because it is insecure**.
 
 To obtain a PAT from an InvenioRDM server, first log in to the server, then visit the page at `/account/settings/applications` and use the interface there to create a token. The token will be a long string of alphanumeric characters such as `OH0KYf4PGYQGnCM4b53ejSGicOC4s4YnonRVzGJbWxY`; set the value of the variable `INVENIO_TOKEN` to this string.
 
 ### Providing a GitHub access token
 
-It _may_ be possible to run IGA without providing a GitHub access token. GitHub allows up to 60 API calls per minute when running without credentials, and though IGA makes several API calls to GitHub each time it runs, for some repositories IGA will not hit the limit. However, if you run IGA multiple times in a row or your repository has many contributors, then you may need to supply a GitHub access token. The preferred way of doing that is to set the value of the environment variable `GITHUB_TOKEN`. Alternatively, you can use the option `--github-token` to pass the token on the command line, but **you are strongly advised to avoid this practice because it is insecure**.  To obtain a PAT from GitHub, visit https://docs.github.com/en/authentication and follow the instructions for creating a "classic" personal access token.
+It _may_ be possible to run IGA without providing a GitHub access token. GitHub allows up to 60 API calls per minute when running without credentials, and though IGA makes several API calls to GitHub each time it runs, for some public repositories IGA will not hit the limit. However, if you are archiving a private repository, run IGA multiple times in a row, or the repository has many contributors, then you will need to supply a GitHub access token. The preferred way of doing that is to set the value of the environment variable `GITHUB_TOKEN`. Alternatively, you can use the option `--github-token` to pass the token on the command line, but **you are strongly advised to avoid this practice because it is insecure**.  To obtain a PAT from GitHub, visit https://docs.github.com/en/authentication and follow the instructions for creating a "classic" personal access token.
 
 Note that when you run IGA as a GitHub Actions workflow, you do not need to create or set a GitHub token because it is obtained automatically by the GitHub Actions workflow.
 
 ### Specifying a GitHub release
 
 A GitHub release can be specified to IGA in one of two mutually-exclusive ways:
  1. The full URL of the web page on GitHub of a tagged release. In this case,
@@ -328,14 +355,16 @@
 
 Running IGA with the option `--save-metadata` will make it create a metadata record, but instead of uploading the record (and any assets) to the InvenioRDM server, IGA will write the result to the given destination. This can be useful not only for debugging but also for creating a starting point for a custom metadata record: first run IGA with `--save-metadata` to save a record to a file, edit the result, then finally run IGA with the `--read-metadata` option to use the modified record to create a release in the InvenioRDM server.
 
 The `--mode` option can be used to change the run mode. Four run modes are available: `quiet`, `normal`, `verbose`, and `debug`. The default mode is `normal`, in which IGA prints a few messages while it's working. The mode `quiet` will make it avoid printing anything unless an error occurs, the mode `verbose` will make it print a detailed trace of what it is doing, and the mode `debug` will make IGA even more verbose. In addition, in `debug` mode, IGA will drop into the `pdb` debugger if it encounters an exception during execution. On Linux and macOS, debug mode also installs a signal handler on signal USR1 that causes IGA to drop into the `pdb` debugger if the signal USR1 is received. (Use `kill -USR1 NNN`, where NNN is the IGA process id.)
 
 By default, informational output is sent to the standard output (normally the terminal console). The option `--log-dest` can be used to send the output to the given destination instead. The value can be `-` (i.e., a dash) to indicate console output, or it can be a file path to send the output to the file. A special exception is that even if a log destination is given, IGA will still print the final record URL to stdout.  This makes it possible to invoke IGA from scripts that capture the record URL while still saving diagnostic output in case debugging is needed.
 
+By default, IGA prints only the record URL when done. The option `--print-doi` will make it also print the DOI of the record. (Note that this only works when publishing records; if options `--draft` or `--community` are used, then there will be no DOI. In those case, only the URL will be printed.)
+
 Reading and writing large files may take a long time; on the other hand, IGA should not wait forever on network operations before reporting an error if a server or network becomes unresponsive. To balance these conflicting needs, IGA automatically scales its network timeout based on file sizes. To override its adaptive algorithm and set an explicit timeout value, use the option `--timeout` with a value in seconds.
 
 If given the `--version` option, this program will print its version and other information, and exit without doing anything else.
 
 Running IGA with the option `--help` will make it print help text and exit without doing anything else.
 
 ### Summary of command-line options
@@ -356,14 +385,15 @@
 | `--invenio-server` _S_ | `-s` _S_ | Send record to InvenioRDM server at address _S_ | Use value in env. var. `INVENIO_SERVER` | | 
 | `--invenio-token` _K_  | `-k` _K_ | Use InvenioRDM access token _K_ | Use value in env. var. `INVENIO_TOKEN` | | 
 | `--list-communities`   | `-L`     | List communities available for use with `--community` | | |
 | `--log-dest` _L_       | `-l` _L_ | Write log output to destination _L_ | Write to terminal | ⚐ |
 | `--mode` _M_           | `-m` _M_ | Run in mode `quiet`, `normal`, `verbose`, or `debug` | `normal` | |
 | `--open`               | `-o`     | Open record's web page in a browser when done | Do nothing when done | |
 | `--parent-record` _N_  | `-p` _N_ | Make this a new version of existing record _N_ | New record is unrelated to other records | ❖ |
+| `--print-doi`          | `-i`     | Print both the DOI & record URL when done | Print only the record URL | |
 | `--read-metadata` _R_  | `-R` _R_ | Read metadata record from file _R_; don\'t build one | Build metadata record | |
 | `--save-metadata` _D_  | `-S` _D_ | Save metadata record to file _D_; don\'t upload it | Upload to InvenioRDM server | |
 | `--timeout` _X_        | `-T` _X_ | Wait on network operations a max of _X_ seconds | Auto-adjusted based on file size | |
 | `--version`            | `-V`     | Print program version info and exit | | |
 
 ⚑ &nbsp; Can repeat the option to specify multiple files.<br>
 ⚐ &nbsp; To write to the console, use the character `-` as the value of _OUT_; otherwise, _OUT_ must be the name of a file where the output should be written.<br>
@@ -386,15 +416,17 @@
 | 7    | an exception or fatal error occurred                     |
 
 
 ## Known issues and limitations
 
 The following are known issues and limitations.
 * As of mid-2023, InvenioRDM requires names of record creators and other contributors to be split into given (first) and family (surname). This is problematic for multiple reasons. The first is that mononyms are common in many countries: a person's name may legitimately be only a single word which is not conceptually a "given" or "family" name.  To compound the difficulty for IGA, names are stored as single fields in GitHub account metadata, so unless a repository has a `codemeta.json` or `CITATION.cff` file (which allow authors more control over how they want their names represented), IGA is forced to try to split the single GitHub name string into two parts. _A foolproof algorithm for doing this does not exist_, so IGA will sometimes get it wrong. (That said, IGA goes to extraordinary lengths to try to do a good job.)
-* Some accounts on GitHub are software automation or "bot" accounts but are not labeled as such. These accounts are generally indistinguishable from human accounts on GitHub. If such an account is the creator of a release in GitHub, and IGA has to use its name-splitting algorithm on the name of the account, it may produce a nonsensical result. For example, it might turn "Travis CI" into an entry with a first name of "Travis" and last name of "CI". 
+* InvenioRDM requires that identities (creators, contributors, etc.) to be labeled as personal or organizational. The nature of identities is usually made clear in `codemeta.json` and `CITATION.cff` files. GitHub also provides a flag that is meant to be used to label organizational accounts, but sometimes people don't set the GitHub account information correctly. Consequently, if IGA has to use GitHub data to get (e.g.) the list of contributors on a project, it may mislabel identities in the InvenioRDM record it produces.
+* Some accounts on GitHub are software automation or "bot" accounts, but are not labeled as such. These accounts are generally indistinguishable from human accounts on GitHub, so if they're not labeled as bot or organizational accounts in GitHub, IGA can't recognize that they're humans. If such an account is the creator of a release in GitHub, and IGA tries to use its name-splitting algorithm on the name of the account, it may produce a nonsensical result. For example, it might turn "Travis CI" into an entry with a first name of "Travis" and last name of "CI".
+* Funder and funding information can only be specified in `codemeta.json` files; neither GitHub nor `CITATION.cff` have provisions to store this kind of metadata. The CodeMeta specification defines two fields for this purpose: `funder` and `funding`. Unfortunately, these map imperfectly to the requirements of InvenioRDM's metadata format. In addition, people don't always follow the CodeMeta guidelines, and sometimes they write funding information as text strings (instead of structured objects), the interpretation of which would require software that can recognize grant and funding agency information from free-text descriptions. This combination of factors means IGA often can't fill in the funding metadata in InvenioRDM records even if there is some funding information in the `codemeta.json` file.
 
 
 ## Getting help
 
 If you find an issue, please submit it in [the GitHub issue tracker](https://github.com/caltechlibrary/iga/issues) for this repository.
```

### Comparing `iga-1.0.3/iga/__init__.py` & `iga-1.1.0/iga/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # .............................................................................
 #
 #  ╭────────────────────── Notice ── Notice ── Notice ─────────────────────╮
 #  |    The following values are automatically updated at every release    |
 #  |    by the Makefile. Manual changes to these values will be lost.      |
 #  ╰────────────────────── Notice ── Notice ── Notice ─────────────────────╯
 
-__version__     = '1.0.3'
+__version__     = '1.1.0'
 __description__ = 'InvenioRDM GitHub Archiver'
 __url__         = 'https://github.com/caltechlibrary/iga'
 __author__      = 'Michael Hucka'
 __email__       = 'helpdesk@library.caltech.edu'
 __license__     = 'https://github.com/caltechlibrary/iga/blob/main/LICENSE'
```

### Comparing `iga-1.0.3/iga/__main__.py` & `iga-1.1.0/iga/__main__.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.3/iga/cli.py` & `iga-1.1.0/iga/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -219,15 +219,15 @@
 
 def _print_help_and_exit(ctx):
     '''Print the help text and exit with a success code.'''
     click.echo(ctx.get_help())
     sys.exit(int(ExitCode.success))
 
 
-def _print_text(text, color='turquoise4', end='\n', wrap=True):
+def _print_text(text, color='dark_cyan', end='\n', wrap=True):
     '''Print text to the console.
 
     If quiet mode is in effect or the log destination is not stdout, this does
     not print output to the console.
     '''
     log(text)
     if os.environ.get('IGA_RUN_MODE') == 'quiet':
@@ -300,15 +300,15 @@
     # Detect URLs and convert them into Rich links.
     if contains_url := ('http' in text):
         import re
         if match := re.search(r'(https?://\S+)', text):
             ustart, uend = match.start(), match.end()
             url = text[ustart:uend]
             text = text[:ustart] + '[link=' + url + ']' + url + '[/]' + text[uend:]
-    _print_text(text, 'turquoise4', end=end, wrap=(not contains_url))
+    _print_text(text, 'dark_cyan', end=end, wrap=(not contains_url))
 
 
 def _quiet_or_redirected():
     '''Return true if the run mode is 'quiet' or the log dest is not '-'.'''
     return (os.environ.get('IGA_RUN_MODE') == 'quiet'
             or os.environ.get('IGA_LOG_DEST', '-') not in ['-', None])
 
@@ -396,14 +396,17 @@
 #
 @click.option('--open', '-o', 'open_in_browser', is_flag=True,
               help='Open the finished record in your web browser')
 #
 @click.option('--parent-record', '-p', 'parent_id', metavar='STR',
               help='Make this a new version of an existing record')
 #
+@click.option('--print-doi', '-i', 'print_doi', is_flag=True,
+              help='Print the DOI in addition to the record URL')
+#
 @click.option('--read-metadata', '-R', 'source', metavar='FILE', type=File('r'),
               help='Read metadata record from _FILE_; don\'t build one')
 #
 @click.option('--save-metadata', '-S', 'dest', metavar='FILE', type=File('w', lazy=False),
               help='Save metadata record to _FILE_; don\'t upload it')
 #
 @click.option('--timeout', '-T', metavar='NUM', type=INT, callback=_read_timeout,
@@ -412,30 +415,30 @@
 @click.option('--version', '-V', callback=_print_version_and_exit, is_flag=True,
               help='Print IGA version and exit', expose_value=False, is_eager=True)
 #
 @click.argument('url_or_tag', required=True)
 @click.pass_context
 def cli(ctx, url_or_tag, all_assets=False, community=None, draft=False,
         files_to_upload=None, account=None, repo=None, github_token=None,
-        server=None, invenio_token=None, list_communities=False,
+        print_doi=False, server=None, invenio_token=None, list_communities=False,
         open_in_browser=False, log_dest=None, mode='normal', parent_id=None,
         all_metadata=False, source=None, dest=None, timeout=None,
         help=False, version=False):  # noqa A002
     '''InvenioRDM GitHub Archiver (IGA) command-line interface.
 \r
 IGA creates a metadata record in an InvenioRDM server and attaches a GitHub
 release archive to the record. The GitHub release can be specified using
 _either_ a full release URL, _or_ a combination of GitHub account + repository
 \+ tag. Different command-line options can be used to adjust this behavior.
 \r
 _**Specification of the InvenioRDM server and access token**_
 \r
 The server address must be provided either as the value of the option
 `--invenio-server` or in an environment variable named `INVENIO_SERVER`.
-If the server address does not begin with "https://", IGA will prepended it
+If the server address does not begin with "https://", IGA will prepend it
 automatically.
 \r
 A Personal Access Token (PAT) for making API calls to the InvenioRDM server
 must be also supplied when invoking IGA. The preferred method is to set the
 value of the environment variable `INVENIO_TOKEN`. Alternatively, you can use
 the option `--invenio-token` to pass the token on the command line, but **you
 are strongly advised to avoid this practice because it is insecure**.
@@ -586,18 +589,23 @@
 `--log-dest` can be used to send the output to the given destination
 instead. The value can be "`-`" to indicate console output, or a file path to
 send the output to the file. A special exception is that even if a log
 destination is given, IGA will still print the final record URL to stdout.
 This makes it possible to invoke IGA from scripts that capture the record URL
 while still saving diagnostic output in case debugging is needed. E.g.,
 ```shell
-  record_url=`iga --mode verbose --log-dest iga.out ....`
+  record_url=`iga --log-dest iga.out --mode verbose ....`
 ```
 \r
-Networks latencies are unpredicatable. Reading and writing large files may take
+By default, IGA prints only the record URL when done. The option `--print-doi`
+will make it also print the DOI of the record. (Note that this only works when
+publishing records; if options `--draft` or `--community` are used, then there
+will be no DOI. In those case, only the URL will be printed.)
+\r
+Networks latencies are unpredictable. Reading and writing large files may take
 a long time; on the other hand, IGA should not wait forever before reporting an
 error if a server or network becomes unresponsive. To balance these conflicting
 needs, IGA automatically scales its network timeout based on file sizes. To
 override its adaptive algorithm and set an explicit timeout value, use the
 option `--timeout` with a value in seconds.
 \r
 If given the `--version` option, this program will print its version and other
@@ -704,18 +712,22 @@
             elif community:
                 invenio_community_send(record, community)
                 _inform(f'The record has been submitted to community "{community}"'
                         f' and the draft is available at {record.draft_url}')
             else:
                 invenio_publish(record)
                 _inform(f'The published record is available at {record.record_url}')
+                if print_doi and record.doi:
+                    _inform(f'The DOI of the record is {record.doi}')
 
             if _quiet_or_redirected():
-                # If no other output is printed, we still print the URL.
+                # If no other output is printed, we still print the URL & DOI.
                 click.echo(record.record_url or record.draft_url)
+                if print_doi and record.doi:
+                    click.echo(record.doi)
             if open_in_browser:
                 log(f'opening {record.record_url or record.draft_url}')
                 click.launch(record.record_url or record.draft_url)
     except KeyboardInterrupt:
         log('keyboard interrupt received')
         exit_code = ExitCode.user_interrupt
     except bdb.BdbQuit:
```

### Comparing `iga-1.0.3/iga/data_utils.py` & `iga-1.1.0/iga/data_utils.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.3/iga/doi.py` & `iga-1.1.0/iga/doi.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.3/iga/exceptions.py` & `iga-1.1.0/iga/exceptions.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.3/iga/exit_codes.py` & `iga-1.1.0/iga/exit_codes.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.3/iga/github.py` & `iga-1.1.0/iga/github.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.3/iga/id_utils.py` & `iga-1.1.0/iga/id_utils.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.3/iga/invenio.py` & `iga-1.1.0/iga/invenio.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,15 @@
     data        : dict                  # The complete record returned by RDM.
     draft_url   : str                   # links 'self'
     review_url  : str                   # links 'review'
     publish_url : str                   # links 'publish'
     record_url  : str                   # links 'record_html' URL
     files_url   : str                   # links 'files'
     assets      : list                  # List of file names or URLs
+    doi         : str                   # links 'doi' (for published records)
 
 
 @dataclass
 class InvenioCommunity():
     '''Represents information about an Invenio community in InvenioRDM.'''
     data  : dict                       # The complete record returned by RDM.
     name  : str                        # The slug field value
@@ -179,15 +180,16 @@
 
     record = InvenioRecord(data=result,
                            draft_url=result['links']['self_html'],
                            review_url=result['links']['review'],
                            publish_url=result['links']['publish'],
                            record_url='',
                            files_url=result['links']['files'],
-                           assets=[])
+                           assets=[],
+                           doi='')
     log(f'new record record_html = {record.draft_url}')
     return record
 
 
 def invenio_upload(record, asset, print_status):
     '''Upload a file asset to InvenioRDM and attach it to the record.
 
@@ -270,16 +272,19 @@
         raise InternalError('Unexpected result in community submission step')
 
 
 def invenio_publish(record):
     '''Tell the InvenioRDM server to publish the record.'''
     log('telling the server to publish the record')
     result = _invenio('post', url=record.publish_url, msg='publish record')
-    record.record_url = result.get('links', {}).get('self_html', '')
+    links = result.get('links', {})
+    record.record_url = links.get('self_html', '')
+    record.doi = links.get('doi', '').replace('https://doi.org/', '')
     log(f'successfully published record at {record.record_url}')
+    log(f'DOI of record is {record.doi}')
 
 
 @cache
 def invenio_vocabulary(vocab):
     '''Return a controlled vocabulary from this server.
 
     The value of vocab must be one of "languages", "licenses", or
```

### Comparing `iga-1.0.3/iga/json_utils.py` & `iga-1.1.0/iga/json_utils.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.3/iga/licenses.py` & `iga-1.1.0/iga/licenses.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.3/iga/metadata.py` & `iga-1.1.0/iga/metadata.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.3/iga/name_utils.py` & `iga-1.1.0/iga/name_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,21 +99,21 @@
     In the most general case, it is impossible to reliably determine whether a
     given string of characters represents the name of a person and not, say,
     the name of a company or product. This function makes a best-effort guess
     using heuristics in combination with methods from natural language
     processing (NLP), but it will sometimes make mistakes.
 
     This function is designed with the assumption that its input is already
-    expected to be the name of a person or organization, and it only needs to
-    make the determination of whether it is the name of a person.
+    expected to be a name, and it only needs to make the determination of
+    whether it is the name of a person or not.
     '''
     if not name:
         return False
 
-    # A string like "Joe's Foobar" is not a person name.
+    # A string like "Joe's Foobar" is not a name.
     if any(item in name for item in _NON_PERSON_ELEMENTS):
         log(f'{name} contains non-person elements => not a person')
         return False
 
     # If the input contains a mix of Latin and CJK characters, it's likely to
     # contain both an English and CJK version of the same thing. (E.g.,
     # someone might write their name in Chinese in parentheses after an English
```

### Comparing `iga-1.0.3/iga/orcid.py` & `iga-1.1.0/iga/orcid.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.3/iga/reference.py` & `iga-1.1.0/iga/reference.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.3/iga/ror.py` & `iga-1.1.0/iga/ror.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.3/iga/text_utils.py` & `iga-1.1.0/iga/text_utils.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.3/iga.egg-info/PKG-INFO` & `iga-1.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,7 @@
-Metadata-Version: 2.1
-Name: iga
-Version: 1.0.3
-Summary: InvenioRDM GitHub Archiver
-Home-page: https://github.com/caltechlibrary/iga
-Author: Michael Hucka
-Author-email: helpdesk@library.caltech.edu
-License: https://github.com/caltechlibrary/iga/blob/main/LICENSE
-Project-URL: Source Code, https://github.com/caltechlibrary/iga
-Project-URL: Bug Tracker, https://github.com/caltechlibrary/iga/issues
-Keywords: Python,applications
-Classifier: Development Status :: 3 - Alpha
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Science/Research
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: Unix
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # IGA<img width="12%" align="right" src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/cloud-upload.png">
 
 IGA is the _InvenioRDM GitHub Archiver_, a standalone program as well as a [GitHub Actions](https://github.com/marketplace/actions/iga) workflow that lets you automatically archive GitHub software releases in an [InvenioRDM](https://inveniosoftware.org/products/rdm/) repository.
 
 [![Latest release](https://img.shields.io/github/v/release/caltechlibrary/iga.svg?style=flat-square&color=b44e88&label=Latest%20release)](https://github.com/caltechlibrary/iga/releases)
 [![License](https://img.shields.io/badge/License-BSD--like-lightgrey.svg?style=flat-square)](https://github.com/caltechlibrary/iga/LICENSE)
 [![Python](https://img.shields.io/badge/Python-3.9+-brightgreen.svg?style=flat-square)](https://www.python.org/downloads/release/python-390/)
@@ -77,20 +53,23 @@
 
 ### IGA as a standalone program
 
 Please choose an approach that suits your situation and preferences.
 
 <details><summary><h4><i>Alternative 1: using <code>pipx</code></i></h4></summary>
 
-[Pipx](https://pypa.github.io/pipx/) lets you install Python programs in a way that isolates Python dependencies, and yet the resulting `iga` command can be run from any shell and directory &ndash; like any normal program on your computer. If you use `pipx` on your system, you can install IGA with the following command:
+[Pipx](https://pypa.github.io/pipx/) lets you install Python programs in a way that isolates Python dependencies from other Python programs on your system, and yet the resulting `iga` command can be run from any shell and directory &ndash; like any normal program on your computer. If you use `pipx` on your system, you can install IGA with the following command:
 ```sh
 pipx install iga
 ```
 
-Pipx can also let you run IGA directly using `pipx run iga`, although in that case, you must always prefix every IGA command with `pipx run`.  Consult the [documentation for `pipx run`](https://github.com/pypa/pipx#walkthrough-running-an-application-in-a-temporary-virtual-environment) for more information.
+After installation, a program named `iga` should end up in a location where other command-line programs are installed on your computer.  Test it by running the following command in a shell:
+```shell
+iga --help
+```
 </details>
 
 <details><summary><h4><i>Alternative 2: using <code>pip</code></i></h4></summary>
 
 IGA is available from the [Python package repository PyPI](https://pypi.org) and can be installed using [`pip`](https://pip.pypa.io/en/stable/installing/):
 ```sh
 python3 -m pip install iga
@@ -98,14 +77,19 @@
 
 As an alternative to getting it from [PyPI](https://pypi.org), you can install `iga` directly from GitHub:
 ```sh
 python3 -m pip install git+https://github.com/caltechlibrary/iga.git
 ```
 
 _If you already installed IGA once before_, and want to update to the latest version, add `--upgrade` to the end of either command line above.
+
+After installation, a program named `iga` should end up in a location where other command-line programs are installed on your computer.  Test it by running the following command in a shell:
+```shell
+iga --help
+```
 </details>
 
 <details><summary><h4><i>Alternative 3: from sources</i></h4></summary>
 
 If  you prefer to install IGA directly from the source code, first obtain a copy by either downloading the source archive from the [IGA releases page on GitHub](https://github.com/caltechlibrary/iga/releases), or by using `git` to clone the repository to a location on your computer. For example,
 ```sh
 git clone https://github.com/caltechlibrary/iga
@@ -114,19 +98,14 @@
 Next, after getting a copy of the files,  run `setup.py` inside the code directory:
 ```sh
 cd iga
 python3 setup.py install
 ```
 </details>
 
-After installation, a program named `iga` should end up in a location where other command-line programs are installed on your computer.  Test it by running the following command in a shell:
-```shell
-iga --help
-```
-
 
 ### IGA as a GitHub Actions workflow
 
 A [GitHub Actions](https://docs.github.com/en/actions) workflow is an automated process that runs on GitHub's servers under control of a file in your repository. Follow these steps to create the IGA workflow file:
 
 1. In the main branch of your GitHub repository, create a `.github/workflows` directory
 2. In the `.github/workflows` directory, create a file named (e.g.) `iga.yml` and copy the [following contents](https://raw.githubusercontent.com/caltechlibrary/iga/main/sample-workflow.yml) into it:
@@ -278,15 +257,15 @@
 
 A personal access token (PAT) for making API calls to the InvenioRDM server must be also supplied when invoking IGA. The preferred method is to set the value of the environment variable `INVENIO_TOKEN`. Alternatively, you can use the option `--invenio-token` to pass the token on the command line, but **you are strongly advised to avoid this practice because it is insecure**.
 
 To obtain a PAT from an InvenioRDM server, first log in to the server, then visit the page at `/account/settings/applications` and use the interface there to create a token. The token will be a long string of alphanumeric characters such as `OH0KYf4PGYQGnCM4b53ejSGicOC4s4YnonRVzGJbWxY`; set the value of the variable `INVENIO_TOKEN` to this string.
 
 ### Providing a GitHub access token
 
-It _may_ be possible to run IGA without providing a GitHub access token. GitHub allows up to 60 API calls per minute when running without credentials, and though IGA makes several API calls to GitHub each time it runs, for some repositories IGA will not hit the limit. However, if you run IGA multiple times in a row or your repository has many contributors, then you may need to supply a GitHub access token. The preferred way of doing that is to set the value of the environment variable `GITHUB_TOKEN`. Alternatively, you can use the option `--github-token` to pass the token on the command line, but **you are strongly advised to avoid this practice because it is insecure**.  To obtain a PAT from GitHub, visit https://docs.github.com/en/authentication and follow the instructions for creating a "classic" personal access token.
+It _may_ be possible to run IGA without providing a GitHub access token. GitHub allows up to 60 API calls per minute when running without credentials, and though IGA makes several API calls to GitHub each time it runs, for some public repositories IGA will not hit the limit. However, if you are archiving a private repository, run IGA multiple times in a row, or the repository has many contributors, then you will need to supply a GitHub access token. The preferred way of doing that is to set the value of the environment variable `GITHUB_TOKEN`. Alternatively, you can use the option `--github-token` to pass the token on the command line, but **you are strongly advised to avoid this practice because it is insecure**.  To obtain a PAT from GitHub, visit https://docs.github.com/en/authentication and follow the instructions for creating a "classic" personal access token.
 
 Note that when you run IGA as a GitHub Actions workflow, you do not need to create or set a GitHub token because it is obtained automatically by the GitHub Actions workflow.
 
 ### Specifying a GitHub release
 
 A GitHub release can be specified to IGA in one of two mutually-exclusive ways:
  1. The full URL of the web page on GitHub of a tagged release. In this case,
@@ -352,14 +331,16 @@
 
 Running IGA with the option `--save-metadata` will make it create a metadata record, but instead of uploading the record (and any assets) to the InvenioRDM server, IGA will write the result to the given destination. This can be useful not only for debugging but also for creating a starting point for a custom metadata record: first run IGA with `--save-metadata` to save a record to a file, edit the result, then finally run IGA with the `--read-metadata` option to use the modified record to create a release in the InvenioRDM server.
 
 The `--mode` option can be used to change the run mode. Four run modes are available: `quiet`, `normal`, `verbose`, and `debug`. The default mode is `normal`, in which IGA prints a few messages while it's working. The mode `quiet` will make it avoid printing anything unless an error occurs, the mode `verbose` will make it print a detailed trace of what it is doing, and the mode `debug` will make IGA even more verbose. In addition, in `debug` mode, IGA will drop into the `pdb` debugger if it encounters an exception during execution. On Linux and macOS, debug mode also installs a signal handler on signal USR1 that causes IGA to drop into the `pdb` debugger if the signal USR1 is received. (Use `kill -USR1 NNN`, where NNN is the IGA process id.)
 
 By default, informational output is sent to the standard output (normally the terminal console). The option `--log-dest` can be used to send the output to the given destination instead. The value can be `-` (i.e., a dash) to indicate console output, or it can be a file path to send the output to the file. A special exception is that even if a log destination is given, IGA will still print the final record URL to stdout.  This makes it possible to invoke IGA from scripts that capture the record URL while still saving diagnostic output in case debugging is needed.
 
+By default, IGA prints only the record URL when done. The option `--print-doi` will make it also print the DOI of the record. (Note that this only works when publishing records; if options `--draft` or `--community` are used, then there will be no DOI. In those case, only the URL will be printed.)
+
 Reading and writing large files may take a long time; on the other hand, IGA should not wait forever on network operations before reporting an error if a server or network becomes unresponsive. To balance these conflicting needs, IGA automatically scales its network timeout based on file sizes. To override its adaptive algorithm and set an explicit timeout value, use the option `--timeout` with a value in seconds.
 
 If given the `--version` option, this program will print its version and other information, and exit without doing anything else.
 
 Running IGA with the option `--help` will make it print help text and exit without doing anything else.
 
 ### Summary of command-line options
@@ -380,14 +361,15 @@
 | `--invenio-server` _S_ | `-s` _S_ | Send record to InvenioRDM server at address _S_ | Use value in env. var. `INVENIO_SERVER` | | 
 | `--invenio-token` _K_  | `-k` _K_ | Use InvenioRDM access token _K_ | Use value in env. var. `INVENIO_TOKEN` | | 
 | `--list-communities`   | `-L`     | List communities available for use with `--community` | | |
 | `--log-dest` _L_       | `-l` _L_ | Write log output to destination _L_ | Write to terminal | ⚐ |
 | `--mode` _M_           | `-m` _M_ | Run in mode `quiet`, `normal`, `verbose`, or `debug` | `normal` | |
 | `--open`               | `-o`     | Open record's web page in a browser when done | Do nothing when done | |
 | `--parent-record` _N_  | `-p` _N_ | Make this a new version of existing record _N_ | New record is unrelated to other records | ❖ |
+| `--print-doi`          | `-i`     | Print both the DOI & record URL when done | Print only the record URL | |
 | `--read-metadata` _R_  | `-R` _R_ | Read metadata record from file _R_; don\'t build one | Build metadata record | |
 | `--save-metadata` _D_  | `-S` _D_ | Save metadata record to file _D_; don\'t upload it | Upload to InvenioRDM server | |
 | `--timeout` _X_        | `-T` _X_ | Wait on network operations a max of _X_ seconds | Auto-adjusted based on file size | |
 | `--version`            | `-V`     | Print program version info and exit | | |
 
 ⚑ &nbsp; Can repeat the option to specify multiple files.<br>
 ⚐ &nbsp; To write to the console, use the character `-` as the value of _OUT_; otherwise, _OUT_ must be the name of a file where the output should be written.<br>
@@ -410,15 +392,17 @@
 | 7    | an exception or fatal error occurred                     |
 
 
 ## Known issues and limitations
 
 The following are known issues and limitations.
 * As of mid-2023, InvenioRDM requires names of record creators and other contributors to be split into given (first) and family (surname). This is problematic for multiple reasons. The first is that mononyms are common in many countries: a person's name may legitimately be only a single word which is not conceptually a "given" or "family" name.  To compound the difficulty for IGA, names are stored as single fields in GitHub account metadata, so unless a repository has a `codemeta.json` or `CITATION.cff` file (which allow authors more control over how they want their names represented), IGA is forced to try to split the single GitHub name string into two parts. _A foolproof algorithm for doing this does not exist_, so IGA will sometimes get it wrong. (That said, IGA goes to extraordinary lengths to try to do a good job.)
-* Some accounts on GitHub are software automation or "bot" accounts but are not labeled as such. These accounts are generally indistinguishable from human accounts on GitHub. If such an account is the creator of a release in GitHub, and IGA has to use its name-splitting algorithm on the name of the account, it may produce a nonsensical result. For example, it might turn "Travis CI" into an entry with a first name of "Travis" and last name of "CI". 
+* InvenioRDM requires that identities (creators, contributors, etc.) to be labeled as personal or organizational. The nature of identities is usually made clear in `codemeta.json` and `CITATION.cff` files. GitHub also provides a flag that is meant to be used to label organizational accounts, but sometimes people don't set the GitHub account information correctly. Consequently, if IGA has to use GitHub data to get (e.g.) the list of contributors on a project, it may mislabel identities in the InvenioRDM record it produces.
+* Some accounts on GitHub are software automation or "bot" accounts, but are not labeled as such. These accounts are generally indistinguishable from human accounts on GitHub, so if they're not labeled as bot or organizational accounts in GitHub, IGA can't recognize that they're humans. If such an account is the creator of a release in GitHub, and IGA tries to use its name-splitting algorithm on the name of the account, it may produce a nonsensical result. For example, it might turn "Travis CI" into an entry with a first name of "Travis" and last name of "CI".
+* Funder and funding information can only be specified in `codemeta.json` files; neither GitHub nor `CITATION.cff` have provisions to store this kind of metadata. The CodeMeta specification defines two fields for this purpose: `funder` and `funding`. Unfortunately, these map imperfectly to the requirements of InvenioRDM's metadata format. In addition, people don't always follow the CodeMeta guidelines, and sometimes they write funding information as text strings (instead of structured objects), the interpretation of which would require software that can recognize grant and funding agency information from free-text descriptions. This combination of factors means IGA often can't fill in the funding metadata in InvenioRDM records even if there is some funding information in the `codemeta.json` file.
 
 
 ## Getting help
 
 If you find an issue, please submit it in [the GitHub issue tracker](https://github.com/caltechlibrary/iga/issues) for this repository.
```

### Comparing `iga-1.0.3/iga.egg-info/SOURCES.txt` & `iga-1.1.0/iga.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iga-1.0.3/iga.egg-info/requires.txt` & `iga-1.1.0/iga.egg-info/requires.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-aenum==3.1.11
+aenum==3.1.12
 arrow==1.2.3
 boltons==21.0.0
-caltechdata-api==1.3.0
-commonpy==1.12.4
+caltechdata-api==1.4.0
+commonpy==1.13.0
 demoji==1.1.0
 dirtyjson==1.0.8
 httpx==0.23.1
-humanize==4.4.0
-idutils==1.2.0
+humanize==4.6.0
+idutils==1.2.1
 iptools==0.7.0
-isbnlib==3.10.12
-json5==0.9.10
+isbnlib==3.10.14
+json5==0.9.14
 latexcodec==2.0.1
 lxml==4.9.2
-Markdown==3.4.1
+Markdown==3.4.3
 markdown-checklist==0.4.4
 mdx-breakless-lists==1.0.1
 mdx_linkify==2.1
 nameparser==1.1.2
 probablepeople==0.5.4
 pybtex==0.24.0
 pybtex-apa7-style==0.1.3
-pymdown-extensions==9.10
+pymdown-extensions==10.0.1
 PyYAML==6.0
-rich-click==1.6.0
+rich-click==1.6.1
 sidetrack==2.0.1
 spacy==3.5.1
 spacy-alignments==0.9.0
 spacy-legacy==3.0.12
 spacy-loggers==1.0.4
 spacy-pkuseg==0.0.32
 spacy-transformers==1.2.2
```

### Comparing `iga-1.0.3/setup.cfg` & `iga-1.1.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = iga
-version = 1.0.3
+version = 1.1.0
 description = InvenioRDM GitHub Archiver
 author = Michael Hucka
 author_email = helpdesk@library.caltech.edu
 license = https://github.com/caltechlibrary/iga/blob/main/LICENSE
 license_files = LICENSE
 url = https://github.com/caltechlibrary/iga
 project_urls =
```

### Comparing `iga-1.0.3/setup.py` & `iga-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.3/tests/test_cli.py` & `iga-1.1.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.3/tests/test_data_utils.py` & `iga-1.1.0/tests/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.3/tests/test_doi.py` & `iga-1.1.0/tests/test_doi.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.3/tests/test_exceptions.py` & `iga-1.1.0/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.3/tests/test_github.py` & `iga-1.1.0/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.3/tests/test_github_mocks.py` & `iga-1.1.0/tests/test_github_mocks.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.3/tests/test_id_utils.py` & `iga-1.1.0/tests/test_id_utils.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.3/tests/test_init.py` & `iga-1.1.0/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.3/tests/test_is_person.py` & `iga-1.1.0/tests/test_is_person.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.3/tests/test_licenses.py` & `iga-1.1.0/tests/test_licenses.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.3/tests/test_name_splitting.py` & `iga-1.1.0/tests/test_name_splitting.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.3/tests/test_name_utils.py` & `iga-1.1.0/tests/test_name_utils.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.3/tests/test_orcid.py` & `iga-1.1.0/tests/test_orcid.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.3/tests/test_record_from_codemeta.py` & `iga-1.1.0/tests/test_record_from_codemeta.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.3/tests/test_reference.py` & `iga-1.1.0/tests/test_reference.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.3/tests/test_ror.py` & `iga-1.1.0/tests/test_ror.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.3/tests/test_text_utils.py` & `iga-1.1.0/tests/test_text_utils.py`

 * *Files identical despite different names*

