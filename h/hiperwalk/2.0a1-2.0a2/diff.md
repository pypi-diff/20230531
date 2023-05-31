# Comparing `tmp/hiperwalk-2.0a1.tar.gz` & `tmp/hiperwalk-2.0a2.tar.gz`

## Comparing `hiperwalk-2.0a1.tar` & `hiperwalk-2.0a2.tar`

### file list

```diff
@@ -1,95 +1,94 @@
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/.readthedocs.yaml
--rwxr-xr-x   0        0        0       62 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/build_and_upload_to_pypi
--rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/Archive/config.py
--rw-r--r--   0        0        0     4261 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/Archive/custom.nbl
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/Archive/custom.py
--rwxr-xr-x   0        0        0     1734 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/Archive/distance.py
--rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/Archive/dtqw1d.nbl
--rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/Archive/dtqw1d.py
--rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/Archive/dtqw2d.nbl
--rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/Archive/dtqw2d.py
--rw-r--r--   0        0        0    12690 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/Archive/gnuplot.py
--rwxr-xr-x   0        0        0      540 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/Archive/hiperwalk.py
--rwxr-xr-x   0        0        0      909 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/Archive/install.sh
--rw-r--r--   0        0        0     3662 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/Archive/ioFunctions.py
--rw-r--r--   0        0        0    22919 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/Archive/neblina.py
--rw-r--r--   0        0        0    29012 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/Archive/operators.py
--rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/Archive/parsing.py
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/Archive/run.py
--rw-r--r--   0        0        0     2787 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/Archive/staggered1d.nbl
--rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/Archive/staggered1d.py
--rw-r--r--   0        0        0     3043 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/Archive/staggered2d.nbl
--rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/Archive/staggered2d.py
--rw-r--r--   0        0        0     4244 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/Archive/standardDeviation.py
--rw-r--r--   0        0        0    12276 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/Archive/state.py
--rw-r--r--   0        0        0    24726 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/Archive/testmode.py
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/Archive/walks.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/Archive/examples/coined1D.in
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/Archive/examples/coined2D.in
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/Archive/examples/custom.in
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/Archive/examples/psi0.dat
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/Archive/examples/staggered1D.in
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/Archive/examples/staggered2D.in
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/Archive/examples/u0.dat
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/Archive/examples/u1.dat
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/docs/Makefile
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/docs/README.md
--rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/docs/conf.py
--rwxr-xr-x   0        0        0       53 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/docs/go
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/docs/index.rst
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/docs/make.bat
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/docs/requirements.txt
--rwxr-xr-x   0        0        0       13 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/docs/test_docs
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/docs/_static/switcher.json
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/docs/_templates/autoclass.rst
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/docs/_templates/autofunctions.rst
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/docs/_templates/automodule.rst
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/docs/_templates/autosummary/class.rst
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/docs/development/index.rst
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/docs/documentation/graph.rst
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/docs/documentation/index.rst
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/docs/documentation/plot.rst
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/docs/documentation/quantum_walk.rst
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/docs/graphviz/coined-cycle-edges-labels.dot
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/docs/graphviz/coined-model-edges-labels.dot
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/docs/graphviz/coined-model-sample.dot
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/docs/graphviz/coined-segment-edges-labels.dot
--rw-r--r--   0        0        0     7564 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/docs/install/index.rst
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/docs/tutorial/index.rst
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/examples/coined-diagonal-lattice.py
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/examples/continuous-cycle.py
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/examples/deleteme.py
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/examples/hypercube.py
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/examples/refactor.py
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/examples/renato.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/hiperwalk/__init__.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/hiperwalk/_constants.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/hiperwalk/graph/__init__.py
--rw-r--r--   0        0        0     5220 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/hiperwalk/graph/cycle.py
--rw-r--r--   0        0        0     3595 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/hiperwalk/graph/graph.py
--rw-r--r--   0        0        0    11813 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/hiperwalk/graph/lattice.py
--rw-r--r--   0        0        0     3708 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/hiperwalk/graph/line.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/hiperwalk/plot/__init__.py
--rw-r--r--   0        0        0    11851 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/hiperwalk/plot/_animation.py
--rw-r--r--   0        0        0    26324 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/hiperwalk/plot/_plot.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/hiperwalk/quantum_walk/__init__.py
--rw-r--r--   0        0        0    11524 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/hiperwalk/quantum_walk/_pyneblina_interface.py
--rw-r--r--   0        0        0    33983 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/hiperwalk/quantum_walk/coined_walk.py
--rw-r--r--   0        0        0    10615 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/hiperwalk/quantum_walk/continuous_walk.py
--rw-r--r--   0        0        0    16420 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/hiperwalk/quantum_walk/quantum_walk.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/tests/__init__.py
--rwxr-xr-x   0        0        0      123 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/tests/run_all.sh
--rwxr-xr-x   0        0        0      124 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/tests/run_hpc.sh
--rwxr-xr-x   0        0        0      124 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/tests/run_nonhpc.sh
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/tests/test_constants.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/tests/unitary/__init__.py
--rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/tests/unitary/coined_cycle.py
--rw-r--r--   0        0        0     2733 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/tests/unitary/coined_line.py
--rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/tests/unitary/coined_segment.py
--rw-r--r--   0        0        0     6758 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/tests/unitary/continuous_graph.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/tests/unitary/lattice_uniform_state.py
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/.gitignore
--rw-r--r--   0        0        0     7560 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/LICENSE
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/README.md
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/pyproject.toml
--rw-r--r--   0        0        0    11956 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/PKG-INFO
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/.readthedocs.yaml
+-rwxr-xr-x   0        0        0       62 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/build_and_upload_to_pypi
+-rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/Archive/config.py
+-rw-r--r--   0        0        0     4261 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/Archive/custom.nbl
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/Archive/custom.py
+-rwxr-xr-x   0        0        0     1734 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/Archive/distance.py
+-rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/Archive/dtqw1d.nbl
+-rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/Archive/dtqw1d.py
+-rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/Archive/dtqw2d.nbl
+-rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/Archive/dtqw2d.py
+-rw-r--r--   0        0        0    12690 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/Archive/gnuplot.py
+-rwxr-xr-x   0        0        0      540 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/Archive/hiperwalk.py
+-rwxr-xr-x   0        0        0      909 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/Archive/install.sh
+-rw-r--r--   0        0        0     3662 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/Archive/ioFunctions.py
+-rw-r--r--   0        0        0    22919 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/Archive/neblina.py
+-rw-r--r--   0        0        0    29012 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/Archive/operators.py
+-rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/Archive/parsing.py
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/Archive/run.py
+-rw-r--r--   0        0        0     2787 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/Archive/staggered1d.nbl
+-rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/Archive/staggered1d.py
+-rw-r--r--   0        0        0     3043 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/Archive/staggered2d.nbl
+-rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/Archive/staggered2d.py
+-rw-r--r--   0        0        0     4244 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/Archive/standardDeviation.py
+-rw-r--r--   0        0        0    12276 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/Archive/state.py
+-rw-r--r--   0        0        0    24726 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/Archive/testmode.py
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/Archive/walks.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/Archive/examples/coined1D.in
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/Archive/examples/coined2D.in
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/Archive/examples/custom.in
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/Archive/examples/psi0.dat
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/Archive/examples/staggered1D.in
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/Archive/examples/staggered2D.in
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/Archive/examples/u0.dat
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/Archive/examples/u1.dat
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/docs/Makefile
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/docs/README.md
+-rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/docs/conf.py
+-rwxr-xr-x   0        0        0       53 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/docs/go
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/docs/index.rst
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/docs/make.bat
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/docs/requirements.txt
+-rwxr-xr-x   0        0        0       13 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/docs/test_docs
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/docs/_static/switcher.json
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/docs/_templates/autoclass.rst
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/docs/_templates/autofunctions.rst
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/docs/_templates/automodule.rst
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/docs/_templates/autosummary/class.rst
+-rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/docs/development/index.rst
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/docs/documentation/graph.rst
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/docs/documentation/index.rst
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/docs/documentation/plot.rst
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/docs/documentation/quantum_walk.rst
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/docs/graphviz/coined-cycle-edges-labels.dot
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/docs/graphviz/coined-model-edges-labels.dot
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/docs/graphviz/coined-model-sample.dot
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/docs/graphviz/coined-segment-edges-labels.dot
+-rw-r--r--   0        0        0     6490 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/docs/install/index.rst
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/docs/tutorial/index.rst
+-rw-r--r--   0        0        0   245072 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/examples/Untitled.ipynb
+-rw-r--r--   0        0        0  1639169 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/examples/Untitled1.ipynb
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/examples/coined-diagonal-lattice.py
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/examples/continuous-cycle.py
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/examples/refactor.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/hiperwalk/__init__.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/hiperwalk/_constants.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/hiperwalk/graph/__init__.py
+-rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/hiperwalk/graph/cycle.py
+-rw-r--r--   0        0        0     5764 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/hiperwalk/graph/graph.py
+-rw-r--r--   0        0        0    14041 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/hiperwalk/graph/lattice.py
+-rw-r--r--   0        0        0     3626 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/hiperwalk/graph/line.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/hiperwalk/plot/__init__.py
+-rw-r--r--   0        0        0    11222 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/hiperwalk/plot/_animation.py
+-rw-r--r--   0        0        0    26318 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/hiperwalk/plot/_plot.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/hiperwalk/quantum_walk/__init__.py
+-rw-r--r--   0        0        0    11173 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/hiperwalk/quantum_walk/_pyneblina_interface.py
+-rw-r--r--   0        0        0    33554 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/hiperwalk/quantum_walk/coined_walk.py
+-rw-r--r--   0        0        0    10568 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/hiperwalk/quantum_walk/continuous_walk.py
+-rw-r--r--   0        0        0    16075 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/hiperwalk/quantum_walk/quantum_walk.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/tests/__init__.py
+-rwxr-xr-x   0        0        0      123 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/tests/run_all.sh
+-rwxr-xr-x   0        0        0      124 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/tests/run_hpc.sh
+-rwxr-xr-x   0        0        0      124 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/tests/run_nonhpc.sh
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/tests/test_constants.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/tests/unitary/__init__.py
+-rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/tests/unitary/coined_cycle.py
+-rw-r--r--   0        0        0     2733 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/tests/unitary/coined_line.py
+-rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/tests/unitary/coined_segment.py
+-rw-r--r--   0        0        0     6758 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/tests/unitary/continuous_graph.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/tests/unitary/lattice_uniform_state.py
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/.gitignore
+-rw-r--r--   0        0        0     7560 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/LICENSE
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/README.md
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/pyproject.toml
+-rw-r--r--   0        0        0    11956 2020-02-02 00:00:00.000000 hiperwalk-2.0a2/PKG-INFO
```

