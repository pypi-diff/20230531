# Comparing `tmp/kern-smooth-1.1.1.tar.gz` & `tmp/kern-smooth-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kern-smooth-1.1.1.tar", last modified: Fri Nov 13 20:58:39 2020, max compression
+gzip compressed data, was "kern-smooth-1.1.2.tar", last modified: Wed May 31 17:28:01 2023, max compression
```

## Comparing `kern-smooth-1.1.1.tar` & `kern-smooth-1.1.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 alexanderbutyaev   (501) staff       (20)        0 2020-11-13 20:58:39.000000 kern-smooth-1.1.1/
--rw-r--r--   0 alexanderbutyaev   (501) staff       (20)     3438 2020-11-13 20:58:39.000000 kern-smooth-1.1.1/PKG-INFO
-drwxr-xr-x   0 alexanderbutyaev   (501) staff       (20)        0 2020-11-13 20:58:39.000000 kern-smooth-1.1.1/kern_smooth.egg-info/
--rw-r--r--   0 alexanderbutyaev   (501) staff       (20)     3438 2020-11-13 20:58:39.000000 kern-smooth-1.1.1/kern_smooth.egg-info/PKG-INFO
--rw-r--r--   0 alexanderbutyaev   (501) staff       (20)      273 2020-11-13 20:58:39.000000 kern-smooth-1.1.1/kern_smooth.egg-info/SOURCES.txt
--rw-r--r--   0 alexanderbutyaev   (501) staff       (20)       19 2020-11-13 20:58:39.000000 kern-smooth-1.1.1/kern_smooth.egg-info/requires.txt
--rw-r--r--   0 alexanderbutyaev   (501) staff       (20)       12 2020-11-13 20:58:39.000000 kern-smooth-1.1.1/kern_smooth.egg-info/top_level.txt
--rw-r--r--   0 alexanderbutyaev   (501) staff       (20)        1 2020-11-13 20:58:39.000000 kern-smooth-1.1.1/kern_smooth.egg-info/dependency_links.txt
-drwxr-xr-x   0 alexanderbutyaev   (501) staff       (20)        0 2020-11-13 20:58:39.000000 kern-smooth-1.1.1/kern_smooth/
--rw-r--r--   0 alexanderbutyaev   (501) staff       (20)     9757 2020-11-13 20:08:06.000000 kern-smooth-1.1.1/kern_smooth/ks.py
--rw-r--r--   0 alexanderbutyaev   (501) staff       (20)       35 2020-07-05 04:13:30.000000 kern-smooth-1.1.1/kern_smooth/__init__.py
--rw-r--r--   0 alexanderbutyaev   (501) staff       (20)      117 2020-07-05 04:13:30.000000 kern-smooth-1.1.1/MANIFEST.in
--rw-r--r--   0 alexanderbutyaev   (501) staff       (20)     2164 2020-11-13 20:14:24.000000 kern-smooth-1.1.1/README
--rw-r--r--   0 alexanderbutyaev   (501) staff       (20)      953 2020-11-13 20:58:31.000000 kern-smooth-1.1.1/setup.py
--rw-r--r--   0 alexanderbutyaev   (501) staff       (20)       76 2020-11-13 20:58:39.000000 kern-smooth-1.1.1/setup.cfg
--rw-r--r--   0 alexanderbutyaev   (501) staff       (20)   293572 2020-11-13 20:54:06.000000 kern-smooth-1.1.1/example_density.png
+drwxr-xr-x   0 alexanderbutyaev   (501) staff       (20)        0 2023-05-31 17:28:01.014327 kern-smooth-1.1.2/
+-rw-r--r--   0 alexanderbutyaev   (501) staff       (20)     1073 2020-07-05 04:13:30.000000 kern-smooth-1.1.2/LICENSE
+-rw-r--r--   0 alexanderbutyaev   (501) staff       (20)      117 2020-07-05 04:13:30.000000 kern-smooth-1.1.2/MANIFEST.in
+-rw-r--r--   0 alexanderbutyaev   (501) staff       (20)     2685 2023-05-31 17:28:01.014632 kern-smooth-1.1.2/PKG-INFO
+-rw-r--r--   0 alexanderbutyaev   (501) staff       (20)     2164 2020-11-13 20:14:24.000000 kern-smooth-1.1.2/README
+-rw-r--r--   0 alexanderbutyaev   (501) staff       (20)   293572 2020-11-13 20:54:06.000000 kern-smooth-1.1.2/example_density.png
+drwxr-xr-x   0 alexanderbutyaev   (501) staff       (20)        0 2023-05-31 17:28:01.010571 kern-smooth-1.1.2/kern_smooth/
+-rw-r--r--   0 alexanderbutyaev   (501) staff       (20)       35 2020-07-05 04:13:30.000000 kern-smooth-1.1.2/kern_smooth/__init__.py
+-rw-r--r--   0 alexanderbutyaev   (501) staff       (20)     9754 2023-05-31 14:53:41.000000 kern-smooth-1.1.2/kern_smooth/ks.py
+drwxr-xr-x   0 alexanderbutyaev   (501) staff       (20)        0 2023-05-31 17:28:01.013863 kern-smooth-1.1.2/kern_smooth.egg-info/
+-rw-r--r--   0 alexanderbutyaev   (501) staff       (20)     2685 2023-05-31 17:28:00.000000 kern-smooth-1.1.2/kern_smooth.egg-info/PKG-INFO
+-rw-r--r--   0 alexanderbutyaev   (501) staff       (20)      281 2023-05-31 17:28:00.000000 kern-smooth-1.1.2/kern_smooth.egg-info/SOURCES.txt
+-rw-r--r--   0 alexanderbutyaev   (501) staff       (20)        1 2023-05-31 17:28:00.000000 kern-smooth-1.1.2/kern_smooth.egg-info/dependency_links.txt
+-rw-r--r--   0 alexanderbutyaev   (501) staff       (20)       19 2023-05-31 17:28:00.000000 kern-smooth-1.1.2/kern_smooth.egg-info/requires.txt
+-rw-r--r--   0 alexanderbutyaev   (501) staff       (20)       12 2023-05-31 17:28:00.000000 kern-smooth-1.1.2/kern_smooth.egg-info/top_level.txt
+-rw-r--r--   0 alexanderbutyaev   (501) staff       (20)       76 2023-05-31 17:28:01.015431 kern-smooth-1.1.2/setup.cfg
+-rw-r--r--   0 alexanderbutyaev   (501) staff       (20)      957 2023-05-31 15:05:53.000000 kern-smooth-1.1.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `kern-smooth-1.1.1/PKG-INFO` & `kern-smooth-1.1.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,104 +1,104 @@
-Metadata-Version: 1.0
+Metadata-Version: 2.1
 Name: kern-smooth
-Version: 1.1.1
+Version: 1.1.2
 Summary: A python implementation of KernSmooth package (https://cran.r-project.org/web/packages/KernSmooth):kernel smoothing and density estimation functions based on the book: Wand, M.P. and Jones, M.C. (1995) "Kernel Smoothing".
 Home-page: https://github.com/AlexanderButyaev/kern_smooth
 Author: Alexander Butyaev
 Author-email: alexander.butyaev@mail.mcgill.ca
 License: MIT
-Description: KernSmooth for Python
-        =====================
-        Porting popular R library KernSmooth to python.
-        
-        Functions for Kernel Smoothing and Density Estimation.
-        
-        Transformed R and Fortran functions into Python(2,3) code.
-        
-        Attention:
-        ----------
-        
-        Please use kern-smooth 1.1.0 or newer.
-        Reason: found not needed log10 density transformation.
-        
-        
-        Installation:
-        -------------
-        
-        .. code:: shell
-        
-        		pip install kern-smooth
-        
-        
-        Main function of the module:
-        ----------------------------
-        
-        .. code:: python
-                
-                def densCols(x, y=None, nbin=128, bandwidth=None)
-        
-        
-        Produces a vector of numbers which encode the local densities at each point in dataset.
-        
-        x, y : 1D numpy array with coordinates of the points density will be estimated on
-        
-        nbin : [optional] int or [int, int] - number of bins along each axis
-            (in case of single value - [nbin, nbin] will be used). Default value 128.
-        
-        bandwidth : [optional] numeric vector (len of 1 or 2) of smoothing bandwidth.
-        
-        Returns: numpy array with numerical representation (in range [0,1]) of point densities.
-        
-        Attention: For return value numpy.nan values are allowed in case of nan / infinite values in original dataset 
-        
-        Source: R::grDevices::densCols
-        
-        
-        Usage
-        -----
-        
-        Generate data for plotting
-        
-        .. code:: python
-        
-            from matplotlib import pyplot as plt
-            from matplotlib import cm
-            import numpy as np
-            np.random.seed(0)
-            # create two 'bulbs' with normal distributions
-            mean1 = [0, 0]
-            cov1 = [[5, 0], [0, 30]]  # diagonal covariance
-            x1, y1 = np.random.multivariate_normal(mean1, cov1, 50000).T
-            mean2 = [5, 17]
-            cov2 = [[30, 0], [0, 5]]  # diagonal covariance
-            x2, y2 = np.random.multivariate_normal(mean2, cov2, 50000).T
-            x = np.hstack([x1,x2])
-            y = np.hstack([y1,y2])
-        
-        
-        Generate point densities:
-        
-        .. code:: python
-        
-            from kern_smooth import densCols
-            densities = densCols(x, y, nbin = 128)
-        
-        
-        Plot the result
-        
-        .. code:: python
-        
-            sc = plt.scatter(x, y, c=densities, s=15, edgecolors='none', alpha=0.75, cmap=cm.jet)
-            plt.colorbar(sc)
-            plt.show()
-        
-        
-        Result
-        ------
-        ![Result](https://github.com/AlexanderButyaev/kern_smooth/blob/master/example_density.png) 
-        
-        Author
-        ------
-        Alexander Butyaev
-        
 Keywords: statistics,probability,KDE,PDF,kernel density estimation
-Platform: UNKNOWN
+License-File: LICENSE
+
+KernSmooth for Python
+=====================
+Porting popular R library KernSmooth to python.
+
+Functions for Kernel Smoothing and Density Estimation.
+
+Transformed R and Fortran functions into Python(2,3) code.
+
+Attention:
+----------
+
+Please use kern-smooth 1.1.0 or newer.
+Reason: found not needed log10 density transformation.
+
+
+Installation:
+-------------
+
+.. code:: shell
+
+		pip install kern-smooth
+
+
+Main function of the module:
+----------------------------
+
+.. code:: python
+        
+        def densCols(x, y=None, nbin=128, bandwidth=None)
+
+
+Produces a vector of numbers which encode the local densities at each point in dataset.
+
+x, y : 1D numpy array with coordinates of the points density will be estimated on
+
+nbin : [optional] int or [int, int] - number of bins along each axis
+    (in case of single value - [nbin, nbin] will be used). Default value 128.
+
+bandwidth : [optional] numeric vector (len of 1 or 2) of smoothing bandwidth.
+
+Returns: numpy array with numerical representation (in range [0,1]) of point densities.
+
+Attention: For return value numpy.nan values are allowed in case of nan / infinite values in original dataset 
+
+Source: R::grDevices::densCols
+
+
+Usage
+-----
+
+Generate data for plotting
+
+.. code:: python
+
+    from matplotlib import pyplot as plt
+    from matplotlib import cm
+    import numpy as np
+    np.random.seed(0)
+    # create two 'bulbs' with normal distributions
+    mean1 = [0, 0]
+    cov1 = [[5, 0], [0, 30]]  # diagonal covariance
+    x1, y1 = np.random.multivariate_normal(mean1, cov1, 50000).T
+    mean2 = [5, 17]
+    cov2 = [[30, 0], [0, 5]]  # diagonal covariance
+    x2, y2 = np.random.multivariate_normal(mean2, cov2, 50000).T
+    x = np.hstack([x1,x2])
+    y = np.hstack([y1,y2])
+
+
+Generate point densities:
+
+.. code:: python
+
+    from kern_smooth import densCols
+    densities = densCols(x, y, nbin = 128)
+
+
+Plot the result
+
+.. code:: python
+
+    sc = plt.scatter(x, y, c=densities, s=15, edgecolors='none', alpha=0.75, cmap=cm.jet)
+    plt.colorbar(sc)
+    plt.show()
+
+
+Result
+------
+![Result](https://github.com/AlexanderButyaev/kern_smooth/blob/master/example_density.png) 
+
+Author
+------
+Alexander Butyaev
```

