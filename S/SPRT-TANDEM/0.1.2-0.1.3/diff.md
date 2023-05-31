# Comparing `tmp/SPRT-TANDEM-0.1.2.tar.gz` & `tmp/SPRT-TANDEM-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SPRT-TANDEM-0.1.2.tar", last modified: Wed May 31 05:33:34 2023, max compression
+gzip compressed data, was "SPRT-TANDEM-0.1.3.tar", last modified: Wed May 31 19:52:26 2023, max compression
```

## Comparing `SPRT-TANDEM-0.1.2.tar` & `SPRT-TANDEM-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,34 @@
-drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-05-31 05:33:34.579323 SPRT-TANDEM-0.1.2/
--rw-r--r--   0 afe       (1000) afe       (1000)     1095 2023-05-01 05:13:22.000000 SPRT-TANDEM-0.1.2/LICENSE
--rw-rw-r--   0 afe       (1000) afe       (1000)    16222 2023-05-31 05:33:34.579323 SPRT-TANDEM-0.1.2/PKG-INFO
--rw-r--r--   0 afe       (1000) afe       (1000)    15643 2023-05-31 03:32:21.000000 SPRT-TANDEM-0.1.2/README.md
-drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-05-31 05:33:34.579323 SPRT-TANDEM-0.1.2/SPRT_TANDEM.egg-info/
--rw-rw-r--   0 afe       (1000) afe       (1000)    16222 2023-05-31 05:33:34.000000 SPRT-TANDEM-0.1.2/SPRT_TANDEM.egg-info/PKG-INFO
--rw-rw-r--   0 afe       (1000) afe       (1000)      246 2023-05-31 05:33:34.000000 SPRT-TANDEM-0.1.2/SPRT_TANDEM.egg-info/SOURCES.txt
--rw-rw-r--   0 afe       (1000) afe       (1000)        1 2023-05-31 05:33:34.000000 SPRT-TANDEM-0.1.2/SPRT_TANDEM.egg-info/dependency_links.txt
--rw-rw-r--   0 afe       (1000) afe       (1000)       30 2023-05-31 05:33:34.000000 SPRT-TANDEM-0.1.2/SPRT_TANDEM.egg-info/requires.txt
--rw-rw-r--   0 afe       (1000) afe       (1000)        7 2023-05-31 05:33:34.000000 SPRT-TANDEM-0.1.2/SPRT_TANDEM.egg-info/top_level.txt
--rw-rw-r--   0 afe       (1000) afe       (1000)       38 2023-05-31 05:33:34.579323 SPRT-TANDEM-0.1.2/setup.cfg
--rw-r--r--   0 afe       (1000) afe       (1000)     1063 2023-05-31 05:33:14.000000 SPRT-TANDEM-0.1.2/setup.py
-drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-05-31 05:33:34.579323 SPRT-TANDEM-0.1.2/tandem/
--rw-r--r--   0 afe       (1000) afe       (1000)      356 2023-05-31 05:14:48.000000 SPRT-TANDEM-0.1.2/tandem/__init__.py
--rwxr--r--   0 afe       (1000) afe       (1000)     2822 2023-05-31 05:19:38.000000 SPRT-TANDEM-0.1.2/tandem/sprt_tandem_main.py
+drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-05-31 19:52:26.647079 SPRT-TANDEM-0.1.3/
+-rw-r--r--   0 afe       (1000) afe       (1000)     1095 2023-05-01 05:13:22.000000 SPRT-TANDEM-0.1.3/LICENSE
+-rw-rw-r--   0 afe       (1000) afe       (1000)    14145 2023-05-31 19:52:26.647079 SPRT-TANDEM-0.1.3/PKG-INFO
+-rw-r--r--   0 afe       (1000) afe       (1000)    13560 2023-05-31 12:20:47.000000 SPRT-TANDEM-0.1.3/README.md
+drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-05-31 19:52:26.647079 SPRT-TANDEM-0.1.3/SPRT_TANDEM.egg-info/
+-rw-rw-r--   0 afe       (1000) afe       (1000)    14145 2023-05-31 19:52:26.000000 SPRT-TANDEM-0.1.3/SPRT_TANDEM.egg-info/PKG-INFO
+-rw-rw-r--   0 afe       (1000) afe       (1000)      675 2023-05-31 19:52:26.000000 SPRT-TANDEM-0.1.3/SPRT_TANDEM.egg-info/SOURCES.txt
+-rw-rw-r--   0 afe       (1000) afe       (1000)        1 2023-05-31 19:52:26.000000 SPRT-TANDEM-0.1.3/SPRT_TANDEM.egg-info/dependency_links.txt
+-rw-rw-r--   0 afe       (1000) afe       (1000)       30 2023-05-31 19:52:26.000000 SPRT-TANDEM-0.1.3/SPRT_TANDEM.egg-info/requires.txt
+-rw-rw-r--   0 afe       (1000) afe       (1000)        7 2023-05-31 19:52:26.000000 SPRT-TANDEM-0.1.3/SPRT_TANDEM.egg-info/top_level.txt
+-rw-rw-r--   0 afe       (1000) afe       (1000)       38 2023-05-31 19:52:26.647079 SPRT-TANDEM-0.1.3/setup.cfg
+-rw-r--r--   0 afe       (1000) afe       (1000)     1077 2023-05-31 19:51:10.000000 SPRT-TANDEM-0.1.3/setup.py
+drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-05-31 19:52:26.647079 SPRT-TANDEM-0.1.3/tandem/
+-rw-r--r--   0 afe       (1000) afe       (1000)      356 2023-05-31 05:14:48.000000 SPRT-TANDEM-0.1.3/tandem/__init__.py
+drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-05-31 19:52:26.647079 SPRT-TANDEM-0.1.3/tandem/config/
+-rw-r--r--   0 afe       (1000) afe       (1000)        0 2023-05-31 19:47:27.000000 SPRT-TANDEM-0.1.3/tandem/config/__init__.py
+-rwxr-xr-x   0 afe       (1000) afe       (1000)    11169 2023-05-31 19:50:55.000000 SPRT-TANDEM-0.1.3/tandem/config/config_definition.py
+drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-05-31 19:52:26.647079 SPRT-TANDEM-0.1.3/tandem/data/
+-rw-r--r--   0 afe       (1000) afe       (1000)        0 2023-05-31 19:47:27.000000 SPRT-TANDEM-0.1.3/tandem/data/__init__.py
+drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-05-31 19:52:26.647079 SPRT-TANDEM-0.1.3/tandem/models/
+-rw-r--r--   0 afe       (1000) afe       (1000)        0 2023-05-31 19:47:27.000000 SPRT-TANDEM-0.1.3/tandem/models/__init__.py
+-rw-r--r--   0 afe       (1000) afe       (1000)    14111 2023-05-31 05:13:13.000000 SPRT-TANDEM-0.1.3/tandem/models/losses.py
+-rwxr--r--   0 afe       (1000) afe       (1000)     1417 2023-05-31 05:14:34.000000 SPRT-TANDEM-0.1.3/tandem/models/optimizers.py
+-rwxr-xr-x   0 afe       (1000) afe       (1000)    26287 2023-05-31 05:17:50.000000 SPRT-TANDEM-0.1.3/tandem/models/temporal_integrators.py
+-rwxr--r--   0 afe       (1000) afe       (1000)     2822 2023-05-31 05:19:38.000000 SPRT-TANDEM-0.1.3/tandem/sprt_tandem_main.py
+drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-05-31 19:52:26.647079 SPRT-TANDEM-0.1.3/tandem/utils/
+-rw-r--r--   0 afe       (1000) afe       (1000)        0 2023-05-31 19:47:27.000000 SPRT-TANDEM-0.1.3/tandem/utils/__init__.py
+-rwxr--r--   0 afe       (1000) afe       (1000)     6340 2023-05-31 05:18:03.000000 SPRT-TANDEM-0.1.3/tandem/utils/checkpoint.py
+-rw-r--r--   0 afe       (1000) afe       (1000)    22645 2023-05-31 05:22:17.000000 SPRT-TANDEM-0.1.3/tandem/utils/data_processing.py
+-rwxr-xr-x   0 afe       (1000) afe       (1000)    26821 2023-05-31 05:18:23.000000 SPRT-TANDEM-0.1.3/tandem/utils/hyperparameter_tuning.py
+-rwxr--r--   0 afe       (1000) afe       (1000)    24962 2023-05-31 05:18:36.000000 SPRT-TANDEM-0.1.3/tandem/utils/logging.py
+-rwxr--r--   0 afe       (1000) afe       (1000)    19979 2023-05-31 05:21:01.000000 SPRT-TANDEM-0.1.3/tandem/utils/misc.py
+-rw-r--r--   0 afe       (1000) afe       (1000)    49570 2023-05-31 05:18:56.000000 SPRT-TANDEM-0.1.3/tandem/utils/performance_metrics.py
+-rw-r--r--   0 afe       (1000) afe       (1000)    10207 2023-05-31 05:23:44.000000 SPRT-TANDEM-0.1.3/tandem/utils/training.py
```

### Comparing `SPRT-TANDEM-0.1.2/LICENSE` & `SPRT-TANDEM-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `SPRT-TANDEM-0.1.2/PKG-INFO` & `SPRT-TANDEM-0.1.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,49 +1,37 @@
 Metadata-Version: 2.1
 Name: SPRT-TANDEM
-Version: 0.1.2
-Summary: SPRT-TANDEM for sequential density ratio estimation to simultaneously optimize speed and accuracy of early-classification.
+Version: 0.1.3
+Summary: SPRT-TANDEM for sequential density ratio estimation to simultaneously optimize both speed and accuracy of early-classification.
 Home-page: https://github.com/Akinori-F-Ebihara/SPRT-TANDEM-PyTorch
 Author: Akinori F. Ebihara
 Author-email: aebihara@nec.com
 License: MIT
-Keywords: Sequential Probability Ratio Testlikelihood ratio,density ratio estimation,early classification,artificial intelligence,machine learning
+Keywords: Sequential Probability Ratio Test,likelihood ratio,density ratio estimation,early classification,artificial intelligence,machine learning
 Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SPRT-TANDEM-PyTorch
 This repository contains the official PyTorch implementation of __SPRT-TANDEM__ ([ICASSP2023](https://arxiv.org/abs/2302.09810), [ICML2021](http://proceedings.mlr.press/v139/miyagawa21a.html), and [ICLR2021](https://openreview.net/forum?id=Rhsu5qD36cL)). __SPRT-TANDEM__ is a neuroscience-inspired sequential density ratio estimation (SDRE) algorithm that estimates log-likelihood ratios of two or more hypotheses for fast and accurate sequential data classification. For an intuitive understanding, please refer to the [SPRT-TANDEM tutorial](https://github.com/Akinori-F-Ebihara/SPRT-TANDEM_tutorial).
 
-<div align="center">
-<figure>
-<img src ="./images/SDRE_3class.png" width=70%>  
-</figure>
-</div>
-<p align="center">Figure 1: Example sequential density ratio estimation (SDRE) results on a 3-class multivariate Gaussian dataset.</p>
-
 
 ## Quickstart
 1. To create a new SDRE dataset, run the [Generate_sequential_Gaussian_as_LMDB.ipynb](https://github.com/Akinori-F-Ebihara/SPRT-TANDEM-PyTorch/blob/main/notebooks/Generate_sequential_Gaussian_as_LMDB.ipynb) notebook.
 2. Edit the user editable block of [config_definition.py](https://github.com/Akinori-F-Ebihara/SPRT-TANDEM-PyTorch/blob/main/config/config_definition.py). Specify path to the dataset file created in step 1. Other frequently used entries include SUBPROJECT_NAME_PREFIX (to tag your experiment) and EXP_PHASE (to specify whether you are trying, tuning, or running statistics. See Hyperparameter Tuning for details).
 3. Execute [sprt_tandem_main.py](https://github.com/Akinori-F-Ebihara/SPRT-TANDEM-PyTorch/blob/main/sprt_tandem_main.py).
 
 ## Tested Environment
 ```
 python      3.8.10
 torch       2.0.0
 notebook    6.5.3
 optuna      3.1.0
 ```
-
-## Requirements for Reading This Article
-
-This article is best read using the Chrome browser with the [MathJax Plugin for GitHub](https://chrome.google.com/webstore/detail/mathjax-plugin-for-github/ioemnmodlmafdkllaclgeombjnmnbima?hl=en) installed.
-
 ## Supported Network Architectures  
 We support the two major architectures for processing time series data: Long short-term memory (LSTM, [1]) and Transformer [2]. To avoid the likelihood ratio saturation problem and approach asymptotic optimality (for details, see [Ebihara+, ICASSP2023](https://arxiv.org/abs/2302.09810)), we developed two novel models based on these architectures: B2Bssqrt-TANDEM (based on LSTM) and TANDEMformer (based on Transformer).
 ### LSTM (B2Bsqrt-TANDEM, [ICASSP2023](https://arxiv.org/abs/2302.09810))  
 The LSTM with the back-to-back square root (B2Bsqrt) activation function can be used by setting the following variables: 
 
 - MODEL_BACKBONE: "LSTM"
 - ACTIVATION_OUTPUT: "B2Bsqrt"  
@@ -52,21 +40,14 @@
 
 \begin{align}
 f_{\mathrm{B2Bsqrt}}(x) := \mathrm{sign}(x)(\sqrt{\alpha+|x|}-\sqrt{\alpha})
 \end{align}
 
 Where $\alpha$ is a hyperparameter. 
 
-<div align="center">
-<figure>
-<img src ="./images/Conceptual_figure_B2Bsqrt.png" width=60%>  
-</figure>
-</div>
-<p align="center">Figure 2: Conceptual figure showing the LSTM cell equipped with the B2Bsqrt activation function. B2Bsqrt can be used as an alternative to the tanh function. With an unbounded range and a finite gradient at the origin, B2Bsqrt prevents the saturation problem while enabling stable training.</p>
-
 
 ### Transformer (TANDEMformer, [ICASSP2023](https://arxiv.org/abs/2302.09810))  
 The Transformer is equipped with the Normalized Summation Pooling (NSP) layer, which is incorporated by default.
 
 Let $X_i^{(t, t+w)}$ be subtokens sampled with a sliding window of size $w \in [N]$, and let $Z_i^{(t, t+w)}:=\{z_i^{(s)}\}^{t+w}_{s=t}$ be the subtokens mixed with self-attention. Given the Markov order $N$, the \texttt{NSP} layer is defined as:
 
 \begin{align}
@@ -74,20 +55,14 @@
 \end{align}
 
 To use it, set the following variable:
 
 - MODEL_BACKBONE: "Transformer"
 
 
-<div align="center">
-<figure>
-<img src ="./images/Conceptual_figure_TANDEMformer.png" width=50%>  
-</figure>
-</div>
-<p align="center">Figure 3: Conceptual figure illustrates the Transformer block equipped with the NSP layer. First, tokens are extracted using a sliding window and then mixed with self-attention. The normalized summation pooling layer then takes the sum of the tokens and divides them by a constant, which is the maximum size of the sliding window.</p>  
 
 ## Supported Loss Functions for SDRE
 SPRT-TANDEM uses both the loss for sequential likelihood ratio estimation (SDRE) and (multiplet-) cross-entropy loss ([ICLR2021](https://openreview.net/forum?id=Rhsu5qD36cL)). The two functions, LSEL and LLLR, are supported loss function for SDRE. To choose the loss function, set the following variables:
 
 - LLLR_VERSION: "LSEL" or "LLLR"
 
 Additionally, modify the values of PARAM_LLR_LOSS and PARAM_MULTIPLET_LOSS to achieve the desired balance between likelihood estimation and cross-entropy loss.
@@ -104,20 +79,14 @@
 \begin{align}
 \hat{L}_{\mathrm{\text{LLLR}}} (\mathbb{\theta}; S) := \mathbb{E} \left[ \left| y - \sigma\left( \hat{\lambda}\_{k,l}   ( X_i^{(1,t)}; \theta) \right) \right| \right]
 \end{align}
 
 ## Order N of Markov assumption
 The Markov order $N$ is used to determine the length of the sliding window that extracts a subset from the entire feature vector of a time series. $N$ is a convenient hyperparameter that incorporates prior knowledge of the time series. An optimal $N$ can be found either based on the \textit{specific time scale} or through hyperparameter tuning. The specific time scale characterizes the data class, e.g., long temporal action such as UCF101 has a long specific time scale, while a spoofing attack such as SiW has a short specific time scale (because one frame can have sufficient information of the attack). Setting $N$ equal to the specific time scale usually works best. Alternatively, $N$ can be objectively chosen using a hyperparameter tuning algorithm such as Optuna, just like other hyperparameters. Because $N$ is only related to the temporal integrator after feature extraction, optimizing it is not computationally expensive.
 
-<div align="center">
-<figure>
-<img src ="./images/Conceptual_figure_streamline.png" width=70%>  
-</figure>
-</div>
-<p align="center">Figure 4: Conceptual figure showing the streamline of online SDRE. A subset of the time series' feature vectors is extracted based on the order of Markov assumption, N. </p>
 
 The log-likelihood ratio is estimated from a subset of the feature vectors extracted using a sliding window of size $N$. This estimation is classification-based. Specifically, the temporal integrator is trained to output class logits, which are then used to update the log-likelihood ratio at each time step based on the TANDEM formula.
 ### TANDEM formula ([ICLR2021](https://openreview.net/forum?id=Rhsu5qD36cL))
 \begin{align}
 &\ \log \left(
 \frac{p(x^{(1)},x^{(2)}, ..., x^{(t)}| y=1)}{p(x^{(1)},x^{(2)}, ..., x^{(t)}| y=0)}
 \right)\nonumber \newline
@@ -201,20 +170,14 @@
 - Optuna_databases: Optuna .db file is stored here.
 - TensorBoard_events: TensorBard event files are saved here.
 - checkpoints: trained parameters are saved as .py files when the best optimation target value is updated.
 - stdout_logs: standard output strings are saved as .log files.
 
 The plot below shows an example image saved in a TensorBoard event file. Note that you can avoid saving figures by setting IS_SAVE_FIGURE=False.
 
-<div align="center">
-<figure>
-<img src ="./images/example_tensorboard.png" width=100%>  
-</figure>
-</div>
-<p align="center">Figure 5: Example image saved in a TensorBoard event file. (left and center) Estimated LLR trajectories and Ground-truth LLR trajectories of 3-class multidimensional Gaussian dataset. (right) Speed-accuracy tradeoff (SAT) curve calculated by running the SPRT algorithm.</p>
 
 Note that "Class $a$ vs. $b$ at $y=a$" indicates that the plotted LLR shows $\log{p(X|y=a) / p(X|y=b)}$, when the ground truth label is $y=a$. 
 
 ## Citation
 ___Please cite the orignal paper(s) if you use the whole or a part of our codes.___
 
 ```