### Comparing `hiperwalk-2.0a1/Archive/config.py` & `hiperwalk-2.0a2/Archive/config.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a1/Archive/custom.nbl` & `hiperwalk-2.0a2/Archive/custom.nbl`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a1/Archive/custom.py` & `hiperwalk-2.0a2/Archive/custom.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a1/Archive/distance.py` & `hiperwalk-2.0a2/Archive/distance.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a1/Archive/dtqw1d.nbl` & `hiperwalk-2.0a2/Archive/dtqw1d.nbl`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a1/Archive/dtqw1d.py` & `hiperwalk-2.0a2/Archive/dtqw1d.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a1/Archive/dtqw2d.nbl` & `hiperwalk-2.0a2/Archive/dtqw2d.nbl`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a1/Archive/dtqw2d.py` & `hiperwalk-2.0a2/Archive/dtqw2d.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a1/Archive/gnuplot.py` & `hiperwalk-2.0a2/Archive/gnuplot.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a1/Archive/hiperwalk.py` & `hiperwalk-2.0a2/Archive/hiperwalk.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a1/Archive/install.sh` & `hiperwalk-2.0a2/Archive/install.sh`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a1/Archive/ioFunctions.py` & `hiperwalk-2.0a2/Archive/ioFunctions.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a1/Archive/neblina.py` & `hiperwalk-2.0a2/Archive/neblina.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a1/Archive/operators.py` & `hiperwalk-2.0a2/Archive/operators.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a1/Archive/parsing.py` & `hiperwalk-2.0a2/Archive/parsing.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a1/Archive/run.py` & `hiperwalk-2.0a2/Archive/run.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a1/Archive/staggered1d.nbl` & `hiperwalk-2.0a2/Archive/staggered1d.nbl`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a1/Archive/staggered1d.py` & `hiperwalk-2.0a2/Archive/staggered1d.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a1/Archive/staggered2d.nbl` & `hiperwalk-2.0a2/Archive/staggered2d.nbl`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a1/Archive/staggered2d.py` & `hiperwalk-2.0a2/Archive/staggered2d.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a1/Archive/standardDeviation.py` & `hiperwalk-2.0a2/Archive/standardDeviation.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a1/Archive/state.py` & `hiperwalk-2.0a2/Archive/state.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a1/Archive/testmode.py` & `hiperwalk-2.0a2/Archive/testmode.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a1/Archive/walks.py` & `hiperwalk-2.0a2/Archive/walks.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a1/docs/Makefile` & `hiperwalk-2.0a2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a1/docs/conf.py` & `hiperwalk-2.0a2/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # -- Project information -----------------------------------------------------
 
 project = 'Hiperwalk'
 copyright = '2023'
 author = 'Gustavo Bezerra'
 
 # The full version, including alpha/beta/rc tags
-release = '2.0a1'
+release = '2.0a2'
 version = 'stable'
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
```

### Comparing `hiperwalk-2.0a1/docs/index.rst` & `hiperwalk-2.0a2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a1/docs/make.bat` & `hiperwalk-2.0a2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a1/docs/_templates/automodule.rst` & `hiperwalk-2.0a2/docs/_templates/automodule.rst`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a1/docs/development/index.rst` & `hiperwalk-2.0a2/docs/development/index.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,55 @@
 ===========
 Development
 ===========
 
+HiperWalk is built on top of some Python libraries.
+Before developing for HiperWalk,
+we must install these libraries.
+HiperWalk requires
+`numpy <https://numpy.org/>`_,
+`scipy <https://scipy.org/>`_,
+`networkx <https://networkx.org/>`_, and
+`matplotlib <https://matplotlib.org/>`_.
+To install these libraries run
+
+.. code-block:: shell
+
+   pip3 install numpy
+   pip3 install scipy
+   pip3 install networkx
+   pip3 install matplotlib
+
 The ``main`` branch is where the new features are developed.
 To contribute, clone the repository.
 
 .. code-block:: shell
 
     git clone https://github.com/hiperwalk/hiperwalk.git
 
 Then, make the desired alterations.
 And make a pull request.
 
