# Comparing `tmp/hiperwalk-2.0a2.tar.gz` & `tmp/hiperwalk-2.0a3.tar.gz`

## Comparing `hiperwalk-2.0a2.tar` & `hiperwalk-2.0a3.tar`

### file list

```diff
@@ -1,94 +1,95 @@
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/.readthedocs.yaml
--rwxr-xr-x   0        0        0       62 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/build_and_upload_to_pypi
--rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/Archive/config.py
--rw-r--r--   0        0        0     4261 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/Archive/custom.nbl
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/Archive/custom.py
--rwxr-xr-x   0        0        0     1734 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/Archive/distance.py
--rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/Archive/dtqw1d.nbl
--rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/Archive/dtqw1d.py
--rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/Archive/dtqw2d.nbl
--rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/Archive/dtqw2d.py
--rw-r--r--   0        0        0    12690 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/Archive/gnuplot.py
--rwxr-xr-x   0        0        0      540 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/Archive/hiperwalk.py
--rwxr-xr-x   0        0        0      909 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/Archive/install.sh
--rw-r--r--   0        0        0     3662 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/Archive/ioFunctions.py
--rw-r--r--   0        0        0    22919 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/Archive/neblina.py
--rw-r--r--   0        0        0    29012 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/Archive/operators.py
--rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/Archive/parsing.py
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/Archive/run.py
--rw-r--r--   0        0        0     2787 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/Archive/staggered1d.nbl
--rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/Archive/staggered1d.py
--rw-r--r--   0        0        0     3043 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/Archive/staggered2d.nbl
--rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/Archive/staggered2d.py
--rw-r--r--   0        0        0     4244 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/Archive/standardDeviation.py
--rw-r--r--   0        0        0    12276 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/Archive/state.py
--rw-r--r--   0        0        0    24726 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/Archive/testmode.py
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/Archive/walks.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/Archive/examples/coined1D.in
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/Archive/examples/coined2D.in
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/Archive/examples/custom.in
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/Archive/examples/psi0.dat
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/Archive/examples/staggered1D.in
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/Archive/examples/staggered2D.in
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/Archive/examples/u0.dat
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/Archive/examples/u1.dat
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/docs/Makefile
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/docs/README.md
--rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/docs/conf.py
--rwxr-xr-x   0        0        0       53 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/docs/go
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/docs/index.rst
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/docs/make.bat
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/docs/requirements.txt
--rwxr-xr-x   0        0        0       13 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/docs/test_docs
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/docs/_static/switcher.json
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/docs/_templates/autoclass.rst
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/docs/_templates/autofunctions.rst
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/docs/_templates/automodule.rst
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/docs/_templates/autosummary/class.rst
--rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/docs/development/index.rst
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/docs/documentation/graph.rst
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/docs/documentation/index.rst
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/docs/documentation/plot.rst
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/docs/documentation/quantum_walk.rst
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/docs/graphviz/coined-cycle-edges-labels.dot
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/docs/graphviz/coined-model-edges-labels.dot
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/docs/graphviz/coined-model-sample.dot
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/docs/graphviz/coined-segment-edges-labels.dot
--rw-r--r--   0        0        0     6490 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/docs/install/index.rst
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/docs/tutorial/index.rst
--rw-r--r--   0        0        0   245072 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/examples/Untitled.ipynb
--rw-r--r--   0        0        0  1639169 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/examples/Untitled1.ipynb
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/examples/coined-diagonal-lattice.py
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/examples/continuous-cycle.py
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/examples/refactor.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/hiperwalk/__init__.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/hiperwalk/_constants.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/hiperwalk/graph/__init__.py
--rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/hiperwalk/graph/cycle.py
--rw-r--r--   0        0        0     5764 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/hiperwalk/graph/graph.py
--rw-r--r--   0        0        0    14041 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/hiperwalk/graph/lattice.py
--rw-r--r--   0        0        0     3626 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/hiperwalk/graph/line.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/hiperwalk/plot/__init__.py
--rw-r--r--   0        0        0    11222 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/hiperwalk/plot/_animation.py
--rw-r--r--   0        0        0    26318 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/hiperwalk/plot/_plot.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/hiperwalk/quantum_walk/__init__.py
--rw-r--r--   0        0        0    11173 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/hiperwalk/quantum_walk/_pyneblina_interface.py
--rw-r--r--   0        0        0    33554 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/hiperwalk/quantum_walk/coined_walk.py
--rw-r--r--   0        0        0    10568 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/hiperwalk/quantum_walk/continuous_walk.py
--rw-r--r--   0        0        0    16075 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/hiperwalk/quantum_walk/quantum_walk.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/tests/__init__.py
--rwxr-xr-x   0        0        0      123 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/tests/run_all.sh
--rwxr-xr-x   0        0        0      124 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/tests/run_hpc.sh
--rwxr-xr-x   0        0        0      124 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/tests/run_nonhpc.sh
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/tests/test_constants.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/tests/unitary/__init__.py
--rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/tests/unitary/coined_cycle.py
--rw-r--r--   0        0        0     2733 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/tests/unitary/coined_line.py
--rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/tests/unitary/coined_segment.py
--rw-r--r--   0        0        0     6758 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/tests/unitary/continuous_graph.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/tests/unitary/lattice_uniform_state.py
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/.gitignore
--rw-r--r--   0        0        0     7560 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/LICENSE
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/README.md
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/pyproject.toml
--rw-r--r--   0        0        0    11956 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/PKG-INFO
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/.readthedocs.yaml
+-rwxr-xr-x   0        0        0       62 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/build_and_upload_to_pypi
+-rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/Archive/config.py
+-rw-r--r--   0        0        0     4261 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/Archive/custom.nbl
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/Archive/custom.py
+-rwxr-xr-x   0        0        0     1734 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/Archive/distance.py
+-rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/Archive/dtqw1d.nbl
+-rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/Archive/dtqw1d.py
+-rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/Archive/dtqw2d.nbl
+-rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/Archive/dtqw2d.py
+-rw-r--r--   0        0        0    12690 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/Archive/gnuplot.py
+-rwxr-xr-x   0        0        0      540 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/Archive/hiperwalk.py
+-rwxr-xr-x   0        0        0      909 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/Archive/install.sh
+-rw-r--r--   0        0        0     3662 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/Archive/ioFunctions.py
+-rw-r--r--   0        0        0    22919 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/Archive/neblina.py
+-rw-r--r--   0        0        0    29012 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/Archive/operators.py
+-rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/Archive/parsing.py
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/Archive/run.py
+-rw-r--r--   0        0        0     2787 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/Archive/staggered1d.nbl
+-rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/Archive/staggered1d.py
+-rw-r--r--   0        0        0     3043 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/Archive/staggered2d.nbl
+-rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/Archive/staggered2d.py
+-rw-r--r--   0        0        0     4244 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/Archive/standardDeviation.py
+-rw-r--r--   0        0        0    12276 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/Archive/state.py
+-rw-r--r--   0        0        0    24726 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/Archive/testmode.py
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/Archive/walks.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/Archive/examples/coined1D.in
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/Archive/examples/coined2D.in
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/Archive/examples/custom.in
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/Archive/examples/psi0.dat
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/Archive/examples/staggered1D.in
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/Archive/examples/staggered2D.in
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/Archive/examples/u0.dat
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/Archive/examples/u1.dat
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/docs/Makefile
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/docs/README.md
+-rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/docs/conf.py
+-rwxr-xr-x   0        0        0       53 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/docs/go
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/docs/index.rst
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/docs/make.bat
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/docs/requirements.txt
+-rwxr-xr-x   0        0        0       13 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/docs/test_docs
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/docs/_static/switcher.json
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/docs/_templates/autoclass.rst
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/docs/_templates/autofunctions.rst
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/docs/_templates/automodule.rst
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/docs/_templates/autosummary/class.rst
+-rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/docs/development/index.rst
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/docs/documentation/graph.rst
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/docs/documentation/index.rst
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/docs/documentation/plot.rst
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/docs/documentation/quantum_walk.rst
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/docs/graphviz/coined-cycle-edges-labels.dot
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/docs/graphviz/coined-model-edges-labels.dot
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/docs/graphviz/coined-model-sample.dot
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/docs/graphviz/coined-segment-edges-labels.dot
+-rw-r--r--   0        0        0     6490 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/docs/install/index.rst
+-rw-r--r--   0        0        0     3690 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/docs/tutorial/index.rst
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/docs/tutorial/plotting_customization.rst
+-rw-r--r--   0        0        0   245035 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/examples/Untitled.ipynb
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/examples/Untitled1.ipynb
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/examples/coined-diagonal-lattice.py
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/examples/continuous-cycle.py
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/examples/refactor.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/hiperwalk/__init__.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/hiperwalk/_constants.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/hiperwalk/graph/__init__.py
+-rw-r--r--   0        0        0     3697 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/hiperwalk/graph/cycle.py
+-rw-r--r--   0        0        0     5764 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/hiperwalk/graph/graph.py
+-rw-r--r--   0        0        0    14531 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/hiperwalk/graph/lattice.py
+-rw-r--r--   0        0        0     3622 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/hiperwalk/graph/line.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/hiperwalk/plot/__init__.py
+-rw-r--r--   0        0        0    11222 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/hiperwalk/plot/_animation.py
+-rw-r--r--   0        0        0    26318 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/hiperwalk/plot/_plot.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/hiperwalk/quantum_walk/__init__.py
+-rw-r--r--   0        0        0    11173 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/hiperwalk/quantum_walk/_pyneblina_interface.py
+-rw-r--r--   0        0        0    33527 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/hiperwalk/quantum_walk/coined_walk.py
+-rw-r--r--   0        0        0    10565 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/hiperwalk/quantum_walk/continuous_walk.py
+-rw-r--r--   0        0        0    16075 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/hiperwalk/quantum_walk/quantum_walk.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/tests/__init__.py
+-rwxr-xr-x   0        0        0      123 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/tests/run_all.sh
+-rwxr-xr-x   0        0        0      124 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/tests/run_hpc.sh
+-rwxr-xr-x   0        0        0      124 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/tests/run_nonhpc.sh
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/tests/test_constants.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/tests/unitary/__init__.py
+-rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/tests/unitary/coined_cycle.py
+-rw-r--r--   0        0        0     2733 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/tests/unitary/coined_line.py
+-rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/tests/unitary/coined_segment.py
+-rw-r--r--   0        0        0     6758 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/tests/unitary/continuous_graph.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/tests/unitary/lattice_uniform_state.py
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/.gitignore
+-rw-r--r--   0        0        0     7560 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/LICENSE
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/README.md
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/pyproject.toml
+-rw-r--r--   0        0        0    11956 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/PKG-INFO
```

