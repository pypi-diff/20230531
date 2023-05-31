# Comparing `tmp/aars-0.7.4.tar.gz` & `tmp/aars-0.7.5.tar.gz`

## Comparing `aars-0.7.4.tar` & `aars-0.7.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 aars-0.7.4/docs-requirements.txt
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 aars-0.7.4/mkdocs.yml
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 aars-0.7.4/requirements.txt
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 aars-0.7.4/.github/workflows/mkdocs-gh-pages.yml
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 aars-0.7.4/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 aars-0.7.4/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     4932 2020-02-02 00:00:00.000000 aars-0.7.4/docs/FastAPI_Cookbook.md
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 aars-0.7.4/docs/index.md -> ../README.md
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 aars-0.7.4/docs/Code_Reference/Exceptions.md
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 aars-0.7.4/docs/Code_Reference/utils.md
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 aars-0.7.4/docs/Code_Reference/core/AARS.md
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 aars-0.7.4/docs/Code_Reference/core/Index.md
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 aars-0.7.4/docs/Code_Reference/core/Record.md
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 aars-0.7.4/src/aars/__init__.py
--rw-r--r--   0        0        0    41699 2020-02-02 00:00:00.000000 aars-0.7.4/src/aars/core.py
--rw-r--r--   0        0        0     3916 2020-02-02 00:00:00.000000 aars-0.7.4/src/aars/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aars-0.7.4/src/aars/py.typed
--rw-r--r--   0        0        0    12374 2020-02-02 00:00:00.000000 aars-0.7.4/src/aars/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aars-0.7.4/tests/__init__.py
--rw-r--r--   0        0        0     6500 2020-02-02 00:00:00.000000 aars-0.7.4/tests/aars.py
--rw-r--r--   0        0        0     4835 2020-02-02 00:00:00.000000 aars-0.7.4/tests/aars_cached.py
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 aars-0.7.4/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 aars-0.7.4/LICENSE
--rw-r--r--   0        0        0     3322 2020-02-02 00:00:00.000000 aars-0.7.4/README.md
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 aars-0.7.4/pyproject.toml
--rw-r--r--   0        0        0     3802 2020-02-02 00:00:00.000000 aars-0.7.4/PKG-INFO
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 aars-0.7.5/docs-requirements.txt
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 aars-0.7.5/mkdocs.yml
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 aars-0.7.5/requirements.txt
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 aars-0.7.5/.github/workflows/mkdocs-gh-pages.yml
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 aars-0.7.5/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 aars-0.7.5/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     4932 2020-02-02 00:00:00.000000 aars-0.7.5/docs/FastAPI_Cookbook.md
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 aars-0.7.5/docs/index.md -> ../README.md
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 aars-0.7.5/docs/Code_Reference/Exceptions.md
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 aars-0.7.5/docs/Code_Reference/utils.md
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 aars-0.7.5/docs/Code_Reference/core/AARS.md
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 aars-0.7.5/docs/Code_Reference/core/Index.md
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 aars-0.7.5/docs/Code_Reference/core/Record.md
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 aars-0.7.5/src/aars/__init__.py
+-rw-r--r--   0        0        0    41700 2020-02-02 00:00:00.000000 aars-0.7.5/src/aars/core.py
+-rw-r--r--   0        0        0     3916 2020-02-02 00:00:00.000000 aars-0.7.5/src/aars/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aars-0.7.5/src/aars/py.typed
+-rw-r--r--   0        0        0    12873 2020-02-02 00:00:00.000000 aars-0.7.5/src/aars/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aars-0.7.5/tests/__init__.py
+-rw-r--r--   0        0        0     6480 2020-02-02 00:00:00.000000 aars-0.7.5/tests/aars.py
+-rw-r--r--   0        0        0     4984 2020-02-02 00:00:00.000000 aars-0.7.5/tests/aars_cached.py
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 aars-0.7.5/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 aars-0.7.5/LICENSE
+-rw-r--r--   0        0        0     3322 2020-02-02 00:00:00.000000 aars-0.7.5/README.md
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 aars-0.7.5/pyproject.toml
+-rw-r--r--   0        0        0     3802 2020-02-02 00:00:00.000000 aars-0.7.5/PKG-INFO
```

### Comparing `aars-0.7.4/mkdocs.yml` & `aars-0.7.5/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `aars-0.7.4/.github/workflows/mkdocs-gh-pages.yml` & `aars-0.7.5/.github/workflows/mkdocs-gh-pages.yml`

 * *Files identical despite different names*

