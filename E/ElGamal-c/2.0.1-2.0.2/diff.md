# Comparing `tmp/ElGamal_c-2.0.1.tar.gz` & `tmp/ElGamal_c-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ElGamal_c-2.0.1.tar", last modified: Mon May 29 16:22:27 2023, max compression
+gzip compressed data, was "ElGamal_c-2.0.2.tar", last modified: Tue May 30 22:19:44 2023, max compression
```

## Comparing `ElGamal_c-2.0.1.tar` & `ElGamal_c-2.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 16:22:27.491795 ElGamal_c-2.0.1/
-drwxrwxrwx   0        0        0        0 2023-05-29 16:22:27.489398 ElGamal_c-2.0.1/ElGamal_c.egg-info/
--rw-rw-rw-   0        0        0      863 2023-05-29 16:22:27.000000 ElGamal_c-2.0.1/ElGamal_c.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      156 2023-05-29 16:22:27.000000 ElGamal_c-2.0.1/ElGamal_c.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 16:22:27.000000 ElGamal_c-2.0.1/ElGamal_c.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-29 16:22:27.000000 ElGamal_c-2.0.1/ElGamal_c.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      863 2023-05-29 16:22:27.491795 ElGamal_c-2.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     9615 2023-05-29 16:15:19.000000 ElGamal_c-2.0.1/encryptmodule.c
--rw-rw-rw-   0        0        0       42 2023-05-29 16:22:27.491795 ElGamal_c-2.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1261 2023-05-29 16:18:29.000000 ElGamal_c-2.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 22:19:44.137715 ElGamal_c-2.0.2/
+drwxrwxrwx   0        0        0        0 2023-05-30 22:19:44.134822 ElGamal_c-2.0.2/ElGamal_c.egg-info/
+-rw-rw-rw-   0        0        0      863 2023-05-30 22:19:43.000000 ElGamal_c-2.0.2/ElGamal_c.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      156 2023-05-30 22:19:43.000000 ElGamal_c-2.0.2/ElGamal_c.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 22:19:43.000000 ElGamal_c-2.0.2/ElGamal_c.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-30 22:19:43.000000 ElGamal_c-2.0.2/ElGamal_c.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      863 2023-05-30 22:19:44.137715 ElGamal_c-2.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0    12680 2023-05-30 21:59:32.000000 ElGamal_c-2.0.2/encryptmodule.c
+-rw-rw-rw-   0        0        0       42 2023-05-30 22:19:44.139909 ElGamal_c-2.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1261 2023-05-30 22:19:10.000000 ElGamal_c-2.0.2/setup.py
```

### Comparing `ElGamal_c-2.0.1/ElGamal_c.egg-info/PKG-INFO` & `ElGamal_c-2.0.2/ElGamal_c.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ElGamal-c
-Version: 2.0.1
+Version: 2.0.2
 Summary: This module is for csc281 encryption project 
 Home-page: https://github.com/Wouze/csc281-project
 Author: Wouze (Mohammad)
 Author-email: m7mdwats1@hotmail.com
 Keywords: python,c,primitive root,encryption,algamal,prime
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `ElGamal_c-2.0.1/PKG-INFO` & `ElGamal_c-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ElGamal_c
-Version: 2.0.1
+Version: 2.0.2
 Summary: This module is for csc281 encryption project 
 Home-page: https://github.com/Wouze/csc281-project
 Author: Wouze (Mohammad)
 Author-email: m7mdwats1@hotmail.com
 Keywords: python,c,primitive root,encryption,algamal,prime
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `ElGamal_c-2.0.1/encryptmodule.c` & `ElGamal_c-2.0.2/encryptmodule.c`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 #include <math.h>
 #include <stdlib.h>
 #include <stdio.h>
 #include <time.h>
 #include "string.h"
 #include "Python.h"
 
-
-unsigned int cis_prime(unsigned int n)
+int cis_prime(long long n)
 {
-  unsigned int last = (unsigned int) sqrt(n) + 1; 
+    
+    long long last = (long long) sqrtl(n) + 1; 
 
-  for (unsigned int j = 2; j <= last; ++j)
+    for (long long j = 2; j <= last; ++j)
     if (n % j == 0)
-      return 0;
+    
 
-  return 1;
+        return 0;
+        
+
+    return 1;
 }
 
 long long cpow_mod(long long x, long long y, long long z)
 {
     long long number = 1;
     while (y)
     {
@@ -26,22 +29,59 @@
             number = number * x % z;
         y >>= 1;  /* diviide 2 */
         x = (unsigned long long)x * x % z;  
     }
     return number;
 }
 
+// Mosaed function after optimization
+long long cpow_mod3(long long g, long long exp, long long n)
+{
+    
+    if (exp == 0)
+        return 1;
+    if (exp == 1)
+        return g % n;
+    if (exp == 2)
+        return (g * g) % n;
+
+    long long g_half_exp = cpow_mod3(g, exp>>1, n); // optimization
+
+    return (cpow_mod3(g, exp%2, n) * (g_half_exp*g_half_exp) % n) % n;
+}
+
+// Mosaed function after optimization
+long long cpow_mod4(long long g, long long exp, long long n)
+{
+    
+    if (exp == 0)
+        return 1;
+    if (exp == 1)
+        return g % n;
+    if (exp == 2){
+        long long rhs = n-g;
+        if (rhs < g)
+            g = rhs;
+
+        return (g * g) % n;
+
+    }
+    
+    long long g_half_exp = cpow_mod4(g, exp>>1, n); // optimization
+
+    return (cpow_mod4(g, exp%2, n) * (g_half_exp*g_half_exp) % n) % n;
+}
 
 int cis_primitive_root(int g, int n)
 {
     int i;
 
     for (i = 1; i < n - 1; i++)
     {
-        if (cpow_mod(g, i, n) == 1)
+        if (cpow_mod4(g, i, n) == 1)
             return 0;
     }
 
     return 1;
 }
 
 int gcd(int a, int b)
@@ -72,31 +112,55 @@
     return 2;
 } 
 
 long long cget_first_primitive_root_loop(long long p){
 
     long long o = 1;
     long long k;
-    
     for (long long r = 2; r < p; r++) {
         k = cpow_mod(r, o, p);
 
         while (k > 1) {
             o++;
             k *= r;
             k %= p;
         }
         if (o == (p - 1)) {
             return r;
         }
         o = 1;
     }
-
+    return -1;
 } 
 
+long long generator (long long p) {
+
+    
+    long* fact = (long*) malloc(p*sizeof(long)); 
+    long long index = 0;
+    long long phi = p-1,  n = phi;
+    for (long long i=2; i*i<=n; ++i)
+        if (n % i == 0) {
+            fact[index++] = i;
+            while (n % i == 0)
+                n /= i;
+        }
+    if (n > 1)
+        fact[index++] = n;
+
+    for (long long res=2; res<p; ++res) {
+        int ok = 1;
+        for (size_t i=0; i<index && ok; ++i)
+            ok &= cpow_mod (res, phi / fact[i], p) != 1;
+        if (ok) return res;
+            
+    }
+    return -1;
+}
+
 
 unsigned long long long_pow(long long base, long long exp){
     unsigned long long number =1;
 
     for (int i = 0; i<exp; i++)
         number *= base;
 
@@ -109,29 +173,41 @@
 
 void gen_g(int*g, int p){
     *g = cget_second_primitive_root(p);
 }
 void gen_g_FAST(int *g, int p){
     *g = cget_first_primitive_root_loop(p);
 }
+void gen_g_FASTEST(long long *g, long long p){
+    *g = generator(p);
+}
 
 void gen_e(int*e, int g, int x_secret, int p){
     *e = cpow_mod(g, x_secret, p);
 }
 
+void gen_e_L(long long*e, long long g, long long x_secret, long long p){
+    *e = cpow_mod(g, x_secret, p);
+}
+
 void gen_keys(int* g, int x_secret, int* e, int p){
     gen_g(g, p);
     gen_e(e, *g, x_secret, p);
 }
 
 void gen_keys_FAST(int* g, int x_secret, int* e, int p){
     gen_g_FAST(g, p);
     gen_e(e, *g, x_secret, p);
 }
 
+void gen_keys_FASTEST(long long* g, long long x_secret, long long* e, long long p){
+    gen_g_FASTEST(g, p);
+    gen_e_L(e, *g, x_secret, p);
+}
+
 
 void str_int(int* intgr, char* str, int str_len){
 
     for (int i = 0; i<str_len; i++){
         intgr[i] = (int) str[i];
     }
 
@@ -159,17 +235,42 @@
         str_decrpt[i] = ((str_encrpt[i] % p) * cpow_mod(secret, p-2, p)) % p;
     }
     str_decrpt[i] = '\0';
 }
 
 int main(){
 
-    int p_GLOBAL = 1009;  // Any large prime //
-    int g_GLOBAL = cget_second_primitive_root(p_GLOBAL);  // generate g //
+    clock_t t;
+    t = clock();
+    
+    long long p = 4000000007;
+    
+    int count =0;
+    // for (int i =1; i < p; i++)
+    // {
+    //     if (cis_primitive_root(i, p)){
+    //         count++;
+    //         // printf("%d Is primitive root to %d\n", i, p);   
+    //     }
+    // }
+    // int g___ = generator(p); printf("g him: %d\n", g___);
+    int g_GLOBAL_ = cget_first_primitive_root_loop(p); printf("g  my: %d\n", g_GLOBAL_);  // generate g //
+
+    t = clock() - t;
+    double time_taken = ((double)t)/CLOCKS_PER_SEC; // in seconds
+ 
+    printf("took %f seconds to execute \n", time_taken);
+    printf("number of primitive roots: %d\n", count);
 
+    return 0;
+
+    int p_GLOBAL = 1009;  // Any large prime //
+    int g_GLOBAL = cget_first_primitive_root_loop(p_GLOBAL);  // generate g //
+    int g__ = generator(p_GLOBAL);
+    printf("g: %d\ng: %d\n", g_GLOBAL, g__);
 
     int x_random_SECRET = rand() % (p_GLOBAL-2) + 1;  // My Secret key //
     x_random_SECRET = 54;
 
     int e_GLOBAL = cpow_mod(g_GLOBAL, x_random_SECRET, p_GLOBAL); // Global e //
 
     gen_keys(&g_GLOBAL, x_random_SECRET, &e_GLOBAL, p_GLOBAL);
@@ -242,30 +343,32 @@
 ###########################################################
             Py module stuff
 ###########################################################
 */
 #if 1
 
 static PyObject* is_prime(PyObject* self, PyObject* args){
-    unsigned int number, sts;
-    
-    if (!PyArg_ParseTuple(args, "i", &number))
+    long long number;
+    int sts;
+    if (!PyArg_ParseTuple(args, "L", &number))
         return NULL;
     
     sts = cis_prime(number);
+
     return PyBool_FromLong(sts);
 }
 
 static PyObject* gen_keys_p(PyObject* self, PyObject* args){
     int p, secret, g_, e_;
     
     if (!PyArg_ParseTuple(args, "ii", &p, &secret))
         return NULL;
     
     gen_keys(&g_, secret, &e_, p);
+    
     PyObject* sts = PyTuple_Pack(2, PyLong_FromLong(g_),  PyLong_FromLong(e_));
 
     return sts;
 }
 
 static PyObject* gen_keys_FAST_p(PyObject* self, PyObject* args){
     int p, secret, g_, e_;
@@ -275,14 +378,26 @@
     
     gen_keys_FAST(&g_, secret, &e_, p);
     PyObject* sts = PyTuple_Pack(2, PyLong_FromLong(g_),  PyLong_FromLong(e_));
 
     return sts;
 }
 
+static PyObject* gen_keys_FASTEST_p(PyObject* self, PyObject* args){
+    long long p, secret, g_, e_;
+    
+    if (!PyArg_ParseTuple(args, "LL", &p, &secret))
+        return NULL;
+    
+    gen_keys_FASTEST(&g_, secret, &e_, p);
+    PyObject* sts = PyTuple_Pack(2, PyLong_FromLongLong(g_),  PyLong_FromLongLong(e_));
+
+    return sts;
+}
+
 static PyObject* gen_c1_p(PyObject* self, PyObject* args){
     int  p, secret, g, sts;
     if (!PyArg_ParseTuple(args, "iii", &g, &secret, &p))
         return NULL;
     
     sts = cpow_mod(g, secret, p);
     return PyLong_FromLong(sts);
@@ -347,14 +462,15 @@
     return Py_BuildValue("s", "Version 0.2.6");
 }
 
 static PyMethodDef ElGamal_cs[] = {
     {"is_prime", is_prime, METH_VARARGS, "Calculates if the number is prime or not."},
     {"gen_keys", gen_keys_p, METH_VARARGS, "generates keys"},
     {"gen_keys_FAST", gen_keys_FAST_p, METH_VARARGS, "generates keys, but Fast"},
+    {"gen_keys_FASTEST", gen_keys_FASTEST_p, METH_VARARGS, "generates keys, but so much Fast"},
     {"gen_c1", gen_c1_p, METH_VARARGS, "generate cypher text 1"},
     {"gen_x_key", gen_x_key_py, METH_VARARGS, "generate x_key for decryption"},
     {"encrypt", encrypt_p, METH_VARARGS, "encrypt message"},
     {"decrypt", decrypt_p, METH_VARARGS, "decrypt c1, c2 cypher messages"},
     {"version", (PyCFunction)version, METH_NOARGS, "Returns the version of the module."},
     {NULL, NULL, 0, NULL}
 };
```

### Comparing `ElGamal_c-2.0.1/setup.py` & `ElGamal_c-2.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 """
 This module have been made for the project of discret math CSC281 at ksu university.
 The project supervisor is Aqil Alazimi. LinkedIn: https://www.linkedin.com/in/aqil-azmi-20903960/
 The project repo is: https://github.com/Wouze/csc281-project
 """
 
 setup(name="ElGamal_c",
-      version="2.0.1",
+      version="2.0.2",
       author="Wouze (Mohammad)",
       author_email="m7mdwats1@hotmail.com",
       description="This module is for csc281 encryption project ",
       long_description_content_type="text/markdown",
       long_description=long_description,
       url='https://github.com/Wouze/csc281-project',
       keywords=['python', 'c', 'primitive root', 'encryption', 'algamal', 'prime'],
```

