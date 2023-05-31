# Comparing `tmp/crankshaft-0.1.1.tar.gz` & `tmp/crankshaft-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crankshaft-0.1.1.tar", max compression
+gzip compressed data, was "crankshaft-0.2.0.tar", max compression
```

## Comparing `crankshaft-0.1.1.tar` & `crankshaft-0.2.0.tar`

### file list

```diff
@@ -1,58 +1,60 @@
--rw-r--r--   0        0        0     1067 2023-05-26 10:06:52.238649 crankshaft-0.1.1/LICENSE
--rw-r--r--   0        0        0      336 2023-05-26 10:06:52.238649 crankshaft-0.1.1/README.md
--rw-r--r--   0        0        0      326 2023-05-26 10:07:51.611181 crankshaft-0.1.1/crankshaft/__init__.py
--rw-r--r--   0        0        0      120 2023-05-26 10:06:52.238649 crankshaft-0.1.1/crankshaft/modules/api.bolt
--rw-r--r--   0        0        0      216 2023-05-26 10:06:52.238649 crankshaft-0.1.1/crankshaft/modules/config.bolt
--rw-r--r--   0        0        0      512 2023-05-26 10:06:52.238649 crankshaft-0.1.1/crankshaft/modules/defer.bolt
--rw-r--r--   0        0        0     2859 2023-05-26 10:06:52.242649 crankshaft-0.1.1/crankshaft/modules/event_handler.bolt
--rw-r--r--   0        0        0     1423 2023-05-26 10:06:52.242649 crankshaft-0.1.1/crankshaft/modules/events/on_entity_attack_player.bolt
--rw-r--r--   0        0        0      240 2023-05-26 10:06:52.242649 crankshaft-0.1.1/crankshaft/modules/events/on_load.bolt
--rw-r--r--   0        0        0      337 2023-05-26 10:06:52.242649 crankshaft-0.1.1/crankshaft/modules/events/on_player_airborne.bolt
--rw-r--r--   0        0        0      661 2023-05-26 10:06:52.242649 crankshaft-0.1.1/crankshaft/modules/events/on_player_airborne_end.bolt
--rw-r--r--   0        0        0      662 2023-05-26 10:06:52.242649 crankshaft-0.1.1/crankshaft/modules/events/on_player_airborne_start.bolt
--rw-r--r--   0        0        0     1423 2023-05-26 10:06:52.242649 crankshaft-0.1.1/crankshaft/modules/events/on_player_attack_entity.bolt
--rw-r--r--   0        0        0      326 2023-05-26 10:06:52.242649 crankshaft-0.1.1/crankshaft/modules/events/on_player_burn.bolt
--rw-r--r--   0        0        0      650 2023-05-26 10:06:52.242649 crankshaft-0.1.1/crankshaft/modules/events/on_player_burn_end.bolt
--rw-r--r--   0        0        0      651 2023-05-26 10:06:52.242649 crankshaft-0.1.1/crankshaft/modules/events/on_player_burn_start.bolt
--rw-r--r--   0        0        0      352 2023-05-26 10:06:52.242649 crankshaft-0.1.1/crankshaft/modules/events/on_player_charge_bow.bolt
--rw-r--r--   0        0        0      779 2023-05-26 10:06:52.242649 crankshaft-0.1.1/crankshaft/modules/events/on_player_charge_bow_end.bolt
--rw-r--r--   0        0        0      780 2023-05-26 10:06:52.242649 crankshaft-0.1.1/crankshaft/modules/events/on_player_charge_bow_start.bolt
--rw-r--r--   0        0        0      328 2023-05-26 10:06:52.242649 crankshaft-0.1.1/crankshaft/modules/events/on_player_glide.bolt
--rw-r--r--   0        0        0      653 2023-05-26 10:06:52.242649 crankshaft-0.1.1/crankshaft/modules/events/on_player_glide_end.bolt
--rw-r--r--   0        0        0      654 2023-05-26 10:06:52.242649 crankshaft-0.1.1/crankshaft/modules/events/on_player_glide_start.bolt
--rw-r--r--   0        0        0      637 2023-05-26 10:06:52.242649 crankshaft-0.1.1/crankshaft/modules/events/on_player_inventory_change.bolt
--rw-r--r--   0        0        0      559 2023-05-26 10:06:52.242649 crankshaft-0.1.1/crankshaft/modules/events/on_player_join.bolt
--rw-r--r--   0        0        0      567 2023-05-26 10:06:52.242649 crankshaft-0.1.1/crankshaft/modules/events/on_player_jump.bolt
--rw-r--r--   0        0        0      668 2023-05-26 10:06:52.242649 crankshaft-0.1.1/crankshaft/modules/events/on_player_land.bolt
--rw-r--r--   0        0        0      375 2023-05-26 10:06:52.242649 crankshaft-0.1.1/crankshaft/modules/events/on_player_load.bolt
--rw-r--r--   0        0        0      520 2023-05-26 10:06:52.242649 crankshaft-0.1.1/crankshaft/modules/events/on_player_shoot_bow.bolt
--rw-r--r--   0        0        0      331 2023-05-26 10:06:52.242649 crankshaft-0.1.1/crankshaft/modules/events/on_player_sneak.bolt
--rw-r--r--   0        0        0      656 2023-05-26 10:06:52.242649 crankshaft-0.1.1/crankshaft/modules/events/on_player_sneak_end.bolt
--rw-r--r--   0        0        0      657 2023-05-26 10:06:52.242649 crankshaft-0.1.1/crankshaft/modules/events/on_player_sneak_start.bolt
--rw-r--r--   0        0        0      336 2023-05-26 10:06:52.242649 crankshaft-0.1.1/crankshaft/modules/events/on_player_sprint.bolt
--rw-r--r--   0        0        0      661 2023-05-26 10:06:52.242649 crankshaft-0.1.1/crankshaft/modules/events/on_player_sprint_end.bolt
--rw-r--r--   0        0        0      662 2023-05-26 10:06:52.242649 crankshaft-0.1.1/crankshaft/modules/events/on_player_sprint_start.bolt
--rw-r--r--   0        0        0      329 2023-05-26 10:06:52.242649 crankshaft-0.1.1/crankshaft/modules/events/on_player_swim.bolt
--rw-r--r--   0        0        0      654 2023-05-26 10:06:52.242649 crankshaft-0.1.1/crankshaft/modules/events/on_player_swim_end.bolt
--rw-r--r--   0        0        0      655 2023-05-26 10:06:52.242649 crankshaft-0.1.1/crankshaft/modules/events/on_player_swim_start.bolt
--rw-r--r--   0        0        0      253 2023-05-26 10:06:52.242649 crankshaft-0.1.1/crankshaft/modules/events/on_player_tick.bolt
--rw-r--r--   0        0        0      240 2023-05-26 10:06:52.242649 crankshaft-0.1.1/crankshaft/modules/events/on_tick.bolt
--rw-r--r--   0        0        0     2007 2023-05-26 10:06:52.242649 crankshaft-0.1.1/crankshaft/modules/events.bolt
--rw-r--r--   0        0        0     3684 2023-05-26 10:06:52.242649 crankshaft-0.1.1/crankshaft/modules/flag.bolt
--rw-r--r--   0        0        0      377 2023-05-26 10:06:52.242649 crankshaft-0.1.1/crankshaft/modules/flags/is_airborne.bolt
--rw-r--r--   0        0        0      402 2023-05-26 10:06:52.242649 crankshaft-0.1.1/crankshaft/modules/flags/is_baby.bolt
--rw-r--r--   0        0        0      411 2023-05-26 10:06:52.242649 crankshaft-0.1.1/crankshaft/modules/flags/is_burning.bolt
--rw-r--r--   0        0        0     1230 2023-05-26 10:06:52.242649 crankshaft-0.1.1/crankshaft/modules/flags/is_charging_bow.bolt
--rw-r--r--   0        0        0      377 2023-05-26 10:06:52.242649 crankshaft-0.1.1/crankshaft/modules/flags/is_gliding.bolt
--rw-r--r--   0        0        0      158 2023-05-26 10:06:52.242649 crankshaft-0.1.1/crankshaft/modules/flags/is_player.bolt
--rw-r--r--   0        0        0      414 2023-05-26 10:06:52.242649 crankshaft-0.1.1/crankshaft/modules/flags/is_sneaking.bolt
--rw-r--r--   0        0        0      417 2023-05-26 10:06:52.242649 crankshaft-0.1.1/crankshaft/modules/flags/is_sprinting.bolt
--rw-r--r--   0        0        0      414 2023-05-26 10:06:52.242649 crankshaft-0.1.1/crankshaft/modules/flags/is_swimming.bolt
--rw-r--r--   0        0        0      443 2023-05-26 10:06:52.242649 crankshaft-0.1.1/crankshaft/modules/flags.bolt
--rw-r--r--   0        0        0      407 2023-05-26 10:06:52.242649 crankshaft-0.1.1/crankshaft/modules/lib/entity_hit_matching/api.bolt
--rw-r--r--   0        0        0      124 2023-05-26 10:06:52.242649 crankshaft-0.1.1/crankshaft/modules/lib/entity_hit_matching/credits.txt
--rw-r--r--   0        0        0    58172 2023-05-26 10:06:52.242649 crankshaft-0.1.1/crankshaft/modules/lib/entity_hit_matching/main.bolt
--rw-r--r--   0        0        0      207 2023-05-26 10:06:52.242649 crankshaft-0.1.1/crankshaft/modules/utils.bolt
--rw-r--r--   0        0        0        0 2023-05-26 10:06:52.242649 crankshaft-0.1.1/crankshaft/py.typed
--rw-r--r--   0        0        0     1260 2023-05-26 10:07:51.627181 crankshaft-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1106 1970-01-01 00:00:00.000000 crankshaft-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-31 18:08:15.450634 crankshaft-0.2.0/LICENSE
+-rw-r--r--   0        0        0      336 2023-05-31 18:08:15.450634 crankshaft-0.2.0/README.md
+-rw-r--r--   0        0        0      326 2023-05-31 18:09:24.291467 crankshaft-0.2.0/crankshaft/__init__.py
+-rw-r--r--   0        0        0      120 2023-05-31 18:08:15.450634 crankshaft-0.2.0/crankshaft/modules/api.bolt
+-rw-r--r--   0        0        0      216 2023-05-31 18:08:15.450634 crankshaft-0.2.0/crankshaft/modules/config.bolt
+-rw-r--r--   0        0        0      512 2023-05-31 18:08:15.450634 crankshaft-0.2.0/crankshaft/modules/defer.bolt
+-rw-r--r--   0        0        0     3721 2023-05-31 18:08:15.450634 crankshaft-0.2.0/crankshaft/modules/event_handler.bolt
+-rw-r--r--   0        0        0     1441 2023-05-31 18:08:15.450634 crankshaft-0.2.0/crankshaft/modules/events/on_entity_attack_player.bolt
+-rw-r--r--   0        0        0      258 2023-05-31 18:08:15.450634 crankshaft-0.2.0/crankshaft/modules/events/on_load.bolt
+-rw-r--r--   0        0        0      355 2023-05-31 18:08:15.450634 crankshaft-0.2.0/crankshaft/modules/events/on_player_airborne.bolt
+-rw-r--r--   0        0        0      679 2023-05-31 18:08:15.450634 crankshaft-0.2.0/crankshaft/modules/events/on_player_airborne_end.bolt
+-rw-r--r--   0        0        0      680 2023-05-31 18:08:15.450634 crankshaft-0.2.0/crankshaft/modules/events/on_player_airborne_start.bolt
+-rw-r--r--   0        0        0     1441 2023-05-31 18:08:15.450634 crankshaft-0.2.0/crankshaft/modules/events/on_player_attack_entity.bolt
+-rw-r--r--   0        0        0      344 2023-05-31 18:08:15.450634 crankshaft-0.2.0/crankshaft/modules/events/on_player_burn.bolt
+-rw-r--r--   0        0        0      668 2023-05-31 18:08:15.450634 crankshaft-0.2.0/crankshaft/modules/events/on_player_burn_end.bolt
+-rw-r--r--   0        0        0      669 2023-05-31 18:08:15.450634 crankshaft-0.2.0/crankshaft/modules/events/on_player_burn_start.bolt
+-rw-r--r--   0        0        0      370 2023-05-31 18:08:15.450634 crankshaft-0.2.0/crankshaft/modules/events/on_player_charge_bow.bolt
+-rw-r--r--   0        0        0      797 2023-05-31 18:08:15.450634 crankshaft-0.2.0/crankshaft/modules/events/on_player_charge_bow_end.bolt
+-rw-r--r--   0        0        0      798 2023-05-31 18:08:15.450634 crankshaft-0.2.0/crankshaft/modules/events/on_player_charge_bow_start.bolt
+-rw-r--r--   0        0        0      346 2023-05-31 18:08:15.450634 crankshaft-0.2.0/crankshaft/modules/events/on_player_glide.bolt
+-rw-r--r--   0        0        0      671 2023-05-31 18:08:15.450634 crankshaft-0.2.0/crankshaft/modules/events/on_player_glide_end.bolt
+-rw-r--r--   0        0        0      672 2023-05-31 18:08:15.450634 crankshaft-0.2.0/crankshaft/modules/events/on_player_glide_start.bolt
+-rw-r--r--   0        0        0      637 2023-05-31 18:08:15.450634 crankshaft-0.2.0/crankshaft/modules/events/on_player_inventory_change.bolt
+-rw-r--r--   0        0        0      577 2023-05-31 18:08:15.450634 crankshaft-0.2.0/crankshaft/modules/events/on_player_join.bolt
+-rw-r--r--   0        0        0      585 2023-05-31 18:08:15.450634 crankshaft-0.2.0/crankshaft/modules/events/on_player_jump.bolt
+-rw-r--r--   0        0        0      686 2023-05-31 18:08:15.450634 crankshaft-0.2.0/crankshaft/modules/events/on_player_land.bolt
+-rw-r--r--   0        0        0      411 2023-05-31 18:08:15.450634 crankshaft-0.2.0/crankshaft/modules/events/on_player_load.bolt
+-rw-r--r--   0        0        0      597 2023-05-31 18:08:15.450634 crankshaft-0.2.0/crankshaft/modules/events/on_player_shoot_bow.bolt
+-rw-r--r--   0        0        0      349 2023-05-31 18:08:15.450634 crankshaft-0.2.0/crankshaft/modules/events/on_player_sneak.bolt
+-rw-r--r--   0        0        0      674 2023-05-31 18:08:15.450634 crankshaft-0.2.0/crankshaft/modules/events/on_player_sneak_end.bolt
+-rw-r--r--   0        0        0      675 2023-05-31 18:08:15.450634 crankshaft-0.2.0/crankshaft/modules/events/on_player_sneak_start.bolt
+-rw-r--r--   0        0        0      354 2023-05-31 18:08:15.450634 crankshaft-0.2.0/crankshaft/modules/events/on_player_sprint.bolt
+-rw-r--r--   0        0        0      679 2023-05-31 18:08:15.450634 crankshaft-0.2.0/crankshaft/modules/events/on_player_sprint_end.bolt
+-rw-r--r--   0        0        0      680 2023-05-31 18:08:15.450634 crankshaft-0.2.0/crankshaft/modules/events/on_player_sprint_start.bolt
+-rw-r--r--   0        0        0      347 2023-05-31 18:08:15.450634 crankshaft-0.2.0/crankshaft/modules/events/on_player_swim.bolt
+-rw-r--r--   0        0        0      672 2023-05-31 18:08:15.450634 crankshaft-0.2.0/crankshaft/modules/events/on_player_swim_end.bolt
+-rw-r--r--   0        0        0      673 2023-05-31 18:08:15.450634 crankshaft-0.2.0/crankshaft/modules/events/on_player_swim_start.bolt
+-rw-r--r--   0        0        0      271 2023-05-31 18:08:15.450634 crankshaft-0.2.0/crankshaft/modules/events/on_player_tick.bolt
+-rw-r--r--   0        0        0      537 2023-05-31 18:08:15.450634 crankshaft-0.2.0/crankshaft/modules/events/on_player_use_coas.bolt
+-rw-r--r--   0        0        0      258 2023-05-31 18:08:15.450634 crankshaft-0.2.0/crankshaft/modules/events/on_tick.bolt
+-rw-r--r--   0        0        0     2007 2023-05-31 18:08:15.450634 crankshaft-0.2.0/crankshaft/modules/events.bolt
+-rw-r--r--   0        0        0     3722 2023-05-31 18:08:15.450634 crankshaft-0.2.0/crankshaft/modules/flag.bolt
+-rw-r--r--   0        0        0      377 2023-05-31 18:08:15.450634 crankshaft-0.2.0/crankshaft/modules/flags/is_airborne.bolt
+-rw-r--r--   0        0        0      402 2023-05-31 18:08:15.450634 crankshaft-0.2.0/crankshaft/modules/flags/is_baby.bolt
+-rw-r--r--   0        0        0      411 2023-05-31 18:08:15.450634 crankshaft-0.2.0/crankshaft/modules/flags/is_burning.bolt
+-rw-r--r--   0        0        0     1248 2023-05-31 18:08:15.450634 crankshaft-0.2.0/crankshaft/modules/flags/is_charging_bow.bolt
+-rw-r--r--   0        0        0      377 2023-05-31 18:08:15.450634 crankshaft-0.2.0/crankshaft/modules/flags/is_gliding.bolt
+-rw-r--r--   0        0        0      379 2023-05-31 18:08:15.450634 crankshaft-0.2.0/crankshaft/modules/flags/is_on_ground.bolt
+-rw-r--r--   0        0        0      158 2023-05-31 18:08:15.450634 crankshaft-0.2.0/crankshaft/modules/flags/is_player.bolt
+-rw-r--r--   0        0        0      414 2023-05-31 18:08:15.450634 crankshaft-0.2.0/crankshaft/modules/flags/is_sneaking.bolt
+-rw-r--r--   0        0        0      417 2023-05-31 18:08:15.450634 crankshaft-0.2.0/crankshaft/modules/flags/is_sprinting.bolt
+-rw-r--r--   0        0        0      414 2023-05-31 18:08:15.450634 crankshaft-0.2.0/crankshaft/modules/flags/is_swimming.bolt
+-rw-r--r--   0        0        0      489 2023-05-31 18:08:15.450634 crankshaft-0.2.0/crankshaft/modules/flags.bolt
+-rw-r--r--   0        0        0      407 2023-05-31 18:08:15.450634 crankshaft-0.2.0/crankshaft/modules/lib/entity_hit_matching/api.bolt
+-rw-r--r--   0        0        0      124 2023-05-31 18:08:15.450634 crankshaft-0.2.0/crankshaft/modules/lib/entity_hit_matching/credits.txt
+-rw-r--r--   0        0        0    58208 2023-05-31 18:08:15.450634 crankshaft-0.2.0/crankshaft/modules/lib/entity_hit_matching/main.bolt
+-rw-r--r--   0        0        0      207 2023-05-31 18:08:15.450634 crankshaft-0.2.0/crankshaft/modules/utils.bolt
+-rw-r--r--   0        0        0        0 2023-05-31 18:08:15.450634 crankshaft-0.2.0/crankshaft/py.typed
+-rw-r--r--   0        0        0     1260 2023-05-31 18:09:24.311467 crankshaft-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1106 1970-01-01 00:00:00.000000 crankshaft-0.2.0/PKG-INFO
```

### Comparing `crankshaft-0.1.1/LICENSE` & `crankshaft-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `crankshaft-0.1.1/crankshaft/modules/defer.bolt` & `crankshaft-0.2.0/crankshaft/modules/defer.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.1.1/crankshaft/modules/event_handler.bolt` & `crankshaft-0.2.0/crankshaft/modules/event_handler.bolt`

 * *Files 14% similar despite different names*

