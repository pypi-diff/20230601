# Comparing `tmp/laminci-0.6.5.tar.gz` & `tmp/laminci-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "laminci-0.6.5.tar", last modified: Tue May 30 09:06:27 2023, max compression
+gzip compressed data, was "laminci-0.6.6.tar", last modified: Thu Jun  1 09:34:58 2023, max compression
```

## Comparing `laminci-0.6.5.tar` & `laminci-0.6.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1371 2023-02-23 21:08:15.192204 laminci-0.6.5/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-02-23 20:36:15.651723 laminci-0.6.5/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2023-02-23 20:36:15.652253 laminci-0.6.5/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1194 2023-02-23 20:36:15.627521 laminci-0.6.5/.gitignore
--rw-r--r--   0        0        0     1770 2023-02-23 20:36:15.623232 laminci-0.6.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0       29 2023-02-23 21:02:08.741159 laminci-0.6.5/README.md
--rw-r--r--   0        0        0     3052 2023-05-30 09:01:05.110946 laminci-0.6.5/docs/changelog.md
--rw-r--r--   0        0        0      339 2023-02-23 20:36:15.640096 laminci-0.6.5/docs/guide/index.md
--rw-r--r--   0        0        0     1415 2023-05-26 15:57:31.631988 laminci-0.6.5/docs/guide/quickstart.ipynb
--rw-r--r--   0        0        0        0 2023-02-23 21:02:08.741423 laminci-0.6.5/docs/index.md
--rw-r--r--   0        0        0      805 2023-02-23 20:36:15.648759 laminci-0.6.5/docs/notes/YYYY-MM-DD-my-design-choice.ipynb
--rw-r--r--   0        0        0      223 2023-02-23 20:36:15.647572 laminci-0.6.5/docs/notes/index.md
--rw-r--r--   0        0        0      122 2023-02-23 20:36:15.618482 laminci-0.6.5/lamin-project.yaml
--rw-r--r--   0        0        0      378 2023-05-30 09:06:24.198057 laminci-0.6.5/laminci/__init__.py
--rw-r--r--   0        0        0     2122 2023-05-26 16:17:30.304228 laminci-0.6.5/laminci/_artifacts.py
--rw-r--r--   0        0        0     1358 2023-05-26 16:17:30.304517 laminci-0.6.5/laminci/_db.py
--rw-r--r--   0        0        0      380 2023-02-23 22:56:58.478640 laminci-0.6.5/laminci/_docs.py
--rw-r--r--   0        0        0      737 2023-02-23 22:56:58.478807 laminci-0.6.5/laminci/_env.py
--rw-r--r--   0        0        0     2745 2023-05-30 09:04:40.786977 laminci-0.6.5/laminci/_nox.py
--rw-r--r--   0        0        0      148 2023-05-26 16:33:21.362381 laminci-0.6.5/laminci/db.py
--rw-r--r--   0        0        0      167 2023-02-23 21:55:02.625861 laminci-0.6.5/laminci/nox.py
--rw-r--r--   0        0        0      497 2023-02-23 21:02:08.742361 laminci-0.6.5/noxfile.py
--rw-r--r--   0        0        0      708 2023-05-28 21:50:19.140197 laminci-0.6.5/pyproject.toml
--rw-r--r--   0        0        0      126 2023-05-26 16:17:30.304991 laminci-0.6.5/tests/test_artifacts.py
--rw-r--r--   0        0        0      495 1970-01-01 00:00:00.000000 laminci-0.6.5/PKG-INFO
+-rw-r--r--   0        0        0     1371 2023-02-23 21:08:15.192204 laminci-0.6.6/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-02-23 20:36:15.651723 laminci-0.6.6/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2023-02-23 20:36:15.652253 laminci-0.6.6/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1194 2023-02-23 20:36:15.627521 laminci-0.6.6/.gitignore
+-rw-r--r--   0        0        0     1770 2023-02-23 20:36:15.623232 laminci-0.6.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       29 2023-02-23 21:02:08.741159 laminci-0.6.6/README.md
+-rw-r--r--   0        0        0     3052 2023-05-30 09:01:05.110946 laminci-0.6.6/docs/changelog.md
+-rw-r--r--   0        0        0      339 2023-02-23 20:36:15.640096 laminci-0.6.6/docs/guide/index.md
+-rw-r--r--   0        0        0     1415 2023-05-26 15:57:31.631988 laminci-0.6.6/docs/guide/quickstart.ipynb
+-rw-r--r--   0        0        0        0 2023-02-23 21:02:08.741423 laminci-0.6.6/docs/index.md
+-rw-r--r--   0        0        0      805 2023-02-23 20:36:15.648759 laminci-0.6.6/docs/notes/YYYY-MM-DD-my-design-choice.ipynb
+-rw-r--r--   0        0        0      223 2023-02-23 20:36:15.647572 laminci-0.6.6/docs/notes/index.md
+-rw-r--r--   0        0        0      122 2023-02-23 20:36:15.618482 laminci-0.6.6/lamin-project.yaml
+-rw-r--r--   0        0        0      378 2023-06-01 09:34:38.124922 laminci-0.6.6/laminci/__init__.py
+-rw-r--r--   0        0        0     2122 2023-05-26 16:17:30.304228 laminci-0.6.6/laminci/_artifacts.py
+-rw-r--r--   0        0        0     1358 2023-05-26 16:17:30.304517 laminci-0.6.6/laminci/_db.py
+-rw-r--r--   0        0        0      380 2023-02-23 22:56:58.478640 laminci-0.6.6/laminci/_docs.py
+-rw-r--r--   0        0        0      737 2023-02-23 22:56:58.478807 laminci-0.6.6/laminci/_env.py
+-rw-r--r--   0        0        0     2727 2023-06-01 09:34:04.219058 laminci-0.6.6/laminci/_nox.py
+-rw-r--r--   0        0        0      148 2023-05-26 16:33:21.362381 laminci-0.6.6/laminci/db.py
+-rw-r--r--   0        0        0      167 2023-02-23 21:55:02.625861 laminci-0.6.6/laminci/nox.py
+-rw-r--r--   0        0        0      497 2023-02-23 21:02:08.742361 laminci-0.6.6/noxfile.py
+-rw-r--r--   0        0        0      708 2023-05-28 21:50:19.140197 laminci-0.6.6/pyproject.toml
+-rw-r--r--   0        0        0      126 2023-05-26 16:17:30.304991 laminci-0.6.6/tests/test_artifacts.py
+-rw-r--r--   0        0        0      495 1970-01-01 00:00:00.000000 laminci-0.6.6/PKG-INFO
```

### Comparing `laminci-0.6.5/.github/workflows/build.yml` & `laminci-0.6.6/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `laminci-0.6.5/.github/workflows/latest-changes.yml` & `laminci-0.6.6/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `laminci-0.6.5/.gitignore` & `laminci-0.6.6/.gitignore`

 * *Files identical despite different names*

### Comparing `laminci-0.6.5/.pre-commit-config.yaml` & `laminci-0.6.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `laminci-0.6.5/docs/changelog.md` & `laminci-0.6.6/docs/changelog.md`

 * *Files identical despite different names*

