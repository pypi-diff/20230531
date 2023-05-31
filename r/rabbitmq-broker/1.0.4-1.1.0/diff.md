# Comparing `tmp/rabbitmq_broker-1.0.4-py3-none-any.whl.zip` & `tmp/rabbitmq_broker-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 10988 bytes, number of entries: 15
--rw-r--r--  2.0 unx       22 b- defN 23-May-26 07:16 rmq_broker/__init__.py
--rw-r--r--  2.0 unx      620 b- defN 23-May-26 07:16 rmq_broker/schemas.py
+Zip file size: 10568 bytes, number of entries: 15
+-rw-r--r--  2.0 unx       22 b- defN 23-May-31 15:11 rmq_broker/__init__.py
+-rw-r--r--  2.0 unx     1080 b- defN 23-May-31 15:11 rmq_broker/schemas.py
 -rw-r--r--  2.0 unx      508 b- defN 23-May-26 07:16 rmq_broker/settings.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-26 07:16 rmq_broker/async_chains/__init__.py
--rw-r--r--  2.0 unx     7529 b- defN 23-May-26 07:16 rmq_broker/async_chains/base.py
+-rw-r--r--  2.0 unx     8374 b- defN 23-May-31 15:11 rmq_broker/async_chains/base.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-26 07:16 rmq_broker/chains/__init__.py
--rw-r--r--  2.0 unx     7493 b- defN 23-May-26 07:16 rmq_broker/chains/base.py
+-rw-r--r--  2.0 unx     4259 b- defN 23-May-31 15:11 rmq_broker/chains/base.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-26 07:16 rmq_broker/queues/__init__.py
 -rw-r--r--  2.0 unx     1107 b- defN 23-May-26 07:16 rmq_broker/queues/base.py
 -rw-r--r--  2.0 unx     1765 b- defN 23-May-26 07:16 rmq_broker/queues/rabbitmq.py
--rw-r--r--  2.0 unx     1074 b- defN 23-May-29 12:02 rabbitmq_broker-1.0.4.dist-info/LICENSE
--rw-r--r--  2.0 unx     4405 b- defN 23-May-29 12:02 rabbitmq_broker-1.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-29 12:02 rabbitmq_broker-1.0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-May-29 12:02 rabbitmq_broker-1.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1251 b- defN 23-May-29 12:02 rabbitmq_broker-1.0.4.dist-info/RECORD
-15 files, 25877 bytes uncompressed, 8892 bytes compressed:  65.6%
+-rw-r--r--  2.0 unx     1074 b- defN 23-May-31 15:12 rabbitmq_broker-1.1.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4405 b- defN 23-May-31 15:12 rabbitmq_broker-1.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-31 15:12 rabbitmq_broker-1.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-May-31 15:12 rabbitmq_broker-1.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1252 b- defN 23-May-31 15:12 rabbitmq_broker-1.1.0.dist-info/RECORD
+15 files, 23949 bytes uncompressed, 8472 bytes compressed:  64.6%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: rmq_broker/queues/base.py
 Comment: 
 
 Filename: rmq_broker/queues/rabbitmq.py
 Comment: 
 
-Filename: rabbitmq_broker-1.0.4.dist-info/LICENSE
+Filename: rabbitmq_broker-1.1.0.dist-info/LICENSE
 Comment: 
 
-Filename: rabbitmq_broker-1.0.4.dist-info/METADATA
+Filename: rabbitmq_broker-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: rabbitmq_broker-1.0.4.dist-info/WHEEL
+Filename: rabbitmq_broker-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: rabbitmq_broker-1.0.4.dist-info/top_level.txt
+Filename: rabbitmq_broker-1.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: rabbitmq_broker-1.0.4.dist-info/RECORD
+Filename: rabbitmq_broker-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## rmq_broker/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "1.0.1"
+__version__ = "1.1.0"
```

## rmq_broker/schemas.py

```diff
@@ -1,8 +1,37 @@
+from typing import TypedDict
+
 from schema import Optional, Or, Schema
