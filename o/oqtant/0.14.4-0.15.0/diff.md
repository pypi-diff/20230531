# Comparing `tmp/oqtant-0.14.4.tar.gz` & `tmp/oqtant-0.15.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oqtant-0.14.4.tar", max compression
+gzip compressed data, was "oqtant-0.15.0.tar", max compression
```

## Comparing `oqtant-0.14.4.tar` & `oqtant-0.15.0.tar`

### file list

```diff
@@ -1,30 +1,29 @@
--rw-r--r--   0        0        0    11341 2023-05-18 18:21:57.682992 oqtant-0.14.4/LICENSE
--rw-r--r--   0        0        0     2458 2023-05-18 18:25:51.795428 oqtant-0.14.4/README.md
--rw-r--r--   0        0        0     7953 2023-05-18 18:26:15.187472 oqtant-0.14.4/documentation/INSTALL.md
--rw-r--r--   0        0        0     4436 2023-05-18 18:23:47.003196 oqtant-0.14.4/documentation/albert_api_docs.md
--rw-r--r--   0        0        0    10947 2023-05-18 18:26:15.187472 oqtant-0.14.4/documentation/job_analysis_docs.md
--rw-r--r--   0        0        0    26364 2023-05-18 18:21:57.682992 oqtant-0.14.4/documentation/main.css
--rw-r--r--   0        0        0     4436 2023-05-18 18:26:15.187472 oqtant-0.14.4/documentation/oqtant_api_docs.md
--rw-r--r--   0        0        0    10316 2023-05-18 18:23:54.771210 oqtant-0.14.4/documentation/oqtant_client_docs.md
--rw-r--r--   0        0        0    15152 2023-05-18 18:27:49.315647 oqtant-0.14.4/documentation/tutorials/tutorial_1_bec_jobs.ipynb
--rw-r--r--   0        0        0     9895 2023-05-18 18:26:15.187472 oqtant-0.14.4/documentation/tutorials/tutorial_1_bec_jobs.md
--rw-r--r--   0        0        0    14537 2023-05-18 18:27:49.311647 oqtant-0.14.4/documentation/tutorials/tutorial_2_barrier_jobs.ipynb
--rw-r--r--   0        0        0     9553 2023-05-18 18:26:15.187472 oqtant-0.14.4/documentation/tutorials/tutorial_2_barrier_jobs.md
--rw-r--r--   0        0        0    31799 2023-05-18 18:27:49.343647 oqtant-0.14.4/documentation/tutorials/tutorial_3_abstractions.ipynb
--rw-r--r--   0        0        0    21972 2023-05-18 18:26:15.187472 oqtant-0.14.4/documentation/tutorials/tutorial_3_abstractions.md
--rw-r--r--   0        0        0    13266 2023-05-18 18:27:49.347647 oqtant-0.14.4/documentation/tutorials/tutorial_4_experiment.ipynb
--rw-r--r--   0        0        0     9097 2023-05-18 18:26:15.191472 oqtant-0.14.4/documentation/tutorials/tutorial_4_experiment.md
--rw-r--r--   0        0        0    16999 2023-05-18 18:27:49.311647 oqtant-0.14.4/documentation/tutorials/tutorial_5_optimization.ipynb
--rw-r--r--   0        0        0    11308 2023-05-18 18:26:15.191472 oqtant-0.14.4/documentation/tutorials/tutorial_5_optimization.md
--rw-r--r--   0        0        0      463 2023-05-18 18:26:15.191472 oqtant-0.14.4/documentation/tutorials/tutorials.md
--rw-r--r--   0        0        0        0 2023-05-18 18:21:57.682992 oqtant-0.14.4/oqtant/__init__.py
--rw-r--r--   0        0        0    21848 2023-05-18 18:26:26.755493 oqtant-0.14.4/oqtant/oqtant_client.py
--rw-r--r--   0        0        0        0 2023-05-18 18:21:57.682992 oqtant-0.14.4/oqtant/schemas/__init__.py
--rw-r--r--   0        0        0    17813 2023-05-18 18:26:26.755493 oqtant-0.14.4/oqtant/schemas/job.py
--rw-r--r--   0        0        0     1002 2023-05-18 18:21:57.682992 oqtant-0.14.4/oqtant/settings.py
--rw-r--r--   0        0        0        0 2023-05-18 18:21:57.682992 oqtant-0.14.4/oqtant/util/__init__.py
--rw-r--r--   0        0        0     2805 2023-05-18 18:26:26.759493 oqtant-0.14.4/oqtant/util/auth.py
--rw-r--r--   0        0        0     1023 2023-05-18 18:21:57.682992 oqtant-0.14.4/oqtant/util/exceptions.py
--rw-r--r--   0        0        0      474 2023-05-18 18:21:57.682992 oqtant-0.14.4/oqtant/util/server.py
--rw-r--r--   0        0        0     3203 2023-05-18 18:26:45.991529 oqtant-0.14.4/pyproject.toml
--rw-r--r--   0        0        0     3739 1970-01-01 00:00:00.000000 oqtant-0.14.4/PKG-INFO
+-rw-r--r--   0        0        0    11341 2023-05-02 20:10:18.126527 oqtant-0.15.0/LICENSE
+-rw-r--r--   0        0        0     2470 2023-05-31 16:33:52.539128 oqtant-0.15.0/README.md
+-rw-r--r--   0        0        0     8005 2023-05-31 16:33:52.539128 oqtant-0.15.0/documentation/INSTALL.md
+-rw-r--r--   0        0        0    10904 2023-05-31 16:33:52.539128 oqtant-0.15.0/documentation/job_analysis_docs.md
+-rw-r--r--   0        0        0     4429 2023-05-31 16:33:52.539128 oqtant-0.15.0/documentation/oqtant_api_docs.md
+-rw-r--r--   0        0        0    10273 2023-05-31 16:33:52.539128 oqtant-0.15.0/documentation/oqtant_client_docs.md
+-rw-r--r--   0        0        0    14940 2023-05-31 16:33:52.539128 oqtant-0.15.0/documentation/walkthroughs/walkthrough_1_bec_jobs.ipynb
+-rw-r--r--   0        0        0    10097 2023-05-31 16:33:52.539128 oqtant-0.15.0/documentation/walkthroughs/walkthrough_1_bec_jobs.md
+-rw-r--r--   0        0        0    14392 2023-05-31 16:33:52.539128 oqtant-0.15.0/documentation/walkthroughs/walkthrough_2_barrier_jobs.ipynb
+-rw-r--r--   0        0        0     9745 2023-05-31 16:33:52.539128 oqtant-0.15.0/documentation/walkthroughs/walkthrough_2_barrier_jobs.md
+-rw-r--r--   0        0        0    31808 2023-05-31 16:33:52.543128 oqtant-0.15.0/documentation/walkthroughs/walkthrough_3_abstractions.ipynb
+-rw-r--r--   0        0        0    22140 2023-05-31 16:33:52.543128 oqtant-0.15.0/documentation/walkthroughs/walkthrough_3_abstractions.md
+-rw-r--r--   0        0        0    17763 2023-05-31 16:33:52.543128 oqtant-0.15.0/documentation/walkthroughs/walkthrough_4_experiment.ipynb
+-rw-r--r--   0        0        0    12609 2023-05-31 16:33:52.543128 oqtant-0.15.0/documentation/walkthroughs/walkthrough_4_experiment.md
+-rw-r--r--   0        0        0    16851 2023-05-31 16:33:52.543128 oqtant-0.15.0/documentation/walkthroughs/walkthrough_5_optimization.ipynb
+-rw-r--r--   0        0        0    11560 2023-05-31 16:33:52.543128 oqtant-0.15.0/documentation/walkthroughs/walkthrough_5_optimization.md
+-rw-r--r--   0        0        0      452 2023-05-31 16:33:52.543128 oqtant-0.15.0/documentation/walkthroughs/walkthroughs.md
+-rw-r--r--   0        0        0        0 2023-05-16 16:24:46.335446 oqtant-0.15.0/oqtant/__init__.py
+-rw-r--r--   0        0        0    21848 2023-05-25 15:03:01.160254 oqtant-0.15.0/oqtant/oqtant_client.py
+-rw-r--r--   0        0        0        0 2023-05-16 16:24:46.335446 oqtant-0.15.0/oqtant/schemas/__init__.py
+-rw-r--r--   0        0        0    17813 2023-05-18 18:23:18.769901 oqtant-0.15.0/oqtant/schemas/job.py
+-rw-r--r--   0        0        0      994 2023-05-25 15:03:01.160254 oqtant-0.15.0/oqtant/settings.py
+-rw-r--r--   0        0        0        0 2023-05-16 16:24:46.335446 oqtant-0.15.0/oqtant/util/__init__.py
+-rw-r--r--   0        0        0     2805 2023-05-18 18:23:18.769901 oqtant-0.15.0/oqtant/util/auth.py
+-rw-r--r--   0        0        0     1023 2023-05-16 16:24:46.335446 oqtant-0.15.0/oqtant/util/exceptions.py
+-rw-r--r--   0        0        0      474 2023-05-16 16:24:46.335446 oqtant-0.15.0/oqtant/util/server.py
+-rw-r--r--   0        0        0     3203 2023-05-31 16:33:52.543128 oqtant-0.15.0/pyproject.toml
+-rw-r--r--   0        0        0     3807 1970-01-01 00:00:00.000000 oqtant-0.15.0/setup.py
+-rw-r--r--   0        0        0     3751 1970-01-01 00:00:00.000000 oqtant-0.15.0/PKG-INFO
```

### Comparing `oqtant-0.14.4/LICENSE` & `oqtant-0.15.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oqtant-0.14.4/README.md` & `oqtant-0.15.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -45,12 +45,12 @@
 
 - To analyze job objects and use Oqtant's job analysis library, reference the OqtantJob class documentation.
 
 Need help? Found a bug? Contact <albert@infleqtion.com> for support. Thank you!
 
 ## 📓 Documentation
 
