# Comparing `tmp/tawazi-0.2.0.tar.gz` & `tmp/tawazi-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tawazi-0.2.0.tar", max compression
+gzip compressed data, was "tawazi-0.3.0.tar", last modified: Thu Jun  1 08:00:33 2023, max compression
```

## Comparing `tawazi-0.2.0.tar` & `tawazi-0.3.0.tar`

### file list

```diff
@@ -1,11 +1,83 @@
--rw-r--r--   0        0        0    11336 2022-06-08 12:47:16.124172 tawazi-0.2.0/LICENSE
--rw-r--r--   0        0        0     4485 2022-10-18 09:25:43.843660 tawazi-0.2.0/README.md
--rw-r--r--   0        0        0     1424 2022-10-18 11:16:41.066125 tawazi-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      397 2022-10-18 11:16:41.066125 tawazi-0.2.0/tawazi/__init__.py
--rw-r--r--   0        0        0      314 2022-10-14 13:28:53.408087 tawazi-0.2.0/tawazi/config.py
--rw-r--r--   0        0        0    18586 2022-10-14 16:02:18.235707 tawazi-0.2.0/tawazi/dag.py
--rw-r--r--   0        0        0      273 2022-10-13 14:23:56.697735 tawazi-0.2.0/tawazi/errors.py
--rw-r--r--   0        0        0     8434 2022-10-17 10:32:16.357687 tawazi-0.2.0/tawazi/node.py
--rw-r--r--   0        0        0     3720 2022-10-17 10:32:16.357687 tawazi-0.2.0/tawazi/ops.py
--rw-r--r--   0        0        0     5520 2022-10-18 12:12:57.452842 tawazi-0.2.0/setup.py
--rw-r--r--   0        0        0     5297 2022-10-18 12:12:57.453199 tawazi-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       74 2023-03-10 19:29:40.629046 tawazi-0.3.0/.bandit
+-rw-r--r--   0        0        0       58 2022-09-09 17:49:07.274039 tawazi-0.3.0/.flake8
+-rw-r--r--   0        0        0      655 2023-03-10 19:29:40.629046 tawazi-0.3.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      567 2023-03-10 19:29:40.629046 tawazi-0.3.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1216 2023-03-10 19:29:40.633046 tawazi-0.3.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      529 2022-09-02 12:29:48.007747 tawazi-0.3.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      625 2023-05-30 16:13:24.605608 tawazi-0.3.0/.github/workflows/documentation-validation-workflow.yml
+-rw-r--r--   0        0        0      686 2023-03-10 19:29:40.633046 tawazi-0.3.0/.github/workflows/formatting-workflow.yml
+-rw-r--r--   0        0        0     1522 2023-03-28 14:35:03.514988 tawazi-0.3.0/.github/workflows/testing-workflow.yml
+-rw-r--r--   0        0        0     1834 2023-03-10 19:29:40.633046 tawazi-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1032 2023-05-23 11:46:23.707166 tawazi-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     3889 2023-06-01 07:58:52.768041 tawazi-0.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0     5220 2022-09-09 17:49:07.274039 tawazi-0.3.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     2376 2022-09-09 17:49:07.274039 tawazi-0.3.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0    11336 2022-06-08 12:47:16.124172 tawazi-0.3.0/LICENSE
+-rw-r--r--   0        0        0     4294 2023-05-24 15:05:58.301886 tawazi-0.3.0/README.md
+-rw-r--r--   0        0        0       54 2023-03-10 19:29:40.633046 tawazi-0.3.0/codecov.yml
+-rw-r--r--   0        0        0      163 2023-05-24 15:53:47.635584 tawazi-0.3.0/documentation/DAGExecution.md
+-rw-r--r--   0        0        0      268 2023-05-24 15:53:47.635584 tawazi-0.3.0/documentation/dag.md
+-rw-r--r--   0        0        0       78 2023-05-24 15:53:47.635584 tawazi-0.3.0/documentation/decorators.md
+-rw-r--r--   0        0        0     2630 2023-03-28 14:31:27.414878 tawazi-0.3.0/documentation/future_developments.md
+-rw-r--r--   0        0        0    21196 2023-05-31 15:06:23.150540 tawazi-0.3.0/documentation/index.md
+-rw-r--r--   0        0        0      323 2023-05-30 16:13:24.605608 tawazi-0.3.0/documentation/nodes.md
+-rw-r--r--   0        0        0      179 2023-05-31 15:06:23.150540 tawazi-0.3.0/documentation/others.md
+-rw-r--r--   0        0        0    86587 2023-03-10 18:51:45.700072 tawazi-0.3.0/documentation/tawazi_GIF.gif
+-rw-r--r--   0        0        0     1733 2023-03-10 19:29:40.633046 tawazi-0.3.0/example.py
+-rw-r--r--   0        0        0     1074 2023-05-31 15:06:23.150540 tawazi-0.3.0/mkdocs.yml
+-rw-r--r--   0        0        0     1972 2023-06-01 07:58:52.768041 tawazi-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      509 2023-06-01 07:58:52.768041 tawazi-0.3.0/tawazi/__init__.py
+-rw-r--r--   0        0        0       70 2023-05-30 15:35:12.327370 tawazi-0.3.0/tawazi/_dag/__init__.py
+-rw-r--r--   0        0        0    46163 2023-05-30 16:13:24.605608 tawazi-0.3.0/tawazi/_dag/dag.py
+-rw-r--r--   0        0        0     5943 2023-05-31 15:06:23.150540 tawazi-0.3.0/tawazi/_dag/digraph.py
+-rw-r--r--   0        0        0    10561 2023-05-31 15:06:23.150540 tawazi-0.3.0/tawazi/_dag/helpers.py
+-rw-r--r--   0        0        0     9781 2023-05-31 15:06:23.150540 tawazi-0.3.0/tawazi/_decorators.py
+-rw-r--r--   0        0        0     3122 2023-05-30 16:13:24.609608 tawazi-0.3.0/tawazi/_helpers.py
+-rw-r--r--   0        0        0      487 2023-05-24 15:05:58.305886 tawazi-0.3.0/tawazi/_object_helpers.py
+-rw-r--r--   0        0        0     2483 2023-05-31 15:06:23.150540 tawazi-0.3.0/tawazi/config.py
+-rw-r--r--   0        0        0     3963 2023-05-31 15:06:23.150540 tawazi-0.3.0/tawazi/consts.py
+-rw-r--r--   0        0        0     1862 2023-05-30 16:13:24.609608 tawazi-0.3.0/tawazi/errors.py
+-rw-r--r--   0        0        0      316 2023-05-24 16:00:12.734872 tawazi-0.3.0/tawazi/node/__init__.py
+-rw-r--r--   0        0        0     2866 2023-05-24 16:00:12.734872 tawazi-0.3.0/tawazi/node/functions.py
+-rw-r--r--   0        0        0      994 2023-05-24 16:00:12.734872 tawazi-0.3.0/tawazi/node/helpers.py
+-rw-r--r--   0        0        0    33386 2023-05-31 15:06:23.150540 tawazi-0.3.0/tawazi/node/node.py
+-rw-r--r--   0        0        0     3362 2023-05-30 16:13:24.609608 tawazi-0.3.0/tawazi/profile.py
+-rw-r--r--   0        0        0        0 2023-03-14 13:47:29.118468 tawazi-0.3.0/tawazi/py.typed
+-rw-r--r--   0        0        0       68 2023-03-10 19:29:40.641045 tawazi-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0     3751 2023-04-12 15:30:48.423260 tawazi-0.3.0/tests/test_active.py
+-rw-r--r--   0        0        0     2641 2023-05-31 15:06:23.150540 tawazi-0.3.0/tests/test_behavior.py
+-rw-r--r--   0        0        0     2292 2023-05-30 09:51:14.013295 tawazi-0.3.0/tests/test_build.py
+-rw-r--r--   0        0        0     7666 2023-05-24 14:25:42.922948 tawazi-0.3.0/tests/test_cache_feature.py
+-rw-r--r--   0        0        0     1425 2023-04-12 15:30:48.423260 tawazi-0.3.0/tests/test_compound_priority.py
+-rw-r--r--   0        0        0     4288 2023-05-31 15:06:23.150540 tawazi-0.3.0/tests/test_config.py
+-rw-r--r--   0        0        0     5337 2023-05-11 14:42:39.170761 tawazi-0.3.0/tests/test_dag_compose.py
+-rw-r--r--   0        0        0     1740 2023-03-10 19:29:40.641045 tawazi-0.3.0/tests/test_dag_config.py
+-rw-r--r--   0        0        0     2883 2023-05-24 18:48:26.478266 tawazi-0.3.0/tests/test_dagexecutor.py
+-rw-r--r--   0        0        0     4022 2023-05-30 16:13:24.609608 tawazi-0.3.0/tests/test_debug_nodes.py
+-rw-r--r--   0        0        0      730 2023-03-10 19:29:40.641045 tawazi-0.3.0/tests/test_decorator.py
+-rw-r--r--   0        0        0     1325 2023-05-30 09:51:14.013295 tawazi-0.3.0/tests/test_edge_cases_dag.py
+-rw-r--r--   0        0        0      362 2023-05-24 14:25:42.922948 tawazi-0.3.0/tests/test_error_during_dag_build.py
+-rw-r--r--   0        0        0     4079 2023-05-30 16:13:24.609608 tawazi-0.3.0/tests/test_exclude_nodes.py
+-rw-r--r--   0        0        0      422 2023-03-10 19:29:40.641045 tawazi-0.3.0/tests/test_execution_time.py
+-rw-r--r--   0        0        0     1318 2023-05-24 14:25:42.922948 tawazi-0.3.0/tests/test_graph.py
+-rw-r--r--   0        0        0      610 2023-03-10 19:29:40.641045 tawazi-0.3.0/tests/test_imbricated_dags.py
+-rw-r--r--   0        0        0     2262 2023-04-12 15:30:48.423260 tawazi-0.3.0/tests/test_methods.py
+-rw-r--r--   0        0        0     5791 2023-05-22 15:30:39.805326 tawazi-0.3.0/tests/test_multiple_return_value_for_exec_node.py
+-rw-r--r--   0        0        0     2446 2023-04-12 15:30:48.423260 tawazi-0.3.0/tests/test_multiple_return_value_for_graph.py
+-rw-r--r--   0        0        0      413 2023-03-10 19:29:40.641045 tawazi-0.3.0/tests/test_non_picklable_arguments.py
+-rw-r--r--   0        0        0     2299 2023-05-31 13:03:56.304999 tawazi-0.3.0/tests/test_op.py
+-rw-r--r--   0        0        0    18550 2023-04-12 15:30:48.423260 tawazi-0.3.0/tests/test_operators.py
+-rw-r--r--   0        0        0     2609 2023-04-12 15:30:48.423260 tawazi-0.3.0/tests/test_ops_interface.py
+-rw-r--r--   0        0        0     1410 2023-05-30 16:13:24.609608 tawazi-0.3.0/tests/test_pipeline_input_output.py
+-rw-r--r--   0        0        0     3388 2023-05-24 14:25:42.922948 tawazi-0.3.0/tests/test_priority_sequential.py
+-rw-r--r--   0        0        0     2801 2023-05-24 14:25:42.922948 tawazi-0.3.0/tests/test_profiling.py
+-rw-r--r--   0        0        0     1508 2023-05-31 15:06:23.150540 tawazi-0.3.0/tests/test_resource.py
+-rw-r--r--   0        0        0     2899 2023-04-12 15:30:48.423260 tawazi-0.3.0/tests/test_safe_execution.py
+-rw-r--r--   0        0        0      279 2023-03-10 19:29:40.645045 tawazi-0.3.0/tests/test_same_op_reuse.py
+-rw-r--r--   0        0        0    10318 2023-05-30 16:13:24.609608 tawazi-0.3.0/tests/test_setup_nodes.py
+-rw-r--r--   0        0        0     3592 2023-05-30 09:51:09.709460 tawazi-0.3.0/tests/test_subgraph.py
+-rw-r--r--   0        0        0      909 2023-04-12 15:30:48.423260 tawazi-0.3.0/tests/test_tags.py
+-rw-r--r--   0        0        0     1841 2023-05-30 16:13:24.609608 tawazi-0.3.0/tests/test_typing.py
+-rw-r--r--   0        0        0      776 2023-03-10 19:29:40.645045 tawazi-0.3.0/tests/test_wrapped_function.py
+-rw-r--r--   0        0        0        0 2023-03-10 18:51:45.704072 tawazi-0.3.0/tests/tests/__init__.py
+-rw-r--r--   0        0        0     5292 1970-01-01 00:00:00.000000 tawazi-0.3.0/PKG-INFO
```

### Comparing `tawazi-0.2.0/LICENSE` & `tawazi-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tawazi-0.2.0/README.md` & `tawazi-0.3.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,141 +1,135 @@
 # tawazi