```diff
@@ -15,20 +15,26 @@
     def __post_init__(self):
         local_dir = f"{Config.ROOT_LOCAL}/event_handler/builtin/{self.event_id}"
         global_dir = f"{Config.ROOT}/event_handler/builtin/{self.event_id}"
 
         self.handler_dir = f"{global_dir}/__handler__"
         self.payload_path = f"{local_dir}/__payload__"
         self.fork_path = f"{global_dir}/__fork__"
+        self.bypass_fork_path = f"{local_dir}/__bypass_fork__"
+        self.bypass_fork_tag_path = f"{global_dir}/__bypass_fork_tag__"
+        self.trigger_path = f"{global_dir}/__trigger__"
 
     def trigger(self, *params):
         """Triggers the event on runtime."""
 
         self.payload_params = params
-        function f"#{self.fork_path}"
+        
+        execute function self.trigger_path:
+            function f"#{self.bypass_fork_tag_path}"       # bypass_fork multipack compatibility
+            function f"#{self.fork_path}"
 
     def activate(self):
         """Activates and deploys the handler into the datapack."""
 
         if self.active:
             return
 
@@ -37,16 +43,24 @@
         self.active = True
 
     def path(self, subpath: str) -> str:
         """Generates a function path inside the event working directory."""
 
         return f"{self.handler_dir}/{subpath}"
 
-    def attach_payload(self, payload_ref: Callable):
-        append function self.payload_path:
+    def attach_payload(self, payload_ref: Callable, bypass_fork=False):
+        path = self.payload_path
+
+        if bypass_fork:
+            # hacky fix for multipack compatibility
+            # redirects the payload making it only run once globally
+            merge function_tag self.bypass_fork_tag_path {"values": [self.bypass_fork_path]}
+            path = self.bypass_fork_path
+
+        append function path:
             payload_ref(*self.payload_params)
 
     def _fork_to_payload(self):
         merge function_tag self.fork_path {"values": [self.payload_path]}
 
 @dataclass
 class CustomEvent:
@@ -86,15 +100,19 @@
 
     @classmethod
     def _get_next_id(cls) -> int:
         index = cls.next_id
         cls.next_id += 1
         return index
 
-
 @dataclass
 class Listener:
     event: Event
+    bypass_fork: bool = field(kw_only=True, default=False)
 
     def __call__(self, callback):
         self.event.activate()
-        self.event.attach_payload(callback)
+
+        if isinstance(self.event, Event):
+            self.event.attach_payload(callback, bypass_fork=self.bypass_fork)
+        else:
+            self.event.attach_payload(callback)
```

