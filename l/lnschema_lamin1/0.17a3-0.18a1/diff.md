# Comparing `tmp/lnschema_lamin1-0.17a3.tar.gz` & `tmp/lnschema_lamin1-0.18a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lnschema_lamin1-0.17a3.tar", last modified: Sat May 27 05:46:40 2023, max compression
+gzip compressed data, was "lnschema_lamin1-0.18a1.tar", last modified: Thu Jun  1 12:09:46 2023, max compression
```

## Comparing `lnschema_lamin1-0.17a3.tar` & `lnschema_lamin1-0.18a1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     3577 2023-04-22 05:28:10.791442 lnschema_lamin1-0.17a3/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-04-22 03:48:17.570277 lnschema_lamin1-0.17a3/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2023-04-22 03:48:17.570464 lnschema_lamin1-0.17a3/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1416 2023-04-22 03:51:54.773184 lnschema_lamin1-0.17a3/.gitignore
--rw-r--r--   0        0        0     1795 2023-04-24 17:49:33.167540 lnschema_lamin1-0.17a3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      154 2023-05-25 15:48:48.190697 lnschema_lamin1-0.17a3/README.md
--rw-r--r--   0        0        0     1069 2023-05-27 05:11:12.141464 lnschema_lamin1-0.17a3/docs/changelog.md
--rw-r--r--   0        0        0     5015 2023-04-24 17:39:09.187958 lnschema_lamin1-0.17a3/docs/guide/01-get-started.ipynb
--rw-r--r--   0        0        0     2190 2023-04-24 17:39:09.199540 lnschema_lamin1-0.17a3/docs/guide/02-orms.ipynb
--rw-r--r--   0        0        0     5397 2023-04-24 17:39:09.201311 lnschema_lamin1-0.17a3/docs/guide/10-migrate.ipynb
--rw-r--r--   0        0        0       65 2023-04-22 04:06:04.615921 lnschema_lamin1-0.17a3/docs/guide/index.md
--rw-r--r--   0        0        0      122 2023-04-22 03:48:11.331800 lnschema_lamin1-0.17a3/docs/index.md
--rw-r--r--   0        0        0       63 2023-04-22 03:51:55.148920 lnschema_lamin1-0.17a3/docs/reference.md
--rw-r--r--   0        0        0      163 2023-04-22 04:44:31.557229 lnschema_lamin1-0.17a3/lamin-project.yaml
--rw-r--r--   0        0        0      684 2023-05-27 05:46:20.947409 lnschema_lamin1-0.17a3/lnschema_lamin1/__init__.py
--rw-r--r--   0        0        0     4310 2023-05-25 21:05:50.419914 lnschema_lamin1-0.17a3/lnschema_lamin1/_core.py
--rw-r--r--   0        0        0     2902 2023-05-25 21:05:50.420200 lnschema_lamin1-0.17a3/lnschema_lamin1/_link.py
--rw-r--r--   0        0        0      259 2023-05-25 15:48:48.191950 lnschema_lamin1-0.17a3/lnschema_lamin1/dev/__init__.py
--rw-r--r--   0        0        0      119 2023-04-22 03:48:17.441295 lnschema_lamin1-0.17a3/lnschema_lamin1/dev/_id.py
--rw-r--r--   0        0        0      346 2023-05-25 15:48:48.192035 lnschema_lamin1-0.17a3/lnschema_lamin1/dev/_type.py
--rw-r--r--   0        0        0     1145 2023-04-22 03:56:14.122435 lnschema_lamin1-0.17a3/lnschema_lamin1/dev/_versions.py
--rw-r--r--   0        0        0       31 2023-04-22 03:48:17.441214 lnschema_lamin1-0.17a3/lnschema_lamin1/dev/id.py
--rw-r--r--   0        0        0      156 2023-05-25 15:48:48.192133 lnschema_lamin1-0.17a3/lnschema_lamin1/dev/type.py
--rw-r--r--   0        0        0      426 2023-05-25 15:48:48.192250 lnschema_lamin1-0.17a3/lnschema_lamin1/link.py
--rw-r--r--   0        0        0     1063 2023-04-24 17:49:33.169471 lnschema_lamin1-0.17a3/lnschema_lamin1/migrations/versions/2023-04-24-652443621d5a-v0_16_0.py
--rw-r--r--   0        0        0     4097 2023-05-25 15:48:48.192371 lnschema_lamin1-0.17a3/lnschema_lamin1/migrations/versions/2023-05-15-a0867fc8d6e5-v0_16_2.py
--rw-r--r--   0        0        0     2251 2023-05-25 15:48:48.192464 lnschema_lamin1-0.17a3/lnschema_lamin1/migrations/versions/2023-05-23-f9f58cf3ab38-v0_16_3.py
--rw-r--r--   0        0        0     5149 2023-05-27 05:45:54.624807 lnschema_lamin1-0.17a3/lnschema_lamin1/migrations/versions/2023-05-25-c3f38ffe9e05-v0_17_0.py
--rw-r--r--   0        0        0      776 2023-04-24 16:11:06.697345 lnschema_lamin1-0.17a3/noxfile.py
--rw-r--r--   0        0        0      663 2023-05-26 15:20:03.193182 lnschema_lamin1-0.17a3/pyproject.toml
--rw-r--r--   0        0        0      811 2023-04-22 04:38:14.658100 lnschema_lamin1-0.17a3/tests/test_migrations.py
--rw-r--r--   0        0        0      481 2023-04-22 03:48:11.224317 lnschema_lamin1-0.17a3/tests/test_notebooks.py
--rw-r--r--   0        0        0      724 1970-01-01 00:00:00.000000 lnschema_lamin1-0.17a3/PKG-INFO
+-rw-r--r--   0        0        0     3403 2023-05-29 08:07:10.544417 lnschema_lamin1-0.18a1/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-04-22 03:48:17.570277 lnschema_lamin1-0.18a1/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2023-04-22 03:48:17.570464 lnschema_lamin1-0.18a1/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1416 2023-04-22 03:51:54.773184 lnschema_lamin1-0.18a1/.gitignore
+-rw-r--r--   0        0        0     1795 2023-04-24 17:49:33.167540 lnschema_lamin1-0.18a1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      154 2023-05-25 15:48:48.190697 lnschema_lamin1-0.18a1/README.md
+-rw-r--r--   0        0        0     1221 2023-06-01 12:09:29.000748 lnschema_lamin1-0.18a1/docs/changelog.md
+-rw-r--r--   0        0        0     5478 2023-05-29 08:15:51.257095 lnschema_lamin1-0.18a1/docs/guide/01-get-started.ipynb
+-rw-r--r--   0        0        0     2190 2023-04-24 17:39:09.199540 lnschema_lamin1-0.18a1/docs/guide/02-orms.ipynb
+-rw-r--r--   0        0        0     3402 2023-05-27 08:19:25.110706 lnschema_lamin1-0.18a1/docs/guide/10-migrate.ipynb
+-rw-r--r--   0        0        0       65 2023-04-22 04:06:04.615921 lnschema_lamin1-0.18a1/docs/guide/index.md
+-rw-r--r--   0        0        0      122 2023-04-22 03:48:11.331800 lnschema_lamin1-0.18a1/docs/index.md
+-rw-r--r--   0        0        0       63 2023-04-22 03:51:55.148920 lnschema_lamin1-0.18a1/docs/reference.md
+-rw-r--r--   0        0        0      163 2023-04-22 04:44:31.557229 lnschema_lamin1-0.18a1/lamin-project.yaml
+-rw-r--r--   0        0        0      684 2023-06-01 12:09:19.607061 lnschema_lamin1-0.18a1/lnschema_lamin1/__init__.py
+-rw-r--r--   0        0        0     5854 2023-06-01 10:57:40.910668 lnschema_lamin1-0.18a1/lnschema_lamin1/_core.py
+-rw-r--r--   0        0        0     2902 2023-05-25 21:05:50.420200 lnschema_lamin1-0.18a1/lnschema_lamin1/_link.py
+-rw-r--r--   0        0        0      259 2023-05-25 15:48:48.191950 lnschema_lamin1-0.18a1/lnschema_lamin1/dev/__init__.py
+-rw-r--r--   0        0        0      346 2023-05-25 15:48:48.192035 lnschema_lamin1-0.18a1/lnschema_lamin1/dev/_type.py
+-rw-r--r--   0        0        0     1145 2023-04-22 03:56:14.122435 lnschema_lamin1-0.18a1/lnschema_lamin1/dev/_versions.py
+-rw-r--r--   0        0        0     1021 2023-06-01 10:57:40.910866 lnschema_lamin1-0.18a1/lnschema_lamin1/dev/id.py
+-rw-r--r--   0        0        0      156 2023-05-25 15:48:48.192133 lnschema_lamin1-0.18a1/lnschema_lamin1/dev/type.py
+-rw-r--r--   0        0        0      426 2023-05-25 15:48:48.192250 lnschema_lamin1-0.18a1/lnschema_lamin1/link.py
+-rw-r--r--   0        0        0     1063 2023-04-24 17:49:33.169471 lnschema_lamin1-0.18a1/lnschema_lamin1/migrations/versions/2023-04-24-652443621d5a-v0_16_0.py
+-rw-r--r--   0        0        0     4097 2023-05-25 15:48:48.192371 lnschema_lamin1-0.18a1/lnschema_lamin1/migrations/versions/2023-05-15-a0867fc8d6e5-v0_16_2.py
+-rw-r--r--   0        0        0     2251 2023-05-25 15:48:48.192464 lnschema_lamin1-0.18a1/lnschema_lamin1/migrations/versions/2023-05-23-f9f58cf3ab38-v0_16_3.py
+-rw-r--r--   0        0        0     5149 2023-05-30 05:26:00.254109 lnschema_lamin1-0.18a1/lnschema_lamin1/migrations/versions/2023-05-25-c3f38ffe9e05-v0_17a.py
+-rw-r--r--   0        0        0     8494 2023-05-30 05:26:00.253105 lnschema_lamin1-0.18a1/lnschema_lamin1/migrations/versions/2023-05-30-be880ab5ad00-v0_17b.py
+-rw-r--r--   0        0        0      776 2023-04-24 16:11:06.697345 lnschema_lamin1-0.18a1/noxfile.py
+-rw-r--r--   0        0        0      722 2023-06-01 12:04:08.676295 lnschema_lamin1-0.18a1/pyproject.toml
+-rw-r--r--   0        0        0      811 2023-04-22 04:38:14.658100 lnschema_lamin1-0.18a1/tests/test_migrations.py
+-rw-r--r--   0        0        0      481 2023-04-22 03:48:11.224317 lnschema_lamin1-0.18a1/tests/test_notebooks.py
+-rw-r--r--   0        0        0      748 1970-01-01 00:00:00.000000 lnschema_lamin1-0.18a1/PKG-INFO
```

### Comparing `lnschema_lamin1-0.17a3/.github/workflows/build.yml` & `lnschema_lamin1-0.18a1/.github/workflows/build.yml`

 * *Files 9% similar despite different names*

```diff
@@ -56,38 +56,34 @@
         run: docker pull postgres:latest && docker image save postgres:latest --output ~/postgres.tar
       - name: Cache postgres use
         if: steps.cache-postgres.outputs.cache-hit == 'true'
         run: docker image load --input ~/postgres.tar
       - name: Install Python dependencies
         run: |
           python -m pip install -U pip