### Comparing `hiperwalk-2.0a2/Archive/config.py` & `hiperwalk-2.0a3/Archive/config.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a2/Archive/custom.nbl` & `hiperwalk-2.0a3/Archive/custom.nbl`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a2/Archive/custom.py` & `hiperwalk-2.0a3/Archive/custom.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a2/Archive/distance.py` & `hiperwalk-2.0a3/Archive/distance.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a2/Archive/dtqw1d.nbl` & `hiperwalk-2.0a3/Archive/dtqw1d.nbl`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a2/Archive/dtqw1d.py` & `hiperwalk-2.0a3/Archive/dtqw1d.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a2/Archive/dtqw2d.nbl` & `hiperwalk-2.0a3/Archive/dtqw2d.nbl`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a2/Archive/dtqw2d.py` & `hiperwalk-2.0a3/Archive/dtqw2d.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a2/Archive/gnuplot.py` & `hiperwalk-2.0a3/Archive/gnuplot.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a2/Archive/hiperwalk.py` & `hiperwalk-2.0a3/Archive/hiperwalk.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a2/Archive/install.sh` & `hiperwalk-2.0a3/Archive/install.sh`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a2/Archive/ioFunctions.py` & `hiperwalk-2.0a3/Archive/ioFunctions.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a2/Archive/neblina.py` & `hiperwalk-2.0a3/Archive/neblina.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a2/Archive/operators.py` & `hiperwalk-2.0a3/Archive/operators.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a2/Archive/parsing.py` & `hiperwalk-2.0a3/Archive/parsing.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a2/Archive/run.py` & `hiperwalk-2.0a3/Archive/run.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a2/Archive/staggered1d.nbl` & `hiperwalk-2.0a3/Archive/staggered1d.nbl`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a2/Archive/staggered1d.py` & `hiperwalk-2.0a3/Archive/staggered1d.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a2/Archive/staggered2d.nbl` & `hiperwalk-2.0a3/Archive/staggered2d.nbl`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a2/Archive/staggered2d.py` & `hiperwalk-2.0a3/Archive/staggered2d.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a2/Archive/standardDeviation.py` & `hiperwalk-2.0a3/Archive/standardDeviation.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a2/Archive/state.py` & `hiperwalk-2.0a3/Archive/state.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a2/Archive/testmode.py` & `hiperwalk-2.0a3/Archive/testmode.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a2/Archive/walks.py` & `hiperwalk-2.0a3/Archive/walks.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a2/docs/Makefile` & `hiperwalk-2.0a3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a2/docs/conf.py` & `hiperwalk-2.0a3/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # -- Project information -----------------------------------------------------
 
 project = 'Hiperwalk'
 copyright = '2023'
 author = 'Gustavo Bezerra'
 
 # The full version, including alpha/beta/rc tags
