# Comparing `tmp/greeneye_monitor-3.0.3-py3-none-any.whl.zip` & `tmp/greeneye_monitor-4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 9950 bytes, number of entries: 10
--rw-r--r--  2.0 unx       30 b- defN 21-Nov-02 04:40 greeneye/__init__.py
--rw-r--r--  2.0 unx     5124 b- defN 22-Jan-06 07:16 greeneye/api.py
--rw-r--r--  2.0 unx    19765 b- defN 22-Feb-21 03:21 greeneye/monitor.py
--rw-r--r--  2.0 unx      325 b- defN 22-Jan-04 05:27 greeneye/protocol.py
--rw-r--r--  2.0 unx        0 b- defN 22-Jan-06 05:32 greeneye/py.typed
--rw-r--r--  2.0 unx     1296 b- defN 22-Feb-21 03:22 greeneye_monitor-3.0.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     2865 b- defN 22-Feb-21 03:22 greeneye_monitor-3.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Feb-21 03:22 greeneye_monitor-3.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 22-Feb-21 03:22 greeneye_monitor-3.0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      801 b- defN 22-Feb-21 03:22 greeneye_monitor-3.0.3.dist-info/RECORD
-10 files, 30307 bytes uncompressed, 8578 bytes compressed:  71.7%
+Zip file size: 12142 bytes, number of entries: 10
+-rw-r--r--  2.0 unx       30 b- defN 22-May-27 16:30 greeneye/__init__.py
+-rw-r--r--  2.0 unx     9130 b- defN 23-May-20 00:16 greeneye/api.py
+-rw-r--r--  2.0 unx    29242 b- defN 23-May-30 18:20 greeneye/monitor.py
+-rw-r--r--  2.0 unx      325 b- defN 23-May-15 16:41 greeneye/protocol.py
+-rw-r--r--  2.0 unx        0 b- defN 22-May-27 16:30 greeneye/py.typed
+-rw-r--r--  2.0 unx     1296 b- defN 23-May-30 22:25 greeneye_monitor-4.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2851 b- defN 23-May-30 22:25 greeneye_monitor-4.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-30 22:25 greeneye_monitor-4.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-May-30 22:25 greeneye_monitor-4.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      791 b- defN 23-May-30 22:25 greeneye_monitor-4.0.dist-info/RECORD
+10 files, 43766 bytes uncompressed, 10790 bytes compressed:  75.3%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: greeneye/protocol.py
 Comment: 
 
 Filename: greeneye/py.typed
 Comment: 
 
-Filename: greeneye_monitor-3.0.3.dist-info/LICENSE
+Filename: greeneye_monitor-4.0.dist-info/LICENSE
 Comment: 
 
-Filename: greeneye_monitor-3.0.3.dist-info/METADATA
+Filename: greeneye_monitor-4.0.dist-info/METADATA
 Comment: 
 
-Filename: greeneye_monitor-3.0.3.dist-info/WHEEL
+Filename: greeneye_monitor-4.0.dist-info/WHEEL
 Comment: 
 
-Filename: greeneye_monitor-3.0.3.dist-info/top_level.txt
+Filename: greeneye_monitor-4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: greeneye_monitor-3.0.3.dist-info/RECORD
+Filename: greeneye_monitor-4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## greeneye/api.py

