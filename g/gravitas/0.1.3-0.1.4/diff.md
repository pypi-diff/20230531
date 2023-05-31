# Comparing `tmp/gravitas-0.1.3.tar.gz` & `tmp/gravitas-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gravitas-0.1.3.tar", last modified: Tue May 30 04:55:34 2023, max compression
+gzip compressed data, was "gravitas-0.1.4.tar", last modified: Wed May 31 04:50:10 2023, max compression
```

## Comparing `gravitas-0.1.3.tar` & `gravitas-0.1.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:55:34.142473 gravitas-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-30 04:55:34.142473 gravitas-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-30 04:55:21.000000 gravitas-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:55:34.138473 gravitas-0.1.3/gravitas/
--rw-r--r--   0 runner    (1001) docker     (123)  2750335 2023-05-30 04:55:21.000000 gravitas-0.1.3/gravitas/EGM96.c
--rw-r--r--   0 runner    (1001) docker     (123)  2750581 2023-05-30 04:55:21.000000 gravitas-0.1.3/gravitas/GRGM360.c
--rw-r--r--   0 runner    (1001) docker     (123)   300782 2023-05-30 04:55:21.000000 gravitas-0.1.3/gravitas/MRO120F.c
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-30 04:55:21.000000 gravitas-0.1.3/gravitas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11496 2023-05-30 04:55:21.000000 gravitas-0.1.3/gravitas/gravlib.c
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-30 04:55:21.000000 gravitas-0.1.3/gravitas/lib.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-30 04:55:21.000000 gravitas-0.1.3/gravitas/libgrav.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:55:34.142473 gravitas-0.1.3/gravitas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-30 04:55:34.000000 gravitas-0.1.3/gravitas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-30 04:55:34.000000 gravitas-0.1.3/gravitas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 04:55:34.000000 gravitas-0.1.3/gravitas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 04:55:33.000000 gravitas-0.1.3/gravitas.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-30 04:55:34.000000 gravitas-0.1.3/gravitas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-30 04:55:34.000000 gravitas-0.1.3/gravitas.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-30 04:55:21.000000 gravitas-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 04:55:34.142473 gravitas-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-30 04:55:21.000000 gravitas-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:50:10.700694 gravitas-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-31 04:50:10.700694 gravitas-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-31 04:49:59.000000 gravitas-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:50:10.696694 gravitas-0.1.4/gravitas/
+-rw-r--r--   0 runner    (1001) docker     (123)  2750335 2023-05-31 04:49:59.000000 gravitas-0.1.4/gravitas/EGM96.c
+-rw-r--r--   0 runner    (1001) docker     (123)  2750581 2023-05-31 04:49:59.000000 gravitas-0.1.4/gravitas/GRGM360.c
+-rw-r--r--   0 runner    (1001) docker     (123)   300782 2023-05-31 04:49:59.000000 gravitas-0.1.4/gravitas/MRO120F.c
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-31 04:49:59.000000 gravitas-0.1.4/gravitas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11272 2023-05-31 04:49:59.000000 gravitas-0.1.4/gravitas/gravlib.c
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-31 04:49:59.000000 gravitas-0.1.4/gravitas/lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-31 04:49:59.000000 gravitas-0.1.4/gravitas/libgrav.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:50:10.700694 gravitas-0.1.4/gravitas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-31 04:50:10.000000 gravitas-0.1.4/gravitas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-31 04:50:10.000000 gravitas-0.1.4/gravitas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 04:50:10.000000 gravitas-0.1.4/gravitas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 04:50:10.000000 gravitas-0.1.4/gravitas.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-31 04:50:10.000000 gravitas-0.1.4/gravitas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-31 04:50:10.000000 gravitas-0.1.4/gravitas.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-31 04:49:59.000000 gravitas-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 04:50:10.700694 gravitas-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-31 04:49:59.000000 gravitas-0.1.4/setup.py
```

### Comparing `gravitas-0.1.3/PKG-INFO` & `gravitas-0.1.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gravitas
-Version: 0.1.3
+Version: 0.1.4
 Author: Liam Robinson
 Author-email: robin502@purdue.edu
 License: GPL-2
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `gravitas-0.1.3/gravitas/EGM96.c` & `gravitas-0.1.4/gravitas/EGM96.c`

 * *Files identical despite different names*

### Comparing `gravitas-0.1.3/gravitas/GRGM360.c` & `gravitas-0.1.4/gravitas/GRGM360.c`

 * *Files identical despite different names*

### Comparing `gravitas-0.1.3/gravitas/MRO120F.c` & `gravitas-0.1.4/gravitas/MRO120F.c`

 * *Files identical despite different names*

### Comparing `gravitas-0.1.3/gravitas/__init__.py` & `gravitas-0.1.4/gravitas/__init__.py`

 * *Files identical despite different names*

