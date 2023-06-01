# Comparing `tmp/pipen_board-0.2.9.tar.gz` & `tmp/pipen_board-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipen_board-0.2.9.tar", max compression
+gzip compressed data, was "pipen_board-0.3.0.tar", max compression
```

## Comparing `pipen_board-0.2.9.tar` & `pipen_board-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     6141 2023-05-30 20:09:06.138199 pipen_board-0.2.9/README.md
--rw-r--r--   0        0        0      268 2023-05-30 20:09:06.138199 pipen_board-0.2.9/pipen_board/__init__.py
--rw-r--r--   0        0        0     8985 2023-05-30 20:09:06.138199 pipen_board-0.2.9/pipen_board/apis.py
--rw-r--r--   0        0        0     4367 2023-05-30 20:09:06.138199 pipen_board-0.2.9/pipen_board/cli.py
--rw-r--r--   0        0        0    26383 2023-05-30 20:09:06.138199 pipen_board-0.2.9/pipen_board/data_manager.py
--rw-r--r--   0        0        0     6243 2023-05-30 20:09:06.138199 pipen_board-0.2.9/pipen_board/defaults.py
--rw-r--r--   0        0        0    23628 2023-05-30 20:09:06.138199 pipen_board-0.2.9/pipen_board/frontend/build/assets/favicon.png
--rw-r--r--   0        0        0   624476 2023-05-30 20:09:06.138199 pipen_board-0.2.9/pipen_board/frontend/build/assets/index.css
--rw-r--r--   0        0        0   738725 2023-05-30 20:09:06.142199 pipen_board-0.2.9/pipen_board/frontend/build/assets/index.js
--rw-r--r--   0        0        0     4128 2023-05-30 20:09:06.142199 pipen_board-0.2.9/pipen_board/frontend/build/assets/schema.json
--rw-r--r--   0        0        0      406 2023-05-30 20:09:06.142199 pipen_board-0.2.9/pipen_board/frontend/build/index.html
--rw-r--r--   0        0        0     7562 2023-05-30 20:09:06.146199 pipen_board-0.2.9/pipen_board/plugin.py
--rw-r--r--   0        0        0     3293 2023-05-30 20:09:06.146199 pipen_board-0.2.9/pipen_board/quart_app.py
--rw-r--r--   0        0        0       22 2023-05-30 20:09:06.146199 pipen_board-0.2.9/pipen_board/version.py
--rw-r--r--   0        0        0      731 2023-05-30 20:09:06.146199 pipen_board-0.2.9/pyproject.toml
--rw-r--r--   0        0        0     7284 1970-01-01 00:00:00.000000 pipen_board-0.2.9/setup.py
--rw-r--r--   0        0        0     6917 1970-01-01 00:00:00.000000 pipen_board-0.2.9/PKG-INFO
+-rw-r--r--   0        0        0     6141 2023-06-01 08:43:44.593572 pipen_board-0.3.0/README.md
+-rw-r--r--   0        0        0      268 2023-06-01 08:43:44.593572 pipen_board-0.3.0/pipen_board/__init__.py
+-rw-r--r--   0        0        0     8985 2023-06-01 08:43:44.593572 pipen_board-0.3.0/pipen_board/apis.py
+-rw-r--r--   0        0        0     4367 2023-06-01 08:43:44.593572 pipen_board-0.3.0/pipen_board/cli.py
+-rw-r--r--   0        0        0    26496 2023-06-01 08:43:44.593572 pipen_board-0.3.0/pipen_board/data_manager.py
+-rw-r--r--   0        0        0     6243 2023-06-01 08:43:44.593572 pipen_board-0.3.0/pipen_board/defaults.py
+-rw-r--r--   0        0        0    23628 2023-06-01 08:43:44.593572 pipen_board-0.3.0/pipen_board/frontend/build/assets/favicon.png
+-rw-r--r--   0        0        0   624476 2023-06-01 08:43:44.597572 pipen_board-0.3.0/pipen_board/frontend/build/assets/index.css
+-rw-r--r--   0        0        0   738678 2023-06-01 08:43:44.601573 pipen_board-0.3.0/pipen_board/frontend/build/assets/index.js
+-rw-r--r--   0        0        0     4128 2023-06-01 08:43:44.601573 pipen_board-0.3.0/pipen_board/frontend/build/assets/schema.json
+-rw-r--r--   0        0        0      406 2023-06-01 08:43:44.601573 pipen_board-0.3.0/pipen_board/frontend/build/index.html
+-rw-r--r--   0        0        0     7562 2023-06-01 08:43:44.605573 pipen_board-0.3.0/pipen_board/plugin.py
+-rw-r--r--   0        0        0     3974 2023-06-01 08:43:44.605573 pipen_board-0.3.0/pipen_board/quart_app.py
+-rw-r--r--   0        0        0       22 2023-06-01 08:43:44.605573 pipen_board-0.3.0/pipen_board/version.py
+-rw-r--r--   0        0        0      731 2023-06-01 08:43:44.605573 pipen_board-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     7284 1970-01-01 00:00:00.000000 pipen_board-0.3.0/setup.py
+-rw-r--r--   0        0        0     6917 1970-01-01 00:00:00.000000 pipen_board-0.3.0/PKG-INFO
```

### Comparing `pipen_board-0.2.9/README.md` & `pipen_board-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pipen_board-0.2.9/pipen_board/apis.py` & `pipen_board-0.3.0/pipen_board/apis.py`

 * *Files identical despite different names*

### Comparing `pipen_board-0.2.9/pipen_board/cli.py` & `pipen_board-0.3.0/pipen_board/cli.py`

 * *Files identical despite different names*

### Comparing `pipen_board-0.2.9/pipen_board/data_manager.py` & `pipen_board-0.3.0/pipen_board/data_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,15 +106,15 @@
         return {}
 
     argspec = {}
     # arginfo: attrs, help, terms
     for arg, arginfo in anno.items():
         argspec[arg] = arginfo.attrs.copy()
         argspec[arg]["desc"] = re.sub(
-            r"([\.\?!])\s*\n",
+            r"([\.\?!:])\s*\n",
             "\\1<br />\n",
             arginfo.help,
         )
         if arg.startswith("<") and arg.endswith(">"):
             argspec[arg].setdefault("order", 999)
         if "btype" not in argspec[arg]:
             if argspec[arg].get("action") in ("store_true", "store_false"):