### Comparing `laminci-0.6.5/docs/guide/quickstart.ipynb` & `laminci-0.6.6/docs/guide/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `laminci-0.6.5/docs/notes/YYYY-MM-DD-my-design-choice.ipynb` & `laminci-0.6.6/docs/notes/YYYY-MM-DD-my-design-choice.ipynb`

 * *Files identical despite different names*

### Comparing `laminci-0.6.5/laminci/_artifacts.py` & `laminci-0.6.6/laminci/_artifacts.py`

 * *Files identical despite different names*

### Comparing `laminci-0.6.5/laminci/_db.py` & `laminci-0.6.6/laminci/_db.py`

 * *Files identical despite different names*

### Comparing `laminci-0.6.5/laminci/_env.py` & `laminci-0.6.6/laminci/_env.py`

 * *Files identical despite different names*

### Comparing `laminci-0.6.5/laminci/_nox.py` & `laminci-0.6.6/laminci/_nox.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,11 +63,11 @@
         session.run("coverage", "xml")
 
 
 def build_docs(session: Session):
     prefix = "." if Path("./lndocs").exists() else ".."
     if nox.options.default_venv_backend == "none":
         session.run(*f"pip install {prefix}/lndocs".split())
-        session.run(*"lamin init --storage ./docsbuild".split())
     else:
         session.install(f"{prefix}/lndocs")
+    # do not simply add instance creation here
     session.run("lndocs")
```

### Comparing `laminci-0.6.5/pyproject.toml` & `laminci-0.6.6/pyproject.toml`

 * *Files identical despite different names*