-          pip install -U laminci
-          pip install -U lamindb
+          pip install lamindb>=0.41a5
       - name: Install apt-get dependencies
         run: |
           sudo apt-get -y install graphviz
           sudo apt-get install sqlite3-tools=3.37.2-2
           sudo apt-get install libpq-dev
       - name: Lint
         run: |
           nox -s lint
-      - name: Configure Google Cloud
-        id: "auth"
-        uses: "google-github-actions/auth@v0"
+      - name: Configure AWS
+        uses: aws-actions/configure-aws-credentials@v1
         with:
-          credentials_json: "${{ secrets.GCP_CREDENTIALS }}"
-      - name: "Set up Cloud SDK"
-        uses: "google-github-actions/setup-gcloud@v0"
+          aws-access-key-id: ${{ secrets.AWS_ACCESS_KEY_ID }}
+          aws-secret-access-key: ${{ secrets.AWS_SECRET_ACCESS_KEY }}
+          aws-region: eu-central-1
       - name: Build
         run: |
           nox -s build --python ${{ matrix.python-version }}
         env:
           GITHUB_EVENT_NAME: ${{ github.event_name }}
-          SUPABASE_STAGING_URL: ${{ secrets.SUPABASE_STAGING_URL }}
-          SUPABASE_STAGING_ANON_KEY: ${{ secrets.SUPABASE_STAGING_ANON_KEY }}
       - name: Codecov
         if: matrix.python-version == '3.9'
         uses: codecov/codecov-action@v2
         with:
           token: ${{ secrets.CODECOV_TOKEN }}
       - name: Read lamin-project.yaml
         if: matrix.python-version == '3.9'