-release = '2.0a2'
+release = '2.0a3'
 version = 'stable'
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
```

### Comparing `hiperwalk-2.0a2/docs/index.rst` & `hiperwalk-2.0a3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a2/docs/make.bat` & `hiperwalk-2.0a3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a2/docs/_templates/automodule.rst` & `hiperwalk-2.0a3/docs/_templates/automodule.rst`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a2/docs/development/index.rst` & `hiperwalk-2.0a3/docs/development/index.rst`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a2/docs/graphviz/coined-model-edges-labels.dot` & `hiperwalk-2.0a3/docs/graphviz/coined-model-edges-labels.dot`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a2/docs/install/index.rst` & `hiperwalk-2.0a3/docs/install/index.rst`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a2/examples/Untitled.ipynb` & `hiperwalk-2.0a3/examples/Untitled.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9954943783068784%*

 * *Differences: {"'cells'": "{0: {'outputs': {0: {'text': {insert: [(0, "*

 * *            "'/home/koruja/.local/lib/python3.10/site-packages/hiperwalk/quantum_walk/quantum_walk.py:12: "*

 * *            'UserWarning: Could not import pyneblina interface. Do you have neblina-core and '*

 * *            "pyneblina installed?\\n')], delete: [0]}}}, 'source': {delete: [1, 0]}}, 2: "*

 * *            "{'execution_count': 3}}"}*