-.. todo::
+Testing
+=======
+
+Tests are located into the ``hiperwalk/tests/`` directory.
+If you performed the complete installation (with HPC support),
+execute
+
+.. code-block:: shell
+
+    ./run_all.sh
+
+If you installed the standalone version (with no HPC support),
+execute
+
+.. code-block:: shell
 
-   Continuous model must be implemented.
+    ./run_nonhpc.sh
 
 Documentation
 =============
 
 It is very likely that there are new features in the ``main`` branch.
 These new features are documentated online in the **latest** version.
```

### Comparing `hiperwalk-2.0a1/docs/graphviz/coined-model-edges-labels.dot` & `hiperwalk-2.0a2/docs/graphviz/coined-model-edges-labels.dot`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a1/docs/install/index.rst` & `hiperwalk-2.0a2/docs/install/index.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,73 @@
 =======
 Install
 =======
 
-HiperWalk is built on top of some Python libraries.
+Hiperwalk is built on top of some Python libraries.
 By just installing the Python libraries,
-HiperWalk does not make use of High-Performance Computing (HPC).
-If an installating without support for HPC is desired,
-you can jump to :ref:`docs_install_hiperwalk`.
+Hiperwalk does not make use of High-Performance Computing (HPC).
+If an installating with HPC support is desired,
+you can jump to :ref:`docs_install_hpc_prerequisites`
+before installing Hiperwalk.
 
-For supporting HPC,
-HiperWalk uses 
-`neblina-core <https://github.com/paulomotta/neblina-core>`_,
-and `pyneblina <https://github.com/paulomotta/pyneblina>`_.
-Although a computer with a **GPU compatible with CUDA** is necessary.
-
-In this page we describe the process of installing HiperWalk in a
+In this page we describe the process of installing Hiperwalk in a
 freshly installed Ubuntu 20.04 operating system.
 We will describe the process of identifying the GPU, and
 installing the GPU drivers, neblina-core, pyneblina, and
 the necessary Python libraries.
 
 .. warning::
 
    Other distributions than Ubuntu 20.04 are currently not supported.
 
    Support for Ubuntu 22.04 is under development.
    Contributions are welcomed.
 
-.. _docs_install_prerequisites:
+.. _docs_install_hiperwalk:
+
+Hiperwalk
+=========
+
+Hiperwalk can be easily installed via pip.
+First of all, install pip.
+
+.. code-block:: shell
+
+   sudo apt install python3-pip
+
+The following command
+install Hiperwalk and all its Python dependencies.
+Namely
+`numpy <https://numpy.org/>`_,
+`scipy <https://scipy.org/>`_,
+`networkx <https://networkx.org/>`_, and
+`matplotlib <https://matplotlib.org/>`_.
+
+.. warning::
+
+   If you have an old version of these packages,
+   it will be probably updated.
+   If you do not wish this to happen, we recommend you to
+   `create a virtual environment
+   <https://docs.python.org/3/library/venv.html>`_.
+
+.. code-block:: shell
+
+   pip3 install hiperwalk
+
+To test if it the installation was successful,
+you can execute any code in
+`repository examples directory
+<https://`https://github.com/hiperwalk/hiperwalk/tree/2.0.x/examples>`_
+or go to the :ref:`docs_tutorial`.
 
-Prerequisites
-=============
+.. _docs_install_hpc_prerequisites:
+
+HPC Prerequisites
+=================
 
 Beforehand, it is recommended to update and upgrade the Ubuntu packages.
 Execute
 
 .. code-block:: shell
 
    sudo apt update
@@ -139,14 +172,21 @@
 
    nvcc --version
 
 
 Installing neblina-core And pyneblina
 =====================================
 
+For HPC support,
+Hiperwalk uses 
+`neblina-core <https://github.com/paulomotta/neblina-core>`_,
+and `pyneblina <https://github.com/paulomotta/pyneblina>`_.
+Although a computer with a **GPU compatible with CUDA** is necessary.
+
+
 We compile the information in
 `Paulo Motta's blog <https://paulomotta.pro.br/wp/2021/05/01/pyneblina-and-neblina-core/>`_,
 `neblina-core github <https://github.com/paulomotta/neblina-core>`_,
 and `pyneblina github <https://github.com/paulomotta/pyneblina>`_.
 
 It is **strongly recommended** that neblina-core and pyneblina
 are installed (i.e. cloned) in the same directory.
@@ -212,103 +252,7 @@
 
 To verify if the installation completed successfully,
 run the test.
 
 .. code-block:: shell
 
    python3 test.py
-
-.. _docs_install_hiperwalk:
-
-HiperWalk
-=========
-
-As stated previously,
-HiperWalk is built on top of some Python libraries.
-Before installing HiperWalk,
-we must install these libraries.
-
-
-.. note::
-
-   If you are installing HiperWalk with no HPC support,
-   you probably did not install ``pip`` as mentioned in
-   :ref:`docs_install_prerequisites`.
-   If that's the case, run the following command.
-
-   .. code-block:: shell
-
-       sudo apt install python3-pip
-
-
-HiperWalk requires
-`numpy <https://numpy.org/>`_,
-`scipy <https://scipy.org/>`_,
-`networkx <https://networkx.org/>`_, and
-`matplotlib <https://matplotlib.org/>`_.
-To install these libraries run
-
-.. code-block:: shell
-
-   pip3 install numpy
-   pip3 install scipy
-   pip3 install networkx
-   pip3 install matplotlib
-
-Then, choose which version you are going to install.
-The stable version or
-the latest version (under development).
-
-Stable
-------
-
-Clone the HiperWalk repository branch tagged as stable.
-For example, run the following command
-in the directory where neblina-core and pyneblina are --
-most likely the home directory.
-
-.. code-block:: shell
-
-   cd ~
-   git clone -b stable https://github.com/hiperwalk/hiperwalk.git
-
-Latest
-------
-
-Clone the HiperWalk repository --
-e.g. in the home directory where neblina-core and pyneblina are.
-
-.. code-block:: shell
-
-   cd ~
-   git clone https://github.com/hiperwalk/hiperwalk.git
-
-
-Testing
--------
-
-The installation is finished.
-To test if it was successful,
-go into the ``hiperwalk/examples/`` directory 
-and execute the test accoring to you installation.
-If you performed the complete installation (with HPC support),
-execute
-
-.. code-block:: shell
-
-    ./run_all.sh
-
-If you installed the standalone version (with no HPC support),
-execute
-
-.. code-block:: shell
-
-    ./run_nonhpc.sh
-
-There are some examples in the ``hiperwalk/examples/`` directory.
-You may execute any code inside this directory.
-For instance,
-
-.. code-block:: shell
-
-    cd ~/hiperwalk/examples/
-    python3 non-hpc-coined-line.py
```

### Comparing `hiperwalk-2.0a1/examples/coined-diagonal-lattice.py` & `hiperwalk-2.0a2/examples/coined-diagonal-lattice.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a1/hiperwalk/_constants.py` & `hiperwalk-2.0a2/hiperwalk/_constants.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '2.0a1'
+__version__ = '2.0a2'
 
 #Declares data types according to neblina-core
 #TODO: make it so it is not hardcoded
 NEBLINA_FLOAT = 2
 NEBLINA_COMPLEX = 13 
 
 from sys import modules as sys_modules
