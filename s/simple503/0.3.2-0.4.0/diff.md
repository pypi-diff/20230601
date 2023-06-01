# Comparing `tmp/simple503-0.3.2.tar.gz` & `tmp/simple503-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple503-0.3.2.tar", last modified: Tue May 17 09:10:25 2022, max compression
+gzip compressed data, was "simple503-0.4.0.tar", last modified: Thu Jun  1 13:36:36 2023, max compression
```

## Comparing `simple503-0.3.2.tar` & `simple503-0.4.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0 runner    (1001) docker     (121)     4913 2022-05-17 09:10:25.938560 simple503-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     4870 2022-05-17 09:10:25.938560 simple503-0.3.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6809 2022-05-17 09:10:25.942560 simple503-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      223 2022-05-17 09:10:25.938560 simple503-0.3.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-05-17 09:10:25.930560 simple503-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-17 09:09:46.198874 simple503-0.3.2/simple503/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     4160 2022-05-17 09:09:46.198874 simple503-0.3.2/simple503/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     3282 2022-05-17 09:09:46.198874 simple503-0.3.2/simple503/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11148 2022-05-17 09:09:46.198874 simple503-0.3.2/simple503/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4967 2023-06-01 13:36:36.599259 simple503-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      223 2023-06-01 13:36:36.599259 simple503-0.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     4872 2023-06-01 13:36:36.599259 simple503-0.4.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1064 2023-06-01 13:36:36.591259 simple503-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     6862 2023-06-01 13:36:36.599259 simple503-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3608 2023-06-01 13:36:05.145726 simple503-0.4.0/simple503/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4686 2023-06-01 13:36:05.145726 simple503-0.4.0/simple503/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-01 13:36:05.145726 simple503-0.4.0/simple503/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)    11431 2023-06-01 13:36:05.145726 simple503-0.4.0/simple503/__init__.py
```

### Comparing `simple503-0.3.2/pyproject.toml` & `simple503-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "whey",]
 build-backend = "whey"
 
 [project]
 name = "simple503"
