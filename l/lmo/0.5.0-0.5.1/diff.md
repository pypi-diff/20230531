# Comparing `tmp/lmo-0.5.0.tar.gz` & `tmp/lmo-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmo-0.5.0.tar", max compression
+gzip compressed data, was "lmo-0.5.1.tar", max compression
```

## Comparing `lmo-0.5.0.tar` & `lmo-0.5.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1505 2023-04-29 15:29:38.675734 lmo-0.5.0/LICENSE
--rw-r--r--   0        0        0      792 2023-05-30 00:24:12.512261 lmo-0.5.0/README.md
--rw-r--r--   0        0        0      648 2023-05-29 17:01:54.387498 lmo-0.5.0/lmo/__init__.py
--rw-r--r--   0        0        0      158 2023-05-02 20:44:05.723493 lmo-0.5.0/lmo/_meta.py
--rw-r--r--   0        0        0     1618 2023-05-29 00:06:01.539181 lmo-0.5.0/lmo/_utils.py
--rw-r--r--   0        0        0     3754 2023-05-29 19:26:06.023457 lmo-0.5.0/lmo/linalg.py
--rw-r--r--   0        0        0    11828 2023-05-30 00:07:26.249912 lmo-0.5.0/lmo/multivariate.py
--rw-r--r--   0        0        0        0 2023-04-29 15:53:33.056174 lmo-0.5.0/lmo/py.typed
--rw-r--r--   0        0        0     4393 2023-05-29 19:14:01.515594 lmo-0.5.0/lmo/stats.py
--rw-r--r--   0        0        0     1609 2023-05-29 19:12:59.718239 lmo-0.5.0/lmo/typing.py
--rw-r--r--   0        0        0    12307 2023-05-29 22:01:31.773252 lmo-0.5.0/lmo/univariate.py
--rw-r--r--   0        0        0     6670 2023-05-29 18:53:48.844937 lmo-0.5.0/lmo/weights.py
--rw-r--r--   0        0        0     1981 2023-05-30 00:24:53.249167 lmo-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     1890 1970-01-01 00:00:00.000000 lmo-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1505 2023-04-29 15:29:38.675734 lmo-0.5.1/LICENSE
+-rw-r--r--   0        0        0      792 2023-05-30 00:24:12.512261 lmo-0.5.1/README.md
+-rw-r--r--   0        0        0      738 2023-05-31 01:27:05.830069 lmo-0.5.1/lmo/__init__.py
+-rw-r--r--   0        0        0    22917 2023-05-31 01:55:50.420399 lmo-0.5.1/lmo/_lm.py
+-rw-r--r--   0        0        0    11824 2023-05-30 21:35:52.549810 lmo-0.5.1/lmo/_lm_co.py
+-rw-r--r--   0        0        0      158 2023-05-02 20:44:05.723493 lmo-0.5.1/lmo/_meta.py
+-rw-r--r--   0        0        0     4810 2023-05-31 01:21:35.070718 lmo-0.5.1/lmo/_pwm.py
+-rw-r--r--   0        0        0     1615 2023-05-30 21:36:14.694306 lmo-0.5.1/lmo/_utils.py
+-rw-r--r--   0        0        0     4467 2023-05-30 20:47:52.462490 lmo-0.5.1/lmo/linalg.py
+-rw-r--r--   0        0        0        0 2023-04-29 15:53:33.056174 lmo-0.5.1/lmo/py.typed
+-rw-r--r--   0        0        0     3387 2023-05-30 21:31:38.836128 lmo-0.5.1/lmo/stats.py
+-rw-r--r--   0        0        0     1609 2023-05-29 19:12:59.718239 lmo-0.5.1/lmo/typing.py
+-rw-r--r--   0        0        0     1981 2023-05-31 01:58:05.887410 lmo-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     1890 1970-01-01 00:00:00.000000 lmo-0.5.1/PKG-INFO
```

### Comparing `lmo-0.5.0/LICENSE` & `lmo-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lmo-0.5.0/README.md` & `lmo-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `lmo-0.5.0/lmo/__init__.py` & `lmo-0.5.1/lmo/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 __all__ = (
     '__version__',
 
+    'l_weights',
     'l_moment',
+    'l_moment_cov',
     'l_ratio',
+    'l_ratio_se',
     'l_loc',
     'l_scale',
     'l_variation',
     'l_skew',
     'l_kurtosis',
 
     'l_comoment',
@@ -15,31 +18,33 @@
     'l_coscale',
     'l_corr',
     'l_coskew',
     'l_cokurtosis',
 )
 
 from typing import Final as _Final
-
 from ._meta import get_version as _get_version
 
-from .univariate import (
+from ._lm import (
+    l_weights,
     l_moment,
+    l_moment_cov,
     l_ratio,
+    l_ratio_se,
     l_loc,
     l_scale,
     l_variation,
     l_skew,
     l_kurtosis,
 )
-from .multivariate import (
+from ._lm_co import (
     l_comoment,
     l_coratio,
+
     l_coloc,
     l_coscale,
     l_corr,
     l_coskew,
     l_cokurtosis,
 )
 
-
 __version__: _Final[str] = _get_version()
```