```

### Comparing `hiperwalk-2.0a1/hiperwalk/graph/graph.py` & `hiperwalk-2.0a2/hiperwalk/graph/line.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,125 +1,118 @@
 import numpy as np
-from warnings import warn
+from scipy.sparse import csr_array
+from sys import path as sys_path
+from .graph import Graph
 
-def _binary_search(v, elem, start=0, end=None):
+class Line(Graph):
     r"""
-    expects sorted array and executes binary search in the subarray
-    v[start:end] searching for elem.
-    Return the index of the element if found, otherwise returns -1
-    Cormen's binary search implementation.
-    Used to improve time complexity
-    """
-    if end == None:
-        end = len(v)
-    
-    while start < end:
-        mid = int((start + end)/2)
-        if elem <= v[mid]:
-            end = mid
-        else:
-            start = mid + 1
-
-    return end if v[end] == elem else -1
-
-class Graph():
-    r"""
-    Graph on which a quantum walk occurs.
-
-    Used for generic graphs.
+    Finite Line Graph (Path Graph).
 
     Parameters
     ----------
-    adj_matrix : :class:`scipy.sparse.csr_array`
-        Adjacency matrix of the graph on
-        which the quantum walk occurs.
-
-    Raises
-    ------
-    TypeError
-        if ``adj_matrix`` is not an instance of
-        :class:`scipy.sparse.csr_array`.
+    num_vert : int
+        Number of vertices on the line.
 
     Notes
     -----
-    Makes a plethora of methods available.
-    These methods may be used by a Quantum Walk model for
-    generating a valid walk.
-    The default arguments for a given model are given by the graph.
-    The Quantum Walk model is ignorant with this regard.
+    .. todo::
 
-    This class may be passed as argument to plotting methods.
-    Then the default representation for the specific graph will be shown.
-    """
+        update
 
-    def __init__(self, adj_matrix):
-        warn("Check if valid adjacency matrix")
-        self.adj_matrix = adj_matrix
-        self.coloring = None
 
-    def default_coin(self):
-        r"""
-        Returns the default coin for the given graph.
+    Since :class:`Segment` is built on top of :class:`Graph`,
+    operators and states respect the edge order
+    (See :class:`Graph` notes for more details).
+    As a consequence, for any vertex :math:`v \in V`,
+    the state :math:`\ket{2v - d}` for :math:`d \in \{0, 1\}`
+    corresponds to the walker being on vertex :math:`v` and the
+    coin pointing rightwars (:math:`d = 0`) or leftwards (:math:`d = 1`).
+    For example, the edges labels of the 4-vertices :class:`Segment`
+    are represented in Figure 1.
+    
+    .. graphviz:: ../../graphviz/coined-segment-edges-labels.dot
+        :align: center
+        :layout: neato
+        :caption: Figure 1.
+    """
 
-        The default coin for the coined quantum walk on general
-        graphs is ``grover``.
-        """
-        return 'grover'
+    def __init__(self, num_vert):
+        # Creating adjacency matrix
+        # The end vertices are only adjacent to 1 vertex.
+        # Every other vertex is adjacent to two vertices.
+        data = np.ones(2*(num_vert-1), dtype=np.int8)
+        # upper diagonal
+        row_ind = [lin+shift for shift in range(2)
+                             for lin in range(num_vert - 1)]
+        # lower digonal
+        col_ind = [col+shift for shift in [1, 0]
+                             for col in range(num_vert - 1)]
+        adj_matrix = csr_array((data, (row_ind, col_ind)))
+    
+        # initializing
+        super().__init__(adj_matrix)
 
     def embeddable(self):
-        r"""
-        Returns whether the graph can be embedded on the plane or not.
+        return True
 
-        If a graph can be embedded on the plane,
-        we can assign directions to edges and arcs.
+    def get_default_coin(self):
+        r"""
+        Returns the default coin name.
 
-        Notes
-        -----
-        The implementation is class-dependent.
-        We do not check the graph structure to determine whether
-        it is embeddable or not.
+        The default coin for the coined quantum walk on the
+        segment is ``'hadamard'``.
         """
-        return False
+        return 'hadamard'
 
     def arc_label(self, tail, head):
-        return _binary_search(self.adj_matrix.indices, head,
-                              start = self.adj_matrix.indptr[tail],
-                              end = self.adj_matrix.indptr[tail + 1])
+        diff = head - tail
+        if diff != 1 and diff != -1:
+            raise ValueError('Invalid arc.')
+
+        return tail*2 if diff == 1 else tail*2 - 1 
 
     def arc(self, label):
-        adj_matrix = self.adj_matrix
-        head = adj_matrix.indices[label]
-        # TODO: binary search
-        for tail in range(len(adj_matrix.indptr)):
-            if adj_matrix.indptr[tail + 1] > label:
-                break
+        tail = (label + 1)//2
+        head = tail + (-1)**(label % 2)
         return (tail, head)
 
     def next_arc(self, arc):
         # implemented only if is embeddable
-        raise AttributeError
+        try:
+            tail, head = arc
+            diff = head - tail
+            if diff != 1 and diff != -1:
+                raise ValueError('Invalid arc')
+
+            if head == 0 or head == self.number_of_vertices() - 1:
+                return (head, tail)
+            
+            return ((tail + 1, head + 1) if diff == 1
+                    else (tail - 1, head - 1))
+        except TypeError:
+            if arc == 1:
+                return 0
+            num_arcs = self.number_of_arcs() 
+            if arc == num_arcs - 2:
+                return num_arcs - 1
+            return arc + 2 if arc % 2 == 0 else arc - 2
 
     def previous_arc(self, arc):
         # implemented only if is embeddable
-        raise AttributeError
-
-    def neighbors(self, vertex):
-        start = self.adj_matrix.indptr[vertex]
-        end = self.adj_matrix.indptr[vertex + 1]
-        return self.adj_matrix.indices[start:end]
-
-    def arcs_with_tail(self, tail):
-        arcs_lim = self.adj_matrix.indptr
-        return np.arange(arcs_lim[tail], arcs_lim[tail + 1])
-
-    def number_of_vertices(self):
-        return self.adj_matrix.shape[0]
-
-    def number_of_arcs(self):
-        return self.adj_matrix.sum()
-
-    def number_of_edges(self):
-        return self.adj_matrix.sum() >> 1
-
-    def degree(self, vertex):
-        indptr = self.adj_matrix.indptr
-        return indptr[vertex + 1] - indptr[vertex]
+        try:
+            tail, head = arc
+            diff = head - tail
+            if diff != 1 and diff != -1:
+                raise ValueError('Invalid arc')
+
+            if tail == 0 or tail == self.number_of_vertices() - 1:
+                return (head, tail)
+            
+            return ((tail - 1, head - 1) if diff == 1
+                    else (tail + 1, head + 1))
+        except TypeError:
+            if arc == 0:
+                return 1
+            num_arcs = self.number_of_arcs() 
+            if arc == num_arcs - 1:
+                return num_arcs - 2
+            return arc - 2 if arc % 2 == 0 else arc + 2
```

### Comparing `hiperwalk-2.0a1/hiperwalk/graph/lattice.py` & `hiperwalk-2.0a2/hiperwalk/graph/lattice.py`

 * *Files 10% similar despite different names*

```diff
@@ -96,22 +96,89 @@
         self.periodic = periodic
         self.diagonal = diagonal
 
     def embeddable(self):
         return True
 
     def vertex_coordinates(self, label):