```

### Comparing `lnschema_lamin1-0.17a3/.github/workflows/latest-changes.yml` & `lnschema_lamin1-0.18a1/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.17a3/.gitignore` & `lnschema_lamin1-0.18a1/.gitignore`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.17a3/.pre-commit-config.yaml` & `lnschema_lamin1-0.18a1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.17a3/docs/changelog.md` & `lnschema_lamin1-0.18a1/docs/changelog.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
-🏗️ Remove SQL-level schema modules | [9](https://github.com/laminlabs/lnschema-lamin1/pull/9) | [falexwolf](https://github.com/falexwolf) | 2023-05-25 | 0.17a2
+➖ Remove lnbase-biolab | [10](https://github.com/laminlabs/lnschema-lamin1/pull/10) | [falexwolf](https://github.com/falexwolf) | 2023-06-01 | 0.18a1
+🏗️ Remove SQL-level schema modules | [9](https://github.com/laminlabs/lnschema-lamin1/pull/9) | [falexwolf](https://github.com/falexwolf) | 2023-05-25 | 0.17.0
 🎨 Add `Well` table, File.cell_lines | [8](https://github.com/laminlabs/lnschema-lamin1/pull/8) | [sunnyosun](https://github.com/sunnyosun) | 2023-05-23 | 0.16.3
 💚 Removed treatment relationships | [4](https://github.com/laminlabs/lnschema-lamin1/pull/4) | [sunnyosun](https://github.com/sunnyosun) | 2023-05-15 | 0.16.2
 ✨ Added `Treatment` table | [3](https://github.com/laminlabs/lnschema-lamin1/pull/3) | [sunnyosun](https://github.com/sunnyosun) | 2023-05-15 |
 🚚 Link `CellType` to `File` | [2](https://github.com/laminlabs/lnschema-lamin1/pull/2) | [falexwolf](https://github.com/falexwolf) | 2023-04-24 | 0.16.1
 🎉 Move content from `lnschema-wetlab` here | [1](https://github.com/laminlabs/lnschema-lamin1/pull/1) | [falexwolf](https://github.com/falexwolf) | 2023-04-22 | 0.15.1
```