@@ -150,15 +150,15 @@
                 if not term.help
                 else term.help.splitlines()[0]
                 for term in arginfo.terms.values()
             ]
             argspec[arg]["desc"] += "\n"
             # Add the choices to the description
             for termname, term in arginfo.terms.items():
-                h = re.sub(r"([\.\?!])\s*\n", "\\1<br />\n", term.help)
+                h = re.sub(r"([\.\?!:])\s*\n", "\\1<br />\n", term.help)
                 argspec[arg]["desc"] += f"- `{termname}`: {h}\n"
         else:
             argspec[arg]["value"] = argspec[arg].pop("default", None)
 
         # determine the itype for list elements
         if t == "list":
             if argspec[arg]["value"] is not None and not isinstance(
@@ -431,15 +431,15 @@
         """
         if configfile:
             with PIPEN_BOARD_DIR.joinpath(configfile).open() as f:
                 self._config_data = json.load(f)
                 return
 
         if (
-            use_cached is True or (use_cached == "auto" and args.dev)
+            use_cached is True or (use_cached == "auto" and not args.dev)
         ) and self._config_data:
             return
 
         # Use multiprocessing to get a clean environment
         # to load the pipeline to avoid conflicts
         def target(conn):
             conn.send(json.dumps(asyncio.run(_get_config_data(args))).encode())
@@ -690,38 +690,41 @@
 
     async def on_job_succeeded(self, data, ws):
         await self._on_job(data, "succeeded", ws)
 
     async def on_job_cached(self, data, ws):
         await self._on_job(data, "succeeded", ws)
 
-    async def run_pipeline(self, command, port):
+    async def run_pipeline(self, command, port, ws_clients):
         """Run a command and send the output to the websocket"""
         self.clear_run_data()
         self._run_data[SECTION_LOG] = self._run_data[SECTION_LOG] or ""
 
         p = await asyncio.create_subprocess_shell(
             command,
             stdin=asyncio.subprocess.PIPE,
             stdout=asyncio.subprocess.PIPE,
             stderr=asyncio.subprocess.STDOUT,
         )
         p.stdin.write(f"pipen-board:{port}\n".encode())
+        p.stdin.close()
         self.running = p.pid
         self._command = command
 
-        async def read_stream(stream):
-            while True:
-                line = await stream.readline()
-                if not line:
-                    break
-                self._run_data[SECTION_LOG] += line.decode()
+        while True:
+            line = await p.stdout.readline()
+            if not line:
+                break
+            self._run_data[SECTION_LOG] += line.decode()
 
-        await asyncio.create_task(read_stream(p.stdout))
         await p.wait()
+        # In case the pipeline fails to start
+        self._run_data["FINISHED"] = True
+        self.running = False
+        await self.send_run_data(ws_clients.get("web"), force=True)
 
     async def stop_pipeline(self):
         """Stop the pipeline"""
         if not self.running:
             return {"ok": False, "msg": "Pipeline is not running"}
 
         logger.debug(
```

### Comparing `pipen_board-0.2.9/pipen_board/defaults.py` & `pipen_board-0.3.0/pipen_board/defaults.py`

 * *Files identical despite different names*

### Comparing `pipen_board-0.2.9/pipen_board/frontend/build/assets/favicon.png` & `pipen_board-0.3.0/pipen_board/frontend/build/assets/favicon.png`

 * *Files identical despite different names*

### Comparing `pipen_board-0.2.9/pipen_board/frontend/build/assets/index.css` & `pipen_board-0.3.0/pipen_board/frontend/build/assets/index.css`

 * *Files identical despite different names*

### Comparing `pipen_board-0.2.9/pipen_board/frontend/build/assets/index.js` & `pipen_board-0.3.0/pipen_board/frontend/build/assets/index.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -16125,15 +16125,15 @@
         u = {};
     for (let c = 0; c < a.length; c += 1) u = assign(u, a[c]);
     return {
         c() {
             e = element("button"), n = element("span"), r = text(t[1]), attr(n, "class", "svelte-1839e8i"), set_attributes(e, u), toggle_class(e, "svelte-1839e8i", !0)
         },
         m(c, _) {
-            insert(c, e, _), append(e, n), append(n, r), e.autofocus && e.focus(), s || (o = listen(e, "click", t[8]), s = !0)
+            insert(c, e, _), append(e, n), append(n, r), e.autofocus && e.focus(), s || (o = listen(e, "click", t[9]), s = !0)
         },
         p(c, [_]) {
             _ & 2 && set_data(r, c[1]), set_attributes(e, u = get_spread_update(a, [_ & 128 && c[7], _ & 252 && l !== (l = "navitem " + (c[4] ? "hidden" : "") + " " + (c[6] ? "active" : "") + " " + (c[2] ? "sub" : "") + " " + (c[5] ? "errored" : "") + " " + (c[3] ? "start-proc" : "") + " " + (c[7].class ? c[7].class : "")) && {
                 class: l
             }])), toggle_class(e, "svelte-1839e8i", !0)
         },
         i: noop,
@@ -16142,15 +16142,15 @@
             c && detach(e), s = !1, o()
         }
     }
 }
 
 function instance$Z(t, e, n) {
     let r;
-    const l = ["text", "activeNavItem", "sub", "is_start", "hidden"];
+    const l = ["text", "activeNavItem", "sub", "is_start", "hidden", "noerror"];
     let s = compute_rest_props(e, l),
         {
             text: o
         } = e,
         {
             activeNavItem: a
         } = e,
@@ -16159,35 +16159,39 @@
         } = e,
         {
             is_start: c = !1
         } = e,
         {
             hidden: _ = !1
         } = e,
-        d = !1;
-    storedErrors.subscribe(h => {
-        n(5, d = Object.keys(h).map(m => m.split(" / ")[0]).includes(o))
+        {
+            noerror: d = !1
+        } = e,
+        p = !1;
+    d || storedErrors.subscribe(m => {
+        n(5, p = Object.keys(m).map(g => g.split(" / ")[0]).includes(o))
     });
-    const p = () => {
+    const h = () => {
         n(0, a = o)
     };
-    return t.$$set = h => {
-        e = assign(assign({}, e), exclude_internal_props(h)), n(7, s = compute_rest_props(e, l)), "text" in h && n(1, o = h.text), "activeNavItem" in h && n(0, a = h.activeNavItem), "sub" in h && n(2, u = h.sub), "is_start" in h && n(3, c = h.is_start), "hidden" in h && n(4, _ = h.hidden)
+    return t.$$set = m => {
+        e = assign(assign({}, e), exclude_internal_props(m)), n(7, s = compute_rest_props(e, l)), "text" in m && n(1, o = m.text), "activeNavItem" in m && n(0, a = m.activeNavItem), "sub" in m && n(2, u = m.sub), "is_start" in m && n(3, c = m.is_start), "hidden" in m && n(4, _ = m.hidden), "noerror" in m && n(8, d = m.noerror)
     }, t.$$.update = () => {
         t.$$.dirty & 3 && n(6, r = o === a)
-    }, [a, o, u, c, _, d, r, s, p]
+    }, [a, o, u, c, _, p, r, s, d, h]
 }
 class NavItem extends SvelteComponent {
     constructor(e) {
         super(), init(this, e, instance$Z, create_fragment$Z, safe_not_equal, {
             text: 1,
             activeNavItem: 0,
             sub: 2,
             is_start: 3,
-            hidden: 4
+            hidden: 4,
+            noerror: 8
         })
     }
 }
 const NavDivider_svelte_svelte_type_style_lang = "";
 
 function create_else_block$i(t) {
     let e, n, r, l, s;
@@ -25916,17 +25920,17 @@
                     },
                     body: JSON.stringify({
                         command: m,
                         config: stringify(finalizeConfig(o)),
                         overwriteConfig: y,
                         tomlfile: r
                     })
-                }, "response");
+                });
                 if (x.ok) n(15, _ = _ + 1);
-                else throw x.status === 409 ? new Error(`Failed to run command: ${r} exists.`) : x.status === 410 ? new Error(`Failed to run command: Failed to save config to ${r}.`) : new Error(`Failed to run command: ${x.status} ${x.statusText}`)
+                else throw new Error(`Failed to run command: ${x.msg}`)
             } catch (x) {
                 n(7, g.kind = "error", g), n(7, g.subtitle = x, g), n(7, g.timeout = 0, g);
                 return
             } finally {
                 n(8, b = !1)
             }
         }, O = () => {
@@ -30937,15 +30941,16 @@
 function create_if_block_14(t) {
     let e, n, r;
 
     function l(o) {
         t[12](o)
     }
     let s = {
-        text: "Log"
+        text: "Log",
+        noerror: !0
     };
     return t[4] !== void 0 && (s.activeNavItem = t[4]), e = new NavItem({
         props: s
     }), binding_callbacks.push(() => bind(e, "activeNavItem", l)), {
         c() {
             create_component(e.$$.fragment)
         },
@@ -30971,15 +30976,16 @@
 function create_if_block_13(t) {
     let e, n, r;
 
     function l(o) {
         t[13](o)
     }
     let s = {
-        text: "Diagram"
+        text: "Diagram",
+        noerror: !0
     };
     return t[4] !== void 0 && (s.activeNavItem = t[4]), e = new NavItem({
         props: s
     }), binding_callbacks.push(() => bind(e, "activeNavItem", l)), {
         c() {
             create_component(e.$$.fragment)
         },
@@ -31005,15 +31011,16 @@
 function create_if_block_12(t) {
     let e, n, r;
 
     function l(o) {
         t[14](o)
     }
     let s = {
-        text: "Reports"
+        text: "Reports",
+        noerror: !0
     };
     return t[4] !== void 0 && (s.activeNavItem = t[4]), e = new NavItem({
         props: s
     }), binding_callbacks.push(() => bind(e, "activeNavItem", l)), {
         c() {
             create_component(e.$$.fragment)
         },
@@ -31094,14 +31101,15 @@
     let e, n, r;
 
     function l(o) {
         t[16](o)
     }
     let s = {
         class: "run-status-" + t[0][SECTION_PROCESSES][t[27]].status,
+        noerror: !0,
         text: t[27],
         sub: !0
     };
     return t[4] !== void 0 && (s.activeNavItem = t[4]), e = new NavItem({
         props: s
     }), binding_callbacks.push(() => bind(e, "activeNavItem", l)), {
         c() {
@@ -31175,14 +31183,15 @@
     let e, n, r;
 
     function l(o) {
         t[18](o)
     }
     let s = {
         class: "run-status-" + t[0][SECTION_PROCGROUPS][t[22]][t[27]].status,
+        noerror: !0,
         sub: !0,
         text: t[27]
     };
     return t[4] !== void 0 && (s.activeNavItem = t[4]), e = new NavItem({
         props: s
     }), binding_callbacks.push(() => bind(e, "activeNavItem", l)), {
         c() {
```

### Comparing `pipen_board-0.2.9/pipen_board/frontend/build/assets/schema.json` & `pipen_board-0.3.0/pipen_board/frontend/build/assets/schema.json`

 * *Files identical despite different names*

### Comparing `pipen_board-0.2.9/pipen_board/plugin.py` & `pipen_board-0.3.0/pipen_board/plugin.py`

 * *Files identical despite different names*

### Comparing `pipen_board-0.2.9/pipen_board/quart_app.py` & `pipen_board-0.3.0/pipen_board/quart_app.py`

 * *Files 13% similar despite different names*

```diff
@@ -81,39 +81,60 @@
         data = await request.get_json()
 
         command = data["command"]
         overwriteConfig = data["overwriteConfig"]
         config = data["config"]
         tomlfile = Path(data["tomlfile"])
         if not overwriteConfig and tomlfile.exists():
-            return {}, 409
+            return {
+                "ok": False,
+                "msg": (
+                    "Config file already exists. "
+                    "Check the box to overwrite it, "
+                    "or use a different configuration file name."
+                )
+            }
         try:
             tomlfile.write_text(config)
-        except Exception:
-            return {}, 410
+        except Exception as ex:
+            return {
+                "ok": False,
+                "msg": f"Failed to write the configuration file: {ex}"
+            }
+
+        if data_manager.running:
+            return {
+                "ok": False,
+                "msg": (
+                    "Pipeline is already running. "
+                    "Please wait for it to finish, or stop it first."
+                )
+            }
 
         logger.info(
             f"[bold][yellow]API[/yellow][/bold] Running pipeline: {command}"
         )
         # Run command at background
         app.add_background_task(
             data_manager.run_pipeline,
             command,
             args.port,
+            clients,
         )
-        return {"ok": True}
+        return {"ok": True, "msg": ""}
 
     @app.route("/api/pipeline/rerun", methods=["POST"])
     async def rerun():
         logger.info(
             f"[bold][yellow]API[/yellow][/bold] Re-Running pipeline: %s",
             data_manager._command,
         )
         # Run command at background
         app.add_background_task(
             data_manager.run_pipeline,
             data_manager._command,
             args.port,
+            clients,
         )
         return {"ok": True}
 
     return app
```

### Comparing `pipen_board-0.2.9/pyproject.toml` & `pipen_board-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pipen-board"
-version = "0.2.9"
+version = "0.3.0"
 description = "Visualization configuration and running of pipen pipelines on the web"
 authors = ["pwwang <pwwang@pwwang.com>"]
 license = "MIT"
 readme = "README.md"
 exclude = ["pipen_board/frontend/[!build]*", "pipen_board/frontend/index.html"]
 
 [tool.poetry.build]
```

### Comparing `pipen_board-0.2.9/setup.py` & `pipen_board-0.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 entry_points = \
 {'pipen': ['board = pipen_board:pipen_board_plugin'],
  'pipen_cli': ['cli-board = pipen_board:PipenCliBoardPlugin']}
 
 setup_kwargs = {
     'name': 'pipen-board',
-    'version': '0.2.9',
+    'version': '0.3.0',
     'description': 'Visualization configuration and running of pipen pipelines on the web',
     'long_description': '# pipen-board\n\nVisualize configuration and running of [pipen][1] pipelines on the web.\n\n## Installation\n\n```bash\npip install pipen-board\n```\n\n## Usage\n\n```bash\n$ pipen board --help\nUsage: pipen board [options] <pipeline> -- [pipeline options]\n\nVisualize configuration and running of pipen pipelines on the web\n\nRequired Arguments:\n  pipeline              The pipeline and the CLI arguments to run the pipeline. For the\n                        pipeline either `/path/to/pipeline.py:<pipeline>` or\n                        `<module.submodule>:<pipeline>` `<pipeline>` must be an instance of\n                        `Pipen` and running the pipeline should be called under `__name__ ==\n                        \'__main__\'.\n\nOptions:\n  -h, --help            show help message and exit\n  --port PORT           Port to serve the UI wizard [default: 18521]\n  --name NAME           The name of the pipeline. Default to the pipeline class name. You\n                        can use a different name to associate with a different set of\n                        configurations.\n  --additional FILE     Additional arguments for the pipeline, in YAML, INI, JSON or TOML\n                        format. Can have sections `ADDITIONAL_OPTIONS` and `RUNNING_OPTIONS`\n  --dev                 Run the pipeline in development mode. This will print verbosal\n                        logging information and reload the pipeline if a new instantce\n                        starts when page reloads.\n  --root ROOT           The root directory of the pipeline. [default: .]\n  --loglevel {auto,debug,info,warning,error,critical}\n                        Logging level. If `auto`, set to `debug` if `--dev` is set,\n                        otherwise `info` [default: auto]\n```\n\n## Describing arguments in docstring\n\n### Docstring schema\n\n```python\nclass ProcessOrProcessGroup:\n    """Short summary\n\n    Long description\n    Long description\n\n    Args:\n        arg1 (<metadata>): description\n            - subarg1 (<metadata>): description\n            - subarg2 (<metadata>): description\n        arg2 (<metadata>): description\n\n    <Other Sections>:\n        <content>\n    """\n```\n\nThe metadata can have multiple attributes, separated by semicolon (`;`). For example:\n\n```\narg1 (action=ns;required): description\n```\n\n### Marks\n\nYou can mark a process using `pipen.utils.mark(<mark>=<value>)` as a decorator to decorate a process. For example:\n\n```python\nfrom pipen import Proc\nfrom pipen.utils import mark\n\n@mark(board_config_no_input=True)\nclass MyProc(Proc):\n    pass\n```\n\nAvailable marks:\n\n- `board_config_no_input`: Whether to show the input section for the process in configuation page. Only affects the start processes. Default to `False`.\n- `board_config_hidden`: Whether to hide the process options in the configuration page. Note that the process is still visible in the process list. Default to `False`.\n\n### Metadata for arguments\n\n\n| Name     | Description | Allowed values |\n| -------- | ----------- | -------------- |\n| `action` | Like the `action` argument in [`argx`][2]*. | `store_true`, `store_false`, `ns`, `namespace`, `append`, `extend`, `clear_append`, `clear_extend` (other values are allowed but ignore, they may be effective for CLI use) |\n| `btype`  | Board type (option type specified directly). If specified, `action` will be ignored | `ns`, `choice`, `mchoice`, `array`, `list`, `json`, `int`, `float`, `bool`, `str`, `text`, `auto`* |\n| `type` | Fallback for `action` and `btype` | Same as `btype` |\n| `ns`/`namespace` | Shortcut for `btype=ns` | No values needed |\n| `choices`/`choice` | Shortcut for `btype=choice` | No values needed |\n| `mchoices`/`mchoice` | Shortcut for `btype=mchoice` | No values needed |\n| `array`/`list` | Shortcut for `btype=array`/`btype=list` | No values needed |\n| `choices`/`choice` | Shortcut for `btype=choice` | No values needed |\n| `mchoices`/`mchoice` | Shortcut for `btype=mchoice` | No values needed |\n| `order` | The order of the argument in the UI. | Any integer |\n| `readonly` | Whether the argument is readonly. | No values needed (True if specified, otherwise False) |\n| `required` | Whether the argument is required. | No values needed (True if specified, otherwise False) |\n| `placeholder` | The placeholder in the UI for the argument. | Any string |\n| `bitype` | The type of the elements in an array or list. | `int`, `float`, `bool`, `str`, `json`, `auto`* |\n| `itype` | Fallback for `bitype` | Same as `bitype` |\n\n- `argx*`: An argument parser for Python, compatible with `argparse`.\n- `auto*`: Automatically infer the type from a string value.\n  - Any of `True`, `TRUE`, `true`, `False`, `FALSE`, `false` will be inferred as a `bool` value.\n  - Any of `None`, `NONE`, `none`, `null`, `NULL` will be inferred as `None`.\n  - Any integers will be inferred as `int`.\n  - Any floats will be inferred as `float`.\n  - Try to parse the value as JSON. If succeed, the value will be inferred as `json`.\n  - Otherwise, the value will be inferred as `str`.\n\n### Types of options in the UI\n\nThe type of an option in the UI is determined by the `btype`, `action` or `type` metadata. If neither is specified, a `PlainText` will be used.\n\n- `BoolOption`: Shown as a switch\n- `TextOption`: Shown as a textarea (allow multiple lines)\n- `ChoiceOption`: Shown as a dropdown list (`subarg1` and `subarg2` in the example above are used as the choices)\n- `MChoiceOption`: Shown as a multiple choice list (`subarg1` and `subarg2` in the example above are used as the choices)\n- `JsonOption`: Shown as a textarea, but the value will be validated and parsed as JSON\n- `ArrayOption`: Shown as a tag input. Items can be added or removed.\n- `AutoOption`: Shown as a 1-row textarea, and the value will be parsed automatically\n- `PlainText`: Shown as a plain text. No validation or parsing will be performed.\n- `MoreLikeOption`: Show as a box with buttons to add or remove sub-options. It\'s usally used together with `ns` type. If there is a sub-option under the option in the docstring wrapped by `<...>`, it indicates that we may have more sub-options.\n\n\n[1]: https://github.com/pwwang/pipen\n[2]: https://github.com/pwwang/argx\n',
     'author': 'pwwang',
     'author_email': 'pwwang@pwwang.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `pipen_board-0.2.9/PKG-INFO` & `pipen_board-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipen-board
-Version: 0.2.9
+Version: 0.3.0
 Summary: Visualization configuration and running of pipen pipelines on the web
 License: MIT
 Author: pwwang
 Author-email: pwwang@pwwang.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