### Comparing `crankshaft-0.1.1/crankshaft/modules/events/on_entity_attack_player.bolt` & `crankshaft-0.2.0/crankshaft/modules/events/on_entity_attack_player.bolt`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 from ../utils import selector
 
 
 def handler(event):
     has_owner = StaticVar(Bool)
     attacker_tag = f"{Config.TAG_ROOT}.event_handler.{event.event_id}.attacker"
     child_tag = f"{Config.TAG_ROOT}.event_handler.{event.event_id}.child"
-    attacker = selector(f"@e[tag={attacker_tag}]")
-    child = selector(f"@e[tag={child_tag}]")
+    attacker = selector(f"@e[tag={attacker_tag}, limit=1]")
+    child = selector(f"@e[tag={child_tag}, limit=1]")
     entrypoint = event.path('entrypoint')
 
     append_player_trigger(entrypoint)
     function entrypoint:
         as @e if score @s reapermc.crankshaft.lib.ehm.id = $direct reapermc.crankshaft.lib.ehm.id function event.path('nested_0'):
             with has_owner.store(mode='success'):
                 this.Owner.get()
```

### Comparing `crankshaft-0.1.1/crankshaft/modules/events/on_player_airborne_end.bolt` & `crankshaft-0.2.0/crankshaft/modules/events/on_player_airborne_end.bolt`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from ../config import Config
 from ../flags/is_airborne import is_airborne
 
 
 def handler(event):
     event_fired_tag = f"{Config.TAG_ROOT}.event_handler.{event.event_id}"
 
-    @Listener(on_player_tick)
+    @Listener(on_player_tick, bypass_fork=True)
     def player_tick():
         if not is_airborne:
             if entity @s[tag=event_fired_tag] function event.path('nest_0'):
                 untag(event_fired_tag)
                 event.trigger()
         else:
             tag(event_fired_tag)
```