```diff
@@ -6,26 +6,24 @@
             "id": "4cd49b2b",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "/home/koruja/hiperwalk/examples/../hiperwalk/quantum_walk/quantum_walk.py:12: UserWarning: Could not import pyneblina interface. Do you have neblina-core and pyneblina installed?\n",
+                        "/home/koruja/.local/lib/python3.10/site-packages/hiperwalk/quantum_walk/quantum_walk.py:12: UserWarning: Could not import pyneblina interface. Do you have neblina-core and pyneblina installed?\n",
                         "#######################\n",
                         "Continuing without hpc.\n",
                         "#######################\n",
                         "\n",
                         "  warn(PYNEBLINA_IMPORT_ERROR_MSG)\n"
                     ]
                 }
             ],
             "source": [
-                "import sys\n",
-                "sys.path.append('..')\n",
                 "import hiperwalk as hpw\n",
                 "\n",
                 "N = 101\n",
                 "cycle = hpw.Cycle(N)\n",
                 "ctqw = hpw.ContinuousWalk(cycle, gamma=0.35)\n",
                 "psi0 = ctqw.ket(N // 2)"
             ]
@@ -39,15 +37,15 @@
             "source": [
                 "psi_final = ctqw.simulate(time=(0, 50, 1), initial_condition=psi0)\n",
                 "prob = ctqw.probability_distribution(psi_final)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": 3,
             "id": "1039a3bb",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<video width=\"1200\" height=\"1000\" controls autoplay loop>\n",
```

