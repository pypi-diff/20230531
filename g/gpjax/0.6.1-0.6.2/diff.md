# Comparing `tmp/gpjax-0.6.1.tar.gz` & `tmp/gpjax-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpjax-0.6.1.tar", max compression
+gzip compressed data, was "gpjax-0.6.2.tar", max compression
```

## Comparing `gpjax-0.6.1.tar` & `gpjax-0.6.2.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0    11357 2023-05-11 20:54:48.036528 gpjax-0.6.1/LICENSE
--rw-r--r--   0        0        0     7200 2023-05-11 21:57:19.191138 gpjax-0.6.1/README.md
--rw-r--r--   0        0        0     2900 2023-05-11 21:33:47.126581 gpjax-0.6.1/gpjax/__init__.py
--rw-r--r--   0        0        0     1068 2023-05-11 21:33:47.126847 gpjax-0.6.1/gpjax/base/__init__.py
--rw-r--r--   0        0        0    12470 2023-05-11 21:33:47.126989 gpjax-0.6.1/gpjax/base/module.py
--rw-r--r--   0        0        0     2254 2023-05-11 21:33:47.127060 gpjax-0.6.1/gpjax/base/param.py
--rw-r--r--   0        0        0     3452 2023-05-11 21:33:47.127136 gpjax-0.6.1/gpjax/dataset.py
--rw-r--r--   0        0        0     8119 2023-05-11 21:33:47.127221 gpjax-0.6.1/gpjax/fit.py
--rw-r--r--   0        0        0     9121 2023-05-11 21:33:47.127395 gpjax-0.6.1/gpjax/gaussian_distribution.py
--rw-r--r--   0        0        0    28181 2023-05-11 21:33:47.127606 gpjax-0.6.1/gpjax/gps.py
--rw-r--r--   0        0        0     1815 2023-05-11 21:33:47.127892 gpjax-0.6.1/gpjax/kernels/__init__.py
--rw-r--r--   0        0        0       68 2023-05-11 21:33:47.128020 gpjax-0.6.1/gpjax/kernels/approximations/__init__.py
--rw-r--r--   0        0        0     3183 2023-05-11 21:33:47.128137 gpjax-0.6.1/gpjax/kernels/approximations/rff.py
--rw-r--r--   0        0        0     6680 2023-05-11 21:33:47.128282 gpjax-0.6.1/gpjax/kernels/base.py
--rw-r--r--   0        0        0     1379 2023-05-11 21:33:47.128558 gpjax-0.6.1/gpjax/kernels/computations/__init__.py
--rw-r--r--   0        0        0     2585 2023-05-11 21:33:47.128682 gpjax-0.6.1/gpjax/kernels/computations/base.py
--rw-r--r--   0        0        0     2478 2023-05-11 21:33:47.128816 gpjax-0.6.1/gpjax/kernels/computations/basis_functions.py
--rw-r--r--   0        0        0     2830 2023-05-11 21:33:47.128972 gpjax-0.6.1/gpjax/kernels/computations/constant_diagonal.py
--rw-r--r--   0        0        0     1661 2023-05-11 21:33:47.129071 gpjax-0.6.1/gpjax/kernels/computations/dense.py
--rw-r--r--   0        0        0     2383 2023-05-11 21:33:47.129171 gpjax-0.6.1/gpjax/kernels/computations/diagonal.py
--rw-r--r--   0        0        0     2165 2023-05-11 21:33:47.129303 gpjax-0.6.1/gpjax/kernels/computations/eigen.py
--rw-r--r--   0        0        0      790 2023-05-11 21:33:47.129595 gpjax-0.6.1/gpjax/kernels/non_euclidean/__init__.py
--rw-r--r--   0        0        0     3511 2023-05-11 21:33:47.129716 gpjax-0.6.1/gpjax/kernels/non_euclidean/graph.py
--rw-r--r--   0        0        0     1620 2023-05-11 21:33:47.129829 gpjax-0.6.1/gpjax/kernels/non_euclidean/utils.py
--rw-r--r--   0        0        0      930 2023-05-11 21:33:47.130081 gpjax-0.6.1/gpjax/kernels/nonstationary/__init__.py
--rw-r--r--   0        0        0     4078 2023-05-11 21:33:47.130162 gpjax-0.6.1/gpjax/kernels/nonstationary/arccosine.py
--rw-r--r--   0        0        0     2016 2023-05-11 21:33:47.130277 gpjax-0.6.1/gpjax/kernels/nonstationary/linear.py
--rw-r--r--   0        0        0     2384 2023-05-11 21:33:47.130397 gpjax-0.6.1/gpjax/kernels/nonstationary/polynomial.py
--rw-r--r--   0        0        0     1323 2023-05-11 21:33:47.130534 gpjax-0.6.1/gpjax/kernels/stationary/__init__.py
--rw-r--r--   0        0        0     2521 2023-05-11 21:33:47.130681 gpjax-0.6.1/gpjax/kernels/stationary/matern12.py
--rw-r--r--   0        0        0     2723 2023-05-11 21:33:47.130817 gpjax-0.6.1/gpjax/kernels/stationary/matern32.py
--rw-r--r--   0        0        0     2792 2023-05-11 21:33:47.130923 gpjax-0.6.1/gpjax/kernels/stationary/matern52.py
--rw-r--r--   0        0        0     2420 2023-05-11 21:33:47.131037 gpjax-0.6.1/gpjax/kernels/stationary/periodic.py
--rw-r--r--   0        0        0     2500 2023-05-11 21:33:47.131171 gpjax-0.6.1/gpjax/kernels/stationary/powered_exponential.py
--rw-r--r--   0        0        0     2389 2023-05-11 21:33:47.131312 gpjax-0.6.1/gpjax/kernels/stationary/rational_quadratic.py
--rw-r--r--   0        0        0     2440 2023-05-11 21:33:47.131400 gpjax-0.6.1/gpjax/kernels/stationary/rbf.py
--rw-r--r--   0        0        0     2226 2023-05-11 21:33:47.131522 gpjax-0.6.1/gpjax/kernels/stationary/utils.py
--rw-r--r--   0        0        0     2072 2023-05-11 21:33:47.131675 gpjax-0.6.1/gpjax/kernels/stationary/white.py
--rw-r--r--   0        0        0     6643 2023-05-11 21:33:47.131830 gpjax-0.6.1/gpjax/likelihoods.py
--rw-r--r--   0        0        0     1609 2023-05-11 21:33:47.132130 gpjax-0.6.1/gpjax/linops/__init__.py
--rw-r--r--   0        0        0     6259 2023-05-11 21:33:47.132259 gpjax-0.6.1/gpjax/linops/constant_diagonal_linear_operator.py
--rw-r--r--   0        0        0     6201 2023-05-11 21:33:47.132389 gpjax-0.6.1/gpjax/linops/dense_linear_operator.py
--rw-r--r--   0        0        0     7179 2023-05-11 21:33:47.132536 gpjax-0.6.1/gpjax/linops/diagonal_linear_operator.py
--rw-r--r--   0        0        0     3607 2023-05-11 21:33:47.132958 gpjax-0.6.1/gpjax/linops/identity_linear_operator.py
--rw-r--r--   0        0        0     7131 2023-05-11 21:33:47.133134 gpjax-0.6.1/gpjax/linops/linear_operator.py
--rw-r--r--   0        0        0     3187 2023-05-11 21:33:47.133506 gpjax-0.6.1/gpjax/linops/triangular_linear_operator.py
--rw-r--r--   0        0        0     3443 2023-05-11 21:33:47.133703 gpjax-0.6.1/gpjax/linops/utils.py
--rw-r--r--   0        0        0     5939 2023-05-11 21:33:47.133915 gpjax-0.6.1/gpjax/linops/zero_linear_operator.py
--rw-r--r--   0        0        0     6081 2023-05-11 21:33:47.134064 gpjax-0.6.1/gpjax/mean_functions.py
--rw-r--r--   0        0        0    15061 2023-05-11 21:33:47.134196 gpjax-0.6.1/gpjax/objectives.py
--rw-r--r--   0        0        0     4407 2023-05-11 21:33:47.134282 gpjax-0.6.1/gpjax/progress_bar.py
--rw-r--r--   0        0        0     2172 2023-05-11 21:33:47.134433 gpjax-0.6.1/gpjax/quadrature.py
--rw-r--r--   0        0        0     5506 2023-05-11 21:33:47.134686 gpjax-0.6.1/gpjax/scan.py
--rw-r--r--   0        0        0     1694 2023-05-11 21:33:47.134827 gpjax-0.6.1/gpjax/typing.py
--rw-r--r--   0        0        0    26453 2023-05-11 21:33:47.135024 gpjax-0.6.1/gpjax/variational_families.py
--rw-r--r--   0        0        0     4953 2023-05-11 22:04:51.774103 gpjax-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     8498 1970-01-01 00:00:00.000000 gpjax-0.6.1/setup.py
--rw-r--r--   0        0        0     8376 1970-01-01 00:00:00.000000 gpjax-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-30 19:04:23.359578 gpjax-0.6.2/LICENSE
+-rw-r--r--   0        0        0     7472 2023-05-30 19:04:23.359790 gpjax-0.6.2/README.md
+-rw-r--r--   0        0        0     2900 2023-05-30 19:04:23.413721 gpjax-0.6.2/gpjax/__init__.py
+-rw-r--r--   0        0        0     1068 2023-05-30 19:04:23.413913 gpjax-0.6.2/gpjax/base/__init__.py
+-rw-r--r--   0        0        0    12487 2023-05-31 18:33:09.977313 gpjax-0.6.2/gpjax/base/module.py
+-rw-r--r--   0        0        0     2271 2023-05-30 19:04:23.414167 gpjax-0.6.2/gpjax/base/param.py
+-rw-r--r--   0        0        0     3452 2023-05-30 19:04:23.414269 gpjax-0.6.2/gpjax/dataset.py
+-rw-r--r--   0        0        0     8136 2023-05-30 19:04:23.414379 gpjax-0.6.2/gpjax/fit.py
+-rw-r--r--   0        0        0     9121 2023-05-30 19:04:23.414517 gpjax-0.6.2/gpjax/gaussian_distribution.py
+-rw-r--r--   0        0        0    28150 2023-05-31 18:33:09.978443 gpjax-0.6.2/gpjax/gps.py
+-rw-r--r--   0        0        0     1815 2023-05-30 19:04:23.414985 gpjax-0.6.2/gpjax/kernels/__init__.py
+-rw-r--r--   0        0        0       68 2023-05-30 19:04:23.415113 gpjax-0.6.2/gpjax/kernels/approximations/__init__.py
+-rw-r--r--   0        0        0     3183 2023-05-30 19:04:23.415213 gpjax-0.6.2/gpjax/kernels/approximations/rff.py
+-rw-r--r--   0        0        0     6680 2023-05-30 19:04:23.415334 gpjax-0.6.2/gpjax/kernels/base.py
+-rw-r--r--   0        0        0     1379 2023-05-30 19:04:23.415474 gpjax-0.6.2/gpjax/kernels/computations/__init__.py
+-rw-r--r--   0        0        0     2585 2023-05-30 19:04:23.415588 gpjax-0.6.2/gpjax/kernels/computations/base.py
+-rw-r--r--   0        0        0     2478 2023-05-30 19:04:23.415673 gpjax-0.6.2/gpjax/kernels/computations/basis_functions.py
+-rw-r--r--   0        0        0     2830 2023-05-30 19:04:23.415758 gpjax-0.6.2/gpjax/kernels/computations/constant_diagonal.py
+-rw-r--r--   0        0        0     1661 2023-05-30 19:04:23.415841 gpjax-0.6.2/gpjax/kernels/computations/dense.py
+-rw-r--r--   0        0        0     2383 2023-05-30 19:04:23.415926 gpjax-0.6.2/gpjax/kernels/computations/diagonal.py
+-rw-r--r--   0        0        0     2165 2023-05-30 19:04:23.416024 gpjax-0.6.2/gpjax/kernels/computations/eigen.py
+-rw-r--r--   0        0        0      790 2023-05-30 19:04:23.416154 gpjax-0.6.2/gpjax/kernels/non_euclidean/__init__.py
+-rw-r--r--   0        0        0     3511 2023-05-30 19:04:23.416256 gpjax-0.6.2/gpjax/kernels/non_euclidean/graph.py
+-rw-r--r--   0        0        0     1620 2023-05-30 19:04:23.416342 gpjax-0.6.2/gpjax/kernels/non_euclidean/utils.py
+-rw-r--r--   0        0        0      930 2023-05-30 19:04:23.416456 gpjax-0.6.2/gpjax/kernels/nonstationary/__init__.py
+-rw-r--r--   0        0        0     4078 2023-05-30 19:04:23.416567 gpjax-0.6.2/gpjax/kernels/nonstationary/arccosine.py
+-rw-r--r--   0        0        0     2016 2023-05-30 19:04:23.416675 gpjax-0.6.2/gpjax/kernels/nonstationary/linear.py
+-rw-r--r--   0        0        0     2384 2023-05-30 19:04:23.416805 gpjax-0.6.2/gpjax/kernels/nonstationary/polynomial.py
+-rw-r--r--   0        0        0     1323 2023-05-30 19:04:23.416936 gpjax-0.6.2/gpjax/kernels/stationary/__init__.py
+-rw-r--r--   0        0        0     2521 2023-05-30 19:04:23.417037 gpjax-0.6.2/gpjax/kernels/stationary/matern12.py
+-rw-r--r--   0        0        0     2723 2023-05-30 19:04:23.417110 gpjax-0.6.2/gpjax/kernels/stationary/matern32.py
+-rw-r--r--   0        0        0     2792 2023-05-30 19:04:23.417181 gpjax-0.6.2/gpjax/kernels/stationary/matern52.py
+-rw-r--r--   0        0        0     2420 2023-05-30 19:04:23.417272 gpjax-0.6.2/gpjax/kernels/stationary/periodic.py
+-rw-r--r--   0        0        0     2677 2023-05-31 18:33:09.978838 gpjax-0.6.2/gpjax/kernels/stationary/powered_exponential.py
+-rw-r--r--   0        0        0     2389 2023-05-30 19:04:23.417470 gpjax-0.6.2/gpjax/kernels/stationary/rational_quadratic.py
+-rw-r--r--   0        0        0     2440 2023-05-30 19:04:23.417547 gpjax-0.6.2/gpjax/kernels/stationary/rbf.py
+-rw-r--r--   0        0        0     2226 2023-05-30 19:04:23.417639 gpjax-0.6.2/gpjax/kernels/stationary/utils.py
+-rw-r--r--   0        0        0     2072 2023-05-30 19:04:23.417729 gpjax-0.6.2/gpjax/kernels/stationary/white.py
+-rw-r--r--   0        0        0     6691 2023-05-31 18:33:09.979251 gpjax-0.6.2/gpjax/likelihoods.py
+-rw-r--r--   0        0        0     1609 2023-05-30 19:04:23.417969 gpjax-0.6.2/gpjax/linops/__init__.py
+-rw-r--r--   0        0        0     6259 2023-05-30 19:04:23.418078 gpjax-0.6.2/gpjax/linops/constant_diagonal_linear_operator.py
+-rw-r--r--   0        0        0     6201 2023-05-30 19:04:23.418223 gpjax-0.6.2/gpjax/linops/dense_linear_operator.py
+-rw-r--r--   0        0        0     7179 2023-05-30 19:04:23.418329 gpjax-0.6.2/gpjax/linops/diagonal_linear_operator.py
+-rw-r--r--   0        0        0     3607 2023-05-30 19:04:23.418426 gpjax-0.6.2/gpjax/linops/identity_linear_operator.py
+-rw-r--r--   0        0        0     7131 2023-05-30 19:04:23.418534 gpjax-0.6.2/gpjax/linops/linear_operator.py
+-rw-r--r--   0        0        0     3187 2023-05-30 19:04:23.418674 gpjax-0.6.2/gpjax/linops/triangular_linear_operator.py
+-rw-r--r--   0        0        0     3443 2023-05-30 19:04:23.418772 gpjax-0.6.2/gpjax/linops/utils.py
+-rw-r--r--   0        0        0     5939 2023-05-30 19:04:23.418880 gpjax-0.6.2/gpjax/linops/zero_linear_operator.py
+-rw-r--r--   0        0        0     6081 2023-05-30 19:04:23.418977 gpjax-0.6.2/gpjax/mean_functions.py
+-rw-r--r--   0        0        0    15061 2023-05-31 18:33:09.980049 gpjax-0.6.2/gpjax/objectives.py
+-rw-r--r--   0        0        0     4407 2023-05-30 19:04:23.419266 gpjax-0.6.2/gpjax/progress_bar.py
+-rw-r--r--   0        0        0     2172 2023-05-31 18:33:09.980179 gpjax-0.6.2/gpjax/quadrature.py
+-rw-r--r--   0        0        0     5506 2023-05-30 19:04:23.419458 gpjax-0.6.2/gpjax/scan.py
+-rw-r--r--   0        0        0     1694 2023-05-30 19:04:23.419555 gpjax-0.6.2/gpjax/typing.py
+-rw-r--r--   0        0        0    26453 2023-05-30 19:04:23.419787 gpjax-0.6.2/gpjax/variational_families.py
+-rw-r--r--   0        0        0     4952 2023-05-31 18:35:21.371134 gpjax-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     8773 1970-01-01 00:00:00.000000 gpjax-0.6.2/setup.py
+-rw-r--r--   0        0        0     8647 1970-01-01 00:00:00.000000 gpjax-0.6.2/PKG-INFO
```

### Comparing `gpjax-0.6.1/LICENSE` & `gpjax-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.1/README.md` & `gpjax-0.6.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 <h2 align='center'>Gaussian processes in Jax.</h2> -->
 <p align="center">
 <img width="700" height="300" src="https://raw.githubusercontent.com/JaxGaussianProcesses/GPJax/main/docs/_static/gpjax_logo.svg" alt="GPJax's logo">
 </p>
 
 [![codecov](https://codecov.io/gh/JaxGaussianProcesses/GPJax/branch/master/graph/badge.svg?token=DM1DRDASU2)](https://codecov.io/gh/JaxGaussianProcesses/GPJax)
 [![CodeFactor](https://www.codefactor.io/repository/github/jaxgaussianprocesses/gpjax/badge)](https://www.codefactor.io/repository/github/jaxgaussianprocesses/gpjax)
-[![Documentation Status](https://readthedocs.org/projects/gpjax/badge/?version=latest)](https://gpjax.readthedocs.io/en/latest/?badge=latest)
+[![Netlify Status](https://api.netlify.com/api/v1/badges/d3950e6f-321f-4508-9e52-426b5dae2715/deploy-status)](https://app.netlify.com/sites/endearing-crepe-c2d5fe/deploys)
 [![PyPI version](https://badge.fury.io/py/GPJax.svg)](https://badge.fury.io/py/GPJax)
 [![DOI](https://joss.theoj.org/papers/10.21105/joss.04455/status.svg)](https://doi.org/10.21105/joss.04455)
 [![Downloads](https://pepy.tech/badge/gpjax)](https://pepy.tech/project/gpjax)
 [![Slack Invite](https://img.shields.io/badge/Slack_Invite--blue?style=social&logo=slack)](https://join.slack.com/t/gpjax/shared_invite/zt-1da57pmjn-rdBCVg9kApirEEn2E5Q2Zw)
 
 [**Quickstart**](#simple-example)
 | [**Install guide**](#installation)
-| [**Documentation**](https://gpjax.readthedocs.io/en/latest/)
+| [**Documentation**](https://docs.jaxgaussianprocesses.com/)
 | [**Slack Community**](https://join.slack.com/t/gpjax/shared_invite/zt-1da57pmjn-rdBCVg9kApirEEn2E5Q2Zw)
 
 GPJax aims to provide a low-level interface to Gaussian process (GP) models in
 [Jax](https://github.com/google/jax), structured to give researchers maximum
 flexibility in extending the code to suit their own needs. The idea is that the
 code should be as close as possible to the maths we write on paper when working
 with GP models.
@@ -44,28 +44,31 @@
 where we can discuss the development of GPJax and broader support for Gaussian
 process modelling.
 
 # Supported methods and interfaces
 
 ## Notebook examples
 
-> - [**Conjugate Inference**](https://gpjax.readthedocs.io/en/latest/examples/regression.html)
-> - [**Classification with MCMC**](https://gpjax.readthedocs.io/en/latest/examples/classification.html)
-> - [**Sparse Variational Inference**](https://gpjax.readthedocs.io/en/latest/examples/uncollapsed_vi.html)
-> - [**BlackJax Integration**](https://gpjax.readthedocs.io/en/latest/examples/classification.html)
-> - [**Laplace Approximation**](https://gpjax.readthedocs.io/en/latest/examples/classification.html#Laplace-approximation)
-> - [**Inference on Non-Euclidean Spaces**](https://gpjax.readthedocs.io/en/latest/examples/kernels.html#Custom-Kernel)
-> - [**Inference on Graphs**](https://gpjax.readthedocs.io/en/latest/examples/graph_kernels.html)
-> - [**Learning Gaussian Process Barycentres**](https://gpjax.readthedocs.io/en/latest/examples/barycentres.html)
-> - [**Deep Kernel Regression**](https://gpjax.readthedocs.io/en/latest/examples/haiku.html)
+> - [**Conjugate Inference**](https://docs.jaxgaussianprocesses.com/examples/regression/)
+> - [**Classification with MCMC**](https://docs.jaxgaussianprocesses.com/examples/classification/)
+> - [**Sparse Variational Inference**](https://docs.jaxgaussianprocesses.com/examples/collapsed_vi/)
+> - [**Stochastic Variational Inference**](https://docs.jaxgaussianprocesses.com/examples/uncollapsed_vi/)
+> - [**BlackJax Integration**](https://docs.jaxgaussianprocesses.com/examples/classification/#mcmc-inference)
+> - [**Laplace Approximation**](https://docs.jaxgaussianprocesses.com/examples/classification/#laplace-approximation)
+> - [**Inference on Non-Euclidean Spaces**](https://docs.jaxgaussianprocesses.com/examples/kernels/#custom-kernel)
+> - [**Inference on Graphs**](https://docs.jaxgaussianprocesses.com/examples/graph_kernels/)
+> - [**Pathwise Sampling**](https://docs.jaxgaussianprocesses.com/examples/spatial/)
+> - [**Learning Gaussian Process Barycentres**](https://docs.jaxgaussianprocesses.com/examples/barycentres/)
+> - [**Deep Kernel Regression**](https://docs.jaxgaussianprocesses.com/examples/deep_kernels/)
+> - [**Poisson Regression**](https://docs.jaxgaussianprocesses.com/examples/poisson/)
 
 ## Guides for customisation
 >
-> - [**Custom kernels**](https://gpjax.readthedocs.io/en/latest/examples/kernels.html#Custom-Kernel)
-> - [**UCI regression**](https://gpjax.readthedocs.io/en/latest/examples/yacht.html)
+> - [**Custom kernels**](https://docs.jaxgaussianprocesses.com/examples/kernels/#custom-kernel)
+> - [**UCI regression**](https://docs.jaxgaussianprocesses.com/examples/yacht/)
 
 ## Conversion between `.ipynb` and `.py`
 Above examples are stored in [examples](examples) directory in the double
 percent (`py:percent`) format. Checkout [jupytext
 using-cli](https://jupytext.readthedocs.io/en/latest/using-cli.html) for more
 info.
 
@@ -160,36 +163,36 @@
 
 
 ## Development version
 > **Warning**
 >
 > This version is possibly unstable and may contain bugs.
 
-Clone a copy of the repository to your local machine and run the setup
-configuration in development mode.
-```bash
-git clone https://github.com/JaxGaussianProcesses/GPJax.git
-cd GPJax
-poetry install
-```
-
 > **Note**
 >
 > We advise you create virtual environment before installing:
 > ```
 > conda create -n gpjax_experimental python=3.10.0
 > conda activate gpjax_experimental
 >  ```
 >
 > and recommend you check your installation passes the supplied unit tests:
 >
 > ```python
 > poetry run pytest
 > ```
 
+Clone a copy of the repository to your local machine and run the setup
+configuration in development mode.
+```bash
+git clone https://github.com/JaxGaussianProcesses/GPJax.git
+cd GPJax
+poetry install
+```
+
 # Citing GPJax
 
 If you use GPJax in your research, please cite our [JOSS paper](https://joss.theoj.org/papers/10.21105/joss.04455#).
 
 ```
 @article{Pinder2022,
   doi = {10.21105/joss.04455},
```

### Comparing `gpjax-0.6.1/gpjax/__init__.py` & `gpjax-0.6.2/gpjax/__init__.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.1/gpjax/base/__init__.py` & `gpjax-0.6.2/gpjax/base/__init__.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 from gpjax.base.module import (
     Module,
     load_tree,
     meta,
     meta_flatten,
     meta_leaves,
     meta_map,
-    static_field,
     save_tree,
+    static_field,
 )
 from gpjax.base.param import param_field
 
 __all__ = [
     "Module",
     "meta_leaves",
     "meta_flatten",
```

### Comparing `gpjax-0.6.1/gpjax/base/module.py` & `gpjax-0.6.2/gpjax/base/module.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 )
 from simple_pytree import Pytree
 import tensorflow_probability.substrates.jax.bijectors as tfb
 
 Self = TypeVar("Self")
 
 
-def static_field(
+def static_field(  # noqa: PLR0913
     default: Any = dataclasses.MISSING,
     *,
     default_factory: Any = dataclasses.MISSING,
     init: bool = True,
     repr: bool = True,
     hash: Optional[bool] = None,
     compare: bool = True,
```

### Comparing `gpjax-0.6.1/gpjax/base/param.py` & `gpjax-0.6.2/gpjax/base/param.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     Any,
     Mapping,
     Optional,
 )
 import tensorflow_probability.substrates.jax.bijectors as tfb
 
 
-def param_field(
+def param_field(  # noqa: PLR0913
     default: Any = dataclasses.MISSING,
     *,
     bijector: Optional[tfb.Bijector] = None,
     trainable: bool = True,
     default_factory: Any = dataclasses.MISSING,
     init: bool = True,
     repr: bool = True,
```

### Comparing `gpjax-0.6.1/gpjax/dataset.py` & `gpjax-0.6.2/gpjax/dataset.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.1/gpjax/fit.py` & `gpjax-0.6.2/gpjax/fit.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 from gpjax.typing import (
     Array,
     KeyArray,
     ScalarFloat,
 )
 
 
-def fit(
+def fit(  # noqa: PLR0913
     *,
     model: Module,
     objective: Union[AbstractObjective, Callable[[Module, Dataset], ScalarFloat]],
     train_data: Dataset,
     optim: ox.GradientTransformation,
     key: KeyArray,
     num_iters: Optional[int] = 100,
```

### Comparing `gpjax-0.6.1/gpjax/gaussian_distribution.py` & `gpjax-0.6.2/gpjax/gaussian_distribution.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.1/gpjax/gps.py` & `gpjax-0.6.2/gpjax/gps.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,16 +108,16 @@
 # GP Priors
 #######################
 @dataclass
 class Prior(AbstractPrior):
     r"""A Gaussian process prior object.
 
     The GP is parameterised by a
-    [mean](https://gpjax.readthedocs.io/en/latest/api.html#module-gpjax.mean_functions)
-    and [kernel](https://gpjax.readthedocs.io/en/latest/api.html#module-gpjax.kernels)
+    [mean](https://docs.jaxgaussianprocesses.com/api/mean_functions/)
+    and [kernel](https://docs.jaxgaussianprocesses.com/api/kernels/base/)
     function.
 
     A Gaussian process prior parameterised by a mean function $`m(\cdot)`$ and a kernel
     function $`k(\cdot, \cdot)`$ is given by
     $`p(f(\cdot)) = \mathcal{GP}(m(\cdot), k(\cdot, \cdot))`$.
 
     To invoke a `Prior` distribution, only a kernel function is required. By
```

### Comparing `gpjax-0.6.1/gpjax/kernels/__init__.py` & `gpjax-0.6.2/gpjax/kernels/__init__.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.1/gpjax/kernels/approximations/rff.py` & `gpjax-0.6.2/gpjax/kernels/approximations/rff.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.1/gpjax/kernels/base.py` & `gpjax-0.6.2/gpjax/kernels/base.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.1/gpjax/kernels/computations/__init__.py` & `gpjax-0.6.2/gpjax/kernels/computations/__init__.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.1/gpjax/kernels/computations/base.py` & `gpjax-0.6.2/gpjax/kernels/computations/base.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.1/gpjax/kernels/computations/basis_functions.py` & `gpjax-0.6.2/gpjax/kernels/computations/basis_functions.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.1/gpjax/kernels/computations/constant_diagonal.py` & `gpjax-0.6.2/gpjax/kernels/computations/constant_diagonal.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.1/gpjax/kernels/computations/dense.py` & `gpjax-0.6.2/gpjax/kernels/computations/dense.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.1/gpjax/kernels/computations/diagonal.py` & `gpjax-0.6.2/gpjax/kernels/computations/diagonal.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.1/gpjax/kernels/computations/eigen.py` & `gpjax-0.6.2/gpjax/kernels/computations/eigen.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.1/gpjax/kernels/non_euclidean/__init__.py` & `gpjax-0.6.2/gpjax/kernels/non_euclidean/__init__.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.1/gpjax/kernels/non_euclidean/graph.py` & `gpjax-0.6.2/gpjax/kernels/non_euclidean/graph.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.1/gpjax/kernels/non_euclidean/utils.py` & `gpjax-0.6.2/gpjax/kernels/non_euclidean/utils.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.1/gpjax/kernels/nonstationary/__init__.py` & `gpjax-0.6.2/gpjax/kernels/nonstationary/__init__.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.1/gpjax/kernels/nonstationary/arccosine.py` & `gpjax-0.6.2/gpjax/kernels/nonstationary/arccosine.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.1/gpjax/kernels/nonstationary/linear.py` & `gpjax-0.6.2/gpjax/kernels/nonstationary/linear.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.1/gpjax/kernels/nonstationary/polynomial.py` & `gpjax-0.6.2/gpjax/kernels/nonstationary/polynomial.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.1/gpjax/kernels/stationary/__init__.py` & `gpjax-0.6.2/gpjax/kernels/stationary/__init__.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.1/gpjax/kernels/stationary/matern12.py` & `gpjax-0.6.2/gpjax/kernels/stationary/matern12.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.1/gpjax/kernels/stationary/matern32.py` & `gpjax-0.6.2/gpjax/kernels/stationary/matern32.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.1/gpjax/kernels/stationary/matern52.py` & `gpjax-0.6.2/gpjax/kernels/stationary/matern52.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.1/gpjax/kernels/stationary/periodic.py` & `gpjax-0.6.2/gpjax/kernels/stationary/periodic.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.1/gpjax/kernels/stationary/powered_exponential.py` & `gpjax-0.6.2/gpjax/kernels/stationary/powered_exponential.py`

 * *Files 15% similar despite different names*

```diff
@@ -27,25 +27,27 @@
     Array,
     ScalarFloat,
 )
 
 
 @dataclass
 class PoweredExponential(AbstractKernel):
-    r"""The powered exponential family of kernels.
+    r"""The powered exponential family of kernels. This also equivalent to the symmetric generalized normal distribution.
 
-    Key reference is Diggle and Ribeiro (2007) - "Model-based Geostatistics".
+    See Diggle and Ribeiro (2007) - "Model-based Geostatistics".
+    and   
+    https://en.wikipedia.org/wiki/Generalized_normal_distribution#Symmetric_version
 
     """
 
     lengthscale: Union[ScalarFloat, Float[Array, " D"]] = param_field(
         jnp.array(1.0), bijector=tfb.Softplus()
     )
     variance: ScalarFloat = param_field(jnp.array(1.0), bijector=tfb.Softplus())
-    power: ScalarFloat = param_field(jnp.array(1.0))
+    power: ScalarFloat = param_field(jnp.array(1.0), bijector=tfb.Sigmoid())
     name: str = "Powered Exponential"
 
     def __call__(self, x: Float[Array, " D"], y: Float[Array, " D"]) -> ScalarFloat:
         r"""Compute the Powered Exponential kernel between a pair of arrays.
 
         Evaluate the kernel on a pair of inputs $`(x, y)`$ with length-scale parameter
         $`\ell`$, $`\sigma`$ and power $`\kappa`$.
```

### Comparing `gpjax-0.6.1/gpjax/kernels/stationary/rational_quadratic.py` & `gpjax-0.6.2/gpjax/kernels/stationary/rational_quadratic.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.1/gpjax/kernels/stationary/rbf.py` & `gpjax-0.6.2/gpjax/kernels/stationary/rbf.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.1/gpjax/kernels/stationary/utils.py` & `gpjax-0.6.2/gpjax/kernels/stationary/utils.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.1/gpjax/kernels/stationary/white.py` & `gpjax-0.6.2/gpjax/kernels/stationary/white.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.1/gpjax/likelihoods.py` & `gpjax-0.6.2/gpjax/likelihoods.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,43 +46,46 @@
     num_datapoints: int = static_field()
 
     def __call__(self, *args: Any, **kwargs: Any) -> tfd.Distribution:
         r"""Evaluate the likelihood function at a given predictive distribution.
 
         Args:
             *args (Any): Arguments to be passed to the likelihood's `predict` method.
-            **kwargs (Any): Keyword arguments to be passed to the likelihood's `predict` method.
+            **kwargs (Any): Keyword arguments to be passed to the likelihood's
+                `predict` method.
 
         Returns
         -------
             tfd.Distribution: The predictive distribution.
         """
         return self.predict(*args, **kwargs)
 
     @abc.abstractmethod
     def predict(self, *args: Any, **kwargs: Any) -> tfd.Distribution:
         r"""Evaluate the likelihood function at a given predictive distribution.
 
         Args:
             *args (Any): Arguments to be passed to the likelihood's `predict` method.
-            **kwargs (Any): Keyword arguments to be passed to the likelihood's `predict` method.
+            **kwargs (Any): Keyword arguments to be passed to the likelihood's
+                `predict` method.
 
         Returns
         -------
             tfd.Distribution: The predictive distribution.
         """
         raise NotImplementedError
 
     @abc.abstractmethod
     def link_function(self, f: Float[Array, "..."]) -> tfd.Distribution:
         r"""Return the link function of the likelihood function.
 
         Returns
         -------
-            tfd.Distribution: The distribution of observations, y, given values of the Gaussian process, f.
+            tfd.Distribution: The distribution of observations, y, given values of the
+                Gaussian process, f.
         """
         raise NotImplementedError
 
 
 @dataclass
 class Gaussian(AbstractLikelihood):
     r"""Gaussian likelihood object."""
```

### Comparing `gpjax-0.6.1/gpjax/linops/__init__.py` & `gpjax-0.6.2/gpjax/linops/__init__.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.1/gpjax/linops/constant_diagonal_linear_operator.py` & `gpjax-0.6.2/gpjax/linops/constant_diagonal_linear_operator.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.1/gpjax/linops/dense_linear_operator.py` & `gpjax-0.6.2/gpjax/linops/dense_linear_operator.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.1/gpjax/linops/diagonal_linear_operator.py` & `gpjax-0.6.2/gpjax/linops/diagonal_linear_operator.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.1/gpjax/linops/identity_linear_operator.py` & `gpjax-0.6.2/gpjax/linops/identity_linear_operator.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.1/gpjax/linops/linear_operator.py` & `gpjax-0.6.2/gpjax/linops/linear_operator.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.1/gpjax/linops/triangular_linear_operator.py` & `gpjax-0.6.2/gpjax/linops/triangular_linear_operator.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.1/gpjax/linops/utils.py` & `gpjax-0.6.2/gpjax/linops/utils.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.1/gpjax/linops/zero_linear_operator.py` & `gpjax-0.6.2/gpjax/linops/zero_linear_operator.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.1/gpjax/mean_functions.py` & `gpjax-0.6.2/gpjax/mean_functions.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.1/gpjax/objectives.py` & `gpjax-0.6.2/gpjax/objectives.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.1/gpjax/progress_bar.py` & `gpjax-0.6.2/gpjax/progress_bar.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.1/gpjax/quadrature.py` & `gpjax-0.6.2/gpjax/quadrature.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.1/gpjax/scan.py` & `gpjax-0.6.2/gpjax/scan.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.1/gpjax/typing.py` & `gpjax-0.6.2/gpjax/typing.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.1/gpjax/variational_families.py` & `gpjax-0.6.2/gpjax/variational_families.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.1/pyproject.toml` & `gpjax-0.6.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "gpjax"
-version = "0.6.1" # Merely a placeholder, will be replaced by the dynamic versioning plugin
+version = "0.6.2" # Merely a placeholder, will be replaced by the dynamic versioning plugin
 description = "Gaussian processes in JAX."
 authors = ["Thomas Pinder <tompinder@live.co.uk>", "Daniel Dodd <daniel_dodd@icloud.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/JaxGaussianProcesses/GPJax"
 repository = "https://github.com/JaxGaussianProcesses/GPJax"
 include = [
     "LICENSE",
 ]
-documentation = "https://gpjax.readthedocs.io/en/latest/"
+documentation = "https://docs.jaxgaussianprocesses.com/"
 keywords = ["gaussian-processes jax machine-learning bayesian"]
 packages = [{include = "gpjax"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 jax = ">=0.4.1"
 optax = "^0.1.4"
```

### Comparing `gpjax-0.6.1/setup.py` & `gpjax-0.6.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -24,17 +24,17 @@
  'orbax-checkpoint>=0.2.0,<0.3.0',
  'simple-pytree>=0.1.7,<0.2.0',
  'tensorflow-probability>=0.19.0,<0.20.0',
  'tqdm>=4.65.0,<5.0.0']
 
 setup_kwargs = {
     'name': 'gpjax',
-    'version': '0.6.1',
+    'version': '0.6.2',
     'description': 'Gaussian processes in JAX.',
-    'long_description': '<!-- <h1 align=\'center\'>GPJax</h1>\n<h2 align=\'center\'>Gaussian processes in Jax.</h2> -->\n<p align="center">\n<img width="700" height="300" src="https://raw.githubusercontent.com/JaxGaussianProcesses/GPJax/main/docs/_static/gpjax_logo.svg" alt="GPJax\'s logo">\n</p>\n\n[![codecov](https://codecov.io/gh/JaxGaussianProcesses/GPJax/branch/master/graph/badge.svg?token=DM1DRDASU2)](https://codecov.io/gh/JaxGaussianProcesses/GPJax)\n[![CodeFactor](https://www.codefactor.io/repository/github/jaxgaussianprocesses/gpjax/badge)](https://www.codefactor.io/repository/github/jaxgaussianprocesses/gpjax)\n[![Documentation Status](https://readthedocs.org/projects/gpjax/badge/?version=latest)](https://gpjax.readthedocs.io/en/latest/?badge=latest)\n[![PyPI version](https://badge.fury.io/py/GPJax.svg)](https://badge.fury.io/py/GPJax)\n[![DOI](https://joss.theoj.org/papers/10.21105/joss.04455/status.svg)](https://doi.org/10.21105/joss.04455)\n[![Downloads](https://pepy.tech/badge/gpjax)](https://pepy.tech/project/gpjax)\n[![Slack Invite](https://img.shields.io/badge/Slack_Invite--blue?style=social&logo=slack)](https://join.slack.com/t/gpjax/shared_invite/zt-1da57pmjn-rdBCVg9kApirEEn2E5Q2Zw)\n\n[**Quickstart**](#simple-example)\n| [**Install guide**](#installation)\n| [**Documentation**](https://gpjax.readthedocs.io/en/latest/)\n| [**Slack Community**](https://join.slack.com/t/gpjax/shared_invite/zt-1da57pmjn-rdBCVg9kApirEEn2E5Q2Zw)\n\nGPJax aims to provide a low-level interface to Gaussian process (GP) models in\n[Jax](https://github.com/google/jax), structured to give researchers maximum\nflexibility in extending the code to suit their own needs. The idea is that the\ncode should be as close as possible to the maths we write on paper when working\nwith GP models.\n\n# Package support\n\nGPJax was founded by [Thomas Pinder](https://github.com/thomaspinder). Today,\nthe maintenance of GPJax is undertaken by [Thomas\nPinder](https://github.com/thomaspinder) and [Daniel\nDodd](https://github.com/Daniel-Dodd).\n\nWe would be delighted to receive contributions from interested individuals and\ngroups. To learn how you can get involved, please read our [guide for\ncontributing](https://github.com/JaxGaussianProcesses/GPJax/blob/master/CONTRIBUTING.md).\nIf you have any questions, we encourage you to [open an\nissue](https://github.com/JaxGaussianProcesses/GPJax/issues/new/choose). For\nbroader conversations, such as best GP fitting practices or questions about the\nmathematics of GPs, we invite you to [open a\ndiscussion](https://github.com/JaxGaussianProcesses/GPJax/discussions).\n\nFeel free to join our [Slack\nChannel](https://join.slack.com/t/gpjax/shared_invite/zt-1da57pmjn-rdBCVg9kApirEEn2E5Q2Zw),\nwhere we can discuss the development of GPJax and broader support for Gaussian\nprocess modelling.\n\n# Supported methods and interfaces\n\n## Notebook examples\n\n> - [**Conjugate Inference**](https://gpjax.readthedocs.io/en/latest/examples/regression.html)\n> - [**Classification with MCMC**](https://gpjax.readthedocs.io/en/latest/examples/classification.html)\n> - [**Sparse Variational Inference**](https://gpjax.readthedocs.io/en/latest/examples/uncollapsed_vi.html)\n> - [**BlackJax Integration**](https://gpjax.readthedocs.io/en/latest/examples/classification.html)\n> - [**Laplace Approximation**](https://gpjax.readthedocs.io/en/latest/examples/classification.html#Laplace-approximation)\n> - [**Inference on Non-Euclidean Spaces**](https://gpjax.readthedocs.io/en/latest/examples/kernels.html#Custom-Kernel)\n> - [**Inference on Graphs**](https://gpjax.readthedocs.io/en/latest/examples/graph_kernels.html)\n> - [**Learning Gaussian Process Barycentres**](https://gpjax.readthedocs.io/en/latest/examples/barycentres.html)\n> - [**Deep Kernel Regression**](https://gpjax.readthedocs.io/en/latest/examples/haiku.html)\n\n## Guides for customisation\n>\n> - [**Custom kernels**](https://gpjax.readthedocs.io/en/latest/examples/kernels.html#Custom-Kernel)\n> - [**UCI regression**](https://gpjax.readthedocs.io/en/latest/examples/yacht.html)\n\n## Conversion between `.ipynb` and `.py`\nAbove examples are stored in [examples](examples) directory in the double\npercent (`py:percent`) format. Checkout [jupytext\nusing-cli](https://jupytext.readthedocs.io/en/latest/using-cli.html) for more\ninfo.\n\n* To convert `example.py` to `example.ipynb`, run:\n\n```bash\njupytext --to notebook example.py\n```\n\n* To convert `example.ipynb` to `example.py`, run:\n\n```bash\njupytext --to py:percent example.ipynb\n```\n\n# Simple example\n\nLet us import some dependencies and simulate a toy dataset $\\mathcal{D}$.\n\n```python\nimport gpjax as gpx\nfrom jax import grad, jit\nimport jax.numpy as jnp\nimport jax.random as jr\nimport optax as ox\n\nkey = jr.PRNGKey(123)\n\nf = lambda x: 10 * jnp.sin(x)\n\nn = 50\nx = jr.uniform(key=key, minval=-3.0, maxval=3.0, shape=(n,1)).sort()\ny = f(x) + jr.normal(key, shape=(n,1))\nD = gpx.Dataset(X=x, y=y)\n\n# Construct the prior\nmeanf = gpx.mean_functions.Zero()\nkernel = gpx.kernels.RBF()\nprior = gpx.Prior(mean_function=meanf, kernel = kernel)\n\n# Define a likelihood\nlikelihood = gpx.Gaussian(num_datapoints = n)\n\n# Construct the posterior\nposterior = prior * likelihood\n\n# Define an optimiser\noptimiser = ox.adam(learning_rate=1e-2)\n\n# Define the marginal log-likelihood\nnegative_mll = jit(gpx.objectives.ConjugateMLL(negative=True))\n\n# Obtain Type 2 MLEs of the hyperparameters\nopt_posterior, history = gpx.fit(\n    model=posterior,\n    objective=negative_mll,\n    train_data=D,\n    optim=optimiser,\n    num_iters=500,\n    safe=True,\n    key=key,\n)\n\n# Infer the predictive posterior distribution\nxtest = jnp.linspace(-3., 3., 100).reshape(-1, 1)\nlatent_dist = opt_posterior(xtest, D)\npredictive_dist = opt_posterior.likelihood(latent_dist)\n\n# Obtain the predictive mean and standard deviation\npred_mean = predictive_dist.mean()\npred_std = predictive_dist.stddev()\n```\n\n# Installation\n\n## Stable version\n\nThe latest stable version of GPJax can be installed via\npip:\n\n```bash\npip install gpjax\n```\n\n> **Note**\n>\n> We recommend you check your installation version:\n> ```python\n> python -c \'import gpjax; print(gpjax.__version__)\'\n> ```\n\n\n\n## Development version\n> **Warning**\n>\n> This version is possibly unstable and may contain bugs.\n\nClone a copy of the repository to your local machine and run the setup\nconfiguration in development mode.\n```bash\ngit clone https://github.com/JaxGaussianProcesses/GPJax.git\ncd GPJax\npoetry install\n```\n\n> **Note**\n>\n> We advise you create virtual environment before installing:\n> ```\n> conda create -n gpjax_experimental python=3.10.0\n> conda activate gpjax_experimental\n>  ```\n>\n> and recommend you check your installation passes the supplied unit tests:\n>\n> ```python\n> poetry run pytest\n> ```\n\n# Citing GPJax\n\nIf you use GPJax in your research, please cite our [JOSS paper](https://joss.theoj.org/papers/10.21105/joss.04455#).\n\n```\n@article{Pinder2022,\n  doi = {10.21105/joss.04455},\n  url = {https://doi.org/10.21105/joss.04455},\n  year = {2022},\n  publisher = {The Open Journal},\n  volume = {7},\n  number = {75},\n  pages = {4455},\n  author = {Thomas Pinder and Daniel Dodd},\n  title = {GPJax: A Gaussian Process Framework in JAX},\n  journal = {Journal of Open Source Software}\n}\n```\n',
+    'long_description': '<!-- <h1 align=\'center\'>GPJax</h1>\n<h2 align=\'center\'>Gaussian processes in Jax.</h2> -->\n<p align="center">\n<img width="700" height="300" src="https://raw.githubusercontent.com/JaxGaussianProcesses/GPJax/main/docs/_static/gpjax_logo.svg" alt="GPJax\'s logo">\n</p>\n\n[![codecov](https://codecov.io/gh/JaxGaussianProcesses/GPJax/branch/master/graph/badge.svg?token=DM1DRDASU2)](https://codecov.io/gh/JaxGaussianProcesses/GPJax)\n[![CodeFactor](https://www.codefactor.io/repository/github/jaxgaussianprocesses/gpjax/badge)](https://www.codefactor.io/repository/github/jaxgaussianprocesses/gpjax)\n[![Netlify Status](https://api.netlify.com/api/v1/badges/d3950e6f-321f-4508-9e52-426b5dae2715/deploy-status)](https://app.netlify.com/sites/endearing-crepe-c2d5fe/deploys)\n[![PyPI version](https://badge.fury.io/py/GPJax.svg)](https://badge.fury.io/py/GPJax)\n[![DOI](https://joss.theoj.org/papers/10.21105/joss.04455/status.svg)](https://doi.org/10.21105/joss.04455)\n[![Downloads](https://pepy.tech/badge/gpjax)](https://pepy.tech/project/gpjax)\n[![Slack Invite](https://img.shields.io/badge/Slack_Invite--blue?style=social&logo=slack)](https://join.slack.com/t/gpjax/shared_invite/zt-1da57pmjn-rdBCVg9kApirEEn2E5Q2Zw)\n\n[**Quickstart**](#simple-example)\n| [**Install guide**](#installation)\n| [**Documentation**](https://docs.jaxgaussianprocesses.com/)\n| [**Slack Community**](https://join.slack.com/t/gpjax/shared_invite/zt-1da57pmjn-rdBCVg9kApirEEn2E5Q2Zw)\n\nGPJax aims to provide a low-level interface to Gaussian process (GP) models in\n[Jax](https://github.com/google/jax), structured to give researchers maximum\nflexibility in extending the code to suit their own needs. The idea is that the\ncode should be as close as possible to the maths we write on paper when working\nwith GP models.\n\n# Package support\n\nGPJax was founded by [Thomas Pinder](https://github.com/thomaspinder). Today,\nthe maintenance of GPJax is undertaken by [Thomas\nPinder](https://github.com/thomaspinder) and [Daniel\nDodd](https://github.com/Daniel-Dodd).\n\nWe would be delighted to receive contributions from interested individuals and\ngroups. To learn how you can get involved, please read our [guide for\ncontributing](https://github.com/JaxGaussianProcesses/GPJax/blob/master/CONTRIBUTING.md).\nIf you have any questions, we encourage you to [open an\nissue](https://github.com/JaxGaussianProcesses/GPJax/issues/new/choose). For\nbroader conversations, such as best GP fitting practices or questions about the\nmathematics of GPs, we invite you to [open a\ndiscussion](https://github.com/JaxGaussianProcesses/GPJax/discussions).\n\nFeel free to join our [Slack\nChannel](https://join.slack.com/t/gpjax/shared_invite/zt-1da57pmjn-rdBCVg9kApirEEn2E5Q2Zw),\nwhere we can discuss the development of GPJax and broader support for Gaussian\nprocess modelling.\n\n# Supported methods and interfaces\n\n## Notebook examples\n\n> - [**Conjugate Inference**](https://docs.jaxgaussianprocesses.com/examples/regression/)\n> - [**Classification with MCMC**](https://docs.jaxgaussianprocesses.com/examples/classification/)\n> - [**Sparse Variational Inference**](https://docs.jaxgaussianprocesses.com/examples/collapsed_vi/)\n> - [**Stochastic Variational Inference**](https://docs.jaxgaussianprocesses.com/examples/uncollapsed_vi/)\n> - [**BlackJax Integration**](https://docs.jaxgaussianprocesses.com/examples/classification/#mcmc-inference)\n> - [**Laplace Approximation**](https://docs.jaxgaussianprocesses.com/examples/classification/#laplace-approximation)\n> - [**Inference on Non-Euclidean Spaces**](https://docs.jaxgaussianprocesses.com/examples/kernels/#custom-kernel)\n> - [**Inference on Graphs**](https://docs.jaxgaussianprocesses.com/examples/graph_kernels/)\n> - [**Pathwise Sampling**](https://docs.jaxgaussianprocesses.com/examples/spatial/)\n> - [**Learning Gaussian Process Barycentres**](https://docs.jaxgaussianprocesses.com/examples/barycentres/)\n> - [**Deep Kernel Regression**](https://docs.jaxgaussianprocesses.com/examples/deep_kernels/)\n> - [**Poisson Regression**](https://docs.jaxgaussianprocesses.com/examples/poisson/)\n\n## Guides for customisation\n>\n> - [**Custom kernels**](https://docs.jaxgaussianprocesses.com/examples/kernels/#custom-kernel)\n> - [**UCI regression**](https://docs.jaxgaussianprocesses.com/examples/yacht/)\n\n## Conversion between `.ipynb` and `.py`\nAbove examples are stored in [examples](examples) directory in the double\npercent (`py:percent`) format. Checkout [jupytext\nusing-cli](https://jupytext.readthedocs.io/en/latest/using-cli.html) for more\ninfo.\n\n* To convert `example.py` to `example.ipynb`, run:\n\n```bash\njupytext --to notebook example.py\n```\n\n* To convert `example.ipynb` to `example.py`, run:\n\n```bash\njupytext --to py:percent example.ipynb\n```\n\n# Simple example\n\nLet us import some dependencies and simulate a toy dataset $\\mathcal{D}$.\n\n```python\nimport gpjax as gpx\nfrom jax import grad, jit\nimport jax.numpy as jnp\nimport jax.random as jr\nimport optax as ox\n\nkey = jr.PRNGKey(123)\n\nf = lambda x: 10 * jnp.sin(x)\n\nn = 50\nx = jr.uniform(key=key, minval=-3.0, maxval=3.0, shape=(n,1)).sort()\ny = f(x) + jr.normal(key, shape=(n,1))\nD = gpx.Dataset(X=x, y=y)\n\n# Construct the prior\nmeanf = gpx.mean_functions.Zero()\nkernel = gpx.kernels.RBF()\nprior = gpx.Prior(mean_function=meanf, kernel = kernel)\n\n# Define a likelihood\nlikelihood = gpx.Gaussian(num_datapoints = n)\n\n# Construct the posterior\nposterior = prior * likelihood\n\n# Define an optimiser\noptimiser = ox.adam(learning_rate=1e-2)\n\n# Define the marginal log-likelihood\nnegative_mll = jit(gpx.objectives.ConjugateMLL(negative=True))\n\n# Obtain Type 2 MLEs of the hyperparameters\nopt_posterior, history = gpx.fit(\n    model=posterior,\n    objective=negative_mll,\n    train_data=D,\n    optim=optimiser,\n    num_iters=500,\n    safe=True,\n    key=key,\n)\n\n# Infer the predictive posterior distribution\nxtest = jnp.linspace(-3., 3., 100).reshape(-1, 1)\nlatent_dist = opt_posterior(xtest, D)\npredictive_dist = opt_posterior.likelihood(latent_dist)\n\n# Obtain the predictive mean and standard deviation\npred_mean = predictive_dist.mean()\npred_std = predictive_dist.stddev()\n```\n\n# Installation\n\n## Stable version\n\nThe latest stable version of GPJax can be installed via\npip:\n\n```bash\npip install gpjax\n```\n\n> **Note**\n>\n> We recommend you check your installation version:\n> ```python\n> python -c \'import gpjax; print(gpjax.__version__)\'\n> ```\n\n\n\n## Development version\n> **Warning**\n>\n> This version is possibly unstable and may contain bugs.\n\n> **Note**\n>\n> We advise you create virtual environment before installing:\n> ```\n> conda create -n gpjax_experimental python=3.10.0\n> conda activate gpjax_experimental\n>  ```\n>\n> and recommend you check your installation passes the supplied unit tests:\n>\n> ```python\n> poetry run pytest\n> ```\n\nClone a copy of the repository to your local machine and run the setup\nconfiguration in development mode.\n```bash\ngit clone https://github.com/JaxGaussianProcesses/GPJax.git\ncd GPJax\npoetry install\n```\n\n# Citing GPJax\n\nIf you use GPJax in your research, please cite our [JOSS paper](https://joss.theoj.org/papers/10.21105/joss.04455#).\n\n```\n@article{Pinder2022,\n  doi = {10.21105/joss.04455},\n  url = {https://doi.org/10.21105/joss.04455},\n  year = {2022},\n  publisher = {The Open Journal},\n  volume = {7},\n  number = {75},\n  pages = {4455},\n  author = {Thomas Pinder and Daniel Dodd},\n  title = {GPJax: A Gaussian Process Framework in JAX},\n  journal = {Journal of Open Source Software}\n}\n```\n',
     'author': 'Thomas Pinder',
     'author_email': 'tompinder@live.co.uk',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/JaxGaussianProcesses/GPJax',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `gpjax-0.6.1/PKG-INFO` & `gpjax-0.6.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpjax
-Version: 0.6.1
+Version: 0.6.2
 Summary: Gaussian processes in JAX.
 Home-page: https://github.com/JaxGaussianProcesses/GPJax
 License: Apache-2.0
 Keywords: gaussian-processes jax machine-learning bayesian
 Author: Thomas Pinder
 Author-email: tompinder@live.co.uk
 Requires-Python: >=3.8,<3.12
@@ -19,35 +19,35 @@
 Requires-Dist: jaxlib (==0.4.7)
 Requires-Dist: jaxtyping (>=0.2.15,<0.3.0)
 Requires-Dist: optax (>=0.1.4,<0.2.0)
 Requires-Dist: orbax-checkpoint (>=0.2.0,<0.3.0)
 Requires-Dist: simple-pytree (>=0.1.7,<0.2.0)
 Requires-Dist: tensorflow-probability (>=0.19.0,<0.20.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
-Project-URL: Documentation, https://gpjax.readthedocs.io/en/latest/
+Project-URL: Documentation, https://docs.jaxgaussianprocesses.com/
 Project-URL: Repository, https://github.com/JaxGaussianProcesses/GPJax
 Description-Content-Type: text/markdown
 
 <!-- <h1 align='center'>GPJax</h1>
 <h2 align='center'>Gaussian processes in Jax.</h2> -->
 <p align="center">
 <img width="700" height="300" src="https://raw.githubusercontent.com/JaxGaussianProcesses/GPJax/main/docs/_static/gpjax_logo.svg" alt="GPJax's logo">
 </p>
 
 [![codecov](https://codecov.io/gh/JaxGaussianProcesses/GPJax/branch/master/graph/badge.svg?token=DM1DRDASU2)](https://codecov.io/gh/JaxGaussianProcesses/GPJax)
 [![CodeFactor](https://www.codefactor.io/repository/github/jaxgaussianprocesses/gpjax/badge)](https://www.codefactor.io/repository/github/jaxgaussianprocesses/gpjax)
-[![Documentation Status](https://readthedocs.org/projects/gpjax/badge/?version=latest)](https://gpjax.readthedocs.io/en/latest/?badge=latest)
+[![Netlify Status](https://api.netlify.com/api/v1/badges/d3950e6f-321f-4508-9e52-426b5dae2715/deploy-status)](https://app.netlify.com/sites/endearing-crepe-c2d5fe/deploys)
 [![PyPI version](https://badge.fury.io/py/GPJax.svg)](https://badge.fury.io/py/GPJax)
 [![DOI](https://joss.theoj.org/papers/10.21105/joss.04455/status.svg)](https://doi.org/10.21105/joss.04455)
 [![Downloads](https://pepy.tech/badge/gpjax)](https://pepy.tech/project/gpjax)
 [![Slack Invite](https://img.shields.io/badge/Slack_Invite--blue?style=social&logo=slack)](https://join.slack.com/t/gpjax/shared_invite/zt-1da57pmjn-rdBCVg9kApirEEn2E5Q2Zw)
 
 [**Quickstart**](#simple-example)
 | [**Install guide**](#installation)
-| [**Documentation**](https://gpjax.readthedocs.io/en/latest/)
+| [**Documentation**](https://docs.jaxgaussianprocesses.com/)
 | [**Slack Community**](https://join.slack.com/t/gpjax/shared_invite/zt-1da57pmjn-rdBCVg9kApirEEn2E5Q2Zw)
 
 GPJax aims to provide a low-level interface to Gaussian process (GP) models in
 [Jax](https://github.com/google/jax), structured to give researchers maximum
 flexibility in extending the code to suit their own needs. The idea is that the
 code should be as close as possible to the maths we write on paper when working
 with GP models.
@@ -73,28 +73,31 @@
 where we can discuss the development of GPJax and broader support for Gaussian
 process modelling.
 
 # Supported methods and interfaces
 
 ## Notebook examples
 
-> - [**Conjugate Inference**](https://gpjax.readthedocs.io/en/latest/examples/regression.html)
-> - [**Classification with MCMC**](https://gpjax.readthedocs.io/en/latest/examples/classification.html)
-> - [**Sparse Variational Inference**](https://gpjax.readthedocs.io/en/latest/examples/uncollapsed_vi.html)
-> - [**BlackJax Integration**](https://gpjax.readthedocs.io/en/latest/examples/classification.html)
-> - [**Laplace Approximation**](https://gpjax.readthedocs.io/en/latest/examples/classification.html#Laplace-approximation)
-> - [**Inference on Non-Euclidean Spaces**](https://gpjax.readthedocs.io/en/latest/examples/kernels.html#Custom-Kernel)
-> - [**Inference on Graphs**](https://gpjax.readthedocs.io/en/latest/examples/graph_kernels.html)
-> - [**Learning Gaussian Process Barycentres**](https://gpjax.readthedocs.io/en/latest/examples/barycentres.html)
-> - [**Deep Kernel Regression**](https://gpjax.readthedocs.io/en/latest/examples/haiku.html)
+> - [**Conjugate Inference**](https://docs.jaxgaussianprocesses.com/examples/regression/)
+> - [**Classification with MCMC**](https://docs.jaxgaussianprocesses.com/examples/classification/)
+> - [**Sparse Variational Inference**](https://docs.jaxgaussianprocesses.com/examples/collapsed_vi/)
+> - [**Stochastic Variational Inference**](https://docs.jaxgaussianprocesses.com/examples/uncollapsed_vi/)
+> - [**BlackJax Integration**](https://docs.jaxgaussianprocesses.com/examples/classification/#mcmc-inference)
+> - [**Laplace Approximation**](https://docs.jaxgaussianprocesses.com/examples/classification/#laplace-approximation)
+> - [**Inference on Non-Euclidean Spaces**](https://docs.jaxgaussianprocesses.com/examples/kernels/#custom-kernel)
+> - [**Inference on Graphs**](https://docs.jaxgaussianprocesses.com/examples/graph_kernels/)
+> - [**Pathwise Sampling**](https://docs.jaxgaussianprocesses.com/examples/spatial/)
+> - [**Learning Gaussian Process Barycentres**](https://docs.jaxgaussianprocesses.com/examples/barycentres/)
+> - [**Deep Kernel Regression**](https://docs.jaxgaussianprocesses.com/examples/deep_kernels/)
+> - [**Poisson Regression**](https://docs.jaxgaussianprocesses.com/examples/poisson/)
 
 ## Guides for customisation
 >
-> - [**Custom kernels**](https://gpjax.readthedocs.io/en/latest/examples/kernels.html#Custom-Kernel)
-> - [**UCI regression**](https://gpjax.readthedocs.io/en/latest/examples/yacht.html)
+> - [**Custom kernels**](https://docs.jaxgaussianprocesses.com/examples/kernels/#custom-kernel)
+> - [**UCI regression**](https://docs.jaxgaussianprocesses.com/examples/yacht/)
 
 ## Conversion between `.ipynb` and `.py`
 Above examples are stored in [examples](examples) directory in the double
 percent (`py:percent`) format. Checkout [jupytext
 using-cli](https://jupytext.readthedocs.io/en/latest/using-cli.html) for more
 info.
 
@@ -189,36 +192,36 @@
 
 
 ## Development version
 > **Warning**
 >
 > This version is possibly unstable and may contain bugs.
 
-Clone a copy of the repository to your local machine and run the setup
-configuration in development mode.
-```bash
-git clone https://github.com/JaxGaussianProcesses/GPJax.git
-cd GPJax
-poetry install
-```
-
 > **Note**
 >
 > We advise you create virtual environment before installing:
 > ```
 > conda create -n gpjax_experimental python=3.10.0
 > conda activate gpjax_experimental
 >  ```
 >
 > and recommend you check your installation passes the supplied unit tests:
 >
 > ```python
 > poetry run pytest
 > ```
 
+Clone a copy of the repository to your local machine and run the setup
+configuration in development mode.
+```bash
+git clone https://github.com/JaxGaussianProcesses/GPJax.git
+cd GPJax
+poetry install
+```
+
 # Citing GPJax
 
 If you use GPJax in your research, please cite our [JOSS paper](https://joss.theoj.org/papers/10.21105/joss.04455#).
 
 ```
 @article{Pinder2022,
   doi = {10.21105/joss.04455},
```