```diff
@@ -1,22 +1,22 @@
 from __future__ import annotations
 
 import aiohttp
 import asyncio
 from dataclasses import dataclass
 from datetime import timedelta
 from enum import Enum, unique
+from itertools import chain
 import logging
 from typing import Any, Optional, Tuple
 from siobrultech_protocols.gem.api import (
-    ApiCall,
     call_api,
 )
 from siobrultech_protocols.gem.packets import PacketFormatType
-from siobrultech_protocols.gem.protocol import BidirectionalProtocol
+from siobrultech_protocols.gem.protocol import ApiCall, ApiType, BidirectionalProtocol
 import struct
 
 LOG = logging.getLogger(__name__)
 
 
 async def set_packet_destination(
     gem_host: str, dest_host: str, dest_port: int, session: aiohttp.ClientSession
@@ -46,29 +46,81 @@
 
 
 @dataclass(frozen=True)
 class GemSettings:
     packet_format: PacketFormatType | None
     packet_send_interval: timedelta
     num_channels: int
-    temperature_unit: TemperatureUnit
-    channel_net_metering: list[bool]
+    temperature_unit: TemperatureUnit | None
+    channel_net_metering: list[bool | None]
+    ct_types: list[int]
+    ct_ranges: list[int]
 
 
 async def get_all_settings(
-    protocol: BidirectionalProtocol, serial_number: Optional[int] = None
+    protocol: BidirectionalProtocol,
+    serial_number: Optional[int] = None,
+    timeout: timedelta | None = None,
 ) -> GemSettings:
-    async with call_api(_GET_ALL_SETTINGS, protocol, serial_number) as f:
+    async with call_api(_GET_ALL_SETTINGS, protocol, serial_number, timeout) as f:
+        return await f(None)
+
+
+async def send_one_packet(
+    protocol: BidirectionalProtocol, serial_number: Optional[int] = None
+) -> None:
+    async with call_api(_SEND_ONE_PACKET, protocol, serial_number) as f:
         return await f(None)
 
 
+async def set_ct_type(
+    protocol: BidirectionalProtocol,
+    channel: int,
+    type: int,
+    serial_number: Optional[int] = None,
+) -> None:
+    assert protocol.api_type == ApiType.GEM
+    async with call_api(_SET_CT_TYPE, protocol, serial_number) as f:
+        await f((channel, type))
+
+
+async def set_ct_range(
+    protocol: BidirectionalProtocol,
+    channel: int,
+    range: int,
+    serial_number: Optional[int] = None,
+) -> None:
+    assert protocol.api_type == ApiType.GEM
+    async with call_api(_SET_CT_RANGE, protocol, serial_number) as f:
+        await f((channel, range))
+
+
+async def set_ct_type_and_range(
+    protocol: BidirectionalProtocol,
+    channel: int,
+    type: int,
+    range: int,
+    serial_number: Optional[int] = None,
+) -> None:
+    if protocol.api_type == ApiType.GEM:
+        await set_ct_type(protocol, channel, type, serial_number)
+        await set_ct_range(protocol, channel, range, serial_number)
+    elif protocol.api_type == ApiType.ECM:
+        async with call_api(_SET_CT_TYPE_AND_RANGE, protocol, serial_number) as f:
+            await f((channel, type, range))
+    else:
+        assert False
+
+
 _ALL_SETTINGS_RESPONSE_PREFIX = "ALL\r\n"
 
 
-def _parse_all_settings(response: str) -> GemSettings:
+def _parse_all_settings(response: str) -> GemSettings | None:
+    if len(response) < 1542:
+        return None
     assert response.startswith(_ALL_SETTINGS_RESPONSE_PREFIX)
     binary = bytes.fromhex(
         response[len(_ALL_SETTINGS_RESPONSE_PREFIX) :].replace(",", "")
     )
     offset = 0
 
     def unpack(format: str | bytes) -> Tuple[Any, ...]:
@@ -80,16 +132,18 @@
         return result
 
     # Unpack all the options defined in the docs. The docs are somewhat spotty, and we only currently
     # need a few of these, so we're exposing only a few accessors.
     _channel_options = unpack("x48B")
     channel_net_metering = [options & 0x40 == 0 for options in _channel_options]
     channel_polarity_toggled = [options & 0x80 == 0x80 for options in _channel_options]
-    _ct_types = unpack("48B")
-    _ct_ranges = unpack("24B")  # These are actually one nybble per CT
+    ct_types = list(unpack("48B"))
+    ct_ranges = list(
+        chain.from_iterable([[b & 0x0F, (b & 0xF0) >> 4] for b in unpack("24B")])
+    )  # These are actually one nybble per CT
     _pt_type = unpack("B")[0]
     _pt_range = unpack("B")[0]
     _packet_format_int = unpack("B")[0]
     try:
         packet_format = PacketFormatType(_packet_format_int)
     except ValueError:
         packet_format = None
@@ -141,14 +195,101 @@
 
     return GemSettings(
         packet_format=packet_format,
         packet_send_interval=packet_send_interval,
         num_channels=num_channels,
         temperature_unit=temperature_unit,
         channel_net_metering=channel_net_metering,
+        ct_types=ct_types,
+        ct_ranges=ct_ranges,
+    )
+
+
+def _parse_all_ecm_settings(binary: bytes) -> GemSettings | None:
+    if len(binary) < 33:
+        return None
+
+    offset = 0
+
+    def unpack(format: str | bytes) -> Tuple[Any, ...]:
+        nonlocal binary
+        nonlocal offset
+        size = struct.calcsize(format)
+        result = struct.unpack_from(format, binary, offset)
+        offset += size
+        return result
+
+    actual_sum = sum(binary[:32])
+
+    ct1_type = unpack("B")[0]
+    ct1_range = unpack("B")[0]
+    ct2_type = unpack("B")[0]
+    ct2_range = unpack("B")[0]
+    ct_types = [ct1_type, ct2_type]
+    ct_ranges = [ct1_range, ct2_range]
+    _pt_type = unpack("B")[0]
+    _pt_range = unpack("B")[0]
+    packet_send_interval = timedelta(seconds=unpack("B")[0])
+    _data_logger_interval = unpack("B")[0]
+    _firmware_version = unpack(">H")[0]
+    _device_id = unpack("B")[0]
+    serial_number = unpack(">H")[0]
+    unpack("16x")
+    _trigger_value = unpack("<H")[0]
+    zero = unpack("B")[0]
+    assert zero == 0
+    checksum = unpack("B")[0]
+    assert checksum == actual_sum % 256
+
+    return GemSettings(
+        packet_format=PacketFormatType.ECM_1220,
+        packet_send_interval=packet_send_interval,
+        num_channels=2,
+        temperature_unit=None,
+        channel_net_metering=[None, None],
+        ct_types=ct_types,
+        ct_ranges=ct_ranges,
     )
 
 
 _CMD_GET_ALL_SETTINGS = "^^^RQSALL"
 _GET_ALL_SETTINGS = ApiCall[None, GemSettings](
-    formatter=lambda _: _CMD_GET_ALL_SETTINGS, parser=_parse_all_settings
+    gem_formatter=lambda _: _CMD_GET_ALL_SETTINGS,
+    gem_parser=_parse_all_settings,
+    ecm_formatter=lambda _: [b"\xfc", b"SET", b"RCV"],
+    ecm_parser=_parse_all_ecm_settings,
+)
+
+_CMD_SEND_ONE_PACKET = "^^^APISPK"
+_SEND_ONE_PACKET = ApiCall[None, None](
+    gem_formatter=lambda _: _CMD_SEND_ONE_PACKET,
+    gem_parser=None,
+    ecm_formatter=None,
+    ecm_parser=None,
+)
+
+_SET_CT_TYPE = ApiCall[(int, int), None](
+    gem_formatter=lambda args: f"^^^C{args[0]:02}TYP{args[1]}",
+    gem_parser=None,
+    ecm_formatter=None,
+    ecm_parser=None,
+)
+_SET_CT_RANGE = ApiCall[(int, int), None](
+    gem_formatter=lambda args: f"^^^C{args[0]:02}RNG{args[1]}",
+    gem_parser=None,
+    ecm_formatter=None,
+    ecm_parser=None,
+)
+_SET_CT_TYPE_AND_RANGE = ApiCall[(int, int, int), None](
+    gem_formatter=None,
+    gem_parser=None,
+    ecm_formatter=lambda args: [
+        b"\xfc",
+        b"SET",
+        f"CT{args[0]}".encode(),
+        b"TYP",
+        bytes([args[1]]),
+        b"RNG",
+        bytes([args[2]]),
+    ],
+    ecm_parser=None,
 )
```

