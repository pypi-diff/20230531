# Comparing `tmp/netbox_lists-3.0.0.tar.gz` & `tmp/netbox_lists-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox_lists-3.0.0.tar", max compression
+gzip compressed data, was "netbox_lists-3.1.0.tar", max compression
```

## Comparing `netbox_lists-3.0.0.tar` & `netbox_lists-3.1.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0    11358 2023-05-03 03:30:58.021344 netbox_lists-3.0.0/LICENSE
--rw-r--r--   0        0        0     2174 2023-05-03 03:30:58.021344 netbox_lists-3.0.0/netbox_lists/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 03:30:58.021344 netbox_lists-3.0.0/netbox_lists/api/__init__.py
--rw-r--r--   0        0        0       95 2023-05-03 03:30:58.021344 netbox_lists-3.0.0/netbox_lists/api/constants.py
--rw-r--r--   0        0        0     1942 2023-05-03 03:30:58.021344 netbox_lists-3.0.0/netbox_lists/api/filtersets.py
--rw-r--r--   0        0        0      547 2023-05-03 03:30:58.021344 netbox_lists-3.0.0/netbox_lists/api/renderers.py
--rw-r--r--   0        0        0     1606 2023-05-03 03:30:58.021344 netbox_lists-3.0.0/netbox_lists/api/serializers.py
--rw-r--r--   0        0        0     1212 2023-05-03 03:30:58.021344 netbox_lists-3.0.0/netbox_lists/api/urls.py
--rw-r--r--   0        0        0     6639 2023-05-03 03:30:58.021344 netbox_lists-3.0.0/netbox_lists/api/utils.py
--rw-r--r--   0        0        0    25564 2023-05-03 03:30:58.021344 netbox_lists-3.0.0/netbox_lists/api/views.py
--rw-r--r--   0        0        0        0 2023-05-03 03:30:58.021344 netbox_lists-3.0.0/netbox_lists/py.typed
--rw-r--r--   0        0        0      979 2023-05-03 03:30:58.021344 netbox_lists-3.0.0/pyproject.toml
--rw-r--r--   0        0        0      485 1970-01-01 00:00:00.000000 netbox_lists-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-05-31 06:15:27.103254 netbox_lists-3.1.0/LICENSE
+-rw-r--r--   0        0        0     8818 2023-05-31 06:15:27.103254 netbox_lists-3.1.0/README.md
+-rw-r--r--   0        0        0     2481 2023-05-31 06:15:27.103254 netbox_lists-3.1.0/netbox_lists/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-31 06:15:27.103254 netbox_lists-3.1.0/netbox_lists/api/__init__.py
+-rw-r--r--   0        0        0       95 2023-05-31 06:15:27.103254 netbox_lists-3.1.0/netbox_lists/api/constants.py
+-rw-r--r--   0        0        0     1942 2023-05-31 06:15:27.103254 netbox_lists-3.1.0/netbox_lists/api/filtersets.py
+-rw-r--r--   0        0        0      547 2023-05-31 06:15:27.103254 netbox_lists-3.1.0/netbox_lists/api/renderers.py
+-rw-r--r--   0        0        0     1831 2023-05-31 06:15:27.103254 netbox_lists-3.1.0/netbox_lists/api/serializers.py
+-rw-r--r--   0        0        0     1305 2023-05-31 06:15:27.103254 netbox_lists-3.1.0/netbox_lists/api/urls.py
+-rw-r--r--   0        0        0     6639 2023-05-31 06:15:27.103254 netbox_lists-3.1.0/netbox_lists/api/utils.py
+-rw-r--r--   0        0        0    25851 2023-05-31 06:15:27.103254 netbox_lists-3.1.0/netbox_lists/api/views.py
+-rw-r--r--   0        0        0        0 2023-05-31 06:15:27.103254 netbox_lists-3.1.0/netbox_lists/py.typed
+-rw-r--r--   0        0        0     1023 2023-05-31 06:15:27.103254 netbox_lists-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0     9428 1970-01-01 00:00:00.000000 netbox_lists-3.1.0/PKG-INFO
```

### Comparing `netbox_lists-3.0.0/LICENSE` & `netbox_lists-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox_lists-3.0.0/netbox_lists/__init__.py` & `netbox_lists-3.1.0/netbox_lists/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -54,11 +54,18 @@
             "__meta_netbox_site_name": ("site", "name"),
             "__meta_netbox_platform_name": ("platform", "name"),
             "__meta_netbox_primary_ip": ("primary_ip", "address", "ip"),
             "__meta_netbox_primary_ip4": ("primary_ip4", "address", "ip"),
             "__meta_netbox_primary_ip6": ("primary_ip6", "address", "ip"),
             "__meta_netbox_serial": ("serial",),
         },
+        "prometheus_ipaddress_sd_target": (("address", "ip"),),
+        "prometheus_ipaddress_sd_labels": {
+            "__meta_netbox_id": ("id",),
+            "__meta_netbox_role": ("role",),
+            "__meta_netbox_dns_name": ("dns_name",),
+            "__meta_netbox_status": ("status",),
+        },
     }
 
 
 config = ListsPluginConfig
```

### Comparing `netbox_lists-3.0.0/netbox_lists/api/filtersets.py` & `netbox_lists-3.1.0/netbox_lists/api/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox_lists-3.0.0/netbox_lists/api/renderers.py` & `netbox_lists-3.1.0/netbox_lists/api/renderers.py`

 * *Files identical despite different names*

### Comparing `netbox_lists-3.0.0/netbox_lists/api/serializers.py` & `netbox_lists-3.1.0/netbox_lists/api/serializers.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 from itertools import chain
 from typing import Dict, Generic, List, TypeVar
 
 from dcim.models import Device
 from django.conf import settings
