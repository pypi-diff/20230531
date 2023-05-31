# Comparing `tmp/epcpy-0.1.6.tar.gz` & `tmp/epcpy-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epcpy-0.1.6.tar", max compression
+gzip compressed data, was "epcpy-0.1.7.tar", max compression
```

## Comparing `epcpy-0.1.6.tar` & `epcpy-0.1.7.tar`

### file list

```diff
@@ -1,33 +1,34 @@
--rw-r--r--   0        0        0      447 2022-03-28 13:53:01.220317 epcpy-0.1.6/epcpy/__init__.py
--rw-r--r--   0        0        0      506 2022-03-28 14:49:08.251705 epcpy-0.1.6/epcpy/epc_schemes/__init__.py
--rw-r--r--   0        0        0     6849 2022-03-28 13:53:01.231318 epcpy-0.1.6/epcpy/epc_schemes/adi.py
--rw-r--r--   0        0        0     6977 2022-03-28 13:53:01.235321 epcpy-0.1.6/epcpy/epc_schemes/base_scheme.py
--rw-r--r--   0        0        0     1023 2022-03-28 13:53:01.242323 epcpy-0.1.6/epcpy/epc_schemes/bic.py
--rw-r--r--   0        0        0    10261 2022-03-28 13:53:01.247324 epcpy-0.1.6/epcpy/epc_schemes/cpi.py
--rw-r--r--   0        0        0     8530 2022-03-28 13:53:01.251318 epcpy-0.1.6/epcpy/epc_schemes/gdti.py
--rw-r--r--   0        0        0     9720 2022-03-28 13:53:01.260321 epcpy-0.1.6/epcpy/epc_schemes/giai.py
--rw-r--r--   0        0        0     4686 2022-03-28 13:53:01.264320 epcpy-0.1.6/epcpy/epc_schemes/gid.py
--rw-r--r--   0        0        0     3300 2022-03-28 13:53:01.268318 epcpy-0.1.6/epcpy/epc_schemes/ginc.py
--rw-r--r--   0        0        0     8422 2022-03-28 13:53:01.274333 epcpy-0.1.6/epcpy/epc_schemes/grai.py
--rw-r--r--   0        0        0     3280 2022-03-28 13:53:01.281319 epcpy-0.1.6/epcpy/epc_schemes/gsin.py
--rw-r--r--   0        0        0     6927 2022-03-28 13:53:01.284318 epcpy-0.1.6/epcpy/epc_schemes/gsrn.py
--rw-r--r--   0        0        0     7017 2022-03-28 13:53:01.287364 epcpy-0.1.6/epcpy/epc_schemes/gsrnp.py
--rw-r--r--   0        0        0      788 2022-03-28 13:53:01.294320 epcpy-0.1.6/epcpy/epc_schemes/imovn.py
--rw-r--r--   0        0        0     9096 2022-03-28 13:53:01.297320 epcpy-0.1.6/epcpy/epc_schemes/itip.py
--rw-r--r--   0        0        0     4590 2022-03-28 14:49:08.259806 epcpy-0.1.6/epcpy/epc_schemes/lgtin.py
--rw-r--r--   0        0        0     2749 2022-03-28 13:53:01.301319 epcpy-0.1.6/epcpy/epc_schemes/pgln.py
--rw-r--r--   0        0        0     7474 2022-03-28 13:53:01.303318 epcpy-0.1.6/epcpy/epc_schemes/sgcn.py
--rw-r--r--   0        0        0     8477 2022-03-28 13:53:01.311320 epcpy-0.1.6/epcpy/epc_schemes/sgln.py
--rw-r--r--   0        0        0    10459 2022-03-28 13:53:01.314319 epcpy-0.1.6/epcpy/epc_schemes/sgtin.py
--rw-r--r--   0        0        0     7101 2022-03-28 13:53:01.318319 epcpy-0.1.6/epcpy/epc_schemes/sscc.py
--rw-r--r--   0        0        0     3114 2022-03-28 13:53:01.322336 epcpy-0.1.6/epcpy/epc_schemes/upui.py
--rw-r--r--   0        0        0     4545 2022-03-28 13:53:01.327322 epcpy-0.1.6/epcpy/epc_schemes/usdod.py
--rw-r--r--   0        0        0        0 2022-01-28 08:08:07.899428 epcpy-0.1.6/epcpy/utils/__init__.py
--rw-r--r--   0        0        0    15481 2022-03-28 13:53:01.331319 epcpy-0.1.6/epcpy/utils/common.py
--rw-r--r--   0        0        0    10590 2022-03-28 14:49:08.267806 epcpy-0.1.6/epcpy/utils/parsers.py
--rw-r--r--   0        0        0    10313 2022-03-28 14:49:08.276835 epcpy-0.1.6/epcpy/utils/regex.py
--rw-r--r--   0        0        0     1088 2022-03-10 08:51:16.034331 epcpy-0.1.6/LICENSE
--rw-r--r--   0        0        0     1118 2022-03-28 14:49:08.284807 epcpy-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      752 2022-03-28 13:53:01.218318 epcpy-0.1.6/README_pip.md
--rw-r--r--   0        0        0     1541 2022-03-28 14:49:34.014781 epcpy-0.1.6/setup.py
--rw-r--r--   0        0        0     1649 2022-03-28 14:49:34.014781 epcpy-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      447 2022-03-29 06:16:40.944633 epcpy-0.1.7/epcpy/__init__.py
+-rw-r--r--   0        0        0      506 2022-03-29 06:16:40.946638 epcpy-0.1.7/epcpy/epc_schemes/__init__.py
+-rw-r--r--   0        0        0     6825 2023-05-31 08:01:16.164692 epcpy-0.1.7/epcpy/epc_schemes/adi.py
+-rw-r--r--   0        0        0     7887 2023-05-31 08:01:16.188691 epcpy-0.1.7/epcpy/epc_schemes/base_scheme.py
+-rw-r--r--   0        0        0     1030 2023-05-31 08:01:16.205692 epcpy-0.1.7/epcpy/epc_schemes/bic.py
+-rw-r--r--   0        0        0    10246 2023-05-31 08:01:16.230698 epcpy-0.1.7/epcpy/epc_schemes/cpi.py
+-rw-r--r--   0        0        0     8515 2023-05-31 08:01:16.256692 epcpy-0.1.7/epcpy/epc_schemes/gdti.py
+-rw-r--r--   0        0        0     9705 2023-05-31 08:01:16.282693 epcpy-0.1.7/epcpy/epc_schemes/giai.py
+-rw-r--r--   0        0        0     4649 2023-05-31 08:01:17.303696 epcpy-0.1.7/epcpy/epc_schemes/gid.py
+-rw-r--r--   0        0        0     3307 2023-05-31 08:01:17.330695 epcpy-0.1.7/epcpy/epc_schemes/ginc.py
+-rw-r--r--   0        0        0     8407 2023-05-31 08:01:17.361698 epcpy-0.1.7/epcpy/epc_schemes/grai.py
+-rw-r--r--   0        0        0     3277 2023-05-31 08:01:17.382692 epcpy-0.1.7/epcpy/epc_schemes/gsin.py
+-rw-r--r--   0        0        0     6912 2023-05-31 08:01:17.407696 epcpy-0.1.7/epcpy/epc_schemes/gsrn.py
+-rw-r--r--   0        0        0     7002 2023-05-31 08:01:17.432694 epcpy-0.1.7/epcpy/epc_schemes/gsrnp.py
+-rw-r--r--   0        0        0      795 2023-05-31 08:01:17.453694 epcpy-0.1.7/epcpy/epc_schemes/imovn.py
+-rw-r--r--   0        0        0     9081 2023-05-31 08:01:17.479695 epcpy-0.1.7/epcpy/epc_schemes/itip.py
+-rw-r--r--   0        0        0     4577 2023-05-31 08:01:17.504693 epcpy-0.1.7/epcpy/epc_schemes/lgtin.py
+-rw-r--r--   0        0        0     2736 2023-05-31 08:01:17.522693 epcpy-0.1.7/epcpy/epc_schemes/pgln.py
+-rw-r--r--   0        0        0     7459 2023-05-31 08:01:17.548693 epcpy-0.1.7/epcpy/epc_schemes/sgcn.py
+-rw-r--r--   0        0        0     8462 2023-05-31 08:01:17.572697 epcpy-0.1.7/epcpy/epc_schemes/sgln.py
+-rw-r--r--   0        0        0    10444 2023-05-31 08:01:17.603697 epcpy-0.1.7/epcpy/epc_schemes/sgtin.py
+-rw-r--r--   0        0        0     7088 2023-05-31 08:01:17.629695 epcpy-0.1.7/epcpy/epc_schemes/sscc.py
+-rw-r--r--   0        0        0     3121 2023-05-31 08:01:17.660698 epcpy-0.1.7/epcpy/epc_schemes/upui.py
+-rw-r--r--   0        0        0     4514 2023-05-31 08:01:17.699693 epcpy-0.1.7/epcpy/epc_schemes/usdod.py
+-rw-r--r--   0        0        0        0 2023-05-31 08:01:17.720694 epcpy-0.1.7/epcpy/py.typed
+-rw-r--r--   0        0        0        0 2022-01-28 08:08:07.899428 epcpy-0.1.7/epcpy/utils/__init__.py
+-rw-r--r--   0        0        0    15500 2023-05-31 08:01:17.764701 epcpy-0.1.7/epcpy/utils/common.py
+-rw-r--r--   0        0        0    10646 2023-05-31 08:01:17.811694 epcpy-0.1.7/epcpy/utils/parsers.py
+-rw-r--r--   0        0        0    10313 2022-03-29 06:16:41.070981 epcpy-0.1.7/epcpy/utils/regex.py
+-rw-r--r--   0        0        0     1088 2022-03-10 08:51:16.034331 epcpy-0.1.7/LICENSE
+-rw-r--r--   0        0        0     1136 2023-05-31 08:01:17.881694 epcpy-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      752 2022-03-29 06:16:40.941624 epcpy-0.1.7/README_pip.md
+-rw-r--r--   0        0        0     1541 2023-05-31 08:01:55.834482 epcpy-0.1.7/setup.py
+-rw-r--r--   0        0        0     1650 2023-05-31 08:01:55.835484 epcpy-0.1.7/PKG-INFO
```

### Comparing `epcpy-0.1.6/epcpy/epc_schemes/adi.py` & `epcpy-0.1.7/epcpy/epc_schemes/adi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from __future__ import annotations
 
