# Comparing `tmp/sat-utils-1.1.4.tar.gz` & `tmp/sat-utils-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sat-utils-1.1.4.tar", last modified: Tue May  9 13:40:33 2023, max compression
+gzip compressed data, was "sat-utils-1.1.8.tar", last modified: Thu Jun  1 16:38:35 2023, max compression
```

## Comparing `sat-utils-1.1.4.tar` & `sat-utils-1.1.8.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0       36 2023-05-05 19:40:30.015119 sat-utils-1.1.4/.coveragerc
--rw-r--r--   0        0        0      220 2023-05-04 18:57:03.282604 sat-utils-1.1.4/.editorconfig
--rw-r--r--   0        0        0      522 2023-05-05 13:45:33.481647 sat-utils-1.1.4/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      799 2023-05-05 13:45:33.481647 sat-utils-1.1.4/.github/workflows/publish.yml
--rw-r--r--   0        0        0      507 2023-05-05 19:55:26.778801 sat-utils-1.1.4/.github/workflows/unit-test.yml
--rw-r--r--   0        0        0     3127 2023-05-05 13:59:16.248588 sat-utils-1.1.4/.gitignore
--rw-r--r--   0        0        0      875 2023-05-04 18:57:03.282604 sat-utils-1.1.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0      452 2023-05-05 19:21:22.269195 sat-utils-1.1.4/Dockerfile
--rw-r--r--   0        0        0     1101 2023-05-05 13:45:33.481647 sat-utils-1.1.4/LICENSE
--rw-r--r--   0        0        0      562 2023-05-09 13:10:43.655515 sat-utils-1.1.4/Makefile
--rw-r--r--   0        0        0     2102 2023-05-05 18:52:51.002148 sat-utils-1.1.4/README.md
--rw-r--r--   0        0        0       24 2023-05-05 19:53:36.881860 sat-utils-1.1.4/bandit.yml
--rw-r--r--   0        0        0     2317 2023-05-09 13:39:20.757802 sat-utils-1.1.4/pyproject.toml
--rw-r--r--   0        0        0      214 2023-05-05 19:48:39.279311 sat-utils-1.1.4/pytest.ini
--rw-r--r--   0        0        0    20604 2023-05-05 14:13:37.388157 sat-utils-1.1.4/requirements/base/base.txt
--rw-r--r--   0        0        0    63054 2023-05-05 14:13:40.956190 sat-utils-1.1.4/requirements/dev/dev.txt
--rw-r--r--   0        0        0       56 2023-05-05 19:40:01.490874 sat-utils-1.1.4/sat/__init__.py
--rw-r--r--   0        0        0     1328 2023-05-05 19:03:13.131659 sat-utils-1.1.4/sat/logs.py
--rw-r--r--   0        0        0     1171 2023-05-05 18:11:06.915108 sat-utils-1.1.4/sat/slack.py
--rw-r--r--   0        0        0        0 2023-05-05 13:45:33.481647 sat-utils-1.1.4/tests/__init__.py
--rw-r--r--   0        0        0      677 2023-05-05 19:50:19.888173 sat-utils-1.1.4/tests/test_logger.py
--rw-r--r--   0        0        0     3318 1970-01-01 00:00:00.000000 sat-utils-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0       49 2023-05-12 18:56:12.988294 sat-utils-1.1.8/.coveragerc
+-rw-r--r--   0        0        0      220 2023-05-12 18:37:20.645836 sat-utils-1.1.8/.editorconfig
+-rw-r--r--   0        0        0      494 2023-05-12 18:42:42.752790 sat-utils-1.1.8/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      665 2023-05-12 18:42:42.752790 sat-utils-1.1.8/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      507 2023-05-12 18:37:20.645836 sat-utils-1.1.8/.github/workflows/unit-test.yml
+-rw-r--r--   0        0        0     3125 2023-05-12 18:37:20.645836 sat-utils-1.1.8/.gitignore
+-rw-r--r--   0        0        0      875 2023-05-12 18:37:20.645836 sat-utils-1.1.8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      452 2023-05-12 18:37:20.645836 sat-utils-1.1.8/Dockerfile
+-rw-r--r--   0        0        0     1102 2023-05-12 18:42:42.752790 sat-utils-1.1.8/LICENSE
+-rw-r--r--   0        0        0      564 2023-05-18 17:57:31.352342 sat-utils-1.1.8/Makefile
+-rw-r--r--   0        0        0     2102 2023-05-12 18:37:20.645836 sat-utils-1.1.8/README.md
+-rw-r--r--   0        0        0       24 2023-05-12 18:37:20.645836 sat-utils-1.1.8/bandit.yml
+-rw-r--r--   0        0        0     2396 2023-05-23 18:51:45.891253 sat-utils-1.1.8/pyproject.toml
+-rw-r--r--   0        0        0      214 2023-05-12 18:54:22.923262 sat-utils-1.1.8/pytest.ini
+-rw-r--r--   0        0        0     8086 2023-05-12 18:42:42.752790 sat-utils-1.1.8/requirements/base/base.txt
+-rw-r--r--   0        0        0    50725 2023-05-12 18:42:42.756790 sat-utils-1.1.8/requirements/dev/dev.txt
+-rw-r--r--   0        0        0       56 2023-05-12 18:37:20.649836 sat-utils-1.1.8/sat/__init__.py
+-rw-r--r--   0        0        0     3734 2023-05-12 18:56:12.988294 sat-utils-1.1.8/sat/ldap.py
+-rw-r--r--   0        0        0     1435 2023-05-23 18:53:45.376372 sat-utils-1.1.8/sat/logs.py
+-rw-r--r--   0        0        0     1171 2023-05-12 18:37:20.649836 sat-utils-1.1.8/sat/slack.py
+-rw-r--r--   0        0        0        0 2023-05-05 13:45:33.481647 sat-utils-1.1.8/tests/__init__.py
+-rw-r--r--   0        0        0     1025 2023-05-23 18:59:47.971772 sat-utils-1.1.8/tests/test_logger.py
+-rw-r--r--   0        0        0     3388 1970-01-01 00:00:00.000000 sat-utils-1.1.8/PKG-INFO
```

### Comparing `sat-utils-1.1.4/.github/workflows/publish.yml` & `sat-utils-1.1.8/.github/workflows/publish.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 name: Publish to PyPI
 
 on:
-    push:
-        branches:
-            - main
+  push:
+    branches:
+      - main
 
 jobs:
-    publish:
-        runs-on: sat-hosted
+  publish:
+    runs-on: sat-hosted
 
-        steps:
-            - uses: actions/checkout@v3
+    steps:
+      - uses: actions/checkout@v3
 
-            - uses: actions/setup-python@v2
-              with:
-                  python-version: 3.9
-
-            - name: Install dependencies
-              run: |
-                  python -m pip install --upgrade pip
-                  pip install twine build
-
-            - name: Build and publish
-              env:
-                  TWINE_USERNAME: ${{ secrets.PYPI_USERNAME }}
-                  TWINE_PASSWORD: ${{ secrets.PYPI_PASSWORD }}
-                  TWINE_REPOSITORY_URL: https://pypi.ehps.ncsu.edu
-
-              run: |
-                  python -m build .
-                  twine upload --verbose ./dist/*
+      - uses: actions/setup-python@v2
+        with:
+          python-version: 3.9
+
+      - name: Install dependencies
+        run: |
+          python -m pip install --upgrade pip
+          pip install twine build
+
+      - name: Build and publish
+        env:
+          TWINE_USERNAME: ${{ secrets.PYPI_USERNAME }}
+          TWINE_PASSWORD: ${{ secrets.PYPI_PASSWORD }}
+          TWINE_REPOSITORY_URL: https://pypi.ehps.ncsu.edu
+
+        run: |
+          python -m build .
+          twine upload --verbose ./dist/*
```

### Comparing `sat-utils-1.1.4/.gitignore` & `sat-utils-1.1.8/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -123,14 +123,16 @@
 .env
 .venv
 env/
 venv/
 ENV/
 env.bak/
 venv.bak/
+.envrc
+.direnv
 
 # Spyder project settings
 .spyderproject
 .spyproject
 
 # Rope project settings
 .ropeproject
@@ -157,11 +159,9 @@
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
 
 .DS_Store
 
-# Jeremy's stuff
-.envrc
-.direnv
-.idea
+# IDE folders
+.idea
```

### Comparing `sat-utils-1.1.4/.pre-commit-config.yaml` & `sat-utils-1.1.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `sat-utils-1.1.4/LICENSE` & `sat-utils-1.1.8/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `sat-utils-1.1.4/Makefile` & `sat-utils-1.1.8/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -8,9 +8,9 @@
 	export PIP_REQUIRE_VIRTUALENV=true; \
 	pip install -U -q pip-tools
 	@echo 'Installing requirements...'
 	pip-sync requirements/base/base.txt requirements/dev/dev.txt
 
 setup:
 	@echo 'Setting up the environment...'
-	pip config --site set site.extra-index-url https://pypi.ehps.ncsu.edu/
+	pip config --site set global.extra-index-url https://pypi.ehps.ncsu.edu/
 	make install-dev
```

### Comparing `sat-utils-1.1.4/README.md` & `sat-utils-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `sat-utils-1.1.4/pyproject.toml` & `sat-utils-1.1.8/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 [build-system]
 requires = ["flit_core>=3.2"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "sat-utils"
-version = "1.1.4"
+version = "1.1.8"
 authors = [
   { name="Ryan Semmler", email="rsemmle@ncsu.edu" },
+  { name="Shawn Taylor", email="staylor8@ncsu.edu" },
 ]
 description = "Contains a collection of shared utility functions"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.9"
 dependencies = [
   "slack-sdk>=3.21.0, <4.0.0",
   "requests>=2.29.0, <3.0.0",
+  "ldap3>=2.9.1, <3.0.0"
 ]
 
 [project.optional-dependencies]
 dev = [
   "pytest>=6.2.5, <7.0.0",
   "pytest-mock>=3.10.0, <4.0.0",
   "pytest-cov>=4.0.0, <5.0.0",
```

### Comparing `sat-utils-1.1.4/requirements/dev/dev.txt` & `sat-utils-1.1.8/requirements/dev/dev.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
 #    pip-compile --extra=dev --generate-hashes --output-file=requirements/dev/dev.txt pyproject.toml
 #
-anyio==3.6.2 \
-    --hash=sha256:25ea0d673ae30af41a0c442f81cf3b38c7e79fdc7b60335a4c14e05eb0947421 \
-    --hash=sha256:fbbe32bd270d2a2ef3ed1c5d45041250284e31fc0a4df4a5a6071842051a51e3
-    # via starlette
 asttokens==2.2.1 \
     --hash=sha256:4622110b2a6f30b77e1473affaa97e711bc2f07d3f10848420ff1898edbe94f3 \
     --hash=sha256:6b0ac9e93fb0335014d382b8fa9b3afa7df546984258005da0b9e7095b3deb1c
     # via stack-data
 attrs==23.1.0 \
     --hash=sha256:1f28b4522cdc2fb4256ac1a020c78acf9cba2c6b461ccd2c126f3aa8e8335d04 \
     --hash=sha256:6279836d581513a26f1bf235f9acd333bc9115683f14f7e8fae46c98fc50e015
@@ -197,32 +193,14 @@
     --hash=sha256:ef9659d1cda9ce9ac9585c045aaa1e59223b143f2407db0eaee0b61a4f266fb6 \
     --hash=sha256:f6f5cab2d7f0c12f8187a376cc6582c477d2df91d63f75341307fcdcb5d60303 \
     --hash=sha256:f81c9b4bd8aa747d417407a7f6f0b1469a43b36a85748145e144ac4e8d303cb5 \
     --hash=sha256:f99ef080288f09ffc687423b8d60978cf3a465d3f404a18d1a05474bd8575a47
     # via
     #   pytest-cov
     #   sat-utils (pyproject.toml)
-cx-oracle==8.3.0 \
-    --hash=sha256:076ffb71279d6b2dcbf7df028f62a01e18ce5bb73d8b01eab582bf14a62f4a61 \
-    --hash=sha256:07f01608dfb6603a8f2a868fc7c7bdc951480f187df8dbc50f4d48c884874e6a \
-    --hash=sha256:3b2d215af4441463c97ea469b9cc307460739f89fdfa8ea222ea3518f1a424d9 \
-    --hash=sha256:3baa878597c5fadb2c72f359f548431c7be001e722ce4a4ebdf3d2293a1bb70b \
-    --hash=sha256:410747d542e5f94727f5f0e42e9706c772cf9094fb348ce965ab88b3a9e4d2d8 \
-    --hash=sha256:4b3afe7a911cebaceda908228d36839f6441cbd38e5df491ec25960562bb01a0 \
-    --hash=sha256:4c82ca74442c298ceec56d207450c192e06ecf8ad52eb4aaad0812e147ceabf7 \
-    --hash=sha256:54164974d526b76fdefb0b66a42b68e1fca5df78713d0eeb8c1d0047b83f6bcf \
-    --hash=sha256:70d3cf030aefd71f99b45beba77237b2af448adf5e26be0db3d0d3dee6ea4230 \
-    --hash=sha256:715a8bbda5982af484ded14d184304cc552c1096c82471dd2948298470e88a04 \
-    --hash=sha256:b6a23da225f03f50a81980c61dbd6a358c3575f212ca7f4c22bb65a9faf94f7f \
-    --hash=sha256:b82e4b165ffd807a2bd256259a6b81b0a2452883d39f987509e2292d494ea163 \
-    --hash=sha256:b902db61dcdcbbf8dd981f5a46d72fef40c5150c7fc0eb0f0698b462d6eb834e \
-    --hash=sha256:bf01ce87edb4ef663b2e5bd604e1e0154d2cc2f12b60301f788b569d9db8a900 \
-    --hash=sha256:de42bdc882abdc5cea54597da27a05593b44143728e5b629ad5d35decb1a2036 \
-    --hash=sha256:df412238a9948340591beee9ec64fa62a2efacc0d91107034a7023e2991fba97
-    # via sat-utils (pyproject.toml)
 decorator==5.1.1 \
     --hash=sha256:637996211036b6385ef91435e4fae22989472f9d571faba8927ba8253acbc330 \
     --hash=sha256:b8c3f85900b9dc423225913c5aace94729fe1fa9763b38939a95226f02d37186
     # via ipython
 distlib==0.3.6 \
     --hash=sha256:14bad2d9b04d3a36127ac97f30b12a19268f211063d8f8ee4f47108896e11b46 \
     --hash=sha256:f35c4b692542ca110de7ef0bea44d73981caeb34ca0b9b6b2e6d7790dda8f80e
@@ -231,18 +209,14 @@
     --hash=sha256:33995a6753c30b7f577febfc2c50411fec6aac7f7ffeb7c4cfe5991072dcf9e6 \
     --hash=sha256:5e1de4d849fee02c63b040a4a3fd567f4ab104defd8a5511fbbc24a8a017efbc
     # via flit
 executing==1.2.0 \
     --hash=sha256:0314a69e37426e3608aada02473b4161d4caf5a4b244d1d0c48072b8fee7bacc \
     --hash=sha256:19da64c18d2d851112f09c287f8d3dbbdf725ab0e569077efb6cdcbd3497c107
     # via stack-data
-fastapi==0.95.1 \
-    --hash=sha256:9569f0a381f8a457ec479d90fa01005cfddaae07546eb1f3fa035bc4797ae7d5 \
-    --hash=sha256:a870d443e5405982e1667dfe372663abf10754f246866056336d7f01c21dab07
-    # via sat-utils (pyproject.toml)
 filelock==3.12.0 \
     --hash=sha256:ad98852315c2ab702aeb628412cbf7e95b7ce8c3bf9565670b4eaecf1db370a9 \
     --hash=sha256:fc03ae43288c013d2ea83c8597001b1129db351aad9c57fe2409327916b8e718
     # via virtualenv
 flit==3.8.0 \
     --hash=sha256:5ee0f88fd1cfa4160d1a8fa01237e96d06d677ae0403a0bbabbb277cb37c5e9c \
     --hash=sha256:d0f2a8f4bd45dc794befbf5839ecc0fd3830d65a57bd52b5997542fac5d5e937
@@ -266,17 +240,15 @@
 identify==2.5.24 \
     --hash=sha256:0aac67d5b4812498056d28a9a512a483f5085cc28640b02b258a59dac34301d4 \
     --hash=sha256:986dbfb38b1140e763e413e6feb44cd731faf72d1909543178aa79b0e258265d
     # via pre-commit
 idna==3.4 \
     --hash=sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4 \
     --hash=sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2
-    # via
-    #   anyio
-    #   requests
+    # via requests
 iniconfig==2.0.0 \
     --hash=sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3 \
     --hash=sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374
     # via pytest
 ipython==8.13.2 \
     --hash=sha256:7dff3fad32b97f6488e02f87b970f309d082f758d7b7fc252e3b19ee0e432dbb \
     --hash=sha256:ffca270240fbd21b06b2974e14a86494d6d29290184e788275f55e0b55914926
@@ -291,14 +263,18 @@
     # via ipython
 jinja2==3.1.2 \
     --hash=sha256:31351a702a408a9e7595a8fc6150fc3f43bb6bf7e319770cbc0db9df9437e852 \
     --hash=sha256:6088930bfe239f0e6710546ab9c19c9ef35e29792895fed6e6e31a023a182a61
     # via
     #   mkdocs
     #   mkdocs-material
+ldap3==2.9.1 \
+    --hash=sha256:5869596fc4948797020d3f03b7939da938778a0f9e2009f7a072ccf92b8e8d70 \
+    --hash=sha256:f3e7fc4718e3f09dda568b57100095e0ce58633bcabbed8667ce3f8fbaa4229f
+    # via sat-utils (pyproject.toml)
 markdown==3.3.7 \
     --hash=sha256:cbb516f16218e643d8e0a95b309f77eb118cb138d39a4f27851e6a63581db874 \
     --hash=sha256:f5da449a6e1c989a4cea2631aa8ee67caa5a2ef855d551c88f9e309f4634c621
     # via
     #   mkdocs
     #   mkdocs-material
     #   pymdown-extensions
@@ -412,41 +388,14 @@
     # via sat-utils (pyproject.toml)
 mypy-extensions==1.0.0 \
     --hash=sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d \
     --hash=sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782
     # via
     #   black
     #   mypy
-mysql-connector-python==8.0.33 \
-    --hash=sha256:0004426e964856148e1cde31e9b8be63ae3013715b048ff0f2ede69a6ddd36f7 \
-    --hash=sha256:016662c6252f2c5f47805d9168187be1316d0c1d7109f9fe668482c3d6e5711d \
-    --hash=sha256:241483065ad062256985e082e3cbb3e7d1d6d2275cee17c66d22525b09096201 \
-    --hash=sha256:34d5c5f6ec7c1e75bf972def40d097138e097dc694e36dec89a5dd604ef7aada \
-    --hash=sha256:37eace5b7eb676a41ff1edc5cf6ce4ae1c28406d1a6fe84941e6aa396d688195 \
-    --hash=sha256:3bedf8265fb31698e4144ca54e241e3386802c3a437745b1a536a74cbe7e4fb9 \
-    --hash=sha256:41db4452a99ee28494313eab1aa7749475d3e39bed7b24a0868aee45bd0d9c73 \
-    --hash=sha256:46ff8a10c13f39996d60f45c30cf2ea15e883bc71d58259ed2fea0a5a6fb93a3 \
-    --hash=sha256:4c82fb70f44f2469c0879434c1d8ee3162f56a40cc8f5ca1cc4d97f06c84cd43 \
-    --hash=sha256:7266d7b2550f9fe0cdcea1647aa6aade352e14095042b6a3921c9152cf8543e8 \
-    --hash=sha256:7318f416b9defe84b2bd025304bab62b68f8d8fcbe479af5593161eff12ef169 \
-    --hash=sha256:753d07fb39a67f7f35fe6e6a4fac12008287661de59f9d5c0bf4da3359d83eb8 \
-    --hash=sha256:96f7fb0ccfe96e6e478e5f0f034c99bda961b99ffa1c746cee39cfea45b0c04d \
-    --hash=sha256:9775331fa60b5d5a6925781d77eee4384e2b54a12dea694ffdefd1cf1a9c0fdb \
-    --hash=sha256:984f5649e6abee04461d6f52fbc77387d7137b8fd003c54bac66505006f17183 \
-    --hash=sha256:9f5eb33e29742c5f8ef23df2d3f0de0e46f4325e4324016e15aba7f8665a68c0 \
-    --hash=sha256:a632d7b0e569a46e6d44e6cd3f8db747995a787a081870697dbfd3ae18949339 \
-    --hash=sha256:af9feec311d8ea51261e1ef1f959a442708e30f0024d08d0fb537b07a1271634 \
-    --hash=sha256:c20a85a69af41d2d7d5cf52106f0b9473775819d189487c6ff3d3f3946931ca2 \
-    --hash=sha256:d8167868ebad8d78ba69babd028626e96a51365cab76edf735b2559731759b62 \
-    --hash=sha256:db422b19347c5d00e078dd64e281e5b1e5a19a2d972dc2d9733b136d79c34798 \
-    --hash=sha256:e853e12c00e3beabc581f4e039222708ee606fef80a3bac6b1f497ed89a31aea \
-    --hash=sha256:ea05590cb972b114efa027c343b4b7110d8e8450493984ebfb9a651e27674636 \
-    --hash=sha256:f324233af7ec9fcb19c23096af27662459708c0465886cb017d78ff3f5b78b55 \
-    --hash=sha256:f403ff22d3514d08028590fef463d17dc107ac72ea27a49429614949d82fda40
-    # via sat-utils (pyproject.toml)
 nodeenv==1.7.0 \
     --hash=sha256:27083a7b96a25f2f5e1d8cb4b6317ee8aeda3bdd121394e5ac54e498028a042e \
     --hash=sha256:e0e7f7dfb85fc5394c6fe1e8fa98131a2473e04311a45afb6508f7cf1836fa2b
     # via pre-commit
 packaging==23.1 \
     --hash=sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61 \
     --hash=sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f
@@ -488,141 +437,42 @@
     --hash=sha256:31ef31af7e474a8d8995027fefdfcf509b5c913ff31f2015b4ec4beb26a6f658 \
     --hash=sha256:e2f91727039fc39a92f58a588a25b87f936de6567eed4f0e673e0507edc75bad
     # via sat-utils (pyproject.toml)
 prompt-toolkit==3.0.38 \
     --hash=sha256:23ac5d50538a9a38c8bde05fecb47d0b403ecd0662857a86f886f798563d5b9b \
     --hash=sha256:45ea77a2f7c60418850331366c81cf6b5b9cf4c7fd34616f733c5427e6abbb1f
     # via ipython
-protobuf==3.20.3 \
-    --hash=sha256:03038ac1cfbc41aa21f6afcbcd357281d7521b4157926f30ebecc8d4ea59dcb7 \
-    --hash=sha256:28545383d61f55b57cf4df63eebd9827754fd2dc25f80c5253f9184235db242c \
-    --hash=sha256:2e3427429c9cffebf259491be0af70189607f365c2f41c7c3764af6f337105f2 \
-    --hash=sha256:398a9e0c3eaceb34ec1aee71894ca3299605fa8e761544934378bbc6c97de23b \
-    --hash=sha256:44246bab5dd4b7fbd3c0c80b6f16686808fab0e4aca819ade6e8d294a29c7050 \
-    --hash=sha256:447d43819997825d4e71bf5769d869b968ce96848b6479397e29fc24c4a5dfe9 \
-    --hash=sha256:67a3598f0a2dcbc58d02dd1928544e7d88f764b47d4a286202913f0b2801c2e7 \
-    --hash=sha256:74480f79a023f90dc6e18febbf7b8bac7508420f2006fabd512013c0c238f454 \
-    --hash=sha256:819559cafa1a373b7096a482b504ae8a857c89593cf3a25af743ac9ecbd23480 \
-    --hash=sha256:899dc660cd599d7352d6f10d83c95df430a38b410c1b66b407a6b29265d66469 \
-    --hash=sha256:8c0c984a1b8fef4086329ff8dd19ac77576b384079247c770f29cc8ce3afa06c \
-    --hash=sha256:9aae4406ea63d825636cc11ffb34ad3379335803216ee3a856787bcf5ccc751e \
-    --hash=sha256:a7ca6d488aa8ff7f329d4c545b2dbad8ac31464f1d8b1c87ad1346717731e4db \
-    --hash=sha256:b6cc7ba72a8850621bfec987cb72623e703b7fe2b9127a161ce61e61558ad905 \
-    --hash=sha256:bf01b5720be110540be4286e791db73f84a2b721072a3711efff6c324cdf074b \
-    --hash=sha256:c02ce36ec760252242a33967d51c289fd0e1c0e6e5cc9397e2279177716add86 \
-    --hash=sha256:d9e4432ff660d67d775c66ac42a67cf2453c27cb4d738fc22cb53b5d84c135d4 \
-    --hash=sha256:daa564862dd0d39c00f8086f88700fdbe8bc717e993a21e90711acfed02f2402 \
-    --hash=sha256:de78575669dddf6099a8a0f46a27e82a1783c557ccc38ee620ed8cc96d3be7d7 \
-    --hash=sha256:e64857f395505ebf3d2569935506ae0dfc4a15cb80dc25261176c784662cdcc4 \
-    --hash=sha256:f4bd856d702e5b0d96a00ec6b307b0f51c1982c2bf9c0052cf9019e9a544ba99 \
-    --hash=sha256:f4c42102bc82a51108e449cbb32b19b180022941c727bac0cfd50170341f16ee
-    # via mysql-connector-python
 ptyprocess==0.7.0 \
     --hash=sha256:4b41f3967fce3af57cc7e94b888626c18bf37a083e3651ca8feeb66d492fef35 \
     --hash=sha256:5c5d0a3b48ceee0b48485e0c26037c0acd7d29765ca3fbb5cb3831d347423220
     # via pexpect
 pure-eval==0.2.2 \
     --hash=sha256:01eaab343580944bc56080ebe0a674b39ec44a945e6d09ba7db3cb8cec289350 \
     --hash=sha256:2b45320af6dfaa1750f543d714b6d1c520a1688dec6fd24d339063ce0aaa9ac3
     # via stack-data
 py==1.11.0 \
     --hash=sha256:51c75c4126074b472f746a24399ad32f6053d1b34b68d2fa41e558e6f4a98719 \
     --hash=sha256:607c53218732647dff4acdfcd50cb62615cedf612e72d1724fb1a0cc6405b378
     # via pytest
-pydantic==1.10.7 \
-    --hash=sha256:01aea3a42c13f2602b7ecbbea484a98169fb568ebd9e247593ea05f01b884b2e \
-    --hash=sha256:0cd181f1d0b1d00e2b705f1bf1ac7799a2d938cce3376b8007df62b29be3c2c6 \
-    --hash=sha256:10a86d8c8db68086f1e30a530f7d5f83eb0685e632e411dbbcf2d5c0150e8dcd \
-    --hash=sha256:193924c563fae6ddcb71d3f06fa153866423ac1b793a47936656e806b64e24ca \
-    --hash=sha256:464855a7ff7f2cc2cf537ecc421291b9132aa9c79aef44e917ad711b4a93163b \
-    --hash=sha256:516f1ed9bc2406a0467dd777afc636c7091d71f214d5e413d64fef45174cfc7a \
-    --hash=sha256:6434b49c0b03a51021ade5c4daa7d70c98f7a79e95b551201fff682fc1661245 \
-    --hash=sha256:64d34ab766fa056df49013bb6e79921a0265204c071984e75a09cbceacbbdd5d \
-    --hash=sha256:670bb4683ad1e48b0ecb06f0cfe2178dcf74ff27921cdf1606e527d2617a81ee \
-    --hash=sha256:68792151e174a4aa9e9fc1b4e653e65a354a2fa0fed169f7b3d09902ad2cb6f1 \
-    --hash=sha256:701daea9ffe9d26f97b52f1d157e0d4121644f0fcf80b443248434958fd03dc3 \
-    --hash=sha256:7d45fc99d64af9aaf7e308054a0067fdcd87ffe974f2442312372dfa66e1001d \
-    --hash=sha256:80b1fab4deb08a8292d15e43a6edccdffa5377a36a4597bb545b93e79c5ff0a5 \
-    --hash=sha256:82dffb306dd20bd5268fd6379bc4bfe75242a9c2b79fec58e1041fbbdb1f7914 \
-    --hash=sha256:8c7f51861d73e8b9ddcb9916ae7ac39fb52761d9ea0df41128e81e2ba42886cd \
-    --hash=sha256:950ce33857841f9a337ce07ddf46bc84e1c4946d2a3bba18f8280297157a3fd1 \
-    --hash=sha256:976cae77ba6a49d80f461fd8bba183ff7ba79f44aa5cfa82f1346b5626542f8e \
-    --hash=sha256:9f6f0fd68d73257ad6685419478c5aece46432f4bdd8d32c7345f1986496171e \
-    --hash=sha256:a7cd2251439988b413cb0a985c4ed82b6c6aac382dbaff53ae03c4b23a70e80a \
-    --hash=sha256:abfb7d4a7cd5cc4e1d1887c43503a7c5dd608eadf8bc615413fc498d3e4645cd \
-    --hash=sha256:ae150a63564929c675d7f2303008d88426a0add46efd76c3fc797cd71cb1b46f \
-    --hash=sha256:b0f85904f73161817b80781cc150f8b906d521fa11e3cdabae19a581c3606209 \
-    --hash=sha256:b4a849d10f211389502059c33332e91327bc154acc1845f375a99eca3afa802d \
-    --hash=sha256:c15582f9055fbc1bfe50266a19771bbbef33dd28c45e78afbe1996fd70966c2a \
-    --hash=sha256:c230c0d8a322276d6e7b88c3f7ce885f9ed16e0910354510e0bae84d54991143 \
-    --hash=sha256:cc1dde4e50a5fc1336ee0581c1612215bc64ed6d28d2c7c6f25d2fe3e7c3e918 \
-    --hash=sha256:cf135c46099ff3f919d2150a948ce94b9ce545598ef2c6c7bf55dca98a304b52 \
-    --hash=sha256:cfc83c0678b6ba51b0532bea66860617c4cd4251ecf76e9846fa5a9f3454e97e \
-    --hash=sha256:d2a5ebb48958754d386195fe9e9c5106f11275867051bf017a8059410e9abf1f \
-    --hash=sha256:d71e69699498b020ea198468e2480a2f1e7433e32a3a99760058c6520e2bea7e \
-    --hash=sha256:d75ae19d2a3dbb146b6f324031c24f8a3f52ff5d6a9f22f0683694b3afcb16fb \
-    --hash=sha256:dfe2507b8ef209da71b6fb5f4e597b50c5a34b78d7e857c4f8f3115effaef5fe \
-    --hash=sha256:e0cfe895a504c060e5d36b287ee696e2fdad02d89e0d895f83037245218a87fe \
-    --hash=sha256:e79e999e539872e903767c417c897e729e015872040e56b96e67968c3b918b2d \
-    --hash=sha256:ecbbc51391248116c0a055899e6c3e7ffbb11fb5e2a4cd6f2d0b93272118a209 \
-    --hash=sha256:f4a2b50e2b03d5776e7f21af73e2070e1b5c0d0df255a827e7c632962f8315af
-    # via fastapi
+pyasn1==0.5.0 \
+    --hash=sha256:87a2121042a1ac9358cabcaf1d07680ff97ee6404333bacca15f76aa8ad01a57 \
+    --hash=sha256:97b7290ca68e62a832558ec3976f15cbf911bf5d7c7039d8b861c2a0ece69fde
+    # via ldap3
 pygments==2.15.1 \
     --hash=sha256:8ace4d3c1dd481894b2005f560ead0f9f19ee64fe983366be1a21e171d12775c \
     --hash=sha256:db2db3deb4b4179f399a09054b023b6a586b76499d36965813c71aa8ed7b5fd1
     # via
     #   ipython
     #   mkdocs-material
     #   rich
     #   sat-utils (pyproject.toml)
-pyjwt==2.6.0 \
-    --hash=sha256:69285c7e31fc44f68a1feb309e948e0df53259d579295e6cfe2b1792329f05fd \
-    --hash=sha256:d83c3d892a77bbb74d3e1a2cfa90afaadb60945205d1095d9221f04466f64c14
-    # via sat-utils (pyproject.toml)
 pymdown-extensions==9.11 \
     --hash=sha256:a499191d8d869f30339de86fcf072a787e86c42b6f16f280f5c2cf174182b7f3 \
     --hash=sha256:f7e86c1d3981f23d9dc43294488ecb54abadd05b0be4bf8f0e15efc90f7853ff
     # via mkdocs-material
-pyodbc==4.0.39 \
-    --hash=sha256:05a0912e852ebddaffa8f235b0f3974475021dd8eb604eb46ea67af06efe1239 \
-    --hash=sha256:0f5901b57eaef0761f4cf02bca8e7c63f589fd0fd723a79f6ccf1ea1275372e5 \
-    --hash=sha256:1b3467157661615d5c30893efa1069b55c9ffa434097fc3ae3739e740d83d2ec \
-    --hash=sha256:1f7fb65191926308f09ce75ae7ccecf89310232ee50cdea74edf17ee04a9b068 \
-    --hash=sha256:27d1b3c3159673b44c97c878f9d8056901d45f747ce2e0b4d5d99f0fb6949dc7 \
-    --hash=sha256:305c7d6337e2d4c8350677cc641b343fc0197b7b9bc167815c66b64545c67a53 \
-    --hash=sha256:39f6c56022c764309aa7552c0eb2c58fbb5902ab5d2010d42b021c0b205aa609 \
-    --hash=sha256:3d9d70e1635d35ba3aee3df216ec8e35f2824909f43331c0112b17f460a93923 \
-    --hash=sha256:400e911d54980098c6badadecc82385fc0d6a9057db525d63d2652317df43efe \
-    --hash=sha256:42649ed57d09c04aa197bdd4fe0aa9ca319790b7aa86d0b0784cc70e78c426e5 \
-    --hash=sha256:530c1ac37ead782803b44fb1934ba4c68ed4a6969f7475cb8bc04ae1da14486e \
-    --hash=sha256:5ec009180fcd7c8197f45d083e6670623d8dfe198a457ca2a50ebb1bafe4107f \
-    --hash=sha256:62bb6d7d0d25dc75d1445e539f946461c9c5a3643ae14676b240f71794ea004f \
-    --hash=sha256:6353044b99c763aeec7ca1760b4340298504d8ee544fdcab3c380a2abec15b78 \
-    --hash=sha256:64c1de1263281de7b5ce585b0352746ab1a483453017a8589f838a79cbe3d6d9 \
-    --hash=sha256:72d364e52f6ca2417881a23834b3a36733c09e0dcd4760f49a6b864218d98d92 \
-    --hash=sha256:74af348dbaee4885998858daf50c8964e767629ecf6c195868b016367b0bb861 \
-    --hash=sha256:8553eaef9f8ec333bbddff6eadf0d322dda34b37f4bab19f0658eb532037840c \
-    --hash=sha256:8eb5547282dc73a7784ce7b99584f68687dd85543538ca6f70cffaa6310676e7 \
-    --hash=sha256:9253e746c5c94bf61e3e9adb08fb7688d413cb68c06ebb287ec233387534760a \
-    --hash=sha256:a3e133621ac2dad22d0870a8521c7e82d4270e24ce02451d64e7eb6a40ad0941 \
-    --hash=sha256:a591a1cf3c251a9c7c1642cfb3774119bf3512f3be56151247238f8a7b22b336 \
-    --hash=sha256:a6f4067f46aaa78e77e8a15ade81eb21fb344563d245fb2d9a0aaa553c367cbd \
-    --hash=sha256:af027a60e84274ea08fad1c75991d37a5f1f6e8bcd30f6bda20db99f0cdfbc7d \
-    --hash=sha256:b36fe804d367d01ad81077fa524a36e667aabc3945e32564c7ef9595b28edfa9 \
-    --hash=sha256:c1a59096f1784d0cda3d0b8f393849f05515c46a10016edb6da1b1960d039800 \
-    --hash=sha256:c5faf2870e9d434c6a85c6adc1cdff55c0e376273baf480f06d9848025405688 \
-    --hash=sha256:cdf5a27e6587d1762f7f0e35d6f0309f09019bf3e19ca9177a4b765121f3f106 \
-    --hash=sha256:e0db69478d00fcd8d0b9bdde8aca0b0eada341fd6ed8c2da84b594b928c84106 \
-    --hash=sha256:e528bb70dd6d6299ee429868925df0866e3e919c772b9eff79c8e17920d8f116 \
-    --hash=sha256:ea08e9379c08663d7260e2b8a6c451f56d36c17291af735191089f8e29ad9578 \
-    --hash=sha256:ebcb900fcaf19ca2bc38632218c5d48c666fcc19fe38b08cde001917f4581456 \
-    --hash=sha256:efccc11dff6fba684a74ae1030c92ff8b82429d7f00e0a50aa2ac6f56621cd9f \
-    --hash=sha256:f792677b88e1dde12dab46de8647620fc8171742c02780d51744f7b1b2135dbc \
-    --hash=sha256:fe4ee87b88867867f582dd0c1236cd982508db359a6cbb5e91623ceb6c83e60a
-    # via sat-utils (pyproject.toml)
 pytest==6.2.5 \
     --hash=sha256:131b36680866a76e6781d13f101efb86cf674ebb9762eb70d3082b6f29889e89 \
     --hash=sha256:7310f8d27bc79ced999e760ca304d69f6ba6c6649c0b60fb0e04a4a77cacc134
     # via
     #   pytest-cov
     #   pytest-mock
     #   sat-utils (pyproject.toml)
@@ -823,26 +673,18 @@
     --hash=sha256:20829bdc1a423ec93dac903470975ebf3bc76fd3fd91a4dadc0eeffc940ecb0c \
     --hash=sha256:de3c07b92479940b61cd68c566f49fbc9974c8f38f661d26244078f3903bb9cc
     # via sat-utils (pyproject.toml)
 smmap==5.0.0 \
     --hash=sha256:2aba19d6a040e78d8b09de5c57e96207b09ed71d8e55ce0959eeee6c8e190d94 \
     --hash=sha256:c840e62059cd3be204b0c9c9f74be2c09d5648eddd4580d9314c3ecde0b30936
     # via gitdb
-sniffio==1.3.0 \
-    --hash=sha256:e60305c5e5d314f5389259b7f22aaa33d8f7dee49763119234af3755c55b9101 \
-    --hash=sha256:eecefdce1e5bbfb7ad2eeaabf7c1eeb404d7757c379bd1f7e5cce9d8bf425384
-    # via anyio
 stack-data==0.6.2 \
     --hash=sha256:32d2dd0376772d01b6cb9fc996f3c8b57a357089dec328ed4b6553d037eaf815 \
     --hash=sha256:cbb2a53eb64e5785878201a97ed7c7b94883f48b87bfb0bbe8b623c74679e4a8
     # via ipython
-starlette==0.26.1 \
-    --hash=sha256:41da799057ea8620e4667a3e69a5b1923ebd32b1819c8fa75634bbe8d8bea9bd \
-    --hash=sha256:e87fce5d7cbdde34b76f0ac69013fd9d190d581d80681493016666e6f96c6d5e
-    # via fastapi
 stevedore==5.0.0 \
     --hash=sha256:2c428d2338976279e8eb2196f7a94910960d9f7ba2f41f3988511e95ca447021 \
     --hash=sha256:bd5a71ff5e5e5f5ea983880e4a1dd1bb47f8feebbb3d95b592398e2f02194771
     # via bandit
 tokenize-rt==4.2.1 \
     --hash=sha256:08a27fa032a81cf45e8858d0ac706004fcd523e8463415ddf1442be38e204ea8 \
     --hash=sha256:0d4f69026fed520f8a1e0103aa36c406ef4661417f20ca643f913e33531b3b94
@@ -867,17 +709,15 @@
     --hash=sha256:f6cde21a9c68cf756af02035f72d5a723bf607e862e7be33ece505abf4a3bad9
     # via
     #   ipython
     #   matplotlib-inline
 typing-extensions==4.5.0 \
     --hash=sha256:5cb5f4a79139d699607b3ef622a1dedafa84e115ab0024e0d9c044a9479ca7cb \
     --hash=sha256:fb33085c39dd998ac16d1431ebc293a8b3eedd00fd4a32de0ff79002c19511b4
-    # via
-    #   mypy
-    #   pydantic
+    # via mypy
 urllib3==2.0.2 \
     --hash=sha256:61717a1095d7e155cdb737ac7bb2f4324a858a1e2e6466f6d03ff630ca68d3cc \
     --hash=sha256:d055c2f9d38dc53c808f6fdc8eab7360b6fdbbde02340ed25cfbcd817c62469e
     # via requests
 virtualenv==20.23.0 \
     --hash=sha256:6abec7670e5802a528357fdc75b26b9f57d5d92f29c5462ba0fbe45feacc685e \
     --hash=sha256:a85caa554ced0c0afbd0d638e7e2d7b5f92d23478d05d17a76daeac8f279f924
```

### Comparing `sat-utils-1.1.4/sat/logs.py` & `sat-utils-1.1.8/sat/logs.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 import logging
+import os
 
 
 class SATLogger:
     def __init__(self, name: str = __name__, level: int = logging.INFO) -> None:
         self.logger = logging.getLogger(name)
-        self.logger.setLevel(level)
+        if os.getenv("DEBUG"):
+            self.logger.setLevel(logging.DEBUG)
+        else:
+            self.logger.setLevel(level)
         self.formatter = logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s")
         self.handler = logging.StreamHandler()
         self.handler.setFormatter(self.formatter)
         self.logger.addHandler(self.handler)
 
     def add_handlers(self, handlers: list[(logging.Handler, logging.Formatter)]) -> None:
         """
```

### Comparing `sat-utils-1.1.4/sat/slack.py` & `sat-utils-1.1.8/sat/slack.py`

 * *Files identical despite different names*

### Comparing `sat-utils-1.1.4/tests/test_logger.py` & `sat-utils-1.1.8/tests/test_logger.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,36 @@
 import logging
 import os
+from unittest import mock
 
 TMP_FILE = "/tmp/test.log"
 
 
+@mock.patch.dict(os.environ, {"USELESS": "VALUE"}, clear=True)
 def test_default_logger(caplog):
     """Test the default logger"""
     from sat.logs import SATLogger
 
     logger = SATLogger()
     logger.info("Test message")
     assert "Test message" in caplog.text
     logger.debug("DEBUG message")
     assert "DEBUG message" not in caplog.text
 
 
+@mock.patch.dict(os.environ, {"DEBUG": "1"}, clear=True)
+def test_debug_logger(caplog):
+    """Test the debug logger"""
+    from sat.logs import SATLogger
+
+    logger = SATLogger()
+    logger.debug("DEBUG message")
+    assert "DEBUG message" in caplog.text
+
+
 def test_add_handlers(caplog):
     """Test adding handlers to the logger"""
     from sat.logs import SATLogger
 
     logger = SATLogger()
     logger.add_handlers([(logging.FileHandler(TMP_FILE), logging.Formatter("%(message)s"))])
     logger.info("Test message")
```

### Comparing `sat-utils-1.1.4/PKG-INFO` & `sat-utils-1.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: sat-utils
-Version: 1.1.4
+Version: 1.1.8
 Summary: Contains a collection of shared utility functions
-Author-email: Ryan Semmler <rsemmle@ncsu.edu>
+Author-email: Ryan Semmler <rsemmle@ncsu.edu>, Shawn Taylor <staylor8@ncsu.edu>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: slack-sdk>=3.21.0, <4.0.0
 Requires-Dist: requests>=2.29.0, <3.0.0
+Requires-Dist: ldap3>=2.9.1, <3.0.0
 Requires-Dist: pytest>=6.2.5, <7.0.0 ; extra == "dev"
 Requires-Dist: pytest-mock>=3.10.0, <4.0.0 ; extra == "dev"
 Requires-Dist: pytest-cov>=4.0.0, <5.0.0 ; extra == "dev"
 Requires-Dist: coverage[toml]>=6.2 ; extra == "dev"
 Requires-Dist: black>=23.3.0, <24.0.0 ; extra == "dev"
 Requires-Dist: mypy>=1.2.0, <2.0.0 ; extra == "dev"
 Requires-Dist: ruff==0.0.263 ; extra == "dev"
```