+from ipam.models import IPAddress
 from rest_framework import serializers
 from utilities.exceptions import AbortRequest
 from virtualization.models import VirtualMachine
 
 from .utils import get_attr, get_attr_str
 
 T = TypeVar("T")
 
 
 class BasePrometheusSerializer(serializers.Serializer, Generic[T]):
     targets = serializers.SerializerMethodField()
     labels = serializers.SerializerMethodField()
 
+    default_target_attr = "name"
+
     def get_targets(self, device: T) -> List[str]:
-        # Default to Name
+        # Default to default_target_attr
         for attrs in chain(
             settings.PLUGINS_CONFIG["netbox_lists"][
                 f"prometheus_{self.settings_type}_sd_target"
             ],
-            (("name",),),
+            ((self.default_target_attr,),),
         ):
-            print(f"Attr: {repr(attrs)}")
             target = get_attr(attrs, device)
             if target is not None:
                 return [str(target)]
 
-        # This shouldn't happen since Name is a required field
+        # This shouldn't happen since default_target_attr should be a required field
         raise AbortRequest(
             f"No target found for {repr(device)}. (this shouldn't happen)"
         )
 
     def get_labels(self, device: T) -> Dict[str, str]:
         labels = {
             k: get_attr_str(v, device)
@@ -47,7 +49,12 @@
 
 class PrometheusVMSerializer(BasePrometheusSerializer[VirtualMachine]):
     settings_type = "vm"
 
 
 class PrometheusDeviceSerializer(BasePrometheusSerializer[Device]):
     settings_type = "device"
+
+
+class PrometheusIPAddressSerializer(BasePrometheusSerializer[IPAddress]):
+    settings_type = "ipaddress"
+    default_target_attr = "address"
```

### Comparing `netbox_lists-3.0.0/netbox_lists/api/urls.py` & `netbox_lists-3.1.0/netbox_lists/api/urls.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     DevicesVMsListViewSet,
     IPAddressListViewSet,
     IPRangeListViewSet,
     ListsRootView,
     PrefixListViewSet,
     PrometheusDeviceSD,
     PrometheusVirtualMachineSD,
+    PrometheusIPAddressSD,
     ServiceListviewSet,
     TagsListViewSet,
     VirtualMachinesListViewSet,
 )
 
 app_name = "lists"
 
@@ -29,11 +30,12 @@
 router.register("tags", TagsListViewSet)
 router.register("devices", DevicesListViewSet, basename="devices")
 router.register(
     "virtual-machines", VirtualMachinesListViewSet, basename="virtual-machines"
 )
 router.register("prometheus-devices", PrometheusDeviceSD)
 router.register("prometheus-vms", PrometheusVirtualMachineSD)
+router.register("prometheus-ip-addresses", PrometheusIPAddressSD)
 
 router.register("devices-vms", DevicesVMsListViewSet)
 router.register("devices-vms-attrs", DevicesVMsAttrsListViewSet)
 urlpatterns = router.urls
```

### Comparing `netbox_lists-3.0.0/netbox_lists/api/utils.py` & `netbox_lists-3.1.0/netbox_lists/api/utils.py`

 * *Files identical despite different names*

### Comparing `netbox_lists-3.0.0/netbox_lists/api/views.py` & `netbox_lists-3.1.0/netbox_lists/api/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,19 @@
 from rest_framework.viewsets import GenericViewSet
 from virtualization.filtersets import VirtualMachineFilterSet
 from virtualization.models import VirtualMachine
 
 from .constants import AS_CIDR_PARAM_NAME, FAMILY_PARAM_NAME, SUMMARIZE_PARAM_NAME
 from .filtersets import CustomPrefixFilterSet
 from .renderers import PlainTextRenderer
-from .serializers import PrometheusDeviceSerializer, PrometheusVMSerializer
+from .serializers import (
+    PrometheusDeviceSerializer,
+    PrometheusIPAddressSerializer,
+    PrometheusVMSerializer,
+)
 from .utils import (
     device_vm_primary_list,
     filter_queryset,
     get_as_cidr_param,
     get_attr_json,
     get_family_param,
     get_service_ips,
@@ -650,14 +654,22 @@
     InvalidFilterCheckMixin, mixins.ListModelMixin, ListsBaseViewSet
 ):
     queryset = VirtualMachine.objects.filter()
     filterset_class = VirtualMachineFilterSet
     serializer_class = PrometheusVMSerializer
 
 
+class PrometheusIPAddressSD(
+    InvalidFilterCheckMixin, mixins.ListModelMixin, ListsBaseViewSet
+):
+    queryset = IPAddress.objects.filter()
+    filterset_class = IPAddressFilterSet
+    serializer_class = PrometheusIPAddressSerializer
+
+
 class DevicesVMsAttrsListViewSet(ListsBaseViewSet):
     renderer_classes = [JSONRenderer, BrowsableAPIRenderer]
     filterset_class = DeviceFilterSet
     filter_backends = (DjangoFilterBackend,)
     queryset = Device.objects.filter()
 
     def _to_dict(
```

### Comparing `netbox_lists-3.0.0/pyproject.toml` & `netbox_lists-3.1.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 [tool.poetry]
 name = "netbox-lists"
-version = "3.0.0"
+version = "3.1.0"
 description = ""
 authors = ["Devon Mar <devonm@mdmm.ca>"]
+license = "Apache-2.0"
+readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.6.2"
 netaddr = "^0.8.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.0"
```