+from typing_extensions import NotRequired
+
+
+class MessageHeader(TypedDict):
+    dst: str
+    src: str
+
+
+class MessageStatus(TypedDict):
+    code: int
+    message: str
+
+
+class BrokerMessage(TypedDict):
+    request_type: str
+    request_id: str
+    header: MessageHeader
+    body: dict
+
+
+class IncomingMessage(BrokerMessage):
+    status: NotRequired[MessageStatus]
+
+
+class OutgoingMessage(BrokerMessage):
+    status: MessageStatus
+
 
 PreMessage = Schema(
     {
         "request_type": str,
         "request_id": str,
         "header": {"src": str, "dst": str},
         "body": object,
```

## rmq_broker/async_chains/base.py

```diff
@@ -1,204 +1,237 @@
 import logging
 from abc import ABC, abstractmethod
-from typing import Any, Callable, Union
 
 from schema import Schema, SchemaError
 from starlette import status
 
-from rmq_broker.schemas import MessageTemplate, PostMessage, PreMessage
+from rmq_broker.schemas import (
+    IncomingMessage,
+    MessageHeader,
+    MessageTemplate,
+    OutgoingMessage,
+    PostMessage,
+    PreMessage,
+)
 
 logger = logging.getLogger(__name__)
 
 
 class AbstractChain(ABC):
     """Интерфейс классов обработчиков.
 
     Args:
         ABC : Вспомогательный класс, предоставляющий стандартный способ
               создания абстрактного класса.
 
-    Attributes:
-        _next_chain: Экземпляр обработчика, являющийся следующим
-                     для данного обработчика.
-        _last_chain: Экземпляр обработчика, являющийся последним в цепочке,
-                     начинающейся с данного обработчика.
+    Arguments:
+        chains (dict): {request_type:объект чейна}
     """
 
-    def __init__(self) -> None:
-        """Создает необходимые атрибуты для объекта цепочки."""
-        logger.debug("%s: initialized" % self.__class__.__name__)
-        self._next_chain: AbstractChain
-        self._last_chain: AbstractChain = self
+    chains: dict = {}
 
-    def add(self, chain) -> None:
+    def add(self, chain: object) -> None:
         """
         Добавляет нового обработчика в цепочку.
         Args:
             chain: Экземпляр обработчика.
 
         Returns:
             None
         """
-        self._last_chain._next_chain = chain
-        self._last_chain = chain
+        self.chains[chain.request_type] = chain
+        logger.debug(
+            f"{self.__class__.__name__}.add(): {chain.__class__.__name__} added to chains."
+        )
 
     @abstractmethod
-    async def handle(
-        self, data: dict[str, Union[str, dict[str, str]]]
-    ) -> Union[Callable, None]:
+    async def handle(self, data: IncomingMessage) -> OutgoingMessage:
         """
         Вызывает метод handle() у следующего обработчика в цепочке.
 
         Args:
             data (dict): Словарь с запросом.
 
         Returns:
             None: если следующий обработчик не определен.
             Обработанный запрос: если следующий обработчик определен.
         """
-        if hasattr(self, "_next_chain"):
-            return await self._next_chain.handle(data)
-        return self.form_response(
-            MessageTemplate,
-            {},
-            status.HTTP_400_BAD_REQUEST,
-            "Can't handle this request type",
-        )
+        ...
 
     @abstractmethod
-    def get_response_header(
-        self, data: dict[str, Union[str, dict[str, str]]]
-    ) -> dict[str, dict[str, str]]:
+    def get_response_header(self, data: IncomingMessage) -> MessageHeader:
         """
         Изменяет заголовок запроса.
 
         Args:
             data (dict): Словарь с запросом.
         """
-        pass  # pragma: no cover
+        ...  # pragma: no cover
 
     @abstractmethod
-    async def get_response_body(
-        self, data: dict[str, Union[str, dict[str, str]]]
-    ) -> dict[str, Union[str, dict[str, str]]]:
+    async def get_response_body(self, data: IncomingMessage) -> OutgoingMessage:
         """
         Изменяет тело запроса.
 
         Args:
             data (dict): Словарь с запросом.
 
         Returns:
             Cловарь c ответом.
         """
-        pass  # pragma: no cover
+        ...  # pragma: no cover
 
     @abstractmethod
-    def validate(self, data: dict[str, Union[str, dict[str, str]]]) -> None:
-        pass  # pragma: no cover
+    def validate(self, data: IncomingMessage) -> None:
+        ...  # pragma: no cover
 
     def form_response(
         self,
-        data: dict,
-        body: Any = {},
+        data: IncomingMessage,
+        body: dict = None,
         code: int = status.HTTP_200_OK,
-        message: Union[int, str] = "",
-    ) -> dict:
+        message: str = "",
+    ) -> OutgoingMessage:
+        body = {} if body is None else body
         data.update({"body": body})
         data.update({"status": {"message": str(message), "code": code}})
+        logger.debug(
+            f"{self.__class__.__name__}.form_response(): Formed response {data=}"
+        )
         return data
 
 
 class BaseChain(AbstractChain):
     """
     Базовый классов обработчиков.
 
     Args:
-        AbstractChain : Интерфейс классов обработчиков.
+        AbstractChain: Интерфейс классов обработчиков.
 
     Attributes:
         request_type (str): Тип запроса, который обработчик способен обработать.
     """
 
     request_type: str = ""
 
-    async def handle(self, data):
+    async def handle(self, data: IncomingMessage) -> OutgoingMessage:
         """
         Обрабатывает запрос, пропуская его через методы обработки
         заголовка и тела запроса.
 
         Args:
             data (dict): Словарь с запросом.
 
         Returns:
             Обработанный запрос: если типы запроса переданного сообщения
             и конкретного экземпляра обработчика совпадают.
 
             Метод handle() у родительского класса: если типы запроса переданного сообщения
             и конкретного экземпляра обработчика отличаются.
         """
+        logger.info(f"{self.__class__.__name__}.get_response_body(): data={data}")
         try:
             self.validate(data, PreMessage)
         except SchemaError as e:
-            logger.error(f"{self.__class__.__name__}: handle(data): Error: {e}")
+            logger.error(f"{self.__class__.__name__}.handle(): SchemaError: {e}")
             return self.form_response(
                 MessageTemplate, {}, status.HTTP_400_BAD_REQUEST, e
             )
-        logger.debug(
-            "%s: handle(data): Successful validation" % self.__class__.__name__
-        )
         response = {}
-        if data["request_type"] == self.request_type:
+        if self.request_type == data["request_type"]:
             response["request_id"] = data["request_id"]
             response["request_type"] = data["request_type"]
-            logger.info("%s: get_response_body(data)" % self.__class__.__name__)
             try:
                 response.update(await self.get_response_body(data))
+                logger.debug(
+                    f"{self.__class__.__name__}.handle(): After body update {response=}"
+                )
             except Exception as e:
                 return self.form_response(
                     MessageTemplate, {}, status.HTTP_400_BAD_REQUEST, e
                 )
-            logger.info(
-                "%s: get_response_header(data) data=%s"
-                % (self.__class__.__name__, data)
-            )
             response.update(self.get_response_header(data))
-            logger.info(f"{self.__class__.__name__}: handle(data) response={response}")
+            logger.debug(
+                f"{self.__class__.__name__}.handle(): After header update {response=}"
+            )
             try:
                 self.validate(response, PostMessage)
                 return response
             except SchemaError as e:
-                logger.error(f"{self.__class__.__name__}: handle(data): Error: {e}")
+                logger.error(f"{self.__class__.__name__}.handle(): SchemaError: {e}")
                 return self.form_response(
                     MessageTemplate, {}, status.HTTP_400_BAD_REQUEST, e
                 )
         else:
-            return await super().handle(data)
+            logger.error(
+                f"{self.__class__.__name__}.handle(): Unknown request_type='{data['request_type']}'"
+            )
+            return self.form_response(
+                MessageTemplate,
+                {},
+                status.HTTP_400_BAD_REQUEST,
+                "Can't handle this request type",
+            )
 
-    def get_response_header(self, data):
+    def get_response_header(self, data: IncomingMessage) -> MessageHeader:
         """
         Меняет местами получателя('dst') и отправителя('src') запроса.
 
         Args:
             data (dict): Словарь с запросом.
 
-        Raises:
-            ShemaError: Любой из ключей ('src', 'dst') отсутствует в словаре запроса.
-
         Returns:
             Словарь заголовка запроса.
         """
-        return {"header": {"src": data["header"]["dst"], "dst": data["header"]["src"]}}
-
-    def validate(
-        self, data: dict[str, Union[str, dict[str, str]]], schema: Schema
-    ) -> None:
+        updated_header = {
+            "header": {"src": data["header"]["dst"], "dst": data["header"]["src"]}
+        }
         logger.debug(
-            "%s.validate(data, schema): Started validation" % self.__class__.__name__
+            f"{self.__class__.__name__}.get_response_header(): {updated_header=}"
         )
-        logger.debug(f"{self.__class__.__name__}.validate(data, schema): data={data}")
+        return updated_header
+
+    def validate(self, message: IncomingMessage, schema: Schema) -> None:
+        """Валидирует сообщение по переданной схеме.
+
+        Raises:
+            SchemaError: Валидация не была пройдена.
+        """
+        schema.validate(message)
         logger.debug(
-            "{}.validate(data, schema): schema{}".format(
-                self.__class__.__name__, schema.__class__.__name__
-            )
+            f"{self.__class__.__name__}.validate(): Successful validation, {message=}"
+        )
+
+
+class ChainManager(BaseChain):
+    """Единая точка для распределения запросов по обработчикам."""
+
+    chains = {}
+
+    def __init__(self, parent_chain: BaseChain = BaseChain) -> None:
+        """Собирает все обработчики в словарь."""
+        if subclasses := parent_chain.__subclasses__():
+            for subclass in subclasses:
+                if subclass.request_type:
+                    self.chains[subclass.request_type] = subclass
+                self.__init__(subclass)
+
+    async def handle(self, data: IncomingMessage) -> OutgoingMessage:
+        """Направляет запрос на нужный обработчик."""
+        try:
+            self.validate(data, PreMessage)
+            chain = self.chains[data["request_type"]]
+            return await chain().handle(data)
+        except SchemaError as e:
+            msg = f"Incoming message validation error: {e}"
+        except KeyError as e:
+            msg = f"Can't handle this request type: {e}"
+        logger.error(f"{self.__class__.__name__}.handle(): {msg}")
+        return self.form_response(
+            MessageTemplate,
+            {},
+            status.HTTP_400_BAD_REQUEST,
+            msg,
         )
-        schema.validate(data)
+
+    async def get_response_body(self, data):
+        pass
```

## rmq_broker/chains/base.py

```diff
@@ -1,204 +1,109 @@
 import logging
-from abc import ABC, abstractmethod
-from typing import Any, Callable, Union
+from abc import abstractmethod
 
-from schema import Schema, SchemaError
+from schema import SchemaError
 from starlette import status
 
-from rmq_broker.schemas import MessageTemplate, PostMessage, PreMessage
+from rmq_broker.async_chains.base import BaseChain as AsyncBaseChain
+from rmq_broker.async_chains.base import ChainManager as AsyncChainManager
+from rmq_broker.schemas import (
+    IncomingMessage,
+    MessageTemplate,
+    OutgoingMessage,
+    PostMessage,
+    PreMessage,
+)
 
 logger = logging.getLogger(__name__)
 
 
-class AbstractChain(ABC):
-    """Интерфейс классов обработчиков.
+class BaseChain(AsyncBaseChain):
+    """Синхронная версия базового класса обработчика."""
 
-    Args:
-        ABC : Вспомогательный класс, предоставляющий стандартный способ
-              создания абстрактного класса.
-
-    Attributes:
-        _next_chain: Экземпляр обработчика, являющийся следующим
-                     для данного обработчика.
-        _last_chain: Экземпляр обработчика, являющийся последним в цепочке,
-                     начинающейся с данного обработчика.
-    """
-
-    def __init__(self) -> None:
-        """Создает необходимые атрибуты для объекта цепочки."""
-        logger.debug("%s: initialized" % self.__class__.__name__)
-        self._next_chain: AbstractChain
-        self._last_chain: AbstractChain = self
-
-    def add(self, chain) -> None:
-        """
-        Добавляет нового обработчика в цепочку.
-        Args:
-            chain: Экземпляр обработчика.
-
-        Returns:
-            None
-        """
-        self._last_chain._next_chain = chain
-        self._last_chain = chain
-
-    @abstractmethod
-    def handle(
-        self, data: dict[str, Union[str, dict[str, str]]]
-    ) -> Union[Callable, None]:
-        """
-        Вызывает метод handle() у следующего обработчика в цепочке.
-
-        Args:
-            data (dict): Словарь с запросом.
-
-        Returns:
-            None: если следующий обработчик не определен.
-            Обработанный запрос: если следующий обработчик определен.
-        """
-        if hasattr(self, "_next_chain"):
-            return self._next_chain.handle(data)
-        return self.form_response(
-            MessageTemplate,
-            {},
-            status.HTTP_400_BAD_REQUEST,
-            "Can't handle this request type",
-        )
-
-    @abstractmethod
-    def get_response_header(
-        self, data: dict[str, Union[str, dict[str, str]]]
-    ) -> dict[str, dict[str, str]]:
-        """
-        Изменяет заголовок запроса.
-
-        Args:
-            data (dict): Словарь с запросом.
-        """
-        pass  # pragma: no cover
-
-    @abstractmethod
-    def get_response_body(
-        self, data: dict[str, Union[str, dict[str, str]]]
-    ) -> dict[str, Union[str, dict[str, str]]]:
-        """
-        Изменяет тело запроса.
-
-        Args:
-            data (dict): Словарь с запросом.
-
-        Returns:
-            Cловарь c ответом.
-        """
-        pass  # pragma: no cover
-
-    @abstractmethod
-    def validate(self, data: dict[str, Union[str, dict[str, str]]]) -> None:
-        pass  # pragma: no cover
-
-    def form_response(
-        self,
-        data: dict,
-        body: Any = {},
-        code: int = status.HTTP_200_OK,
-        message: Union[int, str] = "",
-    ) -> dict:
-        data.update({"body": body})
-        data.update({"status": {"message": str(message), "code": code}})
-        return data
-
-
-class BaseChain(AbstractChain):
-    """
-    Базовый классов обработчиков.
-
-    Args:
-        AbstractChain : Интерфейс классов обработчиков.
-
-    Attributes:
-        request_type (str): Тип запроса, который обработчик способен обработать.
-    """
-
-    request_type: str = ""
-
-    def handle(self, data):
+    def handle(self, data: IncomingMessage) -> OutgoingMessage:
         """
         Обрабатывает запрос, пропуская его через методы обработки
         заголовка и тела запроса.
 
         Args:
             data (dict): Словарь с запросом.
 
         Returns:
             Обработанный запрос: если типы запроса переданного сообщения
             и конкретного экземпляра обработчика совпадают.
 
             Метод handle() у родительского класса: если типы запроса переданного сообщения
             и конкретного экземпляра обработчика отличаются.
         """
+        logger.info(f"{self.__class__.__name__}.get_response_body(): data={data}")
         try:
             self.validate(data, PreMessage)
         except SchemaError as e:
-            logger.error(f"{self.__class__.__name__}: handle(data): Error: {e}")
+            logger.error(f"{self.__class__.__name__}.handle(): SchemaError: {e}")
             return self.form_response(
                 MessageTemplate, {}, status.HTTP_400_BAD_REQUEST, e
             )
-        logger.debug(
-            "%s: handle(data): Successful validation" % self.__class__.__name__
-        )
         response = {}
-        if data["request_type"] == self.request_type:
+        if self.request_type == data["request_type"]:
             response["request_id"] = data["request_id"]
             response["request_type"] = data["request_type"]
-            logger.info("%s: get_response_body(data)" % self.__class__.__name__)
             try:
                 response.update(self.get_response_body(data))
+                logger.debug(
+                    f"{self.__class__.__name__}.handle(): After body update {response=}"
+                )
             except Exception as e:
                 return self.form_response(
                     MessageTemplate, {}, status.HTTP_400_BAD_REQUEST, e
                 )
-            logger.info(
-                "%s: get_response_header(data) data=%s"
-                % (self.__class__.__name__, data)
-            )
             response.update(self.get_response_header(data))
-            logger.info(f"{self.__class__.__name__}: handle(data) response={response}")
+            logger.debug(
+                f"{self.__class__.__name__}.handle(): After header update {response=}"
+            )
             try:
                 self.validate(response, PostMessage)
                 return response
             except SchemaError as e:
-                logger.error(f"{self.__class__.__name__}: handle(data): Error: {e}")
+                logger.error(f"{self.__class__.__name__}.handle(): SchemaError: {e}")
                 return self.form_response(
                     MessageTemplate, {}, status.HTTP_400_BAD_REQUEST, e
                 )
         else:
-            return super().handle(data)
-
-    def get_response_header(self, data):
-        """
-        Меняет местами получателя('dst') и отправителя('src') запроса.
+            logger.error(
+                f"{self.__class__.__name__}.handle(): Unknown request_type='{data['request_type']}'"
+            )
+            return self.form_response(
+                MessageTemplate,
+                {},
+                status.HTTP_400_BAD_REQUEST,
+                "Can't handle this request type",
+            )
 
-        Args:
-            data (dict): Словарь с запросом.
+    @abstractmethod
+    def get_response_body(self, data: IncomingMessage) -> OutgoingMessage:
+        ...
 
-        Raises:
-            ShemaError: Любой из ключей ('src', 'dst') отсутствует в словаре запроса.
 
-        Returns:
-            Словарь заголовка запроса.
-        """
-        return {"header": {"src": data["header"]["dst"], "dst": data["header"]["src"]}}
+class ChainManager(AsyncChainManager):
+    """Синхронная версия менеджера распределения запросов."""
 
-    def validate(
-        self, data: dict[str, Union[str, dict[str, str]]], schema: Schema
-    ) -> None:
-        logger.debug(
-            "%s.validate(data, schema): Started validation" % self.__class__.__name__
-        )
-        logger.debug(f"{self.__class__.__name__}.validate(data, schema): data={data}")
-        logger.debug(
-            "{}.validate(data, schema): schema{}".format(
-                self.__class__.__name__, schema.__class__.__name__
-            )
+    def handle(self, data: IncomingMessage) -> OutgoingMessage:
+        """Направляет запрос на нужный обработчик."""
+        try:
+            self.validate(data, PreMessage)
+            chain = self.chains[data["request_type"]]
+            return chain().handle(data)
+        except SchemaError as e:
+            msg = f"Incoming message validation error: {e}"
+        except KeyError as e:
+            msg = f"Can't handle this request type: {e}"
+        logger.error(f"{self.__class__.__name__}: handle(data): {msg}")
+        return self.form_response(
+            MessageTemplate,
+            {},
+            status.HTTP_400_BAD_REQUEST,
+            msg,
         )
-        schema.validate(data)
+
+    def get_response_body(self, data):
+        pass
```

## Comparing `rabbitmq_broker-1.0.4.dist-info/LICENSE` & `rabbitmq_broker-1.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `rabbitmq_broker-1.0.4.dist-info/METADATA` & `rabbitmq_broker-1.1.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rabbitmq-broker
-Version: 1.0.4
+Version: 1.1.0
 Summary: RPC брокер сообщений
 Author-email: Nikita Sysoev <njt55cs@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