## greeneye/monitor.py

```diff
@@ -1,84 +1,103 @@
+from enum import Enum
 import aiohttp
 import asyncio
 from asyncio.base_events import Server
 from datetime import datetime, timedelta
+from functools import wraps
+import inspect
 import logging
 import socket
 from types import TracebackType
 from typing import Awaitable, Callable, Dict, List, Optional, Tuple, Type, Union
 
 from siobrultech_protocols.gem import api
 from siobrultech_protocols.gem.packets import Packet, PacketFormatType
 from siobrultech_protocols.gem.protocol import (
+    ApiType,
     ConnectionLostMessage,
     ConnectionMadeMessage,
     PacketProtocolMessage,
     PacketReceivedMessage,
 )
 
+from . import api as api_ext
 from .api import (
     GemSettings,
     TemperatureUnit,
-    get_all_settings,
-    set_packet_destination,
 )
 from .protocol import GemProtocol
 
 LOG = logging.getLogger(__name__)
 SECONDS_PER_HOUR = 3600
 WATTS_PER_KILOWATT = 1000
 
 Listener = Union[Callable[[], Awaitable[None]], Callable[[], None]]
 
 
 class PulseCounter:
     """Represents a single GEM pulse-counting channel"""
 
-    def __init__(self, monitor: "Monitor", number: int) -> None:
+    def __init__(self, monitor: "Monitor", number: int, is_aux: bool = False) -> None:
         self._monitor = monitor
         self.number: int = number
         self.pulses: Optional[int] = None
         self.pulses_per_second: Optional[float] = None
         self.seconds: Optional[int] = None
+        self.is_aux: bool = is_aux
         self._listeners: List[Listener] = []
 
     def add_listener(self, listener: Listener) -> None:
         self._listeners.append(listener)
 
     def remove_listener(self, listener: Listener) -> None:
         self._listeners.remove(listener)
 
     async def handle_packet(self, packet: Packet) -> None:
-        new_value = packet.pulse_counts[self.number]
+        if not self.is_aux:
+            new_value = packet.pulse_counts[self.number]
+        else:
+            new_value = packet.aux[self.number]
         if new_value == self.pulses and self.pulses_per_second == 0:
             return
 
         if self.seconds is not None:
             elapsed_seconds = packet.delta_seconds(self.seconds)
-            self.pulses_per_second = (
-                (packet.delta_pulse_count(self.number, self.pulses) / elapsed_seconds)
-                if self.pulses is not None
-                else 0
-            )
+            if not self.is_aux:
+                self.pulses_per_second = (
+                    (
+                        packet.delta_pulse_count(self.number, self.pulses)
+                        / elapsed_seconds
+                    )
+                    if self.pulses is not None and elapsed_seconds > 0
+                    else 0
+                )
+            else:
+                self.pulses_per_second = (
+                    (packet.delta_aux_count(self.number, self.pulses) / elapsed_seconds)
+                    if self.pulses is not None and elapsed_seconds > 0
+                    else 0
+                )
 
         self.seconds = packet.seconds
         self.pulses = new_value
 
         await _invoke_listeners(self._listeners)
 
 
 class TemperatureSensor:
     """Represents a single GEM temperature-sensor channel"""
 
-    def __init__(self, monitor: "Monitor", number: int, unit: TemperatureUnit) -> None:
+    def __init__(
+        self, monitor: "Monitor", number: int, unit: Optional[TemperatureUnit] = None
+    ) -> None:
         self._monitor = monitor
         self.number: int = number
         self.temperature: Optional[float] = None
-        self.unit: TemperatureUnit = unit
+        self.unit: Optional[TemperatureUnit] = unit
         self._listeners: List[Listener] = []
 
     def add_listener(self, listener: Listener) -> None:
         self._listeners.append(listener)
 
     def remove_listener(self, listener: Listener) -> None:
         self._listeners.remove(listener)
@@ -122,38 +141,51 @@
         self.voltage = new_value
         await _invoke_listeners(self._listeners)
 
 
 class Channel:
     """Represents a single GEM CT channel"""
 
-    def __init__(self, monitor: "Monitor", number: int, net_metering: bool) -> None:
+    def __init__(
+        self,
+        monitor: "Monitor",
+        number: int,
+        net_metering: Optional[bool] = None,
+        is_aux: bool = False,
+    ) -> None:
         self._monitor = monitor
         self.number: int = number
-        self.net_metering: bool = net_metering
+        self.net_metering: Optional[bool] = net_metering
         self.total_absolute_watt_seconds: Optional[int] = None
         self.total_polarized_watt_seconds: Optional[int] = None
         self.absolute_watt_seconds: Optional[int] = None
         self.polarized_watt_seconds: Optional[int] = None
         self.amps: Optional[float] = None
         self.seconds: Optional[int] = None
         self.watts: Optional[float] = None
         self.timestamp: Optional[datetime] = None
+        self.ct_type: Optional[int] = None
+        self.ct_range: Optional[int] = None
+        self.is_aux: bool = is_aux
         self._listeners: List[Listener] = []
 
     @property
     def watt_seconds(self) -> Optional[float]:
-        if not self.net_metering:
+        if self.net_metering is None:
+            return None
+        elif not self.net_metering:
             return self.absolute_watt_seconds
         else:
             return self.net_watt_seconds
 
     @property
     def kilowatt_hours(self) -> Optional[float]:
-        if not self.net_metering:
+        if self.net_metering is None:
+            return None
+        elif not self.net_metering:
             return self.absolute_kilowatt_hours
         else:
             return self.net_kilowatt_hours
 
     @property
     def net_watt_seconds(self) -> Optional[float]:
         if self.absolute_watt_seconds is None or self.polarized_watt_seconds is None:
@@ -178,36 +210,91 @@
     @property
     def polarized_kilowatt_hours(self) -> Optional[float]:
         if self.polarized_watt_seconds is None:
             return None
 
         return self.polarized_watt_seconds / WATTS_PER_KILOWATT / SECONDS_PER_HOUR
 
+    async def set_ct_type(self, type: int) -> None:
+        control = self._monitor.control
+        assert control
+        assert control.api_type
+        assert self.ct_type is not None
+        assert self.ct_range is not None
+        assert not self.is_aux
+        if self.ct_type == type:
+            return
+
+        if control.api_type == ApiType.GEM:
+            await control.set_ct_type(channel=self.number + 1, type=type)
+        elif control.api_type == ApiType.ECM:
+            await control.set_ct_type_and_range(
+                channel=self.number + 1, type=type, range=self.ct_range
+            )
+        else:
+            assert False
+
+        self.ct_type = type
+
+    async def set_ct_range(self, range: int) -> None:
+        control = self._monitor.control
+        assert control
+        assert control.api_type
+        assert self.ct_type is not None
+        assert self.ct_range is not None
+        assert not self.is_aux
+        if self.ct_range == range:
+            return
+
+        if control.api_type == ApiType.GEM:
+            await control.set_ct_range(channel=self.number + 1, range=range)
+        elif control.api_type == ApiType.ECM:
+            await control.set_ct_type_and_range(
+                channel=self.number + 1, type=self.ct_type, range=range
+            )
+        else:
+            assert False
+
+        self.ct_range = range
+
     def add_listener(self, listener: Listener) -> None:
         self._listeners.append(listener)
 
     def remove_listener(self, listener: Listener) -> None:
         self._listeners.remove(listener)
 
     async def handle_settings(self, settings: GemSettings) -> None:
         net_metering = settings.channel_net_metering[self.number]
-        if net_metering == self.net_metering:
+        ct_type = settings.ct_types[self.number]
+        ct_range = settings.ct_ranges[self.number]
+        if (
+            net_metering == self.net_metering
+            and ct_type == self.ct_type
+            and ct_range == self.ct_range
+        ):
             return
 
         self.net_metering = net_metering
+        self.ct_type = ct_type
+        self.ct_range = ct_range
         await _invoke_listeners(self._listeners)
 
     async def handle_packet(self, packet: Packet) -> None:
-        new_absolute_watt_seconds = packet.absolute_watt_seconds[self.number]
-        new_polarized_watt_seconds = (
-            packet.polarized_watt_seconds[self.number]
-            if packet.polarized_watt_seconds
-            else None
-        )
-        new_amps = packet.currents[self.number] if packet.currents else None
+        if not self.is_aux:
+            new_absolute_watt_seconds = packet.absolute_watt_seconds[self.number]
+            new_polarized_watt_seconds = (
+                packet.polarized_watt_seconds[self.number]
+                if packet.polarized_watt_seconds
+                else None
+            )
+            new_amps = packet.currents[self.number] if packet.currents else None
+        else:
+            new_absolute_watt_seconds = packet.aux[self.number]
+            new_polarized_watt_seconds = None
+            new_amps = None
 
         if (
             self.absolute_watt_seconds == new_absolute_watt_seconds
             and self.polarized_watt_seconds == new_polarized_watt_seconds
             and self.amps == new_amps
             and self.watts == 0
         ):
@@ -215,21 +302,28 @@
             return
 
         if self.seconds is not None:
             elapsed_seconds = packet.delta_seconds(self.seconds)
 
             # This is the total energy produced or consumed since the last
             # sample.
-            delta_total_watt_seconds = (
-                packet.delta_absolute_watt_seconds(
-                    self.number, self.absolute_watt_seconds
+            if not self.is_aux:
+                delta_total_watt_seconds = (
+                    packet.delta_absolute_watt_seconds(
+                        self.number, self.absolute_watt_seconds
+                    )
+                    if self.absolute_watt_seconds is not None
+                    else 0
+                )
+            else:
+                delta_total_watt_seconds = (
+                    packet.delta_aux_count(self.number, self.absolute_watt_seconds)
+                    if self.absolute_watt_seconds is not None
+                    else 0
                 )
-                if self.absolute_watt_seconds is not None
-                else 0
-            )
 
             # This is the energy produced since the last sample. This will be 0
             # for all channels except for channels in NET metering mode that
             # are actually producing electricity.
             if (
                 self.polarized_watt_seconds is not None
                 and new_polarized_watt_seconds is not None
@@ -243,203 +337,365 @@
             # This is the energy consumed since the last sample.
             delta_watt_seconds_consumed = (
                 delta_total_watt_seconds - delta_watt_seconds_produced
             )
 
             # Now compute the average power over the time since the last sample
             self.watts = (
-                delta_watt_seconds_consumed - delta_watt_seconds_produced
-            ) / elapsed_seconds
+                (delta_watt_seconds_consumed - delta_watt_seconds_produced)
+                / elapsed_seconds
+                if elapsed_seconds > 0
+                else 0
+            )
 
         self.seconds = packet.seconds
         self.absolute_watt_seconds = new_absolute_watt_seconds
         self.polarized_watt_seconds = new_polarized_watt_seconds
         self.amps = new_amps
         self.timestamp = packet.time_stamp
 
         await _invoke_listeners(self._listeners)
 
 
+class Aux:
+    """Represents a single ECM-1240 Aux channel."""
+
+    def __init__(self, monitor: "Monitor", number: int) -> None:
+        self._monitor = monitor
+        self.number: int = number
+        self.pulse_counter = PulseCounter(monitor, number, is_aux=True)
+        self.channel = Channel(monitor, number, net_metering=False, is_aux=True)
+
+    def add_listener(self, listener: Listener) -> None:
+        self.pulse_counter.add_listener(listener)
+        self.channel.add_listener(listener)
+
+    def remove_listener(self, listener: Listener) -> None:
+        self.pulse_counter.remove_listener(listener)
+        self.channel.remove_listener(listener)
+
+    async def handle_packet(self, packet: Packet) -> None:
+        await asyncio.gather(
+            self.pulse_counter.handle_packet(packet),
+            self.channel.handle_packet(packet),
+        )
+
+
 NUM_PULSE_COUNTERS: int = 4
 NUM_TEMPERATURE_SENSORS: int = 8
 
 
+class MonitorControl:
+    """Provides access to APIs that control a monitor."""
+
+    @staticmethod
+    async def try_create(
+        protocol: GemProtocol, serial_number: int, api_timeout: timedelta | None
+    ) -> Optional[Tuple["MonitorControl", GemSettings]]:
+        try:
+            settings = await api_ext.get_all_settings(
+                protocol, serial_number, api_timeout
+            )
+            # await api_ext.send_one_packet(protocol, serial_number)
+            return (MonitorControl(protocol, serial_number), settings)
+        except:
+            # The remote either timed out or returned binary data, which probably indicates it's a DashBox
+            return None
+
+    def __init__(self, protocol: GemProtocol, serial_number: int) -> None:
+        self._protocol = protocol
+        self._serial_number = serial_number
+
+    @property
+    def api_type(self) -> ApiType:
+        return self._protocol.api_type
+
+    def set_protocol(self, protocol: GemProtocol) -> None:
+        self._protocol = protocol
+
+    async def get_settings(self) -> GemSettings:
+        return await api_ext.get_all_settings(self._protocol, self._serial_number)
+
+    async def set_ct_type(self, channel: int, type: int) -> None:
+        await api_ext.set_ct_type(
+            self._protocol,
+            channel=channel,
+            type=type,
+            serial_number=self._serial_number,
+        )
+
+    async def set_ct_range(self, channel: int, range: int) -> None:
+        await api_ext.set_ct_range(
+            self._protocol,
+            channel=channel,
+            range=range,
+            serial_number=self._serial_number,
+        )
+
+    async def set_ct_type_and_range(self, channel: int, type: int, range: int) -> None:
+        await api_ext.set_ct_type_and_range(
+            self._protocol,
+            channel=channel,
+            type=type,
+            range=range,
+            serial_number=self._serial_number,
+        )
+
+    async def set_packet_send_interval(self, seconds: int) -> None:
+        assert seconds > 0 and seconds <= 255
+        await api.set_packet_send_interval(
+            self._protocol,
+            send_interval_seconds=seconds,
+            serial_number=self._serial_number,
+        )
+
+    async def set_packet_destination(
+        self, host: str, port: int, session: aiohttp.ClientSession
+    ) -> None:
+        peername = self._protocol.peername
+        if peername:
+            (gem_host, _) = peername
+
+            await api_ext.set_packet_destination(gem_host, host, port, session)
+            LOG.info(
+                "%d: Configured to send packets to %s:%d",
+                self._serial_number,
+                host,
+                port,
+            )
+            return
+
+    async def set_packet_format(self, format: PacketFormatType) -> None:
+        await api.set_packet_format(self._protocol, format, self._serial_number)
+
+
+class MonitorType(Enum):
+    ECM_1220 = 1
+    ECM_1240 = 2
+    GEM = 3
+
+
 class Monitor:
     """Represents a single GreenEye Monitor"""
 
     def __init__(self, serial_number: int) -> None:
         """serial_number is the 8 digit serial number as it appears in the GEM
         UI"""
         self.serial_number: int = serial_number
         self._protocol: Optional[GemProtocol] = None
+        self._control: Optional[MonitorControl] = None
         self.channels: List[Channel] = []
-        self.pulse_counters: List[PulseCounter] = [
-            PulseCounter(self, num) for num in range(0, NUM_PULSE_COUNTERS)
-        ]
+        self.pulse_counters: List[PulseCounter] = []
         self.temperature_sensors: List[TemperatureSensor] = []
+        self.aux: List[Channel | Aux] = []
         self.voltage_sensor: VoltageSensor = VoltageSensor(self)
         self.packet_send_interval: timedelta = timedelta(seconds=0)
         self.packet_format: Optional[PacketFormatType] = None
+        self.settings: Optional[GemSettings] = None
+        self._configured: bool = False
         self._packet_interval: int = 0
         self._last_packet_seconds: Optional[int] = None
         self._listeners: List[Listener] = []
 
-    async def _set_protocol(self, protocol: Optional[GemProtocol]) -> None:
+    @property
+    def control(self) -> Optional[MonitorControl]:
+        return self._control
+
+    @property
+    def type(self) -> MonitorType:
+        if self.packet_format == PacketFormatType.ECM_1220:
+            return MonitorType.ECM_1220
+        elif self.packet_format == PacketFormatType.ECM_1240:
+            return MonitorType.ECM_1240
+        else:
+            return MonitorType.GEM
+
+    async def _set_protocol(
+        self, protocol: Optional[GemProtocol], api_timeout: timedelta | None = None
+    ) -> None:
         if self._protocol is protocol:
             return
+        if protocol is None:
+            self._protocol = None
+            self._control = None
+            return
 
         self._protocol = protocol
-        if self._protocol:
-            await self._sync_with_settings(self._protocol)
-
-    async def _sync_with_settings(self, protocol: GemProtocol) -> None:
-        settings = await get_all_settings(protocol, self.serial_number)
+        result = await MonitorControl.try_create(
+            self._protocol, self.serial_number, api_timeout
+        )
+        if result is not None:
+            (self._control, settings) = result
+            await self._configure_from_settings(settings, self._control)
 
+    async def _configure_from_settings(
+        self, settings: GemSettings, control: MonitorControl
+    ) -> None:
+        self.settings = settings
         self.packet_send_interval = settings.packet_send_interval
         self.packet_format = settings.packet_format
 
         # Truncate or expand channel listing
         if len(self.channels) < settings.num_channels:
             del self.channels[settings.num_channels :]
         for num in range(len(self.channels), settings.num_channels):
             self.channels.append(Channel(self, num, settings.channel_net_metering[num]))
 
-        # Initialize temperature sensors if needed
-        for num in range(len(self.temperature_sensors), NUM_TEMPERATURE_SENSORS):
-            self.temperature_sensors.append(
-                TemperatureSensor(self, num, settings.temperature_unit)
-            )
+        if self.type == MonitorType.GEM:
+            # Initialize temperature sensors if needed
+            for num in range(len(self.temperature_sensors), NUM_TEMPERATURE_SENSORS):
+                self.temperature_sensors.append(
+                    TemperatureSensor(self, num, settings.temperature_unit)
+                )
 
-        # Pulse counters and voltage sensors were created up front
+            self.pulse_counters = [
+                PulseCounter(self, num) for num in range(0, NUM_PULSE_COUNTERS)
+            ]
+
+        # Voltage sensor was created up front
 
         # Now update settings if needed and trigger listeners
         coroutines = []
         for temperature_sensor in self.temperature_sensors:
             coroutines.append(temperature_sensor.handle_settings(settings))
         for channel in self.channels:
             coroutines.append(channel.handle_settings(settings))
+        self._configured = True
+        LOG.info(f"Configured {self.serial_number} from settings API call.")
+
         for listener in self._listeners:
-            coroutines.append(asyncio.coroutine(listener)())
-        await asyncio.wait(coroutines)
+            coroutines.append(_ensure_coroutine(listener)())
+        await asyncio.gather(*coroutines)
 
-    async def set_packet_destination(
-        self, host: str, port: int, session: aiohttp.ClientSession
-    ) -> None:
-        if self._protocol:
-            peername = self._protocol.peername
-            if peername:
-                (gem_host, _) = peername
-
-                await set_packet_destination(gem_host, host, port, session)
-                LOG.info(
-                    "%d: Configured to send packets to %s:%d",
-                    self.serial_number,
-                    host,
-                    port,
-                )
-                return
+    async def _configure_from_packet(self, packet: Packet) -> None:
+        self.packet_format = packet.packet_format.type
 
-        raise Exception(
-            "Cannot set packet destination when connected to the monitor via something other than a TCP socket."
-        )
+        if not self.aux and len(packet.aux) == 5:
+            for num in range(0, 4):
+                self.aux.append(Channel(self, num, net_metering=False, is_aux=True))
+            self.aux.append(Aux(self, 4))
 
-    async def set_packet_format(self, format: PacketFormatType) -> None:
-        if self._protocol:
-            await api.set_packet_format(self._protocol, format, self.serial_number)
-        else:
-            raise Exception(
-                "Cannot set packet format when not connected to the monitor."
-            )
+        if not self._configured:
+            for num in range(0, packet.num_channels):
+                self.channels.append(Channel(self, num))
+
+            for num in range(0, len(packet.temperatures)):
+                self.temperature_sensors.append(TemperatureSensor(self, num))
+
+            if self.type == MonitorType.GEM:
+                self.pulse_counters = [
+                    PulseCounter(self, num) for num in range(0, NUM_PULSE_COUNTERS)
+                ]
+
+            # Voltage sensor was created up front
+
+            self._configured = True
+            LOG.info(f"Configured {self.serial_number} from first packet.")
+        coroutines = []
+        for listener in self._listeners:
+            coroutines.append(_ensure_coroutine(listener)())
+        await asyncio.gather(*coroutines)
+
+    async def set_packet_send_interval(self, seconds: int) -> None:
+        await self._control.set_packet_send_interval(seconds)
 
     def set_packet_interval(self, seconds: int) -> None:
         self._packet_interval = seconds
 
     def add_listener(self, listener: Listener) -> None:
         self._listeners.append(listener)
 
     def remove_listener(self, listener: Listener) -> None:
         self._listeners.remove(listener)
 
     async def handle_packet(self, packet: Packet) -> None:
+        await self._configure_from_packet(packet)
+
         if self._last_packet_seconds is not None:
             elapsed_seconds = packet.delta_seconds(self._last_packet_seconds)
             if elapsed_seconds < self._packet_interval:
                 return
         self._last_packet_seconds = packet.seconds
 
         await self.voltage_sensor.handle_packet(packet)
         for channel in self.channels:
             await channel.handle_packet(packet)
         for temperature_sensor in self.temperature_sensors:
             await temperature_sensor.handle_packet(packet)
         for pulse_counter in self.pulse_counters:
             await pulse_counter.handle_packet(packet)
+        for aux in self.aux:
+            await aux.handle_packet(packet)
         await _invoke_listeners(self._listeners)
 
 
 async def _invoke_listeners(listeners: List[Listener]) -> None:
-    coroutines = [asyncio.coroutine(listener)() for listener in listeners]
+    coroutines = [_ensure_coroutine(listener)() for listener in listeners]
     if len(coroutines) > 0:
-        await asyncio.wait(coroutines)  # type: ignore
+        await asyncio.gather(*coroutines)  # type: ignore
 
 
 ServerListener = Callable[[PacketProtocolMessage], Awaitable[None]]
 GEM_PORT = 8000
 
 
 class MonitorProtocolProcessor:
     """Listens for connections from GEMs and notifies a listener of each
     packet."""
 
-    def __init__(self, listener: ServerListener) -> None:
+    def __init__(self, listener: ServerListener, send_packet_delay: bool) -> None:
         self._consumer_task = asyncio.ensure_future(self._consumer())
         LOG.debug("Packet processor started")
         self._listener = listener
         self._queue: asyncio.Queue[PacketProtocolMessage] = asyncio.Queue()
         self._server: Optional[Server] = None
         self._protocols: Dict[int, GemProtocol] = {}
+        self._send_packet_delay = send_packet_delay
 
     async def connect(
         self, hostname: str
     ) -> Tuple[asyncio.BaseTransport, asyncio.BaseProtocol]:
         loop = asyncio.get_event_loop()
         return await loop.create_connection(
             self._create_protocol,
             host=hostname,
             port=GEM_PORT,
         )
 
-    async def start_server(self, port: int) -> None:
+    async def start_server(self, desiredPort: int = 0) -> int:
         loop = asyncio.get_event_loop()
         self._server = await loop.create_server(
             self._create_protocol,
             None,
-            port,
+            desiredPort,
             family=socket.AF_INET,
         )
 
-        LOG.info("Server started on {}".format(self._server.sockets[0].getsockname()))
+        host, port = self._server.sockets[0].getsockname()
+        LOG.info(f"Server started on {host}:{port}")
+        return port
 
     async def _consumer(self) -> None:
         try:
             while True:
                 message = await self._queue.get()
                 if isinstance(message, ConnectionLostMessage):
                     del self._protocols[id(message.protocol)]
                 try:
                     await self._listener(message)
-                except Exception as exc:
-                    LOG.exception("Exception while calling the listener!", exc)
+                except Exception:
+                    LOG.exception("Exception while calling the listener!")
                 self._queue.task_done()
         except asyncio.CancelledError:
             LOG.debug("queue consumer is getting canceled")
             raise
 
     def _create_protocol(self) -> GemProtocol:
-        protocol = GemProtocol(self._queue)
+        # TODO: Set API type to GEM when connecting
+        protocol = GemProtocol(self._queue, send_packet_delay=self._send_packet_delay)
         self._protocols[id(protocol)] = protocol
         return protocol
 
     async def close(self) -> None:
         if self._server is not None:
             LOG.info(
                 "Closing server on {}".format(self._server.sockets[0].getsockname())
@@ -470,21 +726,24 @@
 
 MonitorListener = Union[Callable[[Monitor], Awaitable[None]], Callable[[Monitor], None]]
 
 
 class Monitors:
     """Keeps track of all monitors that have reported data"""
 
-    def __init__(self) -> None:
+    def __init__(
+        self, send_packet_delay: bool = True, api_timeout: timedelta | None = None
+    ) -> None:
         self.monitors: Dict[int, Monitor] = {}
-        self._protocol_to_monitors: Dict[int, List[Monitor]] = {}
+        self._protocol_to_monitors: Dict[int, set[Monitor]] = {}
         self._listeners: List[MonitorListener] = []
         self._processor: MonitorProtocolProcessor = MonitorProtocolProcessor(
-            self._handle_message
+            self._handle_message, send_packet_delay=send_packet_delay
         )
+        self._api_timeout: timedelta | None = api_timeout
 
     async def __aenter__(self) -> "Monitors":
         return self
 
     async def __aexit__(
         self,
         exc_type: Optional[Type[BaseException]],
@@ -495,59 +754,75 @@
 
     def add_listener(self, listener: MonitorListener) -> None:
         self._listeners.append(listener)
 
     def remove_listener(self, listener: MonitorListener) -> None:
         self._listeners.remove(listener)
 
-    async def start_server(self, port: int) -> None:
-        await self._processor.start_server(port)
+    async def start_server(self, port: int = 0) -> int:
+        return await self._processor.start_server(port)
 
     async def connect(self, host: str) -> Monitor:
         (_, protocol) = await self._processor.connect(host)
         assert isinstance(protocol, GemProtocol)
-        serial_number = await api.get_serial_number(protocol)
+        serial_number = await api.get_serial_number(protocol, timeout=self._api_timeout)
         monitor = await self._add_monitor(serial_number, protocol)
         return monitor
 
     async def close(self) -> None:
         await self._processor.close()
 
     async def _handle_message(self, message: PacketProtocolMessage) -> None:
         assert isinstance(message.protocol, GemProtocol)
         protocol_id = id(message.protocol)
         if isinstance(message, PacketReceivedMessage):
             packet = message.packet
             serial_number = packet.device_id * 100000 + packet.serial_number
             if serial_number not in self.monitors:
-                await self._add_monitor(serial_number, message.protocol)
-            monitor = self.monitors[serial_number]
-
-            await monitor.handle_packet(packet)
+                await self._add_monitor(serial_number, message.protocol, packet)
+            else:
+                monitor = self.monitors[serial_number]
+                await self._set_monitor_protocol(monitor, message.protocol)
+                await monitor.handle_packet(packet)
         else:
             if isinstance(message, ConnectionLostMessage):
                 for monitor in self._protocol_to_monitors.pop(protocol_id):
                     await monitor._set_protocol(None)
             elif isinstance(message, ConnectionMadeMessage):
-                self._protocol_to_monitors[protocol_id] = []
+                self._protocol_to_monitors[protocol_id] = set()
 
-    async def _add_monitor(self, serial_number: int, protocol: GemProtocol) -> Monitor:
+    async def _add_monitor(
+        self, serial_number: int, protocol: GemProtocol, packet: Packet | None = None
+    ) -> Monitor:
         LOG.info("Discovered new monitor: %d", serial_number)
         monitor = Monitor(serial_number)
         await self._set_monitor_protocol(monitor, protocol)
+        if packet:
+            await monitor.handle_packet(packet)
         self.monitors[serial_number] = monitor
         await self._notify_new_monitor(monitor)
         return monitor
 
     async def _set_monitor_protocol(
         self, monitor: Monitor, protocol: GemProtocol
     ) -> None:
         protocol_id = id(protocol)
-        self._protocol_to_monitors[protocol_id].append(monitor)
-        await monitor._set_protocol(protocol)
+        self._protocol_to_monitors[protocol_id].add(monitor)
+        await monitor._set_protocol(protocol, api_timeout=self._api_timeout)
 
     async def _notify_new_monitor(self, monitor: Monitor) -> None:
         listeners = [
-            asyncio.coroutine(listener)(monitor) for listener in self._listeners
+            _ensure_coroutine(listener)(monitor) for listener in self._listeners
         ]
         if len(listeners) > 0:
-            await asyncio.wait(listeners)  # type: ignore
+            await asyncio.gather(*listeners)  # type: ignore
+
+
+def _ensure_coroutine(listener):
+    if inspect.iscoroutinefunction(listener):
+        return listener
+    else:
+
+        async def async_listener(*args):
+            listener(*args)
+
+        return async_listener
```