### Comparing `crankshaft-0.1.1/crankshaft/modules/events/on_player_airborne_start.bolt` & `crankshaft-0.2.0/crankshaft/modules/events/on_player_sprint_start.bolt`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from lightning_rod:api import tag, untag
 from ../event_handler import Event, Listener
 from ./on_player_tick import on_player_tick
 from ../config import Config
-from ../flags/is_airborne import is_airborne
+from ../flags/is_sprinting import is_sprinting 
 
 
 def handler(event):
     event_fired_tag = f"{Config.TAG_ROOT}.event_handler.{event.event_id}"
 
-    @Listener(on_player_tick)
+    @Listener(on_player_tick, bypass_fork=True)
     def player_tick():
-        if is_airborne:
+        if is_sprinting:
             if entity @s[tag=!event_fired_tag] function event.path('nest_0'):
                 tag(event_fired_tag)
                 event.trigger()
         else:
             untag(event_fired_tag)
 
-on_player_airborne_start = Event(handler=handler, event_id='on_player_airborne_start')
+on_player_sprint_start = Event(handler=handler, event_id='on_player_sprint_start')
```

### Comparing `crankshaft-0.1.1/crankshaft/modules/events/on_player_attack_entity.bolt` & `crankshaft-0.2.0/crankshaft/modules/events/on_player_attack_entity.bolt`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 from ../config import Config
 
 
 def handler(event):
     has_owner = StaticVar(Bool)
     attacker_tag = f"{Config.TAG_ROOT}.event_handler.{event.event_id}.attacker"
     child_tag = f"{Config.TAG_ROOT}.event_handler.{event.event_id}.child"
-    attacker = selector(f"@e[tag={attacker_tag}]")
-    child = selector(f"@e[tag={child_tag}]")
+    attacker = selector(f"@a[tag={attacker_tag}, limit=1]")
+    child = selector(f"@e[tag={child_tag}, limit=1]")
     entrypoint = event.path('entrypoint')
 
     append_target_trigger(entrypoint)
     function entrypoint:
         as @e if score @s reapermc.crankshaft.lib.ehm.id = $direct reapermc.crankshaft.lib.ehm.id function event.path('nested_0'):
             with has_owner.store(mode='success'):
                 this.Owner.get()
```