-- [Getting started](https://gitlab.com/infleqtion/albert/oqtant/-/blob/main/documentation/INSTALL.md) (installation, setting up the environment, How to run the tutorial notebooks)
-- [Tutorials](https://gitlab.com/infleqtion/albert/oqtant/-/blob/main/documentation/tutorials/tutorials.md) (demos for creating and submitting jobs)
+- [Getting started](https://gitlab.com/infleqtion/albert/oqtant/-/blob/main/documentation/INSTALL.md) (installation, setting up the environment, how to run the walkthrough notebooks)
+- [Walkthroughs](https://gitlab.com/infleqtion/albert/oqtant/-/blob/main/documentation/walkthroughs/walkthroughs.md) (demos for creating and submitting jobs)
 - [Oqtant API docs](https://gitlab.com/infleqtion/albert/oqtant/-/blob/main/documentation/oqtant_api_docs.md)
 - [Oqtant API docs](https://gitlab.com/infleqtion/albert/oqtant/-/blob/main/documentation/albert_api_docs.md)
 - [Job Analysis docs](https://gitlab.com/infleqtion/albert/oqtant/-/blob/main/documentation/job_analysis_docs.md)
```

### Comparing `oqtant-0.14.4/documentation/INSTALL.md` & `oqtant-0.15.0/documentation/INSTALL.md`

 * *Files 8% similar despite different names*

```diff
@@ -134,25 +134,25 @@
 
 3. Once activated run the following command to install Oqtant and it's dependencies:
 
    ```
    pip install oqtant
    ```
 
-# Tutorial Notebooks
+# Walkthrough Notebooks
 
-Getting started with Oqtant is easy using the tutorial notebooks (your Oqtant installation already includes the latest version of Jupyter Notebook). These tutorials will walk you through the basic functions of using Oqtant to interact with the Oqtant hardware. Feel free to use these as a starting point for your own code: edit, rename, share… they are yours.
+Getting started with Oqtant is easy using the walkthrough notebooks (your Oqtant installation already includes the latest version of Jupyter Notebook). These walkthroughs will walk you through the basic functions of using Oqtant to interact with the Oqtant hardware. Feel free to use these as a starting point for your own code: edit, rename, share… they are yours.
 
-## Downloading Tutorial Notebooks
+## Downloading Walkthrough Notebooks
 
-You can download a copy of our tutorial notebooks from our GitLab project located here: TODO
+You can download a copy of our walkthrough notebooks from our GitLab project located here: https://gitlab.com/infleqtion/albert/oqtant/-/tree/main/documentation
 
-## Running Tutorial Notebooks
+## Running Walkthrough Notebooks
 
-To start up Jupyter and begin using the tutorial notebooks run the following command in the same directory as the notebook files you have downloaded:
+To start up Jupyter and begin using the walkthrough notebooks run the following command in the same directory as the notebook files you have downloaded:
 
 ```
 jupyter notebook
 ```
 
 - This will open a tab in your default web browser with a file explorer type interface.
 - Using this interface navigate to the location of the provided notebooks and select one to open.
@@ -162,16 +162,14 @@
 
 If you run into `ModuleNotFound` errors when running cells within the notebooks it can be a sign that the notebooks are not using the correct version of python. To fix this close the notebook server, run the following, then restart the notebooks:
 
 ```
 python -m ipykernel install --user
 ```
 
-**Note: You may notice that each tutorial notebook has two files with different extensions (.ipynb and .md). The files you want to be using with Jupyter are the .ipynb files as these are what runs the underlying Oqtant python code. The .md files are static markdown representations of the tutorial notebooks that can be used as reference if needed. The .md files are safe to delete**
+**Note: You may notice that each walkthrough notebook has two files with different extensions (.ipynb and .md). The files you want to be using with Jupyter are the .ipynb files as these are what runs the underlying Oqtant python code. The .md files are static markdown representations of the walkthrough notebooks that can be used as reference if needed. The .md files are safe to delete**
 
 ## Authentication
 
-At the top of each tutorial notebook you will see a step called `Sign into Oqtant`. This step is required for all notebook and client operations to ensure only authorized parties are accessing Oqtant.
+At the top of each walkthrough notebook you will see a step called `Sign into Oqtant`. This step is required for all notebook and client operations to ensure only authorized parties are accessing Oqtant.
 
 This step will require that you already have an account created for Oqtant. If you have not done so yet visit https://albert-dev.coldquanta.com and follow the registration steps to get set up.
-
-<link href="main.css" rel="stylesheet" />
```

### Comparing `oqtant-0.14.4/documentation/albert_api_docs.md` & `oqtant-0.15.0/documentation/oqtant_api_docs.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-# Albert REST API
+# Oqtant REST API
 
-The Albert REST API is the RESTful backend to both Oqtant and the Albert Web App. It's API provides endpoints that can be interacted with via Oqtant's Client API to execute and expand upon the same functionality found in the Albert Web App.
+The Oqtant REST API is the RESTful backend to both Oqtant and the Oqtant Web App. It's API provides endpoints that can be interacted with via Oqtant's Client API to execute and expand upon the same functionality found in the Oqtant Web App.
 
-To see a list of available endpoints and try them out you can visit our [OpenAPI documentation](http://albert-dev.coldquanta.com/api/v1/bert/docs)
+To see a list of available endpoints and try them out you can visit our [OpenAPI documentation](http://albert-dev.coldquanta.com/api/docs)
 
-Communication with the Albert REST API will need to be authorized via your Albert Account. To accomplish this you will need to find your authentication token and provide it when using the OpenAPI documentation. To do this you can follow the steps below:
+Communication with the Oqtant REST API will need to be authorized via your Oqtant Account. To accomplish this you will need to find your authentication token and provide it when using the OpenAPI documentation. To do this you can follow the steps below:
 
 ** Both of these methods requires that oqtant be installed on your system and in a place where your python interpreter can access it. Ideally this would be inside of a virtual environment. For more information on how to set that up refer to our [Installation Guide](INSTALL.md) **
 
 ## Authentication Token via Oqtant Notebooks
 
-When installing Oqtant for the first time you will have received a set of tutorial Jupyter notebooks. Within each of these notebooks you will find that the beginning of each one starts with a step called `Authenticate with Albert`. At the end of this step is a line that contains the following:
+When installing Oqtant for the first time you will have received a set of walkthrough Jupyter notebooks. Within each of these notebooks you will find that the beginning of each one starts with a step called `Authenticate with Oqtant`. At the end of this step is a line that contains the following:
 
 ```python
 token = get_user_token()
 ```
 
-This line is what handles the authorization process for you to begin using Oqtant and as a result the Albert REST API. To be able to use the endpoints available in our OpenAPI documentation you will need to perform the following using the aforementioned step:
+This line is what handles the authorization process for you to begin using Oqtant and as a result the Oqtant REST API. To be able to use the endpoints available in our OpenAPI documentation you will need to perform the following using the aforementioned step:
 
 1. Start up Jupyter
 
    ```shell
    jupyter notebook
    ```
 
-2. Open up one of the tutorial notebooks. Depending on the location you started Jupyter from you may need to navigate the file explorer interface of Jupyter to find them.
+2. Open up one of the walkthrough notebooks. Depending on the location you started Jupyter from you may need to navigate the file explorer interface of Jupyter to find them.
 
 3. In the code cell that contains the import statements and the `get_user_token()` method call, add a new line at the bottom that contains:
 
    ```python
    print(token)
    ```
 
-4. Run the cell in the Jupyter notebook. It will open up a new tab in your default browser where you will be prompted to log in with your Albert Account. Once logged in successfully you can close that tab and return to the Jupyter notebook.
+4. Run the cell in the Jupyter notebook. It will open up a new tab in your default browser where you will be prompted to log in with your Oqtant Account. Once logged in successfully you can close that tab and return to the Jupyter notebook.
 
 5. Now that you are authenticated you can see in the output of the code cell the printed authentication token. Select it all and copy it to your clipboard. This is your token.
 
 ## Authentication Token via Pure Python
 
-While Oqtant comes with a set of tutorial Jupyter notebooks, at its core it is a python library and can be used on its own. To be able to use the endpoint available in our OpenAPI documentation you will need to perform the following inside of a python interpreter:
+While Oqtant comes with a set of walkthrough Jupyter notebooks, at its core it is a python library and can be used on its own. To be able to use the endpoint available in our OpenAPI documentation you will need to perform the following inside of a python interpreter:
 
 1. Inside of a terminal with `oqtant` available open a python interpreter by running `python`
 
 2. Import the `get_user_token`method
 
    ```python
    from oqtant.util.auth import get_user_token
@@ -50,30 +50,30 @@
 
 3. Call the imported method and assign the result to a variable
 
    ```python
    token = get_user_token()
    ```
 
-4. A new tab in your default browser will open where you will be prompted to log in with your Albert Account. Once logged in successfully you can close that tab and return to your python interpreter.
+4. A new tab in your default browser will open where you will be prompted to log in with your Oqtant Account. Once logged in successfully you can close that tab and return to your python interpreter.
 
 5. Print the contents of the variable
 
    ```python
    print(token)
    ```
 
 6. Select all of the output from the printed variable and copy it to your clipboard. This is your token.
 
 ## Authorizing OpenAPI Documentation
 
-Now that you have your authentication token from one of the previous methods you can authorize the OpenAPI documentation to allow for interaction with the Albert REST API endpoints. To do this follow the below steps:
+Now that you have your authentication token from one of the previous methods you can authorize the OpenAPI documentation to allow for interaction with the Oqtant REST API endpoints. To do this follow the below steps:
 
-1. Navigate to our [OpenAPI documentation](https://albert-dev.coldquanta.com/api/v1/bert/docs)
+1. Navigate to our [OpenAPI documentation](https://albert-dev.coldquanta.com/api/docs)
 
-2. Once loaded you will see a list of the endpoints provided by the Albert REST API. Most of these will show a lock icon next to them on the right-hand side. Endpoints with a lock will require the authentication token we retrieved from the above methods.
+2. Once loaded you will see a list of the endpoints provided by the Oqtant REST API. Most of these will show a lock icon next to them on the right-hand side. Endpoints with a lock will require the authentication token we retrieved from the above methods.
 
 3. Near the top right-hand side of the page you will see a green button with the text `Authorize`. Clicking on this will open a pop-up with a form to input `HTTPBearer`inside.
 
 4. Paste the token from our clipboard into this field and click `Authorize`.
 
 5. You should now see a message that says `Authorized`. You can close the pop-up and begin using the endpoints that require an authentication token.
```

### Comparing `oqtant-0.14.4/documentation/job_analysis_docs.md` & `oqtant-0.15.0/documentation/job_analysis_docs.md`

 * *Files 1% similar despite different names*

```diff
@@ -317,9 +317,7 @@
     list parameters: [GpOD, sigx, sigy, TFpOD, rx, ry, xc, yc, os]
 
     G_pOD, TF_pOD = 0.25, 1              # peak OD of Gaussian and TF
     xc, yc = 0, 0                        # center of cloud in x, y-direction
     sigx, sigy = 8, 8                    # Gaussian widths
     rx, ry = 4, 6                        # TF widths
     os = 0.1                             # uniform background level
-
-<link href="main.css" rel="stylesheet" />
```

### Comparing `oqtant-0.14.4/documentation/oqtant_client_docs.md` & `oqtant-0.15.0/documentation/oqtant_client_docs.md`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
     job_id (str): this is the external_id of the job to fetch
     run (Union[int, None]): optional argument if caller wishes to only has a single run returned
     include_notes (bool): optional argument if caller wishes to include any notes associated with OqtantJob inputs. Defaults to False is not provided
 Returns:
     Dict: a Dict representation of an OqtantJob instance
 ```
 
-### generate_albert_job
+### generate_oqtant_job
 
 Generates an instance of OqtantJob from the provided dictionary that contains the job details and input. Will validate the values and raise an informative error if any violations are found. This function is a member of `OqtantClient`
 
 ```
 Args:
     job (Dict): dictionary containing job details and input
 Returns:
@@ -202,9 +202,7 @@
 Utility function to write an OqtantJob instance to a file. Requires the full filepath including the name of the file the write. Files that already exist will cannot be overwritten. This function is a member of `OqtantClient`
 
 ```
 Args:
     job (OqtantJob): the OqtantJob instance to write to file
     filepath (str): the full path to the file to write, including the name of the file
 ```
-
-<link href="main.css" rel="stylesheet" />
```

### Comparing `oqtant-0.14.4/documentation/tutorials/tutorial_1_bec_jobs.ipynb` & `oqtant-0.15.0/documentation/walkthroughs/walkthrough_1_bec_jobs.ipynb`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9826839981006648%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, '# Oqtant Walkthrough 1: Getting Started #\\n'), (4, "*

 * *            "'For more information about Oqtant refer to our documentation: "*

 * *            "https://gitlab.com/infleqtion/albert/oqtant/-/blob/main/README.md\\n'), (5, '\\n'), "*

 * *            "(6, '*Batch job functionality is available for users with a subscription tier of "*

 * *            "EXPLORER or INNOVATOR.*')], delete: [4, 0]}, delete: ['attachments']}, 1: {delete: "*

 * *            "['attachments']}, 3: {delete: [ […]*

```diff
@@ -1,23 +1,23 @@
 {
     "cells": [
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Oqtant Tutorial 1: Getting Started #\n",
+                "# Oqtant Walkthrough 1: Getting Started #\n",
                 "\n",
                 "### This walkthrough covers authorizing an Oqtant session using the Oqtant client, generating, running and viewing the results of a job. ###\n",
                 "\n",
-                "For more information about Oqtant refer to our documentation: https://albert-dev.coldquanta.com/oqtant/manual.md"
+                "For more information about Oqtant refer to our documentation: https://gitlab.com/infleqtion/albert/oqtant/-/blob/main/README.md\n",
+                "\n",
+                "*Batch job functionality is available for users with a subscription tier of EXPLORER or INNOVATOR.*"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Authenticate with Oqtant\n",
                 "\n",
                 "## Before you can view and submit jobs you must first authenticate with your Oqtant account\n",
                 "\n",
@@ -44,15 +44,14 @@
                 "    round_sig\n",
                 ")\n",
                 "\n",
                 "token = get_user_token()"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Creating a Oqtant Client Instance ##\n",
                 "\n",
                 "### After successful login, create an authorized session with the Oqtant Client ###\n",
                 "- the oqtant_client interacts with the albert server to perform remote lab functions.\n",
@@ -65,15 +64,14 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "oqtant_client = get_oqtant_client(token)"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Generate parameters to create a job ##\n",
                 "Every Oqtant job is specified by a **name**, **job_type**, and a dictionary of input parameters. Below is an example with default parameters for a BEC job:"
             ]
         },
@@ -102,20 +100,19 @@
                 "                \"optical_landscape\": None,\n",
                 "                \"lasers\": None,\n",
                 "            },\n",
                 "        }\n",
                 "    ],\n",
                 "}\n",
                 "\n",
-                "example_bec_job = oqtant_client.generate_albert_job(job=default_bec_job)\n",
+                "example_bec_job = oqtant_client.generate_oqtant_job(job=default_bec_job)\n",
                 "print(example_bec_job)"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Add notes to your job input (Optional) ##\n",
                 "Every Oqtant job input can hold notes up to 500 characters long. These notes can be used to add context and additional information to each input. Notes remain tied to their inputs and can be referenced later. To add a note to a job input simply provide a string value to your desired input object like below:"
             ]
         },
@@ -123,19 +120,18 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# In this example we are only working with a single input\n",
                 "# so we will add the note to the first and only input in the array\n",
-                "example_bec_job.inputs[0].notes = \"This is an example BEC job created from Oqtant tutorial #1\""
+                "example_bec_job.inputs[0].notes = \"This is an example BEC job created from Oqtant walkthrough #1\""
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Submit the job to run on the Oqtant hardware ##\n",
                 "\n",
                 "**run_jobs(job_list=jobs)** takes a list of OqtantJob objects and submits them to the online queue for Oqtant Jobs. For each OqtantJob added to the queue a unique UUID is generated and associated to the job.\n",
                 "\n",
@@ -158,15 +154,14 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "[example_bec_job_uuid] = oqtant_client.run_jobs(job_list=[example_bec_job], track_status=True)"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Best practices for referencing ##"
             ]
         },
         {
@@ -176,15 +171,14 @@
             "outputs": [],
             "source": [
                 "with open('example_bec_job-walkthrough0.txt', 'w') as f:\n",
                 "    f.write(example_bec_job_uuid)"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Check the status of this session's active jobs ##\n",
                 "\n",
                 "The **oqtant_client** object contains a dictionary (indexed by job_id) of all the active jobs from the current session. \n",
                 "\n",
@@ -219,15 +213,14 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "oqtant_client.see_active_jobs()"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Wait for job results ##\n",
                 "\n",
                 "If your job is in the PENDING or RUNNING state, wait for 1 minute and update/see active jobs again. When the job \"Example Ultracold Matter Generator Job\" shows status COMPLETE, proceed to the next code block\n",
                 "\n",
@@ -246,15 +239,14 @@
             "outputs": [],
             "source": [
                 "example_bec_job = oqtant_client.active_jobs[example_bec_job_uuid]\n",
                 "print(example_bec_job)"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Loading job results from a previous session ###\n",
                 "\n",
                 "When Oqtant is offline or you wish to analyze jobs from a previous run, use the job id to access it from the database and save it to the session's active_jobs."
             ]
@@ -268,15 +260,14 @@
                 "# for jobs with multiple runs add `run=<int>` where <int> equals the input you wish to view. defaults to the first run\n",
                 "oqtant_client.load_job_from_id(example_bec_job_uuid)\n",
                 "# access job from active_jobs\n",
                 "example_bec_job = oqtant_client.active_jobs[example_bec_job_uuid]"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Accessing job results - TOF images ##\n",
                 "\n",
                 "Job results for jobs run with TOF imaging contain the following fields:"
             ]
@@ -288,15 +279,14 @@
             "outputs": [],
             "source": [
                 "for key in example_bec_job.inputs[0].output.values.dict().keys():\n",
                 "    print(key)"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Viewing TOF images and slice plots ##\n",
                 "\n",
                 "The Oqtant system automatically fits a bimodal distribution to TOF images. The parameters of the fit model are used to calculate statistics about your atom cloud: temperature, number of atoms per phase, and total number of atoms. \n",
                 "\n",
@@ -322,15 +312,14 @@
                 "plt.grid(visible=True)\n",
                 "plt.colorbar(TOF_plot, shrink=0.8)\n",
                 "\n",
                 "plt.show()"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Viewing atom cloud statistics ##\n",
                 "\n",
                 "The Oqtant system performs an automated fit to generate atom cloud statistics. To access the calculated atom number, cloud temperature etc:"
             ]
@@ -345,15 +334,14 @@
                 "print(\"temperature (nK):\"+ str(output.temperature_uk))\n",
                 "print(\"total atoms :\"+ str(output.tof_atom_number))\n",
                 "print(\"condensed atoms :\"+ str(output.condensed_atom_number))\n",
                 "print(\"thermal atoms :\"+ str(output.thermal_atom_number))"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Creating jobs based off previous ones ##\n",
                 "\n",
                 "There may be times where you would like to create a new OqtantJob based off of a previous one. In these cases the `oqtant_client` provides a method that retrieves an entire job's input structure to allow for editing and submission. The steps to do this can be found below."
             ]
@@ -380,23 +368,22 @@
                 "# if you wish to include any job notes associated with the existing job input you can run the\n",
                 "# same command above but with the `include_notes` flag set to True\n",
                 "# new_job_stub = oqtant_client.get_job_inputs_without_output(already_submitted_job_id, include_notes=True)\n",
                 "\n",
                 "# from here you can update any of the inputs and the name of the job to your liking\n",
                 "new_job_stub[\"name\"] = \"this is a stub of another job\"\n",
                 "\n",
-                "# at this point 'new_job_stub' can be provided to the 'generate_albert_job' function and then submitted with\n",
+                "# at this point 'new_job_stub' can be provided to the 'generate_oqtant_job' function and then submitted with\n",
                 "# the 'run_jobs' function as demonstrated in previous steps\n",
-                "new_example_bec_job = oqtant_client.generate_albert_job(job=new_job_stub)\n",
+                "new_example_bec_job = oqtant_client.generate_oqtant_job(job=new_job_stub)\n",
                 "print(\"new job object:\")\n",
                 "print(new_example_bec_job)"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## View your current job limits\n",
                 "\n",
                 "Your account provides you with a limited number of jobs which you can run in a given period of time. You can check your limits and current status against those limits via the `oqtant_client.get_limits()` method:"
             ]
@@ -408,15 +395,14 @@
             "outputs": [],
             "source": [
                 "limits = oqtant_client.get_job_limits()\n",
                 "print(limits)"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "If you are running batch jobs, each run is counted as a job against your limit (i.e., a batch job with 10 runs counts as 10 against your limits)."
             ]
         }
     ],
```

### Comparing `oqtant-0.14.4/documentation/tutorials/tutorial_1_bec_jobs.md` & `oqtant-0.15.0/documentation/walkthroughs/walkthrough_1_bec_jobs.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,22 @@
-# Oqtant Tutorial 1: Getting Started
+# Oqtant Walkthrough 1: Getting Started
 
-### This walkthrough covers authorizing an Oqtant session using the Oqtant client, generating, running and viewing the results of a job.
+### This walkthrough covers authorizing an Oqtant session using the Oqtant client, generating, running and viewing the results of a job. ###
 
-For more information about Oqtant refer to our documentation: https://albert-dev.coldquanta.com/oqtant/manual.md
+For more information about Oqtant refer to our documentation: https://gitlab.com/infleqtion/albert/oqtant/-/blob/main/README.md
+
+*Batch job functionality is available for users with a subscription tier of EXPLORER or INNOVATOR.*
 
 # Authenticate with Oqtant
 
 ## Before you can view and submit jobs you must first authenticate with your Oqtant account
 
 Run the below cell to be re-directed to our login page and provide your account credentials. Once authenticated you can safely close out that tab and return to this notebook.
 
+
 ```python
 from matplotlib import pyplot as plt
 from lmfit import Model
 import numpy as np
 import inspect
 from oqtant.oqtant_client import get_oqtant_client
 from oqtant.util.auth import get_user_token
@@ -24,29 +27,29 @@
     bimodal_dist_2D,
     round_sig
 )
 
 token = get_user_token()
 ```
 
-## Creating a Oqtant Client Instance
-
-### After successful login, create an authorized session with the Oqtant Client
+## Creating a Oqtant Client Instance ##
 
+### After successful login, create an authorized session with the Oqtant Client ###
 - the oqtant_client interacts with the albert server to perform remote lab functions.
 - the oqtant_client object also contains all the jobs which have been submitted, run, or loaded (from database or file) during this python session
 
+
 ```python
 oqtant_client = get_oqtant_client(token)
 ```
 
-## Generate parameters to create a job
-
+## Generate parameters to create a job ##
 Every Oqtant job is specified by a **name**, **job_type**, and a dictionary of input parameters. Below is an example with default parameters for a BEC job:
 
+
 ```python
 default_bec_job = {
     "name": "Example Ultracold Matter Generator Job",
     "job_type": "BEC",
     "inputs": [
         {
             "values": {
@@ -63,128 +66,136 @@
                 "optical_landscape": None,
                 "lasers": None,
             },
         }
     ],
 }
 
-example_bec_job = oqtant_client.generate_albert_job(job=default_bec_job)
+example_bec_job = oqtant_client.generate_oqtant_job(job=default_bec_job)
 print(example_bec_job)
 ```
 
-## Add notes to your job input (Optional)
-
+## Add notes to your job input (Optional) ##
 Every Oqtant job input can hold notes up to 500 characters long. These notes can be used to add context and additional information to each input. Notes remain tied to their inputs and can be referenced later. To add a note to a job input simply provide a string value to your desired input object like below:
 
+
 ```python
 # In this example we are only working with a single input
 # so we will add the note to the first and only input in the array
-example_bec_job.inputs[0].notes = "This is an example BEC job created from Oqtant tutorial #1"
+example_bec_job.inputs[0].notes = "This is an example BEC job created from Oqtant walkthrough #1"
 ```
 
-## Submit the job to run on the Oqtant hardware
+## Submit the job to run on the Oqtant hardware ##
 
 **run_jobs(job_list=jobs)** takes a list of OqtantJob objects and submits them to the online queue for Oqtant Jobs. For each OqtantJob added to the queue a unique UUID is generated and associated to the job.
 
-The output of **run_jobs()** is a list of the unique UUIDs generated during submission.
+The output of **run_jobs()** is a list of the unique UUIDs generated during submission. 
 
 If you are submitting a list of jobs and wish to wait for the results to return, use the flag **track_status=True**.
 
 If you would like the resulting unique UUIDs to be written to a file for later reference you can do so by providing the following flags:
 
 - **track_status=True**
 - **filename="name_of_file"**
 - **write=True**
 
 When writing to a file be sure to <span style="color:red">not overwrite it</span>
 
+
 ```python
 [example_bec_job_uuid] = oqtant_client.run_jobs(job_list=[example_bec_job], track_status=True)
 ```
 
-## Best practices for referencing
+## Best practices for referencing ##
+
 
 ```python
 with open('example_bec_job-walkthrough0.txt', 'w') as f:
     f.write(example_bec_job_uuid)
 ```
 
-## Check the status of this session's active jobs
+## Check the status of this session's active jobs ##
 
-The **oqtant_client** object contains a dictionary (indexed by job_id) of all the active jobs from the current session.
+The **oqtant_client** object contains a dictionary (indexed by job_id) of all the active jobs from the current session. 
 
-**oqtant_client.active jobs** contains jobs that have been submitted with **run_jobs()**, loaded with **load_job_from_id()** or **load_job_from_file()**.
+**oqtant_client.active jobs** contains jobs that have been submitted with **run_jobs()**, loaded with **load_job_from_id()** or **load_job_from_file()**. 
 
 <span style="color:red"> Note: oqtant_client.active_jobs does not automatically include jobs which were submitted on the web app or in a different python session, even if those jobs are currently in the queue to run. </span>
 
-To keep inputs and results organized, all jobs are handled as objects of the **OqtantJob** class.
+To keep inputs and results organized, all jobs are handled as objects of the **OqtantJob** class. 
 
 <span style="color:red"> Note: both BEC and BARRIER job types are represented as OqtantJob objects with different job_type fields </span>
 
-### To access information about a OqtantJob object
+### To access information about a OqtantJob object ###
 
 **EXAMPLEJOB.DESIRED_INFO**
 
 OqtantJob objects have the following relevant fields:
 
-- name
-- job_type
-- status
-- time_submit (datetime object)
-- inputs list (see walkthrough 2 for specifics)
+ - name
+ - job_type
+ - status
+ - time_submit (datetime object)
+ - inputs list (see walkthrough 2 for specifics)
 
-To see all the job information, you can print the object.
+To see all the job information, you can print the object. 
+
+Click [here](https://www.learnpython.org/en/Classes_and_Objects) for an example-based intro to objects and classes in python. 
 
-Click [here](https://www.learnpython.org/en/Classes_and_Objects) for an example-based intro to objects and classes in python.
 
 ```python
 oqtant_client.see_active_jobs()
 ```
 
-## Wait for job results
+## Wait for job results ##
 
 If your job is in the PENDING or RUNNING state, wait for 1 minute and update/see active jobs again. When the job "Example Ultracold Matter Generator Job" shows status COMPLETE, proceed to the next code block
 
-## Loading job results
 
-### From this session
+## Loading job results ##
+
+### From this session ###
 
 When a job is COMPLETE and the active jobs dictionary is updated, the OqtantJob object is automatically populated with the job results. Define a variable to access to job object, or access it by job id directly from the active jobs dictionary.
 
+
 ```python
 example_bec_job = oqtant_client.active_jobs[example_bec_job_uuid]
 print(example_bec_job)
 ```
 
-### Loading job results from a previous session
+### Loading job results from a previous session ###
 
 When Oqtant is offline or you wish to analyze jobs from a previous run, use the job id to access it from the database and save it to the session's active_jobs.
 
+
 ```python
 # for jobs with multiple runs add `run=<int>` where <int> equals the input you wish to view. defaults to the first run
 oqtant_client.load_job_from_id(example_bec_job_uuid)
 # access job from active_jobs
 example_bec_job = oqtant_client.active_jobs[example_bec_job_uuid]
 ```
 
-## Accessing job results - TOF images
+## Accessing job results - TOF images ##
 
 Job results for jobs run with TOF imaging contain the following fields:
 
+
 ```python
 for key in example_bec_job.inputs[0].output.values.dict().keys():
     print(key)
 ```
 
-## Viewing TOF images and slice plots
+## Viewing TOF images and slice plots ##
 
-The Oqtant system automatically fits a bimodal distribution to TOF images. The parameters of the fit model are used to calculate statistics about your atom cloud: temperature, number of atoms per phase, and total number of atoms.
+The Oqtant system automatically fits a bimodal distribution to TOF images. The parameters of the fit model are used to calculate statistics about your atom cloud: temperature, number of atoms per phase, and total number of atoms. 
 
 To view the TOF results in 2D or 1D, use built in functions to plot or access the results directly and plot them yourself.
 
+
 ```python
 example_bec_job.atoms_2dplot(figsize=(6,6))
 
 example_bec_job.atoms_sliceplot()
 
 TOF_data = example_bec_job.get_TOF()
 
@@ -194,30 +205,32 @@
             cmap="nipy_spectral")
 plt.grid(visible=True)
 plt.colorbar(TOF_plot, shrink=0.8)
 
 plt.show()
 ```
 
-## Viewing atom cloud statistics
+## Viewing atom cloud statistics ##
 
 The Oqtant system performs an automated fit to generate atom cloud statistics. To access the calculated atom number, cloud temperature etc:
 
+
 ```python
 output = example_bec_job.inputs[0].output.values
 print("temperature (nK):"+ str(output.temperature_uk))
 print("total atoms :"+ str(output.tof_atom_number))
 print("condensed atoms :"+ str(output.condensed_atom_number))
 print("thermal atoms :"+ str(output.thermal_atom_number))
 ```
 
-## Creating jobs based off previous ones
+## Creating jobs based off previous ones ##
 
 There may be times where you would like to create a new OqtantJob based off of a previous one. In these cases the `oqtant_client` provides a method that retrieves an entire job's input structure to allow for editing and submission. The steps to do this can be found below.
 
+
 ```python
 # identify the job you wish to copy, this can be any job id you want to use.
 # the status of the job does not matter
 already_submitted_job_id = example_bec_job.external_id
 
 # for jobs with multiple input runs add `run=<int>` where <int> equals the input you wish to view.
 # without a targeted input run oqtant will default to the first run
@@ -231,24 +244,25 @@
 # if you wish to include any job notes associated with the existing job input you can run the
 # same command above but with the `include_notes` flag set to True
 # new_job_stub = oqtant_client.get_job_inputs_without_output(already_submitted_job_id, include_notes=True)
 
 # from here you can update any of the inputs and the name of the job to your liking
 new_job_stub["name"] = "this is a stub of another job"
 
-# at this point 'new_job_stub' can be provided to the 'generate_albert_job' function and then submitted with
+# at this point 'new_job_stub' can be provided to the 'generate_oqtant_job' function and then submitted with
 # the 'run_jobs' function as demonstrated in previous steps
-new_example_bec_job = oqtant_client.generate_albert_job(job=new_job_stub)
+new_example_bec_job = oqtant_client.generate_oqtant_job(job=new_job_stub)
 print("new job object:")
 print(new_example_bec_job)
 ```
 
 ## View your current job limits
 
 Your account provides you with a limited number of jobs which you can run in a given period of time. You can check your limits and current status against those limits via the `oqtant_client.get_limits()` method:
 
+
 ```python
 limits = oqtant_client.get_job_limits()
 print(limits)
 ```
 
 If you are running batch jobs, each run is counted as a job against your limit (i.e., a batch job with 10 runs counts as 10 against your limits).
```

### Comparing `oqtant-0.14.4/documentation/tutorials/tutorial_2_barrier_jobs.ipynb` & `oqtant-0.15.0/documentation/walkthroughs/walkthrough_2_barrier_jobs.ipynb`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.983440067415358%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, '# Oqtant Walkthrough 2: Barrier Manipulator #\\n'), (4, "*

 * *            "'For more information about Oqtant refer to our documentation: "*

 * *            "https://gitlab.com/infleqtion/albert/oqtant/-/blob/main/README.md\\n'), (5, '\\n'), "*

 * *            "(6, '*Batch job functionality is available for users with a subscription tier of "*

 * *            "EXPLORER or INNOVATOR.*')], delete: [4, 0]}, delete: ['attachments']}, 1: {'source': "*

 * *            "{insert: [(4, 'Run the be […]*

```diff
@@ -1,31 +1,31 @@
 {
     "cells": [
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Oqtant Tutorial 2: Barrier Manipulator #\n",
+                "# Oqtant Walkthrough 2: Barrier Manipulator #\n",
                 "\n",
                 "### This walkthrough covers authorizing an Oqtant session using the Oqtant client, generating, running and viewing the results of a job. ###\n",
                 "\n",
-                "For more information about Oqtant refer to our documentation: https://albert-dev.coldquanta.com/oqtant/manual.md"
+                "For more information about Oqtant refer to our documentation: https://gitlab.com/infleqtion/albert/oqtant/-/blob/main/README.md\n",
+                "\n",
+                "*Batch job functionality is available for users with a subscription tier of EXPLORER or INNOVATOR.*"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Authenticate with Oqtant\n",
                 "\n",
                 "## Before you can view and submit jobs you must first authenticate with your Oqtant account\n",
                 "\n",
-                "Run the below cell to be re-directed to our login page and provide you account credentials. Once authenticated you can safely close out that tab and return to this notebook."
+                "Run the below cell to be re-directed to our login page and provide your account credentials. Once authenticated you can safely close out that tab and return to this notebook."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -44,15 +44,14 @@
                 "    round_sig\n",
                 ")\n",
                 "\n",
                 "token = get_user_token()"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Creating a Oqtant Client Instance ##\n",
                 "\n",
                 "### After successful login, create an authorized session with the Oqtant Client ###\n",
                 "- the oqtant_client interacts with the albert server to perform remote lab functions. \n",
@@ -65,15 +64,14 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "oqtant_client = get_oqtant_client(token)"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Generate parameters to create a job ##\n",
                 "Every Oqtant job is specified by a **name**, **job_type**, and a dictionary of input parameters. Below is an example with default parameters for a BARRIER job:"
             ]
         },
@@ -119,20 +117,19 @@
                 "                \"optical_landscape\": None,\n",
                 "                \"lasers\": None,\n",
                 "            }\n",
                 "        },\n",
                 "    ],\n",
                 "}\n",
                 "\n",
-                "example_barrier_job = oqtant_client.generate_albert_job(job=default_barrier_job)\n",
+                "example_barrier_job = oqtant_client.generate_oqtant_job(job=default_barrier_job)\n",
                 "print(example_barrier_job)"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Add notes to your job input (Optional) ##\n",
                 "Every Oqtant job input can hold notes up to 500 characters long. These notes can be used to add context and additional information to each input. Notes remain tied to their inputs and can be referenced later. To add a note to a job input simply provide a string value to your desired input object like below:"
             ]
         },
@@ -140,19 +137,18 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# In this example we are only working with a single input\n",
                 "# so we will add the note to the first and only input in the array\n",
-                "example_barrier_job.inputs[0].notes = \"This is an example BARRIER job created from Oqtant tutorial #1\""
+                "example_barrier_job.inputs[0].notes = \"This is an example BARRIER job created from Oqtant walkthrough #1\""
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Submit the job to run on the Oqtant hardware ##\n",
                 "\n",
                 "**run_jobs(job_list=jobs)** takes a list of OqtantJob objects and submits them to the online queue for Oqtant Jobs. For each OqtantJob added to the queue a unique UUID is generated and associated to the job.\n",
                 "\n",
@@ -175,15 +171,14 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "[example_barrier_job_uuid] = oqtant_client.run_jobs(job_list=[example_barrier_job], track_status=True)"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Best practices for referencing"
             ]
         },
         {
@@ -193,15 +188,14 @@
             "outputs": [],
             "source": [
                 "with open('example_barrier_job-walkthrough1.txt', 'w') as f:\n",
                 "    f.write(example_barrier_job_uuid)"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Check the status of this session's active jobs ##\n",
                 "\n",
                 "The **oqtant_client** object contains a dictionary (indexed by job_id) of all the active jobs from the current session. \n",
                 "\n",
@@ -236,15 +230,14 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "oqtant_client.see_active_jobs()"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "\n",
                 "## Loading job results ##\n",
                 "\n",
                 "### From this session ###\n",
@@ -258,15 +251,14 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "example_barrier_job = oqtant_client.active_jobs[example_barrier_job_uuid]"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Loading job results from a previous session ###\n",
                 "\n",
                 "When Oqtant is offline or you wish to analyze jobs from a previous run, use the job id to access it from the database and save it to the session's active_jobs."
             ]
@@ -280,15 +272,14 @@
                 "# for jobs with multiple runs add `run=<int>` where <int> equals the input you wish to view. defaults to the first run\n",
                 "oqtant_client.load_job_from_id(example_barrier_job_uuid)\n",
                 "# access job from active_jobs\n",
                 "example_barrier_job = oqtant_client.active_jobs[example_barrier_job_uuid]"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Accessing job results - IT images ##\n",
                 "\n",
                 "Job results for jobs run with IT imaging contain the following fields:"
             ]