### Comparing `gravitas-0.1.3/gravitas/gravlib.c` & `gravitas-0.1.4/gravitas/gravlib.c`

 * *Files 9% similar despite different names*

```diff
@@ -35,15 +35,16 @@
 
 double numpy_arr_el(PyArrayObject *a, int row, int col) {
     double *el_ptr = PyArray_GETPTR2(a, row, col);
     return *el_ptr;
 }
 
 void numpy_nx3_to_xyz(PyArrayObject *a, double x[], double y[], double z[]) {
-    for(int i = 0; i < PyArray_DIM(a, 0); i++) {
+    int i;
+    for(i = 0; i < PyArray_DIM(a, 0); i++) {
             x[i] = numpy_arr_el(a, i, 0);
             y[i] = numpy_arr_el(a, i, 1);
             z[i] = numpy_arr_el(a, i, 2);
     }
 }
 
 
@@ -142,15 +143,16 @@
         m = m_MRO120F; 
         c = c_MRO120F; 
         s = s_MRO120F; 
         num = ncoef_MRO120F;
         // Coefficients from: https://pds-geosciences.wustl.edu/mro/mro-m-rss-5-sdp-v1/mrors_1xxx/data/shadr/jgmro_120f_sha.tab
     }
     
-    for(int i = 0; i < num; i++) {
+    int i;
+    for(i = 0; i < num; i++) {
         int ind = nm2i(*(n+i), *(m+i));
         cnm[ind] = *(c+i);
         snm[ind] = *(s+i);
         // printf("n=%d, m=%d, c=%.2e, s=%.2e, cnm=%.2e, snm=%.2e\n", *(n+i), *(m+i), *(c+i), *(s+i), cnm[ind], snm[ind]);
         if(*(m+i) == nmax) {
             break;
         }
@@ -170,55 +172,57 @@
     // Based on pinesnorm() from: https://core.ac.uk/download/pdf/76424485.pdf
     double rmag = Vector3Norm(rf);
     Vector3 stu = Vector3Hat(rf);
     int anm_sz = nm2i(nmax+3, nmax+3);
     double *anm = malloc(anm_sz * sizeof(double)); //ansi-c
     // double anm[anm_sz];
     anm[0] = sqrt(2.0);
-     
-    for(int m = 0; m <= nmax+2; m++) {
+
+    int m;
+    for(m = 0; m <= nmax+2; m++) {
         if(m != 0) { // DIAGONAL RECURSION
             anm[nm2i(m,m)] = sqrt(1.0+1.0/(2.0*m))*anm[nm2i(m-1,m-1)];
         }
         if(m != nmax+2) { // FIRST OFF-DIAGONAL RECURSION 
             anm[nm2i(m+1,m)] = sqrt(2*m+3)*stu.z*anm[nm2i(m,m)];
         }
         if(m < nmax+1) {
-            for(int n = m+2; n <= nmax+2; n++) {
+            int n;
+            for(n = m+2; n <= nmax+2; n++) {
                 double alpha_num = (2*n+1)*(2*n-1);
                 double alpha_den = (n-m)*(n+m);
                 double alpha = sqrt(alpha_num/alpha_den);
                 double beta_num = (2*n+1)*(n-m-1)*(n+m-1);
                 double beta_den = (2*n-3)*(n+m)*(n-m);
                 double beta = sqrt(beta_num/beta_den);
                 anm[nm2i(n,m)] = alpha*stu.z*anm[nm2i(n-1,m)] - beta*anm[nm2i(n-2,m)];
             }
         }
     }
-    for(int n = 0; n <= nmax+2; n++) {
+    int n;
+    for(n = 0; n <= nmax+2; n++) {
         anm[nm2i(n,0)] *= sqrt(0.50);
     }
      
     double* rm = (double*) malloc((nmax+2) * sizeof(double)); //ansi-c
     double* im = (double*) malloc((nmax+2) * sizeof(double)); //ansi-c
-    // double rm[nmax+2];
-    // double im[nmax+2];
     rm[0] = 0.00; rm[1] = 1.00; 
     im[0] = 0.00; im[1] = 0.00; 
-    for(int m = 2; m < nmax+2; m++) {
+    for(m = 2; m < nmax+2; m++) {
         rm[m] = stu.x*rm[m-1] - stu.y*im[m-1]; 
         im[m] = stu.x*im[m-1] + stu.y*rm[m-1];
     }
     double rho  = mu/(req*rmag);
     double rhop = req/rmag;
     double g1 = 0.00; double g2 = 0.00; double g3 = 0.00; double g4 = 0.00;
     for (int n = 0; n <= nmax; n++) {
         double g1t = 0.0; double g2t = 0.0; double g3t = 0.0; double g4t = 0.0;
         double sm = 0.5;
-        for(int m = 0; m <= n; m++) {
+        int m;
+        for(m = 0; m <= n; m++) {
             double anmp1;
             if(n == m) {
                 anmp1 = 0.0;
             }
             else {
                 anmp1 = anm[nm2i(n,m+1)];
             }
@@ -252,28 +256,27 @@
     return rv;
 }
 
 typedef struct thread_args{
     int start_ind;
     int end_ind;
     int nmax;
-    double (*cnm)[];
-    double (*snm)[];
+    double *cnm;
+    double *snm;
 }thread_args;
 
 void* thread_func(void* arg) {
     struct thread_args *targs = (struct thread_args *)arg;
-    for(int i = targs->start_ind; i < targs->end_ind; i++) {
-        gs[i] = pinesnorm(rfs[i], *targs->cnm, *targs->snm, targs->nmax, mu, req);
+    int i;
+    for(i = targs->start_ind; i < targs->end_ind; i++) {
+        gs[i] = pinesnorm(rfs[i], targs->cnm, targs->snm, targs->nmax, mu, req);
     }
     return NULL;
 }
 
-// double* egm96_gravity(double x[], double y[], double z[], int npts, int nmax, char* model_name) {
-
 static PyObject *egm96_gravity(PyObject *self, PyObject *args) {
     PyArrayObject *r_ecef;
     int nmax;
     char* model_name = NULL;
     if (!PyArg_ParseTuple(args, "O!is", 
                             &PyArray_Type, &r_ecef, 
                             &nmax,
@@ -285,30 +288,26 @@
     if (PyArray_NDIM(r_ecef) != 2)
         return failure(PyExc_TypeError, "ECEF position must be [n x 3].");
 
     int npts = PyArray_DIM(r_ecef, 0);
     double* x = (double*) malloc(npts * sizeof(double)); //ansi-c
     double* y = (double*) malloc(npts * sizeof(double));
     double* z = (double*) malloc(npts * sizeof(double));
-    // double x[npts];
-    // double y[npts];
-    // double z[npts];
     PyObject* accel_vector = PyList_New(3 * npts);
     numpy_nx3_to_xyz(r_ecef, x, y, z);
 
     set_indices(model_name, &model_index, &body_index);
     set_body_params(body_index, &mu, &req);
     int sz = nm2i(nmax+2, nmax+2);
     double* cnm = (double*) malloc(sz * sizeof(double)); //ansi-c
     double* snm = (double*) malloc(sz * sizeof(double));
-    // double cnm[sz];
-    // double snm[sz];
     read_cnm_snm(nmax, model_index, cnm, snm);
 
-    for(int i = 0; i < npts; i++) {
+    int i;
+    for(i = 0; i < npts; i++) {
         rfs[i] = (Vector3){x[i], y[i], z[i]};
     }
 
     // pthread_t thread[NUM_THREADS];
     // pthread_attr_t attr;
     // pthread_attr_init(&attr);
     // size_t stacksize;
@@ -333,15 +332,15 @@
     //     }
     // }
 
     // If we just want to run on one thread
     thread_func(&(thread_args) {0, npts, nmax, cnm, snm});
     
     double* res = (double*) malloc(3 * npts * sizeof(double));
-    for(int i = 0; i < npts; i++) {
+    for(i = 0; i < npts; i++) {
         res[3*i + 0] = gs[i].x;
         res[3*i + 1] = gs[i].y;
         res[3*i + 2] = gs[i].z;
         
         PyList_SetItem(accel_vector, 3*i+0, PyFloat_FromDouble(gs[i].x));
         PyList_SetItem(accel_vector, 3*i+1, PyFloat_FromDouble(gs[i].y));
         PyList_SetItem(accel_vector, 3*i+2, PyFloat_FromDouble(gs[i].z));
```

