# Comparing `tmp/starrailres-1.0.0.tar.gz` & `tmp/starrailres-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starrailres-1.0.0.tar", max compression
+gzip compressed data, was "starrailres-1.0.1.tar", max compression
```

## Comparing `starrailres-1.0.0.tar` & `starrailres-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0     1083 2023-05-23 12:01:47.249793 starrailres-1.0.0/LICENSE
--rw-r--r--   0        0        0      499 2023-05-31 11:50:36.860460 starrailres-1.0.0/pyproject.toml
--rw-r--r--   0        0        0       59 2023-05-24 08:16:08.001669 starrailres-1.0.0/README.md
--rw-r--r--   0        0        0       22 2023-05-29 15:05:23.416606 starrailres-1.0.0/starrailres/__init__.py
--rw-r--r--   0        0        0    28507 2023-05-30 07:51:56.934078 starrailres-1.0.0/starrailres/index.py
--rw-r--r--   0        0        0     1723 2023-05-29 05:55:48.065843 starrailres-1.0.0/starrailres/models/characters.py
--rw-r--r--   0        0        0      210 2023-05-26 14:44:56.999166 starrailres-1.0.0/starrailres/models/common.py
--rw-r--r--   0        0        0      245 2023-05-25 07:04:39.480460 starrailres-1.0.0/starrailres/models/descriptions.py
--rw-r--r--   0        0        0      295 2023-05-23 14:27:36.388191 starrailres-1.0.0/starrailres/models/elements.py
--rw-r--r--   0        0        0     3189 2023-05-30 05:47:49.671310 starrailres-1.0.0/starrailres/models/info.py
--rw-r--r--   0        0        0      352 2023-05-25 07:16:41.407713 starrailres-1.0.0/starrailres/models/items.py
--rw-r--r--   0        0        0      734 2023-05-29 13:34:04.145217 starrailres-1.0.0/starrailres/models/light_cones.py
--rw-r--r--   0        0        0      269 2023-05-23 14:27:09.523569 starrailres-1.0.0/starrailres/models/paths.py
--rw-r--r--   0        0        0      429 2023-05-29 14:28:24.391190 starrailres-1.0.0/starrailres/models/properties.py
--rw-r--r--   0        0        0      993 2023-05-30 04:32:44.019242 starrailres-1.0.0/starrailres/models/relics.py
--rw-r--r--   0        0        0        0 2023-05-25 07:11:50.015616 starrailres-1.0.0/starrailres/starrailres.py
--rw-r--r--   0        0        0      323 2023-05-25 07:32:33.386416 starrailres-1.0.0/starrailres/utils.py
--rw-r--r--   0        0        0      747 1970-01-01 00:00:00.000000 starrailres-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-05-23 12:01:47.249793 starrailres-1.0.1/LICENSE
+-rw-r--r--   0        0        0      499 2023-05-31 13:17:20.467326 starrailres-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      924 2023-05-31 11:58:49.998393 starrailres-1.0.1/README.md
+-rw-r--r--   0        0        0       22 2023-05-29 15:05:23.416606 starrailres-1.0.1/starrailres/__init__.py
+-rw-r--r--   0        0        0    28999 2023-05-31 13:16:18.774488 starrailres-1.0.1/starrailres/index.py
+-rw-r--r--   0        0        0      216 2023-05-31 13:14:58.577684 starrailres-1.0.1/starrailres/models/avatars.py
+-rw-r--r--   0        0        0     1723 2023-05-29 05:55:48.065843 starrailres-1.0.1/starrailres/models/characters.py
+-rw-r--r--   0        0        0      210 2023-05-26 14:44:56.999166 starrailres-1.0.1/starrailres/models/common.py
+-rw-r--r--   0        0        0      245 2023-05-25 07:04:39.480460 starrailres-1.0.1/starrailres/models/descriptions.py
+-rw-r--r--   0        0        0      295 2023-05-23 14:27:36.388191 starrailres-1.0.1/starrailres/models/elements.py
+-rw-r--r--   0        0        0     3265 2023-05-31 13:16:18.582411 starrailres-1.0.1/starrailres/models/info.py
+-rw-r--r--   0        0        0      352 2023-05-25 07:16:41.407713 starrailres-1.0.1/starrailres/models/items.py
+-rw-r--r--   0        0        0      734 2023-05-29 13:34:04.145217 starrailres-1.0.1/starrailres/models/light_cones.py
+-rw-r--r--   0        0        0      269 2023-05-23 14:27:09.523569 starrailres-1.0.1/starrailres/models/paths.py
+-rw-r--r--   0        0        0      429 2023-05-29 14:28:24.391190 starrailres-1.0.1/starrailres/models/properties.py
+-rw-r--r--   0        0        0      993 2023-05-30 04:32:44.019242 starrailres-1.0.1/starrailres/models/relics.py
+-rw-r--r--   0        0        0        0 2023-05-25 07:11:50.015616 starrailres-1.0.1/starrailres/starrailres.py
+-rw-r--r--   0        0        0      323 2023-05-25 07:32:33.386416 starrailres-1.0.1/starrailres/utils.py
+-rw-r--r--   0        0        0     1573 1970-01-01 00:00:00.000000 starrailres-1.0.1/PKG-INFO
```

### Comparing `starrailres-1.0.0/LICENSE` & `starrailres-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `starrailres-1.0.0/starrailres/index.py` & `starrailres-1.0.1/starrailres/index.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import math
 from copy import deepcopy
 from pathlib import Path
 from typing import Dict, List, Optional
 
+from .models.avatars import AvatarIndex
 from .models.characters import (
     CharacterIndex,
     CharacterPromotionIndex,
     CharacterRankIndex,
     CharacterSkillIndex,
     CharacterSkillTreeIndex,
 )
 from .models.elements import ElementIndex
 from .models.info import (
     AttributeInfo,
+    AvatarInfo,
     CharacterBasicInfo,
     CharacterInfo,
     ElementInfo,
     LevelInfo,
     LightConeBasicInfo,
     LightConeInfo,
     PathInfo,
@@ -55,14 +57,15 @@
     relics: RelicIndex
     relic_sets: RelicSetIndex
     relic_main_affixes: RelicMainAffixIndex
     relic_sub_affixes: RelicSubAffixIndex
     paths: PathIndex
     elements: ElementIndex
     properties: PropertyIndex
+    avatars: AvatarIndex
 
     def __init__(self, folder: Path) -> None:
         if not folder.exists():
             raise Exception("Please select an existing index folder!")
         self.characters = decode_json(folder / "characters.json", CharacterIndex)
         self.character_ranks = decode_json(
             folder / "character_ranks.json", CharacterRankIndex
@@ -90,14 +93,27 @@
         )
         self.relic_sub_affixes = decode_json(
             folder / "relic_sub_affixes.json", RelicSubAffixIndex
         )
         self.paths = decode_json(folder / "paths.json", PathIndex)
         self.elements = decode_json(folder / "elements.json", ElementIndex)
         self.properties = decode_json(folder / "properties.json", PropertyIndex)
+        self.avatars = decode_json(folder / "avatars.json", AvatarIndex)
+
+    def get_avatar_info(self, id: str) -> Optional[AvatarInfo]:
+        """
+        Get avatar info by avatar id.
+        """
+        if id not in self.avatars:
+            return None
+        return AvatarInfo(
+            id=id,
+            name=self.avatars[id].name,
+            icon=self.avatars[id].icon,
+        )
 
     def get_path_info(self, id: str) -> Optional[PathInfo]:
         """
         Get path info by path id.
         """
         if id in self.paths:
             return PathInfo(id, self.paths[id].name, self.paths[id].icon)
```

### Comparing `starrailres-1.0.0/starrailres/models/characters.py` & `starrailres-1.0.1/starrailres/models/characters.py`

 * *Files identical despite different names*

### Comparing `starrailres-1.0.0/starrailres/models/info.py` & `starrailres-1.0.1/starrailres/models/info.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,20 @@
 
 
 class LevelInfo(BaseInfo):
     id: str
     level: int = 0
 
 
+class AvatarInfo(BaseInfo):
+    id: str
+    name: str
+    icon: str
+
+
 class PathInfo(BaseInfo):
     id: str
     name: str
     icon: str
 
 
 class ElementInfo(BaseInfo):
```

### Comparing `starrailres-1.0.0/starrailres/models/light_cones.py` & `starrailres-1.0.1/starrailres/models/light_cones.py`

 * *Files identical despite different names*

### Comparing `starrailres-1.0.0/starrailres/models/relics.py` & `starrailres-1.0.1/starrailres/models/relics.py`

 * *Files identical despite different names*