+        r"""
+        Returns vertex (x, y)-coordinates given its label.
+
+        Parameters
+        ----------
+        label : int
+            Vertex label.
+
+        Returns
+        -------
+        x : int
+            Vertex X-coordinate.
+        y : int
+            Vertex Y-coordinate.
+
+        See Also
+        --------
+        vertex_label
+        """
         return (label % self.x_dim, label // self.x_dim)
 
 
     def vertex_label(self, x, y):
+        r"""
+        Returns vertex label (number) given its coordinates.
+
+        Parameters
+        ----------
+        x : int
+            Vertex X-coordinate.
+        y : int
+            Vertex Y-coordinate.
+
+        Returns
+        -------
+        int
+            Vertex label.
+
+        See Also
+        --------
+        vertex_coordinates
+        """
         return (x + self.x_dim*y) % self.number_of_vertices()
 
     def arc_direction(self, arc):
         r"""
+        Return arc direction.
+
+        Parameters
+        ----------
+        arc
+            Any of the following notations are acceptable.
+            
+            * ((int, int), (int, int))
+                Arc notation with vertices' coordinates.
+            * (int, int)
+                Arc notation with vertices' labels.
+            * int
+                Arc label.
+
+        Returns
+        -------
+        int
+            If natural (not diagonal) lattice:
+                * 0: right
+                * 1: left
+                * 2: up
+                * 3: down
+
+            If diagonal lattice:
+                * 0: right, up
+                * 1: right, down
+                * 2: left, up
+                * 3: left, down
+
         Notes
         -----
         Does not check if arc exists.
         """
         # dealing with coordinates
         try:
             tail, head = arc
@@ -165,14 +232,37 @@
         sub_y = (1 if ((tail // self.x_dim == 0
                         or tail // self.x_dim == self.x_dim - 1)
                        and direction > 2)
                  else 0)
         return label + direction - sub_x - sub_y
 
     def arc(self, label, coordinates=True):
+        r"""
+        Arc in arc notation.
+
+        Given the arc label, returns it in the ``(tail, head)`` notation.
+
+        Parameters
+        ----------
+        label : int
+            Arc label (number)
+        coordinates : bool, default=True
+            Whether the vertices are returned as coordinates or as labels.
+
+        Returns
+        -------
+        (tail, head)
+            There are two possibile formats for the vertices
+            ``tail`` and ``head``.
+
+            (vertex_x, vertex_y) : (int, int)
+                If ``coordinates=True``.
+            label : int
+                If ``coordinates=False``.
+        """
         if not self.periodic and self.diagonal:
             raise NotImplementedError
 
         if self.periodic:
             tail = label // 4
             coin = label % 4
             num_vert = self.number_of_vertices()
@@ -336,26 +426,34 @@
             head = self.vertex_label(head[0], head[1])
 
         if not arc_iterable:
             return self.arc_label(tail, head)
         return (tail, head)
 
     def dimensions(self):
+        r"""
+        Lattice dimensions.
+
+        Returns
+        -------
+        x_dim : int
+            Dimension alongside de X axis.
+        y_dim : int
+            Dimension alongside de Y axis.
+        """
         return (self.x_dim, self.y_dim)
 
     def get_central_vertex(self):
         r"""
         Central vertex is different from center vertex.
         In the sense that...
         """
         warn('`get_central_vertex` is deprecated. '
-             + 'Use `central_vertex` instead.',
+             + 'It will be removed in version 2.1.',
              DeprecationWarning)
-        return self.central_vertex()
 
-    def central_vertex(self):
         if self.x_dim % 2 != 1 or self.y_dim % 2 != 1:
             raise ValueError(
                 "One of lattice dimensions is even. "
                 + "Hence it does not have a single central vertex."
             )
         return np.array([self.x_dim // 2, self.y_dim // 2])
```

### Comparing `hiperwalk-2.0a1/hiperwalk/plot/_animation.py` & `hiperwalk-2.0a2/hiperwalk/plot/_animation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """
 Encapsules Animation class, responsible for managing animations.
 """
 
 import matplotlib.pyplot as plt
 from PIL import Image
 from .._constants import __DEBUG__
-from warnings import warn
 
 if __DEBUG__:
     from time import time
     start = time()
 
 class Animation:
     """
@@ -100,16 +99,14 @@
         # and not showing for any animations
         def update_figure(img):
             ax.imshow(img)
 
             if __DEBUG__:
                 global start
                 end = time()
-                print('update_figure: ' + str(end - start) + 's')
-                print('\t' + str(img))
                 start = end
 
         # TODO: repeat_delay not implemented in animation.save
         self.plt_anim = FuncAnimation(
             fig, update_figure, frames=self.frames,
             interval=interval, repeat=self._is_in_notebook()
         )
@@ -121,15 +118,14 @@
         # removing axes and pads introduced by imshow,
         # i.e. shows only the original axes and pads (from plots_as_imgs)
         plt.axis('off')
         plt.tight_layout(pad=0)
         if __DEBUG__:
             # used to check if no extra padding is being added
             fig.patch.set_facecolor('red')
-            print("Fig dpi " + str(fig.dpi))
 
     # TODO: saving video is supported but not recommended because
     #   fps may not be respected.
     # ffmpeg is necessary for saving video and better quality gifs.
     # Pillow is sufficient for saving gifs,
     # although colorbar may be discretized.
     def save_animation(self, filename):
@@ -168,23 +164,17 @@
         valid_extensions = ['.gif', '.mp4']
 
         extension = filename[-4:]
         if extension not in valid_extensions:
             filename += '.gif'
         self.save_path = filename
 
-        print('--------------------------------')
-        print(self.save_path)
-        print('--------------------------------')
         self.plt_anim.save(self.save_path)
         plt.close()
 
-        if __DEBUG__:
-            print('finished saving')
-
         # by ignoring this condition while using the terminal,
         # a non-aborting exception is thrown:
         # AttributeError: 'NoneType' object has no attribute 'add_callback'.
         # The attributes deleted are needed for saving
         # html5 video in jupyter notebooks
         if not self._is_in_notebook():
             del self.plt_anim
@@ -197,17 +187,14 @@
 
     # returns None if animation is already saved.
     # Otherwise returns the temporary file
     def _save_animation_in_temp_file(self):
         if not self._is_saved():
             import tempfile
             temp = tempfile.NamedTemporaryFile(suffix='.gif')
-            print('---------------------------------')
-            print(temp.name)
-            print('---------------------------------')
             self.save_animation(temp.name)
             return temp
 
         return None
 
     def _is_in_notebook(self):
         try:
@@ -287,15 +274,15 @@
 
                 # exhibits animation in Gtk window
                 img = Gtk.Image.new()
                 img.set_from_file(self.save_path)
                 window.add(img)
 
             def configure_video_window(self):
-                warn('Showing video not supported.')
+                raise NotImplementedError('Showing video not supported.')
 
             if self.save_path[-4:] == '.gif':
                 configure_gif_window(self)
             else:
                 configure_video_window(self)
 
 
@@ -321,17 +308,14 @@
 
             if self.save_path[-4:] == '.gif':
                 configure_gif_window(self)
             else:
                 configure_video_window(self)
 
             def on_activate(app, save_path):
-                print('------------------------------')
-                print(save_path)
-                print('------------------------------')
                 win = Gtk.ApplicationWindow(application=app)
                 ############################
                 from gi.repository import GdkPixbuf
                 pixbuf = GdkPixbuf.PixbufAnimation.new_from_file(save_path)
                 img = Gtk.Image()
                 img.set_from_animation(pixbuf)
                 win.set_child(img)
```

### Comparing `hiperwalk-2.0a1/hiperwalk/plot/_plot.py` & `hiperwalk-2.0a2/hiperwalk/plot/_plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -440,16 +440,16 @@
 
     #fig, ax =_configure_figure(num_vert, fig_width, fig_height) 
     #ax = fig.add_subplot(projection='3d')
     fig, ax = plt.subplots(figsize=(fig_width, fig_height),
                            subplot_kw={"projection": "3d"})
 
     ax.tick_params(length=10, width=1, labelsize=16, pad=10)
-    ax.set_xlabel('Vertex X ID', labelpad=15, fontsize=18)
-    ax.set_ylabel('Vertex Y ID', labelpad=15, fontsize=18)
+    ax.set_xlabel('Vertex X', labelpad=15, fontsize=18)
+    ax.set_ylabel('Vertex Y', labelpad=15, fontsize=18)
     ax.set_zlabel('Probability', labelpad=30, fontsize=18)
     return fig, ax
 
 
 def _plot_probability_distribution_on_bars(
         probabilities, ax, labels=None, graph=None,
         min_prob=None, max_prob=None, **kwargs
```

### Comparing `hiperwalk-2.0a1/hiperwalk/quantum_walk/_pyneblina_interface.py` & `hiperwalk-2.0a2/hiperwalk/quantum_walk/_pyneblina_interface.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,19 +10,15 @@
 import atexit
 
 __engine_initiated = False
 
 def exit_handler():
     global __engine_initiated
     if __engine_initiated:
-        if __DEBUG__:
-            print("Stop engine")
         neblina.stop_engine()
-    elif __DEBUG__:
-        print("Engine not initiated. Not needed to stop engine.")
 
 atexit.register(exit_handler)
 ############################################
 
 # "abstract"
 class PyNeblinaObject:
     def __init__(self, nbl_obj, shape, is_complex):
@@ -101,16 +97,14 @@
             # the vector type right (i.e. real and not complex)
             neblina.vector_set(vec, i, v[i], 0)
 
     # suppose that the vector is going to be used
     # immediately after being transferred
     # TODO: check if this is the case
     neblina.move_vector_device(vec)
-    if __DEBUG__:
-        print("Type of neblina vector obj: " + str(type(vec)))
     return PyNeblinaVector(vec, is_complex, n)
 
 def retrieve_vector(pynbl_vec):
     r"""
     Retrieves vector from the device and converts it to python array.
     By default, it is supposed that the vector is not going to be used in
     other pyneblina calculations,
@@ -152,15 +146,14 @@
     TODO: isn't there a way for neblina-core to use the csr matrix directly?
       In order to avoid double memory usage
     """
     
     _init_engine()
 
     # TODO: check if complex automatically?
-    warn("Only working for square matrices")
     n = M.shape[0]
 
     # creates neblina sparse matrix structure
     # TODO: needs better support from pyneblina to
     #   use next instruction (commented).
     #   For example: neblina.sparse_matrix_set works, but in the real case,
     #   it should not be needed to pass the imaginary part as argument.
@@ -190,30 +183,27 @@
             # TODO: check if smatrix_set_real_value is beign called
             # instead of smatrix_set_complex_value
             neblina.sparse_matrix_set(smat, row, col, M[row, col], 0) 
 
     neblina.sparse_matrix_pack(smat) # TODO: is this needed?
     neblina.move_sparse_matrix_device(smat)
 
-    if __DEBUG__:
-        print("Type of neblina matrix obj: " + str(type(smat)))
-
     return PyNeblinaMatrix(smat, M.shape, is_complex, True)
 
 def _send_dense_matrix(M, is_complex):
     _init_engine()
 
     num_rows, num_cols = M.shape
     mat = (neblina.matrix_new(num_rows, num_cols, NEBLINA_COMPLEX)
            if is_complex
            else neblina.matrix_new(num_rows, num_cols, NEBLINA_FLOAT))
     
     # inserts elements into neblina matrix
-    warn("Check if there really is a difference between real and complex")
-    warn("Check if default value is zero so we can jump setting element.")
+    # TODO: Check if there really is a difference between real and complex
+    # TODO: Check if default value is zero so we can jump setting element. 
 
     for i in range(num_rows):
         for j in range(num_cols):
             neblina.matrix_set(mat, i, j, M[i, j].real, M[i, j].imag)
 
     neblina.move_matrix_device(mat)
 
@@ -239,23 +229,23 @@
     if pynbl_mat.sparse:
         raise NotImplementedError(
             "Cannot retrieve sparse matrix."
         )
 
     nbl_mat = neblina.move_matrix_host(pynbl_mat.nbl_obj)
 
-    warn("Check if using default numpy datatype.")
+    # TODO: Check if using default numpy datatype.
     py_mat = np.zeros(pynbl_mat.shape, dtype=(
         complex if pynbl_mat.is_complex else float
     ))
 
     num_rows, num_cols = pynbl_mat.shape
-    warn("Not vectorized. Implement with list comprehension. "
-         + "This may require the double memory usage. "
-         + "Check memory usage before choosing which method to use.")
+    # TODO: Not vectorized. Implement with list comprehension. 
+    #       This may require the double memory usage. 
+    #       Check memory usage before choosing which method to use.
     for i in range(num_rows):
         for j in range(num_cols):
             if pynbl_mat.is_complex:
                 py_mat[i,j] = (
                       neblina.matrix_get(nbl_mat, 2*i, 2*j)
                     + neblina.matrix_get(nbl_mat, 2*i, 2*j + 1)*1j
                 )
```

### Comparing `hiperwalk-2.0a1/hiperwalk/quantum_walk/coined_walk.py` & `hiperwalk-2.0a2/hiperwalk/quantum_walk/coined_walk.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import numpy as np
 import scipy
 import scipy.sparse
 import networkx as nx
 from .quantum_walk import QuantumWalk
-from warnings import warn
 from .._constants import __DEBUG__, PYNEBLINA_IMPORT_ERROR_MSG
 from scipy.linalg import hadamard, dft
 try:
     from . import _pyneblina_interface as nbl
 except:
     pass
 
@@ -27,18 +26,20 @@
     Parameters
     ----------
     graph
         Graph on which the quantum walk occurs.
         It can be the graph itself (:class:`hiperwalk.graph.Graph`) or
         its adjacency matrix (:class:`scipy.sparse.csr_array`).
 
-    adjacency : :class:`scipy.sparse.csr_array`
-        .. deprecated ::
+    adjacency : :class:`scipy.sparse.csr_array`, optional
+        .. deprecated:: 2.0
+            It will be removed in version 2.1.
             Use ``graph`` instead.
 
+        Use ``graph`` instead.
         Adjacency matrix of the graph.
 
     **kwargs : optional
         Optional arguments for setting the non-default evolution operator.
         See :meth:`set_evolution`.
 
     Warns
@@ -226,17 +227,14 @@
         the ``_graph`` attribute.
 
         The operator is set for future usage.
         If an evolution operator was set previously,
         it is unset for coherence.
         """
 
-        if __DEBUG__:
-            start_time = now()
-
         num_vert = self._graph.number_of_vertices()
         num_arcs = self._graph.number_of_arcs()
 
         S_cols = [self._graph.arc_label(j, i)
                   for i in range(num_vert)
                   for j in self._graph.neighbors(i)]
 
@@ -244,17 +242,14 @@
         # Note that there is only one entry per row and column
         S = scipy.sparse.csr_array(
             ( np.ones(num_arcs, dtype=np.int8),
               S_cols, np.arange(num_arcs+1) ),
             shape=(num_arcs, num_arcs)
         )
 
-        if __DEBUG__:
-            print("flipflop_shift Time: " + str(now() - start_time))
-
         self._shift = S
         self._evolution = None
 
     def has_persistent_shift(self):
         r"""
         Returns if the persistent shift operator is defined
         for the current graph.
@@ -271,32 +266,26 @@
         Create the persistent shift operator (:math:`S`) based on
         the ``_graph`` attribute.
 
         The operator is set for future usage.
         If an evolution operator was set previously,
         it is unset for coherence.
         """
-        if __DEBUG__:
-            start_time = now()
-
         num_arcs = self._graph.number_of_arcs()
 
         S_cols = [self._graph.previous_arc(i) for i in range(num_arcs)]
 
         # Using csr_array((data, indices, indptr), shape)
         # Note that there is only one entry per row and column
         S = scipy.sparse.csr_array(
             ( np.ones(num_arcs, dtype=np.int8),
               S_cols, np.arange(num_arcs+1) ),
             shape=(num_arcs, num_arcs)
         )
 
-        if __DEBUG__:
-            print("persistent shift Time: " + str(now() - start_time))
-
         self._shift = S
         self._evolution = None
 
     def set_shift(self, shift='default'):
         r"""
         Set the shift operator.
 
@@ -484,24 +473,27 @@
         -----
         Due to the chosen computational basis
         (see :class:`CoinedWalk` Notes),
         the resulting operator is a block diagonal where
         each block is the :math:`\deg(v)`-dimensional ``coin``.
         Consequently, there are :math:`|V|` blocks.
 
+        .. todo::
+
+            Check if explicit coin is valid.
+
         """
         try:
             if len(coin.shape) != 2:
                 raise TypeError('Explicit coin is not a matrix.')
 
             # explicit coin
             if not scipy.sparse.issparse(coin):
                 coin = scipy.sparse.csr_array(coin)
 
-            warn('TODO: Check if coin is valid')
             self._coin = coin
             self._evolution = None
             return
 
         except AttributeError:
             pass
 
@@ -842,14 +834,25 @@
         If the coin operator was set as an explicit matrix,
         the marked vertices to not alter it.
         If the coin operator was not set as an explicit matrix
         (e.g. as a list of coins),
         the coin of each marked vertex is substituted as specified by
         the last :meth:`set_marked` call.
 
+        Notes
+        -----
+
+        .. todo::
+            * Sparse matrix multipliation is not supported yet.
+              Converting all matrices to dense.
+              Then converting back to sparse.
+              This uses unnecessary memory and computational time.
+            * Check if matrix is sparse in pynelibna interface
+            * Check if matrices are deleted from memory and GPU.
+
         References
         ----------
         .. [1] Portugal, Renato. "Quantum walks and search algorithms".
             Vol. 19. New York: Springer, 2013.
 
         Examples
         --------
@@ -860,41 +863,31 @@
         if self._evolution is not None:
             # evolution operator was not changed.
             # No need to create it again
             return self._evolution
 
         U = None
         if hpc and not self._pyneblina_imported():
-            warn(PYNEBLINA_IMPORT_ERROR_MSG)
             hpc = False
 
 
         S = self.get_shift()
         C = self.get_coin()
 
         if hpc:
 
-            warn(
-                "Sparse matrix multipliation is not supported yet. "
-                + "Converting all matrices to dense. "
-                + "Then converting back to sparse. "
-                + "This uses unnecessary memory and computational time."
-            )
             S = S.todense()
             C = C.todense()
 
-            warn("CHECK IF MATRIX IS SPARSE IN PYNELIBNA INTERFACE")
             nbl_S = nbl.send_matrix(S)
             del S
             nbl_C = nbl.send_matrix(C)
             del C
             nbl_C = nbl.multiply_matrices(nbl_S, nbl_C)
 
-            warn("Check if matrices are deleted "
-                          + "from memory and GPU.")
             del nbl_S
 
             U = nbl.retrieve_matrix(nbl_C)
             del nbl_C
             U = scipy.sparse.csr_array(U)
 
         else:
@@ -957,17 +950,14 @@
                                   states[i], 
                                   graph.arcs_with_tail(v)
                               )
                           ).sum()
                           for v in range(num_vert)]
                         for i in range(len(states))])
 