@@ -300,15 +291,14 @@
             "outputs": [],
             "source": [
                 "for key in example_barrier_job.inputs[0].output.values.dict().keys():\n",
                 "    print(key)"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Viewing IT images ##\n",
                 "\n",
                 "To view the TOF results in 2D or 1D, use built in functions to plot or access the results directly and plot them yourself."
             ]
@@ -331,15 +321,14 @@
                 "plt.grid(visible=True)\n",
                 "plt.colorbar(IT_plot)\n",
                 "\n",
                 "plt.show()"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Creating jobs based off previous ones ##\n",
                 "\n",
                 "There may be times where you would like to create a new OqtantJob based off of a previous one. In these cases the `oqtant_client` provides a method that retrieves an entire job's input structure to allow for editing and submission. The steps to do this can be found below."
             ]
@@ -366,17 +355,17 @@
                 "# if you wish to include any job notes associated with the existing job input you can run the\n",
                 "# same command above but with the `include_notes` flag set to True\n",
                 "# new_job_stub = oqtant_client.get_job_inputs_without_output(already_submitted_job_id, include_notes=True)\n",
                 "\n",
                 "# from here you can update any of the inputs and the name of the job to your liking\n",
                 "new_job_stub[\"name\"] = \"this is a stub of another job\"\n",
                 "\n",