### Comparing `kern-smooth-1.1.1/kern_smooth.egg-info/PKG-INFO` & `kern-smooth-1.1.2/kern_smooth.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,104 +1,104 @@
-Metadata-Version: 1.0
+Metadata-Version: 2.1
 Name: kern-smooth
-Version: 1.1.1
+Version: 1.1.2
 Summary: A python implementation of KernSmooth package (https://cran.r-project.org/web/packages/KernSmooth):kernel smoothing and density estimation functions based on the book: Wand, M.P. and Jones, M.C. (1995) "Kernel Smoothing".
 Home-page: https://github.com/AlexanderButyaev/kern_smooth
 Author: Alexander Butyaev
 Author-email: alexander.butyaev@mail.mcgill.ca
 License: MIT
-Description: KernSmooth for Python
-        =====================
-        Porting popular R library KernSmooth to python.
-        
-        Functions for Kernel Smoothing and Density Estimation.
-        
-        Transformed R and Fortran functions into Python(2,3) code.
-        
-        Attention:
-        ----------
-        
-        Please use kern-smooth 1.1.0 or newer.
-        Reason: found not needed log10 density transformation.
-        
-        
-        Installation:
-        -------------
-        
-        .. code:: shell
-        
-        		pip install kern-smooth
-        
-        
-        Main function of the module:
-        ----------------------------
-        
-        .. code:: python
-                
-                def densCols(x, y=None, nbin=128, bandwidth=None)
-        
-        
-        Produces a vector of numbers which encode the local densities at each point in dataset.
-        
-        x, y : 1D numpy array with coordinates of the points density will be estimated on
-        
-        nbin : [optional] int or [int, int] - number of bins along each axis
-            (in case of single value - [nbin, nbin] will be used). Default value 128.
-        
-        bandwidth : [optional] numeric vector (len of 1 or 2) of smoothing bandwidth.
-        
-        Returns: numpy array with numerical representation (in range [0,1]) of point densities.
-        
-        Attention: For return value numpy.nan values are allowed in case of nan / infinite values in original dataset 
-        
-        Source: R::grDevices::densCols
-        
-        
-        Usage
-        -----
-        
-        Generate data for plotting
-        
-        .. code:: python
-        
-            from matplotlib import pyplot as plt
-            from matplotlib import cm
-            import numpy as np
-            np.random.seed(0)
-            # create two 'bulbs' with normal distributions
-            mean1 = [0, 0]
-            cov1 = [[5, 0], [0, 30]]  # diagonal covariance
-            x1, y1 = np.random.multivariate_normal(mean1, cov1, 50000).T
-            mean2 = [5, 17]
-            cov2 = [[30, 0], [0, 5]]  # diagonal covariance
-            x2, y2 = np.random.multivariate_normal(mean2, cov2, 50000).T
-            x = np.hstack([x1,x2])
-            y = np.hstack([y1,y2])
-        
-        
-        Generate point densities:
-        
-        .. code:: python
-        
-            from kern_smooth import densCols
-            densities = densCols(x, y, nbin = 128)
-        
-        
-        Plot the result
-        
-        .. code:: python
-        
-            sc = plt.scatter(x, y, c=densities, s=15, edgecolors='none', alpha=0.75, cmap=cm.jet)
-            plt.colorbar(sc)
-            plt.show()
-        
-        
-        Result
-        ------
-        ![Result](https://github.com/AlexanderButyaev/kern_smooth/blob/master/example_density.png) 
-        
-        Author
-        ------
-        Alexander Butyaev
-        
 Keywords: statistics,probability,KDE,PDF,kernel density estimation
-Platform: UNKNOWN
+License-File: LICENSE
+
+KernSmooth for Python
+=====================
+Porting popular R library KernSmooth to python.
+
+Functions for Kernel Smoothing and Density Estimation.
+
+Transformed R and Fortran functions into Python(2,3) code.
+
+Attention:
+----------
+
+Please use kern-smooth 1.1.0 or newer.
+Reason: found not needed log10 density transformation.
+
+
+Installation:
+-------------
+
+.. code:: shell
+
+		pip install kern-smooth
+
+
+Main function of the module:
+----------------------------
+
+.. code:: python
+        
+        def densCols(x, y=None, nbin=128, bandwidth=None)
+
+
+Produces a vector of numbers which encode the local densities at each point in dataset.
+
+x, y : 1D numpy array with coordinates of the points density will be estimated on
+
+nbin : [optional] int or [int, int] - number of bins along each axis
+    (in case of single value - [nbin, nbin] will be used). Default value 128.
+
+bandwidth : [optional] numeric vector (len of 1 or 2) of smoothing bandwidth.
+
+Returns: numpy array with numerical representation (in range [0,1]) of point densities.
+
+Attention: For return value numpy.nan values are allowed in case of nan / infinite values in original dataset 
+
+Source: R::grDevices::densCols
+
+
+Usage
+-----
+
+Generate data for plotting
+
+.. code:: python
+
+    from matplotlib import pyplot as plt
+    from matplotlib import cm
+    import numpy as np
+    np.random.seed(0)
+    # create two 'bulbs' with normal distributions
+    mean1 = [0, 0]
+    cov1 = [[5, 0], [0, 30]]  # diagonal covariance
+    x1, y1 = np.random.multivariate_normal(mean1, cov1, 50000).T
+    mean2 = [5, 17]
+    cov2 = [[30, 0], [0, 5]]  # diagonal covariance
+    x2, y2 = np.random.multivariate_normal(mean2, cov2, 50000).T
+    x = np.hstack([x1,x2])
+    y = np.hstack([y1,y2])
+
+
+Generate point densities:
+
+.. code:: python
+
+    from kern_smooth import densCols
+    densities = densCols(x, y, nbin = 128)
+
+
+Plot the result
+
+.. code:: python
+
+    sc = plt.scatter(x, y, c=densities, s=15, edgecolors='none', alpha=0.75, cmap=cm.jet)
+    plt.colorbar(sc)
+    plt.show()
+
+
+Result
+------
+![Result](https://github.com/AlexanderButyaev/kern_smooth/blob/master/example_density.png) 
+
+Author
+------
+Alexander Butyaev
```

### Comparing `kern-smooth-1.1.1/kern_smooth/ks.py` & `kern-smooth-1.1.2/kern_smooth/ks.py`

 * *Files 0% similar despite different names*

```diff
@@ -188,15 +188,15 @@
     gpoints1 = np.linspace(a[0], b[0], M[0])
     gpoints2 = np.linspace(a[1], b[1], M[1])
     # Linear binning strategy
     gcounts = linbin2D(x[:, 0], x[:, 1], n_break_poins=M,
                        rangex=[[a[0], b[0]], [a[1], b[1]]])
     # Compute kernel weights
     gcounts = gcounts.T
-    L = np.zeros(2, dtype=np.int)
+    L = np.zeros(2, dtype=int)
     kapid = [0, 0]
     for _id in range(2):
         L[_id] = min(math.floor(tau * h[_id] * (M[_id] - 1) /
                                 (b[_id] - a[_id])), M[_id] - 1)
         lvecid = np.array(range(0, L[_id] + 1))
         facid = (b[_id] - a[_id]) / (h[_id] * (M[_id] - 1))
         z = norm.pdf(lvecid * facid) / h[_id]  # supposed to be matrix
```

### Comparing `kern-smooth-1.1.1/README` & `kern-smooth-1.1.2/README`

 * *Files identical despite different names*

### Comparing `kern-smooth-1.1.1/setup.py` & `kern-smooth-1.1.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='kern-smooth',
-    version='1.1.1',
+    version='1.1.2',
     packages=['kern_smooth'],
     install_requires=['numpy', 'pandas', 'scipy'],
     url='https://github.com/AlexanderButyaev/kern_smooth',
     license='MIT',
     author='Alexander Butyaev',
     author_email='alexander.butyaev@mail.mcgill.ca',
     description='A python implementation of KernSmooth package (https://cran.r-project.org/web/packages/KernSmooth):' + \
-     			'kernel smoothing and density estimation functions based on the book: '+ \
-     			'Wand, M.P. and Jones, M.C. (1995) "Kernel Smoothing".',
+          'kernel smoothing and density estimation functions based on the book: '+ \
+          'Wand, M.P. and Jones, M.C. (1995) "Kernel Smoothing".',
     long_description = long_description, 
     # long_description_content_type='text/markdown',
     keywords=['statistics','probability','KDE','PDF','kernel density estimation'],
 )
```

### Comparing `kern-smooth-1.1.1/example_density.png` & `kern-smooth-1.1.2/example_density.png`

 * *Files identical despite different names*