-        if __DEBUG__:
-            end = now()
-            print("probability_distribution: " + str(end - start) + 's')
         # TODO: benchmark (time and memory usage)
         return prob
 
     def state(self, *args):
         """
         Generates a valid state.
```

### Comparing `hiperwalk-2.0a1/hiperwalk/quantum_walk/continuous_walk.py` & `hiperwalk-2.0a2/hiperwalk/quantum_walk/continuous_walk.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import numpy as np
 import scipy.sparse
 import scipy.linalg
 from .quantum_walk import QuantumWalk
 from .._constants import PYNEBLINA_IMPORT_ERROR_MSG
-from warnings import warn
 try:
     from . import _pyneblina_interface as nbl
 except:
     pass
 
 class ContinuousWalk(QuantumWalk):
     r"""
@@ -24,23 +23,17 @@
 
         :class:`hiperwalk.graph.Graph` :
             The graph itself.
 
         :class:`class:scipy.sparse.csr_array`:
             The graph adjacency matrix.
 
-        .. todo::
-            * Accept other types such as numpy array
-
-
-
-    adjacency : :class:`scipy.sparse.csr_array`
-        .. deprecated ::
-            This parameter is deprecated and will be removed in
-            future versions.
+    adjacency : :class:`scipy.sparse.csr_array`, optional
+        .. deprecated:: 2.0
+            It will be removed in version 2.1.
             Use ``graph`` instead.
 
         Adjacency matrix of the graph on which the quantum occurs
         is going to occur.
 
     **kwargs : optional
         Arguments for setting Hamiltonian.