-                "# at this point 'new_job_stub' can be provided to the 'generate_albert_job' function and then submitted with\n",
+                "# at this point 'new_job_stub' can be provided to the 'generate_octant_job' function and then submitted with\n",
                 "# the 'run_jobs' function as demonstrated in previous steps\n",
-                "new_example_barrier_job = oqtant_client.generate_albert_job(job=new_job_stub)\n",
+                "new_example_barrier_job = oqtant_client.generate_oqtant_job(job=new_job_stub)\n",
                 "print(\"new job object:\")\n",
                 "print(new_example_barrier_job)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
```

### Comparing `oqtant-0.14.4/documentation/tutorials/tutorial_2_barrier_jobs.md` & `oqtant-0.15.0/documentation/walkthroughs/walkthrough_2_barrier_jobs.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-# Oqtant Tutorial 2: Barrier Manipulator
+# Oqtant Walkthrough 2: Barrier Manipulator
 
-### This walkthrough covers authorizing an Oqtant session using the Oqtant client, generating, running and viewing the results of a job.
+### This walkthrough covers authorizing an Oqtant session using the Oqtant client, generating, running and viewing the results of a job. ###
 
-For more information about Oqtant refer to our documentation: https://albert-dev.coldquanta.com/oqtant/manual.md
+For more information about Oqtant refer to our documentation: https://gitlab.com/infleqtion/albert/oqtant/-/blob/main/README.md
+
+*Batch job functionality is available for users with a subscription tier of EXPLORER or INNOVATOR.*
 
 # Authenticate with Oqtant
 
 ## Before you can view and submit jobs you must first authenticate with your Oqtant account
 
-Run the below cell to be re-directed to our login page and provide you account credentials. Once authenticated you can safely close out that tab and return to this notebook.
+Run the below cell to be re-directed to our login page and provide your account credentials. Once authenticated you can safely close out that tab and return to this notebook.
+
 
 ```python
 from matplotlib import pyplot as plt
 from lmfit import Model
 import numpy as np
 import inspect
 from oqtant.oqtant_client import get_oqtant_client
@@ -24,29 +27,29 @@
     bimodal_dist_2D,
     round_sig
 )
 
 token = get_user_token()
 ```
 
-## Creating a Oqtant Client Instance
-
-### After successful login, create an authorized session with the Oqtant Client
+## Creating a Oqtant Client Instance ##
 
-- the oqtant_client interacts with the albert server to perform remote lab functions.
+### After successful login, create an authorized session with the Oqtant Client ###
+- the oqtant_client interacts with the albert server to perform remote lab functions. 
 - the oqtant_client object also contains all the jobs which have been submitted, run, or loaded (from database or file) during this python session
 
+
 ```python
 oqtant_client = get_oqtant_client(token)
 ```
 
-## Generate parameters to create a job
-
+## Generate parameters to create a job ##
 Every Oqtant job is specified by a **name**, **job_type**, and a dictionary of input parameters. Below is an example with default parameters for a BARRIER job:
 
+
 ```python
 default_barrier_job = {
     "name": "Example Barrier Manipulator Job",
     "job_type": "BARRIER",
     "inputs": [
         {
             "values": {
@@ -80,121 +83,129 @@
                 "optical_landscape": None,
                 "lasers": None,
             }
         },
     ],
 }
 
-example_barrier_job = oqtant_client.generate_albert_job(job=default_barrier_job)
+example_barrier_job = oqtant_client.generate_oqtant_job(job=default_barrier_job)
 print(example_barrier_job)
 ```
 
-## Add notes to your job input (Optional)
-
+## Add notes to your job input (Optional) ##
 Every Oqtant job input can hold notes up to 500 characters long. These notes can be used to add context and additional information to each input. Notes remain tied to their inputs and can be referenced later. To add a note to a job input simply provide a string value to your desired input object like below:
 
+
 ```python
 # In this example we are only working with a single input
 # so we will add the note to the first and only input in the array
-example_barrier_job.inputs[0].notes = "This is an example BARRIER job created from Oqtant tutorial #1"
+example_barrier_job.inputs[0].notes = "This is an example BARRIER job created from Oqtant walkthrough #1"
 ```
 
-## Submit the job to run on the Oqtant hardware
+## Submit the job to run on the Oqtant hardware ##
 
 **run_jobs(job_list=jobs)** takes a list of OqtantJob objects and submits them to the online queue for Oqtant Jobs. For each OqtantJob added to the queue a unique UUID is generated and associated to the job.
 
-The output of **run_jobs()** is a list of the unique UUIDs generated during submission.
+The output of **run_jobs()** is a list of the unique UUIDs generated during submission. 
 
 If you are submitting a list of jobs and wish to wait for the results to return, use the flag **track_status=True**.
 
 If you would like the resulting unique UUIDs to be written to a file for later reference you can do so by providing the following flags:
 
 - **track_status=True**
 - **filename="name_of_file"**
 - **write=True**
 
 When writing to a file be sure to <span style="color:red">not overwrite it</span>
 
+
 ```python
 [example_barrier_job_uuid] = oqtant_client.run_jobs(job_list=[example_barrier_job], track_status=True)
 ```
 
 ## Best practices for referencing
 
+
 ```python
 with open('example_barrier_job-walkthrough1.txt', 'w') as f:
     f.write(example_barrier_job_uuid)
 ```
 
-## Check the status of this session's active jobs
+## Check the status of this session's active jobs ##
 
-The **oqtant_client** object contains a dictionary (indexed by job_id) of all the active jobs from the current session.
+The **oqtant_client** object contains a dictionary (indexed by job_id) of all the active jobs from the current session. 
 
-**oqtant_client.active jobs** contains jobs that have been submitted with **run_jobs()**, loaded with **load_job_from_id()** or **load_job_from_file()**.
+**oqtant_client.active jobs** contains jobs that have been submitted with **run_jobs()**, loaded with **load_job_from_id()** or **load_job_from_file()**. 
 
 <span style="color:red"> Note: oqtant_client.active_jobs does not automatically include jobs which were submitted on the web app or in a different python session, even if those jobs are currently in the queue to run. </span>
 
-To keep inputs and results organized, all jobs are handled as objects of the **OqtantJob** class.
+To keep inputs and results organized, all jobs are handled as objects of the **OqtantJob** class. 
 
 <span style="color:red"> Note: both BEC and BARRIER job types are represented as OqtantJob objects with different job_type fields </span>
 
-### To access information about a OqtantJob object
+### To access information about a OqtantJob object ###
 
 **EXAMPLEJOB.DESIRED_INFO**
 
 OqtantJob objects have the following relevant fields:
 
-- name
-- job_type
-- status
-- time_submit (datetime object)
-- inputs list (see walkthrough 2 for specifics)
+ - name
+ - job_type
+ - status
+ - time_submit (datetime object)
+ - inputs list (see walkthrough 2 for specifics)
+
+To see all the job information, you can print the object. 
 