-[![Python 3.7](https://img.shields.io/badge/python-3.7-blue.svg)](https://www.python.org/downloads/release/python-370/)
-[![Python 3.8](https://img.shields.io/badge/python-3.8-blue.svg)](https://www.python.org/downloads/release/python-380/)
-[![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-390/)
-[![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-3100/)
+<!--Python badges -->
+[![Python 3.7](https://img.shields.io/badge/python-3.7%20|%203.8%20|%203.9%20|%203.10%20|%203.11-blue.svg)](https://www.python.org/)
+[![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 [![CodeFactor](https://www.codefactor.io/repository/github/mindee/tawazi/badge)](https://www.codefactor.io/repository/github/mindee/tawazi)
+[![Downloads](https://img.shields.io/pypi/dm/tawazi)](https://pypi.org/project/tawazi/)
 
+<!--Tawazi Badge-->
 ![Tawazi GIF](documentation/tawazi_GIF.gif)
 
 ## Introduction
 
 <!-- TODO: put a link explaining what a DAG is-->
 
-The tawazi library enables **parallel** execution of functions in a [DAG](https://en.wikipedia.org/wiki/Directed_acyclic_graph) dependency structure.
-This library satisfies the following:
-* Stable, robust, well tested
-* lightweight
-* Thread Safety
-* Low to no dependencies
-* Legacy Python versions support (in the future)
-* pypy support (in the future)
+[Tawazi](https://pypi.org/project/tawazi/) facilitates **parallel** execution of functions using a [DAG](https://en.wikipedia.org/wiki/Directed_acyclic_graph) dependency structure.
 
-In the context of tawazi, the computation sequence to be run in parallel is referred to as DAG and the functions that must run in parallel are called `ExecNode`s.
+### Explanation
 
-This library supports:
-* Limitation of the number of "Threads"
-* Priority Choice of each `ExecNode`
-* Per `ExecNode` choice of parallelization (i.e. An `ExecNode` is allowed to run in parallel with other `ExecNode`s or not)
+Consider the function `f` that depends on the function `g` and `h`:
+```python
+def g():
+    print("g")
+    return "g"
+def h():
+    print("h")
+    return "h"
+def f(g_var, h_var):
+    print("received", g_var, h_var)
+    print("f")
+    return "f"
 
-**Note**: The library is still at an [advanced state of development](#future-developments). Your contributions are highly welcomed.
+def main():
+    f(g(), h())
 
+main()
+```
+The [DAG](https://en.wikipedia.org/wiki/Directed_acyclic_graph) described in `main` can be accelerated if `g` and `h` are executed in parallel. This is what [Tawazi](https://pypi.org/project/tawazi/) does by adding a decorator to the functions `g`, `h`, `f`, and `main`:
 
-## Usage
 ```python
+from tawazi import dag, xn
+@xn
+def g():
+    print("g")
+    return "g"
+@xn
+def h():
+    print("h")
+    return "h"
+@xn
+def f(g_var, h_var):
+    print("received", g_var, h_var)
+    print("f")
+    return "f"
+@dag(max_concurrency=2)
+def main():
+    f(g(), h())
 
-# type: ignore
+main()
+```
+The total execution time of `main()` is **1 second instead of 2** which proves that the `g` and `h` have run in parallel, you can measure the speed up in the previous code:
+```python
 from time import sleep, time
-from tawazi import op, to_dag
-
-@op
-def a():
-    print("Function 'a' is running", flush=True)
+from tawazi import dag, xn
+@xn
+def g():
     sleep(1)
-    return "A"
-
-@op
-def b():
-    print("Function 'b' is running", flush=True)
+    print("g")
+    return "g"
+@xn
+def h():
     sleep(1)
-    return "B"
-
-@op
-def c(a, b):
-    print("Function 'c' is running", flush=True)
-    print(f"Function 'c' received {a} from 'a' & {b} from 'b'", flush=True)
-    return f"{a} + {b} = C"
-
-@to_dag(max_concurrency=2)
-def deps_describer():
-  result_a = a()
-  result_b = b()
-  result_c = c(result_a, result_b)
-
-if __name__ == "__main__":
-
-  t0 = time()
-  # executing the dag takes a single line of code
-  deps_describer().execute()
-  execution_time = time() - t0
-  assert execution_time < 1.5
-  print(f"Graph execution took {execution_time:.2f} seconds")
-
+    print("h")
+    return "h"
+@xn
+def f(g_var, h_var):
+    print("received", g_var, h_var)
+    print("f")
+    return "f"
+
+@dag(max_concurrency=2)
+def main():
+    f(g(), h())
+
+start = time()
+main()
+end = time()
+print("time taken", end - start)
+# h
+# g
+# received g h
+# f
+# time taken 1.004307508468628
 ```
 
-## Advanced Usage
+### Features
 
-```python
+This library satisfies the following:
+* robust, well tested
+* lightweight
+* Thread Safe
+* Few dependencies
+* Legacy Python versions support (in the future)
+* MyPy compatible
+* Many Python implementations support (in the future)
 
-# type: ignore
-from time import sleep, time
-from tawazi import op, to_dag
+In [Tawazi](https://pypi.org/project/tawazi/), a computation sequence is referred to as `DAG`. The functions invoked inside the computation sequence are referred to as `ExecNode`s.
 
-@op
-def a():
-    print("Function 'a' is running", flush=True)
-    sleep(1)
-    return "A"
+Current features are:
+* Specifying the number of "Threads" that the `DAG` uses
+* setup `ExecNode`s: These nodes only run once per DAG instance
+* debug `ExecNode`s: These are nodes that run only if `RUN_DEBUG_NODES` environment variable is set
+* running a subgraph of the `DAG` instance
+* Excluding an `ExecNode` from running
+* caching the results of the execution of a `DAG` for faster subsequent execution
+* Priority Choice of each `ExecNode` for fine control of execution order
+* Per `ExecNode` choice of parallelization (i.e. An `ExecNode` is allowed to run in parallel with other `ExecNode`s or not)
+* and more!
 
-# optionally configure each op using the decorator:
-# is_sequential = True to prevent op from running in parallel with other ops
-# priority to choose the op in the next execution phase
-# argument_name to choose the name of the argument that will be used
-@op(is_sequential=True, priority=10, argument_name="arg_b")
-def b():
-    print("Function 'b' is running", flush=True)
-    sleep(1)
-    return "B"
+### Documentation
+You can find the documentation here: [Tawazi](https://mindee.github.io/tawazi/).
 
-@op
-def c(a, arg_b):
-    print("Function 'c' is running", flush=True)
-    print(f"Function 'c' received {a} from 'a' & {arg_b} from 'b'", flush=True)
-    return f"{a} + {arg_b} = C"
-
-# optionally customize the DAG
-@to_dag(max_concurrency=2, behavior="strict")
-def deps_describer():
-  result_a = a()
-  result_b = b()
-  result_c = c(result_a, result_b)
-
-if __name__ == "__main__":
-
-  t0 = time()
-  # the dag instance is reusable.
-  # This is recommended if you want to do the same computation multiple times
-  dag = deps_describer()
-  results_1 = dag.execute()
-  execution_time = time() - t0
-  print(f"Graph execution took {execution_time:.2f} seconds")
-
-  # debugging the code using `dag.safe_execute()` is easier
-  # because the execution doesn't go through the Thread pool
-  results_2 = dag.safe_execute()
-
-  # you can look throught the results of each operation like this:
-  for my_op in [a, b, c]:
-    assert results_1[my_op.id].result == results_2[my_op.id].result
-
-```
+In [this blog](https://blog.mindee.com/directed-acyclic-graph-dag-scheduler-library/) we also talk about the purpose of using `Tawazi` in more detail.
 
+**Note**: The library is still at an [advanced state of development](#future-developments). Breaking changes might happen on the minor version (v0.Minor.Patch). Please pin [Tawazi](https://pypi.org/project/tawazi/) to the __Minor Version__. Your contributions are highly welcomed.
 
 ## Name explanation
 The libraries name is inspired from the arabic word تَوَازٍ which means parallel.
 
 ## Building the doc
-The general documentation has no dedicated space at the moment and is being hosted offline (on your machine).
-Expect future developments on this side as well. To build it, simply run `mkdocs build` and `mkdocs serve` at the root of the repository.
+Only the latest version's documentation is hosted. 
+
+If you want to check the documentation of a previous version please checkout the corresponding release, install the required packages and run: `mkdocs serve`
 
 ## Future developments
-*This library is still in development. Breaking changes are expected.
+__This library is still in development. Breaking changes are expected.__
```

### Comparing `tawazi-0.2.0/tawazi/ops.py` & `tawazi-0.3.0/CHANGELOG.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,92 +1,76 @@
-import functools
-from typing import Any, Callable, Optional
+# Changelog
 
-from tawazi import DAG
-from tawazi.errors import ErrorStrategy
+## v0.3.0 (2023-05-31)
 
-from . import node
-from .config import Cfg
-from .node import LazyExecNode, exec_nodes_lock
-
-
-# TODO: modify is_sequential's default value according to the pre used default
-def op(
-    func: Optional[Callable[..., Any]] = None,
-    *,
-    priority: int = 0,
-    argument_name: Optional[str] = None,
-    is_sequential: bool = Cfg.TAWAZI_IS_SEQUENTIAL,
-) -> "LazyExecNode":
-    """
-    Decorate a function to make it an ExecNode. When the decorated function is called, you are actually calling
-    an ExecNode. This way we can record the dependencies in order to build the actual DAG.
-    Please check the example in the README for a guide to the usage.
-    Args:
-        func: a Callable that will be executed in the DAG
-        priority: priority of the execution with respect to other ExecNodes
-        argument_name: name of the argument used by other ExecNodes referring to the returned value.
-             Explanation:
-             This ExecNode will return a value.
-             This value will be used by other ExecNodes via their arguments.
-             The name of the argument to be used is specified by this value.
-        is_sequential: whether to allow the execution of this ExecNode with others or not
-
-    Returns:
-        LazyExecNode
-    """
-
-    def my_custom_op(_func: Callable[..., Any]) -> "LazyExecNode":
-        lazy_exec_node = LazyExecNode(_func, priority, argument_name, is_sequential)
-        functools.update_wrapper(lazy_exec_node, _func)
-        return lazy_exec_node
-
-    # case #1: arguments are provided to the decorator
-    if func is None:
-        return my_custom_op  # type: ignore
-    # case #2: no argument is provided to the decorator
-    else:
-        return my_custom_op(func)
-
-
-def to_dag(
-    declare_dag_function: Optional[Callable[..., Any]] = None,
-    *,
-    max_concurrency: int = 1,
-    behavior: ErrorStrategy = ErrorStrategy.strict,
-) -> Callable[..., Any]:
-    """
-    Transform the declared ops into a DAG that can be executed by tawazi.
-    The same DAG can be executed multiple times.
-    Note: to_dag is thread safe because it uses an internal lock.
-        If you need to construct lots of DAGs in multiple threads,
-        it is best to construct your dag once and then consume it as much as you like in multiple threads.
-    Please check the example in the README for a guide to the usage.
-    Args:
-        declare_dag_function: a function that contains the execution of the DAG.
-        if the functions are decorated with @op decorator they can be executed in parallel.
-        Otherwise, they will be executed immediately. Currently mixing the two behaviors isn't supported.
-        max_concurrency: the maximum number of concurrent threads to execute in parallel
-        behavior: the behavior of the dag when an error occurs during the execution of a function (ExecNode)
-    Returns: a DAG instance
-
-    """
-
-    def intermediate_wrapper(_func: Callable[..., Any]) -> Callable[..., DAG]:
-        def wrapped(*args: Any, **kwargs: Any) -> DAG:
-            # TODO: modify this horrible pattern
-            with exec_nodes_lock:
-                node.exec_nodes = []
-                _func(*args, **kwargs)
-                d = DAG(node.exec_nodes, max_concurrency=max_concurrency, behavior=behavior)
-                node.exec_nodes = []
-
-            return d
-
-        return wrapped
-
-    # case 1: arguments are provided to the decorator
-    if declare_dag_function is None:
-        return intermediate_wrapper
-    # case 2: arguments aren't provided to the decorator
-    else:
-        return intermediate_wrapper(declare_dag_function)
+### Improvement
+
+* Run the ExecNode’s function with arbitrary arguments names
+* pass in arguments & return values from created DAGs like normal functions
+* Setup ExecNodes
+* Debug ExecNodes
+* Tag an ExecNode or multiple ExecNodes
+* ExecNode is reusable (even inside the same DAG)
+* Create a SubDag by specifying output ExecNodes of the DAG using Tag, id or the ExecNode itself
+* Setup ExecNode do not accept dynamic arguments (arguments that can change between executions)
+* DAG can return multiple values via dict, tuple or list
+* Cache results of a specific DAG execution inside a file and reuse it later to skip running the same executions again
+* An ExecNode can not be debug and setup at the same time!
+* Configure ExecNodes using yaml, json or a python dict
+* Profile the DAG execution (profiling of each ExecNode's execution)
+* Create a SubDag by specifying ExecNodes to exclude of the DAG using Tag, id or the ExecNode itself
+* pass in a thread-name prefix to the DAG
+* Cache all the dependencies of some ExecNodes but not the specified ExecNodes themselves (helpful for debugging these ExecNodes)
+* Introduce DAGExecution class which is an instance holding an execution of a DAG
+* DAGExecution.scheduled_nodes contains the ExecNodes that will be executed in the next DAGExecution.run() call
+* Support mypy typing
+* Add a documentation page using mkdocs
+* A single ExecNode can have multiple Tags
+* + - * ** / // % divmod abs << >> < <= == > >= operations implemented for ExecNode
+* Conditionally execute an ExecNode inside a DAG using `twz_active`
+* helpers and_, or_, not_ are provided to do logical operations on ExecNodes
+* LazyExecNode can be executed outside of DAG description according to env var TAWAZI_EXECNODE_OUTSIDE_DAG_BEHAVIOR
+* unpack the results of an ExecNode execution using `unpack_to` property
+* Check `unpack_to` property against typing
+* Experimental compose a subdag from a single DAG by choosing the input ExecNodes and the output ExecNodes
+* ExecNode can wrap anonymous functions that have no __qualname__ attribute
+* Choose where an ExecNode is executed (in main-thread or in a thread-pool)
+* Document Usage of the Library
+
+### Breaking Changes
+* Improved Interface to create DAGs using `dag` decorator
+* Improved Interface to create ExecNodes using `xn` decorator
+
+### Internal Changes
+* Use NoVal instead of None to express not yet calculated result in ExecNode
+* Copy ExecNode instead of deep-copying it
+* Run tests against Python 3.7, 3.8, 3.9, 3.10, 3.11
+* Run tests against the documentation
+* Test Mypy
+* Use Ruff in pre-commit
+* use pytest code-blocks instead of mkcodes
+* CI tests building the documentation
+
+## v0.2.0 (2022-10-17)
+
+### New
+* :green_heart: CI with tests on 6 different environments. (Coverage: **99%**)
+* :white_check_mark: Tested on python 3.6, 3.7, 3.8, 3.9, 3.10.
+* :white_check_mark: Tested on Windows and Linux.
+* :recycle: Change the default DAG interface creation to make it ergonomic.
+* :zap: choose Nodes that have more successors over Nodes that no successors.
+* :sparkles: execute the DAG safely without using the scheduler.
+* :sparkles: test the code in the README.
+* :wrench: :technologist: Dynamic configuration of the library with custom environment variables.
+* :memo: :technologist: Static general documentation with mkdocs.
+* :label: Repository passes mypy (not tested on the `--strict` option which is too coercive at the moment).
+* :loud_sound: Changed logging to loguru by default.
+* :sparkles: Implementation of the subgraph execution feature.
+* :green_heart: Dependabot integration.
+* :arrow_up: Switched from requirements to poetry for dependency management.
+* :art: Revamp of the repository.
+* :technologist: :green_heart: Better pre-commit configuration for ease of development.
+
+## v0.1.0 (2022-07-20)
+
+### New
+* :sparkles: first functional iteration of the DAG
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