### Comparing `hiperwalk-2.0a2/examples/coined-diagonal-lattice.py` & `hiperwalk-2.0a3/examples/coined-diagonal-lattice.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a2/hiperwalk/_constants.py` & `hiperwalk-2.0a3/hiperwalk/_constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '2.0a2'
+__version__ = '2.0a3'
 
 #Declares data types according to neblina-core
 #TODO: make it so it is not hardcoded
 NEBLINA_FLOAT = 2
 NEBLINA_COMPLEX = 13 
 
 from sys import modules as sys_modules
```

### Comparing `hiperwalk-2.0a2/hiperwalk/graph/cycle.py` & `hiperwalk-2.0a3/hiperwalk/graph/cycle.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     
         # initializing
         super().__init__(adj_matrix)
 
     def embeddable(self):
         return True
 
-    def get_default_coin(self):
+    def default_coin(self):
         r"""
         Returns the default coin name.
         """
         return 'hadamard'
 
     def arc_label(self, tail, head):
         num_vert = self.number_of_vertices()
```

### Comparing `hiperwalk-2.0a2/hiperwalk/graph/graph.py` & `hiperwalk-2.0a3/hiperwalk/graph/graph.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a2/hiperwalk/graph/lattice.py` & `hiperwalk-2.0a3/hiperwalk/graph/lattice.py`

 * *Files 3% similar despite different names*

```diff
@@ -440,16 +440,31 @@
         y_dim : int
             Dimension alongside de Y axis.
         """
         return (self.x_dim, self.y_dim)
 
     def get_central_vertex(self):
         r"""
-        Central vertex is different from center vertex.
-        In the sense that...
+        Vertex with label in the center of the graph as grid.
+
+        .. deprecated:: 2.0a1
+            ``get_central_vertex`` will be removed in Python 2.1 because
+            the user can calculate the central vertex easily using
+            :meth:`dimensions`.
+
+        The central vertex is the vertex that would be located at the
+        grid center after mapping every vertex ``(x, y)`` to its
+        respetive grid point.
+        
+        This is not the center vertex.
+
+        Raises
+        ------
+        ValueError
+            If any lattice dimension is even.
         """
         warn('`get_central_vertex` is deprecated. '
              + 'It will be removed in version 2.1.',
              DeprecationWarning)
 
         if self.x_dim % 2 != 1 or self.y_dim % 2 != 1:
             raise ValueError(
```

### Comparing `hiperwalk-2.0a2/hiperwalk/graph/line.py` & `hiperwalk-2.0a3/hiperwalk/graph/line.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     
         # initializing
         super().__init__(adj_matrix)
 
     def embeddable(self):
         return True
 
-    def get_default_coin(self):
+    def default_coin(self):
         r"""
         Returns the default coin name.
 
         The default coin for the coined quantum walk on the
         segment is ``'hadamard'``.
         """
         return 'hadamard'
```

### Comparing `hiperwalk-2.0a2/hiperwalk/plot/_animation.py` & `hiperwalk-2.0a3/hiperwalk/plot/_animation.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a2/hiperwalk/plot/_plot.py` & `hiperwalk-2.0a3/hiperwalk/plot/_plot.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a2/hiperwalk/quantum_walk/_pyneblina_interface.py` & `hiperwalk-2.0a3/hiperwalk/quantum_walk/_pyneblina_interface.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a2/hiperwalk/quantum_walk/coined_walk.py` & `hiperwalk-2.0a3/hiperwalk/quantum_walk/coined_walk.py`

 * *Files 1% similar despite different names*

```diff
@@ -834,35 +834,33 @@
         If the coin operator was set as an explicit matrix,
         the marked vertices to not alter it.
         If the coin operator was not set as an explicit matrix
         (e.g. as a list of coins),
         the coin of each marked vertex is substituted as specified by
         the last :meth:`set_marked` call.
 
-        Notes
-        -----
-
         .. todo::
             * Sparse matrix multipliation is not supported yet.
               Converting all matrices to dense.
               Then converting back to sparse.
               This uses unnecessary memory and computational time.
             * Check if matrix is sparse in pynelibna interface
             * Check if matrices are deleted from memory and GPU.
 
+
         References
         ----------
         .. [1] Portugal, Renato. "Quantum walks and search algorithms".
             Vol. 19. New York: Springer, 2013.
 
         Examples
         --------
 
         .. todo::
-            valid examples to clear behaviour
+            Valid examples to clear behaviour.
         """
         if self._evolution is not None:
             # evolution operator was not changed.
             # No need to create it again
             return self._evolution
 
         U = None
