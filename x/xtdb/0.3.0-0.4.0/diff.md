# Comparing `tmp/xtdb-0.3.0.tar.gz` & `tmp/xtdb-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xtdb-0.3.0.tar", max compression
+gzip compressed data, was "xtdb-0.4.0.tar", max compression
```

## Comparing `xtdb-0.3.0.tar` & `xtdb-0.4.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    13827 2023-05-27 08:43:25.416783 xtdb-0.3.0/LICENSE
--rw-r--r--   0        0        0     3565 2023-05-27 08:43:25.416783 xtdb-0.3.0/README.md
--rw-r--r--   0        0        0     1567 2023-05-27 08:43:25.416783 xtdb-0.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-27 08:43:25.416783 xtdb-0.3.0/xtdb/__init__.py
--rw-r--r--   0        0        0      211 2023-05-27 08:43:25.416783 xtdb-0.3.0/xtdb/__main__.py
--rw-r--r--   0        0        0    10485 2023-05-27 08:43:25.416783 xtdb-0.3.0/xtdb/datalog.py
--rw-r--r--   0        0        0      120 2023-05-27 08:43:25.416783 xtdb-0.3.0/xtdb/exceptions.py
--rw-r--r--   0        0        0     1769 2023-05-27 08:43:25.416783 xtdb-0.3.0/xtdb/orm.py
--rw-r--r--   0        0        0     6303 2023-05-27 08:43:25.416783 xtdb-0.3.0/xtdb/query.py
--rw-r--r--   0        0        0    11713 2023-05-27 08:43:25.420783 xtdb-0.3.0/xtdb/session.py
--rw-r--r--   0        0        0     4245 1970-01-01 00:00:00.000000 xtdb-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-05-31 14:49:53.663241 xtdb-0.4.0/LICENSE
+-rw-r--r--   0        0        0     4797 2023-05-31 14:49:53.663241 xtdb-0.4.0/README.md
+-rw-r--r--   0        0        0     1567 2023-05-31 14:49:53.667241 xtdb-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-31 14:49:53.667241 xtdb-0.4.0/xtdb/__init__.py
+-rw-r--r--   0        0        0      211 2023-05-31 14:49:53.667241 xtdb-0.4.0/xtdb/__main__.py
+-rw-r--r--   0        0        0     9555 2023-05-31 14:49:53.667241 xtdb-0.4.0/xtdb/datalog.py
+-rw-r--r--   0        0        0      120 2023-05-31 14:49:53.667241 xtdb-0.4.0/xtdb/exceptions.py
+-rw-r--r--   0        0        0     1711 2023-05-31 14:49:53.667241 xtdb-0.4.0/xtdb/orm.py
+-rw-r--r--   0        0        0     6151 2023-05-31 14:49:53.667241 xtdb-0.4.0/xtdb/query.py
+-rw-r--r--   0        0        0    11748 2023-05-31 14:49:53.667241 xtdb-0.4.0/xtdb/session.py
+-rw-r--r--   0        0        0     5477 1970-01-01 00:00:00.000000 xtdb-0.4.0/PKG-INFO
```

### Comparing `xtdb-0.3.0/pyproject.toml` & `xtdb-0.4.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xtdb"
-version = "0.3.0"
+version = "0.4.0"
 packages = [{ include = "xtdb" }]
 include  = ["xtdb/**"]
 exclude = [
     "**/.idea",
     "**/.git*",
     "**/.*ignore",
     "**/.flake8",
```

### Comparing `xtdb-0.3.0/xtdb/datalog.py` & `xtdb-0.4.0/xtdb/datalog.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,15 @@
 from typing import Any, List, Optional, Union
 
 from xtdb.exceptions import XTDBException
 
 
 class Clause:
-    @classmethod
-    def commutative(cls):
-        return True
-
-    @classmethod
-    def idempotent(cls):
-        return True
+    commutative = True
+    idempotent = True
 
     def compile(self, root: bool = True, *, separator=" ") -> str:
         raise NotImplementedError
 
     def format(self) -> str:
         return self.compile(separator="\n    ")
 
@@ -62,50 +57,46 @@
     def __init__(self, clauses: List[Clause], query_section: str = "where"):
         super().__init__()
 
         self.clauses = clauses
         self.query_section = query_section
 
     def compile(self, root: bool = True, *, separator=" ") -> str:
-        collected = self._collect(separator=separator)
-
-        if all(clause.idempotent() for clause in self.clauses):
-            collected = list(set(collected))
-
-        if all(clause.commutative() for clause in self.clauses):
-            expression = separator + separator.join(sorted(collected))
-        else:
-            expression = separator + separator.join(collected)
+        compiled_clauses = self._collect(separator=separator)
+        expression = separator + separator.join(compiled_clauses)
 
         if root:
             return f":{self.query_section} [{expression}]"
 
         return expression
 
     def _collect(self, *, separator=" ") -> List:
         collected = []
 
         for clause in self.clauses:
             collected.extend(clause._collect(separator=separator))
 
+        if all(clause.idempotent for clause in self.clauses):
+            collected = list(set(collected))
+        if all(clause.commutative for clause in self.clauses):
+            collected = sorted(collected)
+
         return collected
 
     def _or(self, other: Clause) -> "Clause":
         if isinstance(other, Where):
             raise XTDBException("Cannot | on a single where, use & instead")
 
         return Or([self, other])
 
     def _and(self, other: Clause) -> Clause:
         if self.query_section != "find" and issubclass(type(other), Find):
             raise XTDBException("Cannot perform a where-find. User find-where instead.")
-
         if self.query_section == "find" and isinstance(other, And) and other.query_section != "find":
             return FindWhere(self, other)
-
         if self.query_section == "find" and isinstance(other, Where):
             return FindWhere(self, other)
 
         return And(self.clauses + [other], self.query_section)
 
 
 class Or(Clause):
@@ -119,26 +110,24 @@
 
         for clause in self.clauses:
             if isinstance(clause, And):
                 collected.append(f"(and{clause.compile(root=False, separator=separator)})")
             else:
                 collected.append(clause.compile(root=False, separator=separator))
 
-        if all(clause.idempotent() for clause in self.clauses):
+        if all(clause.idempotent for clause in self.clauses):
             collected = list(set(collected))
 
-        if all(clause.commutative() for clause in self.clauses):
-            expression = separator + separator.join(sorted(collected))
-        else:
-            expression = separator + separator.join(collected)
+        if all(clause.commutative for clause in self.clauses):
+            collected = sorted(collected)
 
         if root:
-            return f":where [(or{expression})]"
+            return f":where [(or{separator}{separator.join(collected)})]"
 
-        return f"(or{expression})"
+        return f"(or{separator}{separator.join(collected)})"
 
     def _or(self, other: Clause) -> Clause:
         return Or(self.clauses + [other])
 
 
 class Where(Clause):
     def __init__(self, document: str, field: str, value: Any = ""):
@@ -165,114 +154,88 @@
     def __init__(self, statement: str):
         self.statement = statement
 
     def __str__(self):
         return self.statement
 
 
-class Aggregate(Expression):
-    supported_aggregates = {
-        "sum": (),
-        "min": (),
-        "max": (),
-        "count": (),
-        "avg": (),
-        "median": (),
-        "variance": (),
-        "stddev": (),
-        "rand": ("N",),
-        "sample": ("N",),
-        "distinct": (),
-    }
+class _BaseAggregate(Expression):
+    supported_aggregates = ["sum", "min", "max", "count", "avg", "median", "variance", "stddev", "distinct"]
+    supported_aggregates_with_arg = ["rand", "sample"]
 
     def __init__(self, function: str, expression: str, *args):
-        if function not in self.supported_aggregates:
+        if function not in self.supported_aggregates + self.supported_aggregates_with_arg:
             raise XTDBException("Invalid aggregate function")
 
-        if len(self.supported_aggregates[function]) != len(args):
-            raise XTDBException(
-                f"Invalid arguments to aggregate function, needs: {self.supported_aggregates[function]}",
-            )
-
-        if self.supported_aggregates[function]:
-            statement = f"({function} {' '.join(args)} {expression})"
-        else:
-            statement = f"({function} {expression})"
+        if function in self.supported_aggregates:
+            super().__init__(f"({function} {expression})")
+
+        if function in self.supported_aggregates_with_arg:
+            if len(args) != 1:
+                raise XTDBException("Invalid arguments to aggregate, it needs one argument: N")
 
-        super().__init__(statement)
+            super().__init__(f"({function} {' '.join(args)} {expression})")
 
 
 class QueryKey(Clause):
     def compile(self, root: bool = True, *, separator=" ") -> str:
         raise NotImplementedError
 
     def _or(self, other: Clause) -> Clause:
         raise XTDBException("Cannot use | on query keys")
 
+    def _and(self, other: Clause) -> Clause:
+        return And([self, other])
+
 
 class Find(QueryKey):
+    commutative = False
+    idempotent = False
+
     def __init__(self, expression: Union[str, Expression]):
         self.expression = expression
 
-    @classmethod
-    def commutative(cls):
-        return False
-
-    @classmethod
-    def idempotent(cls):
-        return False
-
     def compile(self, root: bool = True, *, separator=" ") -> str:
         if root:
             return f":find [{self.expression}]"
 
         return str(self.expression)
 
     def _and(self, other: Clause) -> Clause:
         if isinstance(other, And) and other.query_section != "find":
             return FindWhere(self, other)
-
         if isinstance(other, Where):
             return FindWhere(self, other)
 
         return And([self, other], "find")
 
 
 class Limit(QueryKey):
     def __init__(self, limit: int):
         self.limit = limit
 
     def compile(self, root: bool = True, *, separator=" ") -> str:
         return f" :limit {self.limit}"
 
-    def _and(self, other: Clause) -> Clause:
-        return And([self, other])
-
 
 class Offset(QueryKey):
     def __init__(self, offset: int):
         self.offset = offset
 
     def compile(self, root: bool = True, *, separator=" ") -> str:
         return f" :offset {self.offset}"
 
-    def _and(self, other: Clause) -> Clause:
-        return And([self, other])
-
 
 class Timeout(QueryKey):
     def __init__(self, timeout: int):
         self.timeout = timeout
 
     def compile(self, root: bool = True, *, separator=" ") -> str:
         return f" :timeout {self.timeout}"
 
-    def _and(self, other: Clause) -> Clause:
-        return And([self, other])
-
 
 class FindWhere(QueryKey):
     def __init__(
         self,
         find: Clause,
         where: Clause,
         limit: Optional[Limit] = None,
@@ -297,76 +260,45 @@
         if self.timeout is not None:
             q += self.timeout.compile(separator=separator)
 
         return q + "}}"
 
     def _and(self, other: Clause) -> Clause:
         if isinstance(other, Limit):
-            return self.__class__(self.find, self.where, other, self.offset, self.timeout)
-
+            return FindWhere(self.find, self.where, other, self.offset, self.timeout)
         if isinstance(other, Offset):
-            return self.__class__(self.find, self.where, self.limit, other, self.timeout)
-
+            return FindWhere(self.find, self.where, self.limit, other, self.timeout)
         if isinstance(other, Timeout):
-            return self.__class__(self.find, self.where, self.limit, self.offset, other)
+            return FindWhere(self.find, self.where, self.limit, self.offset, other)
 
         raise XTDBException("And operator is not supported for find-where clauses")
 
 
-class Sum(Find):
-    def __init__(self, expression: str):
-        super().__init__(Aggregate("sum", expression))
-
-
-class Min(Find):
-    def __init__(self, expression: str):
-        super().__init__(Aggregate("min", expression))
-
-
-class Max(Find):
-    def __init__(self, expression: str):
-        super().__init__(Aggregate("max", expression))
-
-
-class Count(Find):
-    def __init__(self, expression: str):
-        super().__init__(Aggregate("count", expression))
-
-
-class CountDistinct(Find):
-    def __init__(self, expression: str):
-        super().__init__(Aggregate("count-distinct", expression))
-
-
-class Avg(Find):
-    def __init__(self, expression: str):
-        super().__init__(Aggregate("avg", expression))
-
-
-class Median(Find):
-    def __init__(self, expression: str):
-        super().__init__(Aggregate("median", expression))
-
-
-class Variance(Find):
-    def __init__(self, expression: str):
-        super().__init__(Aggregate("variance", expression))
-
-
-class Stddev(Find):
-    def __init__(self, expression: str):
-        super().__init__(Aggregate("stddev", expression))
-
-
-class Distinct(Find):
-    def __init__(self, expression: str):
-        super().__init__(Aggregate("distinct", expression))
-
-
-class Rand(Find):
-    def __init__(self, expression: str, N: int):
-        super().__init__(Aggregate("rand", expression, str(N)))
-
-
-class Sample(Find):
-    def __init__(self, expression: str, N: int):
-        super().__init__(Aggregate("sample", expression, str(N)))
+def _build_find_aggregation_class(name: str):
+    class Extended(Find):
+        def __init__(self, expression: str):
+            super().__init__(_BaseAggregate(name, expression))
+
+    return Extended
+
+
+def _build_find_aggregation_class_with_argument(name: str):
+    class Extended(Find):
+        def __init__(self, expression: str, N: int):
+            super().__init__(_BaseAggregate(name, expression, str(N)))
+
+    return Extended
+
+
+# Dynamically create classes extending the Find clause but do aggregations
+Sum = _build_find_aggregation_class("sum")
+Min = _build_find_aggregation_class("min")
+Max = _build_find_aggregation_class("max")
+Count = _build_find_aggregation_class("count")
+CountDistinct = _build_find_aggregation_class("count-distinct")
+Avg = _build_find_aggregation_class("avg")
+Median = _build_find_aggregation_class("median")
+Variance = _build_find_aggregation_class("variance")
+Stddev = _build_find_aggregation_class("stddev")
+Distinct = _build_find_aggregation_class("distinct")
+Rand = _build_find_aggregation_class_with_argument("rand")
+Sample = _build_find_aggregation_class_with_argument("sample")
```

### Comparing `xtdb-0.3.0/xtdb/orm.py` & `xtdb-0.4.0/xtdb/orm.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,48 +15,44 @@
         return self._pk_proxy
 
     @classmethod
     def fields(cls):
         return cls.__dataclass_fields__
 
     @classmethod
-    def _relations(cls) -> List[str]:
+    def relations(cls) -> List[str]:
         return [key for key, value in cls.fields().items() if issubclass(value.type, Base)]
 
     @classmethod
-    def _subclasses(cls) -> List[Type["Base"]]:
+    def subclasses(cls) -> List[Type["Base"]]:
         return cls.__subclasses__()
 
     @classmethod
     def alias(cls):
         return cls.__name__
 
     def dict(self) -> Dict:
-        result = {}
+        result = {"xt/id": self.id, "type": self.alias()}
 
         for key, value in asdict(self).items():
             if issubclass(self.fields().get(key).type, Base):
                 field = self.__getattribute__(key)
 
                 # Foreign keys are not always hydrated
                 result[f"{self.alias()}/{key}"] = field.id if isinstance(field, Base) else field
             else:
                 result[f"{self.alias()}/{key}"] = value
 
-        result["xt/id"] = self.id
-        result["type"] = self.alias()
-
         return result
 
     @classmethod
     def from_dict(cls, document: Dict) -> "Base":
         doc = {key.replace(f"{cls.alias()}/", ""): value for key, value in document.items()}
-        pk = doc["xt/id"]
+        pk = doc.pop("xt/id")
 
-        del doc["xt/id"]
         del doc["type"]
 
         instance = cls(**doc)
         instance._pk_proxy = pk
 
         return instance
```

### Comparing `xtdb-0.3.0/xtdb/query.py` & `xtdb-0.4.0/xtdb/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,31 +19,28 @@
     Stddev,
     Sum,
     Timeout,
     Variance,
     Where,
 )
 from xtdb.exceptions import InvalidField
-from xtdb.orm import Base
+from xtdb.orm import TYPE_FIELD, Base
 
 
 @dataclass
 class Var:
     val: str
 
     def __str__(self):
         return f"?{self.val}"
 
 
 @dataclass
 class Query:
-    """Object representing an XTDB query.
-
-        result_type: Object being queried: executing the query should yield only this Object.
-
+    """
     Example usage:
 
     >>> query = Query(Object1).where(Object1, name="test")
     >>> query = query.where(Object2, object_one_reference=Object1)
     >>> query.format()
     '
     {:query {:find [(pull Object1 [*])] :where [
@@ -53,15 +50,14 @@
     '
     """
 
     result_type: Type[Base]
 
     _find: Optional[Clause] = None
     _where: Optional[Clause] = None
-
     _limit: Optional[Limit] = None
     _offset: Optional[Offset] = None
     _timeout: Optional[Timeout] = None
 
     _preserved_return_type: bool = True
 
     def where(self, object_type: Type[Base], **kwargs) -> "Query":
@@ -168,54 +164,47 @@
         self, object_type: Type[Base], field_name: str, value: Union[Type[Base], Var, str, None]
     ) -> None:
         if field_name not in object_type.fields():
             raise InvalidField(f'"{field_name}" is not a field of {object_type.alias()}')
 
         if isinstance(value, str):
             value = value.replace('"', r"\"")
-            self._add_where_statement(object_type, field_name, f'"{value}"')
-            return
+            return self._add_where_statement(object_type, field_name, f'"{value}"')
 
-        if type(value) in [int, float, bool, Var]:
-            self._add_where_statement(object_type, field_name, f"{value}")
-            return
+        if isinstance(value, (int, float, bool, Var)):
+            return self._add_where_statement(object_type, field_name, f"{str(value).lower()}")
 
         if value is None:
-            self._add_where_statement(object_type, field_name, "nil")
-            return
+            return self._add_where_statement(object_type, field_name, "nil")
 
         # TODO: support for list and dict?
         if not isinstance(value, type):
             raise InvalidField(f"value '{value}' should be a string or a Base Type")
-
         if not issubclass(value, Base):
             raise InvalidField(f"{value} is not an Base Type")
-
-        if field_name not in object_type._relations():
+        if field_name not in object_type.relations():
             raise InvalidField(f'"{field_name}" is not a relation of {object_type.alias()}')
 
-        if object_type._subclasses():
-            self._add_or_statement(object_type, field_name, value.alias())
-            return
+        if object_type.subclasses():
+            return self._add_or_statement(object_type, field_name, value.alias())
 
         self._add_where_statement(object_type, field_name, value.alias())
 
     def _add_where_statement(self, object_type: Type[Base], field_name: str, to_alias: str) -> None:
         self._where = self._where & Where(object_type.alias(), f"{object_type.alias()}/{field_name}", to_alias)
 
     def _add_or_statement(self, object_type: Type[Base], field_name: str, to_alias: str) -> None:
         clauses = [
-            Where(object_type.alias(), f"{sc.alias()}/{field_name}", to_alias) for sc in object_type._subclasses()
+            Where(object_type.alias(), f"{sc.alias()}/{field_name}", to_alias) for sc in object_type.subclasses()
         ]
         self._where = self._where & Or(clauses)  # type: ignore
 
     def _compile(self, *, separator=" ") -> str:
-        where = self._where & Where(self.result_type.alias(), "type", f'"{self.result_type.alias()}"')
+        where = self._where & Where(self.result_type.alias(), TYPE_FIELD, f'"{self.result_type.alias()}"')
         find = Find(f"(pull {self.result_type.alias()} [*])") if self._find is None else self._find
-
         find_where = find & where & self._limit & self._offset & self._timeout
 
         return find_where.compile(separator=separator)
 
     def __str__(self) -> str:
         return self._compile()
```

### Comparing `xtdb-0.3.0/xtdb/session.py` & `xtdb-0.4.0/xtdb/session.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,19 +5,20 @@
 from enum import Enum
 from typing import Any, Dict, List, Literal, Optional, Type, Union
 
 from requests import HTTPError, Response, Session
 from requests.adapters import HTTPAdapter
 from urllib3 import Retry
 
+from xtdb.datalog import Clause, FindWhere
 from xtdb.exceptions import XTDBException
 from xtdb.orm import Base, Fn
 from xtdb.query import Query
 
-logger = logging.getLogger(__name__)
+logger = logging.getLogger("XTDB")
 
 
 @dataclass
 class XTDBStatus:
     version: Optional[str]
     revision: Optional[str]
     indexVersion: Optional[int]
@@ -43,18 +44,16 @@
 
     def to_list(self):
         if self.valid_time is None:
             self.valid_time = datetime.now(timezone.utc)
 
         if self.type is OperationType.MATCH:
             return [self.type.value, self.value["xt/id"], self.value, self.valid_time.isoformat()]
-
         if self.type is OperationType.FN:
             return [self.type.value, self.value["identifier"], *self.value["args"]]
-
         if self.type is OperationType.PUT and "xt/fn" in self.value:
             return [self.type.value, self.value]
 
         return [self.type.value, self.value, self.valid_time.isoformat()]
 
     @classmethod
     def put(cls, document: Dict, valid_time: Optional[datetime] = None) -> "Operation":
@@ -92,75 +91,62 @@
     def __init__(self, base_url: str):
         self.base_url = base_url
 
         self._session = Session()
         self._session.mount("http://", HTTPAdapter(max_retries=Retry(total=6, backoff_factor=0.5)))
         self._session.mount("https://", HTTPAdapter(max_retries=Retry(total=6, backoff_factor=0.5)))
         self._session.headers["Accept"] = "application/json"
+        self._session.hooks["response"] = self._verify_response
+
+        logger.debug("Initialized HTTP session to %s", self.base_url)
 
     @staticmethod
-    def _verify_response(response: Response) -> None:
+    def _verify_response(response: Response, *args, **kwargs) -> None:
+        logger.debug('"%s %s" %s', response.request.method, response.request.url, response.status_code)
+
         try:
             response.raise_for_status()
         except HTTPError as e:
             logger.exception("Request failed")
 
             raise XTDBException from e
 
     def status(self) -> XTDBStatus:
-        res = self._session.get(f"{self.base_url}/status")
-        self._verify_response(res)
-
-        return XTDBStatus(**res.json())
+        return XTDBStatus(**self._session.get(f"{self.base_url}/status").json())
 
     def get_entity(
         self,
         eid: str,
         *,
         valid_time: Optional[datetime] = None,
         tx_time: Optional[datetime] = None,
         tx_id: Optional[int] = None,
     ) -> Dict:
-        params = {"eid": eid}
-
-        if valid_time is not None:
-            params["valid-time"] = valid_time.isoformat()
-
-        if tx_time is not None:
-            params["tx-time"] = tx_time.isoformat()
-
-        if tx_id is not None:
-            params["tx-id"] = str(tx_id)
+        params = self._format_parameter("eid", eid)
+        params = self._format_parameter("valid-time", valid_time, params)
+        params = self._format_parameter("tx-time", tx_time, params)
+        params = self._format_parameter("tx-id", tx_id, params)
 
         res = self._session.get(f"{self.base_url}/entity", params=params)
-        self._verify_response(res)
         return res.json()
 
     def get_entity_transactions(
         self,
         eid: str,
         *,
         valid_time: Optional[datetime] = None,
         tx_time: Optional[datetime] = None,
         tx_id: Optional[int] = None,
     ) -> Dict:
-        params = {"eid": eid}
-
-        if valid_time is not None:
-            params["valid-time"] = valid_time.isoformat()
+        params = self._format_parameter("eid", eid)
+        params = self._format_parameter("valid-time", valid_time, params)
+        params = self._format_parameter("tx-time", tx_time, params)
+        params = self._format_parameter("tx-id", tx_id, params)
 
-        if tx_time is not None:
-            params["tx-time"] = tx_time.isoformat()
-
-        if tx_id is not None:
-            params["tx-id"] = str(tx_id)
-
-        res = self._session.get(f"{self.base_url}/entity-tx", params=params)
-        self._verify_response(res)
-        return res.json()
+        return self._session.get(f"{self.base_url}/entity-tx", params=params).json()
 
     def get_entity_history(
         self,
         eid: str,
         *,
         sort_order: Literal["asc", "desc"] = "asc",
         with_corrections: bool = False,
@@ -168,161 +154,112 @@
         start_valid_time: Optional[datetime] = None,
         start_tx_time: Optional[datetime] = None,
         start_tx_id: Optional[int] = None,
         end_valid_time: Optional[datetime] = None,
         end_tx_time: Optional[datetime] = None,
         end_tx_id: Optional[int] = None,
     ) -> Dict:
-        params = {
-            "eid": eid,
-            "history": "true",
-            "sortOrder": sort_order,
-            "with-corrections": str(with_corrections).lower(),
-            "with-docs": str(with_docs).lower(),
-        }
-
-        if start_valid_time is not None:
-            params["start-valid-time"] = start_valid_time.isoformat()
-
-        if start_tx_time is not None:
-            params["start-tx-time"] = start_tx_time.isoformat()
-
-        if start_tx_id is not None:
-            params["start-tx-id"] = str(start_tx_id)
+        params = self._format_parameter("eid", eid)
+        params = self._format_parameter("history", True, params)
+        params = self._format_parameter("sort-order", sort_order, params)
+        params = self._format_parameter("with-corrections", with_corrections, params)
+        params = self._format_parameter("with-docs", with_docs, params)
+        params = self._format_parameter("start-valid-time", start_valid_time, params)
+        params = self._format_parameter("start-tx-time", start_tx_time, params)
+        params = self._format_parameter("start-tx-id", start_tx_id, params)
+        params = self._format_parameter("end-valid-time", end_valid_time, params)
+        params = self._format_parameter("end-tx-time", end_tx_time, params)
+        params = self._format_parameter("end-tx-id", end_tx_id, params)
 
-        if end_valid_time is not None:
-            params["end-valid-time"] = end_valid_time.isoformat()
-
-        if end_tx_time is not None:
-            params["end-tx-time"] = end_tx_time.isoformat()
-
-        if end_tx_id is not None:
-            params["end-tx-id"] = str(end_tx_id)
-
-        res = self._session.get(f"{self.base_url}/entity", params=params)
-        self._verify_response(res)
-        return res.json()
+        return self._session.get(f"{self.base_url}/entity", params=params).json()
 
     def get_attribute_stats(self):
-        res = self._session.get(f"{self.base_url}/attribute-stats")
-        self._verify_response(res)
-
-        return res.json()
+        return self._session.get(f"{self.base_url}/attribute-stats").json()
 
     def sync(self, timeout: Optional[int] = None):
-        params = {} if timeout is None else {"timeout": timeout}
-
-        res = self._session.get(f"{self.base_url}/sync", params=params)
-        self._verify_response(res)
-
-        return res.json()
+        return self._session.get(f"{self.base_url}/sync", params=self._format_parameter("timeout", timeout)).json()
 
     def query(
         self,
-        query: Union[str, Query],
+        query: Union[str, Query, Clause],
         *,
         valid_time: Optional[datetime] = None,
         tx_time: Optional[datetime] = None,
         tx_id: Optional[int] = None,
     ) -> Union[List, Dict]:
-        params = {}
-
-        if valid_time is not None:
-            params["valid-time"] = valid_time.isoformat()
-
-        if tx_time is not None:
-            params["tx-time"] = tx_time.isoformat()
+        if not isinstance(query, (str, Query)) and not issubclass(type(query), FindWhere):
+            raise XTDBException("Cannot query using incomplete clause")
 
-        if tx_id is not None:
-            params["tx-id"] = str(tx_id)
-
-        res = self._session.post(
-            f"{self.base_url}/query",
-            params=params,
-            data=str(query),
-            headers={"Content-Type": "application/edn"},
-        )
-        self._verify_response(res)
-        return res.json()
+        params = self._format_parameter("valid-time", valid_time)
+        params = self._format_parameter("tx-time", tx_time, params)
+        params = self._format_parameter("tx-id", tx_id, params)
+
+        return self._session.post(
+            f"{self.base_url}/query", str(query), params=params, headers={"Content-Type": "application/edn"}
+        ).json()
 
     def await_transaction(self, tx_id: int, timeout: Optional[int] = None) -> None:
-        params = {"txId": tx_id} if timeout is None else {"txId": tx_id, "timeout": timeout}
+        params = self._format_parameter("timeout", timeout)
+        params = self._format_parameter("tx-id", tx_id, params)
 
         self._session.get(f"{self.base_url}/await-tx", params=params)
 
     def await_transaction_time(self, tx_time: datetime, timeout: Optional[int] = None) -> None:
-        params = {"tx-time": tx_time.isoformat()}
-
-        if timeout is not None:
-            params["timeout"] = str(timeout)
+        params = self._format_parameter("tx-time", tx_time)
+        params = self._format_parameter("timeout", timeout, params)
 
         self._session.get(f"{self.base_url}/await-tx-time", params=params)
 
     def get_transaction_log(self, after_tx_id: Optional[int] = None, with_ops: Optional[bool] = None):
-        params = {}
-
-        if after_tx_id is not None:
-            params["after-tx-id"] = str(after_tx_id)
+        params = self._format_parameter("after-tx-id", after_tx_id)
+        params = self._format_parameter("with-ops?", with_ops, params)
 
-        if with_ops is not None:
-            params["with-ops?"] = str(with_ops).lower()
-
-        res = self._session.get(f"{self.base_url}/tx-log", params=params)
-        self._verify_response(res)
-
-        return res.json()
+        return self._session.get(f"{self.base_url}/tx-log", params=params).json()
 
     def submit_transaction(self, transaction: Union[Transaction, List]) -> None:
         if isinstance(transaction, list):
             transaction = Transaction(operations=transaction)
 
         res = self._session.post(
-            f"{self.base_url}/submit-tx",
-            data=transaction.json(),
-            headers={"Content-Type": "application/json"},
+            f"{self.base_url}/submit-tx", transaction.json(), headers={"Content-Type": "application/json"}
         )
 
-        self._verify_response(res)
         self.await_transaction(res.json()["txId"])
 
     def get_transaction_committed(self, tx_id: int):
-        res = self._session.get(f"{self.base_url}/tx-committed", params={"tx-id": tx_id})
-
-        self._verify_response(res)
-        return res.json()
+        return self._session.get(f"{self.base_url}/tx-committed", params=self._format_parameter("tx-id", tx_id)).json()
 
     def get_latest_completed_transaction(self):
-        res = self._session.get(f"{self.base_url}/latest-completed-tx")
-
-        self._verify_response(res)
-        return res.json()
+        return self._session.get(f"{self.base_url}/latest-completed-tx").json()
 
     def get_latest_submitted_transaction(self):
-        res = self._session.get(f"{self.base_url}/latest-submitted-tx")
-
-        self._verify_response(res)
-        return res.json()
+        return self._session.get(f"{self.base_url}/latest-submitted-tx").json()
 
     def get_active_queries(self):
-        res = self._session.get(f"{self.base_url}/active-queries")
-
-        self._verify_response(res)
-        return res.json()
+        return self._session.get(f"{self.base_url}/active-queries").json()
 
     def get_recent_queries(self):
-        res = self._session.get(f"{self.base_url}/recent-queries")
-
-        self._verify_response(res)
-        return res.json()
+        return self._session.get(f"{self.base_url}/recent-queries").json()
 
     def get_slowest_queries(self):
-        res = self._session.get(f"{self.base_url}/slowest-queries")
+        return self._session.get(f"{self.base_url}/slowest-queries").json()
 
-        self._verify_response(res)
-        return res.json()
+    @staticmethod
+    def _format_parameter(
+        key: str, parameter: Union[None, datetime, int, str, bool], current_params: Optional[Dict] = None
+    ) -> Dict:
+        if current_params is None:
+            current_params = {}
+
+        if isinstance(parameter, datetime):
+            current_params[key] = parameter.isoformat()
+        if isinstance(parameter, (int, str, bool)):
+            current_params[key] = str(parameter).lower()
+
+        return current_params
 
 
 class XTDBSession:
     def __init__(self, base_url: str):
         self.client = XTDBClient(base_url)
         self._transaction = Transaction()
 
@@ -356,14 +293,15 @@
     def evict(self, document: Base, valid_time: Optional[datetime] = None) -> None:
         self._transaction.add(Operation.evict(document.id, valid_time))
 
     def fn(self, function: Fn, *args) -> None:
         self._transaction.add(Operation.fn(function.identifier, *args))
 
     def commit(self) -> None:
-        if not self._transaction.operations:
+        if operation_count := len(self._transaction.operations) == 0:
             return
 
         try:
             self.client.submit_transaction(self._transaction)
+            logger.debug("Committed %s operations", operation_count)
         finally:
             self._transaction = Transaction()
```

### Comparing `xtdb-0.3.0/PKG-INFO` & `xtdb-0.4.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xtdb
-Version: 0.3.0
+Version: 0.4.0
 Summary: A Python ORM for XTDB.
 Home-page: https://github.com/Donnype/xtdb-py
 Author: Donny Peeters
 Author-email: donny.peeters@hotmail.com
 Maintainer: Donny Peeters
 Maintainer-email: donny.peeters@hotmail.com
 Requires-Python: >=3.8,<4.0
@@ -13,59 +13,84 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: requests (>=2.26.0,<3.0.0)
 Project-URL: Repository, https://github.com/Donnype/xtdb-py
 Description-Content-Type: text/markdown
 
-![Logo](docs/logo.png)
+![Logo](https://raw.githubusercontent.com/Donnype/xtdb-py/main/docs/logo.png)
 
-# XTDB Python: A Python ORM for XTDB
+# XTDB Python: A Python ORM for [XTDB](https://www.xtdb.com/)
 
+<div align="center">
 
-[![Tests](https://github.com/Donnype/xtdb-py/actions/workflows/tests.yml/badge.svg)](https://github.com/Donnype/xtdb-py/actions/workflows/tests.yml)
-[![Stable Version](https://img.shields.io/pypi/v/xtdb?label=stable)](https://pypi.org/project/xtdb/#history)
 [![Python Versions](https://img.shields.io/pypi/pyversions/xtdb)](https://pypi.org/project/xtdb/)
+[![Stable Version](https://img.shields.io/pypi/v/xtdb?label=stable)](https://pypi.org/project/xtdb/#history)
 
+[![Tests](https://github.com/Donnype/xtdb-py/actions/workflows/tests.yml/badge.svg)](https://github.com/Donnype/xtdb-py/actions/workflows/tests.yml)
+[![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/Donnype/xtdb-py/blob/main/.pre-commit-config.yaml)
+[![License](https://img.shields.io/github/license/Donnype/xtdb-py)](https://github.com/Donnype/xtdb-py/blob/main/LICENSE)
+
+</div>
 
 ## Installation
 
 You can install this project using pip:
 
 ```bash
-pip install xtdb
+$ pip install xtdb
 ```
 
 ## Usage
 
 The following examples assume you have set the `XTDB_URI` variable in your environment.
 To start experimenting, you could use the following setup using Docker:
 ```bash
 $ docker run -p 3000:3000 -d juxt/xtdb-standalone-rocksdb:1.21.0
 $ export XTDB_URI=http://localhost:3000/_xtdb
 ```
 
-### Using the client
+### Using the Client
 
-The `XTDBClient` supports the full HTTP API spec.
+The `XTDBClient` supports the full [HTTP API spec](https://docs.xtdb.com/clients/http/).
 
 ```python3
-import os
+>>> import os
+>>> from xtdb.session import XTDBClient, Operation
+>>>
+>>> client = XTDBClient(os.environ["XTDB_URI"])
+>>> client.submit_transaction([Operation.put({"xt/id": "123", "name": "fred"})])
+>>>
+>>> client.query('{:query {:find [(pull ?e [*])] :where [[ ?e :name "fred" ]]}}')
+[[{'name': 'fred', 'xt/id': '123'}]]
+>>>
+>>> client.get_entity("123")
+{'name': 'fred', 'xt/id': '123'}
+```
 
-from xtdb.session import XTDBClient, Operation
+Take a look at the spec to see the full range of functionality that maps directly to the client.
 
-client = XTDBClient(os.environ["XTDB_URI"])
-client.submit_transaction([Operation.put({"xt/id": "123", "name": "fred"})])
+### Using the Datalog module
 
-client.query('{:query {:find [(pull ?e [*])] :where [[ ?e :name "fred" ]]}}')
-client.get_entity("123")
+The [datalog](xtdb/datalog.py) module also provides a layer to construct queries with more easily.
+Given the data from [the cities example](examples/cities) has been seeded:
+```python3
+>>> from xtdb.datalog import Find, Where
+>>>
+>>> query = Find("(pull Country [*])") & Find("City") & (Where("City", "City/country", "Country") & Where("City", "City/name", '"Rome"'))
+>>> str(query)
+{:query {:find [ (pull Country [*]) City] :where [ [ City :City/country Country ] [ City :City/name "Rome" ]]}}
+>>>
+>>> client.query(query)
+[[{'type': 'Country', 'Country/name': 'Italy', 'xt/id': 'c095839f-031f-46ad-85e1-097f634ba4f0'}, '33aa7fa6-b752-4982-a772-d2dbaeda58ae']]
 ```
 
+To see more datalog query examples, check out the [unit tests](tests/test_datalog.py).
 
-### Using the ORM
+### Using the ORM and Session
 
 Below is an example of how to use the ORM functionality.
 
 ```python3
 import os
 from dataclasses import dataclass
 
@@ -80,71 +105,47 @@
 
 
 @dataclass
 class SecondEntity(Base):
     age: int
     test_entity: TestEntity
 
-
 session = XTDBSession(os.environ["XTDB_URI"])
-
 entity = TestEntity(name="test")
-session.put(entity)
-session.commit()
+
+with session:
+    session.put(entity)
 
 query = Query(TestEntity).where(TestEntity, name="test")
 result = session.query(query)
 
-assert result[0].dict() == {"TestEntity/name": "test", "type": "TestEntity", "xt/id": entity.id}
+result[0].dict() #  {"TestEntity/name": "test", "type": "TestEntity", "xt/id": "fe2a3ee0-9254-41dc-91cc-74ad9e2a16db"}
 ```
 
 To see more examples, check out the [examples directory](examples).
 Don't hesitate to add your own examples!
 
 ### Using the CLI for querying
 
 This package also comes with an easy CLI tool to query XTDB.
 To query XTDB using a plain query you can run
 
 ```bash
-$ echo '{:query {:find [(pull ?e [*])] :where [[ ?e :name "fred" ]]}}' | python -m xtdb | jq
-[
-  [
-    {
-      "xt/id": "123"
-      "name": "fred",
-      "somenil": null,
-      "somedict": {
-        "c": 3,
-        "a": "b"
-      },
-    }
-  ]
-]
+$ echo '{:query {:find [(pull ?e [*])] :where [[ ?e :name "fred" ]]}}' | python -m xtdb
+[[{"name": "fred", "xt/id": "123"}]]
 ```
 
 To use a query file the command can be modified to the following:
 
 ```bash
 $ cat query.txt
 {:query {:find [(pull ?e [*])] :where [[ ?e :name "fred" ]]}}
-$ python -m xtdb < query.txt | jq
-[
-  [
-    {
-      "xt/id": "123"
-      "name": "fred",
-      "somenil": null,
-      "somedict": {
-        "c": 3,
-        "a": "b"
-      },
-    }
-  ]
-]
+$
+$ python -m xtdb < query.txt
+[[{"name": "fred", "xt/id": "123"}]]
 ```
 
 ## Contributing
 
 
 ### Installation
```