-import math
 import re
 from enum import Enum
 
-from epcpy.epc_schemes.base_scheme import EPCScheme, TagEncodable
+from epcpy.epc_schemes.base_scheme import TagEncodable
 from epcpy.utils.common import (
     ConvertException,
     binary_to_int,
     decode_cage_code_six_bits,
     decode_string_six_bits,
     encode_cage_code_six_bits,
     encode_string_six_bits,
@@ -83,15 +82,15 @@
     GROUND_SUPPORT_EQUIPMENT = "59"
     OTHER_NON_FLYABLE_EQUIPMENT = "60"
     RESERVED_61 = "61"
     RESERVED_62 = "62"
     RESERVED_63 = "63"
 
 
-class ADI(EPCScheme, TagEncodable):
+class ADI(TagEncodable):
     """ADI EPC scheme implementation.
 
     ADI pure identities are of the form:
         urn:epc:id:adi:<CAGEOrDODAAC>.<OriginalPartNumber>.<Serial>
 
     Example:
         urn:epc:id:adi:W81X9C.3KL984PX1.2WMA52
@@ -110,15 +109,15 @@
     class BinaryCodingScheme(Enum):
         ADI_VAR = "adi-var"
 
     class BinaryHeader(Enum):
         ADI_VAR = "00111011"
 
     def __init__(self, epc_uri) -> None:
-        super().__init__()
+        super().__init__(epc_uri)
 
         if not ADI_URI_REGEX.fullmatch(epc_uri):
             raise ConvertException(message=f"Invalid ADI URI {epc_uri}")
 
         self._cage_dodaac, self._part_number, self._serial = epc_uri.split(":")[
             4
         ].split(".")
@@ -205,18 +204,18 @@
             raise ConvertException(
                 message="Invalid binary for ADI, missing 6-bit terminators"
             )
 
         part_number_binary, _, *serial_binary = re.split(
             "([0]{6})", truncated_binary[50:]
         )
-        serial_binary = "".join(serial_binary)[:-6]
+        serial_binary_trimmed = "".join(serial_binary)[:-6]
 
         filter_string = binary_to_int(filter_binary)
         cage_code_string = decode_cage_code_six_bits(cage_code_binary)
-        part_number_string = decode_string_six_bits(part_number_binary, math.inf)
+        part_number_string = decode_string_six_bits(part_number_binary, 32)
 
-        serial_string = decode_string_six_bits(serial_binary, math.inf)
+        serial_string = decode_string_six_bits(serial_binary_trimmed, 30)
 
         return cls.from_tag_uri(
             f"{cls.TAG_URI_PREFIX}{binary_coding_scheme.value}:{filter_string}.{cage_code_string}.{part_number_string}.{serial_string}"
         )
```

### Comparing `epcpy-0.1.6/epcpy/epc_schemes/base_scheme.py` & `epcpy-0.1.7/epcpy/epc_schemes/base_scheme.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 from __future__ import annotations
 
 import re
-from typing import Any, Dict
+from enum import Enum
+from typing import Dict, Optional, Type, TypeVar
 
 from epcpy.utils.common import ConvertException, hex_to_base64, hex_to_binary
 from epcpy.utils.regex import TAG_URI
 
+T_EPCScheme = TypeVar("T_EPCScheme", bound="EPCScheme")
+T_GS1Element = TypeVar("T_GS1Element", bound="GS1Element")
+T_TagEncodable = TypeVar("T_TagEncodable", bound="TagEncodable")
+
 
 class EPCScheme:
     """Base class for EPC schemes
 
     Attributes:
         epc_uri (str): The EPC pure identity URI
     """
 
-    def __init__(self) -> None:
+    def __init__(self, epc_uri: str) -> None:
         super().__init__()
-        self.epc_uri = None
+        self.epc_uri = epc_uri
 
     def __eq__(self, other: object) -> bool:
         """Verify equality of two classes by validing if its an EPCScheme and whether the EPC URIs are equal.
 
         Args:
             other (object): Other object to compare against
 
@@ -29,130 +34,146 @@
         """
         if not isinstance(other, EPCScheme):
             return False
 
         return self.epc_uri == other.epc_uri
 
     @classmethod
-    def from_epc_uri(cls, epc_uri: str) -> EPCScheme:
+    def from_epc_uri(cls: Type[T_EPCScheme], epc_uri: str) -> EPCScheme:
         """Instantiate an EPCScheme class from an EPC pure identity URI.
 
         Args:
             epc_uri (str): EPC pure identity URI.
 
         Returns:
             EPCScheme: Instance of EPCScheme class
         """
         return cls(epc_uri)
 
 
-class TagEncodable:
+class TagEncodable(EPCScheme):
     """Base class for tag encodable EPCSchemes
 
     Attributes:
         tag_uri (str): The EPC tag URI
         binary (str): Binary representation of the EPC tag URI
         hex (str): Hexadecimal representation of the EPC tag URI
         base64 (str): Base64 representation of the EPC tag URI
     """
 
+    class BinaryCodingScheme(Enum):
+        """Binary coding schemes for tag encodable EPC schemes"""
+
+        pass
+
+    class BinaryHeader(Enum):
+        """Binary headers for tag encodable EPC schemes"""
+
+        pass
+
     TAG_URI_REGEX = re.compile(TAG_URI)
     TAG_URI_PREFIX = "urn:epc:tag:"
 
-    def __init__(self) -> None:
-        super().__init__()
-        self._base64 = None
-        self._binary = None
-        self._hex = None
-        self._tag_uri = None
+    def __init__(self, epc_uri: str) -> None:
+        super().__init__(epc_uri)
 
-    def tag_uri(self, **kwargs) -> str:
+        self._base64: Optional[str] = None
+        self._binary: Optional[str] = None
+        self._hex: Optional[str] = None
+        self._tag_uri: Optional[str] = None
+
+    def tag_uri(self, *args, **kwargs) -> str:
         """Return the tag URI of the tag encodable
 
         Raises:
             NotImplementedError: Method not implemented by default.
 
         Returns:
             str: The tag URI.
         """
         raise NotImplementedError
 
-    def binary(self, **kwargs) -> str:
+    def binary(self, *args, **kwargs) -> str:
         """Return the binary representation of the tag encodable
 
         Raises:
             NotImplementedError: Method not implemented by default.
 
         Returns:
             str: The binary representation.
         """
         raise NotImplementedError
 
-    def hex(self, **kwargs) -> str:
+    def hex(self, *args, **kwargs) -> str:
         """Return the hexadecimal representation of the tag encodable
 
         Returns:
             str: The hexadecimal representation.
         """
         binary = self.binary(**kwargs)
 
         padding = (16 - (len(binary) % 16)) % 16
         padded_binary = f"{binary:<0{len(binary) + padding}}"
 
         return f"{int(padded_binary, 2):X}"
 
-    def base64(self, **kwargs) -> str:
+    def base64(self, *args, **kwargs) -> str:
         """Return the base64 representation of the tag encodable
 
         Returns:
             str: The base64 representation.
         """
         hex_string = self.hex(**kwargs)
 
         return hex_to_base64(hex_string)
 
-    def from_binary(tag_binary_string: str) -> TagEncodable:
+    @classmethod
+    def from_binary(
+        cls: Type[T_TagEncodable], tag_binary_string: str
+    ) -> T_TagEncodable:
         """Instantiate a TagEncodable class from a binary string.
 
         Args:
             tag_binary_string (str): Binary representation of a tag URI.
 
         Returns:
             TagEncodable: Instance of TagEncodable class
         """
         raise NotImplementedError
 
     @classmethod
-    def from_hex(cls, tag_hex_string: str) -> TagEncodable:
+    def from_hex(cls: Type[T_TagEncodable], tag_hex_string: str) -> T_TagEncodable:
         """Instantiate a TagEncodable class from a hexidecimal string.
 
         Args:
             tag_hex_string (str): Hexidecimal representation of a tag URI.
 
         Returns:
             TagEncodable: Instance of TagEncodable class
         """
         return cls.from_binary(hex_to_binary(tag_hex_string))
 
     @classmethod
-    def from_base64(cls, tag_base64_string: str) -> TagEncodable:
+    def from_base64(
+        cls: Type[T_TagEncodable], tag_base64_string: str
+    ) -> T_TagEncodable:
         """Instantiate a TagEncodable class from a base64 string.
 
         Args:
             tag_base64_string (str): Base64 representation of a tag URI.
 
         Returns:
             TagEncodable: Instance of TagEncodable class
         """
         return cls.from_binary(hex_to_base64(tag_base64_string))
 
     @classmethod
     def from_tag_uri(
-        cls, epc_tag_uri: str, includes_filter: bool = True
-    ) -> TagEncodable:
+        cls: Type[T_TagEncodable], epc_tag_uri: str, includes_filter: bool = True
+    ) -> T_TagEncodable:
         """Instantiate a TagEncodable class from a tag URI.
 
         Args:
             epc_tag_uri (str): Tag URI.
             includes_filter (bool, optional): Whether a filter value is included in the tag URI.
                 Defaults to True.
 
@@ -171,45 +192,47 @@
             value = ".".join(":".join(epc_tag_uri.split(":")[3:]).split(".")[1:])
         else:
             value = epc_tag_uri.split(":")[4]
 
         return cls(f"urn:epc:id:{epc_scheme.split('-')[0]}:{value}")
 
     @classmethod
-    def header_to_schemes(cls) -> Dict[str, Any]:
+    def header_to_schemes(cls: Type[T_TagEncodable]) -> Dict[str, Enum]:
         """Create dictionary of binary header -> binary coding scheme
 
         Returns:
             Dict[str, Any]: Dictionary mapping of binary header -> binary coding scheme
         """
         return {
             binary_header.value: cls.BinaryCodingScheme[binary_header.name]
             for binary_header in cls.BinaryHeader
         }
 
 
-class GS1Element:
-    def __init__(self) -> None:
-        super().__init__()
+class GS1Element(EPCScheme):
+    gs1_element_string_regex: re.Pattern
+
+    def __init__(self, epc_uri: str) -> None:
+        super().__init__(epc_uri)
 
     def gs1_element_string(self, *args, **kwargs) -> str:
         """GS1 element string of the given EPC scheme
 
         Raises:
             NotImplementedError: not implemented by default
 
         Returns:
             str: GS1 element string
         """
         raise NotImplementedError
 
     @classmethod
     def from_gs1_element_string(
-        cls, gs1_element_string: str, company_prefix_length: int
-    ) -> GS1Element:
+        cls: Type[T_GS1Element], gs1_element_string: str, company_prefix_length: int
+    ) -> T_GS1Element:
         """Create a GS1Element instance from a GS1 element string and company prefix length.
 
         Args:
             gs1_element_string (str): GS1 element string
             company_prefix_length (int): Company prefix length
 
         Raises:
@@ -218,16 +241,16 @@
         Returns:
             GS1Element: GS1Element instance
         """
         raise NotImplementedError
 
 
 class GS1Keyed(GS1Element):
