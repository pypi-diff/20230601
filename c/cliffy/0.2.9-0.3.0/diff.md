# Comparing `tmp/cliffy-0.2.9.tar.gz` & `tmp/cliffy-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cliffy-0.2.9.tar", max compression
+gzip compressed data, was "cliffy-0.3.0.tar", max compression
```

## Comparing `cliffy-0.2.9.tar` & `cliffy-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1060 2023-05-23 01:00:11.848763 cliffy-0.2.9/LICENSE
--rw-r--r--   0        0        0     6575 2023-05-23 01:00:11.848763 cliffy-0.2.9/README.md
--rw-r--r--   0        0        0        0 2023-05-23 01:00:11.848763 cliffy-0.2.9/cliffy/__init__.py
--rw-r--r--   0        0        0       97 2023-05-23 01:00:11.848763 cliffy-0.2.9/cliffy/__main__.py
--rw-r--r--   0        0        0     1657 2023-05-23 01:00:11.848763 cliffy-0.2.9/cliffy/builder.py
--rw-r--r--   0        0        0     6705 2023-05-23 01:00:11.848763 cliffy-0.2.9/cliffy/cli.py
--rw-r--r--   0        0        0        0 2023-05-23 01:00:11.848763 cliffy-0.2.9/cliffy/clis/__init__.py
--rw-r--r--   0        0        0     4074 2023-05-23 01:00:11.848763 cliffy-0.2.9/cliffy/commander.py
--rw-r--r--   0        0        0        0 2023-05-23 01:00:11.848763 cliffy-0.2.9/cliffy/commanders/__init__.py
--rw-r--r--   0        0        0      981 2023-05-23 01:00:11.848763 cliffy-0.2.9/cliffy/commanders/click.py
--rw-r--r--   0        0        0     1939 2023-05-23 01:00:11.848763 cliffy-0.2.9/cliffy/commanders/typer.py
--rw-r--r--   0        0        0     2877 2023-05-23 01:00:11.848763 cliffy-0.2.9/cliffy/helper.py
--rw-r--r--   0        0        0     3030 2023-05-23 01:00:11.848763 cliffy-0.2.9/cliffy/homer.py
--rw-r--r--   0        0        0     1392 2023-05-23 01:00:11.848763 cliffy-0.2.9/cliffy/loader.py
--rw-r--r--   0        0        0      297 2023-05-23 01:00:11.848763 cliffy-0.2.9/cliffy/manifests/__init__.py
--rw-r--r--   0        0        0     7504 2023-05-23 01:00:11.848763 cliffy-0.2.9/cliffy/manifests/v1.py
--rw-r--r--   0        0        0      137 2023-05-23 01:00:11.848763 cliffy-0.2.9/cliffy/merger.py
--rw-r--r--   0        0        0     4971 2023-05-23 01:00:11.848763 cliffy-0.2.9/cliffy/parser.py
--rw-r--r--   0        0        0      905 2023-05-23 01:00:11.848763 cliffy-0.2.9/cliffy/rich.py
--rw-r--r--   0        0        0       47 2023-05-23 01:00:11.848763 cliffy-0.2.9/cliffy/run.py
--rw-r--r--   0        0        0     4271 2023-05-23 01:00:11.848763 cliffy-0.2.9/cliffy/transformer.py
--rw-r--r--   0        0        0     1092 2023-05-23 01:00:11.852763 cliffy-0.2.9/pyproject.toml
--rw-r--r--   0        0        0     7536 1970-01-01 00:00:00.000000 cliffy-0.2.9/PKG-INFO
+-rw-r--r--   0        0        0     1060 2023-06-01 04:37:15.978807 cliffy-0.3.0/LICENSE
+-rw-r--r--   0        0        0     6755 2023-06-01 04:37:15.978807 cliffy-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-01 04:37:15.978807 cliffy-0.3.0/cliffy/__init__.py
+-rw-r--r--   0        0        0       97 2023-06-01 04:37:15.978807 cliffy-0.3.0/cliffy/__main__.py
+-rw-r--r--   0        0        0     1657 2023-06-01 04:37:15.978807 cliffy-0.3.0/cliffy/builder.py
+-rw-r--r--   0        0        0     7365 2023-06-01 04:37:15.978807 cliffy-0.3.0/cliffy/cli.py
+-rw-r--r--   0        0        0        0 2023-06-01 04:37:15.978807 cliffy-0.3.0/cliffy/clis/__init__.py
+-rw-r--r--   0        0        0     6452 2023-06-01 04:37:15.978807 cliffy-0.3.0/cliffy/commander.py
+-rw-r--r--   0        0        0        0 2023-06-01 04:37:15.978807 cliffy-0.3.0/cliffy/commanders/__init__.py
+-rw-r--r--   0        0        0      981 2023-06-01 04:37:15.978807 cliffy-0.3.0/cliffy/commanders/click.py
+-rw-r--r--   0        0        0     1976 2023-06-01 04:37:15.978807 cliffy-0.3.0/cliffy/commanders/typer.py
+-rw-r--r--   0        0        0     3492 2023-06-01 04:37:15.978807 cliffy-0.3.0/cliffy/helper.py
+-rw-r--r--   0        0        0     3036 2023-06-01 04:37:15.978807 cliffy-0.3.0/cliffy/homer.py
+-rw-r--r--   0        0        0     1392 2023-06-01 04:37:15.978807 cliffy-0.3.0/cliffy/loader.py
+-rw-r--r--   0        0        0      396 2023-06-01 04:37:15.978807 cliffy-0.3.0/cliffy/manifests/__init__.py
+-rw-r--r--   0        0        0     7356 2023-06-01 04:37:15.978807 cliffy-0.3.0/cliffy/manifests/v1.py
+-rw-r--r--   0        0        0      137 2023-06-01 04:37:15.978807 cliffy-0.3.0/cliffy/merger.py
+-rw-r--r--   0        0        0     4655 2023-06-01 04:37:15.978807 cliffy-0.3.0/cliffy/parser.py
+-rw-r--r--   0        0        0      972 2023-06-01 04:37:15.982807 cliffy-0.3.0/cliffy/rich.py
+-rw-r--r--   0        0        0       47 2023-06-01 04:37:15.982807 cliffy-0.3.0/cliffy/run.py
+-rw-r--r--   0        0        0     4102 2023-06-01 04:37:15.982807 cliffy-0.3.0/cliffy/transformer.py
+-rw-r--r--   0        0        0     1062 2023-06-01 04:37:15.982807 cliffy-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     7708 1970-01-01 00:00:00.000000 cliffy-0.3.0/PKG-INFO
```

### Comparing `cliffy-0.2.9/LICENSE` & `cliffy-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cliffy-0.2.9/README.md` & `cliffy-0.3.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [![PyPI](https://img.shields.io/pypi/v/cliffy)](https://pypi.org/project/cliffy/)
 ![GitHub](https://img.shields.io/github/license/jaykv/cliffy)
 
 # cliffy :mountain:
 cliffy is a YAML-defined CLI generator, manager, and bundler for python. It offers dynamic abstractions to rapidly build, test, and deploy CLIs.
 
 ## Features
-* Generate CLIs from YAML files
+* Rapidly build CLIs with YAML-defined manifests
 * Manage CLIs- load, list, update, and remove
 * Built-in shell and Python scripting support
 * Supports Jinja2-templating
 * Build and bundle CLIs into self-contained, portable zipapps
 
 ## Install
 * `pip install cliffy`
@@ -19,28 +19,30 @@
 
 * `pip install "cliffy[rich]"` to include [Rich](https://github.com/Textualize/rich) for beautiful text and formatting
 
 ## How it works
 1. Define CLI manifests in YAML files
 2. Run `cli` commands to load, list, update, and remove CLIs
 3. When loaded, cliffy parses the manifest and generates a [Typer](https://github.com/tiangolo/typer) CLI that is deployed directly as a script
-4. Run loaded CLIs straight from the terminal
-5. When ready to share, run `build` or `bundle` to generate portable zipapps built with [Shiv](https://github.com/linkedin/shiv)
+4. Any code starting with `$` will translate to subprocess calls via [PyBash](https://github.com/cliffy-sh/pybash)
+5. Run loaded CLIs straight from the terminal
+6. When ready to share, run `build` or `bundle` to generate portable zipapps built with [Shiv](https://github.com/linkedin/shiv)
 
 ## Usage
 `cli <command>`
-* `init <cli name>`: Generate a template CLI manifest for a new CLI
+* `init <cli name> --raw`: Generate a template CLI manifest for a new CLI
 * `load <manifest>`: Add a new CLI based on the manifest
 * `render <manifest>`: View generated CLI script for a manifest
 * `list` or `ls`: Output a list of loaded CLIs 
 * `update <cli name>`: Reload a loaded CLI
 * `remove <cli name>` or `rm <cli name>`: Remove a loaded CLI
 * `run <manifest> -- <args>`: Runs a CLI manifest as a one-time operation
 * `build <manifest>`: Build a CLI manifest into a self-contained zipapp
 * `bundle <cli name>`: Bundle a loaded CLI into a self-contained zipapp
+* `info <cli name>`: Display CLI metadata
 
 ### Load
 
 1. Define a manifest
 ```yaml
 # hello.yaml
 name: hello
```

### Comparing `cliffy-0.2.9/cliffy/builder.py` & `cliffy-0.3.0/cliffy/builder.py`

 * *Files 23% similar despite different names*

```diff
@@ -18,37 +18,37 @@
         deps = []
 
     if output_dir and not Path(output_dir).exists():
         os.mkdir(output_dir)
 
     with TemporaryDirectory() as tdist:
         copy(script_path, os.path.join(tdist, f"{cli_name}.py"))
-        pip_deps = ['typer'] + deps
+        pip_deps = ["typer"] + deps
 
         pip.install(["--target", tdist] + pip_deps)
 
         runner = CliRunner()
-        output_file = os.path.join(output_dir, f'{cli_name}') if output_dir else cli_name
+        output_file = os.path.join(output_dir, f"{cli_name}") if output_dir else cli_name
 
         return runner.invoke(
             shiv_cli.main,
             [
-                '--site-packages',
+                "--site-packages",
                 tdist,
-                '--compressed',
-                '-e',
-                f'{cli_name}.cli',
-                '-o',
+                "--compressed",
+                "-e",
+                f"{cli_name}.cli",
+                "-o",
                 output_file,
             ],
         )
 
 
 def run_cli(cli_name: str, script_code: str, args: tuple) -> None:
-    with NamedTemporaryFile(mode='w', prefix=f'{cli_name}_', suffix='.py', delete=True) as runner_file:
+    with NamedTemporaryFile(mode="w", prefix=f"{cli_name}_", suffix=".py", delete=True) as runner_file:
         runner_file.write(script_code)
         runner_file.flush()
         module_path, module_filename = os.path.split(runner_file.name)
         sys.path.append(module_path)
         module = import_module(module_filename[:-3])
 
     runner_argvs = [runner_file.name] + list(args)
```

### Comparing `cliffy-0.2.9/cliffy/cli.py` & `cliffy-0.3.0/cliffy/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,21 +9,21 @@
     from rich_click.rich_group import RichGroup as AliasGroup  # type: ignore
 except ImportError:
     import click
     from .rich import Console
     from click import Group as AliasGroup
 
 from .builder import build_cli, run_cli
-from .helper import CLIFFY_CLI_DIR, out, out_err, print_rich_table, write_to_file
+from .helper import CLIFFY_CLI_DIR, age_datetime, exit_err, indent_block, out, out_err, print_rich_table, write_to_file
 from .homer import get_clis, get_metadata, get_metadata_path, remove_metadata, save_metadata
 from .loader import Loader
 from .manifests import Manifest, set_manifest_version
 from .transformer import Transformer
 
-CONTEXT_SETTINGS = dict(help_option_names=['-h', '--help'])
+CONTEXT_SETTINGS = dict(help_option_names=["-h", "--help"])
 
 
 class AliasedGroup(AliasGroup):  # type: ignore
     def get_command(self, ctx, cmd_name):
         with contextlib.suppress(KeyError):
             cmd_name = ALIASES[cmd_name].name
         return super().get_command(ctx, cmd_name or "")
@@ -32,28 +32,28 @@
 @click.group(context_settings=CONTEXT_SETTINGS, cls=AliasedGroup)
 @click.version_option()
 def cli() -> None:
     pass
 
 
 @cli.command()
-@click.argument('manifests', type=click.File('rb'), nargs=-1)
+@click.argument("manifests", type=click.File("rb"), nargs=-1)
 def load(manifests: list[TextIO]) -> None:
     """Load CLI for given manifest(s)"""
     for manifest in manifests:
         T = Transformer(manifest)
         Loader.load_from_cli(T.cli)
         save_metadata(manifest.name, T.cli)
         out(f"✨ Generated {T.cli.name} CLI v{T.cli.version} ✨", fg="green")
         out("$", fg="magenta", nl=False)
         out(f" {T.cli.name} -h")
 
 
 @cli.command()
-@click.argument('cli_names', type=str, nargs=-1)
+@click.argument("cli_names", type=str, nargs=-1)
 def update(cli_names: list[str]) -> None:
     """Reloads CLI by name"""
     for cli_name in cli_names:
         if cli_metadata := get_metadata(cli_name):
             T = Transformer(open(cli_metadata.runner_path, "r"))
             Loader.load_from_cli(T.cli)
             save_metadata(cli_metadata.runner_path, T.cli)
@@ -61,38 +61,38 @@
             out("$", fg="magenta", nl=False)
             out(f" {T.cli.name} -h")
         else:
             out_err(f"~ {cli_name} not found")
 
 
 @cli.command()
-@click.argument('manifest', type=click.File('rb'))
+@click.argument("manifest", type=click.File("rb"))
 def render(manifest: TextIO) -> None:
     """Render the CLI manifest generation as code"""
     T = Transformer(manifest)
     console = Console()
     console.print(T.cli.code, overflow="fold", emoji=False, markup=False)
     out(f"# Rendered {T.cli.name} CLI v{T.cli.version} ~", fg="green")
 
 
 @cli.command("run")
-@click.argument('manifest', type=click.File('rb'))
-@click.argument('cli_args', type=str, nargs=-1)
+@click.argument("manifest", type=click.File("rb"))
+@click.argument("cli_args", type=str, nargs=-1)
 def cliffy_run(manifest: TextIO, cli_args: tuple[str]) -> None:
     """Run CLI for a manifest"""
     T = Transformer(manifest)
     run_cli(T.cli.name, T.cli.code, cli_args)
 
 
 @cli.command()
-@click.argument('cli_name', type=str, default="cliffy")
-@click.option('--version', '-v', type=str, show_default=True, default="v1", help="Manifest version")
-@click.option('--render', is_flag=True, show_default=True, default=False, help="Render template to terminal directly")
+@click.argument("cli_name", type=str, default="cliffy")
+@click.option("--version", "-v", type=str, show_default=True, default="v1", help="Manifest version")
+@click.option("--render", is_flag=True, show_default=True, default=False, help="Render template to terminal directly")
 @click.option(
-    '--raw',
+    "--raw",
     type=bool,
     is_flag=True,
     show_default=True,
     default=False,
     help="Raw template without boilerplate helpers and examples.",
 )
 def init(cli_name: str, version: str, render: bool, raw: bool) -> None:
@@ -101,88 +101,102 @@
     template = Manifest.get_raw_template(cli_name) if raw else Manifest.get_template(cli_name)
 
     if render:
         console = Console()
         console.print(template, overflow="fold", emoji=False, markup=False)
     else:
         try:
-            write_to_file(f'{cli_name}.yaml', text=template)
+            write_to_file(f"{cli_name}.yaml", text=template)
         except Exception as e:
-            out_err(f"~ error writing to file: {e}")
-            raise SystemExit(1)
+            exit_err(f"~ error writing to file: {e}")
         out(f"+ {cli_name}.yaml", fg="green")
 
 
 @cli.command("list")
 def cliffy_list() -> None:
     "List all CLIs loaded"
-    cols = ["Name", "Version", "Manifest"]
-    rows = [[metadata.cli_name, metadata.version, metadata.runner_path] for metadata in get_clis()]
-    print_rich_table(cols, rows, styles=["cyan", "magenta", "green"])
+    cols = ["Name", "Version", "Age", "Manifest"]
+    rows = [
+        [metadata.cli_name, metadata.version, age_datetime(metadata.loaded), metadata.runner_path]
+        for metadata in get_clis()
+    ]
+    print_rich_table(cols, rows, styles=["cyan", "magenta", "green", "blue"])
 
 
 @cli.command()
-@click.argument('cli_names', type=str, nargs=-1)
+@click.argument("cli_names", type=str, nargs=-1)
 def remove(cli_names: list[str]) -> None:
     "Remove a loaded CLI by name"
     for cli_name in cli_names:
         if get_metadata_path(cli_name):
             remove_metadata(cli_name)
             Loader.unload_cli(cli_name)
             out(f"~ {cli_name} removed 💥", fg="green")
         else:
             out_err(f"~ {cli_name} not loaded")
 
 
 @cli.command()
-@click.argument('cli_names', type=str, nargs=-1)
-@click.option('--debug', is_flag=True, show_default=True, default=False, help="Display build output")
-@click.option('--output-dir', '-o', type=click.Path(file_okay=False, dir_okay=True, writable=True), help="Output dir")
+@click.argument("cli_names", type=str, nargs=-1)
+@click.option("--debug", is_flag=True, show_default=True, default=False, help="Display build output")
+@click.option("--output-dir", "-o", type=click.Path(file_okay=False, dir_okay=True, writable=True), help="Output dir")
 def bundle(cli_names: list[str], debug: bool, output_dir: str) -> None:
     "Bundle a loaded CLI into a zipapp"
     for cli_name in cli_names:
         if not (metadata := get_metadata(cli_name)):
             out_err(f"~ {cli_name} not loaded")
             continue
 
         result = build_cli(
-            cli_name, script_path=f'{CLIFFY_CLI_DIR}/{cli_name}.py', deps=metadata.requires, output_dir=output_dir
+            cli_name, script_path=f"{CLIFFY_CLI_DIR}/{cli_name}.py", deps=metadata.requires, output_dir=output_dir
         )
 
         if result.exit_code != 0:
             out(result.stdout)
             out_err(f"~ {cli_name} bundle failed")
             continue
 
         if debug:
             out(result.stdout)
         out(f"+ {cli_name} bundled 📦", fg="green")
 
 
 @cli.command()
-@click.argument('manifests', type=click.File('rb'), nargs=-1)
-@click.option('--debug', is_flag=True, show_default=True, default=False, help="Display build output")
-@click.option('--output-dir', '-o', type=click.Path(file_okay=False, dir_okay=True, writable=True), help="Output dir")
+@click.argument("manifests", type=click.File("rb"), nargs=-1)
+@click.option("--debug", is_flag=True, show_default=True, default=False, help="Display build output")
+@click.option("--output-dir", "-o", type=click.Path(file_okay=False, dir_okay=True, writable=True), help="Output dir")
 def build(manifests: list[TextIO], debug: bool, output_dir: str) -> None:
     "Build a CLI manifest into a zipapp"
     for manifest in manifests:
         T = Transformer(manifest, validate_requires=False)
-        with NamedTemporaryFile(mode='w', prefix=f'{T.cli.name}_', suffix='.py', delete=True) as script:
+        with NamedTemporaryFile(mode="w", prefix=f"{T.cli.name}_", suffix=".py", delete=True) as script:
             script.write(T.cli.code)
             script.flush()
             result = build_cli(T.cli.name, script_path=script.name, deps=T.cli.requires, output_dir=output_dir)
 
         if result.exit_code != 0:
             out(result.stdout)
             out_err(f"~ {T.cli.name} build failed")
             continue
 
         if debug:
             out(result.stdout)
         out(f"+ {T.cli.name} built 📦", fg="green")
 
 
+@cli.command()
+@click.argument("cli_name", type=str)
+def info(cli_name: str):
+    "Display CLI info"
+    metadata = get_metadata(cli_name) or exit_err(f"~ {cli_name} not loaded")
+    out(f"{click.style('name:', fg='blue')} {metadata.cli_name}")
+    out(f"{click.style('version:', fg='blue')} {metadata.version}")
+    out(f"{click.style('requires:', fg='blue')} {metadata.requires}")
+    out(f"{click.style('age:', fg='blue')} {age_datetime(metadata.loaded)} ({metadata.loaded.ctime()})")
+    out(f"{click.style('manifest:', fg='blue')}\n{indent_block(metadata.manifest, spaces=2)}")
+
+
 ALIASES = {
     "add": load,
     "rm": remove,
     "ls": cliffy_list,
 }
```

### Comparing `cliffy-0.2.9/cliffy/commander.py` & `cliffy-0.3.0/cliffy/commander.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,114 +1,180 @@
-from collections import defaultdict, namedtuple
+from collections import defaultdict
 from typing import DefaultDict
 
-from .manifests import Manifest
+from pybash.transformer import transform as transform_bash
+from pydantic import BaseModel
+
+from .manifests import COMMAND_BLOCK, Manifest
 from .parser import Parser
 
-Command = namedtuple('Command', ['name', 'script'])
-CLI = namedtuple('CLI', ['name', 'version', 'code', 'requires'])
+
+class Command(BaseModel):
+    name: str
+    script: COMMAND_BLOCK
+
+
+class CLI(BaseModel):
+    name: str
+    version: str
+    code: str
+    requires: list[str] = []
+
+
+class Group(BaseModel):
+    name: str
+    commands: list[Command]
+    help: str = ""
 
 
 class Commander:
     """Generates commands based on the command config"""
 
-    __slots__ = ('manifest', 'parser', 'cli', 'groups', 'greedy')
+    __slots__ = ("manifest", "parser", "cli", "groups", "greedy", "commands", "root_commands")
 
     def __init__(self, manifest: Manifest) -> None:
         self.manifest = manifest
         self.parser = Parser(self.manifest)
         self.cli: str = ""
-        self.groups: DefaultDict[str, dict] = defaultdict(lambda: defaultdict())
+        self.groups: dict[str, Group] = {}
         self.greedy: list[Command] = []
+        self.commands: list[Command] = [
+            Command(name=name, script=script) for name, script in self.manifest.commands.items()
+        ]
+        self.root_commands: list[Command] = [command for command in self.commands if "." not in command.name]
+        self.build_groups()
+
+    def build_groups(self) -> None:
+        groups: DefaultDict[str, list[Command]] = defaultdict(list)
+        group_help_dict: dict[str, str] = {}
+        for command in self.commands:
+            # Check for greedy commands- evaluate them at the end
+            if self.is_greedy(command.name):
+                self.greedy.append(command)
+                continue
+
+            if "." in command.name:
+                group_name = command.name.split(".")[:-1][-1]
+                groups[group_name].append(command)
+            else:
+                for script_block in command.script:
+                    if isinstance(script_block, dict) and script_block.get("help"):
+                        group_help = script_block["help"]
+                        group_help_dict[command.name] = group_help
+
+        for group_name, commands in groups.items():
+            self.groups[group_name] = Group(
+                name=group_name, commands=commands, help=group_help_dict.get(group_name, "")
+            )
 
     def build_cli(self) -> None:
         self.add_base_imports()
         self.add_imports()
+        self.add_vars()
         self.add_base_cli()
         self.add_functions()
-        for name, script in self.manifest.commands.items():
-            current_command = Command(name, script)
-            self.add_command(current_command)
-
+        self.add_root_commands()
+        self.add_subcommands()
         self.add_greedy_commands()
         self.add_main_block()
 
-    def add_command(self, command: Command) -> None:
-        # Check for greedy commands- evaluate them at the end
-        if self.is_greedy(command.name):
-            self.greedy.append(command)
-            return
-
-        if '.' in command.name:
-            # Sub command- nested commands
-            group = command.name.split('.')[:-1][-1]
-
-            if group not in self.groups:
-                self.add_group(group, command)
-
-            self.groups[group][command.name] = command
-            self.add_sub_command(command, group)
-        else:
-            # Group command- top-level commands
-            if command.name not in self.groups:
-                self.groups[command.name] = {}
-
-                # TODO: by default, add a group app from here to allow for group-level invokes
-                # self.add_group(command.name, command)
-
-            self.add_group_command(command)
+    def add_root_commands(self) -> None:
+        for root_command in self.root_commands:
+            self.add_root_command(root_command)
+
+    def add_subcommands(self) -> None:
+        for group in self.groups.values():
+            self.add_group(group)
+            for subcommand in group.commands:
+                self.add_sub_command(subcommand, group)
 
     def add_imports(self) -> None:
+        if not self.manifest.imports:
+            return
+
         if isinstance(self.manifest.imports, str):
             self.cli += self.manifest.imports + "\n"
         elif isinstance(self.manifest.imports, list):
             for _import in self.manifest.imports:
                 self.cli += _import + "\n"
+        self.cli += "\n"
 
-    def add_functions(self) -> None:
+    def add_vars(self) -> None:
+        if not self.manifest.vars:
+            return
+
+        for var, val in self.manifest.vars.items():
+            if isinstance(val, dict):
+                self.cli += f"{var} = {next(iter(val))}\n"
+            else:
+                self.cli += f"{var} = '{val}'\n"
         self.cli += "\n"
+
+    def add_functions(self) -> None:
+        if not self.manifest.functions:
+            return
+
         for func in self.manifest.functions:
-            self.cli += f"{func}\n"
+            self.cli += f"{transform_bash(func)}\n"
         self.cli += "\n"
 
+    def add_command(self, command: Command) -> None:
+        if "." in command.name:
+            group = command.name.split(".")[:-1][-1]
+            self.add_sub_command(command, self.groups[group])
+
     def add_greedy_commands(self) -> None:
         """Greedy commands get lazy-loaded. Only supported for group-commands currently"""
         for greedy_command in self.greedy:
-            if greedy_command.name.startswith('(*)'):
+            if greedy_command.name.startswith("(*)"):
                 for group in self.groups:
                     # make it lazy and interpolate
-                    lazy_command_name = greedy_command.name.replace('(*)', group)
-                    lazy_command_script = greedy_command.script.replace('{(*)}', group)
+                    lazy_command_name = greedy_command.name.replace("(*)", group)
+                    lazy_command_script = ""
+                    if isinstance(greedy_command.script, str):
+                        lazy_command_script = greedy_command.script.replace("{(*)}", group)
+                    elif isinstance(greedy_command.script, list):
+                        lazy_command_script = []
+                        for script_block in greedy_command.script:
+                            if isinstance(script_block, dict):
+                                lazy_command_script.append(script_block["help"].replace("{(*)}", group))
+                            else:
+                                lazy_command_script.append(script_block.replace("{(*)}", group))
 
                     if greedy_command_args := self.manifest.args.get(greedy_command.name):
                         self.manifest.args[lazy_command_name] = greedy_command_args
 
-                    # lazy parse
-                    self.add_command(Command(lazy_command_name, lazy_command_script))
+                    # lazy load
+                    lazy_command = Command(name=lazy_command_name, script=lazy_command_script)
+                    self.commands.append(lazy_command)
+                    self.add_command(lazy_command)
 
     def is_greedy(self, val: str) -> bool:
         """Greedy strings must contain (*)- marked to be evaluated lazily."""
-        return '(*)' in val
+        return "(*)" in val
 
-    def add_group(self, group: str, command: Command) -> None:
+    def add_group(self, group: Group) -> None:
         raise NotImplementedError
 
     def add_base_imports(self) -> None:
         raise NotImplementedError
 
     def add_base_cli(self) -> None:
         raise NotImplementedError
 
+    def add_root_command(self, command: Command) -> None:
+        raise NotImplementedError
+
     def add_group_command(self, command: Command) -> None:
         raise NotImplementedError
 
-    def add_sub_command(self, command: Command, group: str) -> None:
+    def add_sub_command(self, command: Command, group: Group) -> None:
         raise NotImplementedError
 
     def add_main_block(self) -> None:
         raise NotImplementedError
 
 
 def build_cli(manifest: Manifest, commander_cls=Commander) -> CLI:
     commander = commander_cls(manifest)
     commander.build_cli()
-    return CLI(manifest.name, manifest.version, commander.cli, manifest.requires)
+    return CLI(name=manifest.name, version=manifest.version, code=commander.cli, requires=manifest.requires)
```

### Comparing `cliffy-0.2.9/cliffy/commanders/click.py` & `cliffy-0.3.0/cliffy/commanders/click.py`

 * *Files identical despite different names*

### Comparing `cliffy-0.2.9/cliffy/commanders/typer.py` & `cliffy-0.3.0/cliffy/commanders/typer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,63 +1,66 @@
 import datetime
 
-from ..commander import Command, Commander
+from ..commander import Command, Commander, Group
 
 
 class TyperCommander(Commander):
     """Generates commands based on the command config"""
 
     def add_base_imports(self):
         self.cli = f"""## Generated {self.manifest.name} on {datetime.datetime.now()}
 import typer
 import subprocess
 from typing import Optional
-CONTEXT_SETTINGS = dict(help_option_names=['-h', '--help'])
 """
 
     def add_base_cli(self) -> None:
         self.cli += """
+CONTEXT_SETTINGS = dict(help_option_names=['-h', '--help'])
 cli = typer.Typer(context_settings=CONTEXT_SETTINGS"""
 
         if self.manifest.cli_options:
             self.cli += f",{self.parser.to_args(self.manifest.cli_options)}"
         if self.manifest.help:
-            self.cli += f', help="{self.manifest.help}"'
+            self.cli += f', help="""{self.manifest.help}"""'
 
         self.cli += f""")
 __version__ = '{self.manifest.version}'
 __cli_name__ = '{self.manifest.name}'
 
+
 def version_callback(value: bool):
     if value:
         print(f"{{__cli_name__}}, {{__version__}}")
         raise typer.Exit()
 
+
 @cli.callback()
 def main(version: Optional[bool] = typer.Option(None, '--version', callback=version_callback, is_eager=True)):
     pass
-"""
 
-    def add_group(self, group: str, command: Command) -> None:
-        self.cli += f"""{group}_app = typer.Typer(); cli.add_typer({group}_app, name="{group}");"""
+"""
 
-    def add_group_command(self, command: Command) -> None:
+    def add_root_command(self, command: Command) -> None:
         self.cli += f"""
 @cli.command("{self.parser.get_parsed_command_name(command)}")
 def {self.parser.get_command_func_name(command)}({self.parser.parse_args(command)}):
 {self.parser.parse_command(command.script)}
+"""
 
+    def add_group(self, group: Group) -> None:
+        self.cli += f"""{group.name}_app = typer.Typer()
+cli.add_typer({group.name}_app, name="{group.name}", help="{group.help}")
 """
 
-    def add_sub_command(self, command: Command, group: str) -> None:
+    def add_sub_command(self, command: Command, group: Group) -> None:
         self.cli += f"""
-@{group}_app.command("{self.parser.get_parsed_command_name(command)}")
+@{group.name}_app.command("{self.parser.get_parsed_command_name(command)}")
 def {self.parser.get_command_func_name(command)}({self.parser.parse_args(command)}):
 {self.parser.parse_command(command.script)}
-
 """
 
     def add_main_block(self) -> None:
         self.cli += """
 if __name__ == "__main__":
     cli()
 """
```

### Comparing `cliffy-0.2.9/cliffy/helper.py` & `cliffy-0.3.0/cliffy/helper.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 import operator
 import os
 import platform
 import subprocess
 import sys
+from datetime import datetime
 from importlib.resources import files
 from pathlib import Path
-from typing import Any, Optional
+from typing import Any, NoReturn, Optional
 
 from click import secho
 from packaging import version
 from pydantic import BaseModel
 
 try:
     from rich.console import Console  # type: ignore
     from rich.table import Table  # type: ignore
 except ImportError:
     from .rich import Console, Table
 
 HOME_PATH = str(Path.home())
 PYTHON_BIN = f"{sys.exec_prefix}/Scripts" if platform.system() == "Windows" else f"{sys.exec_prefix}/bin"
 PYTHON_EXECUTABLE = sys.executable
-CLIFFY_CLI_DIR = files('cliffy.clis')
+CLIFFY_CLI_DIR = files("cliffy.clis")
 CLIFFY_HOME_PATH = f"{HOME_PATH}/.cliffy"
 OPERATOR_MAP = {
-    '==': operator.eq,
-    '!=': operator.ne,
-    '>=': operator.ge,
-    '<=': operator.le,
-    '<': operator.lt,
-    '>': operator.gt,
+    "==": operator.eq,
+    "!=": operator.ne,
+    ">=": operator.ge,
+    "<=": operator.le,
+    "<": operator.lt,
+    ">": operator.gt,
 }
 
 
 class RequirementSpec(BaseModel):
     name: str
     operator: Optional[str]
     version: Optional[str]
@@ -49,51 +50,56 @@
 
 def make_executable(path: str) -> None:
     mode = os.stat(path).st_mode
     mode |= (mode & 0o444) >> 2
     os.chmod(path, mode)
 
 
+def indent_block(block: str, spaces=4) -> str:
+    blocklines = block.splitlines()
+    return "\n".join([" " * spaces + line for line in blocklines])
+
+
 def wrap_as_comment(text: str, split_on: Optional[str] = None) -> str:
     if split_on:
         joiner = "\n# "
         return f"# {joiner.join(text.split(split_on))}"
 
     return f"# {text}"
 
 
 def wrap_as_var(text: str) -> str:
-    return '{{' + text + '}}'
+    return "{{" + text + "}}"
 
 
 def print_rich_table(cols: list[str], rows: list[list[str]], styles: list[str]) -> None:
     table = Table()
     for style, col in zip(styles, cols):
         table.add_column(col, style=style)
     for row in rows:
         table.add_row(*row)
 
     console = Console()
     console.print(table)
 
 
 def get_installed_pip_packages() -> dict[str, str]:
-    reqs = subprocess.check_output([sys.executable, '-m', 'pip', 'freeze'])
+    reqs = subprocess.check_output([sys.executable, "-m", "pip", "freeze"])
     installed_packages = {}
     for r in reqs.split():
-        r_spec = r.decode().split('==')
+        r_spec = r.decode().split("==")
         if len(r_spec) > 1:
             installed_packages[r_spec[0]] = r_spec[1]
     return installed_packages
 
 
 def parse_requirement(requirement: str) -> RequirementSpec:
     for op in OPERATOR_MAP:
         if op in requirement:
-            parts = requirement.replace(' ', '').split(op)
+            parts = requirement.replace(" ", "").split(op)
             return RequirementSpec(name=parts[0], operator=op, version=parts[1])
 
     return RequirementSpec(name=requirement.strip(), operator=None, version=None)
 
 
 def compare_versions(version1: str, version2: str, op: str) -> bool:
     v1 = version.parse(version1)
@@ -102,8 +108,24 @@
 
 
 def out(text: str, **echo_kwargs: Any) -> None:
     secho(text, **echo_kwargs)
 
 
 def out_err(text: str) -> None:
-    secho(f"{text} 💔", fg='red', err=True)
+    secho(f"{text} 💔", fg="red", err=True)
+
+
+def exit_err(text: str) -> NoReturn:
+    secho(f"{text} 💔", fg="red", err=True)
+    raise SystemExit(1)
+
+
+def age_datetime(date: datetime) -> str:
+    delta = datetime.now() - date
+    if delta.seconds > 86400:
+        return f"{delta.days}d"
+    elif delta.seconds > 3600:
+        return f"{delta.seconds // 3600}h"
+    elif delta.seconds > 60:
+        return f"{delta.seconds // 60}m"
+    return f"{delta.seconds}s"
```

### Comparing `cliffy-0.2.9/cliffy/homer.py` & `cliffy-0.3.0/cliffy/homer.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,28 +15,28 @@
     """Stores CLI metadata
 
     Args:
         manifest_path (str): CLI manifest path
         cli (CLI): CLI
     """
     abs_manifest_path = os.path.realpath(manifest_path)
-    encoded_runnerpath = b32encode(cli.name.encode('ascii')).decode('utf-8')
+    encoded_runnerpath = b32encode(cli.name.encode("ascii")).decode("utf-8")
     save_metadata_path = f"{CLIFFY_HOME_PATH}/{encoded_runnerpath}/{cli.name}.json"
     with open(manifest_path, "r") as manifest:
         write_to_file(
             save_metadata_path,
             json.dumps(
                 CLIMetadata(
                     cli_name=cli.name,
                     runner_path=abs_manifest_path,
                     version=cli.version,
                     loaded=datetime.now(),
                     manifest=manifest.read(),
                     requires=cli.requires,
-                ).dict(),
+                ).model_dump(),
                 default=str,
             ),
         )
 
 
 def remove_metadata(cli_name: str) -> None:
     """Clears CLI metadata by name
@@ -106,10 +106,10 @@
 
 def get_clis() -> Iterator[CLIMetadata]:
     """Fetches loaded CLIs metadata iteratively
 
     Yields:
         Iterator[CLIMetadata]: CLI metadata
     """
-    metadata_paths = Path(CLIFFY_HOME_PATH).glob('*/*')
+    metadata_paths = Path(CLIFFY_HOME_PATH).glob("*/*")
     for metadata_path in metadata_paths:
         yield get_metadata_bypath(metadata_path)
```

### Comparing `cliffy-0.2.9/cliffy/loader.py` & `cliffy-0.3.0/cliffy/loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 from .commander import CLI
 from .helper import CLIFFY_CLI_DIR, PYTHON_BIN, PYTHON_EXECUTABLE, write_to_file
 
 
 class Loader:
-    __slots__ = ('cli',)
+    __slots__ = ("cli",)
 
     def __init__(self, cli: CLI) -> None:
         self.cli = cli
 
     def deploy_cli(self) -> str:
         cli_path = Loader.get_cli_path(self.cli.name)
         write_to_file(cli_path, self.cli.code)
```

### Comparing `cliffy-0.2.9/cliffy/manifests/v1.py` & `cliffy-0.3.0/cliffy/manifests/v1.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from datetime import datetime
-from typing import Literal, Union
+from typing import Any, Literal, Union
 
 from pydantic import BaseModel, Field
 
 from ..helper import wrap_as_comment, wrap_as_var
 
+COMMAND_BLOCK = Union[str, list[Union[str, dict[Literal["help"], str]]]]
+
 
 class CLIManifest(BaseModel):
     name: str = Field(
         description="The name of the CLI. "
         "This will be used as the script name when invoking the CLI from the command line."
     )
     version: str = Field(
@@ -26,22 +28,22 @@
     )
     includes: list[str] = Field(
         [],
         description="List of external CLI manifest paths to include into the main manifest. "
         "Performs a deep merge of manifests sequentially in the order given to assemble a merged manifest. "
         "and finally, deep merges the merged manifest with the main manifest.",
     )
-    vars: dict[str, str] = Field(
+    vars: dict[str, Union[str, dict[str, None]]] = Field(
         {},
         description="A mapping defining manifest variables that can be referenced in any other blocks. "
         "Environments variables can be used in this section with ${some_env_var} for dynamic parsing. "
         "Supports jinja2 formatted expressions as values. "
         "Interpolate defined vars in other blocks jinja2-styled {{ var_name }}.",
     )
-    commands: dict[str, Union[str, list[Union[str, dict[Literal['help'], str]]]]] = Field(
+    commands: dict[str, COMMAND_BLOCK] = Field(
         {},
         description="A mapping containing the command definitions for the CLI. "
         "Each command should have a unique key- which can be either a group command or nested subcommands. "
         "Nested subcommands are joined by '.' in between each level. "
         "A special (*) wildcard can be used to spread the subcommand to all group-level commands. "
         "The value is the python code to run when the command is called "
         "OR a list of bash commands to run (prefixed with $).",
@@ -65,75 +67,79 @@
     )
     types: dict[str, str] = Field(
         {},
         description="A mapping containing any shared type definitions. "
         "These types can be referenced by name in the args section to provide type annotations "
         "for params and options defined in the args section.",
     )
-    cli_options: dict[str, str] = Field(
+    cli_options: dict[str, Any] = Field(
         {},
-        Description="A mapping for any additional options that can be used to customize the behavior of the CLI.",
+        description="A mapping for any additional options that can be used to customize the behavior of the CLI.",
     )
 
     @classmethod
-    def get_field_description(cls, field_name: str, as_comment: bool = False) -> str:
-        field = cls.__fields__.get(field_name)
-        if field and field.field_info.description:
+    def get_field_description(cls, field_name: str, as_comment: bool = True) -> str:
+        field = cls.model_fields.get(field_name)
+        if field and field.description:
             if as_comment:
-                return wrap_as_comment(field.field_info.description, split_on=". ")
-            return field.field_info.description
+                return wrap_as_comment(field.description, split_on=". ")
+            return field.description
         return ""
 
     @classmethod
     def get_template(cls, name: str) -> str:
         return f"""# cliffy v1 template
 manifestVersion: v1
 
-{cls.get_field_description('name', as_comment=True)}
+{cls.get_field_description('name')}
 name: {name} 
 
-{cls.get_field_description('version', as_comment=True)}
+{cls.get_field_description('version')}
 version: 0.1.0
 
-{cls.get_field_description('includes', as_comment=True)}
+{cls.get_field_description('help')}
+help: hello world
+
+{cls.get_field_description('includes')}
 includes: []
 
-{cls.get_field_description('requires', as_comment=True)}
+{cls.get_field_description('requires')}
 requires: []
 
-{cls.get_field_description('vars', as_comment=True)}
+{cls.get_field_description('vars')}
 vars:
     default_mood: happy
+    debug_mode: "{{ env['DEBUG'] or 'False' }}"
 
-{cls.get_field_description('imports', as_comment=True)}
+{cls.get_field_description('imports')}
 imports:
     - import os
     - |
         from collections import defaultdict
         import re
 
-{cls.get_field_description('functions', as_comment=True)}
+{cls.get_field_description('functions')}
 functions:
     - |
         def greet_name(name: str):
             print("hello " + name)
 
-{cls.get_field_description('types', as_comment=True)}
+{cls.get_field_description('types')}
 types:
     Language: str = typer.Option("english", "-l", help="Language to greet in", prompt=True)
 
-{cls.get_field_description('args', as_comment=True)}
+{cls.get_field_description('args')}
 args:
     world: [--name|-n: str!]                      # a REQUIRED option
     greet.all: 
         - names: str!                             # a REQUIRED param as denoted by the ! at the end
         - mood: str = "{wrap_as_var("default_mood")}"          # an OPTIONAL param that uses a manifest var as default
         - --language: Language                    # an option with a default that uses Language type as arg definition
 
-{cls.get_field_description('commands', as_comment=True)}
+{cls.get_field_description('commands')}
 commands:
     # this is a parent command that will get invoked with: hello world
     world: 
         - |
             \"\"\"
             Help text for list
             \"\"\"
@@ -151,48 +157,51 @@
     @classmethod
     def get_raw_template(cls, name: str) -> str:
         return f"""
 # cliffy v1 raw template
 
 manifestVersion: v1
 
-{cls.get_field_description('name', as_comment=True)}
+{cls.get_field_description('name')}
 name: {name} 
 
-{cls.get_field_description('version', as_comment=True)}
+{cls.get_field_description('version')}
 version: 0.1.0
 
-{cls.get_field_description('includes', as_comment=True)}
+{cls.get_field_description('help')}
+help: 
+
+{cls.get_field_description('includes')}
 includes: []
 
-{cls.get_field_description('vars', as_comment=True)}
+{cls.get_field_description('vars')}
 vars: {{}}
 
-{cls.get_field_description('imports', as_comment=True)}
+{cls.get_field_description('imports')}
 imports: []
 
-{cls.get_field_description('functions', as_comment=True)}
+{cls.get_field_description('functions')}
 functions: []
 
-{cls.get_field_description('types', as_comment=True)}
+{cls.get_field_description('types')}
 types: {{}}
 
-{cls.get_field_description('args', as_comment=True)}
+{cls.get_field_description('args')}
 args: {{}}
 
-{cls.get_field_description('commands', as_comment=True)}
+{cls.get_field_description('commands')}
 commands: {{}}
 
 """
 
 
 class IncludeManifest(BaseModel):
     """Special manifest specifically to define the allowed named objects that can be included"""
 
-    commands: dict[str, Union[str, list[Union[str, dict[Literal['help'], str]]]]] = {}
+    commands: dict[str, Union[str, list[Union[str, dict[Literal["help"], str]]]]] = {}
     imports: Union[str, list[str]] = []
     functions: list[str] = []
     args: dict[str, list[dict[str, str]]] = {}
     types: dict[str, str] = {}
     cli_options: dict[str, str] = {}
     requires: list[str]
```

### Comparing `cliffy-0.2.9/cliffy/parser.py` & `cliffy-0.3.0/cliffy/parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,56 +4,52 @@
 from pybash.transformer import transform as transform_bash
 
 from .manifests import Manifest
 
 
 class Parser:
 
-    __slots__ = ('manifest',)
+    __slots__ = ("manifest",)
 
     def __init__(self, manifest: Manifest) -> None:
         self.manifest = manifest
 
     def is_param_required(self, param_type: str) -> bool:
         return (
-            param_type.strip().endswith('!')
-            if '=' not in param_type
-            else param_type.split('=')[0].strip().endswith('!')
+            param_type.strip().endswith("!")
+            if "=" not in param_type
+            else param_type.split("=")[0].strip().endswith("!")
         )
 
     def is_param_option(self, param_name: str) -> bool:
-        return '-' in param_name
+        return "-" in param_name
 
     def get_default_param_val(self, param_type: str) -> str:
-        return param_type.split('=')[1].strip() if '=' in param_type else ""
+        return param_type.split("=")[1].strip() if "=" in param_type else ""
 
     def capture_param_aliases(self, param_name: str) -> Tuple[str, list[str]]:
-        if '|' not in param_name:
-            return param_name.replace('-', ''), []
+        if "|" not in param_name:
+            return param_name.replace("-", ""), []
 
-        base_param_name = param_name.split('|')[0].replace('-', '')
-        aliases = param_name.split('|')[1:]
+        base_param_name = param_name.split("|")[0].replace("-", "").strip()
+        aliases = param_name.split("|")[1:]
 
         return base_param_name, aliases
 
-    def parse_command_block(self, script: str):
-        ## Bash commands start with $
-        if script.strip().startswith('$'):
-            pybash_script = f'>{script[1:].strip()}'
-            return " " * 4 + transform_bash(pybash_script)
+    def parse_command_block(self, script: str) -> str:
+        script = transform_bash(script)
+        return "".join(" " * 4 + line + "\n" for line in script.split("\n"))
 
-        return "".join(" " * 4 + line + "\n" for line in script.split('\n'))
-
-    def parse_command(self, block: Union[str, list[Union[str, dict[Literal['help'], str]]]]) -> str:
+    def parse_command(self, block: Union[str, list[Union[str, dict[Literal["help"], str]]]]) -> str:
         if isinstance(block, list):
             script_block = []
             help_text = ""
             for block_elem in block:
                 if isinstance(block_elem, dict):
-                    help_text = block_elem.get('help', '')
+                    help_text = block_elem.get("help", "")
                 else:
                     script_block.append(block_elem)
 
             code = f'    """\n    {help_text}\n    """\n' if help_text else ""
             code += "".join(map(self.parse_command_block, script_block))
         else:
             code = self.parse_command_block(block)
@@ -71,33 +67,33 @@
     ) -> str:
         parsed_arg_type = f"{arg_name}: {arg_type} = typer.{typer_cls}"
 
         if not default_val:
             # Required param needs ...
             parsed_arg_type += "(..." if is_required else "(None"
         else:
-            parsed_arg_type += f"({default_val}"
+            parsed_arg_type += f"({default_val.strip()}"
 
         if aliases:
             parsed_arg_type += f', "--{arg_name}"'
             for alias in aliases:
-                parsed_arg_type += f', "{alias}"'
+                parsed_arg_type += f', "{alias.strip()}"'
 
-        parsed_arg_type += '),'
+        parsed_arg_type += "),"
         return parsed_arg_type
 
     def parse_arg(self, arg_name: str, arg_type: str) -> str:
         is_required = self.is_param_required(arg_type)
         default_val = self.get_default_param_val(arg_type)
-        param_type = 'Option' if self.is_param_option(arg_name) else 'Argument'
+        param_type = "Option" if self.is_param_option(arg_name) else "Argument"
         arg_aliases: list[str] = []
 
         # extract default val before parsing it
-        if '=' in arg_type:
-            arg_type = arg_type.split('=')[0].strip()
+        if "=" in arg_type:
+            arg_type = arg_type.split("=")[0].strip()
 
         # strip - before parsing it
         if self.is_param_option(arg_name):
             arg_name, arg_aliases = self.capture_param_aliases(arg_name)
 
         # strip ! before parsing it
         if is_required:
@@ -123,27 +119,23 @@
         command_args = self.manifest.args.get(command.name)
         if not command_args:
             return ""
 
         parsed_command_args = ""
         for arg in command_args:
             arg_name, arg_type = next(iter(arg.items()))
-            parsed_command_args += f'{self.parse_arg(arg_name.strip(), arg_type.strip())} '
+            parsed_command_args += f"{self.parse_arg(arg_name.strip(), arg_type.strip())} "
 
         # strip the extra ", "
         return parsed_command_args[:-2]
 
     def get_command_func_name(self, command) -> str:
-        """land.build -> land_build or sell -> sell"""
-        return command.name.replace('.', '_')
+        """a.b -> a_b, c -> c"""
+        return command.name.replace(".", "_")
 
     def get_parsed_command_name(self, command) -> str:
-        """land.build -> build or sell -> sell"""
-        return command.name.split('.')[-1] if '.' in command.name else command.name
-
-    def indent_block(self, block: str) -> str:
-        blocklines = block.splitlines()
-        return "\n".join([" " * 4 + line for line in blocklines])
+        """a.b -> b or a -> a"""
+        return command.name.split(".")[-1] if "." in command.name else command.name
 
     def to_args(self, d: dict) -> str:
         s = "".join(f" {k}={v}," for k, v in d.items())
         return s[:-1]
```

### Comparing `cliffy-0.2.9/cliffy/rich.py` & `cliffy-0.3.0/cliffy/rich.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ## Mimic rich API methods for rich-less support
-from typing import Any, Union
+from typing import Any
 
 import click
 
 
 class Console:
     def __init__(self) -> None:
         pass
@@ -13,26 +13,28 @@
             click.echo(text)
         else:
             print(text)
 
 
 class Table:
 
-    __slots__ = ('cols', 'rows')
+    __slots__ = ("cols", "rows", "styles")
 
     def __init__(self) -> None:
         self.cols: list[str] = []
         self.rows: list[list[str]] = []
+        self.styles: list[str] = []
 
-    def add_column(self, col: str, style: Union[str, None] = None) -> None:
+    def add_column(self, col: str, style: str = "") -> None:
         self.cols.append(col)
+        self.styles.append(style)
 
     def add_row(self, *row) -> None:
         self.rows.append([*row])
 
     def __str__(self) -> str:
-        text = "".join([click.style(f"{col:10}", fg="magenta") for col in self.cols]) + "\n"
+        text = "".join([click.style(f"{col:10}", fg=self.styles.pop(0)) for col in self.cols]) + "\n"
         for row in self.rows:
             for col in row:
                 text += f"{col:10}"
             text += "\n"
         return text
```

### Comparing `cliffy-0.2.9/cliffy/transformer.py` & `cliffy-0.3.0/cliffy/transformer.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,79 +4,76 @@
 import yaml
 from jinja2 import BaseLoader, Environment, FileSystemLoader
 from pydantic import ValidationError
 from typing_extensions import Self
 
 from .commander import build_cli
 from .commanders.typer import TyperCommander
-from .helper import compare_versions, get_installed_pip_packages, out, out_err, parse_requirement
+from .helper import compare_versions, exit_err, get_installed_pip_packages, out, parse_requirement
 from .manifests import IncludeManifest, Manifest, set_manifest_version
 from .merger import cliffy_merger
 
 
 class Transformer:
     """Loads command manifest and transforms it into a CLI"""
 
-    __slots__ = ('manifest_io', 'command_config', 'manifest_version', 'includes_config', 'manifest', 'cli')
+    __slots__ = ("manifest_io", "command_config", "manifest_version", "includes_config", "manifest", "cli")
 
     def __init__(self, manifest_io: TextIO, *, as_include: bool = False, validate_requires: bool = True) -> None:
         self.manifest_io = manifest_io
         self.command_config = self.load_manifest(manifest_io)
-        self.manifest_version = self.command_config.pop('manifestVersion', 'v1')
+        self.manifest_version = self.command_config.pop("manifestVersion", "v1")
         if self.command_config.get("includes"):
             self.includes_config = self.resolve_includes()
             cliffy_merger.merge(self.command_config, self.includes_config)
 
         set_manifest_version(self.manifest_version)
         if as_include:
             try:
                 self.manifest = IncludeManifest(**self.command_config)
             except ValidationError as e:
-                out_err(f"~ error validating {manifest_io.name}")
                 out(f"{e}")
-                raise SystemExit(1)
+                exit_err(f"~ error validating {manifest_io.name}")
         else:
             try:
                 self.manifest = Manifest(**self.command_config)
             except ValidationError as e:
-                out_err(f"~ error validating {manifest_io.name}")
                 out(f"{e}")
-                raise SystemExit(1)
+                exit_err(f"~ error validating {manifest_io.name}")
+
             if validate_requires:
                 self.validate_cli_requires()
             self.cli = build_cli(self.manifest, commander_cls=TyperCommander)
 
     def validate_cli_requires(self) -> None:
         if not self.manifest.requires:
             return
 
         installed_pip_packages = get_installed_pip_packages()
         for dep in self.manifest.requires:
             dep_spec = parse_requirement(dep)
             if dep_spec.name not in installed_pip_packages:
-                out_err(f"~ missing requirement: `{self.manifest_io.name}` requires `{dep}` to be installed")
-                raise SystemExit(1)
+                exit_err(f"~ missing requirement: `{self.manifest_io.name}` requires `{dep}` to be installed")
 
             if (
                 dep_spec.version
                 and dep_spec.operator
                 and not compare_versions(
                     installed_pip_packages[dep_spec.name],
                     dep_spec.version,
                     dep_spec.operator,
                 )
             ):
-                out_err(
+                exit_err(
                     f"~ missing requirement: `{self.manifest_io.name}` requires `{dep}` to be installed"
                     f"    found version `{installed_pip_packages[dep_spec.name]}`"
                 )
-                raise SystemExit(1)
 
     def resolve_includes(self) -> dict:
-        include_transforms = map(self.resolve_include_by_path, set(self.command_config['includes']))
+        include_transforms = map(self.resolve_include_by_path, set(self.command_config["includes"]))
         merged_config: dict[str, Any] = {}
         for transformed_include in include_transforms:
             cliffy_merger.merge(merged_config, transformed_include.command_config)
 
         return merged_config
 
     @classmethod
@@ -84,20 +81,19 @@
         with open(path, "r") as m:
             return cls(m, as_include=True)
 
     @staticmethod
     def load_manifest(manifest_io: TextIO) -> dict[str, Any]:
         try:
             manifest_path = os.path.realpath(manifest_io.name)
-            all_vars = yaml.safe_load(open(manifest_path, "r")).get('vars', {})
-            all_vars['env'] = os.environ
+            all_vars = yaml.safe_load(open(manifest_path, "r")).get("vars", {})
+            all_vars["env"] = os.environ
             var_env = Environment(loader=BaseLoader())
             interpolated_vars = {
                 var_env.from_string(str(k)).render(all_vars): var_env.from_string(str(v)).render(all_vars)
                 for k, v in all_vars.items()
             }
             manifest_env = Environment(loader=FileSystemLoader(manifest_path)).get_template("")
             return yaml.safe_load(manifest_env.render(interpolated_vars))
         except yaml.YAMLError as e:
-            out_err("~ error loading manifest")
             out(f"{e}")
-            raise SystemExit(1)
+            exit_err("~ error loading manifest")
```

### Comparing `cliffy-0.2.9/pyproject.toml` & `cliffy-0.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "cliffy"
-version = "0.2.9"
+version = "0.3.0"
 description = "$ cli load from.yaml"
 authors = ["Jay <jay.github0@gmail.com>"]
 repository = "https://github.com/jaykv/cliffy"
 readme = "README.md"
 packages = [{include = "cliffy"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pybash = "^0.3.0"
 pyyaml = "^6.0"
 typer = "^0.9.0"
-pydantic = "^1.10.7"
+pydantic = ">=2.0a4"
 deepmerge = "^1.1.0"
 jinja2 = "^3.1.2"
 packaging = "^23.1"
 rich-click = { version = "^1.6.1", optional = true }
 shellingham = { version = "^1.5.0.post1", optional = true }
 shiv = "^1.0.3"
 
@@ -37,15 +37,14 @@
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
-skip-string-normalization = 1
 
 [tool.isort]
 profile = "black"
 line_length = 120
 default_section = "THIRDPARTY"
 known_first_party = "cliffy"
```

### Comparing `cliffy-0.2.9/PKG-INFO` & `cliffy-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: cliffy
-Version: 0.2.9
+Version: 0.3.0
 Summary: $ cli load from.yaml
 Home-page: https://github.com/jaykv/cliffy
 Author: Jay
 Author-email: jay.github0@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: rich
 Requires-Dist: deepmerge (>=1.1.0,<2.0.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: packaging (>=23.1,<24.0)
 Requires-Dist: pybash (>=0.3.0,<0.4.0)
-Requires-Dist: pydantic (>=1.10.7,<2.0.0)
+Requires-Dist: pydantic (>=2.0a4)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: rich-click (>=1.6.1,<2.0.0) ; extra == "rich"
 Requires-Dist: shellingham (>=1.5.0.post1,<2.0.0) ; extra == "rich"
 Requires-Dist: shiv (>=1.0.3,<2.0.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
 Project-URL: Repository, https://github.com/jaykv/cliffy
 Description-Content-Type: text/markdown
@@ -28,15 +28,15 @@
 [![PyPI](https://img.shields.io/pypi/v/cliffy)](https://pypi.org/project/cliffy/)
 ![GitHub](https://img.shields.io/github/license/jaykv/cliffy)
 
 # cliffy :mountain:
 cliffy is a YAML-defined CLI generator, manager, and bundler for python. It offers dynamic abstractions to rapidly build, test, and deploy CLIs.
 
 ## Features
-* Generate CLIs from YAML files
+* Rapidly build CLIs with YAML-defined manifests
 * Manage CLIs- load, list, update, and remove
 * Built-in shell and Python scripting support
 * Supports Jinja2-templating
 * Build and bundle CLIs into self-contained, portable zipapps
 
 ## Install
 * `pip install cliffy`
@@ -45,28 +45,30 @@
 
 * `pip install "cliffy[rich]"` to include [Rich](https://github.com/Textualize/rich) for beautiful text and formatting
 
 ## How it works
 1. Define CLI manifests in YAML files
 2. Run `cli` commands to load, list, update, and remove CLIs
 3. When loaded, cliffy parses the manifest and generates a [Typer](https://github.com/tiangolo/typer) CLI that is deployed directly as a script
-4. Run loaded CLIs straight from the terminal
-5. When ready to share, run `build` or `bundle` to generate portable zipapps built with [Shiv](https://github.com/linkedin/shiv)
+4. Any code starting with `$` will translate to subprocess calls via [PyBash](https://github.com/cliffy-sh/pybash)
+5. Run loaded CLIs straight from the terminal
+6. When ready to share, run `build` or `bundle` to generate portable zipapps built with [Shiv](https://github.com/linkedin/shiv)
 
 ## Usage
 `cli <command>`
-* `init <cli name>`: Generate a template CLI manifest for a new CLI
+* `init <cli name> --raw`: Generate a template CLI manifest for a new CLI
 * `load <manifest>`: Add a new CLI based on the manifest
 * `render <manifest>`: View generated CLI script for a manifest
 * `list` or `ls`: Output a list of loaded CLIs 
 * `update <cli name>`: Reload a loaded CLI
 * `remove <cli name>` or `rm <cli name>`: Remove a loaded CLI
 * `run <manifest> -- <args>`: Runs a CLI manifest as a one-time operation
 * `build <manifest>`: Build a CLI manifest into a self-contained zipapp
 * `bundle <cli name>`: Bundle a loaded CLI into a self-contained zipapp
+* `info <cli name>`: Display CLI metadata
 
 ### Load
 
 1. Define a manifest
 ```yaml
 # hello.yaml
 name: hello
```