@@ -176,14 +169,21 @@
         self._hamiltonian = H
         # since the hamiltonian was changed,
         # the previous evolution operator may not be coherent.
         self._evolution_operator = None
         return H
 
     def get_hamiltonian(self):
+        r"""
+        Returns Hamiltonian.
+
+        Returns
+        -------
+        :class:`scipy.sparse.csr_array`
+        """
         return self._hamiltonian
 
     def set_evolution(self, **kwargs):
         r"""
         Alias for :meth:`set_hamiltonian`.
         """
         self.set_hamiltonian(**kwargs)
@@ -224,25 +224,31 @@
         .. math::
             U = e^{-\text{i}tH}
 
         where :math:`H` is a Hamiltonian matrix, and
         :math:`t` is the time.
 
         The evolution operator is constructed by Taylor Series expansion.
+
+        .. warning::
+            For floating time (not integer),
+            the result is approximated. It is recommended to
+             choose a small time interval and performing
+             multiple matrix multiplications to
+             mitigate uounding errors.
         """
         if time is None or time < 0:
             raise ValueError(
                 "Expected non-negative `time` value."
             )
 
         if self._hamiltonian is None:
             raise AssertionError
 
         if hpc and not self._pyneblina_imported():
-            warn(PYNEBLINA_IMPORT_ERROR_MSG)
             hpc = False
 
         if hpc:
             # determining the number of terms in power series
             max_val = np.max(np.abs(self._hamiltonian))
             if max_val*time <= 1:
                 nbl_U = nbl.matrix_power_series(
@@ -257,18 +263,14 @@
                     new_time = 1
                     num_mult = time - 1
                 else:
                     new_time = max_val*time
                     order = np.ceil(np.math.log(new_time, 20))
                     new_time /= 10**order
                     num_mult = int(np.round(time/new_time)) - 1
-                    warn("Result is approximated. It is recommended to "
-                         + "choose a small time interval and performing "
-                         + "multiple matrix multiplications to "
-                         + "mitigate uounding errors.")
 
                 new_nbl_U = nbl.matrix_power_series(
                         -1j*new_time*self._hamiltonian, 20)
                 nbl_U = nbl.multiply_matrices(new_nbl_U, new_nbl_U)
                 for i in range(num_mult - 1):
                     nbl_U = nbl.multiply_matrices(nbl_U, new_nbl_U)
```

### Comparing `hiperwalk-2.0a1/hiperwalk/quantum_walk/quantum_walk.py` & `hiperwalk-2.0a2/hiperwalk/quantum_walk/quantum_walk.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,17 +21,20 @@
     Parameters
     ----------
     graph
         Graph on which the quantum walk occurs.
         It can be the graph itself (:class:`hiperwalk.graph.Graph`) or
         its adjacency matrix (:class:`scipy.sparse.csr_array`).
 
-    adjacency : optional
+    adjacency : :class:`scipy.sparse.csr_array`, optional
+        .. deprecated:: 2.0
+            It will be removed in version 2.1.
+            Use ``graph`` instead.
+
         The adjacency matrix.
-        It is deprecated. Use ``graph`` instead.
 
     Attributes
     ----------
     hilb_dim : int, default=0
         Hilbert Space dimension.
         It must be updated by the subclass' ``__init__``.
 
@@ -45,15 +48,16 @@
         if ``adj_matrix`` is not an instance of
         :class:`scipy.sparse.csr_array`.
 
     Notes
     -----
 
     .. todo::
-        The following methods must be overwritten.
+        * List the that methods must be overwritten.
+        * Accept other types as ``graph`` such as numpy array
 
     """
 
     @abstractmethod
     def __init__(self, graph=None, adjacency=None, **kwargs):
         if adjacency is not None:
             if graph is None:
@@ -439,69 +443,51 @@
             )
 
         ###########################
         ### Auxiliary functions ###
         ###########################
 
         def __prepare_engine(self):
-            if __DEBUG__:
-                print("Preparing engine")
-
             if hpc:
                 self._simul_mat = nbl.send_matrix(self._evolution)
                 self._simul_vec = nbl.send_vector(initial_condition)
 
             else:
                 self._simul_mat = self._evolution
                 self._simul_vec = initial_condition
 
-            if __DEBUG__:
-                print("Done\n")
-
         def __simulate_step(self, step):
             """
             Apply the simulation evolution operator ``step`` times
             to the simulation vector.
             Simulation vector is then updated.
             """
-            if __DEBUG__:
-                print("Simulating steps")
-
             if hpc:
                 # TODO: request multiple multiplications at once
                 #       to neblina-core
                 # TODO: check if intermediate states are being freed
                 for i in range(step):
                     self._simul_vec = nbl.multiply_matrix_vector(
                         self._simul_mat, self._simul_vec)
             else:
                 for i in range(step):
                     self._simul_vec = self._simul_mat @ self._simul_vec
 
                 # TODO: compare with numpy.linalg.matrix_power
 
-            if __DEBUG__:
-                print("Done\n")
-
         def __save_simul_vec(self):
-            if __DEBUG__:
-                print("Saving simulated vec")
-
             ret = None
 
             if hpc:
                 # TODO: check if vector must be deleted or
                 #       if it can be reused via neblina-core commands.
                 ret = nbl.retrieve_vector(self._simul_vec)
             else:
                 ret = self._simul_vec
 
-            if __DEBUG__:
-                print("Done\n")
-
             return ret
 
 
         ###############################
         ### simulate implemantation ###
         ###############################
 
@@ -512,17 +498,14 @@
         if not np.all([e.is_integer() for e in time]):
             raise ValueError("`time` has non-int entry.")
 
         start, end, step = time
 
         
         if hpc and not self._pyneblina_imported():
-            if __DEBUG__:
-                print("IMPORTING PYNEBLINA")
-            warn(PYNEBLINA_IMPORT_ERROR_MSG)
             hpc = False
 
         __prepare_engine(self)
 
         # number of states to save
         num_states = int(end/step) + 1
         num_states -= (int((start - 1)/step) + 1) if start > 0 else 0
```

### Comparing `hiperwalk-2.0a1/tests/unitary/coined_cycle.py` & `hiperwalk-2.0a2/tests/unitary/coined_cycle.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a1/tests/unitary/coined_line.py` & `hiperwalk-2.0a2/tests/unitary/coined_line.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a1/tests/unitary/coined_segment.py` & `hiperwalk-2.0a2/tests/unitary/coined_segment.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a1/tests/unitary/continuous_graph.py` & `hiperwalk-2.0a2/tests/unitary/continuous_graph.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a1/.gitignore` & `hiperwalk-2.0a2/.gitignore`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a1/LICENSE` & `hiperwalk-2.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a1/README.md` & `hiperwalk-2.0a2/README.md`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a1/pyproject.toml` & `hiperwalk-2.0a2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "hiperwalk"
-version = "2.0a1"
+version = "2.0a2"
 description = "High-Performance Quantum Walk Simulator"
 license = {file="LICENSE"}
 readme = "README.md"
 authors = [
   { name="Gustavo Bezerra", email="gbezerra@posgrad.lncc.br" },
   { name="Paulo Motta", email="prmottajr@gmail.com" },
   { name="Renato Portugal", email="portugal@lncc.br" },
```

### Comparing `hiperwalk-2.0a1/PKG-INFO` & `hiperwalk-2.0a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hiperwalk
-Version: 2.0a1
+Version: 2.0a2
 Summary: High-Performance Quantum Walk Simulator
 Project-URL: homepage, http://qubit.lncc.br/qwalk/
 Project-URL: documentation, https://hiperwalk.readthedocs.io/
 Project-URL: source, https://github.com/hiperwalk/hiperwalk
 Author-email: Gustavo Bezerra <gbezerra@posgrad.lncc.br>, Paulo Motta <prmottajr@gmail.com>, Renato Portugal <portugal@lncc.br>
 Maintainer-email: Hiperwalk Organization <hiperwalk@gmail.com>
 License: GNU Lesser General Public License
```