### Comparing `lnschema_lamin1-0.17a3/docs/guide/01-get-started.ipynb` & `lnschema_lamin1-0.18a1/docs/guide/01-get-started.ipynb`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9797619047619048%*

 * *Differences: {"'cells'": "{0: {'attachments': OrderedDict()}, 1: {'attachments': OrderedDict()}, 2: "*

 * *            "{'attachments': OrderedDict()}, 4: {'attachments': OrderedDict()}, 5: {'attachments': "*

 * *            "OrderedDict()}, 8: {'attachments': OrderedDict()}, 9: {'attachments': OrderedDict()}, "*

 * *            "12: {'attachments': OrderedDict()}, 13: {'attachments': OrderedDict()}, 14: "*

 * *            "{'attachments': OrderedDict()}, 15: {'attachments': OrderedDict()}, 18: "*

 * *            "{'attachments': OrderedDict()} […]*

```diff
@@ -1,30 +1,33 @@
 {
     "cells": [
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "7f26a335-cf1c-4e69-be3b-0c26b154606a",
             "metadata": {},
             "source": [
                 "# Get started"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "a51faaf3-ee27-43c6-b48d-13be1adb5c46",
             "metadata": {},
             "source": [
                 "Install all required dependencies:\n",
                 "\n",
                 "```\n",
                 "pip install git+https://github.com/laminlabs/lnschema-lamin1\n",
                 "```"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "01f45721",
             "metadata": {},
             "source": [
                 "We use a test account for CI:"
             ]
         },