-To see all the job information, you can print the object.
+Click [here](https://www.learnpython.org/en/Classes_and_Objects) for an example-based intro to objects and classes in python. 
 
-Click [here](https://www.learnpython.org/en/Classes_and_Objects) for an example-based intro to objects and classes in python.
 
 ```python
 oqtant_client.see_active_jobs()
 ```
 
-## Loading job results
 
-### From this session
+## Loading job results ##
+
+### From this session ###
 
 When a job is COMPLETE and the active jobs dictionary is updated, the BEC_job object is automatically populated with the job results. Define a variable to access to job object, or access it by job id directly from the active jobs dictionary.
 
+
 ```python
 example_barrier_job = oqtant_client.active_jobs[example_barrier_job_uuid]
 ```
 
-### Loading job results from a previous session
+### Loading job results from a previous session ###
 
 When Oqtant is offline or you wish to analyze jobs from a previous run, use the job id to access it from the database and save it to the session's active_jobs.
 
+
 ```python
 # for jobs with multiple runs add `run=<int>` where <int> equals the input you wish to view. defaults to the first run
 oqtant_client.load_job_from_id(example_barrier_job_uuid)
 # access job from active_jobs
 example_barrier_job = oqtant_client.active_jobs[example_barrier_job_uuid]
 ```
 
-## Accessing job results - IT images
+## Accessing job results - IT images ##
 
 Job results for jobs run with IT imaging contain the following fields:
 
+
 ```python
 for key in example_barrier_job.inputs[0].output.values.dict().keys():
     print(key)
 ```
 
-## Viewing IT images
+## Viewing IT images ##
 
 To view the TOF results in 2D or 1D, use built in functions to plot or access the results directly and plot them yourself.
 
+
 ```python
 IT_OD = example_barrier_job.get_IT()
 pix_cal = example_barrier_job.pix_cal
 
 plt.figure(figsize=(12,4))
 plt.title("In-Trap Optical Depth")
 IT_plot = plt.imshow(IT_OD,origin="lower",
@@ -203,18 +214,19 @@
 plt.ylabel("Y position (um)")
 plt.grid(visible=True)
 plt.colorbar(IT_plot)
 
 plt.show()
 ```
 
-## Creating jobs based off previous ones
+## Creating jobs based off previous ones ##
 
 There may be times where you would like to create a new OqtantJob based off of a previous one. In these cases the `oqtant_client` provides a method that retrieves an entire job's input structure to allow for editing and submission. The steps to do this can be found below.
 
+
 ```python
 # identify the job you wish to copy, this can be any job id you want to use.
 # the status of the job does not matter
 already_submitted_job_id = example_barrier_job.external_id
 
 # for jobs with multiple input runs add `run=<int>` where <int> equals the input you wish to view.
 # without a targeted input run oqtant will default to the first run
@@ -228,13 +240,13 @@
 # if you wish to include any job notes associated with the existing job input you can run the
 # same command above but with the `include_notes` flag set to True
 # new_job_stub = oqtant_client.get_job_inputs_without_output(already_submitted_job_id, include_notes=True)
 
 # from here you can update any of the inputs and the name of the job to your liking
 new_job_stub["name"] = "this is a stub of another job"
 
-# at this point 'new_job_stub' can be provided to the 'generate_albert_job' function and then submitted with
+# at this point 'new_job_stub' can be provided to the 'generate_octant_job' function and then submitted with
 # the 'run_jobs' function as demonstrated in previous steps
-new_example_barrier_job = oqtant_client.generate_albert_job(job=new_job_stub)
+new_example_barrier_job = oqtant_client.generate_oqtant_job(job=new_job_stub)
 print("new job object:")
 print(new_example_barrier_job)
 ```
```

### Comparing `oqtant-0.14.4/documentation/tutorials/tutorial_3_abstractions.ipynb` & `oqtant-0.15.0/documentation/walkthroughs/walkthrough_3_abstractions.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9982534029236695%*

 * *Differences: {"'cells'": "{3: {'source': ['In this walkthrough, we will explore the structure of jobs that you "*

 * *            'submit to Oqtant.  In an earlier walkthrough, we saw that a basic BEC job could be '*

 * *            'defined by a dictionary structure like\']}, 5: {\'source\': {insert: [(0, "We could '*

 * *            "then feed the above data structure to the API's *generate_Oqtant_job()* function to "*

 * *            'create the job object.  Here, we would like to explore the contents of the underlying '*

 * *            'jo […]*

```diff
@@ -28,15 +28,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "4942af2d",
             "metadata": {},
             "source": [
-                "In this tutorial, we will explore the structure of jobs that you submit to Oqtant.  In an earlier tutorial, we saw that a basic BEC job could be defined by a dictionary structure like"
+                "In this walkthrough, we will explore the structure of jobs that you submit to Oqtant.  In an earlier walkthrough, we saw that a basic BEC job could be defined by a dictionary structure like"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "c08f5594",
             "metadata": {},
@@ -67,15 +67,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "61960d47",
             "metadata": {},
             "source": [
-                "We could then feed the above data structure to the API's *generate_Oqtant_job()* function to create the job object.  Here, we would like to explore the contents of the underlying job data structure more in depth.  The fields that control the behavior of the quantum matter machine are contained as *values* in the *inputs* list ([]).  For now, we will only discuss cases where the *inputs* list contains a single element.  When this list's length is greater than one, it signifies a so-called *batch* job, which will be discussed in a later tutorial.  \n",
+                "We could then feed the above data structure to the API's *generate_Oqtant_job()* function to create the job object.  Here, we would like to explore the contents of the underlying job data structure more in depth.  The fields that control the behavior of the quantum matter machine are contained as *values* in the *inputs* list ([]).  For now, we will only discuss cases where the *inputs* list contains a single element.  When this list's length is greater than one, it signifies a so-called *batch* job, which will be discussed in a later walkthrough.  \n",
                 "\n",
                 "The contents of *values* includes directives on the type of imaging to perform (*image_type* etc.) and how long to run the experiment (*end_time_ms*) after evaporation to BEC is complete.  Also included are various job primitives that can be created and edited as programmable objects in their own right.  These primitives include *rf_evaporation*, *optical_barriers*, *optical_landscape*, and *lasers*.  Much like an *OqtantJob* itself, these constituent primitives are programmatic objects in their own right and can be instantiated and manipulated outside of a job object.  Although not shown explicitly in our simple job data structure above, both *optical_barriers* and *lasers* are lists containing *Barrier* and *Laser* objects, respectively.  These objects will be explored below.  You are likely already familiar with the structure of the *rf_evaporation* data and how defining that data controls the evaporation to BEC in the experiment.  The *optical_landscape* data is a bit more complicated and will be explored in more detail below in a dedicated section.       \n",
                 "\n",
                 "Not all job types support every one of these data structures.  For the basic BEC-type job above, we did not have data entries for barriers, the landscape, or lasers.  BEC jobs, for instance, only support the rf_evaporation primitive.  After all, the purpose of a BEC job is to keep things simple and just focus on the ability to tune the creation of the condensate.  At the next level of complexity, BARRIER jobs support both *rf_evaporation* and *optical_barriers* but not \"optical_landscape\" or \"lasers\".  What data structures are supported by different job types will become clear as those job types are created/used/submitted.  As a preview, please refer to the following table.\n",
                 "\n",
                 "| Job type   | Supports       |                  |                   |        |\n",
                 "|------------|----------------|------------------|-------------------|--------|\n",
@@ -763,15 +763,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.6"
+            "version": "3.11.3"
         },
         "vscode": {
             "interpreter": {
                 "hash": "13fb51af87d45e56afa36501f99325526ec135b669e4eea3c0d0150b11fb593e"
             }
         }
     },
```

### Comparing `oqtant-0.14.4/documentation/tutorials/tutorial_3_abstractions.md` & `oqtant-0.15.0/documentation/walkthroughs/walkthrough_3_abstractions.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 ## Imports
 
+
 ```python
 %matplotlib inline
 from bert_schemas import job as JobSchema
 ```
 
 ## Oqtant jobs and their constituent primitives
 
-In this tutorial, we will explore the structure of jobs that you submit to Oqtant. In an earlier tutorial, we saw that a basic BEC job could be defined by a dictionary structure like
+In this walkthrough, we will explore the structure of jobs that you submit to Oqtant. In an earlier walkthrough, we saw that a basic BEC job could be defined by a dictionary structure like
 
 ```python
 default_bec_job_data = {
     "name": "Example BEC Job",
     "job_type": "BEC",
     "inputs": [
         {
@@ -30,226 +31,240 @@
                 "lasers": None
             }
         }
     ]
 }
 ```
 
-We could then feed the above data structure to the API's _generate_Oqtant_job()_ function to create the job object. Here, we would like to explore the contents of the underlying job data structure more in depth. The fields that control the behavior of the quantum matter machine are contained as _values_ in the _inputs_ list ([]). For now, we will only discuss cases where the _inputs_ list contains a single element. When this list's length is greater than one, it signifies a so-called _batch_ job, which will be discussed in a later tutorial.
+We could then feed the above data structure to the API's _generate_oqtant_job()_ function to create the job object. Here, we would like to explore the contents of the underlying job data structure more in depth. The fields that control the behavior of the quantum matter machine are contained as _values_ in the _inputs_ list ([]). For now, we will only discuss cases where the _inputs_ list contains a single element. When this list's length is greater than one, it signifies a so-called _batch_ job, which will be discussed in a later walkthrough.
 
-The contents of _values_ includes directives on the type of imaging to perform (_image_type_ etc.) and how long to run the experiment (_end_time_ms_) after evaporation to BEC is complete. Also included are various job primitives that can be created and edited as programmable objects in their own right. These primitives include _rf_evaporation_, _optical_barriers_, _optical_landscape_, and _lasers_. Much like an _OqtantJob_ itself, these constituent primitives are programmatic objects in their own right and can be instantiated and manipulated outside of a job object. Although not shown explicitly in our simple job data structure above, both _optical_barriers_ and _lasers_ are lists containing _Barrier_ and _Laser_ objects, respectively. These objects will be explored below. You are likely already familiar with the structure of the _rf_evaporation_ data and how defining that data controls the evaporation to BEC in the experiment. The _optical_landscape_ data is a bit more complicated and will be explored in more detail below in a dedicated section.
+The contents of *values* includes directives on the type of imaging to perform (*image_type* etc.) and how long to run the experiment (*end_time_ms*) after evaporation to BEC is complete.  Also included are various job primitives that can be created and edited as programmable objects in their own right.  These primitives include *rf_evaporation*, *optical_barriers*, *optical_landscape*, and *lasers*.  Much like an *OqtantJob* itself, these constituent primitives are programmatic objects in their own right and can be instantiated and manipulated outside of a job object.  Although not shown explicitly in our simple job data structure above, both *optical_barriers* and *lasers* are lists containing *Barrier* and *Laser* objects, respectively.  These objects will be explored below.  You are likely already familiar with the structure of the *rf_evaporation* data and how defining that data controls the evaporation to BEC in the experiment.  The *optical_landscape* data is a bit more complicated and will be explored in more detail below in a dedicated section.       
 
-Not all job types support every one of these data structures. For the basic BEC-type job above, we did not have data entries for barriers, the landscape, or lasers. BEC jobs, for instance, only support the rf*evaporation primitive. After all, the purpose of a BEC job is to keep things simple and just focus on the ability to tune the creation of the condensate. At the next level of complexity, BARRIER jobs support both \_rf_evaporation* and _optical_barriers_ but not "optical_landscape" or "lasers". What data structures are supported by different job types will become clear as those job types are created/used/submitted. As a preview, please refer to the following table.
+Not all job types support every one of these data structures.  For the basic BEC-type job above, we did not have data entries for barriers, the landscape, or lasers.  BEC jobs, for instance, only support the rf_evaporation primitive.  After all, the purpose of a BEC job is to keep things simple and just focus on the ability to tune the creation of the condensate.  At the next level of complexity, BARRIER jobs support both *rf_evaporation* and *optical_barriers* but not "optical_landscape" or "lasers".  What data structures are supported by different job types will become clear as those job types are created/used/submitted.  As a preview, please refer to the following table.
 
 | Job type   | Supports       |                  |                   |        |
-| ---------- | -------------- | ---------------- | ----------------- | ------ |
+|------------|----------------|------------------|-------------------|--------|
 |            | rf_evaporation | optical_barriers | optical_landscape | lasers |
 | BEC        |                |                  |                   |        |
 | BARRIER    | X              | X                |                   |        |
 | TRANSISTOR | X              | X                | X                 | X      |
 | PAINT_1D   | X              | X                | X                 | X      |
 
 Please note that not all these job types are yet available at the time of this writing.
 
 ## The RfEvaporation Object
 
-Every job input has exactly one constituent RfEvaporation object defined by the "rf_evaporation" data shown above. The behavior of this object controls the RF knife evaporation from an ultracold gas to Bose-Einstein condensate (BEC), as well as providing flexibility for applying RF fields during the experiment phase after the initial evaporation is complete. The evaporation stage results in a tradeoff between final atom number and temperature -- evaporating more deeply, signified by RF detuning values closer to 0, produces less atoms but at colder temperature (and correspondingly higher condensate fraction). Applying RF radiation during the experiment phase allows for hot atoms above some temperature, produced for example by rapid manipulation of optical barries or landscape potentials (explored below), to be removed the experiment -- a so-called "RF shield".
+Every job input has exactly one constituent RfEvaporation object defined by the "rf_evaporation" data shown above.  The behavior of this object controls the RF knife evaporation from an ultracold gas to Bose-Einstein condensate (BEC), as well as providing flexibility for applying RF fields during the experiment phase after the initial evaporation is complete.  The evaporation stage results in a tradeoff between final atom number and temperature -- evaporating more deeply, signified by RF detuning values closer to 0, produces less atoms but at colder temperature (and correspondingly higher condensate fraction).  Applying RF radiation during the experiment phase allows for hot atoms above some temperature, produced for example by rapid manipulation of optical barries or landscape potentials (explored below), to be removed the experiment -- a so-called "RF shield". 
 
-It is important to note here that we adopt the convention that time = 0 refers to the _end_ of the evaporation period. As such, the initial evaporation to BEC, as defined by the object under current inspection, will involve negative (relative) times. In our trap, the entire evaporation cycle takes on the order of a second, and times are specified in ms, so we should see negative times as large as a few thousand ms.
+It is important to note here that we adopt the convention that time = 0 refers to the *end* of the evaporation period.  As such, the initial evaporation to BEC, as defined by the object under current inspection, will involve negative (relative) times.  In our trap, the entire evaporation cycle takes on the order of a second, and times are specified in ms, so we should see negative times as large as a few thousand ms.   
 
 ### Construction
 
-Let us begin by constructing a stand-alone RfEvaporation object completely independently of any specific Oqtant job. We can create this object by either calling the constructor directly with the required data fields:
+Let us begin by constructing a stand-alone RfEvaporation object completely independently of any specific Oqtant job.  We can create this object by either calling the constructor directly with the required data fields:
+
 
 ```python
 evap = JobSchema.RfEvaporation(
         times_ms = [-1600, -1200, -800, -400, 0],
         frequencies_mhz = [17.0, 8.0, 4.0, 1.2, 0.045],
         powers_mw = [500.0, 500.0, 475.0, 360.0, 220.0],
         interpolation = "LINEAR"
 )
 ```
 
 or by placing the underlying data in a dictionary and unpacking that dictionary in order to pass it to the constructor:
 
+
 ```python
 evap = JobSchema.RfEvaporation(**{
         "times_ms": [-1600, -1200, -800, -400, 0],
         "frequencies_mhz": [17.0, 8.0, 4.0, 1.2, 0.045],
         "powers_mw": [500.0, 490.0, 475.0, 360.0, 220.0],
         "interpolation": "LINEAR"
 })
 ```
 
-Inherent to the RfEvaporation object are three lists, _times_ms_, _frequencies_mhz_, and _powers_mw_. The key prefix corresponds to the parameter being controlled, while the suffix refers to the associated units. In this case, we specify a list of times in milliseconds (ms), frequencies in MHz (mhz), and powers in milliwatts (mw). Note that all units are lower case, which can cause confusion if taken out of context. All three lists must share the same length as each time element is paired with the corresponding element of the frequencies/powers list(s). The specified behavior of the RF evaporation stage defind by the above data is as follows: At -1.6 seconds the RF power is set at 500 mW and the frequency (detuning) at 17 MHz. By the end of the evaporation period, defined by t=0, the frequency/detuning has decreased to 0.045 MHz = 45 kHz and the power has been reduced to 220 mW. Intermediate values of frequency and power are adopted between those two points in time, with the full time dependence being a result of the given data and chosen interpolation type, which controls how the RF fields behave between the given data points.
+Inherent to the RfEvaporation object are three lists, *times_ms*, *frequencies_mhz*, and *powers_mw*.  The key prefix corresponds to the parameter being controlled, while the suffix refers to the associated units.  In this case, we specify a list of times in milliseconds (ms), frequencies in MHz (mhz), and powers in milliwatts (mw).  Note that all units are lower case, which can cause confusion if taken out of context.  All three lists must share the same length as each time element is paired with the corresponding element of the frequencies/powers list(s).  The specified behavior of the RF evaporation stage defind by the above data is as follows: At -1.6 seconds the RF power is set at 500 mW and the frequency (detuning) at 17 MHz.  By the end of the evaporation period, defined by t=0, the frequency/detuning has decreased to 0.045 MHz = 45 kHz and the power has been reduced to 220 mW.  Intermediate values of frequency and power are adopted between those two points in time, with the full time dependence being a result of the given data and chosen interpolation type, which controls how the RF fields behave between the given data points.      
 
-Frequencies are given as a detuning with respect to the energetic trap bottom, so RF fields at a frequency/detuning of 0 would eliminate all atoms from the trap. Achieving final BEC temperatures on the order of 100 nK usually corresponds to final RF frequencies of a few tens of kHz. Powers refer to the amount of power delivered to an antenna that bathes the ultracold atoms with RF radiation. The actual local RF field experienced by the atoms depends on system losses and the exact geometry of the antenna.
+Frequencies are given as a detuning with respect to the energetic trap bottom, so RF fields at a frequency/detuning of 0 would eliminate all atoms from the trap.  Achieving final BEC temperatures on the order of 100 nK usually corresponds to final RF frequencies of a few tens of kHz.  Powers refer to the amount of power delivered to an antenna that bathes the ultracold atoms with RF radiation.  The actual local RF field experienced by the atoms depends on system losses and the exact geometry of the antenna.      
 
 ### Time-dependent evaporation parameters
 
-We can explore the time-dependence of the RFEvaporation object frequency and power, as defined by the data structure above, using some useful functions included with oqtant. For example, we can query the object for the instantaneous power or frequency at any point in time. Recall that the units of power are mW and the units of frequency are MHz.
+We can explore the time-dependence of the RFEvaporation object frequency and power, as defined by the data structure above, using some useful functions included with oqtant.  For example, we can query the object for the instantaneous power or frequency at any point in time.  Recall that the units of power are mW and the units of frequency are MHz.
+
 
 ```python
 print(evap.get_power(time = -100))
 print(evap.get_frequency(time = -750))
 ```
 
 If we request the power or frequency for a time value outside the range of the underlying data, which would require extrapolation, we get 0.0:
 
+
 ```python
 print(evap.get_power(time = 100))           # request after last defined object time of 0 ms -> 0.0
 print(evap.get_frequency(time = -1800))     # request before first defined object time of -1600 ms -> 0.0
 ```
 
-This behavior is generic to most objects in oqtant -- any temporal or spatial extrapolation requests yield 0.0.
+This behavior is generic to most objects in oqtant -- any temporal or spatial extrapolation requests yield 0.0.  
 
 There are also functions that extract the time-dependent parameters for a list of input times:
 
+
 ```python
 print(evap.get_powers(times = [-1600, -1000, -500, 0]))
 print(evap.get_frequencies(times = [-1600, -1000, -600, 0]))
 ```
 
 There are even useful plotting functions for visualizing these parameters over time.
 
+
 ```python
 evap.plot_power()
 evap.plot_frequency()
 ```
 
 ## Barrier Objects
 
+  
+
 ### Construction
 
-First, let us demonstrate the construction of a Barrier object, which represents a one-dimensional optical potential barrier to the BEC. A barrier is characterized by a shape, a time-dependent position, height, and width, and information on how to interpolate over the underlying data in time. For example, let us construct a Barrier object named _barr_ for which the center scans from 1-11 microns in the first 10 ms of an experiment. Over this same time period, the barrier height will increase from 1 kHz to 11 kHz. The width will remain constant at 1 micron throughout, as will the (fixed) Gaussian shape. In this case, the width parameter corresponds to the Gaussian width of the barrier.
+First, let us demonstrate the construction of a Barrier object, which represents a one-dimensional optical potential barrier to the BEC.  A barrier is characterized by a shape, a time-dependent position, height, and width, and information on how to interpolate over the underlying data in time.  For example, let us construct a Barrier object named *barr* for which the center scans from 1-11 microns in the first 10 ms of an experiment.  Over this same time period, the barrier height will increase from 1 kHz to 11 kHz.  The width will remain constant at 1 micron throughout, as will the (fixed) Gaussian shape.  In this case, the width parameter corresponds to the Gaussian width of the barrier.
+
 
 ```python
 barr = JobSchema.Barrier(
-    times_ms = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10],
+    times_ms = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10], 
     positions_um = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11],
     heights_khz = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11],
     widths_um = [1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1],
     interpolation = 'LINEAR',
     shape = 'GAUSSIAN'
 )
 ```
 
-Alternatively, as above, we can create the same object by generating the underlying data in a dictionary and then unpacking that dictionary (using the \*\* prefix) when we pass it to the Barrier class constructor:
+Alternatively, as above, we can create the same object by generating the underlying data in a dictionary and then unpacking that dictionary (using the ** prefix) when we pass it to the Barrier class constructor:
+
 
 ```python
 barr = JobSchema.Barrier(**{
-    "times_ms": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10],
-    "positions_um": [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11],
-    "heights_khz": [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11],
-    "widths_um": [1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1],
-    "interpolation": "LINEAR",
+    "times_ms": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10], 
+    "positions_um": [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11], 
+    "heights_khz": [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11], 
+    "widths_um": [1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1], 
+    "interpolation": "LINEAR", 
     "shape": "GAUSSIAN"
 })
 ```
 
-The lists of time-dependent quantities (position, height, and width) used to define _barr_ must have the same length as the corresponding list of times. In this case, the ordered pairs consisting of a list of, e.g., [times, positions], will be linearly interpolated in time.
+The lists of time-dependent quantities (position, height, and width) used to define *barr* must have the same length as the corresponding list of times.  In this case, the ordered pairs consisting of a list of, e.g., [times, positions], will be linearly interpolated in time.  
 
 ### Time-dependent barrier parameters
 
-We can explore the time-dependence of the barrier parameters using some in-built functions in pyubert. For example, we can retrieve and/or plot the barriers positions over time:
+We can explore the time-dependence of the barrier parameters using some in-built functions in pyubert.  For example, we can retrieve and/or plot the barriers positions over time:
+
 
 ```python
 print(barr.get_position(time = 2))
 print(barr.get_positions(times = [1,2,3]))
 ```
 
-Similarly, there are native functions for extracting a Barrier objects height and width at specified time(s). In our case, the width evolution is trivial (constant).
+Similarly, there are native functions for extracting a Barrier objects height and width at specified time(s).  In our case, the width evolution is trivial (constant).
+
 
 ```python
 print(barr.get_height(1.5))
 print(barr.get_heights([1.5, 2.5, 3.5]))
 
 print(barr.get_width(1.5))
 print(barr.get_widths([1.5, 2.5, 3.5]))
 ```
 
-As well as methods for extracting the time-dependent parameters of the barrier, we can also use some in-built plotting functions. In the examples below, you can see the underlying data points (that we used to define the Barrier object) as points, with the full dynamics of the barrier parameters over time determined by the interpolation style and indicated by a solid line. In an actual experiment, the barrier positions are updated every 100 microseconds, so the time-dependent barrier parameters will only approximately follow the idealized interpolated line.
+As well as methods for extracting the time-dependent parameters of the barrier, we can also use some in-built plotting functions.  In the examples below, you can see the underlying data points (that we used to define the Barrier object) as points, with the full dynamics of the barrier parameters over time determined by the interpolation style and indicated by a solid line. In an actual experiment, the barrier positions are updated every 100 microseconds, so the time-dependent barrier parameters will only approximately follow the idealized interpolated line.   
+
 
 ```python
 barr.plot_position()
 barr.plot_height()
 barr.plot_width()
 ```
 
-### Plotting the potential energy for a barrier
+### Plotting the potential energy for a barrier  
+
+There are also methods native to oqtant for plotting Barrier object potential energies at different times of the experiment.  Here, we will explicitly specify the positional range of the plot (x-axis domain) in order to better be able to see the barrier displacement. 
 
-There are also methods native to oqtant for plotting Barrier object potential energies at different times of the experiment. Here, we will explicitly specify the positional range of the plot (x-axis domain) in order to better be able to see the barrier displacement.
 
 ```python
 xlim = [-5, 15]
 ylim = [0, 12.5]
 barr.plot_potential(time = 1, x_limits = xlim, y_limits = ylim)
 barr.plot_potential(time = 5, x_limits = xlim, y_limits = ylim)
 barr.plot_potential(time = 9, x_limits = xlim, y_limits = ylim)
 ```
 
 ### Exploring Barrier shape options
 
-Supported Barrier shape options include GAUSSIAN, SQUARE, and LORENTZIAN. In all three cases, the "width_um" parameter list means something slightly different. For the GAUSSIAN case, the functional form of the barrier potential $U(x)$ follows the standard Gaussian formula
-
+Supported Barrier shape options include GAUSSIAN, SQUARE, and LORENTZIAN.  In all three cases, the "width_um" parameter list means something slightly different.  For the GAUSSIAN case, the functional form of the barrier potential $U(x)$ follows the standard Gaussian formula
 $$
 U(x) = H e^{-\frac{(x - x_0)^2}{2 w^2}} \quad \textrm{(GAUSSIAN)}
 $$
-
-where $H=H(t)$, $x_{0} = x_{0}(t)$, and $w = w(t)$ represent the time-dependent barrier height, center position, and width, respectively. In this case, our width parameter corresponds to the traditional definition of the Gaussian width, often denoted as $\sigma$.
+where $H=H(t)$, $x_{0} = x_{0}(t)$, and $w = w(t)$ represent the time-dependent barrier height, center position, and width, respectively.  In this case, our width parameter corresponds to the traditional definition of the Gaussian width, often denoted as $\sigma$.    
 
 For the LORENTZIAN case, the potential follows
-
 $$
 U(x) = \frac{H}{1 + (x - x_0)^{2} / w^{2}} \quad \textrm{(LORENTZIAN)},
 $$
-
 i.e. our width parameter w(t) corresponds to the half-width half-max of the Lorentzian.
 
-For the SQUARE case, the potential is simple a flat-topped potential-energy hill of height H(t) and _full_ width w(t).
+For the SQUARE case, the potential is simple a flat-topped potential-energy hill of height H(t) and *full* width w(t).  
+
 
 ```python
 barr.shape = JobSchema.ShapeType.SQUARE
 barr.plot_potential(time = 5, x_limits = [-25,25])
 
 barr.shape = JobSchema.ShapeType.LORENTZIAN
 barr.plot_potential(time = 5, x_limits = [-25,25])
 ```
 
-Note that the resolution of the projected light optical system is on the order of 2 microns. Thus, _Barrier_ objects with small widths will all appear similar in reality (the experiment) even if they have different _shape_ settings.
+Note that the resolution of the projected light optical system is on the order of 2 microns.  Thus, *Barrier* objects with small widths will all appear similar in reality (the experiment) even if they have different *shape* settings.
 
 ### Exploring Barrier interpolation options
 
-A Barrier object's 'interpolation' style determines how the time-dependent position, height, and width are determined for intermediate times between the provided data points in the 'times*ms' list class member. At this time, the interpolation choice is \_shared* for all three time-dependent barrier parameters. Let us explore the effects of different interpolation choices by altering the time-dependent position of our barrier, to make it a little more interesting, and then plot the position over time for a few different interpolation choices.
+A Barrier object's 'interpolation' style determines how the time-dependent position, height, and width are determined for intermediate times between the provided data points in the 'times_ms' list class member. At this time, the interpolation choice is *shared* for all three time-dependent barrier parameters.  Let us explore the effects of different interpolation choices by altering the time-dependent position of our barrier, to make it a little more interesting, and then plot the position over time for a few different interpolation choices.  
+
 
 ```python
 barr.positions_um = [2, 4, 6, 8, 10, 2, 4, 6, 8, 6, 4]
 
 barr.interpolation = JobSchema.InterpolationType.STEP
 barr.plot_position()
 
 barr.interpolation = JobSchema.InterpolationType.CUBIC
 barr.plot_position()
 ```
 
-As you can see above, 'STEP' style interpolation gives a "jumpy" barrier that changes position at discrete times. Other interpolation options, like 'SMOOTH' (which is functionally equivalent to 'CUBIC'), give rise to a continually varying barrier position (and height/width). The full list of interpolation options is as follows:
+As you can see above, 'STEP' style interpolation gives a "jumpy" barrier that changes position at discrete times.  Other interpolation options, like 'SMOOTH' (which is functionally equivalent to 'CUBIC'), give rise to a continually varying barrier position (and height/width).  The full list of interpolation options is as follows:
+
 
 ```python
 print([e.value for e in JobSchema.InterpolationType])
 ```
 
 ## The Optical Landscape Object
 
-Another Oqtant job primitive is the (singular) 'OpticalLandscape' object. This construct is similar to the optical barriers list in the sense that it instructs the experiment to apply 1D optical potentials, in the form of painted blue-detuned light, to the condensate over the course of the experiment. However, now the user (you!) is free to specify a list of positions and corresponding potential energies at specified times, instead of being limited to the concept of a singular barrier or combination of multiple barriers.
+Another Oqtant job primitive is the (singular) 'OpticalLandscape' object.  This construct is similar to the optical barriers list in the sense that it instructs the experiment to apply 1D optical potentials, in the form of painted blue-detuned light, to the condensate over the course of the experiment.  However, now the user (you!) is free to specify a list of positions and corresponding potential energies at specified times, instead of being limited to the concept of a singular barrier or combination of multiple barriers.    
 
-The OpticalLandscape object consists of a list of individual potential-energy landscapes and an interpolation option on how those landscapes connect together _in time_ (if there exists more than one underlying landscape). Let us begin by constructing a couple Landscape objects, from which we will compose the OpticalLandscape container object.
+The OpticalLandscape object consists of a list of individual potential-energy landscapes and an interpolation option on how those landscapes connect together *in time* (if there exists more than one underlying landscape).  Let us begin by constructing a couple Landscape objects, from which we will compose the OpticalLandscape container object.   
 
 ### Construction
 
-We can directly compose an _OpticalLandscape_ object, as above with the _Barrier_ object(s), or we can compose the constituent Landscape objects and then compose the full _OpticalLandscape_ object accordingly:
+We can directly compose an *OpticalLandscape* object, as above with the *Barrier* object(s), or we can compose the constituent Landscape objects and then compose the full *OpticalLandscape* object accordingly:
+
 
 ```python
 landscape_1 = JobSchema.Landscape(
     time_ms = 1.0,
     positions_um = [-50, -25, 0, 25, 50],
     potentials_khz = [100, 50, 0, 50, 100],
     spatial_interpolation = 'LINEAR'
@@ -266,53 +281,57 @@
     interpolation = 'LINEAR',
     landscapes = [landscape_1, landscape_2]
 )
 ```
 
 ### Inspecting consituent 'Landscape' objects
 
+
 ```python
 print(landscape_1.get_potential_at_position(10))
 print(landscape_2.get_potential_at_positions([-75, -50, -25, 0, 25, 50, 75]))
 ```
 
+
 ```python
 landscape_1.plot_potential()
 landscape_2.plot_potential(y_limits = [-1, 101])
 ```
 
-In the plots above, you can see the potential energy profile specified by our two Landscape objects. The underlying data shows up as points, with the overall profile determined by the values of these points and the chosen value for _spatial_interpolation_. The same values are available here as were for (temporal) interpolation options for Barrier objects.
+In the plots above, you can see the potential energy profile specified by our two Landscape objects.  The underlying data shows up as points, with the overall profile determined by the values of these points and the chosen value for *spatial_interpolation*.  The same values are available here as were for (temporal) interpolation options for Barrier objects.  
 
 ### Understanding the time dependence of the composed OpticalLandscape object
 
-The time-dependence of the overall optical potential-energy landscape, as derived from the individual _landscapes[]_ list, is somewhat complicated. As for _Barrier_ and other similar objects, any temporal extrapolation (behavior for data outside the defined time period, i.e. before the first or after the last elements of the _landscapes[]_ list) results in zero potential (in the absence of any other sources, such as Barriers). Therefore, the only way to get a non-zero painted potential optical landscape is to define at least two landscapes that can be interpolated between. To hold a static (unchanging) potential during a period of the experiment, one would define two elements of the _landscapes[]_ list with identical potential energy profiles but differing times, with the potential being applied between those two times. If one desires the potential to change dynamically, then adjacent elements of the _landscapes[]_ list (elements with the nearest _time_ms_ values) should define the snapshots of the desired potential at the temporal endpoints. In between these endpoints the potential landscape is interpolated point-by-point (in position) according to the user-specified value for _interpolation_. This process continues so that, at the specified times of the elements of _landscapes[]_, the overall optical potential energy landscape instantaneously equal to those individual landscapes.
+The time-dependence of the overall optical potential-energy landscape, as derived from the individual *landscapes[]* list, is somewhat complicated.  As for *Barrier* and other similar objects, any temporal extrapolation (behavior for data outside the defined time period, i.e. before the first or after the last elements of the *landscapes[]* list) results in zero potential  (in the absence of any other sources, such as Barriers).  Therefore, the only way to get a non-zero painted potential optical landscape is to define at least two landscapes that can be interpolated between.  To hold a static (unchanging) potential during a period of the experiment, one would define two elements of the *landscapes[]* list with identical potential energy profiles but differing times, with the potential being applied between those two times.  If one desires the potential to change dynamically, then adjacent elements of the *landscapes[]* list (elements with the nearest *time_ms* values) should define the snapshots of the desired potential at the temporal endpoints.  In between these endpoints the potential landscape is interpolated point-by-point (in position) according to the user-specified value for *interpolation*.  This process continues so that, at the specified times of the elements of *landscapes[]*, the overall optical potential energy landscape instantaneously equal to those individual landscapes.  
+
+In our example above, with linear interpolation, this means that there will be a period of no optical potential between 0 and 1 ms, our *landscape_1* potential will start being applied at 1 ms, this potential will smoothly (linearly, in this case) morph into the *landscape_2* potential between 1 and 10 ms, and then this potential landscape will be held until the end of the experiment.  Let us use oqtant's visualization functions to inspect this behavior to make it clear.       
 
-In our example above, with linear interpolation, this means that there will be a period of no optical potential between 0 and 1 ms, our _landscape_1_ potential will start being applied at 1 ms, this potential will smoothly (linearly, in this case) morph into the _landscape_2_ potential between 1 and 10 ms, and then this potential landscape will be held until the end of the experiment. Let us use oqtant's visualization functions to inspect this behavior to make it clear.
 
 ```python
 optical_landscape.plot_potential(time = 0.9)
 optical_landscape.plot_potential(time = 1)
 optical_landscape.plot_potential(time = 3)
 optical_landscape.plot_potential(time = 5)
 optical_landscape.plot_potential(time = 7)
 optical_landscape.plot_potential(time = 9)
 optical_landscape.plot_potential(time = 11)
 ```
 
-As descibed above, we can see zero overall potential both before the first and after the last times of the individual Landscape objects. At 1 ms, the first Landscape is assumed. The potential landscape then morphs into our second Landscape object at t = 10 ms.
+As descibed above, we can see zero overall potential both before the first and after the last times of the individual Landscape objects.  At 1 ms, the first Landscape is assumed.  The potential landscape then morphs into our second Landscape object at t = 10 ms.  
 
-## Laser Objects
+## Laser Objects 
 
-The last data structure to explore here is the _lasers[]_ list in the job data. This is a list of _Laser_ objects. Currently, the user is limited to a single element/laser.
+The last data structure to explore here is the *lasers[]* list in the job data.  This is a list of *Laser* objects.  Currently, the user is limited to a single element/laser.  
 
 ### Construction
 
-Let us begin by constructing a _Laser_ object, which gives the user control over near-resonant laser light applied to the atoms over the course of the experiment. This differs from the painted potential laser, which is far off-resonance in order to apply potential energy landscapes and barriers to the trapped condensate. Resonant or near-resonant light, on the other hand, results in scattering of photons from the light field by the atoms. This is useful, for example, in TRANSISTOR jobs where we want to remove atoms from some spatial region of the trap using a so-called TERMINATOR laser.
+Let us begin by constructing a *Laser* object, which gives the user control over near-resonant laser light applied to the atoms over the course of the experiment.  This differs from the painted potential laser, which is far off-resonance in order to apply potential energy landscapes and barriers to the trapped condensate.  Resonant or near-resonant light, on the other hand, results in scattering of photons from the light field by the atoms.  This is useful, for example, in TRANSISTOR jobs where we want to remove atoms from some spatial region of the trap using a so-called TERMINATOR laser.  
+
+A *Laser* object gives the user control of the time-dependence of laser light applied to the atomic ensemble, including the time-dependent intensity and detuning given by a series of *pulse* objects specified by a *pulses[]* list.  We can construct such an object as follows:
 
-A _Laser_ object gives the user control of the time-dependence of laser light applied to the atomic ensemble, including the time-dependent intensity and detuning given by a series of _pulse_ objects specified by a _pulses[]_ list. We can construct such an object as follows:
 
 ```python
 pulse_1 = JobSchema.Pulse(
     times_ms = [1, 1.5, 2, 3],
     intensities_mw_per_cm2 = [0, 10, 2, 0],
     detuning_mhz = 5,
     interpolation = 'SMOOTH'
@@ -334,10 +353,11 @@
 
 laser = JobSchema.Laser(
     type = 'TERMINATOR',
     pulses = [pulse_1, pulse_2, pulse_3]
 )
 ```
 
+
 ```python
 laser.plot_intensity()
 ```
```

### Comparing `oqtant-0.14.4/documentation/tutorials/tutorial_5_optimization.ipynb` & `oqtant-0.15.0/documentation/walkthroughs/walkthrough_5_optimization.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9837390734265734%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, '# Oqtant Walkthrough 4: BEC Experimentation #\\n'), (4, "*

 * *            "'For more information about Oqtant refer to our documentation: "*

 * *            "https://gitlab.com/infleqtion/albert/oqtant/-/blob/main/README.md\\n'), (5, '\\n'), "*

 * *            "(6, '*Batch job functionality is available for users with a subscription tier of "*

 * *            "EXPLORER or INNOVATOR.*')], delete: [4, 0]}, delete: ['attachments']}, 1: {'source': "*

 * *            "{insert: [(4, 'Run the be […]*

```diff
@@ -1,31 +1,31 @@
 {
     "cells": [
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Oqtant Tutorial 4: BEC Experimentation #\n",
+                "# Oqtant Walkthrough 4: BEC Experimentation #\n",
                 "\n",
                 "### This walkthrough reviews authorizing an Oqtant session and an example of optimization for BEC. ###\n",
                 "\n",
-                "For more information about Oqtant refer to our documentation: https://albert-dev.coldquanta.com/oqtant/manual.md"
+                "For more information about Oqtant refer to our documentation: https://gitlab.com/infleqtion/albert/oqtant/-/blob/main/README.md\n",
+                "\n",
+                "*Batch job functionality is available for users with a subscription tier of EXPLORER or INNOVATOR.*"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Sign into Oqtant\n",
                 "\n",
                 "## Before you can view and submit jobs you must first sign into your Oqtant account\n",
                 "\n",
-                "Run the below cell to be re-directed to our login page and provide you account credentials. Once authenticated you can safely close out that tab and return to this notebook."
+                "Run the below cell to be re-directed to our login page and provide your account credentials. Once authenticated you can safely close out that tab and return to this notebook."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -52,15 +52,14 @@
                 ")\n",
                 "import csv\n",
                 "\n",
                 "token = get_user_token()"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Creating a Oqtant Client Instance ##\n",
                 "\n",
                 "### After successful login, create an authorized session with the Oqtant Client ###\n",
                 "- the oqtant_client interacts with the albert server to perform remote lab functions. \n",
@@ -73,15 +72,14 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "oqtant_client = get_oqtant_client(token)"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Define a cost function for optimization ## \n",
                 "\n",
                 "A cost function is a metric calculated for the system of interest which is lowered over time via some optimization script \n",
                 "\n",
@@ -130,40 +128,39 @@
                 "}\n",
                 "\n",
                 "def cost_func_9D(RF_freqs_RF_powers):\n",
                 "    RF_freqs = RF_freqs_RF_powers[:5]\n",
                 "    RF_powers = RF_freqs_RF_powers[5:] # this needs to have 5 powers in it now\n",
                 "    default_bec_job[\"inputs\"][0][\"values\"][\"rf_evaporation\"][\"frequencies_mhz\"] = RF_freqs\n",
                 "    default_bec_job[\"inputs\"][0][\"values\"][\"rf_evaporation\"][\"powers_mw\"] = RF_powers\n",
-                "    albert_job = oqtant_client.generate_albert_job(job=default_bec_job)\n",
+                "    albert_job = oqtant_client.generate_oqtant_job(job=default_bec_job)\n",
                 "    [job_id] = oqtant_client.run_jobs(job_list=[albert_job], track_status=True)\n",
                 "    job_output = oqtant_client.active_jobs[job_id].inputs[0].output.values\n",
                 "    Nth = job_output.thermal_atom_number\n",
                 "    T = job_output.temperature_uk\n",
                 "    Nc = job_output.condensed_atom_number+1\n",
                 "    C = (Nth*T)/Nc\n",
                 "    costs_9D.append(C)\n",
                 "    return C\n",
                 "\n",
                 "def cost_func_5D(RF_freqs, RF_powers = [500, 475, 450, 400, 400]): # added 5th power to default\n",
                 "    default_bec_job[\"inputs\"][0][\"values\"][\"rf_evaporation\"][\"frequencies_mhz\"] = RF_freqs\n",
                 "    default_bec_job[\"inputs\"][0][\"values\"][\"rf_evaporation\"][\"powers_mw\"] = RF_powers\n",
-                "    albert_job = oqtant_client.generate_albert_job(job=default_bec_job)\n",
+                "    albert_job = oqtant_client.generate_oqtant_job(job=default_bec_job)\n",
                 "    [job_id] = oqtant_client.run_jobs(job_list=[albert_job], track_status=True)\n",
                 "    job_output = oqtant_client.active_jobs[job_id].inputs[0].output.values\n",
                 "    Nth = job_output.thermal_atom_number\n",
                 "    T = job_output.temperature_uk\n",
                 "    Nc = job_output.condensed_atom_number\n",
                 "    C = (Nth*T)/Nc\n",
                 "    costs_5D.append(C)\n",
                 "    return C"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Set bounds for optimization ## \n",
                 "\n",
                 "Bounds will prevent invalid jobs parameters from being submitted to the job runner."
             ]
@@ -175,15 +172,14 @@
             "outputs": [],
             "source": [
                 "bnds_5d = ((0,50),(0,50),(0,50),(0,50),(0,50))\n",
                 "bnds_9d = ((0,50),(0,50),(0,50),(0,50),(0,50),(0,500),(0,500),(0,500),(0,500))"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Choose an optimization algorithm ##\n",
                 "\n",
                 "Here, I chose a truncated Newton method (TNC). TNC uses a truncated Newton algorithm to minimize a function with variables subject to bounds. Within scipy.optimize.minimize there are several options for optimizers which allow for bounded variables:  \n",
                 "\n",
@@ -212,37 +208,34 @@
                 "#print(res_5d)\n",
                 "\n",
                 "#print(\"optimization results freq and power tuning:\")\n",
                 "#print(res_9d)"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Bayesian Optimization with a Gaussian Process model ##\n"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Extract and shape the training data: ##\n",
                 "\n",
                 "X_train_array-like of shape (n_samples, n_features) or list of object\n",
                 "Feature vectors or other representations of training data (also required for prediction).\n",
                 "\n",
                 "y_train_array-like of shape (n_samples,) or (n_samples, n_targets)\n",
                 "Target values in training data (also required for prediction)"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Define a new target cost function ##"
             ]
         },
         {
@@ -312,15 +305,14 @@
                 "    with catch_warnings():\n",
                 "        # ignore generated warnings\n",
                 "        simplefilter(\"ignore\")\n",
                 "        return model.predict(X, return_std=True)"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Define an acquisition function ## \n",
                 "\n",
                 "This is a score assigned to each candidate sample on the domain. \n",
                 "\n",
@@ -355,15 +347,14 @@
                 "    #mu = mu[:, 0]\n",
                 "    # calculate the probability of improvement\n",
                 "    probs = norm.cdf((mu - best) / (std+1E-9))\n",
                 "    return probs"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Define a domain ##\n",
                 "\n",
                 "This is the domain of the samples. This one point where we inject prior knowledge of the system from previous experience"
             ]
@@ -381,15 +372,14 @@
                 "    scale = domain[0]-domain[1]\n",
                 "    random_number = np.random.uniform()+(1E-9)\n",
                 "    sample = scale*random_number+domain[1]\n",
                 "    return sample"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Define an optimizer on the acquisition function ##\n",
                 "\n",
                 "Here I have chosen a random search over the domain, but other search algorithms can be used. "
             ]
@@ -408,15 +398,14 @@
                 "    scores = acquisition(X, Xsamples, model)\n",
                 "    # locate the index of the largest scores\n",
                 "    ix = np.argmax(scores)\n",
                 "    return Xsamples[ix]"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Perform the optimization ##"
             ]
         },
         {
```

### Comparing `oqtant-0.14.4/documentation/tutorials/tutorial_5_optimization.md` & `oqtant-0.15.0/documentation/walkthroughs/walkthrough_5_optimization.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-# Oqtant Tutorial 4: BEC Experimentation
+# Oqtant Walkthrough 4: BEC Experimentation
 
-### This walkthrough reviews authorizing an Oqtant session and an example of optimization for BEC.
+### This walkthrough reviews authorizing an Oqtant session and an example of optimization for BEC. ###
 
-For more information about Oqtant refer to our documentation: https://albert-dev.coldquanta.com/oqtant/manual.md
+For more information about Oqtant refer to our documentation: https://gitlab.com/infleqtion/albert/oqtant/-/blob/main/README.md
+
+*Batch job functionality is available for users with a subscription tier of EXPLORER or INNOVATOR.*
 
 # Sign into Oqtant
 
 ## Before you can view and submit jobs you must first sign into your Oqtant account
 
-Run the below cell to be re-directed to our login page and provide you account credentials. Once authenticated you can safely close out that tab and return to this notebook.
+Run the below cell to be re-directed to our login page and provide your account credentials. Once authenticated you can safely close out that tab and return to this notebook.
+
 
 ```python
 from sklearn.gaussian_process import GaussianProcessRegressor as GPR
 from matplotlib import pyplot as plt
 from scipy.optimize import minimize
 from warnings import catch_warnings
 from warnings import simplefilter
@@ -32,42 +35,41 @@
     round_sig
 )
 import csv
 
 token = get_user_token()
 ```
 
-## Creating a Oqtant Client Instance
-
-### After successful login, create an authorized session with the Oqtant Client
+## Creating a Oqtant Client Instance ##
 
-- the oqtant_client interacts with the albert server to perform remote lab functions.
+### After successful login, create an authorized session with the Oqtant Client ###
+- the oqtant_client interacts with the albert server to perform remote lab functions. 
 - the oqtant_client object also contains all the jobs which have been submitted, run, or loaded (from database or file) during this python session
 
+
 ```python
 oqtant_client = get_oqtant_client(token)
 ```
 
-## Define a cost function for optimization
-
-A cost function is a metric calculated for the system of interest which is lowered over time via some optimization script
+## Define a cost function for optimization ## 
 
-Larger value = Good: Condensed and total atom number, condensate fraction
-Smaller value = Good: Thermal atom number, temperature
+A cost function is a metric calculated for the system of interest which is lowered over time via some optimization script 
 
-Ad hoc Cost function: **C = (Nth\*T)/Nc**
+Larger value = Good:  Condensed and total atom number, condensate fraction 
+Smaller value = Good: Thermal atom number, temperature 
 
-### cost_func_5D
+Ad hoc Cost function: **C = (Nth*T)/Nc**
 
+### cost_func_5D ### 
 This cost function is for a 5-dimensional optimization space, where the 5 dimensions are the RF corner frequencies.
 
-### cost_func_9D
-
+### cost_func_9D ### 
 This cost function is for a 9-dimensional optimization space, where the 9 dimensions are the RF corner frequencies and the RF powers.
 
+
 ```python
 costs_9D = []
 costs_5D = []
 
 default_bec_job = {
     "name": "Example Ultracold Matter Generator Job",
     "job_type": "BEC",
@@ -92,204 +94,214 @@
 }
 
 def cost_func_9D(RF_freqs_RF_powers):
     RF_freqs = RF_freqs_RF_powers[:5]
     RF_powers = RF_freqs_RF_powers[5:] # this needs to have 5 powers in it now
     default_bec_job["inputs"][0]["values"]["rf_evaporation"]["frequencies_mhz"] = RF_freqs
     default_bec_job["inputs"][0]["values"]["rf_evaporation"]["powers_mw"] = RF_powers
-    albert_job = oqtant_client.generate_albert_job(job=default_bec_job)
+    albert_job = oqtant_client.generate_oqtant_job(job=default_bec_job)
     [job_id] = oqtant_client.run_jobs(job_list=[albert_job], track_status=True)
     job_output = oqtant_client.active_jobs[job_id].inputs[0].output.values
     Nth = job_output.thermal_atom_number
     T = job_output.temperature_uk
     Nc = job_output.condensed_atom_number+1
     C = (Nth*T)/Nc
     costs_9D.append(C)
     return C
 
 def cost_func_5D(RF_freqs, RF_powers = [500, 475, 450, 400, 400]): # added 5th power to default
     default_bec_job["inputs"][0]["values"]["rf_evaporation"]["frequencies_mhz"] = RF_freqs
     default_bec_job["inputs"][0]["values"]["rf_evaporation"]["powers_mw"] = RF_powers
-    albert_job = oqtant_client.generate_albert_job(job=default_bec_job)
+    albert_job = oqtant_client.generate_oqtant_job(job=default_bec_job)
     [job_id] = oqtant_client.run_jobs(job_list=[albert_job], track_status=True)
     job_output = oqtant_client.active_jobs[job_id].inputs[0].output.values
     Nth = job_output.thermal_atom_number
     T = job_output.temperature_uk
     Nc = job_output.condensed_atom_number
     C = (Nth*T)/Nc
     costs_5D.append(C)
     return C
 ```
 
-## Set bounds for optimization
+## Set bounds for optimization ## 
 
 Bounds will prevent invalid jobs parameters from being submitted to the job runner.
 
+
 ```python
 bnds_5d = ((0,50),(0,50),(0,50),(0,50),(0,50))
 bnds_9d = ((0,50),(0,50),(0,50),(0,50),(0,50),(0,500),(0,500),(0,500),(0,500))
 ```
 
-## Choose an optimization algorithm
-
-Here, I chose a truncated Newton method (TNC). TNC uses a truncated Newton algorithm to minimize a function with variables subject to bounds. Within scipy.optimize.minimize there are several options for optimizers which allow for bounded variables:
+## Choose an optimization algorithm ##
 
-- L-BFGS-B
-- TNC
-- COBYLA
-- SLSQP
+Here, I chose a truncated Newton method (TNC). TNC uses a truncated Newton algorithm to minimize a function with variables subject to bounds. Within scipy.optimize.minimize there are several options for optimizers which allow for bounded variables:  
 
-## Provide initial conditions and max iterations
+ - L-BFGS-B 
+ - TNC
+ - COBYLA
+ - SLSQP
+ 
+ 
+ ## Provide initial conditions and max iterations ##
+ 
+ I chose the web app default parameters for a mixed cloud for the x0 initial conditions. Specify iterations with **options={'maxiter':10}**. Note that each iteration may involve several evaluations of the cost function (which means several jobs), so setting **'maxiter':30** will not run within a single 24 hour period. 
 
-I chose the web app default parameters for a mixed cloud for the x0 initial conditions. Specify iterations with **options={'maxiter':10}**. Note that each iteration may involve several evaluations of the cost function (which means several jobs), so setting **'maxiter':30** will not run within a single 24 hour period.
 
 ```python
 #res_5d = minimize(cost_func_5D, method="TNC", bounds=bnds_5d, x0 = np.array([17,8,4,1.2,0.05]), options={'maxiter':10})
-#res_9d = minimize(cost_func_10D, method="TNC",
+#res_9d = minimize(cost_func_10D, method="TNC", 
 #                   x0 = np.array([17,8,4,1.2,0.07,500,475,450,400]), bounds = bnds_9d,options={'maxiter':10})
 
 #print("optimization results freq tuning only:")
 #print(res_5d)
 
 #print("optimization results freq and power tuning:")
 #print(res_9d)
 ```
 
-## Bayesian Optimization with a Gaussian Process model
+## Bayesian Optimization with a Gaussian Process model ##
 
-## Extract and shape the training data:
+
+## Extract and shape the training data: ##
 
 X_train_array-like of shape (n_samples, n_features) or list of object
 Feature vectors or other representations of training data (also required for prediction).
 
 y_train_array-like of shape (n_samples,) or (n_samples, n_targets)
 Target values in training data (also required for prediction)
 
-## Define a new target cost function
+## Define a new target cost function ##
+
 
 ```python
 def cost(Nc, Nth, T):
     C = (Nth*T)/Nc
     return C
 ```
 
+
 ```python
 X_global_train = []
 y_global_train = []
 with open('output.csv', newline='') as csvfile:
     r = csv.reader(csvfile, delimiter=' ', quotechar='|')
     for row in r:
         if len(row)==26:
-
+            
             rf_a_mhz = float(row[4][:-1])
             rf_b_mhz = float(row[6][:-1])
             rf_c_mhz = float(row[8][:-1])
             rf_d_mhz = float(row[10][:-1])
             rf_e_mhz = float(row[12][:-1])
             pow_a_mw = float(row[14][:-1])
             pow_b_mw = float(row[16][:-1])
             pow_c_mw = float(row[18][:-1])
             pow_d_mw = float(row[20][:-27])
-
+            
             condensed_atom_number = round(float(row[23][:-1]))
             thermal_atom_number = round(float(row[21][:-1]))
             temperature_uk = float(row[25][:-2])
             if temperature_uk > 0 and condensed_atom_number > 100:
                 X_global_train.append([rf_a_mhz,
                                        rf_b_mhz,
                                        rf_c_mhz,
                                        rf_d_mhz,
                                        rf_e_mhz,
-                                      pow_a_mw,
-                                      pow_b_mw,
-                                      pow_c_mw,
+                                      pow_a_mw, 
+                                      pow_b_mw, 
+                                      pow_c_mw, 
                                       pow_d_mw])
                 y_global_train.append(cost(condensed_atom_number, thermal_atom_number, temperature_uk))
 
 #X_global_train = np.asarray(X_global_train)
 #y_global_train = np.asarray(y_global_train)
 
-
+                
 ```
 
+
 ```python
 # surrogate or approximation for the objective function
 def surrogate(model, X):
     # catch any warning generated when making a prediction
     with catch_warnings():
         # ignore generated warnings
         simplefilter("ignore")
         return model.predict(X, return_std=True)
 ```
 
-## Define an acquisition function
+## Define an acquisition function ## 
 
-This is a score assigned to each candidate sample on the domain.
+This is a score assigned to each candidate sample on the domain. 
 
 The surrogate function can be used as an acquisition (minimizing the surrogate is the goal after all)
 
 OR
 
 An acquisition function can be used. 3 common options:
-
 - Probability of Improvement (PI).
 - Expected Improvement (EI).
 - Lower Confidence Bound (LCB).
 
-Here I chose probability of improvement
+Here I chose probability of improvement 
 
 **PI = cdf((mu – best_mu) / stdev)**
 
 Where PI is the probability of improvement, cdf() is the normal cumulative distribution function, mu is the mean of the surrogate function for a given sample x, stdev is the standard deviation of the surrogate function for a given sample x, and best_mu is the mean of the surrogate function for the best sample found so far.
 
+
 ```python
 def acquisition(X, Xsamples, model):
     # calculate the best surrogate score found so far
     yhat, _ = surrogate(model, X)
     best = max(yhat)
     # calculate mean and stdev via surrogate function
     mu, std = surrogate(model, Xsamples)
     #mu = mu[:, 0]
     # calculate the probability of improvement
     probs = norm.cdf((mu - best) / (std+1E-9))
     return probs
 ```
 
-## Define a domain
+## Define a domain ##
 
 This is the domain of the samples. This one point where we inject prior knowledge of the system from previous experience
 
+
 ```python
 domain = [(20.,15.),(12.,5.),(5.,2.),(1.9,0.2),(0.2,0.01),
           (500.,470.),(470.,460.),(459.,420.),(420.,350.)]
 
 def rand_domain_sample(domain):
     scale = domain[0]-domain[1]
     random_number = np.random.uniform()+(1E-9)
     sample = scale*random_number+domain[1]
     return sample
 ```
 
-## Define an optimizer on the acquisition function
+## Define an optimizer on the acquisition function ##
+
+Here I have chosen a random search over the domain, but other search algorithms can be used. 
 
-Here I have chosen a random search over the domain, but other search algorithms can be used.
 
 ```python
 def optimize_acquisition(X, y, model, sample_population):
     # random search, generate random samples
     Xsamples = np.asarray([[rand_domain_sample(domain[i]) for i in range(len(X[0]))] for j in range(sample_population)])
     Xsamples = Xsamples.reshape(len(Xsamples), len(X[0]))
     # calculate the acquisition function for each sample
     scores = acquisition(X, Xsamples, model)
     # locate the index of the largest scores
     ix = np.argmax(scores)
     return Xsamples[ix]
 ```
 
-## Perform the optimization
+## Perform the optimization ##
+
 
 ```python
 #X = sample_domain
 #y = np.asarray([cost_func_9D(x) for x in X])
 #Oqtant_model = GPR()
 #Oqtant_model.fit(X, y)
 
@@ -313,14 +325,15 @@
     # add the data to the dataset
     X = np.vstack((X, [x]))
     y.append(actual)
     # update the model
     Oqtant_model.fit(X, y)
 ```
 
+
 ```python
 # plot all samples and the final surrogate function
 plt.plot(cost[5:])
 #plt.yscale("log")
 plt.xlabel("function evaluations")
 plt.ylabel("Cost")
 plt.title("20 evaluations, 500 surrogate samples, 335pm 5_5_21")
```

### Comparing `oqtant-0.14.4/oqtant/oqtant_client.py` & `oqtant-0.15.0/oqtant/oqtant_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     This class contains tools for:
         - Accessing all of the functionality of the Oqtant Web App (https://albert-dev.coldquanta.com)
             - BARRIER (Barrier Manipulator) jobs
             - BEC (Ultracold Matter) jobs
         - Building parameterized (i.e. optimization) experiments using OqtantJobs
         - Submitting and retrieving OqtantJob results
     How Oqtant works:
-        1.) Construct a single or list of OqtantJobs using 'generate_albert_job()'
+        1.) Construct a single or list of OqtantJobs using 'generate_oqtant_job()'
         2.) Run the single or list of OqtantJobs on the Oqtant hardware using 'run_jobs()'
             - There is a limit of 30 OqtantJobs per use of 'run_jobs()'
         3.) As OqtantJobs are running, the results are automatically stored in 'active_jobs'
             - The OqtantJobs stored in 'active_jobs' are available until the python session ends
         4.) If you choose to not track the status of OqtantJobs with 'run_jobs()' you can see the status
             of your session's active OqtantJobs with 'see_active_jobs()'
         5.) To operate on jobs submitted in a previous session you can load them into your 'active_jobs'