### Comparing `crankshaft-0.1.1/crankshaft/modules/events/on_player_burn_end.bolt` & `crankshaft-0.2.0/crankshaft/modules/events/on_player_burn_start.bolt`

 * *Files 6% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 from ../config import Config
 from ../flags/is_burning import is_burning
 
 
 def handler(event):
     event_fired_tag = f"{Config.TAG_ROOT}.event_handler.{event.event_id}"
 
-    @Listener(on_player_tick)
+    @Listener(on_player_tick, bypass_fork=True)
     def player_tick():
-        if not is_burning:
-            if entity @s[tag=event_fired_tag] function event.path('nest_0'):
-                untag(event_fired_tag)
+        if is_burning:
+            if entity @s[tag=!event_fired_tag] function event.path('nest_0'):
+                tag(event_fired_tag)
                 event.trigger()
         else:
-            tag(event_fired_tag)
+            untag(event_fired_tag)
 
-on_player_burn_end = Event(handler=handler, event_id='on_player_burn_end')
+on_player_burn_start = Event(handler=handler, event_id='on_player_burn_start')
```

### Comparing `crankshaft-0.1.1/crankshaft/modules/events/on_player_burn_start.bolt` & `crankshaft-0.2.0/crankshaft/modules/events/on_player_land.bolt`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from lightning_rod:api import tag, untag
 from ../event_handler import Event, Listener
 from ./on_player_tick import on_player_tick
 from ../config import Config
-from ../flags/is_burning import is_burning
+from ../flags/is_airborne import is_airborne
 
 
 def handler(event):
-    event_fired_tag = f"{Config.TAG_ROOT}.event_handler.{event.event_id}"
-
-    @Listener(on_player_tick)
+    @Listener(on_player_tick, bypass_fork=True)
     def player_tick():
-        if is_burning:
-            if entity @s[tag=!event_fired_tag] function event.path('nest_0'):
-                tag(event_fired_tag)
-                event.trigger()
+        available_tag = f"{Config.TAG_ROOT}.event_handler.{event.event_id}"
+
+        if is_airborne:
+            tag(available_tag)
         else:
-            untag(event_fired_tag)
+            if entity @s[tag=available_tag]:
+                execute function event.path('main'):
+                    untag(available_tag)
+                    event.trigger()
 
-on_player_burn_start = Event(handler=handler, event_id='on_player_burn_start')
+on_player_land = Event(handler=handler, event_id='on_player_land')
```

### Comparing `crankshaft-0.1.1/crankshaft/modules/events/on_player_charge_bow_end.bolt` & `crankshaft-0.2.0/crankshaft/modules/events/on_player_charge_bow_end.bolt`

 * *Files 15% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from ./on_player_charge_bow import on_player_charge_bow
 from ./on_player_tick import on_player_tick
 
 
 def handler(event):
     event_fired_tag = f"{Config.TAG_ROOT}.event_handler.{event.event_id}"
 
-    @Listener(on_player_tick)
+    @Listener(on_player_tick, bypass_fork=True)
     def player_tick():
         if not is_charging_bow:
             if entity @s[tag=event_fired_tag] function event.path('nest_0'):
                 untag(event_fired_tag)
                 event.trigger()
         else:
             tag(event_fired_tag)
```

### Comparing `crankshaft-0.1.1/crankshaft/modules/events/on_player_charge_bow_start.bolt` & `crankshaft-0.2.0/crankshaft/modules/events/on_player_charge_bow_start.bolt`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from ./on_player_charge_bow import on_player_charge_bow
 from ./on_player_tick import on_player_tick
 
 
 def handler(event):
     event_fired_tag = f"{Config.TAG_ROOT}.event_handler.{event.event_id}"
 
-    @Listener(on_player_tick)
+    @Listener(on_player_tick, bypass_fork=True)
     def player_tick():
         if is_charging_bow:
             if entity @s[tag=!event_fired_tag] function event.path('nest_0'):
                 tag(event_fired_tag)
                 event.trigger()
         else:
             untag(event_fired_tag)
```

### Comparing `crankshaft-0.1.1/crankshaft/modules/events/on_player_glide_end.bolt` & `crankshaft-0.2.0/crankshaft/modules/events/on_player_sprint_end.bolt`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from lightning_rod:api import tag, untag
 from ../event_handler import Event, Listener
 from ./on_player_tick import on_player_tick
 from ../config import Config
-from ../flags/is_gliding import is_gliding 
+from ../flags/is_sprinting import is_sprinting 
 
 
 def handler(event):
     event_fired_tag = f"{Config.TAG_ROOT}.event_handler.{event.event_id}"
 