### Comparing `aars-0.7.4/.github/workflows/publish.yml` & `aars-0.7.5/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `aars-0.7.4/.github/workflows/python-publish.yml` & `aars-0.7.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `aars-0.7.4/docs/FastAPI_Cookbook.md` & `aars-0.7.5/docs/FastAPI_Cookbook.md`

 * *Files identical despite different names*

### Comparing `aars-0.7.4/src/aars/core.py` & `aars-0.7.5/src/aars/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1015,15 +1015,15 @@
 
         while aleph_resp is None:
             try:
                 aleph_resp = await cls.session.get_messages(
                     channels=channels,
                     addresses=owners,
                     refs=[ref],
-                    pagination=50,
+                    pagination=200,
                     page=page,
                 )
             except ServerDisconnectedError:
                 retries -= 1
                 if retries == 0:
                     raise
         for message in aleph_resp.messages:
```

### Comparing `aars-0.7.4/src/aars/exceptions.py` & `aars-0.7.5/src/aars/exceptions.py`

 * *Files identical despite different names*

### Comparing `aars-0.7.4/src/aars/utils.py` & `aars-0.7.5/src/aars/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,14 +76,26 @@
                 raise KeyError(
                     f"Invalid key '{key}' for record type {record_type.__name__}"
                 )
             values[key] = item[1]
         super().__init__(values)
         self.record_type = record_type
 
+    def __repr__(self) -> str:
+        return (
+            self.record_type.__name__
+            + "."
+            + ".".join(
+                [
+                    key + "__" + self.comparators[key].name.lower() + "=" + repr(self[key])
+                    for key in self.keys()
+                ]
+            )
+        )
+
     def get_index_name(self) -> str:
         """
         Get the name of the index that this query would use.
         Returns:
             The name of the index to query.
         """
         return self.record_type.__name__ + "." + ".".join(self.keys())
@@ -128,15 +140,19 @@
         for key, comparator in self.comparators.items():
             if comparator == Comparator.IN:
                 for value in self[key]:
                     yield from IndexQuery(
                         self.record_type, **{key: value}
                     ).get_unfolded_queries()
             else:
-                yield self
+                if all(
+                    comparator != Comparator.IN
+                    for comparator in self.comparators.values()
+                ):
+                    yield self
 
 
 class PageableResponse(AsyncIterator[T], Generic[T]):
     """
     A wrapper around an AsyncIterator that allows for easy pagination and iteration, while also preventing multiple
     iterations. This is mainly used for nicer syntax when not using the async generator syntax.
```

### Comparing `aars-0.7.4/tests/aars.py` & `aars-0.7.5/tests/aars.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,18 +87,18 @@
 async def test_in_query():
     books = await asyncio.gather(
         Book(title="Siddhartha", author="Hermann Hesse", year=1922).save(),
         Book(title="Fahrenheit 451", author="Ray Bradbury", year=1953).save(),
     )
     await asyncio.sleep(1)
     fetched_books = await Book.filter(
-        title__in=["Siddhartha", "Fahrenheit 451"], year__in=[1922, 1953]
+        title="Siddhartha", year__in=[1922, 1953]
     ).all()
     assert books[0] in fetched_books
-    assert books[1] in fetched_books
+    assert books[1] not in fetched_books
 
 
 @pytest.mark.asyncio
 async def test_amending_record():
     book = await Book(title="Neurodancer", author="William Gibson").save()
     assert book.current_revision == 0
     book.title = "Neuromancer"
```

### Comparing `aars-0.7.4/tests/aars_cached.py` & `aars-0.7.5/tests/aars_cached.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,149 +1,149 @@
-import asyncio
-
-import pytest
-from aleph.sdk import AuthenticatedAlephClient
-from aleph.sdk.chains.ethereum import get_fallback_account
-from aleph.sdk.conf import settings
-from aleph.sdk.vm.cache import TestVmCache
-
-from src.aars import AARS, Index, Record
-from src.aars.exceptions import AlreadyForgottenError
-from tests.aars import Book, Library
-
-AARS(
-    session=AuthenticatedAlephClient(
-        get_fallback_account(), api_server=settings.API_HOST
-    ),
-    cache=TestVmCache(),
-)
-
-
-@pytest.fixture(scope="session")
-def event_loop():
-    yield AARS.session.http_session.loop
-    asyncio.run(AARS.session.http_session.close())
-
-
-@pytest.fixture(scope="session", autouse=True)
-def create_indices(request):
-    try:
-        Index(Book, "title")
-        Index(Book, ["title", "author"])
-        Index(Library, on="name")
-    except ValueError:
-        pass
-
-
-@pytest.mark.asyncio
-async def test_deserialization_from_cache():
-    book = await Book(title="Cached Book", author="John Doe").save()
-    await asyncio.sleep(1)
-    book.title = "Cached Book 2: The Recaching"
-    await book.save()
-    await asyncio.sleep(1)
-    fetched_book = await Book.fetch(book.item_hash).first()
-    assert book == fetched_book
-
-
-@pytest.mark.asyncio
-async def test_multi_index():
-    new_book = await Book(title="Lila", author="Robert M. Pirsig", year=1991).save()
-    # wait a few secs
-    await asyncio.sleep(1)
-    should_be_none = await Book.filter(title="Lila", author="Yo Momma").all()
-    assert len(should_be_none) == 0
-    fetched_book = await Book.filter(title="Lila", author="Robert M. Pirsig").first()
-    assert new_book == fetched_book
-
-
-@pytest.mark.asyncio
-async def test_in_query():
-    books = await asyncio.gather(
-        Book(title="Siddhartha", author="Hermann Hesse", year=1922).save(),
-        Book(title="Fahrenheit 451", author="Ray Bradbury", year=1953).save(),
-    )
-    await asyncio.sleep(1)
-    fetched_books = await Book.filter(
-        title__in=["Siddhartha", "Fahrenheit 451"], year__in=[1922, 1953]
-    ).all()
-    assert books[0] in fetched_books
-    assert books[1] in fetched_books
-
-
-@pytest.mark.asyncio
-async def test_amending_record():
-    book = await Book(title="Neurodancer", author="William Gibson").save()
-    assert book.current_revision == 0
-    book.title = "Neuromancer"
-    book = await book.save()
-    assert book.title == "Neuromancer"
-    assert len(book.revision_hashes) == 2
-    assert book.current_revision == 1
-    assert book.revision_hashes[0] == book.item_hash
-    assert book.revision_hashes[1] != book.item_hash
-    await asyncio.sleep(1)
-    old_book = await book.fetch_revision(rev_no=0)
-    old_timestamp = old_book.timestamp
-    assert old_book.title == "Neurodancer"
-    new_book = await book.fetch_revision(rev_no=1)
-    assert new_book.title == "Neuromancer"
-    assert new_book.timestamp > old_timestamp
-    assert book == new_book
-
-
-@pytest.mark.asyncio
-async def test_store_and_index_record_of_records():
-    books = await asyncio.gather(
-        Book(title="Atlas Shrugged", author="Ayn Rand").save(),
-        Book(title="The Martian", author="Andy Weir").save(),
-    )
-    new_library = await Library(name="The Library", books=books).save()
-    await asyncio.sleep(1)
-    fetched_library = await Library.filter(name="The Library").first()
-    assert new_library == fetched_library
-
-
-@pytest.mark.asyncio
-async def test_forget_object():
-    forgettable_book = await Book(
-        title="The Forgotten Book", author="Mechthild Gläser"
-    ).save()  # I'm sorry.
-    await asyncio.sleep(1)
-    await forgettable_book.forget()
-    assert forgettable_book.forgotten is True
-    await asyncio.sleep(1)
-    assert len(await Book.fetch(forgettable_book.item_hash).all()) == 0
-    with pytest.raises(AlreadyForgottenError):
-        await forgettable_book.forget()
-
-
-@pytest.mark.asyncio
-async def test_store_and_wrong_where_eq():
-    new_book = await Book(title="Atlas Shrugged", author="Ayn Rand").save()
-    assert new_book.title == "Atlas Shrugged"
-    assert new_book.author == "Ayn Rand"
-    with pytest.raises(KeyError):
-        await Book.filter(title="Atlas Shrugged", foo="bar").all()
-
-
-@pytest.mark.asyncio
-async def test_fetch_all_pagination():
-    page_one = await Book.fetch_objects().page(1, 1)
-    page_two = await Book.fetch_objects().page(2, 1)
-    assert len(page_one) == 1
-    assert len(page_two) == 1
-    assert page_one[0] != page_two[0]
-
-
-@pytest.mark.asyncio
-async def test_dict_field_save():
-    class BookWithDictAuthor(Record):
-        title: str
-        author: dict
-
-    book = await BookWithDictAuthor(
-        title="Test Book", author={"first": "John", "last": "Doe"}
-    ).save()
-    await asyncio.sleep(1)
-    fetched_book = await BookWithDictAuthor.fetch(book.item_hash).first()
-    assert fetched_book.author == {"first": "John", "last": "Doe"}
+import asyncio
+
+import pytest
+from aleph.sdk import AuthenticatedAlephClient
+from aleph.sdk.chains.ethereum import get_fallback_account
+from aleph.sdk.conf import settings
+from aleph.sdk.vm.cache import TestVmCache
+
+from src.aars import AARS, Index, Record
+from src.aars.exceptions import AlreadyForgottenError
+from tests.aars import Book, Library
+
+AARS(
+    session=AuthenticatedAlephClient(
+        get_fallback_account(), api_server=settings.API_HOST
+    ),
+    cache=TestVmCache(),
+)
+
+
+@pytest.fixture(scope="session")
+def event_loop():
+    yield AARS.session.http_session.loop
+    asyncio.run(AARS.session.http_session.close())
+
+
+@pytest.fixture(scope="session", autouse=True)
+def create_indices(request):
+    try:
+        Index(Book, "title")
+        Index(Book, ["title", "author"])
+        Index(Library, on="name")
+    except ValueError:
+        pass
+
+
+@pytest.mark.asyncio
+async def test_deserialization_from_cache():
+    book = await Book(title="Cached Book", author="John Doe").save()
+    await asyncio.sleep(1)
+    book.title = "Cached Book 2: The Recaching"
+    await book.save()
+    await asyncio.sleep(1)
+    fetched_book = await Book.fetch(book.item_hash).first()
+    assert book == fetched_book
+
+
+@pytest.mark.asyncio
+async def test_multi_index():
+    new_book = await Book(title="Lila", author="Robert M. Pirsig", year=1991).save()
+    # wait a few secs
+    await asyncio.sleep(1)
+    should_be_none = await Book.filter(title="Lila", author="Yo Momma").all()
+    assert len(should_be_none) == 0
+    fetched_book = await Book.filter(title="Lila", author="Robert M. Pirsig").first()
+    assert new_book == fetched_book
+
+
+@pytest.mark.asyncio
+async def test_in_query():
+    books = await asyncio.gather(
+        Book(title="Siddhartha", author="Hermann Hesse", year=1922).save(),
+        Book(title="Fahrenheit 451", author="Ray Bradbury", year=1953).save(),
+    )
+    await asyncio.sleep(1)
+    fetched_books = await Book.filter(
+        title__in=["Siddhartha", "Fahrenheit 451"], year__in=[1922, 1953]
+    ).all()
+    assert books[0] in fetched_books
+    assert books[1] in fetched_books
+
+
+@pytest.mark.asyncio
+async def test_amending_record():
+    book = await Book(title="Neurodancer", author="William Gibson").save()
+    assert book.current_revision == 0
+    book.title = "Neuromancer"
+    book = await book.save()
+    assert book.title == "Neuromancer"
+    assert len(book.revision_hashes) == 2
+    assert book.current_revision == 1
+    assert book.revision_hashes[0] == book.item_hash
+    assert book.revision_hashes[1] != book.item_hash
+    await asyncio.sleep(1)
+    old_book = await book.fetch_revision(rev_no=0)
+    old_timestamp = old_book.timestamp
+    assert old_book.title == "Neurodancer"
+    new_book = await book.fetch_revision(rev_no=1)
+    assert new_book.title == "Neuromancer"
+    assert new_book.timestamp > old_timestamp
+    assert book == new_book
+
+
+@pytest.mark.asyncio
+async def test_store_and_index_record_of_records():
+    books = await asyncio.gather(
+        Book(title="Atlas Shrugged", author="Ayn Rand").save(),
+        Book(title="The Martian", author="Andy Weir").save(),
+    )
+    new_library = await Library(name="The Library", books=books).save()
+    await asyncio.sleep(1)
+    fetched_library = await Library.filter(name="The Library").first()
+    assert new_library == fetched_library
+
+
+@pytest.mark.asyncio
+async def test_forget_object():
+    forgettable_book = await Book(
+        title="The Forgotten Book", author="Mechthild Gläser"
+    ).save()  # I'm sorry.
+    await asyncio.sleep(1)
+    await forgettable_book.forget()
+    assert forgettable_book.forgotten is True
+    await asyncio.sleep(1)
+    assert len(await Book.fetch(forgettable_book.item_hash).all()) == 0
+    with pytest.raises(AlreadyForgottenError):
+        await forgettable_book.forget()
+
+
+@pytest.mark.asyncio
+async def test_store_and_wrong_where_eq():
+    new_book = await Book(title="Atlas Shrugged", author="Ayn Rand").save()
+    assert new_book.title == "Atlas Shrugged"
+    assert new_book.author == "Ayn Rand"
+    with pytest.raises(KeyError):
+        await Book.filter(title="Atlas Shrugged", foo="bar").all()
+
+
+@pytest.mark.asyncio
+async def test_fetch_all_pagination():
+    page_one = await Book.fetch_objects().page(1, 1)
+    page_two = await Book.fetch_objects().page(2, 1)
+    assert len(page_one) == 1
+    assert len(page_two) == 1
+    assert page_one[0] != page_two[0]
+
+
+@pytest.mark.asyncio
+async def test_dict_field_save():
+    class BookWithDictAuthor(Record):
+        title: str
+        author: dict
+
+    book = await BookWithDictAuthor(
+        title="Test Book", author={"first": "John", "last": "Doe"}
+    ).save()
+    await asyncio.sleep(1)
+    fetched_book = await BookWithDictAuthor.fetch(book.item_hash).first()
+    assert fetched_book.author == {"first": "John", "last": "Doe"}
```

### Comparing `aars-0.7.4/.gitignore` & `aars-0.7.5/.gitignore`

 * *Files identical despite different names*

### Comparing `aars-0.7.4/LICENSE` & `aars-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aars-0.7.4/README.md` & `aars-0.7.5/README.md`

 * *Files identical despite different names*

### Comparing `aars-0.7.4/pyproject.toml` & `aars-0.7.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "aars"
-version = "0.7.4"
+version = "0.7.5"
 authors = [
   { name="Mike Hukiewitz", email="mike.hukiewitz@robotter.ai" },
 ]
 description = "Experimental Object-Document-Mapper using pydantic to store objects on Aleph.im"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `aars-0.7.4/PKG-INFO` & `aars-0.7.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aars
-Version: 0.7.4
+Version: 0.7.5
 Summary: Experimental Object-Document-Mapper using pydantic to store objects on Aleph.im
 Project-URL: Homepage, https://github.com/aleph-im/active-record-sdk
 Project-URL: Bug Tracker, https://github.com/aleph-im/active-record-sdk/issues
 Author-email: Mike Hukiewitz <mike.hukiewitz@robotter.ai>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