@@ -127,29 +127,29 @@
             raise api_exceptions.ValidationError(f"Failed to get job {job_id}: {err}")
         if not include_notes:
             job.inputs[0].notes = ""
         job = job.dict()
         job.pop("input_count")
         return job
 
-    def generate_albert_job(self, *, job: dict) -> OqtantJob:
+    def generate_oqtant_job(self, *, job: dict) -> OqtantJob:
         """Generates an instance of OqtantJob from the provided dictionary that contains the
            job details and input. Will validate the values and raise an informative error if
            any violations are found.
         Args:
            job (dict): dictionary containing job details and input
         Returns:
            OqtantJob: an OqtantJob instance containing the details and input from the provided
               dictionary
         """
         try:
-            albert_job = OqtantJob(**job)
+            oqtant_job = OqtantJob(**job)
         except ValidationError as err:
             raise api_exceptions.ValidationError(f"Failed to generate OqtantJob: {err}")
-        return albert_job
+        return oqtant_job
 
     def submit_job(self, *, job: OqtantJob) -> dict:
         """Submits a single OqtantJob to the Oqtant REST API. Upon successful submission this
            function will return a dictionary containing the external_id of the job and it's
            position in the queue.
         Args:
            job (OqtantJob): the OqtantJob instance to submit for processing
```

### Comparing `oqtant-0.14.4/oqtant/schemas/job.py` & `oqtant-0.15.0/oqtant/schemas/job.py`

 * *Files identical despite different names*

### Comparing `oqtant-0.14.4/oqtant/settings.py` & `oqtant-0.15.0/oqtant/settings.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,10 +14,10 @@
 # dev
 class Settings(BaseSettings):
     auth0_base_url: str = "https://coldquanta-dev.us.auth0.com"
     auth0_client_id: str = "ZzQdn5ZZq1dmpP5N55KINr33u47RBRiu"
     auth0_scope: str = "offline_access bec_dev_service:client"
     auth0_audience: str = "https://albert-dev.coldquanta.com/oqtant"
     signin_local_callback_url: str = "http://localhost:8080"
-    base_url: str = "https://albert-dev.coldquanta.com/api/v1/bert/jobs"
+    base_url: str = "https://albert-dev.coldquanta.com/api/jobs"
     max_ind_var: int = 2
     max_job_batch_size: int = 30
```

### Comparing `oqtant-0.14.4/oqtant/util/auth.py` & `oqtant-0.15.0/oqtant/util/auth.py`

 * *Files identical despite different names*

### Comparing `oqtant-0.14.4/oqtant/util/exceptions.py` & `oqtant-0.15.0/oqtant/util/exceptions.py`

 * *Files identical despite different names*

### Comparing `oqtant-0.14.4/pyproject.toml` & `oqtant-0.15.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oqtant"
-version = "0.14.4"
+version = "0.15.0"
 description = "Oqtant Desktop Suite"
 authors = [
   "Larry Buza <lawrence.buza@coldquanta.com>",
   "Hannah North <hannah.north@coldquanta.com>",
   "Mike McGrath <michael.mcgrath@coldquanta.com>",
 ]
 license = "Apache-2.0"
@@ -34,15 +34,15 @@
 urllib3 = "^1.26.12"
 notebook = "^6.4.12"
 lmfit = "^1.0.3"
 fastapi = "^0.92.0"
 uvicorn = { extras = ["standard"], version = "^0.20.0" }
 scikit-learn = "^1.2.0"
 python-dotenv = "^0.21.1"
-bert-schemas = "^1.18.0"
+bert-schemas = "^1.18.2"
 pyjwt = { extras = ["crypto"], version = "^2.6.0" }
 semver = "^3.0.0"
 ipykernel = "^6.23.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.3"
 pytest-xdist = "^3.2.0"
```

### Comparing `oqtant-0.14.4/PKG-INFO` & `oqtant-0.15.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: oqtant
-Version: 0.14.4
+Version: 0.15.0
 Summary: Oqtant Desktop Suite
 License: Apache-2.0
 Author: Larry Buza
 Author-email: lawrence.buza@coldquanta.com
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
-Requires-Dist: bert-schemas (>=1.18.0,<2.0.0)
+Requires-Dist: bert-schemas (>=1.18.2,<2.0.0)
 Requires-Dist: fastapi (>=0.92.0,<0.93.0)
 Requires-Dist: ipykernel (>=6.23.1,<7.0.0)
 Requires-Dist: lmfit (>=1.0.3,<2.0.0)
 Requires-Dist: matplotlib (>=3.6.2,<3.7.0)
 Requires-Dist: notebook (>=6.4.12,<7.0.0)
 Requires-Dist: numpy (>=1.23.2,<2.0.0)
 Requires-Dist: pydantic (>=1.10.1,<2.0.0)
@@ -78,13 +78,13 @@
 
 - To analyze job objects and use Oqtant's job analysis library, reference the OqtantJob class documentation.
 
 Need help? Found a bug? Contact <albert@infleqtion.com> for support. Thank you!
 
 ## 📓 Documentation
 
-- [Getting started](https://gitlab.com/infleqtion/albert/oqtant/-/blob/main/documentation/INSTALL.md) (installation, setting up the environment, How to run the tutorial notebooks)
-- [Tutorials](https://gitlab.com/infleqtion/albert/oqtant/-/blob/main/documentation/tutorials/tutorials.md) (demos for creating and submitting jobs)
+- [Getting started](https://gitlab.com/infleqtion/albert/oqtant/-/blob/main/documentation/INSTALL.md) (installation, setting up the environment, how to run the walkthrough notebooks)
+- [Walkthroughs](https://gitlab.com/infleqtion/albert/oqtant/-/blob/main/documentation/walkthroughs/walkthroughs.md) (demos for creating and submitting jobs)
 - [Oqtant API docs](https://gitlab.com/infleqtion/albert/oqtant/-/blob/main/documentation/oqtant_api_docs.md)
 - [Oqtant API docs](https://gitlab.com/infleqtion/albert/oqtant/-/blob/main/documentation/albert_api_docs.md)
 - [Job Analysis docs](https://gitlab.com/infleqtion/albert/oqtant/-/blob/main/documentation/job_analysis_docs.md)
```