### Comparing `gravitas-0.1.3/gravitas/lib.py` & `gravitas-0.1.4/gravitas/lib.py`

 * *Files identical despite different names*

### Comparing `gravitas-0.1.3/gravitas/libgrav.h` & `gravitas-0.1.4/gravitas/libgrav.h`

 * *Files identical despite different names*

### Comparing `gravitas-0.1.3/gravitas.egg-info/PKG-INFO` & `gravitas-0.1.4/gravitas.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gravitas
-Version: 0.1.3
+Version: 0.1.4
 Author: Liam Robinson
 Author-email: robin502@purdue.edu
 License: GPL-2
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `gravitas-0.1.3/pyproject.toml` & `gravitas-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gravitas-0.1.3/setup.py` & `gravitas-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         #     if self.compiler.compiler_type == 'msvc':
         #         ext.extra_compile_args.append('/std:c90')
         super().build_extensions()
 
 # _LIB_DIR
 setup(
     name='gravitas',
-    version='0.1.3',
+    version='0.1.4',
     packages=find_packages(),
     license='GPL-2',
     long_description="""High-fidelity gravity fields for satellite propagation""",
     long_description_content_type='text/markdown',
     author="Liam Robinson",
     author_email="robin502@purdue.edu",
     install_requires=['numpy'],
```