### Comparing `lmo-0.5.0/lmo/_utils.py` & `lmo-0.5.1/lmo/_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 __all__ = 'clean_order', 'ensure_axis_at', 'as_float_array'
 
 from typing import Any, SupportsIndex, TypeVar
 
 import numpy as np
 import numpy.typing as npt
 
-from lmo.typing import IndexOrder
+from .typing import IndexOrder
 
 T = TypeVar('T', bound=np.generic)
 
 def clean_order(
     order: SupportsIndex,
     /,
     name: str = 'r',
```

### Comparing `lmo-0.5.0/lmo/linalg.py` & `lmo-0.5.1/lmo/linalg.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,48 @@
-__all__ = 'sh_legendre', 'succession_matrix', 'tl_jacobi'
+__all__ = 'sandwich', 'sh_legendre', 'succession_matrix', 'hosking_jacobi'
 
 from typing import Any, TypeVar
 
 import numpy as np
 import numpy.typing as npt
 
-_T = TypeVar('_T', bound=npt.NBitBase)
-_N = TypeVar('_N', bound=np.number[Any])
+T = TypeVar('T', bound=np.number[Any])
+
+
+def sandwich(
+    A: npt.NDArray[np.number[Any]],
+    X: npt.NDArray[T | np.number[Any]],
+    /,
+    dtype: np.dtype[T] | type[T] = np.float_,
+) -> npt.NDArray[T]:
+    """
+    Calculates the "sandwich" matrix product (`A @ X @ A.T`) along the
+    specified `X` axis.
+
+    Args:
+        A: 2-D array of shape `(s, r)`, the "bread".
+        dtype: The data type of the result.
+        X: Array of shape `(r, r, ...)`.
+    Returns:
+        C: Array of shape `(s, s, ...)`.
+
+    See Also:
+        - https://wikipedia.org/wiki/Covariance_matrix
+
+    """
+    # if X is 1 - d, this is equivalent to: C @ S_b @ C.T
+    spec = 'ui, ij..., vj -> uv...'
+    return np.einsum(spec, A, X, A, dtype=dtype)  # pyright: ignore
 
 
 def sh_legendre(
     m : int,
     /,
-    dtype: type[_N] = np.int_,
-) -> npt.NDArray[_N]:
+    dtype: type[T] = np.int_,
+) -> npt.NDArray[T]:
     """
     Shifted legendre polynomial coefficient matrix $P^*$ of shape `(m, m)`,
     where the $k$-th coefficient of the shifted Legendre polynomial of
     degree $n$ is at $(n, k)$:
 
     $$
     p^*_{n, k} = (-1)^{n - k} \\binom{n}{k} \\binom{n + k}{k}
@@ -69,32 +94,32 @@
             lp[i, j] = lp[i - 1, j - 1] - lp[i - 1, j]
             p2[i, j] = p2[i - 1, j] + p2[i, j - 1]
 
     np.multiply(lp, p2, out=lp)
     return lp
 
 
-def succession_matrix(c: npt.NDArray[_N], /) -> npt.NDArray[_N]:
+def succession_matrix(c: npt.NDArray[T], /) -> npt.NDArray[T]:
     # TODO: docsstring + tests
 
     n, k = np.atleast_1d(c).shape
     i = np.linspace(0, n - 1, n, dtype=np.int64)
 
     out = np.zeros((n, n + k - 1), dtype=c.dtype)
     for d in range(k):
         out[i, i + d] = c[:, d]
 
     return out
 
 
-def tl_jacobi(
+def hosking_jacobi(
     r: int,
     /,
     trim: tuple[int, int],
-    dtype: type[_N] = np.float_,
+    dtype: np.dtype[T] | type[T] = np.float_,
 ) -> npt.NDArray[np.floating[Any]]:
     # TODO: docsstring + tests
 
     assert r >= 0
 
     if r == 0:
         return np.empty((0, 0), dtype=dtype)
@@ -116,16 +141,16 @@
             # (r + 1)(r + 2) / (2 r (2r + 1)) * (l_r +/- l_{r+2})
             # and (r + 1)(r + 2) / (2 r (2r + 1)) = c0 * (r + 1) / (2 r)
             return succession_matrix(np.outer(c0 * (.5 + .5 / rr), [1, 0, -1]))
         case (s, t) if s < t:
             # ((r+s+t) * _[r+0] - (r+1) * (r+s) * _[r+1] / r) / (2r+s+t-1)
             c1 = -(rr + 1) * (rr + s) / (rr * nc)
             m0 = succession_matrix(np.c_[c0, c1])
-            m1 = tl_jacobi(r + 1, (s, t - 1), dtype)
+            m1 = hosking_jacobi(r + 1, (s, t - 1), dtype)
             return m0 @ m1
         case (s, t) if s >= t:
             c1 = (rr + 1) * (rr + t) / (rr * nc)
             m0 = succession_matrix(np.c_[c0, c1])
-            m1 = tl_jacobi(r + 1, (s - 1, t), dtype)
+            m1 = hosking_jacobi(r + 1, (s - 1, t), dtype)
             return m0 @ m1
         case _ as wtf:
             assert False, wtf
```

### Comparing `lmo-0.5.0/lmo/multivariate.py` & `lmo-0.5.1/lmo/_lm_co.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 
 from typing import Any, TypeVar, cast
 
 import numpy as np
 from numpy import typing as npt
 
 from ._utils import clean_order
+from ._lm import l_weights
 from .stats import order_stats
 from .typing import AnyInt, IntVector, SortKind
-from .weights import l_weights
 
 T = TypeVar('T', bound=np.floating[Any])
 
 
 def l_comoment(
     a: npt.ArrayLike,
     r: AnyInt | IntVector,
```

### Comparing `lmo-0.5.0/lmo/stats.py` & `lmo-0.5.1/lmo/stats.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,18 @@
-__all__ = 'order_stats', 'l_ratio_max'
+__all__ = 'order_stats',
 
-from math import factorial as fact
 from typing import Any, TypeVar
 
 import numpy as np
 import numpy.typing as npt
 
-from ._utils import as_float_array, clean_order
+from ._utils import as_float_array
 from .typing import IntVector, SortKind
 
-
-T = TypeVar('T', bound=npt.NBitBase)
+T = TypeVar('T', bound=np.floating[Any])
 
 
 def _apply_aweights(
     x: npt.NDArray[np.floating[Any]],
     v: npt.NDArray[np.floating[Any]],
     axis: int,
 ) -> npt.NDArray[np.float_]:
@@ -84,17 +82,15 @@
         return np.sort(_x, axis=axis, kind=sort)
     elif y is not None:
         _y = _clean_array(y)
         i_k = np.argsort(_y, axis=axis if _y.ndim > 1 else -1, kind=sort)
     else:
         i_k = np.argsort(_x, axis=axis, kind=sort)
 
-    def _sort_like(
-        a: npt.NDArray[np.floating[T]],
-    ) -> npt.NDArray[np.floating[T]]:
+    def _sort_like(a: npt.NDArray[T]) -> npt.NDArray[T]:
         return (
             np.take(  # pyright: ignore [reportUnknownMemberType]
                 a,
                 i_k,
                 axis=None if a.ndim == i_k.ndim else axis
             )
             if min(a.ndim, i_k.ndim) <= 1
@@ -104,46 +100,7 @@
     x_k = _sort_like(_x)
 
     if aweights is None:
         return x_k
 
     w_k = _sort_like(_clean_array(aweights))
     return _apply_aweights(x_k, w_k, axis=axis or 0)
-
-
-def l_ratio_max(
-    r: int,
-    s: int = 2,
-    /,
-    trim: tuple[int, int] = (0, 0),
-) -> float:
-    """
-    The theoretical upper bound on the absolute TL-ratios, i.e.::
-
-        abs(lmo.l_ratio(a, r, s, trim)) <= tl_ratio_max(r, s, trim)
-
-    is True for all samples `a`.
-
-    References:
-        * Hosking, J.R.M., Some Theory and Practical Uses of Trimmed L-moments.
-          Page 6, equation 14.
-
-    """
-
-    # the zeroth (TL-)moment is 1. I.e. the total area under the pdf (or the
-    # sum of the ppf if discrete) is 1.
-    _r = clean_order(r)
-    _s = clean_order(s, name='s')
-
-    if _r in (0, _s):
-        return 1.0
-    if not _s:
-        return float('inf')
-
-    t1, t2 = trim
-    m = min(t1, t2)
-
-    # disclaimer: the `k` instead of a `2` here is just a guess
-    return (
-        _s * fact(m + _s - 1) * fact(t1 + t2 + _r) /
-        (_r * fact(m + _r - 1) * fact(t1 + t2 + _s))
-    )
```

### Comparing `lmo-0.5.0/lmo/typing.py` & `lmo-0.5.1/lmo/typing.py`

 * *Files identical despite different names*

### Comparing `lmo-0.5.0/pyproject.toml` & `lmo-0.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "oldest-supported-numpy"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "lmo"
-version = "0.5.0"
+version = "0.5.1"
 description = "L-Moments for robust statistics."
 authors = ["Joren Hammudoglu <jhammudoglu@gmail.com>"]
 readme = "README.md"
 license = "BSD-3-Clause"
 homepage = "https://jorenham.github.io/lmo/"
 repository = "https://github.com/jorenham/lmo/"
 classifiers = [
```

### Comparing `lmo-0.5.0/PKG-INFO` & `lmo-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmo
-Version: 0.5.0
+Version: 0.5.1
 Summary: L-Moments for robust statistics.
 Home-page: https://jorenham.github.io/lmo/
 License: BSD-3-Clause
 Author: Joren Hammudoglu
 Author-email: jhammudoglu@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
```