-    def __init__(self) -> None:
-        super().__init__()
+    def __init__(self, epc_uri: str) -> None:
+        super().__init__(epc_uri)
 
     def gs1_key(self, *args, **kwargs) -> str:
         """GS1 key of the given EPC scheme
 
         Raises:
             NotImplementedError: not implemented by default
```

### Comparing `epcpy-0.1.6/epcpy/epc_schemes/bic.py` & `epcpy-0.1.7/epcpy/epc_schemes/bic.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     Example:
         urn:epc:id:bic:CSQU3054383
 
     This class can be created using EPC pure identities via its constructor
     """
 
     def __init__(self, epc_uri) -> None:
-        super().__init__()
+        super().__init__(epc_uri)
 
         if not BIC_URI_REGEX.fullmatch(epc_uri):
             raise ConvertException(message=f"Invalid BIC URI {epc_uri}")
 
         self.epc_uri = epc_uri
 
         container_code = epc_uri.split(":")[4]
```

### Comparing `epcpy-0.1.6/epcpy/epc_schemes/cpi.py` & `epcpy-0.1.7/epcpy/epc_schemes/cpi.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import re
 from enum import Enum
 
-from epcpy.epc_schemes.base_scheme import EPCScheme, GS1Element, TagEncodable
+from epcpy.epc_schemes.base_scheme import GS1Element, TagEncodable
 from epcpy.utils.common import (
     ConvertException,
     binary_to_int,
     decode_partition_table,
     encode_partition_table,
     parse_header_and_truncate_binary,
     str_to_binary,
@@ -164,15 +164,15 @@
     return cpi.replace("%23", "#").replace("%2F", "/")
 
 
 def revert_cpi_escapes(cpi: str) -> str:
     return cpi.replace("#", "%23").replace("/", "%2F")
 
 
-class CPI(EPCScheme, GS1Element, TagEncodable):
+class CPI(GS1Element, TagEncodable):
     """CPI EPC scheme implementation.
 
     CPI pure identities are of the form:
         urn:epc:id:cpi:<CompanyPrefix>.<ComponentPartReference>.<Serial>
 
     Example:
         urn:epc:id:cpi:0614141.123ABC.123456789
@@ -197,15 +197,15 @@
     class BinaryHeader(Enum):
         CPI_96 = "00111100"
         CPI_VAR = "00111101"
 
     gs1_element_string_regex = re.compile(CPI_GS1_ELEMENT_STRING)
 
     def __init__(self, epc_uri) -> None:
-        super().__init__()
+        super().__init__(epc_uri)
 
         if not CPI_URI_REGEX.fullmatch(epc_uri):
             raise ConvertException(message=f"Invalid CPI URI {epc_uri}")
 
         self._company_pref, self._cp_ref, self._serial = epc_uri.split(":")[4].split(
             "."
         )
```

### Comparing `epcpy-0.1.6/epcpy/epc_schemes/gdti.py` & `epcpy-0.1.7/epcpy/epc_schemes/gdti.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import re
 from enum import Enum
 
-from epcpy.epc_schemes.base_scheme import EPCScheme, GS1Keyed, TagEncodable
+from epcpy.epc_schemes.base_scheme import GS1Keyed, TagEncodable
 from epcpy.utils.common import (
     ConvertException,
     binary_to_int,
     calculate_checksum,
     decode_partition_table,
     decode_string,
     encode_partition_table,
@@ -92,15 +92,15 @@
     RESERVED_3 = "3"
     RESERVED_4 = "4"
     RESERVED_5 = "5"
     RESERVED_6 = "6"
     RESERVED_7 = "7"
 
 
-class GDTI(EPCScheme, TagEncodable, GS1Keyed):
+class GDTI(TagEncodable, GS1Keyed):
     """GDTI EPC scheme implementation.
 
     GDTI pure identities are of the form:
         urn:epc:id:gdti:<CompanyPrefix>.<DocumentType>.<SerialNumber>
 
     Example:
         urn:epc:id:gdti:0614141.12345.400
@@ -126,15 +126,15 @@
     class BinaryHeader(Enum):
         GDTI_96 = "00101100"
         GDTI_174 = "00111110"
 
     gs1_element_string_regex = re.compile(GDTI_GS1_ELEMENT_STRING)
 
     def __init__(self, epc_uri) -> None:
-        super().__init__()
+        super().__init__(epc_uri)
 
         if not GDTI_URI_REGEX.fullmatch(epc_uri):
             raise ConvertException(message=f"Invalid GDTI URI {epc_uri}")
 
         self._serial = ".".join(":".join(epc_uri.split(":")[4:]).split(".")[2:])
         verify_gs3a3_component(self._serial)
```

### Comparing `epcpy-0.1.6/epcpy/epc_schemes/giai.py` & `epcpy-0.1.7/epcpy/epc_schemes/giai.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import re
 from enum import Enum
 
-from epcpy.epc_schemes.base_scheme import EPCScheme, GS1Keyed, TagEncodable
+from epcpy.epc_schemes.base_scheme import GS1Keyed, TagEncodable
 from epcpy.utils.common import (
     ConvertException,
     binary_to_int,
     decode_partition_table,
     encode_partition_table,
     parse_header_and_truncate_binary,
     replace_uri_escapes,
@@ -151,15 +151,15 @@
     RESERVED_3 = "3"
     RESERVED_4 = "4"
     RESERVED_5 = "5"
     RESERVED_6 = "6"
     RESERVED_7 = "7"
 
 
-class GIAI(EPCScheme, TagEncodable, GS1Keyed):
+class GIAI(TagEncodable, GS1Keyed):
     """GIAI EPC scheme implementation.
 
     GIAI pure identities are of the form:
         urn:epc:id:giai:<CompanyPrefix>.<IndividulAssetReference>
 
     Example:
         urn:epc:id:giai:0614141.12345400
@@ -185,15 +185,15 @@
     class BinaryHeader(Enum):
         GIAI_96 = "00110100"
         GIAI_202 = "00111000"
 
     gs1_element_string_regex = re.compile(GIAI_GS1_ELEMENT_STRING)
 
     def __init__(self, epc_uri) -> None:
-        super().__init__()
+        super().__init__(epc_uri)
 
         if not GIAI_URI_REGEX.fullmatch(epc_uri):
             raise ConvertException(message=f"Invalid GIAI URI {epc_uri}")
 
         company_prefix, *asset_reference = epc_uri.split(":")[4].split(".")
         asset_reference = ".".join(asset_reference)
```

### Comparing `epcpy-0.1.6/epcpy/epc_schemes/gid.py` & `epcpy-0.1.7/epcpy/epc_schemes/gid.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from __future__ import annotations
 
 import re
 from enum import Enum
 
-from epcpy.epc_schemes.base_scheme import EPCScheme, TagEncodable
+from epcpy.epc_schemes.base_scheme import TagEncodable
 from epcpy.utils.common import (
     ConvertException,
     binary_to_int,
     parse_header_and_truncate_binary,
     str_to_binary,
 )
 from epcpy.utils.regex import GID_URI
 
 GID_URI_REGEX = re.compile(GID_URI)
 
 
-class GID(EPCScheme, TagEncodable):
+class GID(TagEncodable):
     """GID EPC scheme implementation.
 
     GID pure identities are of the form:
         urn:epc:id:gid:<ManagerNumber>.<ObjectClass>.<SerialNumber>
 
     Example:
         urn:epc:id:gid:95100000.12345.400
@@ -38,15 +38,15 @@
     class BinaryCodingScheme(Enum):
         GID_96 = "gid-96"
 
     class BinaryHeader(Enum):
         GID_96 = "00110101"
 
     def __init__(self, epc_uri) -> None:
-        super().__init__()
+        super().__init__(epc_uri)
 
         if not GID_URI_REGEX.fullmatch(epc_uri):
             raise ConvertException(message=f"Invalid GID URI {epc_uri}")
 
         self._manager, self._object, self._serial = epc_uri.split(":")[4].split(".")
 
         if int(self._manager) >= pow(2, 28):
@@ -60,30 +60,30 @@
         ):
             raise ConvertException(message=f"Serial out of range: (max: {pow(2, 36)})")
 
         self.epc_uri = epc_uri
 
     def tag_uri(
         self,
-        binary_coding_scheme: GID.BinaryCodingScheme.GID_96 = BinaryCodingScheme.GID_96,
+        binary_coding_scheme: BinaryCodingScheme = BinaryCodingScheme.GID_96,
     ) -> str:
         """Return the tag URI belonging to this GID with the provided binary coding scheme and filter value.
 
         Args:
             binary_coding_scheme (BinaryCodingScheme): Coding scheme
             filter_value (GIDFilterValue): Filter value
 
         Returns:
             str: Tag URI
         """
         return f"{self.TAG_URI_PREFIX}{binary_coding_scheme.value}:{self._manager}.{self._object}.{self._serial}"
 
     def binary(
         self,
-        binary_coding_scheme: GID.BinaryCodingScheme.GID_96 = BinaryCodingScheme.GID_96,
+        binary_coding_scheme: BinaryCodingScheme = BinaryCodingScheme.GID_96,
     ) -> str:
         """Return the binary representation belonging to this GID with the provided binary coding scheme and filter value.
 
         Args:
             binary_coding_scheme (BinaryCodingScheme): Coding scheme
             filter_value (GIDFilterValue): Filter value
```

### Comparing `epcpy-0.1.6/epcpy/epc_schemes/ginc.py` & `epcpy-0.1.7/epcpy/epc_schemes/ginc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from __future__ import annotations
 
 import re
 
-from epcpy.epc_schemes.base_scheme import EPCScheme, GS1Keyed
+from epcpy.epc_schemes.base_scheme import GS1Keyed
 from epcpy.utils.common import (
     ConvertException,
     replace_uri_escapes,
     revert_uri_escapes,
     verify_gs3a3_component,
 )
 from epcpy.utils.regex import GINC_GS1_ELEMENT_STRING, GINC_URI
 
 GINC_URI_REGEX = re.compile(GINC_URI)
 
 
-class GINC(EPCScheme, GS1Keyed):
+class GINC(GS1Keyed):
     """GINC EPC scheme implementation.
 
     GINC pure identities are of the form:
         urn:epc:id:ginc:<CompanyPrefix>.<ConsignmentReference>
 
     Example:
         urn:epc:id:ginc:0614141.xyz3311cba
@@ -30,24 +30,24 @@
         gs1_key (str): GS1 key
         gs1_element_string (str): GS1 element string
     """
 
     gs1_element_string_regex = re.compile(GINC_GS1_ELEMENT_STRING)
 
     def __init__(self, epc_uri) -> None:
-        super().__init__()
+        super().__init__(epc_uri)
 
         if not GINC_URI_REGEX.fullmatch(epc_uri):
             raise ConvertException(message=f"Invalid GINC URI {epc_uri}")
 
-        company_prefix, *consignment_reference = ":".join(epc_uri.split(":")[4:]).split(
-            "."
-        )
+        company_prefix, *consignment_reference_components = ":".join(
+            epc_uri.split(":")[4:]
+        ).split(".")
 
-        consignment_reference = ".".join(consignment_reference)
+        consignment_reference = ".".join(consignment_reference_components)
         verify_gs3a3_component(consignment_reference)
         consignment_reference = replace_uri_escapes(consignment_reference)
 
         if not (6 <= len(company_prefix) <= 12):
             raise ConvertException(
                 message=f"Invalid company prefix length {len(company_prefix)}"
             )
```

### Comparing `epcpy-0.1.6/epcpy/epc_schemes/grai.py` & `epcpy-0.1.7/epcpy/epc_schemes/grai.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import re
 from enum import Enum
 
-from epcpy.epc_schemes.base_scheme import EPCScheme, GS1Keyed, TagEncodable
+from epcpy.epc_schemes.base_scheme import GS1Keyed, TagEncodable
 from epcpy.utils.common import (
     ConvertException,
     binary_to_int,
     calculate_checksum,
     decode_partition_table,
     decode_string,
     encode_partition_table,
@@ -92,15 +92,15 @@
     RESERVED_3 = "3"
     RESERVED_4 = "4"
     RESERVED_5 = "5"
     RESERVED_6 = "6"
     RESERVED_7 = "7"
 
 
-class GRAI(EPCScheme, TagEncodable, GS1Keyed):
+class GRAI(TagEncodable, GS1Keyed):
     """GRAI EPC scheme implementation.
 
     GRAI pure identities are of the form:
         urn:epc:id:grai:<CompanyPrefix>.<AssetType>.<SerialNumber>
 
     Example:
         urn:epc:id:grai:0614141.12345.400
@@ -126,15 +126,15 @@
     class BinaryHeader(Enum):
         GRAI_96 = "00110011"
         GRAI_170 = "00110111"
 
     gs1_element_string_regex = re.compile(GRAI_GS1_ELEMENT_STRING)
 
     def __init__(self, epc_uri) -> None:
-        super().__init__()
+        super().__init__(epc_uri)
 
         if not GRAI_URI_REGEX.fullmatch(epc_uri):
             raise ConvertException(message=f"Invalid GRAI URI {epc_uri}")
 
         self._serial = ".".join(":".join(epc_uri.split(":")[4:]).split(".")[2:])
         verify_gs3a3_component(self._serial)
```

### Comparing `epcpy-0.1.6/epcpy/epc_schemes/gsin.py` & `epcpy-0.1.7/epcpy/epc_schemes/gsin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import re
 
-from epcpy.epc_schemes.base_scheme import EPCScheme, GS1Keyed
+from epcpy.epc_schemes.base_scheme import GS1Keyed
 from epcpy.utils.common import ConvertException
 from epcpy.utils.regex import GSIN_GS1_ELEMENT_STRING, GSIN_URI
 
 GSIN_URI_REGEX = re.compile(GSIN_URI)
 
 
 def calculate_checksum(digits: str) -> int:
@@ -14,26 +14,26 @@
 
     Args:
         digits (str): String of digits
 
     Returns:
         int: Check digit
     """
-    digits = [int(d) for d in digits]
-    odd, even = digits[1::2], digits[0::2]
+    digit_list = [int(d) for d in digits]
+    odd, even = digit_list[1::2], digit_list[0::2]
 
     val1 = sum(odd)
     val2 = sum(even)
 
     checksum = (10 - ((3 * (val1) + (val2)) % 10)) % 10
 
     return checksum
 
 
-class GSIN(EPCScheme, GS1Keyed):
+class GSIN(GS1Keyed):
     """GSIN EPC scheme implementation.
 
     GSIN pure identities are of the form:
         urn:epc:id:gsin:<CompanyPrefix>.<ShipperReference>
 
     Example:
         urn:epc:id:gsin:0614141.123456789
@@ -45,15 +45,15 @@
         gs1_key (str): GS1 key
         gs1_element_string (str): GS1 element string
     """
 
     gs1_element_string_regex = re.compile(GSIN_GS1_ELEMENT_STRING)
 
     def __init__(self, epc_uri) -> None:
-        super().__init__()
+        super().__init__(epc_uri)
 
         if not GSIN_URI_REGEX.fullmatch(epc_uri):
             raise ConvertException(message=f"Invalid GSIN URI {epc_uri}")
 
         self._company_prefix, self._shipper_ref = epc_uri.split(":")[4].split(".")
 
         if len(f"{self._company_prefix}{self._shipper_ref}") != 16 or not (
```

### Comparing `epcpy-0.1.6/epcpy/epc_schemes/gsrn.py` & `epcpy-0.1.7/epcpy/epc_schemes/gsrn.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import re
 from enum import Enum
 
-from epcpy.epc_schemes.base_scheme import EPCScheme, GS1Keyed, TagEncodable
+from epcpy.epc_schemes.base_scheme import GS1Keyed, TagEncodable
 from epcpy.utils.common import (
     ConvertException,
     binary_to_int,
     calculate_checksum,
     decode_partition_table,
     encode_partition_table,
     parse_header_and_truncate_binary,
@@ -88,15 +88,15 @@
     RESERVED_3 = "3"
     RESERVED_4 = "4"
     RESERVED_5 = "5"
     RESERVED_6 = "6"
     RESERVED_7 = "7"
 
 
-class GSRN(EPCScheme, TagEncodable, GS1Keyed):
+class GSRN(TagEncodable, GS1Keyed):
     """GSRN EPC scheme implementation.
 
     GSRN pure identities are of the form:
         urn:epc:id:gsrn:<CompanyPrefix>.<ServiceReference>
 
     Example:
         urn:epc:id:gsrn:0614141.1234567890
@@ -120,15 +120,15 @@
 
     class BinaryHeader(Enum):
         GSRN_96 = "00101101"
 
     gs1_element_string_regex = re.compile(GSRN_GS1_ELEMENT_STRING)
 
     def __init__(self, epc_uri) -> None:
-        super().__init__()
+        super().__init__(epc_uri)
 
         if not GSRN_URI_REGEX.fullmatch(epc_uri):
             raise ConvertException(message=f"Invalid GSRN URI {epc_uri}")
 
         self._company_pref, self._service_ref = epc_uri.split(":")[4].split(".")
 
         if len(f"{self._company_pref}{self._service_ref}") != 17 or not (
```

### Comparing `epcpy-0.1.6/epcpy/epc_schemes/gsrnp.py` & `epcpy-0.1.7/epcpy/epc_schemes/gsrnp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import re
 from enum import Enum
 
-from epcpy.epc_schemes.base_scheme import EPCScheme, GS1Keyed, TagEncodable
+from epcpy.epc_schemes.base_scheme import GS1Keyed, TagEncodable
 from epcpy.utils.common import (
     ConvertException,
     binary_to_int,
     calculate_checksum,
     decode_partition_table,
     encode_partition_table,
     parse_header_and_truncate_binary,
@@ -88,15 +88,15 @@
     RESERVED_3 = "3"
     RESERVED_4 = "4"
     RESERVED_5 = "5"
     RESERVED_6 = "6"
     RESERVED_7 = "7"
 
 
-class GSRNP(EPCScheme, TagEncodable, GS1Keyed):
+class GSRNP(TagEncodable, GS1Keyed):
     """GSRNP EPC scheme implementation.
 
     GSRNP pure identities are of the form:
         urn:epc:id:gsrnp:<CompanyPrefix>.<ServiceReference>
 
     Example:
         urn:epc:id:gsrnp:0614141.1234567890
@@ -120,15 +120,15 @@
 
     class BinaryHeader(Enum):
         GSRNP_96 = "00101110"
 
     gs1_element_string_regex = re.compile(GSRNP_GS1_ELEMENT_STRING)
 
     def __init__(self, epc_uri) -> None:
-        super().__init__()
+        super().__init__(epc_uri)
 
         if not GSRNP_URI_REGEX.fullmatch(epc_uri):
             raise ConvertException(message=f"Invalid GSRNP URI {epc_uri}")
 
         self._company_pref, self._service_ref = epc_uri.split(":")[4].split(".")
 
         if len(f"{self._company_pref}{self._service_ref}") != 17 or not (
```

### Comparing `epcpy-0.1.6/epcpy/epc_schemes/imovn.py` & `epcpy-0.1.7/epcpy/epc_schemes/imovn.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     Example:
         urn:epc:id:imovn:9176187
 
     This class can be created using EPC pure identities via its constructor
     """
 
     def __init__(self, epc_uri) -> None:
-        super().__init__()
+        super().__init__(epc_uri)
 
         if not IMOVN_URI_REGEX.fullmatch(epc_uri):
             raise ConvertException(message=f"Invalid IMOVN URI {epc_uri}")
 
         self.epc_uri = epc_uri
 
         self._vessel_number = epc_uri.split(":")[4]
```

### Comparing `epcpy-0.1.6/epcpy/epc_schemes/itip.py` & `epcpy-0.1.7/epcpy/epc_schemes/itip.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import re
 from enum import Enum
 
-from epcpy.epc_schemes.base_scheme import EPCScheme, GS1Element, TagEncodable
+from epcpy.epc_schemes.base_scheme import GS1Element, TagEncodable
 from epcpy.utils.common import (
     ConvertException,
     binary_to_int,
     calculate_checksum,
     decode_fixed_width_integer,
     decode_partition_table,
     decode_string,
@@ -94,15 +94,15 @@
     RESERVED_3 = "3"
     RESERVED_4 = "4"
     RESERVED_5 = "5"
     RESERVED_6 = "6"
     RESERVED_7 = "7"
 
 
-class ITIP(EPCScheme, GS1Element, TagEncodable):
+class ITIP(GS1Element, TagEncodable):
     """ITIP EPC scheme implementation.
 
     ITIP pure identities are of the form:
         urn:epc:id:itip:<CompanyPrefix>.<ItemRefAndIndicator>.<Piece>.<Total>.<SerialNumber>
 
     Example:
         urn:epc:id:itip:4012345.012345.01.02.987
@@ -127,15 +127,15 @@
     class BinaryHeader(Enum):
         ITIP_110 = "01000000"
         ITIP_212 = "01000001"
 
     gs1_element_string_regex = re.compile(ITIP_GS1_ELEMENT_STRING)
 
     def __init__(self, epc_uri) -> None:
-        super().__init__()
+        super().__init__(epc_uri)
 
         if not ITIP_URI_REGEX.fullmatch(epc_uri):
             raise ConvertException(message=f"Invalid ITIP URI {epc_uri}")
 
         (
             self._company_pref,
             self._item_ref,
```

### Comparing `epcpy-0.1.6/epcpy/epc_schemes/lgtin.py` & `epcpy-0.1.7/epcpy/epc_schemes/lgtin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import re
 from enum import IntEnum
 
-from epcpy.epc_schemes.base_scheme import EPCScheme, GS1Keyed
+from epcpy.epc_schemes.base_scheme import GS1Keyed
 from epcpy.utils.common import (
     ConvertException,
     calculate_checksum,
     replace_uri_escapes,
     revert_uri_escapes,
     verify_gs3a3_component,
 )
@@ -19,15 +19,15 @@
 class GTIN_TYPE(IntEnum):
     GTIN8 = (8,)
     GTIN12 = (12,)
     GTIN13 = (13,)
     GTIN14 = 14
 
 
-class LGTIN(EPCScheme, GS1Keyed):
+class LGTIN(GS1Keyed):
     """LGTIN EPC scheme implementation.
 
     LGTIN pure identities are of the form:
         urn:epc:class:lgtin:<CompanyPrefix>.<ItemRefAndIndicator>.<Lot>
 
     Example:
         urn:epc:class:lgtin:061414.0123456.xyz3311cba
@@ -39,15 +39,15 @@
         gs1_key (str): GS1 key
         gs1_element_string (str): GS1 element string
     """
 
     gs1_element_string_regex = re.compile(LGTIN_GS1_ELEMENT_STRING)
 
     def __init__(self, epc_class) -> None:
-        super().__init__()
+        super().__init__(epc_class)
 
         if not LGTIN_CLASS_REGEX.fullmatch(epc_class):
             raise ConvertException(message=f"Invalid LGTIN CLASS {epc_class}")
 
         self._company_pref, self._item_ref, *lot = ":".join(
             epc_class.split(":")[4:]
         ).split(".")
```

### Comparing `epcpy-0.1.6/epcpy/epc_schemes/pgln.py` & `epcpy-0.1.7/epcpy/epc_schemes/pgln.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from __future__ import annotations
 
 import re
 
-from epcpy.epc_schemes.base_scheme import EPCScheme, GS1Keyed
+from epcpy.epc_schemes.base_scheme import GS1Keyed
 from epcpy.utils.common import ConvertException, calculate_checksum
 from epcpy.utils.regex import PGLN_GS1_ELEMENT_STRING, PGLN_URI
 
 PGLN_URI_REGEX = re.compile(PGLN_URI)
 
 
-class PGLN(EPCScheme, GS1Keyed):
+class PGLN(GS1Keyed):
     """PGLN EPC scheme implementation.
 
     PGLN pure identities are of the form:
         urn:epc:id:pgln:<CompanyPrefix>.<PartyReference>
 
     Example:
         urn:epc:id:pgln:1234567.89012
@@ -21,18 +21,19 @@
     This class can be created using EPC pure identities via its constructor, or using:
         - PGLN.from_gs1_element_string
 
     Attributes:
         gs1_key (str): GS1 key
         gs1_element_string (str): GS1 element string
     """
+
     gs1_element_string_regex = re.compile(PGLN_GS1_ELEMENT_STRING)
 
     def __init__(self, epc_uri) -> None:
-        super().__init__()
+        super().__init__(epc_uri)
 
         if not PGLN_URI_REGEX.fullmatch(epc_uri):
             raise ConvertException(message=f"Invalid PGLN URI {epc_uri}")
 
         self._company_pref, self._party_ref = epc_uri.split(":")[4].split(".")
 
         if len(f"{self._company_pref}{self._party_ref}") != 12 or not (
```

### Comparing `epcpy-0.1.6/epcpy/epc_schemes/sgcn.py` & `epcpy-0.1.7/epcpy/epc_schemes/sgcn.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import re
 from enum import Enum
 
-from epcpy.epc_schemes.base_scheme import EPCScheme, GS1Keyed, TagEncodable
+from epcpy.epc_schemes.base_scheme import GS1Keyed, TagEncodable
 from epcpy.utils.common import (
     ConvertException,
     binary_to_int,
     calculate_checksum,
     decode_numeric_string,
     decode_partition_table,
     encode_numeric_string,
@@ -91,15 +91,15 @@
     RESERVED_3 = "3"
     RESERVED_4 = "4"
     RESERVED_5 = "5"
     RESERVED_6 = "6"
     RESERVED_7 = "7"
 
 
-class SGCN(EPCScheme, TagEncodable, GS1Keyed):
+class SGCN(TagEncodable, GS1Keyed):
     """SGCN EPC scheme implementation.
 
     SGCN pure identities are of the form:
         urn:epc:id:sgcn:<CompanyPrefix>.<CouponReference>.<SerialComponent>
 
     Example:
         urn:epc:id:sgcn:4012345.67890.04711
@@ -123,15 +123,15 @@
 
     class BinaryHeader(Enum):
         SGCN_96 = "00111111"
 
     gs1_element_string_regex = re.compile(SGCN_GS1_ELEMENT_STRING)
 
     def __init__(self, epc_uri) -> None:
-        super().__init__()
+        super().__init__(epc_uri)
 
         if not SGCN_URI_REGEX.fullmatch(epc_uri):
             raise ConvertException(message=f"Invalid SGCN URI {epc_uri}")
 
         self._company_pref, self._coupon_ref, self._serial = epc_uri.split(":")[
             4
         ].split(".")
```

### Comparing `epcpy-0.1.6/epcpy/epc_schemes/sgln.py` & `epcpy-0.1.7/epcpy/epc_schemes/sgln.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import re
 from enum import Enum
 
-from epcpy.epc_schemes.base_scheme import EPCScheme, GS1Keyed, TagEncodable
+from epcpy.epc_schemes.base_scheme import GS1Keyed, TagEncodable
 from epcpy.utils.common import (
     ConvertException,
     binary_to_int,
     calculate_checksum,
     decode_partition_table,
     decode_string,
     encode_partition_table,
@@ -92,15 +92,15 @@
     RESERVED_3 = "3"
     RESERVED_4 = "4"
     RESERVED_5 = "5"
     RESERVED_6 = "6"
     RESERVED_7 = "7"
 
 
-class SGLN(EPCScheme, TagEncodable, GS1Keyed):
+class SGLN(TagEncodable, GS1Keyed):
     """SGLN EPC scheme implementation.
 
     SGLN pure identities are of the form:
         urn:epc:id:sgln:<CompanyPrefix>.<LocationReference>.<Extension>
 
     Example:
         urn:epc:id:sgln:0614141.12345.400
@@ -126,15 +126,15 @@
     class BinaryHeader(Enum):
         SGLN_96 = "00110010"
         SGLN_195 = "00111001"
 
     gs1_element_string_regex = re.compile(SGLN_GS1_ELEMENT_STRING)
 
     def __init__(self, epc_uri) -> None:
-        super().__init__()
+        super().__init__(epc_uri)
 
         if not SGLN_URI_REGEX.fullmatch(epc_uri):
             raise ConvertException(message=f"Invalid SGLN URI {epc_uri}")
 
         self._company_pref, self._location_ref = epc_uri.split(":")[4].split(".")[:2]
         self._serial = ".".join(":".join(epc_uri.split(":")[4:]).split(".")[2:])
```

### Comparing `epcpy-0.1.6/epcpy/epc_schemes/sgtin.py` & `epcpy-0.1.7/epcpy/epc_schemes/sgtin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import re
 from enum import Enum, IntEnum
 
-from epcpy.epc_schemes.base_scheme import EPCScheme, GS1Keyed, TagEncodable
+from epcpy.epc_schemes.base_scheme import GS1Keyed, TagEncodable
 from epcpy.utils.common import (
     ConvertException,
     binary_to_int,
     calculate_checksum,
     decode_partition_table,
     decode_string,
     encode_partition_table,
@@ -99,15 +99,15 @@
 class GTIN_TYPE(IntEnum):
     GTIN8 = (8,)
     GTIN12 = (12,)
     GTIN13 = (13,)
     GTIN14 = 14
 
 
-class SGTIN(EPCScheme, TagEncodable, GS1Keyed):
+class SGTIN(TagEncodable, GS1Keyed):
     """SGTIN EPC scheme implementation.
 
     SGTIN pure identities are of the form:
         urn:epc:id:sgtin:<CompanyPrefix>.<ItemRefAndIndicator>.<SerialNumber>
 
     Example:
         urn:epc:id:sgtin:0614141.112345.400
@@ -135,15 +135,15 @@
     class BinaryHeader(Enum):
         SGTIN_96 = "00110000"
         SGTIN_198 = "00110110"
 
     gs1_element_string_regex = re.compile(SGTIN_GS1_ELEMENT_STRING)
 
     def __init__(self, epc_uri) -> None:
-        super().__init__()
+        super().__init__(epc_uri)
 
         if not SGTIN_REGEX.fullmatch(epc_uri):
             raise ConvertException(message=f"Invalid SGTIN URI {epc_uri}")
 
         self.epc_uri = epc_uri
 
         value = self.epc_uri.split(":")[4]
```

### Comparing `epcpy-0.1.6/epcpy/epc_schemes/sscc.py` & `epcpy-0.1.7/epcpy/epc_schemes/sscc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import re
 from enum import Enum
 
-from epcpy.epc_schemes.base_scheme import EPCScheme, GS1Keyed, TagEncodable
+from epcpy.epc_schemes.base_scheme import GS1Keyed, TagEncodable
 from epcpy.utils.common import (
     ConvertException,
     binary_to_int,
     calculate_checksum,
     decode_partition_table,
     encode_partition_table,
     parse_header_and_truncate_binary,
@@ -87,15 +87,15 @@
     RESERVED_3 = "3"
     RESERVED_4 = "4"
     RESERVED_5 = "5"
     UNIT_LOAD = "6"
     RESERVED_7 = "7"
 
 
-class SSCC(EPCScheme, TagEncodable, GS1Keyed):
+class SSCC(TagEncodable, GS1Keyed):
     """SSCC EPC scheme implementation.
 
     SSCC pure identities are of the form:
         urn:epc:id:sscc:<CompanyPrefix>.<SerialReference>
 
     Example:
         urn:epc:id:sscc:0614141.1234567890
@@ -115,18 +115,19 @@
     """
 
     class BinaryCodingScheme(Enum):
         SSCC_96 = "sscc-96"
 
     class BinaryHeader(Enum):
         SSCC_96 = "00110001"
+
     gs1_element_string_regex = re.compile(SSCC_GS1_ELEMENT_STRING)
 
     def __init__(self, epc_uri) -> None:
-        super().__init__()
+        super().__init__(epc_uri)
 
         if not SSCC_URI_REGEX.fullmatch(epc_uri):
             raise ConvertException(message=f"Invalid SSCC URI {epc_uri}")
 
         self.epc_uri = epc_uri
 
         self._company_pref, self._serial = self.epc_uri.split(":")[-1].split(".")
```

### Comparing `epcpy-0.1.6/epcpy/epc_schemes/upui.py` & `epcpy-0.1.7/epcpy/epc_schemes/upui.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from __future__ import annotations
 
 import re
 
-from epcpy.epc_schemes.base_scheme import EPCScheme, GS1Element
+from epcpy.epc_schemes.base_scheme import GS1Element
 from epcpy.utils.common import (
     ConvertException,
     calculate_checksum,
     replace_uri_escapes,
     revert_uri_escapes,
     verify_gs3a3_component,
 )
 from epcpy.utils.regex import UPUI_GS1_ELEMENT_STRING, UPUI_URI
 
 UPUI_URI_REGEX = re.compile(UPUI_URI)
 
 
-class UPUI(EPCScheme, GS1Element):
+class UPUI(GS1Element):
     """UPUI EPC scheme implementation.
 
     UPUI pure identities are of the form:
         urn:epc:id:upui:<CompanyPrefix>.<ItemRefAndIndicator>.<TPX>
 
     Example:
         urn:epc:id:upui:1234567.089456.51qIgY)%3C%26Jp3*j7`SDB
@@ -30,24 +30,24 @@
     Attributes:
         gs1_element_string (str): GS1 element string
     """
 
     gs1_element_string_regex = re.compile(UPUI_GS1_ELEMENT_STRING)
 
     def __init__(self, epc_uri) -> None:
-        super().__init__()
+        super().__init__(epc_uri)
 
         if not UPUI_URI_REGEX.fullmatch(epc_uri):
             raise ConvertException(message=f"Invalid UPUI URI {epc_uri}")
 
-        self._company_pref, self._item_ref, *tpx = ":".join(
+        self._company_pref, self._item_ref, *tpx_components = ":".join(
             epc_uri.split(":")[4:]
         ).split(".")
 
-        tpx = ".".join(tpx)
+        tpx = ".".join(tpx_components)
         verify_gs3a3_component(tpx)
         self._tpx = replace_uri_escapes(tpx)
 
         if not (1 <= len(self._tpx) <= 28):
             raise ConvertException(message=f"Incorrect TPX size")
 
         if len(f"{self._company_pref}{self._item_ref}") != 13:
```

### Comparing `epcpy-0.1.6/epcpy/epc_schemes/usdod.py` & `epcpy-0.1.7/epcpy/epc_schemes/usdod.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import re
 from enum import Enum
 
-from epcpy.epc_schemes.base_scheme import EPCScheme, TagEncodable
+from epcpy.epc_schemes.base_scheme import TagEncodable
 from epcpy.utils.common import (
     ConvertException,
     binary_to_int,
     decode_cage_code,
     encode_cage_code,
     parse_header_and_truncate_binary,
     str_to_binary,
@@ -32,15 +32,15 @@
     RESERVED_11 = "11"
     RESERVED_12 = "12"
     RESERVED_13 = "13"
     RESERVED_14 = "14"
     RESERVED_15 = "15"
 
 
-class USDOD(EPCScheme, TagEncodable):
+class USDOD(TagEncodable):
     """USDOD EPC scheme implementation.
 
     USDOD pure identities are of the form:
         urn:epc:id:usdod:<CAGEOrDODAAC>.<SerialNumber>
 
     Example:
         urn:epc:id:usdod:2S194.12345678901
@@ -51,22 +51,23 @@
         - USDOD.from_base64
         - USDOD.from_tag_uri
 
     Attributes:
         tag_uri (str): Tag URI
         binary (str): Binary representation
     """
+
     class BinaryCodingScheme(Enum):
         USDOD_96 = "usdod-96"
 
     class BinaryHeader(Enum):
         USDOD_96 = "00101111"
 
     def __init__(self, epc_uri) -> None:
-        super().__init__()
+        super().__init__(epc_uri)
 
         if not USDOD_URI_REGEX.fullmatch(epc_uri):
             raise ConvertException(message=f"Invalid USDOD URI {epc_uri}")
 
         self._cage_dodaac, self._serial = epc_uri.split(":")[4].split(".")
 
         if int(self._serial) >= pow(2, 36) or (
@@ -87,15 +88,15 @@
             filter_value (USDODFilterValue): Filter value
             binary_coding_scheme (BinaryCodingScheme): Coding scheme
                 Defaults to BinaryCodingScheme.USDOD_96
 
         Returns:
             str: Tag URI
         """
-        return f"{self.TAG_URI_PREFIX}{binary_coding_scheme.USDOD_96.value}:{filter_value.value}.{self._cage_dodaac}.{self._serial}"
+        return f"{self.TAG_URI_PREFIX}{binary_coding_scheme.value}:{filter_value.value}.{self._cage_dodaac}.{self._serial}"
 
     def binary(
         self,
         filter_value: USDODFilterValue,
         binary_coding_scheme: BinaryCodingScheme = BinaryCodingScheme.USDOD_96,
     ) -> str:
         """Return the binary representation belonging to this USDOD with the provided binary coding scheme and filter value.
@@ -104,15 +105,15 @@
             filter_value (USDODFilterValue): Filter value
             binary_coding_scheme (BinaryCodingScheme): Coding scheme
                 Defaults to BinaryCodingScheme.USDOD_96
 
         Returns:
             str: binary representation
         """
-        header = USDOD.BinaryHeader[binary_coding_scheme.USDOD_96.name].value
+        header = USDOD.BinaryHeader[binary_coding_scheme.name].value
         filter_binary = str_to_binary(filter_value.value, 4)
         cage_code_binary = encode_cage_code(f"{self._cage_dodaac:>6}")
         serial_binary = str_to_binary(self._serial, 36)
 
         return header + filter_binary + cage_code_binary + serial_binary
 
     @classmethod
```

### Comparing `epcpy-0.1.6/epcpy/utils/common.py` & `epcpy-0.1.7/epcpy/utils/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import base64
 import re
 from enum import Enum
-from math import inf, log
+from math import log
 from typing import Dict, List, Tuple
 
 from epcpy.utils.regex import VERIFY_GS3A3_CHARS
 
 ESCAPE_CHARACTERS = {
     "0100010": "%22",
     "0100101": "%25",
@@ -167,17 +167,17 @@
         str: Binary string
     """
     res = ""
     for g in re.split("(%[0-9a-fA-F]{2})", string):
         if len(g) == 0:
             continue
         elif g[0] != "%":
-            res += "".join([str_to_binary(ord(s), 7) for s in g])
+            res += "".join([str_to_binary(str(ord(s)), 7) for s in g])
         else:
-            res += str_to_binary(int(g[1:], 16), 7)
+            res += str_to_binary(str(int(g[1:], 16)), 7)
     return f"{res:<0{num_bits}}"
 
 
 def decode_string_six_bits(binary: str, max_chars: int) -> str:
     """Decode binary string by decoding every sequence of six bits.
 
     Args:
@@ -226,15 +226,15 @@
             res += "".join(
                 [
                     f"11{int(s):04b}" if s.isnumeric() else f"{int(ord(s) - 64):06b}"
                     for s in g
                 ]
             )
         else:
-            res += str_to_binary(int(g[1:], 16), 6)
+            res += str_to_binary(str(int(g[1:], 16)), 6)
     return f"{res}000000"
 
 
 def decode_binary_char(binary: str) -> str:
     """Decode a single binary sequence of seven bits
 
     Args:
@@ -268,15 +268,15 @@
             )
         )
     )
 
 
 def encode_partition_table(
     parts: List[str],
-    partition_table: List[Dict[str, Dict[str, int]]],
+    partition_table: Dict[int, Dict[str, int]],
     string_partition=False,
     six_bit_variable_partition=False,
 ) -> str:
     """Encode a string based on a partition table
 
     Args:
         parts (List[str]): Parts of the string to encode
@@ -309,15 +309,15 @@
         )
 
     return P_bin + C_bin + D_bin
 
 
 def decode_partition_table(
     binary_string: str,
-    partition_table: List[Dict[str, Dict[str, int]]],
+    partition_table: Dict[int, Dict[str, int]],
     unpadded_partition=False,
     string_partition=False,
     six_bit_variable_partition=False,
 ) -> str:
     """Decode a binary string using a partition table.
 
     Args:
@@ -345,23 +345,23 @@
     D_bin = binary_string[(3 + partition["M"]) : (3 + partition["M"] + partition["N"])]
 
     if string_partition:
         D = decode_string(D_bin)
     elif six_bit_variable_partition:
         D = decode_string_six_bits(D_bin, partition["K"])
     else:
-        D = binary_to_int(D_bin) if partition["K"] != 0 else ""
+        D = str(binary_to_int(D_bin)) if partition["K"] != 0 else ""
 
     compare_D = not (
         unpadded_partition or string_partition or six_bit_variable_partition
     )
 
     if not C < pow(10, partition["L"]):
         raise ConvertException(message=f"Company prefix length too large")
-    if D != "" and compare_D and not D < pow(10, partition["K"]):
+    if D != "" and compare_D and not int(D) < pow(10, partition["K"]):
         raise ConvertException(message=f"Item reference length too large")
 
     return f"{C:>0{partition['L']}}.{D:>0{partition['K'] if compare_D else 0}}"
 
 
 def encode_numeric_string(string: str, bit_count: int) -> str:
     """Encode a numeric string
@@ -474,15 +474,15 @@
 
     Returns:
         str: Decoded string
     """
     if binary.startswith("100000"):
         binary = binary[6:]
 
-    return decode_string_six_bits(binary, inf)
+    return decode_string_six_bits(binary, 6)
 
 
 def encode_cage_code_six_bits(chars: str) -> str:
     """Encode a character sequence using six bit cage codes
 
     Args:
         chars (str): Character sequence to encode
@@ -523,31 +523,31 @@
 
     Args:
         digits (str): String of digits
 
     Returns:
         int: Check digit
     """
-    digits = [int(d) for d in digits]
-    odd, even = digits[1::2], digits[0::2]
+    digit_list = [int(d) for d in digits]
+    odd, even = digit_list[1::2], digit_list[0::2]
 
     if len(digits) % 2 == 0:
         val1 = sum(odd)
         val2 = sum(even)
     else:
         val1 = sum(even)
         val2 = sum(odd)
 
     checksum = (10 - ((3 * (val1) + (val2)) % 10)) % 10
 
     return checksum
 
 
 def parse_header_and_truncate_binary(
-    binary_string: str, header_to_schemes: Dict[str, str]
+    binary_string: str, header_to_schemes: Dict[str, Enum]
 ) -> Tuple[Enum, str]:
     """Parse a binary header, detect the scheme and truncate the binary string based on the scheme.
 
     Args:
         binary_string (str): Full length binary string
         header_to_schemes (Dict[str, str]): Mapping from binary headers to schemes
```

### Comparing `epcpy-0.1.6/epcpy/utils/parsers.py` & `epcpy-0.1.7/epcpy/utils/parsers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import re
-from typing import List, Union
+from typing import Dict, List, Optional, Type
 
 from epcpy.epc_schemes import (
     ADI,
     BIC,
     CPI,
     GDTI,
     GIAI,
@@ -34,15 +34,15 @@
 from epcpy.utils.regex import EPC_URI, GS1_ELEMENT_STRING, IDPAT_URI, TAG_URI
 
 EPC_URI_REGEX = re.compile(EPC_URI)
 GS1_ELEMENT_STRING_REGEX = re.compile(GS1_ELEMENT_STRING)
 IDPAT_URI_REGEX = re.compile(IDPAT_URI)
 TAG_URI_REGEX = re.compile(TAG_URI)
 
-EPC_SCHEMES: List[EPCScheme] = [
+EPC_SCHEMES: List[Type[EPCScheme]] = [
     ADI,
     BIC,
     CPI,
     GDTI,
     GIAI,
     GID,
     GINC,
@@ -57,44 +57,46 @@
     SGCN,
     SGLN,
     SGTIN,
     SSCC,
     UPUI,
     USDOD,
 ]
-GS1_KEYED_CLASSES: List[GS1Keyed] = [
+GS1_KEYED_CLASSES: List[Type[GS1Keyed]] = [
     cls for cls in EPC_SCHEMES if issubclass(cls, GS1Keyed)
 ]
-TAG_ENCODABLE_CLASSES: List[TagEncodable] = [
+TAG_ENCODABLE_CLASSES: List[Type[TagEncodable]] = [
     cls for cls in EPC_SCHEMES if issubclass(cls, TagEncodable)
 ]
 
 TAG_ENCODABLE_BINARY_HEADERS = {
     h.value: cls for cls in TAG_ENCODABLE_CLASSES for h in cls.BinaryHeader
 }
 TAG_ENCODABLE_HEX_HEADERS = {
     binary_to_hex(h.value): cls
     for cls in TAG_ENCODABLE_CLASSES
     for h in cls.BinaryHeader
 }
 
-GS1_ELEMENT_STRING_REGEX_TO_SCHEME: Union[re.Pattern, GS1Element] = {
+GS1_ELEMENT_STRING_REGEX_TO_SCHEME: Dict[re.Pattern, Type[GS1Element]] = {
     cls.gs1_element_string_regex: cls
     for cls in EPC_SCHEMES
     if issubclass(cls, GS1Element)
 }
 
 EPC_SCHEME_IDENTIFIERS = {cls.__name__.lower(): cls for cls in EPC_SCHEMES}
 TAG_ENCODABLE_SCHEME_IDENTIFIERS = {
     cls.__name__.lower(): cls for cls in TAG_ENCODABLE_CLASSES
 }
 GS1_KEYED_SCHEME_IDENTIFIERS = {cls.__name__.lower(): cls for cls in GS1_KEYED_CLASSES}
 
 
-def get_gs1_key(source: str, company_prefix_length: int = None, **kwargs) -> str:
+def get_gs1_key(
+    source: str, company_prefix_length: Optional[int] = None, **kwargs
+) -> str:
     """Get the GS1 key belonging to the source string.
     This method can identify and parse:
     - EPC pure identity URIs
     - EPC tag URIs
     - GS1 element strings (company_prefix_length should be provided)
     - IDPAT URIs
     - Binary strings
@@ -111,15 +113,15 @@
     Returns:
         str: GS1 key of source string
     """
     scheme = None
 
     if EPC_URI_REGEX.fullmatch(source):
         scheme = epc_pure_identity_to_scheme(source)
-    elif GS1_ELEMENT_STRING_REGEX.fullmatch(source):
+    elif GS1_ELEMENT_STRING_REGEX.fullmatch(source) and company_prefix_length:
         scheme = gs1_element_string_to_gs1_element(source, company_prefix_length)
     elif TAG_URI_REGEX.fullmatch(source):
         scheme = tag_uri_to_tag_encodable(source)
     elif IDPAT_URI_REGEX.fullmatch(source):
         scheme = _idpat_to_gs1_keyed_scheme(source)
     elif source[:8] in TAG_ENCODABLE_BINARY_HEADERS.keys():
         scheme = binary_to_tag_encodable(source)
@@ -289,23 +291,23 @@
         raise ConvertException(message="Unknown GS1Keyed identifier")
 
     # Create URI from idpat
     uri = idpat.replace("idpat", "id", 1)
 
     # URI already matches existing scheme
     if EPC_URI_REGEX.fullmatch(uri):
-        return GS1_KEYED_SCHEME_IDENTIFIERS[identifier].from_epc_uri(uri)
+        return GS1_KEYED_SCHEME_IDENTIFIERS[identifier](uri)
 
     if identifier not in ONE_ESCAPE_ALLOWED_SCHEMES:
         raise ConvertException(message="URI exceeds maximum number of escaped patterns")
 
     # Create URI with dummy serial to create GS1 key
     dummy_uri = re.sub("\.\*$", ".0", uri, 1)
     if EPC_URI_REGEX.fullmatch(dummy_uri):
-        return GS1_KEYED_SCHEME_IDENTIFIERS[identifier].from_epc_uri(dummy_uri)
+        return GS1_KEYED_SCHEME_IDENTIFIERS[identifier](dummy_uri)
 
     raise ConvertException(message="Could not create valid scheme from given id pat")
 
 
 def tag_uri_to_tag_encodable(epc_tag_uri: str) -> TagEncodable:
     """EPC tag URI to TagEncodable class
```

### Comparing `epcpy-0.1.6/epcpy/utils/regex.py` & `epcpy-0.1.7/epcpy/utils/regex.py`

 * *Files identical despite different names*

### Comparing `epcpy-0.1.6/LICENSE` & `epcpy-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `epcpy-0.1.6/pyproject.toml` & `epcpy-0.1.7/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "epcpy"
-version = "0.1.6"
+version = "0.1.7"
 description = "A Python module for creation, validation, and transformation of EPC representations as defined in GS1's EPC Tag Data Standard."
 license = "MIT"
 authors = ["Nedap Retail <sander.meinderts@nedap.com>"]
 readme = "README_pip.md"
 homepage = "https://github.com/nedap/retail-epcpy"
 repository = "https://github.com/nedap/retail-epcpy"
 keywords =  [
@@ -15,26 +15,27 @@
     "sgtin"
 ]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
 ]
 
 [tool.poetry.scripts]
 test = "scripts:test"
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 
 [tool.poetry.dev-dependencies]
-black = "22.1.0"
-coverage = "^6.3.2"
+black = "latest"
+coverage = "latest"
+mypy = "latest"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `epcpy-0.1.6/README_pip.md` & `epcpy-0.1.7/README_pip.md`

 * *Files identical despite different names*

### Comparing `epcpy-0.1.6/setup.py` & `epcpy-0.1.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 {'': ['*']}
 
 entry_points = \
 {'console_scripts': ['test = scripts:test']}
 
 setup_kwargs = {
     'name': 'epcpy',
-    'version': '0.1.6',
+    'version': '0.1.7',
     'description': "A Python module for creation, validation, and transformation of EPC representations as defined in GS1's EPC Tag Data Standard.",
     'long_description': "# EPCPY\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)\n[![PyPI version](https://badge.fury.io/py/epcpy.svg)](https://badge.fury.io/py/epcpy)\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/epcpy.svg)](https://pypi.org/project/epcpy/)\n\n\nA Python module for creation, validation, and transformation of EPC representations as defined in GS1's EPC Tag Data Standard (https://www.gs1.org/standards/rfid/tds).\n\n## Installation\n```python\npip install epcpy\n```\n\n## Documentation\nDocumentation can be found on [Git](https://github.com/nedap/retail-epcpy).",
     'author': 'Nedap Retail',
     'author_email': 'sander.meinderts@nedap.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/nedap/retail-epcpy',
     'packages': packages,
     'package_data': package_data,
     'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
+    'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `epcpy-0.1.6/PKG-INFO` & `epcpy-0.1.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: epcpy
-Version: 0.1.6
+Version: 0.1.7
 Summary: A Python module for creation, validation, and transformation of EPC representations as defined in GS1's EPC Tag Data Standard.
 Home-page: https://github.com/nedap/retail-epcpy
 License: MIT
 Keywords: gs1,epc,python,gtin,sgtin
 Author: Nedap Retail
 Author-email: sander.meinderts@nedap.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Project-URL: Repository, https://github.com/nedap/retail-epcpy
 Description-Content-Type: text/markdown
 
 # EPCPY
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