-version = "0.3.2"
+version = "0.4.0"
 description = "PEP 503 Python package repository generator."
 readme = "README.rst"
 keywords = [ "pep503", "pep658", "pip", "pypi",]
 dynamic = []
 dependencies = [
     "airium>=0.2.2",
     "apeye>=1.0.1",
@@ -27,14 +27,15 @@
     "Environment :: Console",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Topic :: System :: Archiving :: Packaging",
@@ -150,15 +151,15 @@
 base-classifiers = [
     "Development Status :: 3 - Alpha",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Topic :: System :: Archiving :: Packaging",
     "Typing :: Typed",
 ]
-python-versions = [ "3.6", "3.7", "3.8", "3.9", "3.10",]
+python-versions = [ "3.6", "3.7", "3.8", "3.9", "3.10", "3.11",]
 python-implementations = [ "CPython", "PyPy",]
 platforms = [ "Windows", "macOS", "Linux",]
 license-key = "MIT"
 
 [tool.dep_checker]
 allowed_unused = [ "dataclasses",]
```

### Comparing `simple503-0.3.2/README.rst` & `simple503-0.4.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -61,16 +61,16 @@
 	:target: https://github.com/repo-helper/simple503/actions?query=workflow%3A%22Flake8%22
 	:alt: Flake8 Status
 
 .. |actions_mypy| image:: https://github.com/repo-helper/simple503/workflows/mypy/badge.svg
 	:target: https://github.com/repo-helper/simple503/actions?query=workflow%3A%22mypy%22
 	:alt: mypy status
 
-.. |requires| image:: https://dependency-dash.herokuapp.com/github/repo-helper/simple503/badge.svg
-	:target: https://dependency-dash.herokuapp.com/github/repo-helper/simple503/
+.. |requires| image:: https://dependency-dash.repo-helper.uk/github/repo-helper/simple503/badge.svg
+	:target: https://dependency-dash.repo-helper.uk/github/repo-helper/simple503/
 	:alt: Requirements Status
 
 .. |coveralls| image:: https://img.shields.io/coveralls/github/repo-helper/simple503/master?logo=coveralls
 	:target: https://coveralls.io/github/repo-helper/simple503?branch=master
 	:alt: Coverage
 
 .. |codefactor| image:: https://img.shields.io/codefactor/grade/github/repo-helper/simple503?logo=codefactor
@@ -96,23 +96,23 @@
 .. |license| image:: https://img.shields.io/github/license/repo-helper/simple503
 	:target: https://github.com/repo-helper/simple503/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/repo-helper/simple503
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/simple503/v0.3.2
+.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/simple503/v0.4.0
 	:target: https://github.com/repo-helper/simple503/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/repo-helper/simple503
 	:target: https://github.com/repo-helper/simple503/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2022
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/simple503
 	:target: https://pypi.org/project/simple503/
 	:alt: PyPI - Downloads
 
 .. end shields
```

### Comparing `simple503-0.3.2/PKG-INFO` & `simple503-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple503
-Version: 0.3.2
+Version: 0.4.0
 Summary: PEP 503 Python package repository generator.
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 License: MIT
 Keywords: pep503,pep658,pip,pypi
 Home-page: https://github.com/repo-helper/simple503
 Project-URL: Issue Tracker, https://github.com/repo-helper/simple503/issues
 Project-URL: Source Code, https://github.com/repo-helper/simple503
@@ -20,14 +20,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: System :: Archiving :: Packaging
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Requires-Dist: airium>=0.2.2
 Requires-Dist: apeye>=1.0.1
@@ -110,16 +111,16 @@
 	:target: https://github.com/repo-helper/simple503/actions?query=workflow%3A%22Flake8%22
 	:alt: Flake8 Status
 
 .. |actions_mypy| image:: https://github.com/repo-helper/simple503/workflows/mypy/badge.svg
 	:target: https://github.com/repo-helper/simple503/actions?query=workflow%3A%22mypy%22
 	:alt: mypy status
 
-.. |requires| image:: https://dependency-dash.herokuapp.com/github/repo-helper/simple503/badge.svg
-	:target: https://dependency-dash.herokuapp.com/github/repo-helper/simple503/
+.. |requires| image:: https://dependency-dash.repo-helper.uk/github/repo-helper/simple503/badge.svg
+	:target: https://dependency-dash.repo-helper.uk/github/repo-helper/simple503/
 	:alt: Requirements Status
 
 .. |coveralls| image:: https://img.shields.io/coveralls/github/repo-helper/simple503/master?logo=coveralls
 	:target: https://coveralls.io/github/repo-helper/simple503?branch=master
 	:alt: Coverage
 
 .. |codefactor| image:: https://img.shields.io/codefactor/grade/github/repo-helper/simple503?logo=codefactor
@@ -145,23 +146,23 @@
 .. |license| image:: https://img.shields.io/github/license/repo-helper/simple503
 	:target: https://github.com/repo-helper/simple503/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/repo-helper/simple503
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/simple503/v0.3.2
+.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/simple503/v0.4.0
 	:target: https://github.com/repo-helper/simple503/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/repo-helper/simple503
 	:target: https://github.com/repo-helper/simple503/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2022
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/simple503
 	:target: https://pypi.org/project/simple503/
 	:alt: PyPI - Downloads
 
 .. end shields
```

### Comparing `simple503-0.3.2/LICENSE` & `simple503-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `simple503-0.3.2/simple503/config.py` & `simple503-0.4.0/simple503/config.py`

 * *Files 13% similar despite different names*

```diff
@@ -58,21 +58,23 @@
 
 	#: The list of keys parsed from ``pyproject.toml``
 	keys: List[str] = [
 			"base-url",
 			"sort",
 			"copy",
 			"target",
+			"extract_metadata",
 			]
 
 	defaults: ClassVar[Dict[str, Any]] = {
 			"sort": False,
 			"copy": False,
 			"base-url": '/',
 			"target": None,
+			"extract_metadata": True,
 			}
 
 	def parse_base_url(self, config: Dict[str, TOML_TYPES]) -> str:
 		"""
 		Parse the ``base-url`` key.
 
 		**Format**: :toml:`String`
@@ -127,14 +129,34 @@
 		:param config: The unparsed TOML config for the ``simple503`` table.
 		"""
 
 		sort = config["sort"]
 		self.assert_type(sort, bool, ["simple503", "sort"])
 		return sort
 
+	def parse_extract_metadata(self, config: Dict[str, TOML_TYPES]) -> str:
+		"""
+		Parse the ``extract_metadata`` key.
+
+		**Format**: :toml:`Boolean`
+
+		:bold-title:`Example:`
+
+		.. code-block:: TOML
+
+			[simple503]
+			extract_metadata = false
+
+		:param config: The unparsed TOML config for the ``simple503`` table.
+		"""
+
+		extract_metadata = config["extract_metadata"]
+		self.assert_type(extract_metadata, bool, ["simple503", "extract_metadata"])
+		return extract_metadata
+
 	def parse_copy(self, config: Dict[str, TOML_TYPES]) -> str:
 		"""
 		Parse the ``copy`` key.
 
 		**Format**: :toml:`Boolean`
 
 		:bold-title:`Example:`
```

### Comparing `simple503-0.3.2/simple503/__main__.py` & `simple503-0.4.0/simple503/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,40 +25,41 @@
 #  OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE
 #  OR OTHER DEALINGS IN THE SOFTWARE.
 #
 
 # stdlib
 import os.path
 import sys
-from typing import Optional
+from typing import Any, Dict, Optional, cast
 
 # 3rd party
 import click
 from consolekit import click_command
 from consolekit.options import auto_default_argument, auto_default_option, flag_option
 from domdf_python_tools.typing import PathLike
 
 __all__ = ["main"]
 
 
-def _configure(ctx, _, filename):
+def _configure(ctx: click.Context, _, filename: PathLike) -> None:
 	# 3rd party
 	import dom_toml
 
 	# this package
 	from simple503.config import Simple503ConfigParser
 
 	if os.path.isfile(filename):
 		config_file_contents = dom_toml.load(filename)
 
 		if "simple503" in config_file_contents:
-			ctx.default_map = Simple503ConfigParser().parse(
+			parsed_config = Simple503ConfigParser().parse(
 					config_file_contents["simple503"],
 					set_defaults=False,
 					)
+			ctx.default_map = cast(Dict[str, Any], parsed_config)
 
 
 @flag_option("--cleanup", help="Cleanup files generated by simple503 in the target directory, and exit.")
 @click.option(
 		"--config",
 		type=click.Path(dir_okay=False),
 		default="simple503.toml",
@@ -74,14 +75,20 @@
 		help="Copy files from the source to the destination, rather than moving them.",
 		)
 @flag_option(
 		"-s/-S",
 		"--sort/--no-sort",
 		help="Sort the wheel files into per-project base directories.",
 		)
+@flag_option(
+		"-e/-E",
+		"--extract-metadata/--no-extract-metadata",
+		help="Extract and serve METADATA files per PEP 658",
+		default=True
+		)
 @auto_default_option(
 		"-B",
 		"--base-url",
 		type=click.STRING,
 		help="The base URL for the Python package repository.",
 		show_default=True,
 		)
@@ -89,29 +96,30 @@
 @click.argument("origin", type=click.STRING)
 @click_command()
 def main(
 		origin: PathLike,
 		target: Optional[PathLike] = None,
 		base_url: str = '/',
 		sort: bool = False,
+		extract_metadata: bool = True,
 		copy: bool = False,
 		cleanup: bool = False,
-		):
+		) -> None:
 	"""
 	Generate a PEP 503 Python package repository in TARGET for the wheels in ORIGIN.
 	"""
 
 	if cleanup:
 		# this package
 		from simple503 import cleanup as do_cleanup
 
 		do_cleanup(target or origin)
 
 	else:
 		# this package
 		from simple503 import make_simple
 
-		make_simple(origin, target, base_url=base_url, sort=sort, copy=copy)
+		make_simple(origin, target, base_url=base_url, sort=sort, copy=copy, extract_metadata=extract_metadata)
 
 
 if __name__ == "__main__":
 	sys.exit(main())
```

### Comparing `simple503-0.3.2/simple503/__init__.py` & `simple503-0.4.0/simple503/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 			from _hashlib import Hash as _Hash
 		except ImportError:
 			pass
 
 __author__: str = "Dominic Davis-Foster"
 __copyright__: str = "2021 Dominic Davis-Foster"
 __license__: str = "MIT License"
-__version__: str = "0.3.2"
+__version__: str = "0.4.0"
 __email__: str = "dominic@davis-foster.co.uk"
 
 __all__ = [
 		"WheelFile",
 		"generate_index",
 		"generate_project_page",
 		"make_simple",
@@ -77,38 +77,42 @@
 def make_simple(
 		origin: PathLike,
 		target: Optional[PathLike] = None,
 		base_url: Union[str, URL] = '/',
 		*,
 		sort: bool = False,
 		copy: bool = False,
+		extract_metadata: bool = True,
 		) -> Dict[str, List["WheelFile"]]:
 	"""
 	Generate a simple repository of Python wheels.
 
 	:param origin: A directory containing wheels. The wheels may be arranged in subdirectories.
 	:param target: The directory to create the repository in.
 		The directory structure of ``origin`` will be recreated there.
 		Defaults to ``origin``.
 	:no-default target:
 	:param base_url: The base URL of the simple repository.
 	:param sort: Sort the wheel files into per-project base directories.
 	:param copy: Copy files from the source to the destination, rather than moving them.
+	:param extract_metadata: Extract and serve METADATA files per :pep:`658`.
 
 	:returns: A mapping of (unnormalized) project names to a list of wheels for that project.
 
 	.. versionchanged:: 0.2.0
 
 		Now ignores wheels in the following directories: ``.git``, ``.hg``, ``.tox``, ``.tox4``,
 		``.nox``, ``venv``, ``.venv``.
 
 	.. versionchanged:: 0.3.0
 
 		* Renamed the ``move`` option to ``sort`` to better reflect its behaviour.
 		* Files are moved to the destination by default, unless the ``copy`` option is :py:obj:`True`.
+
+	.. versionchanged:: 0.4.0  Added the ``extract_metadata`` option.
 	"""
 
 	if target is None:
 		target = origin
 
 	origin = PathPlus(origin).abspath()
 	target = PathPlus(target).abspath()
@@ -142,23 +146,28 @@
 
 		else:
 			if not target_file.is_file() or not wheel_file.samefile(target_file):
 				# note: will not overwrite files with the same name, even if the source file changed
 				target_file.parent.maybe_make(parents=True)
 				move_operation(wheel_file, target_file)
 
-		metadata_filename = target_file.with_suffix(f"{target_file.suffix}.metadata")
-		metadata_filename.write_text(metadata_string)
+		if extract_metadata:
+			metadata_filename = target_file.with_suffix(f"{target_file.suffix}.metadata")
+			metadata_filename.write_text(metadata_string)
+			metadata_hash = get_sha256_hash(metadata_filename)
+
+		else:
+			metadata_hash = None
 
 		projects[wheel_metadata["Name"]].append(
 				WheelFile(
 						filename=target_file.relative_to(target).as_posix(),
 						wheel_hash=get_sha256_hash(target_file),
 						requires_python=wheel_metadata.get("Requires-Python"),
-						metadata_hash=get_sha256_hash(metadata_filename),
+						metadata_hash=metadata_hash,
 						)
 				)
 
 	index_content = str(generate_index(projects.keys(), base_url=base_url))
 	_update_file(target / "index.html", index_content)
 
 	for project_name, project_files in projects.items():
@@ -297,22 +306,22 @@
 			for wheel_file in files:
 				wheel_file.as_anchor(page, base_url)
 				page.br()
 
 	return page
 
 
-def get_meta_tags(page: Airium):
+def get_meta_tags(page: Airium) -> None:
 	# Not part of the spec, but allowed
 	page.meta(name="generator", content=f"simple503 version {__version__}")
 	page.meta(name="pypi:repository-version", content="1.0")
 	page.meta(charset="UTF-8")
 
 
-def cleanup(directory: PathLike):
+def cleanup(directory: PathLike) -> None:
 	"""
 	Cleanup files generated by ``simple503`` in the directory.
 
 	This entails removing:
 
 	* all ``index.html`` files
 	* all ``.whl.metadata`` files
```