@@ -35,48 +38,66 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "!lamin login testuser1@lamin.ai --password=\"cEvcwMJFX4OwbsYVaMt2Os6GxxGgDUlBGILs2RyS\""
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "234947fa",
             "metadata": {},
             "source": [
                 "After the first log in on your environment, you can log in just with your user handle: `lamin testuser1`"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "47e8839b-8acf-46f1-b071-6b91139aca9e",
             "metadata": {},
             "source": [
                 "## Choose your instance"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "aae9ea65",
+            "metadata": {
+                "tags": [
+                    "hide-cell"
+                ]
+            },
+            "outputs": [],
+            "source": [
+                "!lamin close"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
             "id": "051e43fa",
             "metadata": {},
             "outputs": [],
             "source": [
                 "import lamindb as ln"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "43b3d4dd-051c-4982-929f-445c6cec2d3e",
             "metadata": {},
             "source": [
                 "### Company-wide production instance: Postgres + GCP bucket"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "a45f84b1",
             "metadata": {},
             "source": [
                 "```{note}\n",
                 "\n",
                 "All of the following calls can also be done using the CLI, e.g., `lamin init --storage ...`\n",
@@ -109,46 +130,50 @@
                 "```{code}\n",
                 "\n",
                 "ln.setup.load(\"testuser1/lamin1\")\n",
                 "```"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "4a4c43b1-55d8-465c-9eaa-4aeed603d265",
             "metadata": {},
             "source": [
                 "For pointing your existing instance to cold storage use (assuming `ln-lamin1-pg-cold` is your bucket name):\n",
                 "\n",
                 "```{code}\n",
                 "\n",
                 "ln.setup.set.storage(\"gs://ln-lamin1-pg-cold\")\n",
                 "```"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "5b22cceb-0456-4f68-bd47-1fa909b1f2f2",
             "metadata": {},
             "source": [
                 "### Mini-instance: SQLite + GCP bucket"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "49d4a2e1-7ee2-48ce-b4ac-6855920bb19b",
             "metadata": {},
             "source": [
                 "```{code}\n",
                 "\n",
                 "ln.setup.init(storage=\"gs://ln-lamin1-sqlite\", schema=\"lamin1,bionty\")\n",
                 "```"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "501b7e65",
             "metadata": {},
             "source": [
                 "### Fast CI runs: SQlite + local storage"
             ]
         },
@@ -168,14 +193,15 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "ln.setup.init(storage=\"./lamin1db\", schema=\"lamin1,bionty\")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "31926241",
             "metadata": {},
             "source": [
                 "## View the schema"
             ]
         },
```

### Comparing `lnschema_lamin1-0.17a3/docs/guide/02-orms.ipynb` & `lnschema_lamin1-0.18a1/docs/guide/02-orms.ipynb`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.17a3/lnschema_lamin1/__init__.py` & `lnschema_lamin1-0.18a1/lnschema_lamin1/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,16 +24,16 @@
    dev
    link
 
 """
 
 _schema_id = "tvhn"
 _name = "lamin1"
-_migration = "c3f38ffe9e05"
-__version__ = "0.17a3"
+_migration = "be880ab5ad00"
+__version__ = "0.18a1"
 
 # prints warning of python versions
 from lamin_logger import py_version_warning
 
 py_version_warning("3.8", "3.10")
```

### Comparing `lnschema_lamin1-0.17a3/lnschema_lamin1/_link.py` & `lnschema_lamin1-0.18a1/lnschema_lamin1/_link.py`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.17a3/lnschema_lamin1/dev/_versions.py` & `lnschema_lamin1-0.18a1/lnschema_lamin1/dev/_versions.py`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.17a3/lnschema_lamin1/migrations/versions/2023-04-24-652443621d5a-v0_16_0.py` & `lnschema_lamin1-0.18a1/lnschema_lamin1/migrations/versions/2023-04-24-652443621d5a-v0_16_0.py`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.17a3/lnschema_lamin1/migrations/versions/2023-05-15-a0867fc8d6e5-v0_16_2.py` & `lnschema_lamin1-0.18a1/lnschema_lamin1/migrations/versions/2023-05-15-a0867fc8d6e5-v0_16_2.py`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.17a3/lnschema_lamin1/migrations/versions/2023-05-23-f9f58cf3ab38-v0_16_3.py` & `lnschema_lamin1-0.18a1/lnschema_lamin1/migrations/versions/2023-05-23-f9f58cf3ab38-v0_16_3.py`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.17a3/lnschema_lamin1/migrations/versions/2023-05-25-c3f38ffe9e05-v0_17_0.py` & `lnschema_lamin1-0.18a1/lnschema_lamin1/migrations/versions/2023-05-25-c3f38ffe9e05-v0_17a.py`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.17a3/noxfile.py` & `lnschema_lamin1-0.18a1/noxfile.py`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.17a3/pyproject.toml` & `lnschema_lamin1-0.18a1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -4,26 +4,25 @@
 
 [project]
 name = "lnschema_lamin1"
 authors = [{name = "Lamin Labs", email = "laminlabs@gmail.com"}]
 readme = "README.md"
 dynamic = ["version", "description"]
 dependencies = [
-    "lamindb[bionty,biolab]>=0.41a2",
+    "lnschema_bionty",  # do not pin lamindb, lamindb pins lnschema_lamin1!
 ]
 
 [project.urls]
 Home = "https://github.com/laminlabs/lnschema-lamin1"
 
 [project.optional-dependencies]
-dev = [
+test = [
+    "lamindb[bionty]==0.41.2",
     "pre-commit",
     "nox",
-]
-test = [
     "pytest>=6.0",
     "pytest-cov",
     "nbproject_test>=0.4.1",
 ]
 
 [tool.black]
 preview = true
```

### Comparing `lnschema_lamin1-0.17a3/tests/test_migrations.py` & `lnschema_lamin1-0.18a1/tests/test_migrations.py`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.17a3/PKG-INFO` & `lnschema_lamin1-0.18a1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: lnschema_lamin1
-Version: 0.17a3
+Version: 0.18a1
 Summary: Lamin's `lamin1` lab schema (`tvhn`).
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
-Requires-Dist: lamindb[bionty,biolab]>=0.41a2
-Requires-Dist: pre-commit ; extra == "dev"
-Requires-Dist: nox ; extra == "dev"
+Requires-Dist: lnschema_bionty
+Requires-Dist: lamindb[bionty]==0.41.2 ; extra == "test"
+Requires-Dist: pre-commit ; extra == "test"
+Requires-Dist: nox ; extra == "test"
 Requires-Dist: pytest>=6.0 ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Requires-Dist: nbproject_test>=0.4.1 ; extra == "test"
 Project-URL: Home, https://github.com/laminlabs/lnschema-lamin1
-Provides-Extra: dev
 Provides-Extra: test
 
 # lnschema-lamin1: Customized schema of Lamin (`tvhn`)
 
 Latest developer docs: [netlify](https://lnschema-lamin1-tvhn.netlify.app/docs/lnschema-lamin1/).
```