-    @Listener(on_player_tick)
+    @Listener(on_player_tick, bypass_fork=True)
     def player_tick():
-        if not is_gliding:
+        if not is_sprinting:
             if entity @s[tag=event_fired_tag] function event.path('nest_0'):
                 untag(event_fired_tag)
                 event.trigger()
         else:
             tag(event_fired_tag)
 
-on_player_glide_end = Event(handler=handler, event_id='on_player_glide_end')
+on_player_sprint_end = Event(handler=handler, event_id='on_player_sprint_end')
```

### Comparing `crankshaft-0.1.1/crankshaft/modules/events/on_player_glide_start.bolt` & `crankshaft-0.2.0/crankshaft/modules/events/on_player_glide_start.bolt`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from ../config import Config
 from ../flags/is_gliding import is_gliding 
 
 
 def handler(event):
     event_fired_tag = f"{Config.TAG_ROOT}.event_handler.{event.event_id}"
 
-    @Listener(on_player_tick)
+    @Listener(on_player_tick, bypass_fork=True)
     def player_tick():
         if is_gliding:
             if entity @s[tag=!event_fired_tag] function event.path('nest_0'):
                 tag(event_fired_tag)
                 event.trigger()
         else:
             untag(event_fired_tag)
```

### Comparing `crankshaft-0.1.1/crankshaft/modules/events/on_player_inventory_change.bolt` & `crankshaft-0.2.0/crankshaft/modules/events/on_player_inventory_change.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.1.1/crankshaft/modules/events/on_player_join.bolt` & `crankshaft-0.2.0/crankshaft/modules/events/on_player_jump.bolt`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from wicked_expressions:api import Scoreboard
 from ../event_handler import Event, Listener
 from ../config import Config
 from ./on_player_tick import on_player_tick
 
 
 def handler(event):
-    @Listener(on_player_tick)
+    @Listener(on_player_tick, bypass_fork=True)
     def player_tick():
-        join_tracker = Scoreboard(f"{Config.SCOREBOARD_ROOT}.{event.event_id}", 'custom:leave_game')['@s']
+        jump_tracker = Scoreboard(f"{Config.SCOREBOARD_ROOT}.event_handler.{event.event_id}", 'custom:jump')['@s']
 
-        if join_tracker >= 1:
+        if jump_tracker >= 1:
             execute function event.path('main'):
-                join_tracker = 0
+                jump_tracker = 0
                 event.trigger()
 
-on_player_join = Event(handler=handler, event_id='on_player_join')
+on_player_jump = Event(handler=handler, event_id='on_player_jump')
```

### Comparing `crankshaft-0.1.1/crankshaft/modules/events/on_player_jump.bolt` & `crankshaft-0.2.0/crankshaft/modules/events/on_player_glide_end.bolt`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,20 @@
-from wicked_expressions:api import Scoreboard
+from lightning_rod:api import tag, untag
 from ../event_handler import Event, Listener
-from ../config import Config
 from ./on_player_tick import on_player_tick
+from ../config import Config
+from ../flags/is_gliding import is_gliding 
 
 
 def handler(event):
-    @Listener(on_player_tick)
-    def player_tick():
-        jump_tracker = Scoreboard(f"{Config.SCOREBOARD_ROOT}.event_handler.{event.event_id}", 'custom:jump')['@s']
+    event_fired_tag = f"{Config.TAG_ROOT}.event_handler.{event.event_id}"
 
-        if jump_tracker >= 1:
-            execute function event.path('main'):
-                jump_tracker = 0
+    @Listener(on_player_tick, bypass_fork=True)
+    def player_tick():
+        if not is_gliding:
+            if entity @s[tag=event_fired_tag] function event.path('nest_0'):
+                untag(event_fired_tag)
                 event.trigger()
+        else:
+            tag(event_fired_tag)
 
-on_player_jump = Event(handler=handler, event_id='on_player_jump')
+on_player_glide_end = Event(handler=handler, event_id='on_player_glide_end')
```

### Comparing `crankshaft-0.1.1/crankshaft/modules/events/on_player_land.bolt` & `crankshaft-0.2.0/crankshaft/modules/events/on_player_shoot_bow.bolt`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,17 @@
-from lightning_rod:api import tag, untag
+from wicked_expressions:api import Scoreboard
 from ../event_handler import Event, Listener
-from ./on_player_tick import on_player_tick
 from ../config import Config
-from ../flags/is_airborne import is_airborne
+from ./on_player_tick import on_player_tick
 
 
 def handler(event):
-    @Listener(on_player_tick)
+    @Listener(on_player_tick, bypass_fork=True)
     def player_tick():
-        available_tag = f"{Config.TAG_ROOT}.event_handler.{event.event_id}"
+        shoot_tracker = Scoreboard(f"{Config.SCOREBOARD_ROOT}.event_handler.{event.event_id}", 'used:bow')['@s']
 
-        if is_airborne:
-            tag(available_tag)
-        else:
-            if entity @s[tag=available_tag]:
-                execute function event.path('main'):
-                    untag(available_tag)
-                    event.trigger()
+        if shoot_tracker >= 1:
+            execute function event.path('nest_0'):
+                shoot_tracker = 0
+                event.trigger()
 
-on_player_land = Event(handler=handler, event_id='on_player_land')
+on_player_shoot_bow = Event(handler=handler, event_id='on_player_shoot_bow')
```

### Comparing `crankshaft-0.1.1/crankshaft/modules/events/on_player_shoot_bow.bolt` & `crankshaft-0.2.0/crankshaft/modules/events/on_player_airborne_start.bolt`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,20 @@
-from wicked_expressions:api import Scoreboard
+from lightning_rod:api import tag, untag
 from ../event_handler import Event, Listener
-from ../config import Config
 from ./on_player_tick import on_player_tick
+from ../config import Config
+from ../flags/is_airborne import is_airborne
 
 
 def handler(event):
-    @Listener(on_player_tick)
-    def player_tick():
-        shoot_tracker = Scoreboard(f"{Config.SCOREBOARD_ROOT}.event_handler.{event.event_id}", 'used:bow')['@s']
+    event_fired_tag = f"{Config.TAG_ROOT}.event_handler.{event.event_id}"
 
-        if shoot_tracker >= 1:
-            shoot_tracker = 0
-            event.trigger()
+    @Listener(on_player_tick, bypass_fork=True)
+    def player_tick():
+        if is_airborne:
+            if entity @s[tag=!event_fired_tag] function event.path('nest_0'):
+                tag(event_fired_tag)
+                event.trigger()
+        else:
+            untag(event_fired_tag)
 
-on_player_shoot_bow = Event(handler=handler, event_id='on_player_shoot_bow')
+on_player_airborne_start = Event(handler=handler, event_id='on_player_airborne_start')
```