```

### Comparing `SPRT-TANDEM-0.1.2/README.md` & `SPRT-TANDEM-0.1.3/SPRT_TANDEM.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,37 @@
+Metadata-Version: 2.1
+Name: SPRT-TANDEM
+Version: 0.1.3
+Summary: SPRT-TANDEM for sequential density ratio estimation to simultaneously optimize both speed and accuracy of early-classification.
+Home-page: https://github.com/Akinori-F-Ebihara/SPRT-TANDEM-PyTorch
+Author: Akinori F. Ebihara
+Author-email: aebihara@nec.com
+License: MIT
+Keywords: Sequential Probability Ratio Test,likelihood ratio,density ratio estimation,early classification,artificial intelligence,machine learning
+Platform: UNKNOWN
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # SPRT-TANDEM-PyTorch
 This repository contains the official PyTorch implementation of __SPRT-TANDEM__ ([ICASSP2023](https://arxiv.org/abs/2302.09810), [ICML2021](http://proceedings.mlr.press/v139/miyagawa21a.html), and [ICLR2021](https://openreview.net/forum?id=Rhsu5qD36cL)). __SPRT-TANDEM__ is a neuroscience-inspired sequential density ratio estimation (SDRE) algorithm that estimates log-likelihood ratios of two or more hypotheses for fast and accurate sequential data classification. For an intuitive understanding, please refer to the [SPRT-TANDEM tutorial](https://github.com/Akinori-F-Ebihara/SPRT-TANDEM_tutorial).
 
-<div align="center">
-<figure>
-<img src ="./images/SDRE_3class.png" width=70%>  
-</figure>
-</div>
-<p align="center">Figure 1: Example sequential density ratio estimation (SDRE) results on a 3-class multivariate Gaussian dataset.</p>
-
 
 ## Quickstart
 1. To create a new SDRE dataset, run the [Generate_sequential_Gaussian_as_LMDB.ipynb](https://github.com/Akinori-F-Ebihara/SPRT-TANDEM-PyTorch/blob/main/notebooks/Generate_sequential_Gaussian_as_LMDB.ipynb) notebook.
 2. Edit the user editable block of [config_definition.py](https://github.com/Akinori-F-Ebihara/SPRT-TANDEM-PyTorch/blob/main/config/config_definition.py). Specify path to the dataset file created in step 1. Other frequently used entries include SUBPROJECT_NAME_PREFIX (to tag your experiment) and EXP_PHASE (to specify whether you are trying, tuning, or running statistics. See Hyperparameter Tuning for details).
 3. Execute [sprt_tandem_main.py](https://github.com/Akinori-F-Ebihara/SPRT-TANDEM-PyTorch/blob/main/sprt_tandem_main.py).
 
 ## Tested Environment
 ```
 python      3.8.10
 torch       2.0.0
 notebook    6.5.3
 optuna      3.1.0
 ```
-
-## Requirements for Reading This Article
-
-This article is best read using the Chrome browser with the [MathJax Plugin for GitHub](https://chrome.google.com/webstore/detail/mathjax-plugin-for-github/ioemnmodlmafdkllaclgeombjnmnbima?hl=en) installed.
-
 ## Supported Network Architectures  
 We support the two major architectures for processing time series data: Long short-term memory (LSTM, [1]) and Transformer [2]. To avoid the likelihood ratio saturation problem and approach asymptotic optimality (for details, see [Ebihara+, ICASSP2023](https://arxiv.org/abs/2302.09810)), we developed two novel models based on these architectures: B2Bssqrt-TANDEM (based on LSTM) and TANDEMformer (based on Transformer).
 ### LSTM (B2Bsqrt-TANDEM, [ICASSP2023](https://arxiv.org/abs/2302.09810))  
 The LSTM with the back-to-back square root (B2Bsqrt) activation function can be used by setting the following variables: 
 
 - MODEL_BACKBONE: "LSTM"
 - ACTIVATION_OUTPUT: "B2Bsqrt"  
@@ -38,21 +40,14 @@
 
 \begin{align}
 f_{\mathrm{B2Bsqrt}}(x) := \mathrm{sign}(x)(\sqrt{\alpha+|x|}-\sqrt{\alpha})
 \end{align}
 
 Where $\alpha$ is a hyperparameter. 
 
-<div align="center">
-<figure>
-<img src ="./images/Conceptual_figure_B2Bsqrt.png" width=60%>  
-</figure>
-</div>
-<p align="center">Figure 2: Conceptual figure showing the LSTM cell equipped with the B2Bsqrt activation function. B2Bsqrt can be used as an alternative to the tanh function. With an unbounded range and a finite gradient at the origin, B2Bsqrt prevents the saturation problem while enabling stable training.</p>
-
 
 ### Transformer (TANDEMformer, [ICASSP2023](https://arxiv.org/abs/2302.09810))  
 The Transformer is equipped with the Normalized Summation Pooling (NSP) layer, which is incorporated by default.
 
 Let $X_i^{(t, t+w)}$ be subtokens sampled with a sliding window of size $w \in [N]$, and let $Z_i^{(t, t+w)}:=\{z_i^{(s)}\}^{t+w}_{s=t}$ be the subtokens mixed with self-attention. Given the Markov order $N$, the \texttt{NSP} layer is defined as:
 
 \begin{align}
@@ -60,20 +55,14 @@
 \end{align}
 
 To use it, set the following variable:
 
 - MODEL_BACKBONE: "Transformer"
 
 
-<div align="center">
-<figure>
-<img src ="./images/Conceptual_figure_TANDEMformer.png" width=50%>  
-</figure>
-</div>
-<p align="center">Figure 3: Conceptual figure illustrates the Transformer block equipped with the NSP layer. First, tokens are extracted using a sliding window and then mixed with self-attention. The normalized summation pooling layer then takes the sum of the tokens and divides them by a constant, which is the maximum size of the sliding window.</p>  
 
 ## Supported Loss Functions for SDRE
 SPRT-TANDEM uses both the loss for sequential likelihood ratio estimation (SDRE) and (multiplet-) cross-entropy loss ([ICLR2021](https://openreview.net/forum?id=Rhsu5qD36cL)). The two functions, LSEL and LLLR, are supported loss function for SDRE. To choose the loss function, set the following variables:
 
 - LLLR_VERSION: "LSEL" or "LLLR"
 
 Additionally, modify the values of PARAM_LLR_LOSS and PARAM_MULTIPLET_LOSS to achieve the desired balance between likelihood estimation and cross-entropy loss.
@@ -90,20 +79,14 @@
 \begin{align}
 \hat{L}_{\mathrm{\text{LLLR}}} (\mathbb{\theta}; S) := \mathbb{E} \left[ \left| y - \sigma\left( \hat{\lambda}\_{k,l}   ( X_i^{(1,t)}; \theta) \right) \right| \right]
 \end{align}
 
 ## Order N of Markov assumption
 The Markov order $N$ is used to determine the length of the sliding window that extracts a subset from the entire feature vector of a time series. $N$ is a convenient hyperparameter that incorporates prior knowledge of the time series. An optimal $N$ can be found either based on the \textit{specific time scale} or through hyperparameter tuning. The specific time scale characterizes the data class, e.g., long temporal action such as UCF101 has a long specific time scale, while a spoofing attack such as SiW has a short specific time scale (because one frame can have sufficient information of the attack). Setting $N$ equal to the specific time scale usually works best. Alternatively, $N$ can be objectively chosen using a hyperparameter tuning algorithm such as Optuna, just like other hyperparameters. Because $N$ is only related to the temporal integrator after feature extraction, optimizing it is not computationally expensive.
 
-<div align="center">
-<figure>
-<img src ="./images/Conceptual_figure_streamline.png" width=70%>  
-</figure>
-</div>
-<p align="center">Figure 4: Conceptual figure showing the streamline of online SDRE. A subset of the time series' feature vectors is extracted based on the order of Markov assumption, N. </p>
 
 The log-likelihood ratio is estimated from a subset of the feature vectors extracted using a sliding window of size $N$. This estimation is classification-based. Specifically, the temporal integrator is trained to output class logits, which are then used to update the log-likelihood ratio at each time step based on the TANDEM formula.
 ### TANDEM formula ([ICLR2021](https://openreview.net/forum?id=Rhsu5qD36cL))
 \begin{align}
 &\ \log \left(
 \frac{p(x^{(1)},x^{(2)}, ..., x^{(t)}| y=1)}{p(x^{(1)},x^{(2)}, ..., x^{(t)}| y=0)}
 \right)\nonumber \newline
@@ -187,20 +170,14 @@
 - Optuna_databases: Optuna .db file is stored here.
 - TensorBoard_events: TensorBard event files are saved here.
 - checkpoints: trained parameters are saved as .py files when the best optimation target value is updated.
 - stdout_logs: standard output strings are saved as .log files.
 
 The plot below shows an example image saved in a TensorBoard event file. Note that you can avoid saving figures by setting IS_SAVE_FIGURE=False.
 
-<div align="center">
-<figure>
-<img src ="./images/example_tensorboard.png" width=100%>  
-</figure>
-</div>
-<p align="center">Figure 5: Example image saved in a TensorBoard event file. (left and center) Estimated LLR trajectories and Ground-truth LLR trajectories of 3-class multidimensional Gaussian dataset. (right) Speed-accuracy tradeoff (SAT) curve calculated by running the SPRT algorithm.</p>
 
 Note that "Class $a$ vs. $b$ at $y=a$" indicates that the plotted LLR shows $\log{p(X|y=a) / p(X|y=b)}$, when the ground truth label is $y=a$. 
 
 ## Citation
 ___Please cite the orignal paper(s) if you use the whole or a part of our codes.___
 
 ```
@@ -238,7 +215,9 @@
 3. A. Vaswani, N. Shazeer, N. Parmar, J. Uszkoreit, L. Jones, A. N. Gomez, L. u. Kaiser, and I. Polosukhin, “Attention is all you need,” in NeurIPS, 2017, vol. 30, pp. 5998–6008.
 
 ## Contacts
 SPRT-TANDEM marks its 4th anniversary. What started as a small project has now become a huge undertaking that we never imagined. Due to its complexity, it is difficult for me to explain all the details in this README section. Please feel free to reach out to me anytime if you have any questions.
 - email: aebihara[at]nec.com
 - twitter: [@non_iid](http/twitter.com/non_iid)
 - GitHub issues: see the link above or click [here](https://github.com/Akinori-F-Ebihara/SPRT-TANDEM-PyTorch/issues)
+
+
```

### Comparing `SPRT-TANDEM-0.1.2/SPRT_TANDEM.egg-info/PKG-INFO` & `SPRT-TANDEM-0.1.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,49 +1,23 @@
-Metadata-Version: 2.1
-Name: SPRT-TANDEM
-Version: 0.1.2
-Summary: SPRT-TANDEM for sequential density ratio estimation to simultaneously optimize speed and accuracy of early-classification.
-Home-page: https://github.com/Akinori-F-Ebihara/SPRT-TANDEM-PyTorch
-Author: Akinori F. Ebihara
-Author-email: aebihara@nec.com
-License: MIT
-Keywords: Sequential Probability Ratio Testlikelihood ratio,density ratio estimation,early classification,artificial intelligence,machine learning
-Platform: UNKNOWN
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # SPRT-TANDEM-PyTorch
 This repository contains the official PyTorch implementation of __SPRT-TANDEM__ ([ICASSP2023](https://arxiv.org/abs/2302.09810), [ICML2021](http://proceedings.mlr.press/v139/miyagawa21a.html), and [ICLR2021](https://openreview.net/forum?id=Rhsu5qD36cL)). __SPRT-TANDEM__ is a neuroscience-inspired sequential density ratio estimation (SDRE) algorithm that estimates log-likelihood ratios of two or more hypotheses for fast and accurate sequential data classification. For an intuitive understanding, please refer to the [SPRT-TANDEM tutorial](https://github.com/Akinori-F-Ebihara/SPRT-TANDEM_tutorial).
 
-<div align="center">
-<figure>
-<img src ="./images/SDRE_3class.png" width=70%>  
-</figure>
-</div>
-<p align="center">Figure 1: Example sequential density ratio estimation (SDRE) results on a 3-class multivariate Gaussian dataset.</p>
-
 
 ## Quickstart
 1. To create a new SDRE dataset, run the [Generate_sequential_Gaussian_as_LMDB.ipynb](https://github.com/Akinori-F-Ebihara/SPRT-TANDEM-PyTorch/blob/main/notebooks/Generate_sequential_Gaussian_as_LMDB.ipynb) notebook.
 2. Edit the user editable block of [config_definition.py](https://github.com/Akinori-F-Ebihara/SPRT-TANDEM-PyTorch/blob/main/config/config_definition.py). Specify path to the dataset file created in step 1. Other frequently used entries include SUBPROJECT_NAME_PREFIX (to tag your experiment) and EXP_PHASE (to specify whether you are trying, tuning, or running statistics. See Hyperparameter Tuning for details).
 3. Execute [sprt_tandem_main.py](https://github.com/Akinori-F-Ebihara/SPRT-TANDEM-PyTorch/blob/main/sprt_tandem_main.py).
 
 ## Tested Environment
 ```
 python      3.8.10
 torch       2.0.0
 notebook    6.5.3
 optuna      3.1.0
 ```
-
-## Requirements for Reading This Article
-
-This article is best read using the Chrome browser with the [MathJax Plugin for GitHub](https://chrome.google.com/webstore/detail/mathjax-plugin-for-github/ioemnmodlmafdkllaclgeombjnmnbima?hl=en) installed.
-
 ## Supported Network Architectures  
 We support the two major architectures for processing time series data: Long short-term memory (LSTM, [1]) and Transformer [2]. To avoid the likelihood ratio saturation problem and approach asymptotic optimality (for details, see [Ebihara+, ICASSP2023](https://arxiv.org/abs/2302.09810)), we developed two novel models based on these architectures: B2Bssqrt-TANDEM (based on LSTM) and TANDEMformer (based on Transformer).
 ### LSTM (B2Bsqrt-TANDEM, [ICASSP2023](https://arxiv.org/abs/2302.09810))  
 The LSTM with the back-to-back square root (B2Bsqrt) activation function can be used by setting the following variables: 
 
 - MODEL_BACKBONE: "LSTM"
 - ACTIVATION_OUTPUT: "B2Bsqrt"  
@@ -52,21 +26,14 @@
 
 \begin{align}
 f_{\mathrm{B2Bsqrt}}(x) := \mathrm{sign}(x)(\sqrt{\alpha+|x|}-\sqrt{\alpha})
 \end{align}
 
 Where $\alpha$ is a hyperparameter. 
 
-<div align="center">
-<figure>
-<img src ="./images/Conceptual_figure_B2Bsqrt.png" width=60%>  
-</figure>
-</div>
-<p align="center">Figure 2: Conceptual figure showing the LSTM cell equipped with the B2Bsqrt activation function. B2Bsqrt can be used as an alternative to the tanh function. With an unbounded range and a finite gradient at the origin, B2Bsqrt prevents the saturation problem while enabling stable training.</p>
-
 
 ### Transformer (TANDEMformer, [ICASSP2023](https://arxiv.org/abs/2302.09810))  
 The Transformer is equipped with the Normalized Summation Pooling (NSP) layer, which is incorporated by default.
 
 Let $X_i^{(t, t+w)}$ be subtokens sampled with a sliding window of size $w \in [N]$, and let $Z_i^{(t, t+w)}:=\{z_i^{(s)}\}^{t+w}_{s=t}$ be the subtokens mixed with self-attention. Given the Markov order $N$, the \texttt{NSP} layer is defined as:
 
 \begin{align}
@@ -74,20 +41,14 @@
 \end{align}
 
 To use it, set the following variable:
 
 - MODEL_BACKBONE: "Transformer"
 
 
-<div align="center">
-<figure>
-<img src ="./images/Conceptual_figure_TANDEMformer.png" width=50%>  
-</figure>
-</div>
-<p align="center">Figure 3: Conceptual figure illustrates the Transformer block equipped with the NSP layer. First, tokens are extracted using a sliding window and then mixed with self-attention. The normalized summation pooling layer then takes the sum of the tokens and divides them by a constant, which is the maximum size of the sliding window.</p>  
 
 ## Supported Loss Functions for SDRE
 SPRT-TANDEM uses both the loss for sequential likelihood ratio estimation (SDRE) and (multiplet-) cross-entropy loss ([ICLR2021](https://openreview.net/forum?id=Rhsu5qD36cL)). The two functions, LSEL and LLLR, are supported loss function for SDRE. To choose the loss function, set the following variables:
 
 - LLLR_VERSION: "LSEL" or "LLLR"
 
 Additionally, modify the values of PARAM_LLR_LOSS and PARAM_MULTIPLET_LOSS to achieve the desired balance between likelihood estimation and cross-entropy loss.
@@ -104,20 +65,14 @@
 \begin{align}
 \hat{L}_{\mathrm{\text{LLLR}}} (\mathbb{\theta}; S) := \mathbb{E} \left[ \left| y - \sigma\left( \hat{\lambda}\_{k,l}   ( X_i^{(1,t)}; \theta) \right) \right| \right]
 \end{align}
 
 ## Order N of Markov assumption
 The Markov order $N$ is used to determine the length of the sliding window that extracts a subset from the entire feature vector of a time series. $N$ is a convenient hyperparameter that incorporates prior knowledge of the time series. An optimal $N$ can be found either based on the \textit{specific time scale} or through hyperparameter tuning. The specific time scale characterizes the data class, e.g., long temporal action such as UCF101 has a long specific time scale, while a spoofing attack such as SiW has a short specific time scale (because one frame can have sufficient information of the attack). Setting $N$ equal to the specific time scale usually works best. Alternatively, $N$ can be objectively chosen using a hyperparameter tuning algorithm such as Optuna, just like other hyperparameters. Because $N$ is only related to the temporal integrator after feature extraction, optimizing it is not computationally expensive.
 
-<div align="center">
-<figure>
-<img src ="./images/Conceptual_figure_streamline.png" width=70%>  
-</figure>
-</div>
-<p align="center">Figure 4: Conceptual figure showing the streamline of online SDRE. A subset of the time series' feature vectors is extracted based on the order of Markov assumption, N. </p>
 
 The log-likelihood ratio is estimated from a subset of the feature vectors extracted using a sliding window of size $N$. This estimation is classification-based. Specifically, the temporal integrator is trained to output class logits, which are then used to update the log-likelihood ratio at each time step based on the TANDEM formula.
 ### TANDEM formula ([ICLR2021](https://openreview.net/forum?id=Rhsu5qD36cL))
 \begin{align}
 &\ \log \left(
 \frac{p(x^{(1)},x^{(2)}, ..., x^{(t)}| y=1)}{p(x^{(1)},x^{(2)}, ..., x^{(t)}| y=0)}
 \right)\nonumber \newline
@@ -201,20 +156,14 @@
 - Optuna_databases: Optuna .db file is stored here.
 - TensorBoard_events: TensorBard event files are saved here.
 - checkpoints: trained parameters are saved as .py files when the best optimation target value is updated.
 - stdout_logs: standard output strings are saved as .log files.
 
 The plot below shows an example image saved in a TensorBoard event file. Note that you can avoid saving figures by setting IS_SAVE_FIGURE=False.
 
-<div align="center">
-<figure>
-<img src ="./images/example_tensorboard.png" width=100%>  
-</figure>
-</div>
-<p align="center">Figure 5: Example image saved in a TensorBoard event file. (left and center) Estimated LLR trajectories and Ground-truth LLR trajectories of 3-class multidimensional Gaussian dataset. (right) Speed-accuracy tradeoff (SAT) curve calculated by running the SPRT algorithm.</p>
 
 Note that "Class $a$ vs. $b$ at $y=a$" indicates that the plotted LLR shows $\log{p(X|y=a) / p(X|y=b)}$, when the ground truth label is $y=a$. 
 
 ## Citation
 ___Please cite the orignal paper(s) if you use the whole or a part of our codes.___
 
 ```
@@ -252,9 +201,7 @@
 3. A. Vaswani, N. Shazeer, N. Parmar, J. Uszkoreit, L. Jones, A. N. Gomez, L. u. Kaiser, and I. Polosukhin, “Attention is all you need,” in NeurIPS, 2017, vol. 30, pp. 5998–6008.
 
 ## Contacts
 SPRT-TANDEM marks its 4th anniversary. What started as a small project has now become a huge undertaking that we never imagined. Due to its complexity, it is difficult for me to explain all the details in this README section. Please feel free to reach out to me anytime if you have any questions.
 - email: aebihara[at]nec.com
 - twitter: [@non_iid](http/twitter.com/non_iid)
 - GitHub issues: see the link above or click [here](https://github.com/Akinori-F-Ebihara/SPRT-TANDEM-PyTorch/issues)
-
-
```

### Comparing `SPRT-TANDEM-0.1.2/setup.py` & `SPRT-TANDEM-0.1.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,26 +5,27 @@
 with open(
     path.join(path.abspath(path.dirname(__file__)), "README.md"), encoding="utf-8"
 ) as f:
     long_description = f.read()
 
 setup(
     name="SPRT-TANDEM",
-    version="0.1.2",
+    version="0.1.3",
     license="MIT",
-    description="SPRT-TANDEM for sequential density ratio estimation to simultaneously optimize speed and accuracy of early-classification.",
+    description="SPRT-TANDEM for sequential density ratio estimation to simultaneously optimize both speed and accuracy of early-classification.",
     author="Akinori F. Ebihara",
     author_email="aebihara@nec.com",
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     include_package_data=True,
     url="https://github.com/Akinori-F-Ebihara/SPRT-TANDEM-PyTorch",
     keywords=[
-        "Sequential Probability Ratio Test" "likelihood ratio",
+        "Sequential Probability Ratio Test",
+        "likelihood ratio",
         "density ratio estimation",
         "early classification",
         "artificial intelligence",
         "machine learning",
     ],
     install_requires=["torch", "torchinfo", "optuna", "loguru"],
     python_requires=">=3.8",
```

### Comparing `SPRT-TANDEM-0.1.2/tandem/sprt_tandem_main.py` & `SPRT-TANDEM-0.1.3/tandem/sprt_tandem_main.py`

 * *Files identical despite different names*