```

### Comparing `hiperwalk-2.0a2/hiperwalk/quantum_walk/continuous_walk.py` & `hiperwalk-2.0a3/hiperwalk/quantum_walk/continuous_walk.py`

 * *Files 0% similar despite different names*

```diff
@@ -228,17 +228,17 @@
         :math:`t` is the time.
 
         The evolution operator is constructed by Taylor Series expansion.
 
         .. warning::
             For floating time (not integer),
             the result is approximated. It is recommended to
-             choose a small time interval and performing
-             multiple matrix multiplications to
-             mitigate uounding errors.
+            choose a small time interval and performing
+            multiple matrix multiplications to
+            mitigate uounding errors.
         """
         if time is None or time < 0:
             raise ValueError(
                 "Expected non-negative `time` value."
             )
 
         if self._hamiltonian is None:
```

### Comparing `hiperwalk-2.0a2/hiperwalk/quantum_walk/quantum_walk.py` & `hiperwalk-2.0a3/hiperwalk/quantum_walk/quantum_walk.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a2/tests/unitary/coined_cycle.py` & `hiperwalk-2.0a3/tests/unitary/coined_cycle.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a2/tests/unitary/coined_line.py` & `hiperwalk-2.0a3/tests/unitary/coined_line.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a2/tests/unitary/coined_segment.py` & `hiperwalk-2.0a3/tests/unitary/coined_segment.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a2/tests/unitary/continuous_graph.py` & `hiperwalk-2.0a3/tests/unitary/continuous_graph.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a2/.gitignore` & `hiperwalk-2.0a3/.gitignore`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a2/LICENSE` & `hiperwalk-2.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a2/README.md` & `hiperwalk-2.0a3/README.md`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a2/pyproject.toml` & `hiperwalk-2.0a3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "hiperwalk"
-version = "2.0a2"
+version = "2.0a3"
 description = "High-Performance Quantum Walk Simulator"
 license = {file="LICENSE"}
 readme = "README.md"
 authors = [
   { name="Gustavo Bezerra", email="gbezerra@posgrad.lncc.br" },
   { name="Paulo Motta", email="prmottajr@gmail.com" },
   { name="Renato Portugal", email="portugal@lncc.br" },
```

### Comparing `hiperwalk-2.0a2/PKG-INFO` & `hiperwalk-2.0a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hiperwalk
-Version: 2.0a2
+Version: 2.0a3
 Summary: High-Performance Quantum Walk Simulator
 Project-URL: homepage, http://qubit.lncc.br/qwalk/
 Project-URL: documentation, https://hiperwalk.readthedocs.io/
 Project-URL: source, https://github.com/hiperwalk/hiperwalk
 Author-email: Gustavo Bezerra <gbezerra@posgrad.lncc.br>, Paulo Motta <prmottajr@gmail.com>, Renato Portugal <portugal@lncc.br>
 Maintainer-email: Hiperwalk Organization <hiperwalk@gmail.com>
 License: GNU Lesser General Public License
```