## Comparing `greeneye_monitor-3.0.3.dist-info/LICENSE` & `greeneye_monitor-4.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `greeneye_monitor-3.0.3.dist-info/METADATA` & `greeneye_monitor-4.0.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: greeneye-monitor
-Version: 3.0.3
+Version: 4.0
 Summary: Receive data packets from GreenEye Monitor (http://www.brultech.com/greeneye/)
 Home-page: https://github.com/jkeljo/greeneye-monitor
 Author: Jonathan Keljo
-License: UNKNOWN
 Keywords: greeneye
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Home Automation
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.5
-Requires-Python: ~=3.5
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: ~=3.10
+License-File: LICENSE
 Requires-Dist: aiohttp
-Requires-Dist: siobrultech-protocols (==0.5)
+Requires-Dist: siobrultech-protocols (==0.12)
 
 ==================
 `greeneye-monitor`
 ==================
 
 Receive data from your `GreenEye Monitor <http://www.brultech.com/greeneye/>`_ in Python.
 
@@ -59,9 +58,7 @@
 5. Set the "Packet Send Interval" if you want something other than the default
 6. Click "Save"
 7. Click the "Network" tab
 8. Enter the IP address of the computer on which you'll be running this software, and the port of your choice
 9. Click "Save"
 10. Click "Return" when it becomes available
 11. Click "Exit Setup Mode"
-
-
```

