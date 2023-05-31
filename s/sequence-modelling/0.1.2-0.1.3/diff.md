# Comparing `tmp/sequence_modelling-0.1.2.tar.gz` & `tmp/sequence_modelling-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sequence_modelling-0.1.2.tar", max compression
+gzip compressed data, was "sequence_modelling-0.1.3.tar", max compression
```

## Comparing `sequence_modelling-0.1.2.tar` & `sequence_modelling-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1500 2023-05-10 14:10:44.782212 sequence_modelling-0.1.2/LICENSE
--rw-r--r--   0        0        0     2083 2023-05-10 14:10:44.782212 sequence_modelling-0.1.2/README.md
--rw-r--r--   0        0        0      842 2023-05-10 14:10:44.782212 sequence_modelling-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     9876 2023-05-10 14:10:44.782212 sequence_modelling-0.1.2/src/sequence_modelling/DiscreteOptim.py
--rw-r--r--   0        0        0        0 2023-05-10 14:10:44.782212 sequence_modelling-0.1.2/src/sequence_modelling/__init__.py
--rw-r--r--   0        0        0     5924 2023-05-10 14:10:44.782212 sequence_modelling-0.1.2/src/sequence_modelling/emissionplus.py
--rw-r--r--   0        0        0     5215 2023-05-10 14:10:44.782212 sequence_modelling-0.1.2/src/sequence_modelling/emmissions.py
--rw-r--r--   0        0        0    18459 2023-05-10 14:10:44.782212 sequence_modelling-0.1.2/src/sequence_modelling/hmm.py
--rw-r--r--   0        0        0     5939 2023-05-10 14:10:44.782212 sequence_modelling-0.1.2/src/sequence_modelling/hmmviz.py
--rw-r--r--   0        0        0    14727 2023-05-10 14:10:44.782212 sequence_modelling-0.1.2/src/sequence_modelling/qdhmm.py
--rw-r--r--   0        0        0    11882 2023-05-10 14:10:44.782212 sequence_modelling-0.1.2/src/sequence_modelling/qdhmm_logscaled.py
--rw-r--r--   0        0        0     1538 2023-05-10 14:10:44.782212 sequence_modelling-0.1.2/src/sequence_modelling/utils.py
--rw-r--r--   0        0        0     2807 1970-01-01 00:00:00.000000 sequence_modelling-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1500 2023-05-31 11:57:22.882421 sequence_modelling-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2306 2023-05-31 11:57:22.882421 sequence_modelling-0.1.3/README.md
+-rw-r--r--   0        0        0      841 2023-05-31 11:57:22.882421 sequence_modelling-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     9871 2023-05-31 11:57:22.882421 sequence_modelling-0.1.3/src/sequence_modelling/DiscreteOptim.py
+-rw-r--r--   0        0        0        0 2023-05-31 11:57:22.882421 sequence_modelling-0.1.3/src/sequence_modelling/__init__.py
+-rw-r--r--   0        0        0     5887 2023-05-31 11:57:22.882421 sequence_modelling-0.1.3/src/sequence_modelling/emissionplus.py
+-rw-r--r--   0        0        0     5211 2023-05-31 11:57:22.882421 sequence_modelling-0.1.3/src/sequence_modelling/emmissions.py
+-rw-r--r--   0        0        0    18426 2023-05-31 11:57:22.882421 sequence_modelling-0.1.3/src/sequence_modelling/hmm.py
+-rw-r--r--   0        0        0     5900 2023-05-31 11:57:22.886421 sequence_modelling-0.1.3/src/sequence_modelling/hmmviz.py
+-rw-r--r--   0        0        0    14709 2023-05-31 11:57:22.886421 sequence_modelling-0.1.3/src/sequence_modelling/qdhmm.py
+-rw-r--r--   0        0        0    11895 2023-05-31 11:57:22.886421 sequence_modelling-0.1.3/src/sequence_modelling/qdhmm_logscaled.py
+-rw-r--r--   0        0        0     1531 2023-05-31 11:57:22.886421 sequence_modelling-0.1.3/src/sequence_modelling/utils.py
+-rw-r--r--   0        0        0     2987 1970-01-01 00:00:00.000000 sequence_modelling-0.1.3/PKG-INFO
```

### Comparing `sequence_modelling-0.1.2/LICENSE` & `sequence_modelling-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sequence_modelling-0.1.2/README.md` & `sequence_modelling-0.1.3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-[![tests](https://github.com/nbhushan/Quasi-Deterministic-HMMs/actions/workflows/app-test.yml/badge.svg?branch=master)](https://github.com/nbhushan/Quasi-Deterministic-HMMs/actions/workflows/app-test.yml) [![docs](https://github.com/nbhushan/Quasi-Deterministic-HMMs/actions/workflows/docs-pages.yaml/badge.svg?branch=master)](https://github.com/nbhushan/Quasi-Deterministic-HMMs/actions/workflows/docs-pages.yaml) 
+[![tests](https://github.com/nbhushan/Quasi-Deterministic-HMMs/actions/workflows/app-test.yml/badge.svg?branch=master)](https://github.com/nbhushan/Quasi-Deterministic-HMMs/actions/workflows/app-test.yml) [![docs](https://github.com/nbhushan/Quasi-Deterministic-HMMs/actions/workflows/docs-pages.yaml/badge.svg?branch=master)](https://github.com/nbhushan/Quasi-Deterministic-HMMs/actions/workflows/docs-pages.yaml) [![build](https://github.com/nbhushan/sequence-modelling/actions/workflows/build-publish.yml/badge.svg?branch=master)](https://github.com/nbhushan/sequence-modelling/actions/workflows/build-publish.yml)
 
 # sequence-modelling
 
 Numerically optimized time-series and sequence modelling in Python.
 
 ## Key features
 
 - Hidden Markov Models and Quasi-Deterministic Hidden Markov Models
 - Numerically stable: floating point arithmetic performed in log space to avoid underflow
 - Easy to use (based on the scikit-learn API)
 - Pure Python and Numpy based
 - Open source and commercially usable (BSD license)
-- Support for discrete and continuous emissions
+- Support for discrete and continuous (Gaussian) emissions
 
 ## Installation
 
 The easiest way to install sequence-modelling is using pip:
 
 ```python
    pip install sequence-modelling
@@ -26,37 +26,38 @@
 ```python
 
    import numpy as np
    from sequence_modelling.emmissions import Gaussian
    from sequence_modelling.hmm import StandardHMM
    import sequence_modelling.hmmviz as plt
 
-   # Build a 2-state HMM model with one-dimensional Gaussian emissions
+   # define a 2-state HMM estimator with one-dimensional Gaussian emissions
 
    # the transition matrix
    A = np.array([[0.6, 0.4],
                  [0.3, 0.7],
                  [0.5, 0.5]])
 
    # the emission object
    O = Gaussian(mu=np.array([[-100.0, 100.0]]),
              covar=np.array([[[10.0]], [[10.0]]]))
 
-   # Build the HMM model object
+   # build the HMM model object
    hmm = StandardHMM(A, O)
 
-   # Sample 1000 observations from the generative model
+   # sample 100 observations from the generative model
    obs, path = hmm.sample(dim=1, N=100)
 
-    # Fit the model to the data
-   likelihood, ll, duration, rankn, res = hmm.hmmFit([obs])
+    # fit the model to the data
+   likelihood, ll, duration, rankn, res = hmm.fit([obs])
 
-   # Decode (Predict) the most likely state sequence using the Viterbi algorithm
+   # decode (predict) the most likely state sequence using the Viterbi algorithm
    decoded_path = hmm.viterbi(obs)
 
-   # Visualize the state sequence
+   # visualize the decoded state sequence
    from matplotlib.pyplot import figure, show
    fa = figure()
    plt.view_viterbi(fa.add_subplot(1, 1, 1), [obs], [decoded_path], hmm.O.mu, seq=0)
    fa.tight_layout()
    show()
+
 ```
```

### Comparing `sequence_modelling-0.1.2/pyproject.toml` & `sequence_modelling-0.1.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 [tool.poetry]
 name = "sequence_modelling"
-version = "0.1.2"
+version = "0.1.3"
 description = "sequence modelling using HMMs"
 authors = ["Nitin Bhushan <bhushan.nitin@posteo.net>"]
 readme = "README.md"
 license = "BSD-2-Clause"
 
 
 [tool.poetry.dependencies]
 python = "3.9.*"
 numpy = "^1.24.2"
 scipy = "^1.10.1"
-pre-commit = "^3.1.1"
 Sphinx = { version = "4.2.0", optional = true }
 sphinx-rtd-theme = { version = "1.0.0", optional = true }
 sphinxcontrib-napoleon = { version = "0.7", optional = true }
 
-
 [tool.poetry.group.dev.dependencies]
 matplotlib = "^3.7.0"
 2to3 = "^1.0"
 pep8 = "^1.7.1"
 mypy = "^0.910"
 seaborn = "^0.11.2"
 pep8-naming = "^0.12.1"
 pytest = "^7.2.1"
 unittest2 = "^1.1.0"
+pre-commit = "^3.1.1"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `sequence_modelling-0.1.2/src/sequence_modelling/DiscreteOptim.py` & `sequence_modelling-0.1.3/src/sequence_modelling/DiscreteOptim.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # -*- coding: utf-8 -*-
 """
-Created on Mon Aug 19 17:16:56 2013
+Optimization methods for QDHMM
 
 @author: nbhushan
-"""
 
+"""
 
-import numpy as np
 import random
 import itertools
+import numpy as np
 
 
 def objective(taus, K, obs, weights):
     """Objective function
 
     The objective function is essentially the weighted average of
     the variance along the splits.
```

### Comparing `sequence_modelling-0.1.2/src/sequence_modelling/emissionplus.py` & `sequence_modelling-0.1.3/src/sequence_modelling/emissionplus.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # -*- coding: utf-8 -*-
 """
-Created on Thu May 30 16:49:58 2013
+Emission distributions for QDHMM
 
 @author: nbhushan
+
 """
 
+import time
+import pdb
+
 import numpy as np
 from scipy.stats import norm
 
-# from scipy.optimize import anneal
-import time
 import sequence_modelling.DiscreteOptim as optim
 import sequence_modelling.hmmviz as viz
-import pdb
 
 
 class Gaussian:
     """The Gaussian emission model for a QDHMM.
 
     Attributes
     ----------
```

### Comparing `sequence_modelling-0.1.2/src/sequence_modelling/emmissions.py` & `sequence_modelling-0.1.3/src/sequence_modelling/emmissions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 """
-Created on Tue Apr 23 12:02:37 2013
+Emission distributions for HMM
 
 @author: nbhushan
+
 """
 
 import numpy as np
 from sequence_modelling.utils import logsumexp
 from scipy.stats import norm
```

### Comparing `sequence_modelling-0.1.2/src/sequence_modelling/hmm.py` & `sequence_modelling-0.1.3/src/sequence_modelling/hmm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 # -*- coding: utf-8 -*-
 """
-Created on Tue Apr 23 12:04:01 2013
+The HMM class
 
 @author: nbhushan
+
 """
 
+import logging, sys, time, pdb
 import numpy as np
-import logging, sys
 from sequence_modelling.utils import logsumexp
-import time
-import pdb
 
 # set up the logger
 logger = logging.getLogger(__name__)
 hdlr = logging.StreamHandler(sys.stderr)
 logger.addHandler(hdlr)
 logger.setLevel(logging.INFO)
```

### Comparing `sequence_modelling-0.1.2/src/sequence_modelling/hmmviz.py` & `sequence_modelling-0.1.3/src/sequence_modelling/hmmviz.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 """
-Created on Tue Apr 23 12:04:01 2013
+Visualization utils
 
 @author: nbhushan
 
 """
 
 import numpy as np
 
@@ -32,16 +32,16 @@
         ax.plot(
             r[t],
             v * np.ones((t.sum(),), float),
             ".",
             label="State {0}: {1:g}".format(k, v),
         )
     ax.set_title("Viterbi State sequence; seq : " + str(seq))
-    ax.set_xlabel("time (s)")
-    ax.set_ylabel("Power (W)")
+    ax.set_xlabel("time")
+    ax.set_ylabel("obs")
     ax.legend(prop=dict(size="xx-small"))
 
 
 def view_postduration(ax, obs, path, mean, reslist, ranknlist, seq):
     """Visualize the estimated state durations based on the posterior
     distribution.
     """
@@ -63,16 +63,16 @@
             r[t],
             v * np.ones((t.sum(),), float),
             ".",
             c=clr[::-1][k],
             label="State {0}: {1:g}".format(k, v),
         )
     ax.set_title("HMM State duration estimation, seq :" + str(seq))
-    ax.set_xlabel("time ")
-    ax.set_ylabel("Power (W)")
+    ax.set_xlabel("time")
+    ax.set_ylabel("obs")
     ax.legend(prop=dict(size="xx-small"))
     for k in range(1, len(m) - 1):
         c = np.argsort(rankn[k])
         for label, x, z in zip(
             np.char.mod("%.2f", res[k][c]),
             rankn[k][c] + 1,
             [mean.flatten()[k]] * res.shape[1],
@@ -114,15 +114,15 @@
     z = ksi[:, 0, 1]
     z_min, z_max = -np.abs(z).max(), np.abs(z).max()
     az.pcolor(x[:-1], x[:-1], z, cmap="RdBu", vmin=z_min, vmax=z_max)
     # az.pcolor(x[:-1], y[:-1], z, cmap='RdBu', vmin=z_min, vmax=z_max)
     az.colorbar()
     # az.plot(ksi[:,0, 1]*500, label = "Active to Idle")
     # az.plot(ksi[:,1, 2]*100, label = "Idle to Sleep")
-    az.set_ylabel("Power (W)")
+    az.set_ylabel("obs")
     az.set_title("Posterior probability of transitions from Active to Idle ")
     az.legend()
     show()
 
 
 def view_statedurations(fc, path, K):
     """View histograms of state duration.
```

### Comparing `sequence_modelling-0.1.2/src/sequence_modelling/qdhmm.py` & `sequence_modelling-0.1.3/src/sequence_modelling/qdhmm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 """
-Created on Thu May 30 15:38:44 2013
+The QDHMM object
 
 @author: nbhushan
+
 """
 
 import numpy as np
 from scipy import sparse
 import logging, sys
 import time
```

### Comparing `sequence_modelling-0.1.2/src/sequence_modelling/qdhmm_logscaled.py` & `sequence_modelling-0.1.3/src/sequence_modelling/qdhmm_logscaled.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 """
-Created on Thu May 30 15:38:44 2013
+QDHMM in logscale to deal with numerical issues
 
 @author: nbhushan
+
 """
 
 import numpy as np
 from sequence_modelling.utils import logsumexp
 from scipy import sparse
 import matplotlib.pyplot as plt
 import logging, sys
```

### Comparing `sequence_modelling-0.1.2/src/sequence_modelling/utils.py` & `sequence_modelling-0.1.3/src/sequence_modelling/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 """
-Created on Tue Jun 11 16:26:49 2013
+Numerical stability helpers
 
 @author: nbhushan
+
 """
 import numpy as np
 
 
 def logsumexp(a, axis=None):
     """Compute the log of the sum of exponentials of input elements,
        Modified scipy.misc logsumexp to accept [-inf,-inf].
```

### Comparing `sequence_modelling-0.1.2/PKG-INFO` & `sequence_modelling-0.1.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,40 @@
 Metadata-Version: 2.1
 Name: sequence-modelling
-Version: 0.1.2
+Version: 0.1.3
 Summary: sequence modelling using HMMs
 License: BSD-2-Clause
 Author: Nitin Bhushan
 Author-email: bhushan.nitin@posteo.net
 Requires-Python: >=3.9.0,<3.10.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: docs
 Requires-Dist: Sphinx (==4.2.0) ; extra == "docs"
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
-Requires-Dist: pre-commit (>=3.1.1,<4.0.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Requires-Dist: sphinx-rtd-theme (==1.0.0) ; extra == "docs"
 Requires-Dist: sphinxcontrib-napoleon (==0.7) ; extra == "docs"
 Description-Content-Type: text/markdown
 
-[![tests](https://github.com/nbhushan/Quasi-Deterministic-HMMs/actions/workflows/app-test.yml/badge.svg?branch=master)](https://github.com/nbhushan/Quasi-Deterministic-HMMs/actions/workflows/app-test.yml) [![docs](https://github.com/nbhushan/Quasi-Deterministic-HMMs/actions/workflows/docs-pages.yaml/badge.svg?branch=master)](https://github.com/nbhushan/Quasi-Deterministic-HMMs/actions/workflows/docs-pages.yaml) 
+[![tests](https://github.com/nbhushan/Quasi-Deterministic-HMMs/actions/workflows/app-test.yml/badge.svg?branch=master)](https://github.com/nbhushan/Quasi-Deterministic-HMMs/actions/workflows/app-test.yml) [![docs](https://github.com/nbhushan/Quasi-Deterministic-HMMs/actions/workflows/docs-pages.yaml/badge.svg?branch=master)](https://github.com/nbhushan/Quasi-Deterministic-HMMs/actions/workflows/docs-pages.yaml) [![build](https://github.com/nbhushan/sequence-modelling/actions/workflows/build-publish.yml/badge.svg?branch=master)](https://github.com/nbhushan/sequence-modelling/actions/workflows/build-publish.yml)
 
 # sequence-modelling
 
 Numerically optimized time-series and sequence modelling in Python.
 
 ## Key features
 
 - Hidden Markov Models and Quasi-Deterministic Hidden Markov Models
 - Numerically stable: floating point arithmetic performed in log space to avoid underflow
 - Easy to use (based on the scikit-learn API)
 - Pure Python and Numpy based
 - Open source and commercially usable (BSD license)
-- Support for discrete and continuous emissions
+- Support for discrete and continuous (Gaussian) emissions
 
 ## Installation
 
 The easiest way to install sequence-modelling is using pip:
 
 ```python
    pip install sequence-modelling
@@ -46,38 +45,39 @@
 ```python
 
    import numpy as np
    from sequence_modelling.emmissions import Gaussian
    from sequence_modelling.hmm import StandardHMM
    import sequence_modelling.hmmviz as plt
 
-   # Build a 2-state HMM model with one-dimensional Gaussian emissions
+   # define a 2-state HMM estimator with one-dimensional Gaussian emissions
 
    # the transition matrix
    A = np.array([[0.6, 0.4],
                  [0.3, 0.7],
                  [0.5, 0.5]])
 
    # the emission object
    O = Gaussian(mu=np.array([[-100.0, 100.0]]),
              covar=np.array([[[10.0]], [[10.0]]]))
 
-   # Build the HMM model object
+   # build the HMM model object
    hmm = StandardHMM(A, O)
 
-   # Sample 1000 observations from the generative model
+   # sample 100 observations from the generative model
    obs, path = hmm.sample(dim=1, N=100)
 
-    # Fit the model to the data
-   likelihood, ll, duration, rankn, res = hmm.hmmFit([obs])
+    # fit the model to the data
+   likelihood, ll, duration, rankn, res = hmm.fit([obs])
 
-   # Decode (Predict) the most likely state sequence using the Viterbi algorithm
+   # decode (predict) the most likely state sequence using the Viterbi algorithm
    decoded_path = hmm.viterbi(obs)
 
-   # Visualize the state sequence
+   # visualize the decoded state sequence
    from matplotlib.pyplot import figure, show
    fa = figure()
    plt.view_viterbi(fa.add_subplot(1, 1, 1), [obs], [decoded_path], hmm.O.mu, seq=0)
    fa.tight_layout()
    show()
+
 ```
```