### Comparing `crankshaft-0.1.1/crankshaft/modules/events/on_player_sneak_end.bolt` & `crankshaft-0.2.0/crankshaft/modules/events/on_player_sneak_start.bolt`

 * *Files 14% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 from ../config import Config
 from ../flags/is_sneaking import is_sneaking 
 
 
 def handler(event):
     event_fired_tag = f"{Config.TAG_ROOT}.event_handler.{event.event_id}"
 
-    @Listener(on_player_tick)
+    @Listener(on_player_tick, bypass_fork=True)
     def player_tick():
-        if not is_sneaking:
-            if entity @s[tag=event_fired_tag] function event.path('nest_0'):
-                untag(event_fired_tag)
+        if is_sneaking:
+            if entity @s[tag=!event_fired_tag] function event.path('nest_0'):
+                tag(event_fired_tag)
                 event.trigger()
         else:
-            tag(event_fired_tag)
+            untag(event_fired_tag)
 
-on_player_sneak_end = Event(handler=handler, event_id='on_player_sneak_end')
+on_player_sneak_start = Event(handler=handler, event_id='on_player_sneak_start')
```

### Comparing `crankshaft-0.1.1/crankshaft/modules/events/on_player_sneak_start.bolt` & `crankshaft-0.2.0/crankshaft/modules/events/on_player_burn_end.bolt`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from lightning_rod:api import tag, untag
 from ../event_handler import Event, Listener
 from ./on_player_tick import on_player_tick
 from ../config import Config
-from ../flags/is_sneaking import is_sneaking 
+from ../flags/is_burning import is_burning
 
 
 def handler(event):
     event_fired_tag = f"{Config.TAG_ROOT}.event_handler.{event.event_id}"
 
-    @Listener(on_player_tick)
+    @Listener(on_player_tick, bypass_fork=True)
     def player_tick():
-        if is_sneaking:
-            if entity @s[tag=!event_fired_tag] function event.path('nest_0'):
-                tag(event_fired_tag)
+        if not is_burning:
+            if entity @s[tag=event_fired_tag] function event.path('nest_0'):
+                untag(event_fired_tag)
                 event.trigger()
         else:
-            untag(event_fired_tag)
+            tag(event_fired_tag)
 
-on_player_sneak_start = Event(handler=handler, event_id='on_player_sneak_start')
+on_player_burn_end = Event(handler=handler, event_id='on_player_burn_end')
```

### Comparing `crankshaft-0.1.1/crankshaft/modules/events/on_player_sprint_end.bolt` & `crankshaft-0.2.0/crankshaft/modules/events/on_player_sneak_end.bolt`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from lightning_rod:api import tag, untag
 from ../event_handler import Event, Listener
 from ./on_player_tick import on_player_tick
 from ../config import Config
-from ../flags/is_sprinting import is_sprinting 
+from ../flags/is_sneaking import is_sneaking 
 
 
 def handler(event):
     event_fired_tag = f"{Config.TAG_ROOT}.event_handler.{event.event_id}"
 
-    @Listener(on_player_tick)
+    @Listener(on_player_tick, bypass_fork=True)
     def player_tick():
-        if not is_sprinting:
+        if not is_sneaking:
             if entity @s[tag=event_fired_tag] function event.path('nest_0'):
                 untag(event_fired_tag)
                 event.trigger()
         else:
             tag(event_fired_tag)
 
-on_player_sprint_end = Event(handler=handler, event_id='on_player_sprint_end')
+on_player_sneak_end = Event(handler=handler, event_id='on_player_sneak_end')
```

### Comparing `crankshaft-0.1.1/crankshaft/modules/events/on_player_sprint_start.bolt` & `crankshaft-0.2.0/crankshaft/modules/events/on_player_swim_start.bolt`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from lightning_rod:api import tag, untag
 from ../event_handler import Event, Listener
 from ./on_player_tick import on_player_tick
 from ../config import Config
-from ../flags/is_sprinting import is_sprinting 
+from ../flags/is_swimming import is_swimming 
 
 
 def handler(event):
     event_fired_tag = f"{Config.TAG_ROOT}.event_handler.{event.event_id}"
 
-    @Listener(on_player_tick)
+    @Listener(on_player_tick, bypass_fork=True)
     def player_tick():
-        if is_sprinting:
+        if is_swimming:
             if entity @s[tag=!event_fired_tag] function event.path('nest_0'):
                 tag(event_fired_tag)
                 event.trigger()
         else:
             untag(event_fired_tag)
 
-on_player_sprint_start = Event(handler=handler, event_id='on_player_sprint_start')
+on_player_swim_start = Event(handler=handler, event_id='on_player_swim_start')
```

### Comparing `crankshaft-0.1.1/crankshaft/modules/events/on_player_swim_end.bolt` & `crankshaft-0.2.0/crankshaft/modules/events/on_player_swim_end.bolt`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from ../config import Config
 from ../flags/is_swimming import is_swimming 
 
 
 def handler(event):
     event_fired_tag = f"{Config.TAG_ROOT}.event_handler.{event.event_id}"
 
-    @Listener(on_player_tick)
+    @Listener(on_player_tick, bypass_fork=True)
     def player_tick():
         if not is_swimming:
             if entity @s[tag=event_fired_tag] function event.path('nest_0'):
                 untag(event_fired_tag)
                 event.trigger()
         else:
             tag(event_fired_tag)
```

### Comparing `crankshaft-0.1.1/crankshaft/modules/events.bolt` & `crankshaft-0.2.0/crankshaft/modules/events.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.1.1/crankshaft/modules/flag.bolt` & `crankshaft-0.2.0/crankshaft/modules/flag.bolt`

 * *Files 6% similar despite different names*

```diff
@@ -9,18 +9,20 @@
 @dataclass
 class Flag:
     body: Callable = field(kw_only=True, repr=False)
     flag_id: str = field(kw_only=True)
 
     invert: bool = field(kw_only=True, default=False)
     initialized: bool = field(kw_only=True, default=False)
-    gate: ClassVar[ExpressionNode] = StaticVar(Bool)
-    active: bool = field(init=False, default=False)
+    active: bool = field(default=False)
+    # gate: ClassVar[ExpressionNode] = StaticVar(Bool)
 
     def __post_init__(self):
+        self.gate = StaticVar(Bool)
+
         local_dir = f"{Config.ROOT_LOCAL}/flag/builtin/{self.flag_id}"
         global_dir = f"{Config.ROOT}/flag/builtin/{self.flag_id}"
 
         self.root_dir = f"{global_dir}/__root__"
         self.condition_path = f"{global_dir}/__condition__"
 
     @contextmanager
@@ -35,15 +37,15 @@
             if self.gate == 1:
                 yield True
         else:
             if self.gate == 0:
                 yield True
 
     def __not__(self):
-        return self.__class__(body=self.body, flag_id=self.flag_id, invert=not self.invert, initialized=self.initialized)
+        return self.__class__(body=self.body, flag_id=self.flag_id, invert=not self.invert, initialized=self.initialized, active=self.active)
 
     @contextmanager
     def set_condition(self):
         """Use along the 'with' statement to set the flag condition."""
 
         function self.condition_path:
             with self.gate.store(mode='success'):
@@ -64,21 +66,21 @@
         self.body(self)
         self.active = True
 
 @dataclass
 class CustomFlag:
     body: Callable = field(kw_only=True, repr=False)
 
-    gate: ClassVar[ExpressionNode] = StaticVar(Bool)
-    active: bool = field(init=False, default=False)
     invert: bool = field(kw_only=True, default=False)
     initialized: bool = field(kw_only=True, default=False)
+    active: bool = field(default=False)
     next_id: ClassVar[int] = 0
 
     def __post_init__(self):
+        self.gate = StaticVar(Bool)
         self.flag_id = f"{self._get_next_id()}__{ctx.project_id}"
 
         local_dir = f"{Config.ROOT_LOCAL}/flag/custom/{self.flag_id}"
 
         self.root_dir = f"{local_dir}/__root__"
         self.condition_path = f"{local_dir}/__condition__"
 
@@ -94,15 +96,15 @@
             if self.gate == 1:
                 yield True
         else:
             if self.gate == 0:
                 yield True
 
     def __not__(self):
-        return self.__class__(body=self.body, invert=not self.invert, initialized=self.initialized)
+        return self.__class__(body=self.body, invert=not self.invert, initialized=self.initialized, active=self.active)
 
     @contextmanager
     def set_condition(self):
         """Use along the 'with' statement to set the flag condition."""
 
         function self.condition_path:
             with self.gate.store(mode='success'):
```

### Comparing `crankshaft-0.1.1/crankshaft/modules/flags/is_charging_bow.bolt` & `crankshaft-0.2.0/crankshaft/modules/flags/is_charging_bow.bolt`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 def body(flag):
     is_charging = Scoreboard(f"{Config.SCOREBOARD_ROOT}.flag.{flag.flag_id}")['@s']
     advancement_path = flag.path('advancement')
     reward_path = flag.path('advancement_reward')
 
-    @Listener(on_player_tick)
+    @Listener(on_player_tick, bypass_fork=True)
     def player_tick():
         nonlocal is_charging
 
         is_charging -= 1
 
     advancement advancement_path {
         "criteria": {
```

### Comparing `crankshaft-0.1.1/crankshaft/modules/lib/entity_hit_matching/main.bolt` & `crankshaft-0.2.0/crankshaft/modules/lib/entity_hit_matching/main.bolt`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         "minecraft:chest_minecart",
         "minecraft:chest_boat",
         "minecraft:marker"
     ]
 }
 
 
-@Listener(on_load)
+@Listener(on_load, bypass_fork=True)
 def load():
 	execute function f"{ROOT_DIR}/load":
 		# This objective tracks IDs, along with variables and constants
 		scoreboard objectives add f"{ROOT_GENERIC}.id" dummy
 		scoreboard players set #3 f"{ROOT_GENERIC}.id" 3
 
 		# These objectives track the individual bits of IDs
@@ -59,15 +59,15 @@
 		scoreboard objectives add f"{ROOT_GENERIC}.id.4" dummy
 		scoreboard objectives add f"{ROOT_GENERIC}.id.5" dummy
 		scoreboard objectives add f"{ROOT_GENERIC}.id.6" dummy
 		scoreboard objectives add f"{ROOT_GENERIC}.id.7" dummy
 		scoreboard objectives add f"{ROOT_GENERIC}.id.8" dummy
 #
 
-@Listener(on_tick)
+@Listener(on_tick, bypass_fork=True)
 def tick():
 	execute function f"{ROOT_DIR}/tick":
 		# Assigns IDs to the entities that need them
 		execute as @e unless score @s f"{ROOT_GENERIC}.id" = @s f"{ROOT_GENERIC}.id" run function f"{ROOT_DIR}/id/filter"
 #
 
 function f"{ROOT_DIR}/id/assign":
```

### Comparing `crankshaft-0.1.1/pyproject.toml` & `crankshaft-0.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "crankshaft"
-version = "0.1.1"
+version = "0.2.0"
 description = "Flow control library for the Bolt scripting language."
 authors = ["ArcticYeti <arcticyeti1@gmail.com>"]
 license = "MIT"
 
 homepage = "https://github.com/reapermc/crankshaft"
 readme = "README.md"
```

### Comparing `crankshaft-0.1.1/PKG-INFO` & `crankshaft-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crankshaft
-Version: 0.1.1
+Version: 0.2.0
 Summary: Flow control library for the Bolt scripting language.
 Home-page: https://github.com/reapermc/crankshaft
 License: MIT
 Keywords: beet,bolt,minecraft,datapack,minecraft-commands,mcfunction,library,reapermc
 Author: ArcticYeti
 Author-email: arcticyeti1@gmail.com
 Requires-Python: >=3.10,<4.0
```

