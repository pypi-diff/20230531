# Comparing `tmp/panos_upgrade_assurance-0.0.1.tar.gz` & `tmp/panos_upgrade_assurance-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panos_upgrade_assurance-0.0.1.tar", max compression
+gzip compressed data, was "panos_upgrade_assurance-0.0.2.tar", max compression
```

## Comparing `panos_upgrade_assurance-0.0.1.tar` & `panos_upgrade_assurance-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1081 2023-05-09 06:13:35.366704 panos_upgrade_assurance-0.0.1/LICENSE
--rw-r--r--   0        0        0      967 2023-05-16 07:21:29.870298 panos_upgrade_assurance-0.0.1/README.md
--rw-r--r--   0        0        0        0 2023-01-13 09:03:37.587982 panos_upgrade_assurance-0.0.1/panos_upgrade_assurance/__init__.py
--rw-r--r--   0        0        0    34913 2023-05-16 07:21:29.885255 panos_upgrade_assurance-0.0.1/panos_upgrade_assurance/check_firewall.py
--rw-r--r--   0        0        0    34300 2023-05-16 07:21:29.887016 panos_upgrade_assurance-0.0.1/panos_upgrade_assurance/firewall_proxy.py
--rw-r--r--   0        0        0    29926 2023-05-16 07:21:29.888661 panos_upgrade_assurance-0.0.1/panos_upgrade_assurance/snapshot_compare.py
--rw-r--r--   0        0        0    11729 2023-05-16 07:21:29.890188 panos_upgrade_assurance-0.0.1/panos_upgrade_assurance/utils.py
--rw-r--r--   0        0        0      782 2023-05-16 07:21:29.891969 panos_upgrade_assurance-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1660 1970-01-01 00:00:00.000000 panos_upgrade_assurance-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-05-31 01:35:38.966524 panos_upgrade_assurance-0.0.2/LICENSE
+-rw-r--r--   0        0        0      930 2023-05-31 01:35:38.966524 panos_upgrade_assurance-0.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 01:35:38.970525 panos_upgrade_assurance-0.0.2/panos_upgrade_assurance/__init__.py
+-rw-r--r--   0        0        0    36412 2023-05-31 01:35:38.970525 panos_upgrade_assurance-0.0.2/panos_upgrade_assurance/check_firewall.py
+-rw-r--r--   0        0        0    34581 2023-05-31 01:35:38.970525 panos_upgrade_assurance-0.0.2/panos_upgrade_assurance/firewall_proxy.py
+-rw-r--r--   0        0        0    30971 2023-05-31 01:35:38.970525 panos_upgrade_assurance-0.0.2/panos_upgrade_assurance/snapshot_compare.py
+-rw-r--r--   0        0        0    12052 2023-05-31 01:35:38.970525 panos_upgrade_assurance-0.0.2/panos_upgrade_assurance/utils.py
+-rw-r--r--   0        0        0      932 2023-05-31 01:36:17.018704 panos_upgrade_assurance-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1577 1970-01-01 00:00:00.000000 panos_upgrade_assurance-0.0.2/PKG-INFO
```

### Comparing `panos_upgrade_assurance-0.0.1/LICENSE` & `panos_upgrade_assurance-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `panos_upgrade_assurance-0.0.1/README.md` & `panos_upgrade_assurance-0.0.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 The `panos-upgrade-assurance` package includes the set of classes written in `Python` to ease the process of writing checks and state snapshots during PanOS upgrade on the Next Generation Firewall.
 
 Both checks and snapshots can be used to verify the state of a device during an upgrade process. What more, it is possible to generate a report for these checks.
 
 The libraries were written to support Ansible and XSOAR integrations. They depend on [pan-os-python](https://pan.dev/panos/docs/panospython/) libraries and therefore are quite easy to fit into the [PanOS Ansible modules collection](https://galaxy.ansible.com/paloaltonetworks/panos).
 
-For more detailed documentation please refer to [PAN.DEV](https://pan.dev/panos-upgrade-assurance/docs/) portal.
+For more detailed documentation please refer to [PAN.DEV](https://pan.dev/panos/docs/panos-upgrade-assurance/) portal.
 
 ## Installation
 
 To install the package you can use `pip`:
 
 ``` console
-python -m pip install 'git+https://github.com/PaloAltoNetworks/pan-os-upgrade-assurance'
+python -m pip install panos-upgrade-assurance
 ```
```

### Comparing `panos_upgrade_assurance-0.0.1/panos_upgrade_assurance/check_firewall.py` & `panos_upgrade_assurance-0.0.2/panos_upgrade_assurance/check_firewall.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,109 +1,129 @@
-from typing import Optional, Union, List, Iterable, Dict
+from typing import Optional, Union, List, Dict
 from math import ceil
 from datetime import datetime
+import locale
 
-from panos_upgrade_assurance.utils import CheckResult, ConfigParser, interpret_yes_no, CheckType, SnapType, CheckStatus
+from panos_upgrade_assurance.utils import (
+    CheckResult,
+    ConfigParser,
+    interpret_yes_no,
+    CheckType,
+    SnapType,
+    CheckStatus,
+)
 from panos_upgrade_assurance.firewall_proxy import FirewallProxy
 from panos import PanOSVersion
 from panos.errors import PanDeviceXapiError
 
+
 class ContentDBVersionInFutureException(Exception):
     """Used when the installed Content DB version is newer than the latest available version."""
+
     pass
 
+
 class WrongDataTypeException(Exception):
     """Used when passed configuration does not meet the data type requirements."""
+
     pass
 
+
 class ImageVersionNotAvailableException(Exception):
     """Used when requested image version is not available for downloading."""
+
     pass
 
+
 class UpdateServerConnectivityException(Exception):
     """Used when connection to the Update Server cannot be established."""
+
     pass
 
+
 class CheckFirewall:
     """Class responsible for running readiness checks and creating Firewall state snapshots.
 
     This class is designed to:
 
-    * run one or more [`FirewallProxy`](/panos-upgrade-assurance/docs/api/firewall-proxy#class-firewallproxy) class methods,
+    * run one or more [`FirewallProxy`](/panos/docs/panos-upgrade-assurance/api/firewall_proxy#class-firewallproxy) class methods,
     * gather and interpret results,
     * present results.
-    
+
     It is split into two parts responsible for:
 
     1. running readiness checks, all methods related to this functionality are prefixed with `check_`,
-    2. running state snapshots, all methods related to this functionality are prefixed with `get_`, although usually the [`FirewallProxy`](/panos-upgrade-assurance/docs/api/firewall-proxy#class-firewallproxy) methods are run directly.
+    2. running state snapshots, all methods related to this functionality are prefixed with `get_`, although usually the [`FirewallProxy`](/panos/docs/panos-upgrade-assurance/api/firewall_proxy#class-firewallproxy) methods are run directly.
 
     Although it is possible to run the methods directly, the preferred way is to run them through one of the following `run` methods:
 
     * [`run_readiness_checks()`](#checkfirewallrun_readiness_checks) is responsible for running specified readiness checks,
     * [`run_snapshots()`](#checkfirewallrun_snapshots) is responsible for getting a snapshot of specified device areas.
 
     # Attributes
 
     _snapshot_method_mapping (dict): Internal variable containing a map of all valid snapshot types mapped to the specific methods.
-    
-    This mapping is used to verify the requested snapshot types and to map the snapshot with an actual method that will eventually run. Keys in this dictionary are snapshot names as defined in the [`SnapType`](/panos-upgrade-assurance/docs/api/utils#class-snaptype) class, values are references to methods that will be run.
 
-    _check_method_mapping (dict): Internal variable containing the map of all valid check types mapped to the specific methods. This mapping is used to verify requested check types and to map a check with an actual method that will be eventually run. Keys in this dictionary are check names as defined in the [`CheckType`](/panos-upgrade-assurance/docs/api/utils#class-checktype) class, values are references to methods that will be run.
+    This mapping is used to verify the requested snapshot types and to map the snapshot with an actual method that will eventually run. Keys in this dictionary are snapshot names as defined in the [`SnapType`](/panos/docs/panos-upgrade-assurance/api/utils#class-snaptype) class, values are references to methods that will be run.
+
+    _check_method_mapping (dict): Internal variable containing the map of all valid check types mapped to the specific methods. This mapping is used to verify requested check types and to map a check with an actual method that will be eventually run. Keys in this dictionary are check names as defined in the [`CheckType`](/panos/docs/panos-upgrade-assurance/api/utils#class-checktype) class, values are references to methods that will be run.
 
     """
 
     def __init__(self, node: FirewallProxy) -> None:
         """CheckFirewall constructor.
 
         # Parameters
 
-        node (FirewallProxy): Object representing a device against which checks and/or snapshots are run. See [`FirewallProxy`](/panos-upgrade-assurance/docs/api/firewall-proxy#class-firewallproxy) class' documentation.
+        node (FirewallProxy): Object representing a device against which checks and/or snapshots are run. See [`FirewallProxy`](/panos/docs/panos-upgrade-assurance/api/firewall_proxy#class-firewallproxy) class' documentation.
 
         """
         self._node = node
         self._snapshot_method_mapping = {
             SnapType.NICS: self._node.get_nics,
             SnapType.ROUTES: self._node.get_routes,
             SnapType.LICENSE: self._node.get_licenses,
             SnapType.ARP_TABLE: self._node.get_arp_table,
             SnapType.CONTENT_VERSION: self.get_content_db_version,
             SnapType.SESSION_STATS: self._node.get_session_stats,
-            SnapType.IPSEC_TUNNELS: self.get_ip_sec_tunnels
+            SnapType.IPSEC_TUNNELS: self.get_ip_sec_tunnels,
         }
 
-        self._check_method_mapping =  {
+        self._check_method_mapping = {
             CheckType.PANORAMA: self.check_panorama_connectivity,
             CheckType.HA: self.check_ha_status,
             CheckType.NTP_SYNC: self.check_ntp_synchronization,
             CheckType.CANDIDATE_CONFIG: self.check_pending_changes,
             CheckType.EXPIRED_LICENSES: self.check_expired_licenses,
             CheckType.ACTIVE_SUPPORT: self.check_active_support_license,
             CheckType.CONTENT_VERSION: self.check_content_version,
             CheckType.SESSION_EXIST: self.check_critical_session,
             CheckType.ARP_ENTRY_EXIST: self.check_arp_entry,
             CheckType.IPSEC_TUNNEL_STATUS: self.check_ipsec_tunnel_status,
             CheckType.FREE_DISK_SPACE: self.check_free_disk_space,
-            CheckType.MP_DP_CLOCK_SYNC: self.check_mp_dp_sync
+            CheckType.MP_DP_CLOCK_SYNC: self.check_mp_dp_sync,
         }
+        locale.setlocale(
+            locale.LC_ALL, "en_US"
+        )  # force locale for datetime string parsing when non-English locale is set on host
 
     def check_pending_changes(self) -> CheckResult:
         """Check if there are pending changes on device.
 
         It checks two states:
 
         1. if there is full commit required on the device,
         2. if not, if there is a candidate config pending on a device.
 
         # Returns
 
-        CheckResult: Object of [`CheckResult`](/panos-upgrade-assurance/docs/api/utils#class-checkresult) class representing the result of the content version check:
+        CheckResult: Object of [`CheckResult`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkresult) class representing the result of the content version check:
 
-        * [`CheckStatus.SUCCESS`](/panos-upgrade-assurance/docs/api/utils#class-checkstatus) if there is no pending configuration,
-        * [`CheckStatus.FAIL`](/panos-upgrade-assurance/docs/api/utils#class-checkstatus) otherwise.
+        * [`CheckStatus.SUCCESS`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) if there is no pending configuration,
+        * [`CheckStatus.FAIL`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) otherwise.
 
         """
         if self._node.is_full_commit_required():
             return CheckResult(reason="Full commit required on device.")
         else:
             if self._node.is_pending_changes():
                 return CheckResult(reason="Pending changes found on device.")
@@ -111,233 +131,249 @@
                 return CheckResult(status=CheckStatus.SUCCESS)
 
     def check_panorama_connectivity(self) -> CheckResult:
         """Check connectivity with the Panorama service.
 
         # Returns
 
-        CheckResult: Object of [`CheckResult`](/panos-upgrade-assurance/docs/api/utils#class-checkresult) class representing a state of Panorama connection:
+        CheckResult: Object of [`CheckResult`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkresult) class representing a state of Panorama connection:
 
-        * [`CheckStatus.SUCCESS`](/panos-upgrade-assurance/docs/api/utils#class-checkstatus) when device is connected to Panorama,
-        * [`CheckStatus.FAIL`](/panos-upgrade-assurance/docs/api/utils#class-checkstatus) otherwise,
-        * [`CheckStatus.ERROR`](/panos-upgrade-assurance/docs/api/utils#class-checkstatus) is returned when no Panorama configuration is found.
+        * [`CheckStatus.SUCCESS`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) when device is connected to Panorama,
+        * [`CheckStatus.FAIL`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) otherwise,
+        * [`CheckStatus.ERROR`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) is returned when no Panorama configuration is found.
 
         """
 
         if self._node.is_panorama_configured():
             if self._node.is_panorama_connected():
                 return CheckResult(status=CheckStatus.SUCCESS)
             else:
                 return CheckResult(reason="Device not connected to Panorama.")
         else:
-            return CheckResult(status=CheckStatus.ERROR, reason="Device not configured with Panorama.")
+            return CheckResult(
+                status=CheckStatus.ERROR, reason="Device not configured with Panorama."
+            )
 
     def check_ha_status(self, skip_config_sync: Optional[bool] = False) -> CheckResult:
         """Checks HA pair status from the perspective of the current device.
 
         Currently, only Active-Passive configuration is supported.
 
         # Parameters:
 
         skip_config_sync (bool, optional): (defaults to `False`) Use with caution, when set to `True` will skip checking if configuration is synchronized between nodes. Helpful when verifying a state of a partially upgraded HA pair.
 
         # Returns
 
-        CheckResult: Object of [`CheckResult`](/panos-upgrade-assurance/docs/api/utils#class-checkresult) class representing results of HA pair status inspection:
+        CheckResult: Object of [`CheckResult`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkresult) class representing results of HA pair status inspection:
 
-        * [`CheckStatus.SUCCESS`](/panos-upgrade-assurance/docs/api/utils#class-checkstatus) when pair is configured correctly,
-        * [`CheckStatus.FAIL`](/panos-upgrade-assurance/docs/api/utils#class-checkstatus) otherwise,
-        * [`CheckStatus.ERROR`](/panos-upgrade-assurance/docs/api/utils#class-checkstatus) is returned when device is not a member of an HA pair or the pair is not in Active-Passive configuration.
+        * [`CheckStatus.SUCCESS`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) when pair is configured correctly,
+        * [`CheckStatus.FAIL`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) otherwise,
+        * [`CheckStatus.ERROR`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) is returned when device is not a member of an HA pair or the pair is not in Active-Passive configuration.
 
         """
         states = ("active", "passive")
 
         ha_config = self._node.get_ha_configuration()
         result = CheckResult()
 
-        if interpret_yes_no(ha_config['enabled']):
-            ha_pair = ha_config['group']
+        if interpret_yes_no(ha_config["enabled"]):
+            ha_pair = ha_config["group"]
 
-            if ha_pair['mode'] != 'Active-Passive':
+            if ha_pair["mode"] != "Active-Passive":
                 result.status = CheckStatus.ERROR
                 result.reason = "HA pair is not in Active-Passive mode."
 
-            elif ha_pair['local-info']['state'] not in states:
+            elif ha_pair["local-info"]["state"] not in states:
                 result.reason = "Local device is not in active or passive state."
 
-            elif ha_pair['peer-info']['state'] not in states:
+            elif ha_pair["peer-info"]["state"] not in states:
                 result.reason = "Peer device is not in active or passive state."
 
-            elif ha_pair['local-info']['state'] == ha_pair['peer-info']['state']:
+            elif ha_pair["local-info"]["state"] == ha_pair["peer-info"]["state"]:
                 result.status = CheckStatus.ERROR
                 result.reason = f"Both devices have the same state: {ha_pair['local-info']['state']}."
 
-            elif not skip_config_sync and interpret_yes_no(ha_pair['running-sync-enabled']) and ha_pair['running-sync'] != 'synchronized':
+            elif (
+                not skip_config_sync
+                and interpret_yes_no(ha_pair["running-sync-enabled"])
+                and ha_pair["running-sync"] != "synchronized"
+            ):
                 result.status = CheckStatus.ERROR
-                result.reason = 'Device configuration is not synchronized between the nodes.'
+                result.reason = (
+                    "Device configuration is not synchronized between the nodes."
+                )
 
             else:
                 result.status = CheckStatus.SUCCESS
         else:
             result.reason = "Device is not a member of an HA pair."
             result.status = CheckStatus.ERROR
 
         return result
 
-    def check_is_ha_active(self, skip_config_sync: Optional[bool] = False) -> CheckResult:
+    def check_is_ha_active(
+        self, skip_config_sync: Optional[bool] = False
+    ) -> CheckResult:
         """Checks whether this is an active node of an HA pair.
 
-        Before checking the state of the current device, the [`check_ha_status()`](#checkfirewallcheck_ha_status) method is run. If this method does not end with [`CheckStatus.SUCCESS`](/panos-upgrade-assurance/docs/api/utils#class-checkstatus), its return value is passed as the result of [`check_is_ha_active()`](#checkfirewallcheck_is_ha_active).
+        Before checking the state of the current device, the [`check_ha_status()`](#checkfirewallcheck_ha_status) method is run. If this method does not end with [`CheckStatus.SUCCESS`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus), its return value is passed as the result of [`check_is_ha_active()`](#checkfirewallcheck_is_ha_active).
 
         Detailed results matrix looks like this:
 
-        * [`CheckStatus.SUCCESS`](/panos-upgrade-assurance/docs/api/utils#class-checkstatus) the actual state of the device in an HA pair is checked, if the state is:
-            * active - [`CheckStatus.SUCCESS`](/panos-upgrade-assurance/docs/api/utils#class-checkstatus) is returned,
-            * passive - [`CheckStatus.FAIL`](/panos-upgrade-assurance/docs/api/utils#class-checkstatus) is returned,
-        * anything else than [`CheckStatus.SUCCESS`](/panos-upgrade-assurance/docs/api/utils#class-checkstatus), the [`check_ha_status()`](#checkfirewallcheck_ha_status) return value is passed as a return value of this method.
+        * [`CheckStatus.SUCCESS`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) the actual state of the device in an HA pair is checked, if the state is:
+            * active - [`CheckStatus.SUCCESS`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) is returned,
+            * passive - [`CheckStatus.FAIL`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) is returned,
+        * anything else than [`CheckStatus.SUCCESS`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus), the [`check_ha_status()`](#checkfirewallcheck_ha_status) return value is passed as a return value of this method.
 
 
         # Parameters
 
         skip_config_sync (bool, optional): (defaults to `False`) Use with caution, when set to `True` will skip checking if configuration is synchronized between nodes. Helpful when working with a partially upgraded HA pair.
-        
+
         # Returns
 
         CheckResult: Boolean information reflecting the state of the device.
 
         """
         ha_status = self.check_ha_status(skip_config_sync=skip_config_sync)
         if ha_status:
             ha_config = self._node.get_ha_configuration()
             result = CheckResult()
-            if ha_config['group']['local-info']['state'] == 'active':
+            if ha_config["group"]["local-info"]["state"] == "active":
                 result.status = CheckStatus.SUCCESS
             else:
-                result.reason = f"Node state is: {ha_config['group']['local-info']['state']}."
+                result.reason = (
+                    f"Node state is: {ha_config['group']['local-info']['state']}."
+                )
             return result
         else:
             return ha_status
 
     def check_expired_licenses(self, skip_licenses: Optional[list] = []) -> CheckResult:
         """Check if any license is expired.
 
         # Parameters
 
         skip_licenses (list, optional): (defaults to `[]`) List of license names that should be skipped during the check.
 
         # Returns
 
-        CheckResult: Object of [`CheckResult`](/panos-upgrade-assurance/docs/api/utils#class-checkresult) class taking value of:
+        CheckResult: Object of [`CheckResult`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkresult) class taking value of:
 
-        * [`CheckStatus.SUCCESS`](/panos-upgrade-assurance/docs/api/utils#class-checkstatus) if no license is expired,
-        * [`CheckStatus.FAIL`](/panos-upgrade-assurance/docs/api/utils#class-checkstatus) otherwise.
+        * [`CheckStatus.SUCCESS`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) if no license is expired,
+        * [`CheckStatus.FAIL`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) otherwise.
 
         """
         if not isinstance(skip_licenses, list):
-            raise WrongDataTypeException(f'The skip_licenses variable is a {type(skip_licenses)} but should be a list')
+            raise WrongDataTypeException(
+                f"The skip_licenses variable is a {type(skip_licenses)} but should be a list"
+            )
 
         licenses = self._node.get_licenses()
 
         expired_licenses = ""
         result = CheckResult()
         for lic, value in licenses.items():
-            if not lic in skip_licenses:
+            if lic not in skip_licenses:
                 if interpret_yes_no(value["expired"]):
                     expired_licenses += f"{lic}, "
 
         if expired_licenses:
             result.reason = f"Found expired licenses:  {expired_licenses[:-2]}."
         else:
             result.status = CheckStatus.SUCCESS
 
         return result
 
     def check_active_support_license(self) -> CheckResult:
         """Check active support license with update server.
-        
+
         # Raises
 
         UpdateServerConnectivityException: Thrown when a connection to an update server cannot be established during support license verification.
 
         # Returns
 
-        dict: Object of [`CheckResult`](/panos-upgrade-assurance/docs/api/utils#class-checkresult) class taking value of:
+        dict: Object of [`CheckResult`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkresult) class taking value of:
 
-        - [`CheckStatus.SUCCESS`](/panos-upgrade-assurance/docs/api/utils#class-checkstatus) if the support license is not expired,
-        - [`CheckStatus.FAIL`](/panos-upgrade-assurance/docs/api/utils#class-checkstatus) otherwise,
-        - [`CheckStatus.ERROR`](/panos-upgrade-assurance/docs/api/utils#class-checkstatus) when no information about the support license expiration date can be found in response from the firewall.
+        - [`CheckStatus.SUCCESS`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) if the support license is not expired,
+        - [`CheckStatus.FAIL`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) otherwise,
+        - [`CheckStatus.ERROR`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) when no information about the support license expiration date can be found in response from the firewall.
 
         """
 
         result = CheckResult()
 
         try:
             support_license = self._node.get_support_license()
         except PanDeviceXapiError as exc:  # raised when connectivity timeouts
-            raise UpdateServerConnectivityException('Can not reach update servers to check active support license.') from exc
+            raise UpdateServerConnectivityException(
+                "Can not reach update servers to check active support license."
+            ) from exc
 
         if not support_license.get("support_expiry_date"):  # if None or empty string
-            result.reason = 'No ExpiryDate found for support license.'
+            result.reason = "No ExpiryDate found for support license."
             result.status = CheckStatus.ERROR
             return result
 
         dt_expiry = datetime.strptime(
-            support_license['support_expiry_date'],
-            "%B %d, %Y"
+            support_license["support_expiry_date"], "%B %d, %Y"
         )
         dt_today = datetime.now()
 
-        if (dt_expiry < dt_today):
-            result.reason = 'Support License expired.'
+        if dt_expiry < dt_today:
+            result.reason = "Support License expired."
         else:
             result.status = CheckStatus.SUCCESS
 
         return result
 
     def check_critical_session(
         self,
         source: Optional[str] = None,
         destination: Optional[str] = None,
-        dest_port: Optional[Union[str, int]] = None) -> CheckResult:
+        dest_port: Optional[Union[str, int]] = None,
+    ) -> CheckResult:
         """Check if a critical session is present in the sessions table.
 
         # Parameters
 
         source (str, optional): (defaults to `None`) Source IPv4 address for the examined session.
         destination (str, optional): (defaults to `None`) Destination IPv4 address for the examined session.
         dest_port (int, str, optional): (defaults to `None`) Destination port value. This should be an integer value, but string representations such as `"8080"` are also accepted.
 
         # Returns
 
-        CheckResult: Object of [`CheckResult`](/panos-upgrade-assurance/docs/api/utils#class-checkresult) class taking value of:
+        CheckResult: Object of [`CheckResult`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkresult) class taking value of:
 
-        * [`CheckStatus.SUCCESS`](/panos-upgrade-assurance/docs/api/utils#class-checkstatus) if a session is found in the sessions table,
-        * [`CheckStatus.FAIL`](/panos-upgrade-assurance/docs/api/utils#class-checkstatus) otherwise,
-        * [`CheckStatus.SKIPPED`](/panos-upgrade-assurance/docs/api/utils#class-checkstatus) when no config is passed,
-        * [`CheckStatus.ERROR`](/panos-upgrade-assurance/docs/api/utils#class-checkstatus) if the session table is empty.
+        * [`CheckStatus.SUCCESS`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) if a session is found in the sessions table,
+        * [`CheckStatus.FAIL`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) otherwise,
+        * [`CheckStatus.SKIPPED`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) when no config is passed,
+        * [`CheckStatus.ERROR`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) if the session table is empty.
 
         """
 
         result = CheckResult()
 
         if None in [source, destination, dest_port]:
-            result.reason = 'Missing critical session description. Failing check.'
+            result.reason = "Missing critical session description. Failing check."
             result.status = CheckStatus.SKIPPED
             return result
 
         sessions = self._node.get_sessions()
         if not sessions:
             result.reason = "Device's session table is empty."
             result.status = CheckStatus.ERROR
             return result
 
         for session in sessions:
-            source_check = session['source'] == source
-            destination_check = session['xdst'] == destination
-            port_check = session['dport'] == str(dest_port)
+            source_check = session["source"] == source
+            destination_check = session["xdst"] == destination
+            port_check = session["dport"] == str(dest_port)
             if all((source_check, destination_check, port_check)):
                 result.status = CheckStatus.SUCCESS
                 return result
 
         result.reason = "Session not found in session table."
         return result
 
@@ -354,111 +390,125 @@
         version (str, optional): (defaults to `None`) Target version of the content DB.
 
         # Raises
 
         ContentDBVersionInFutureException: If the data returned from a device is newer than the latest version available.
 
         # Returns
-        CheckResult: Object of [`CheckResult`](/panos-upgrade-assurance/docs/api/utils#class-checkresult) class taking value off:
+        CheckResult: Object of [`CheckResult`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkresult) class taking value off:
 
-        * [`CheckStatus.SUCCESS`](/panos-upgrade-assurance/docs/api/utils#class-checkstatus) when the installed Content DB met the requirements.
-        * [`CheckStatus.FAIL`](/panos-upgrade-assurance/docs/api/utils#class-checkstatus) when it did not.
+        * [`CheckStatus.SUCCESS`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) when the installed Content DB met the requirements.
+        * [`CheckStatus.FAIL`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) when it did not.
 
         """
         result = CheckResult()
 
-        required_version = version if version else self._node.get_latest_available_content_version()
+        required_version = (
+            version if version else self._node.get_latest_available_content_version()
+        )
         installed_version = self._node.get_content_db_version()
 
         if required_version == installed_version:
             result.status = CheckStatus.SUCCESS
         else:
-            exception_text = f'Wrong data returned from device, installed version ({installed_version}) is higher than the required_version available ({required_version}).'
-            conditional_success_text = f'Installed content DB version ({installed_version}) is higher than the requested one ({required_version}).'
+            exception_text = f"Wrong data returned from device, installed version ({installed_version}) is higher than the required_version available ({required_version})."
+            conditional_success_text = f"Installed content DB version ({installed_version}) is higher than the requested one ({required_version})."
 
             # we already know that the versions are different, so as a default result we assume FAILED
             # now let's handle corner cases
-            if int(required_version.split('-')[0]) < int(installed_version.split('-')[0]):
+            if int(required_version.split("-")[0]) < int(
+                installed_version.split("-")[0]
+            ):
                 # if the passed required version is higher that the installed then we assume the test passed
                 # this is a type of a test where we look for the minimum version
                 if version:
                     result.status = CheckStatus.SUCCESS
                     result.reason = conditional_success_text
                 else:
                     # in case where no version was passed we treat this situation as an exception
-                    # latest version cannot by lower than the installed one. 
+                    # latest version cannot by lower than the installed one.
                     raise ContentDBVersionInFutureException(exception_text)
-            elif int(required_version.split('-')[0]) == int(installed_version.split('-')[0]):
+            elif int(required_version.split("-")[0]) == int(
+                installed_version.split("-")[0]
+            ):
                 # majors the same, compare minors assuming the same logic we used for majors
-                if int(required_version.split('-')[1]) < int(installed_version.split('-')[1]):
+                if int(required_version.split("-")[1]) < int(
+                    installed_version.split("-")[1]
+                ):
                     if version:
                         result.status = CheckStatus.SUCCESS
                         result.reason = conditional_success_text
                     else:
                         raise ContentDBVersionInFutureException(exception_text)
 
             if not result:
-                reason_suffix = f'older then the request one ({required_version}).' if version else f'not the latest one ({required_version}).'
+                reason_suffix = (
+                    f"older then the request one ({required_version})."
+                    if version
+                    else f"not the latest one ({required_version})."
+                )
                 result.reason = f"Installed content DB version ({installed_version}) is {reason_suffix}"
 
         return result
 
     def check_ntp_synchronization(self) -> CheckResult:
         """Check synchronization with NTP server.
 
         # Returns
 
-        CheckResult: Object of [`CheckResult`](/panos-upgrade-assurance/docs/api/utils#class-checkresult) class taking value of:
+        CheckResult: Object of [`CheckResult`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkresult) class taking value of:
 
-        * [`CheckStatus.SUCCESS`](/panos-upgrade-assurance/docs/api/utils#class-checkstatus) when a device is synchronized with the NTP server.
-        * [`CheckStatus.FAIL`](/panos-upgrade-assurance/docs/api/utils#class-checkstatus) when a device is not synchronized with the NTP server.
-        * [`CheckStatus.ERROR`](/panos-upgrade-assurance/docs/api/utils#class-checkstatus) when a device is not configured for NTP synchronization.
+        * [`CheckStatus.SUCCESS`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) when a device is synchronized with the NTP server.
+        * [`CheckStatus.FAIL`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) when a device is not synchronized with the NTP server.
+        * [`CheckStatus.ERROR`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) when a device is not configured for NTP synchronization.
 
         """
 
         result = CheckResult()
-        
+
         response = self._node.get_ntp_servers()
-        if response['synched'] == 'LOCAL':
+        if response["synched"] == "LOCAL":
             if len(response) == 1:
-                result.reason = 'No NTP server configured.'
+                result.reason = "No NTP server configured."
                 result.status = CheckStatus.ERROR
             else:
-                del response['synched']
+                del response["synched"]
                 srvs_state = ""
                 for v in response.values():
                     srvs_state += f"{v['name']} - {v['status']}, "
                 result.reason = f"No NTP synchronization in active, servers in following state: {srvs_state[:-2]}."
         else:
-            synched = response['synched']
-            del response['synched']
+            synched = response["synched"]
+            del response["synched"]
 
-            if synched in [v['name'] for v in response.values()]:
+            if synched in [v["name"] for v in response.values()]:
                 result.status = CheckStatus.SUCCESS
             else:
-                result.reason = f'NTP synchronization in unknown state: {synched}.'
+                result.reason = f"NTP synchronization in unknown state: {synched}."
 
         return result
 
-    def check_arp_entry(self, ip: Optional[str] = None, interface: Optional[str] = None) -> CheckResult:
+    def check_arp_entry(
+        self, ip: Optional[str] = None, interface: Optional[str] = None
+    ) -> CheckResult:
         """Check if a given ARP entry is available in the ARP table.
 
         # Parameters
 
         interface (str, optional): (defaults to `None`) A name of an interface we examine for the ARP entries. When skipped, all interfaces are examined.
         ip (str, optional): (defaults to `None`) IP address of the ARP entry we look for.
 
         # Returns
 
-        CheckResult: Object of [`CheckResult`](/panos-upgrade-assurance/docs/api/utils#class-checkresult) class taking value of:
-        
-        * [`CheckStatus.SUCCESS`](/panos-upgrade-assurance/docs/api/utils#class-checkstatus) when the ARP entry is found.
-        * [`CheckStatus.FAIL`](/panos-upgrade-assurance/docs/api/utils#class-checkstatus) when the ARP entry is not found.
-        * [`CheckStatus.SKIPPED`](/panos-upgrade-assurance/docs/api/utils#class-checkstatus) when `ip` is not provided.
-        * [`CheckStatus.ERROR`](/panos-upgrade-assurance/docs/api/utils#class-checkstatus) when the ARP table is empty.
+        CheckResult: Object of [`CheckResult`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkresult) class taking value of:
+
+        * [`CheckStatus.SUCCESS`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) when the ARP entry is found.
+        * [`CheckStatus.FAIL`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) when the ARP entry is not found.
+        * [`CheckStatus.SKIPPED`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) when `ip` is not provided.
+        * [`CheckStatus.ERROR`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) when the ARP table is empty.
 
         """
 
         result = CheckResult()
 
         if ip is None:
             result.reason = "Missing ARP table entry description."
@@ -470,61 +520,65 @@
         if not arp_table:
             result.reason = "ARP table empty."
             result.status = CheckStatus.ERROR
             return result
 
         for arp_entry in arp_table.values():
             if interface is not None:
-                found = ip == arp_entry.get('ip') and interface == arp_entry.get('interface')
+                found = ip == arp_entry.get("ip") and interface == arp_entry.get(
+                    "interface"
+                )
             else:
-                found = ip == arp_entry.get('ip')
+                found = ip == arp_entry.get("ip")
 
             if found:
                 result.status = CheckStatus.SUCCESS
                 return result
 
         result.reason = "Entry not found in ARP table."
         return result
 
-    def check_ipsec_tunnel_status(self, tunnel_name: Optional[str] = None) -> CheckResult:
+    def check_ipsec_tunnel_status(
+        self, tunnel_name: Optional[str] = None
+    ) -> CheckResult:
         """Check if a given IPSec tunnel is in active state.
 
         # Parameters
 
         tunnel_name (str, optional): (defaults to `None`) Name of the searched IPSec tunnel.
 
         # Returns
 
-        CheckResult: Object of [`CheckResult`](/panos-upgrade-assurance/docs/api/utils#class-checkresult) class taking value of:
- 
-        * [`CheckStatus.SUCCESS`](/panos-upgrade-assurance/docs/api/utils#class-checkstatus) when a tunnel is found and is in active state.
-        * [`CheckStatus.FAIL`](/panos-upgrade-assurance/docs/api/utils#class-checkstatus) when a tunnel is either not active or missing in the current configuration.
-        * [`CheckStatus.SKIPPED`](/panos-upgrade-assurance/docs/api/utils#class-checkstatus) when `tunnel_name` is not provided.
-        * [`CheckStatus.ERROR`](/panos-upgrade-assurance/docs/api/utils#class-checkstatus) when no IPSec tunnels are configured on the device.
+        CheckResult: Object of [`CheckResult`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkresult) class taking value of:
+
+        * [`CheckStatus.SUCCESS`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) when a tunnel is found and is in active state.
+        * [`CheckStatus.FAIL`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) when a tunnel is either not active or missing in the current configuration.
+        * [`CheckStatus.SKIPPED`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) when `tunnel_name` is not provided.
+        * [`CheckStatus.ERROR`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) when no IPSec tunnels are configured on the device.
 
         """
 
         result = CheckResult()
 
         if tunnel_name is None:
             result.status = CheckStatus.SKIPPED
-            result.reason = 'Missing tunnel specification.'
+            result.reason = "Missing tunnel specification."
             return result
-            
+
         tunnels = self._node.get_tunnels()
 
         if not tunnels.get("IPSec"):
-            result.reason = 'No IPSec Tunnel is configured on the device.'
+            result.reason = "No IPSec Tunnel is configured on the device."
             result.status = CheckStatus.ERROR
             return result
 
-        for name in tunnels['IPSec']:
-            data = tunnels['IPSec'][name]
+        for name in tunnels["IPSec"]:
+            data = tunnels["IPSec"][name]
             if name == tunnel_name:
-                if data["state"] == 'active':
+                if data["state"] == "active":
                     result.status = CheckStatus.SUCCESS
                 else:
                     result.reason = f"Tunnel {tunnel_name} in state: {data['state']}."
                 return result
 
         result.reason = f"Tunnel {tunnel_name} not found."
 
@@ -532,119 +586,135 @@
 
     def check_free_disk_space(self, image_version: Optional[str] = None) -> CheckResult:
         """Check if a there is enough space on the `/opt/panrepo` volume for downloading an PanOS image.
 
         This is a check intended to be run before the actual upgrade process starts.
 
         The method operates in two modes:
-        
+
         * default - to be used as last resort, it will verify that the `/opt/panrepo` volume has at least 3GB free space available. This amount of free space is somewhat arbitrary and it's based maximum image sizes (path level + base image) available at the time the method was written (+ some additional error margin).
         * specific target image - suggested mode, it will take one argument `image_version` which is the target PanOS version. For that version the actual image size (path + base image) will be calculated. Next, the available free space is verified against that image size + 10% (as an error margin).
 
         # Parameters
 
-        image_version (str, optional): (defaults to `None`) Version of the target PanOS image. 
+        image_version (str, optional): (defaults to `None`) Version of the target PanOS image.
 
         # Returns
 
-        CheckResult: Object of [`CheckResult`](/panos-upgrade-assurance/docs/api/utils#class-checkresult) class taking value of:
+        CheckResult: Object of [`CheckResult`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkresult) class taking value of:
+
+        * [`CheckStatus.SUCCESS`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) when there is enough free space to download an image.
+        * [`CheckStatus.FAIL`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) when there is NOT enough free space, additionally the actual free space available is provided as the fail reason.
 
-        * [`CheckStatus.SUCCESS`](/panos-upgrade-assurance/docs/api/utils#class-checkstatus) when there is enough free space to download an image.
-        * [`CheckStatus.FAIL`](/panos-upgrade-assurance/docs/api/utils#class-checkstatus) when there is NOT enough free space, additionally the actual free space available is provided as the fail reason.
-        
         """
         result = CheckResult()
         minimum_free_space = ceil(3.0 * 1024)
         if image_version:
             image_sem_version = PanOSVersion(image_version)
             available_versions = self._node.get_available_image_data()
-            
+
             if str(image_sem_version) in available_versions:
                 requested_base_image_size = 0
-                requested_image_size = int(available_versions[str(image_sem_version)]['size'])
+                requested_image_size = int(
+                    available_versions[str(image_sem_version)]["size"]
+                )
 
                 if image_sem_version.patch != 0:
-                    base_image_version = f'{image_sem_version.major}.{image_sem_version.minor}.0'
+                    base_image_version = (
+                        f"{image_sem_version.major}.{image_sem_version.minor}.0"
+                    )
                     if base_image_version in available_versions:
-                        if not interpret_yes_no(available_versions[base_image_version]['downloaded']):
-                            requested_base_image_size = int(available_versions[base_image_version]['size'])
+                        if not interpret_yes_no(
+                            available_versions[base_image_version]["downloaded"]
+                        ):
+                            requested_base_image_size = int(
+                                available_versions[base_image_version]["size"]
+                            )
                     else:
-                        raise ImageVersionNotAvailableException(f'Base image {base_image_version} does not exist.')
-
-                minimum_free_space = ceil(1.1*(requested_base_image_size + requested_image_size))
+                        raise ImageVersionNotAvailableException(
+                            f"Base image {base_image_version} does not exist."
+                        )
+
+                minimum_free_space = ceil(
+                    1.1 * (requested_base_image_size + requested_image_size)
+                )
 
             else:
-                raise ImageVersionNotAvailableException(f'Image {str(image_sem_version)} does not exist.')
+                raise ImageVersionNotAvailableException(
+                    f"Image {str(image_sem_version)} does not exist."
+                )
 
         free_space = self._node.get_disk_utilization()
-        free_space_panrepo = free_space['/opt/panrepo']
+        free_space_panrepo = free_space["/opt/panrepo"]
 
         if free_space_panrepo > minimum_free_space:
             result.status = CheckStatus.SUCCESS
         else:
             result.reason = f"There is not enough free space, only {str(round(free_space_panrepo/1024,1)) + 'G' if free_space_panrepo >= 1024 else str(free_space_panrepo) + 'M'}B is available."
         return result
 
     def check_mp_dp_sync(self, diff_threshold: int = 0) -> CheckResult:
         """Check if the Data and Management clocks are in sync.
 
         # Parameters
 
-        diff_threshold (int, optional): (defaults to `0`) Maximum allowable difference in seconds between both clocks. 
+        diff_threshold (int, optional): (defaults to `0`) Maximum allowable difference in seconds between both clocks.
 
         # Returns
 
-        CheckResult: Object of [`CheckResult`](/panos-upgrade-assurance/docs/api/utils#class-checkresult) class taking value of:
+        CheckResult: Object of [`CheckResult`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkresult) class taking value of:
 
-        * [`CheckStatus.SUCCESS`](/panos-upgrade-assurance/docs/api/utils#class-checkstatus) when both clocks are the same or within threshold.
-        * [`CheckStatus.FAIL`](/panos-upgrade-assurance/docs/api/utils#class-checkstatus) when both clocks differ.
+        * [`CheckStatus.SUCCESS`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) when both clocks are the same or within threshold.
+        * [`CheckStatus.FAIL`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) when both clocks differ.
 
         """
         if not isinstance(diff_threshold, int):
-            raise WrongDataTypeException(f"[diff_threshold] should be of type [int] but is of type [{type(diff_threshold)}].")
+            raise WrongDataTypeException(
+                f"[diff_threshold] should be of type [int] but is of type [{type(diff_threshold)}]."
+            )
 
         result = CheckResult()
 
         mp_clock = self._node.get_mp_clock()
         dp_clock = self._node.get_dp_clock()
 
         mp_dt = datetime.strptime(
             f"{mp_clock['year']}-{mp_clock['month']}-{mp_clock['day']} {mp_clock['time']}",
-            "%Y-%b-%d %H:%M:%S"
+            "%Y-%b-%d %H:%M:%S",
         )
         dp_dt = datetime.strptime(
             f"{dp_clock['year']}-{dp_clock['month']}-{dp_clock['day']} {dp_clock['time']}",
-            "%Y-%b-%d %H:%M:%S"
+            "%Y-%b-%d %H:%M:%S",
         )
 
         time_fluctuation = abs((mp_dt - dp_dt).total_seconds())
         if time_fluctuation > diff_threshold:
             result.reason = f"The data plane clock and management clock are different by {time_fluctuation} seconds."
         else:
             result.status = CheckStatus.SUCCESS
 
         return result
 
-    def get_content_db_version(self) -> Dict[str,str]:
+    def get_content_db_version(self) -> Dict[str, str]:
         """Get Content DB version.
-        
+
         # Returns
 
         dict(str): To keep the standard of all `get` methods returning a dictionary this value is also returned as a dictionary in the following format:
 
         ``` yaml
         {
             'version': 'xxxx-yyyy'
         }
         ```
 
         """
-        return {'version': self._node.get_content_db_version()}
+        return {"version": self._node.get_content_db_version()}
 
-    def get_ip_sec_tunnels(self) -> Dict[str,Union[str,int]]:
+    def get_ip_sec_tunnels(self) -> Dict[str, Union[str, int]]:
         """Extract information about IPSEC tunnels from all tunnel data retrieved from a device.
 
         # Returns
 
         dict: Currently configured IPSEC tunnels. The returned value is similar to the example below. It can differ though depending on the version of PanOS:
 
         ``` yaml
@@ -661,81 +731,96 @@
                 "owner": "1",
                 "id": "1"
             }
         }
         ```
 
         """
-        return self._node.get_tunnels()['IPSec']
-
+        return self._node.get_tunnels()["IPSec"]
 
     def run_readiness_checks(
         self,
         checks_configuration: Optional[List[Union[str, dict]]] = None,
-        report_style: bool = False
-    ) -> Union[Dict[str, dict], Dict[str,str]]:
+        report_style: bool = False,
+    ) -> Union[Dict[str, dict], Dict[str, str]]:
         """Run readiness checks.
 
-        This method provides a convenient way of running readiness checks methods. For details on configuration see [readiness checks](/panos-upgrade-assurance/docs/configuration-details#readiness-checks) documentation.
+        This method provides a convenient way of running readiness checks methods. For details on configuration see [readiness checks](/panos/docs/panos-upgrade-assurance/configuration-details#readiness-checks) documentation.
 
         # Parameters
 
         checks_configuration (list(str,dict), optional): (defaults to `None`) List of readiness checks to run.
         report_style (bool): (defaults to `False`) Changes the output to more descriptive. Can be used when generating a report from the checks.
 
         # Raises
-        
+
         WrongDataTypeException: An exception is raised when the configuration is in a data type different then `str` or `dict`.
 
         # Returns
 
         dict: Results of all configured checks.
 
         """
         result = {}
-        checks_list = ConfigParser(valid_elements=set(self._check_method_mapping.keys()),
-                                   requested_config=checks_configuration).prepare_config()
+        checks_list = ConfigParser(
+            valid_elements=set(self._check_method_mapping.keys()),
+            requested_config=checks_configuration,
+        ).prepare_config()
 
         for check in checks_list:
             if isinstance(check, dict):
                 check_type, check_config = next(iter(check.items()))
                 # check_result = self._check_method_mapping[check_type](check_config)
             elif isinstance(check, str):
                 check_type, check_config = check, {}
                 # check_result = self._check_method_mapping[check_type]()
             else:
-                raise WrongDataTypeException(f'Wrong configuration format for check: {check}.')
-
-            check_result = self._check_method_mapping[check_type](**check_config)  # (**) would pass dict config values as seperate parameters to method.
-            result[check_type] = str(check_result) if report_style else {'state': bool(check_result), 'reason': str(check_result)}
+                raise WrongDataTypeException(
+                    f"Wrong configuration format for check: {check}."
+                )
+
+            check_result = self._check_method_mapping[check_type](
+                **check_config
+            )  # (**) would pass dict config values as seperate parameters to method.
+            result[check_type] = (
+                str(check_result)
+                if report_style
+                else {"state": bool(check_result), "reason": str(check_result)}
+            )
 
         return result
 
-    def run_snapshots(self, snapshots_config: Optional[List[Union[str, dict]]] = None) -> Dict[str, dict]:
+    def run_snapshots(
+        self, snapshots_config: Optional[List[Union[str, dict]]] = None
+    ) -> Dict[str, dict]:
         """Run snapshots of different firewall areas states.
 
-        This method provides a convenient way of running snapshots of a device state. For details on configuration see [state snapshots](/panos-upgrade-assurance/docs/configuration-details#state-snapshots) documentation.
+        This method provides a convenient way of running snapshots of a device state. For details on configuration see [state snapshots](/panos/docs/panos-upgrade-assurance/configuration-details#state-snapshots) documentation.
 
         # Parameters
 
         snapshots_config (list(str), optional): (defaults to `None`) Defines snapshots of which areas will be taken.
-        
+
         # Raises
 
         WrongDataTypeException: An exception is raised when the configuration in a data type is different than in a string.
 
         # Returns
 
-        dict: The results of the executed snapshots. 
+        dict: The results of the executed snapshots.
 
         """
         result = {}
-        snaps_list = ConfigParser(valid_elements=set(self._snapshot_method_mapping.keys()),
-                                  requested_config=snapshots_config).prepare_config()
+        snaps_list = ConfigParser(
+            valid_elements=set(self._snapshot_method_mapping.keys()),
+            requested_config=snapshots_config,
+        ).prepare_config()
 
         for snap_type in snaps_list:
             if not isinstance(snap_type, str):
-                raise WrongDataTypeException(f'Wrong configuration format for snapshot: {snap_type}.')
+                raise WrongDataTypeException(
+                    f"Wrong configuration format for snapshot: {snap_type}."
+                )
 
             result[snap_type] = self._snapshot_method_mapping[snap_type]()
 
         return result
```

### Comparing `panos_upgrade_assurance-0.0.1/panos_upgrade_assurance/firewall_proxy.py` & `panos_upgrade_assurance-0.0.2/panos_upgrade_assurance/firewall_proxy.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,81 +1,99 @@
 import xml.etree.ElementTree as ET
 from panos_upgrade_assurance.utils import interpret_yes_no
 from xmltodict import parse as XMLParse
-from typing import Optional, Union, Dict, List
+from typing import Optional, Union
 from panos.firewall import Firewall
 from math import floor
 
+
 class CommandRunFailedException(Exception):
     """Used when a command run on a device does not return the `success` status."""
+
     pass
 
+
 class MalformedResponseException(Exception):
     """A generic exception class used when a response does not meet the expected standards."""
+
     pass
 
+
 class ContentDBVersionsFormatException(Exception):
     """Used when parsing Content DB versions fail due to an unknown version format (assuming `XXXX-YYYY`)."""
+
     pass
 
+
 class PanoramaConfigurationMissingException(Exception):
     """Used when checking Panorama connectivity on a device that was not configured with Panorama."""
+
     pass
 
+
 class WrongDiskSizeFormatException(Exception):
     """Used when parsing free disk size information."""
+
     pass
 
+
 class FirewallProxy(Firewall):
     """Class representing a Firewall.
 
-    Proxy in this class means that it is between the *high level* [`CheckFirewall`](/panos-upgrade-assurance/docs/api/check-firewall#class-checkfirewall) class and a device itself.
+    Proxy in this class means that it is between the *high level* [`CheckFirewall`](/panos/docs/panos-upgrade-assurance/api/check_firewall#class-checkfirewall) class and a device itself.
     Inherits the [Firewall][fw] class but adds methods to interpret XML API commands. The class constructor is also inherited from the [Firewall][fw] class.
 
     All interaction with a device are read-only. Therefore, a less privileged user can be used.
 
     All methods starting with `is_` check the state, they do not present any data besides simple `boolean`values.
 
-    All methods starting with `get_` fetch data from a device by running a command and parsing the output. 
+    All methods starting with `get_` fetch data from a device by running a command and parsing the output.
     The return data type can be different depending on what kind of information is returned from a device.
 
     [fw]: https://pan-os-python.readthedocs.io/en/latest/module-firewall.html#module-panos.firewall
     """
-    
-    def op_parser(self, cmd: str, cmd_in_xml: Optional[bool] = False, return_xml: Optional[bool] = False) -> Union[dict, ET.Element]:
+
+    def op_parser(
+        self,
+        cmd: str,
+        cmd_in_xml: Optional[bool] = False,
+        return_xml: Optional[bool] = False,
+    ) -> Union[dict, ET.Element]:
         """Execute a command on node, parse, and return response.
 
         This is just a wrapper around the [`Firewall.op()`](https://pan-os-python.readthedocs.io/en/latest/module-firewall.html#panos.firewall.Firewall.op) method. It additionally does basic error handling and tries to extract the actual device response.
 
         # Parameters
 
         cmd (str): The actual XML API command to be run on the device. Can be either a free form or an XML formatted command.
         cmd_in_xml (bool): (defaults to `False`) Set to `True` if the command is XML-formatted.
-        return_xml (bool): (defaults to `False`) When set to `True`, the return data is an [`XML object`](https://docs.python.org/3/library/xml.etree.elementtree.html#xml.etree.ElementTree.Element) instead of a python dictionary. 
+        return_xml (bool): (defaults to `False`) When set to `True`, the return data is an [`XML object`](https://docs.python.org/3/library/xml.etree.elementtree.html#xml.etree.ElementTree.Element) instead of a python dictionary.
 
         # Raises
 
         CommandRunFailedException: An exception is raised if the command run status returned by a device is not successful.
-        MalformedResponseException: An exception is raised when a response is not parsable, no `result` element is found in the XML response. 
+        MalformedResponseException: An exception is raised when a response is not parsable, no `result` element is found in the XML response.
 
         # Returns
         dict, xml.etree.ElementTree.Element: The actual command output. A type is defined by the `return_xml` parameter.
 
         """
 
         raw_response = self.op(cmd, xml=False, cmd_xml=not cmd_in_xml, vsys=self.vsys)
-        if raw_response.get('status') != 'success':
-            raise CommandRunFailedException(f'Failed to run command: {cmd}.')
+        if raw_response.get("status") != "success":
+            raise CommandRunFailedException(f"Failed to run command: {cmd}.")
 
-        resp_result = raw_response.find('result')
+        resp_result = raw_response.find("result")
         if resp_result is None:
-            raise MalformedResponseException(f'No result field returned for: {cmd}')
+            raise MalformedResponseException(f"No result field returned for: {cmd}")
 
         if not return_xml:
-            resp_result = XMLParse(ET.tostring(resp_result, encoding='utf8', method='xml'))['result']
+            resp_result = XMLParse(
+                ET.tostring(resp_result, encoding="utf8", method="xml")
+            )["result"]
 
         return resp_result
 
     def is_pending_changes(self) -> bool:
         """Get information if there is a candidate configuration pending to be committed.
 
         The actual API command run is `check pending-changes`.
@@ -111,30 +129,30 @@
         """
         return False if self.op_parser(cmd="show panorama-status") is None else True
 
     def is_panorama_connected(self) -> bool:
         """Get Panorama connectivity status.
 
         The actual API command run is `show panorama-status`.
-        
+
         An output of this command is usually a string. This method is responsible for parsing this string and trying to extract information if at least one of the Panoramas configured is connected.
 
         Since the API response is a string (that we need to parse) this method expects a strict format. For single Panorama this is:
 
         ```python
-        
+
             Panorama Server 1 : 1.2.3.4
                 Connected     : no
                 HA state      : disconnected
         ```
 
         For two Panoramas (HA pair for example) those are just two blocks:
 
         ```python
-        
+
             Panorama Server 1 : 1.2.3.4
                 Connected     : no
                 HA state      : disconnected
             Panorama Server 2 : 5.6.7.8
                 Connected     : yes
                 HA state      : disconnected
         ```
@@ -150,32 +168,38 @@
         # Returns
 
         bool: `True` when connection is up, `False` otherwise.
 
         """
 
         pan_status = self.op_parser(cmd="show panorama-status")
-        if pan_status == None:
-            raise PanoramaConfigurationMissingException("Device not configured with Panorama.")
+        if pan_status is None:
+            raise PanoramaConfigurationMissingException(
+                "Device not configured with Panorama."
+            )
 
         if not isinstance(pan_status, str):
-            raise MalformedResponseException("Response from device is not type of string.")
+            raise MalformedResponseException(
+                "Response from device is not type of string."
+            )
 
-        pan_status_list = pan_status.split('\n')
+        pan_status_list = pan_status.split("\n")
         pan_status_list_length = len(pan_status_list)
 
-        if pan_status_list_length in [3,6]:
-            for i in range(1,pan_status_list_length,3):
+        if pan_status_list_length in [3, 6]:
+            for i in range(1, pan_status_list_length, 3):
                 pan_connected = interpret_yes_no(
-                    (pan_status_list[i].split(':')[1]).strip()
+                    (pan_status_list[i].split(":")[1]).strip()
                 )
                 if pan_connected:
                     return True
         else:
-            raise MalformedResponseException(f"Panorama configuration block does not have typical structure: <{resp}>.")
+            raise MalformedResponseException(
+                f"Panorama configuration block does not have typical structure: <{pan_status}>."
+            )
 
         return False
 
     def get_ha_configuration(self) -> dict:
         """Get high-availability configuration status.
 
         The actual API command is `show high-availability state`.
@@ -309,54 +333,56 @@
 
     def get_nics(self) -> dict:
         """Get status of the configured network interfaces.
 
         The actual API command run is `show interface "hardware"`.
 
         # Raises
-        
+
         MalformedResponseException: Exception when no `hw` entry is available in the response.
 
         # Returns
 
         dict: Status of the configured network interfaces. Sample output:
 
         ```yaml
         {
-            'ethernet1/1': 'down', 
-            'ethernet1/2': 'down', 
+            'ethernet1/1': 'down',
+            'ethernet1/2': 'down',
             'ethernet1/3': 'up'
         }
         ```
 
         """
 
         response = self.op_parser(cmd=r'show interface "hardware"')
 
-        hardware = response['hw']
+        hardware = response["hw"]
         if hardware is None:
-            raise MalformedResponseException('Malformed response from device, no [hw] element present.')
+            raise MalformedResponseException(
+                "Malformed response from device, no [hw] element present."
+            )
 
         results = {}
-        entries = hardware['entry']
+        entries = hardware["entry"]
         if isinstance(entries, dict):
             entries = [entries]
         for nic in entries:
-            results[nic['name']] = nic['state']
+            results[nic["name"]] = nic["state"]
         return results
 
     def get_licenses(self) -> dict:
         """Get device licenses.
 
         The actual API command is `request license info`.
 
         # Returns
 
         dict: Licenses available on a device.. Sample output:
-            
+
         ```yaml
         {
             'AutoFocus Device License': {
                 'authcode': 'Snnnnnnn',
                 'base-license-name': 'PA-VM',
                 'description': 'AutoFocus Device License',
                 'expired': 'yes',
@@ -378,17 +404,17 @@
         }
         ```
 
         """
         response = self.op_parser(cmd="request license info")
 
         result = {}
-        licenses = response['licenses']['entry']
+        licenses = response["licenses"]["entry"]
         for lic in licenses if isinstance(licenses, list) else [licenses]:
-            result[lic['feature']] = dict(lic)
+            result[lic["feature"]] = dict(lic)
         return result
 
     def get_support_license(self) -> dict:
         """Get support license information from update servers.
 
         The actual API command is `request support check`.
 
@@ -427,29 +453,33 @@
 
         - the expiry date,
         - the support level.
         """
         result = {}
         response = self.op_parser(cmd="request support check", return_xml=True)
 
-        result['support_expiry_date'] = response.findtext('./SupportInfoResponse/Support/ExpiryDate')
-        result['support_level'] = response.findtext('./SupportInfoResponse/Support/SupportLevel')
+        result["support_expiry_date"] = response.findtext(
+            "./SupportInfoResponse/Support/ExpiryDate"
+        )
+        result["support_level"] = response.findtext(
+            "./SupportInfoResponse/Support/SupportLevel"
+        )
         return result
 
     def get_routes(self) -> dict:
         """Get route table entries, either retrieved from DHCP or configured manually.
 
         The actual API command is `show routing route`.
 
         In the returned `dict` the key is made of three route properties delimited with an underscore (`_`) in the following order:
-        
+
         * virtual router name,
         * destination CIDR,
         * network interface name if one is available, empty string otherwise.
-        
+
         The key does not provide any meaningful information, it's there only to introduce uniqueness for each entry. All properties that make a key are also available in the value of a dictionary element. Sample output:
 
         ```yaml
         {
             private_0.0.0.0/0_private/i3': {
                 'age': None,
                 'destination': '0.0.0.0/0',
@@ -470,41 +500,41 @@
                 'route-table': 'unicast',
                 'virtual-router': 'public'
             }
         }
         ```
 
         # Returns
-        
+
         dict: Routes information.
 
         """
 
         response = self.op_parser(cmd="show routing route")
 
         result = {}
-        if 'entry' in response:
-            routes = response['entry']
+        if "entry" in response:
+            routes = response["entry"]
             for route in routes if isinstance(routes, list) else [routes]:
                 result[
-                    f"{route['virtual-router']}_{route['destination']}_{route['interface'] if route['interface'] else ''}"] = dict(
-                    route)
+                    f"{route['virtual-router']}_{route['destination']}_{route['interface'] if route['interface'] else ''}"
+                ] = dict(route)
 
         return result
 
     def get_arp_table(self) -> dict:
         """Get the currently available ARP table entries.
 
         The actual API command is `<show><arp><entry name = 'all'/></arp></show>`.
 
         In the returned `dict` the key is made of two properties delimited with an underscore (`_`) in the following order:
-            
+
         * interface name,
         * IP address.
-            
+
         The key does not provide any meaningful information, it's there only to introduce uniqueness for each entry. All properties that make a key are also available in the value of a dictionary element. Sample output:
 
         ```yaml
         {
             'ethernet1/1_10.0.2.1': {
                 'interface': 'ethernet1/1',
                 'ip': '10.0.2.1',
@@ -521,34 +551,36 @@
                 'status': 'c',
                 'ttl': '1094'
             }
         }
         ```
 
         # Returns
-        
-        dict: ARP table entries. 
+
+        dict: ARP table entries.
 
         """
         result = {}
-        response = self.op_parser(cmd=f"<show><arp><entry name = 'all'/></arp></show>", cmd_in_xml=True)
+        response = self.op_parser(
+            cmd="<show><arp><entry name = 'all'/></arp></show>", cmd_in_xml=True
+        )
 
         if response.get("entries", {}):
-            arp_table = response['entries'].get("entry", [])
+            arp_table = response["entries"].get("entry", [])
             for entry in arp_table if isinstance(arp_table, list) else [arp_table]:
                 result[f'{entry["interface"]}_{entry["ip"]}'] = dict(entry)
         return result
 
     def get_sessions(self) -> list:
         """Get information about currently running sessions.
 
         The actual API command run is `show session all`.
 
         # Returns
-        
+
         list: Information about the current sessions. Sample output:
 
         ```yaml
         [
             {
                 'application': 'undecided',
                 'decrypt-mirror': 'False',
@@ -580,17 +612,17 @@
             },
             ...
         ]
         ```
 
         """
         result = []
-        raw_response = self.op_parser(cmd='show session all')
-        if not raw_response is None:
-            sessions = raw_response['entry']
+        raw_response = self.op_parser(cmd="show session all")
+        if raw_response is not None:
+            sessions = raw_response["entry"]
             result = sessions if isinstance(sessions, list) else [sessions]
 
         return result
 
     def get_session_stats(self) -> dict:
         """Get basic session statistics.
 
@@ -598,15 +630,15 @@
 
         **NOTE**
         This is raw output. Names of stats are the same as returned by API. No translation is made on purpose. The output of this command might vary depending on the version of PanOS.
 
         For meaning and available statistics, refer to the official PanOS documentation.
 
         # Returns
-        
+
         dict: Session stats in a form of a dictionary. Sample output:
 
         ```yaml
         {
             'age-accel-thresh': '80',
             'age-accel-tsf': '2',
             'age-scan-ssf': '8',
@@ -694,58 +726,70 @@
             },
             'SSL-VPN': {},
             'hop': {}
         }
         ```
 
         """
-        response = self.op_parser(cmd='show running tunnel flow all')
+        response = self.op_parser(cmd="show running tunnel flow all")
         result = {}
         for tunnelType, tunnelData in dict(response).items():
             if tunnelData is None:
                 result[tunnelType] = dict()
             elif not isinstance(tunnelData, str):
                 result[tunnelType] = dict()
-                for tunnel in tunnelData['entry'] if isinstance(tunnelData['entry'], list) else [tunnelData['entry']]:
-                    result[tunnelType][tunnel['name']] = dict(tunnel)
+                for tunnel in (
+                    tunnelData["entry"]
+                    if isinstance(tunnelData["entry"], list)
+                    else [tunnelData["entry"]]
+                ):
+                    result[tunnelType][tunnel["name"]] = dict(tunnel)
         return result
 
     def get_latest_available_content_version(self) -> str:
         """Get the latest, downloadable content version.
 
         The actual API command run is `request content upgrade check`.
 
         Values returned by API are not ordered. This method tries to reorder them and find the highest available Content DB version. The following assumptions are made:
 
         * versions are always increasing,
         * both components of the version string are numbers.
 
         # Raises
-        
+
         ContentDBVersionsFormatException: An exception is thrown when the Content DB version does not match the expected format.
 
         # Returns
 
         str: The latest available content version. Sample output:
 
-        ```python 
+        ```python
         '8670-7824'
         ```
 
         """
         response = self.op_parser(cmd="request content upgrade check", return_xml=False)
         try:
-            content_versions = [ entry['version'] for entry in response['content-updates']['entry'] ]
-            majors = [ int(ver.split('-')[0]) for ver in content_versions ]
+            content_versions = [
+                entry["version"] for entry in response["content-updates"]["entry"]
+            ]
+            majors = [int(ver.split("-")[0]) for ver in content_versions]
             majors.sort()
-            major_minors = [ int(ver.split('-')[1]) for ver in content_versions if ver.startswith(f"{majors[-1]}-") ]
+            major_minors = [
+                int(ver.split("-")[1])
+                for ver in content_versions
+                if ver.startswith(f"{majors[-1]}-")
+            ]
             major_minors.sort()
             latest = f"{majors[-1]}-{major_minors[-1]}"
         except Exception as exc:
-            raise ContentDBVersionsFormatException('Cannot parse list of available updates for Content DB.') from exc
+            raise ContentDBVersionsFormatException(
+                "Cannot parse list of available updates for Content DB."
+            ) from exc
 
         return latest
 
     def get_content_db_version(self) -> str:
         """Get the currently installed Content DB version.
 
         The actual API command is `show system info`.
@@ -756,22 +800,22 @@
 
         ```python
         '8670-7824'
         ```
 
         """
         response = self.op_parser(cmd="show system info", return_xml=True)
-        return response.findtext('./system/app-version')
+        return response.findtext("./system/app-version")
 
     def get_ntp_servers(self) -> dict:
         """Get the NTP synchronization configuration.
 
         The actual API command is `show ntp`.
 
-        The actual return value of this method can differ depending on whether the NTP servers are configured or not: 
+        The actual return value of this method can differ depending on whether the NTP servers are configured or not:
 
         - no NTP servers configured:
 
             ```yaml
             {
                 'synched': 'LOCAL'
             }
@@ -796,15 +840,15 @@
                 'synched': '1.pool.ntp.org'
             }
             ```
 
         # Returns
 
         dict: The NTP synchronization configuration.
-        
+
 
         """
         return dict(self.op_parser(cmd="show ntp"))
 
     def get_disk_utilization(self) -> dict:
         """Get the disk utilization (in MB) and parse it to a machine readable format.
 
@@ -827,37 +871,37 @@
         }
         ```
 
         """
         result = dict()
 
         disk_space = self.op_parser(cmd="show system disk-space")
-        disk_space_list = disk_space.split('\n')
+        disk_space_list = disk_space.split("\n")
 
         # we start with index 1 to skip header
-        for i in range(1,len(disk_space_list)):
+        for i in range(1, len(disk_space_list)):
             row = disk_space_list[i]
-            row_items = row.split(' ')
-            row_items_trimmed = [item for item in row_items if item != '']
-                
+            row_items = row.split(" ")
+            row_items_trimmed = [item for item in row_items if item != ""]
+
             mount_point = row_items_trimmed[-1]
             free_size_short = row_items_trimmed[3]
             free_size_name = free_size_short[-1]
             free_size_number = float(free_size_short[0:-1])
 
             if isinstance(free_size_name, str):
-                if free_size_name == 'G':
-                    free_size = free_size_number*1024
-                elif free_size_name == 'M':
+                if free_size_name == "G":
+                    free_size = free_size_number * 1024
+                elif free_size_name == "M":
                     free_size = free_size_number
-                elif free_size_name == 'K':
-                    free_size = free_size_number/1024
+                elif free_size_name == "K":
+                    free_size = free_size_number / 1024
 
             elif isinstance(free_size_name, int):
-                free_size = free_size_short/1024/1024
+                free_size = free_size_short / 1024 / 1024
 
             else:
                 raise WrongDiskSizeFormatException("Free disk size has wrong format.")
 
             result[mount_point] = floor(free_size)
 
         return result
@@ -901,17 +945,17 @@
         }
         ```
 
         """
         result = dict()
 
         image_data = self.op_parser(cmd="request system software check")
-        images = dict(image_data['sw-updates']['versions'])['entry']
+        images = dict(image_data["sw-updates"]["versions"])["entry"]
         for image in images if isinstance(images, list) else [images]:
-            result[image['version']] = dict(image)
+            result[image["version"]] = dict(image)
 
         return result
 
     def get_mp_clock(self) -> dict:
         """Get the clock information from management plane.
 
         The actual API command is `show clock`.
@@ -929,25 +973,25 @@
             'year': '2023',
             'day_of_week': 'Wed'
         }
         ```
 
         """
         time_string = self.op_parser(cmd="show clock")
-        time_dict = time_string.split(' ')
+        time_dict = time_string.split(" ")
         result = {
-            'time': time_dict[3],
-            'tz':  time_dict[4],
-            'day':  time_dict[2],
-            'month':  time_dict[1],
-            'year':  time_dict[5],
-            'day_of_week':  time_dict[0],
+            "time": time_dict[3],
+            "tz": time_dict[4],
+            "day": time_dict[2],
+            "month": time_dict[1],
+            "year": time_dict[5],
+            "day_of_week": time_dict[0],
         }
-        
-        return(result)
+
+        return result
 
     def get_dp_clock(self) -> dict:
         """Get the clock information from data plane.
 
         The actual API command is `show clock more`.
 
         # Returns
@@ -963,19 +1007,19 @@
             'year': '2023',
             'day_of_week': 'Wed'
         }
         ```
 
         """
         response = self.op_parser(cmd="show clock more")
-        time_string = dict(response)['member']
-        time_dict = time_string.split(' ')
+        time_string = dict(response)["member"]
+        time_dict = time_string.split(" ")
         result = {
-            'time': time_dict[5],
-            'tz':  time_dict[6],
-            'day':  time_dict[4],
-            'month':  time_dict[3],
-            'year':  time_dict[7],
-            'day_of_week':  time_dict[2],
+            "time": time_dict[5],
+            "tz": time_dict[6],
+            "day": time_dict[4],
+            "month": time_dict[3],
+            "year": time_dict[7],
+            "day_of_week": time_dict[2],
         }
-        
-        return(result)
+
+        return result
```

### Comparing `panos_upgrade_assurance-0.0.1/panos_upgrade_assurance/snapshot_compare.py` & `panos_upgrade_assurance-0.0.2/panos_upgrade_assurance/snapshot_compare.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,50 +1,56 @@
 from typing import Optional, Union, List, Dict
 from panos_upgrade_assurance.utils import ConfigParser, SnapType
 
 
 class MissingKeyException(Exception):
     """Used when an exception about the missing keys in a dictionary is thrown."""
+
     pass
 
+
 class WrongDataTypeException(Exception):
     """Used when a variable does not meet the data type requirements."""
+
     pass
 
+
 class SnapshotSchemeMismatchException(Exception):
     """Used when a snapshot element contains different properties in both snapshots."""
+
     pass
 
 
 class SnapshotCompare:
     """Class comparing snapshots of Firewall Nodes.
 
-    This object can be used to compare two Firewall snapshots made with the [CheckFirewall.run_snapshots()](/panos-upgrade-assurance/docs/api/check-firewall#checkfirewallrun_snapshots) method and present results of this comparison.
-    Its main purpose is to compare two snapshots made with the [`CheckFirewall`](/panos-upgrade-assurance/docs/api/check-firewall#class-checkfirewall) class. However, the code is generic enough to compare any two dictionaries as long as they follow the schema below:
+    This object can be used to compare two Firewall snapshots made with the [CheckFirewall.run_snapshots()](/panos/docs/panos-upgrade-assurance/api/check_firewall#checkfirewallrun_snapshots) method and present results of this comparison.
+    Its main purpose is to compare two snapshots made with the [`CheckFirewall`](/panos/docs/panos-upgrade-assurance/api/check_firewall#class-checkfirewall) class. However, the code is generic enough to compare any two dictionaries as long as they follow the schema below:
 
     ```yaml
     {
         'root_key': {
             'key': value
         }
     }
     ```
 
     Where:
 
-    * `root_key` has to be present and mapped to a method in the `self._functions_mapping` variable in order to be recognized during a comparison. 
-    * `value` can be either of a simple type (`str`, `int`, `float`, `bool`) or a nested `dict`. 
+    * `root_key` has to be present and mapped to a method in the `self._functions_mapping` variable in order to be recognized during a comparison.
+    * `value` can be either of a simple type (`str`, `int`, `float`, `bool`) or a nested `dict`.
 
     # Attributes
 
     _functions_mapping (dict): Internal variable containing the map of all valid report types mapped to the specific methods.
-        
-    This mapping is used to verify the requested report and to map the report to an actual method that will eventually run. Keys in this dictionary are report names as defined in the [`SnapType`](/panos-upgrade-assurance/docs/api/utils#class-snaptype) class. Essentially, these are the same values that one would specify when creating a snapshot with the [CheckFirewall.run_snapshots()](/panos-upgrade-assurance/docs/api/check-firewall#checkfirewallrun_snapshots) method. Values are references to the methods that will run.
+
+    This mapping is used to verify the requested report and to map the report to an actual method that will eventually run. Keys in this dictionary are report names as defined in the [`SnapType`](/panos/docs/panos-upgrade-assurance/api/utils#class-snaptype) class. Essentially, these are the same values that one would specify when creating a snapshot with the [CheckFirewall.run_snapshots()](/panos/docs/panos-upgrade-assurance/api/check_firewall#checkfirewallrun_snapshots) method. Values are references to the methods that will run.
 
     """
+
     def __init__(
         self,
         left_snapshot: Dict[str, Union[str, dict]],
         right_snapshot: Dict[str, Union[str, dict]],
     ) -> None:
         """SnapshotCompare constructor.
 
@@ -61,109 +67,127 @@
         self._functions_mapping = {
             SnapType.NICS: self.get_diff_and_threshold,
             SnapType.ROUTES: self.get_diff_and_threshold,
             SnapType.LICENSE: self.get_diff_and_threshold,
             SnapType.ARP_TABLE: self.get_diff_and_threshold,
             SnapType.CONTENT_VERSION: self.get_diff_and_threshold,
             SnapType.SESSION_STATS: self.get_count_change_percentage,
-            SnapType.IPSEC_TUNNELS: self.get_diff_and_threshold
+            SnapType.IPSEC_TUNNELS: self.get_diff_and_threshold,
         }
 
     def compare_snapshots(
-        self,
-        reports: Optional[List[Union[dict, str]]] = None
+        self, reports: Optional[List[Union[dict, str]]] = None
     ) -> Dict[str, dict]:
         """A method that triggers the actual snapshot comparison.
 
         This is a single point of entry to generate a comparison report. It takes both reports stored in the class object and compares areas specified in the `reports` parameter.
 
         # Parameters
 
-        reports (list, optional): A list of reports - snapshot state areas with optional configuration. This parameter follows the  [`dialect`](/panos-upgrade-assurance/docs/dialect) of [`ConfigParser`](/panos-upgrade-assurance/docs/api/utils#class-configparser) class.
+        reports (list, optional): A list of reports - snapshot state areas with optional configuration. This parameter follows the  [`dialect`](/panos/docs/panos-upgrade-assurance/dialect) of [`ConfigParser`](/panos/docs/panos-upgrade-assurance/api/utils#class-configparser) class.
 
-            The reports list is essentially the list of keys present in the snapshots. These keys, however, are the state areas specified when the snapshot is made with the [`CheckFirewall.run_snapshots()`](/panos-upgrade-assurance/docs/api/check-firewall#checkfirewallrun_snapshots) method. This means that the reports list is basically the list of state areas. The only difference is that for reports, it is possible to specify an additional configuration. This means that the list can be specified in two ways, as `str` or `dict` (in the same manner as for [`CheckFirewall.run_readiness_checks()`](/panos-upgrade-assurance/docs/api/check-firewall#checkfirewallrun_readiness_checks)).
+            The reports list is essentially the list of keys present in the snapshots. These keys, however, are the state areas specified when the snapshot is made with the [`CheckFirewall.run_snapshots()`](/panos/docs/panos-upgrade-assurance/api/check_firewall#checkfirewallrun_snapshots) method. This means that the reports list is basically the list of state areas. The only difference is that for reports, it is possible to specify an additional configuration. This means that the list can be specified in two ways, as `str` or `dict` (in the same manner as for [`CheckFirewall.run_readiness_checks()`](/panos/docs/panos-upgrade-assurance/api/check_firewall#checkfirewallrun_readiness_checks)).
 
             For the elements specified as
 
             * `str` - the element value is the name of the report (state area),
             * `dict` - the element contains the report name (state area) and the key value and report configuration as the element value.
 
-            Refer to the [documentation on reporting](/panos-upgrade-assurance/docs/configuration-details#reports) for details on the currently available snapshot areas and optional parameters that can be configured for them.
+            Refer to the [documentation on reporting](/panos/docs/panos-upgrade-assurance/configuration-details#reports) for details on the currently available snapshot areas and optional parameters that can be configured for them.
 
         # Raises
 
         WrongDataTypeException: An exception is raised when the configuration in a data type is different than `str` or `dict`.
 
         # Returns
-        
+
         dict: Result of comparison in a form of the Python dictionary. Keys in this dictionary are again state areas where values depend on the actual comparison method that was run.
 
         """
 
         result = {}
         reports = ConfigParser(
-                               valid_elements=set(self._functions_mapping.keys()),
-                               requested_config=reports
-                  ).prepare_config()
+            valid_elements=set(self._functions_mapping.keys()), requested_config=reports
+        ).prepare_config()
 
         for report in reports:
             if isinstance(report, dict):
                 report_type, report_config = list(report.items())[0]
-                report_config.update({'report_type': report_type})
+                report_config.update({"report_type": report_type})
             elif isinstance(report, str):
                 report_type = report
-                report_config = {'report_type': report_type}
+                report_config = {"report_type": report_type}
             else:
-                raise WrongDataTypeException(f'Wrong configuration format for report: {report}.')
+                raise WrongDataTypeException(
+                    f"Wrong configuration format for report: {report}."
+                )
 
             self.key_checker(self.left_snap, self.right_snap, report_type)
-            result.update({report_type: self._functions_mapping[report_type](**report_config)})
+            result.update(
+                {report_type: self._functions_mapping[report_type](**report_config)}
+            )
 
         return result
 
     @staticmethod
-    def key_checker(left_dict: dict, right_dict: dict, key: str) -> None:
-        """The static method to check if a key is available in both dictionaries.
+    def key_checker(
+        left_dict: dict, right_dict: dict, key: Union[str, set, list]
+    ) -> None:
+        """The static method to check if a key or a list/set of keys is available in both dictionaries.
 
-        This method looks for a given key in two dictionaries. Its main purpose is to assure that when comparing a key-value pair from two dictionaries, it actually exists in both.
+        This method looks for a given key or list/set of keys in two dictionaries. Its main purpose is to assure that when comparing a key-value pair from two dictionaries, it actually exists in both.
 
         # Parameters
 
         left_dict (dict): 1st dictionary to verify.
         right_dict (dict): 2nd dictionary to verify.
-        key (str): Key name to check.
+        key (str, set, list): Key name or set/list of keys to check.
 
         # Raises
 
         MissingKeyException: when key is not available in at least one snapshot.
 
         """
-        left_snap_missing_key = False if key in left_dict else True
-        right_snap_missing_key = False if key in right_dict else True
+
+        if isinstance(key, str):
+            key_set = set([key])
+        elif isinstance(key, (set, list)):
+            key_set = set(key)
+        else:
+            raise WrongDataTypeException(
+                f"The key variable is a {type(key)} but should be either: str, set or list"
+            )
+
+        left_snap_missing_key = False if key_set.issubset(left_dict.keys()) else True
+        right_snap_missing_key = False if key_set.issubset(right_dict.keys()) else True
 
         if left_snap_missing_key and right_snap_missing_key:
-            raise MissingKeyException(f"{key} is missing in both snapshots")
+            raise MissingKeyException(
+                f"{key} (some elements if set/list) is missing in both snapshots"
+            )
         if left_snap_missing_key or right_snap_missing_key:
-            raise MissingKeyException(f"{key} is missing in {'left snapshot' if left_snap_missing_key else 'right snapshot'}")
+            raise MissingKeyException(
+                f"{key} (some elements if set/list) is missing in {'left snapshot' if left_snap_missing_key else 'right snapshot'}"
+            )
 
     @staticmethod
     def calculate_change_percentage(
-        first_value: Union[str,int],
-        second_value: Union[str,int],
-        threshold: Union[str,float]
+        first_value: Union[str, int],
+        second_value: Union[str, int],
+        threshold: Union[str, float],
     ) -> Dict[str, Union[bool, float]]:
         """The static method to compare differences between values against a given threshold.
 
         Values to be compared should be the `int` or `str` representation of `int`. This method is used when comparing a count of elements so a floating point value here is not expected. The threshold value, on the other hand, should be the `float` or `str` representation of `float`. This is a percentage value.
 
         The format of the returned value is the following:
 
         ```yaml
         {
-            passed: bool, 
+            passed: bool,
             change_percentage: float,
             change_threshold: float
         }
         ```
 
         Where:
 
@@ -176,47 +200,53 @@
         # Parameters
 
         first_value (int, str): First value to compare.
         second_value (int, str): Second value to compare.
         threshold (float, str): Maximal difference between values given as percentage.
 
         # Raises
-        
+
         WrongDataTypeException: An exception is raised when the threshold value is not between `0` and `100` (typical percentage boundaries).
 
         # Returns
 
         dict: A dictionary with the comparison results.
 
         """
         first_value = int(first_value)
         second_value = int(second_value)
         threshold = float(threshold)
 
         result = dict(
-            passed=True,
-            change_percentage=float(0),
-            change_threshold=threshold
+            passed=True, change_percentage=float(0), change_threshold=threshold
         )
 
         if not (first_value == 0 and second_value == 0):
             if threshold < 0 or threshold > 100:
-                raise WrongDataTypeException('The threshold should be a percentage value between 0 and 100.')
+                raise WrongDataTypeException(
+                    "The threshold should be a percentage value between 0 and 100."
+                )
 
-            result['change_percentage'] = round(
-                (abs(first_value - second_value) / (first_value if first_value >= second_value else second_value)) * 100, 2)
-            if result['change_percentage'] > threshold:
-                result['passed'] = False
+            result["change_percentage"] = round(
+                (
+                    abs(first_value - second_value)
+                    / (first_value if first_value >= second_value else second_value)
+                )
+                * 100,
+                2,
+            )
+            if result["change_percentage"] > threshold:
+                result["passed"] = False
         return result
 
     @staticmethod
     def calculate_diff_on_dicts(
-            left_side_to_compare: Dict[str, Union[str,dict]],
-            right_side_to_compare: Dict[str, Union[str,dict]],
-            properties: Optional[List[str]] = None,
+        left_side_to_compare: Dict[str, Union[str, dict]],
+        right_side_to_compare: Dict[str, Union[str, dict]],
+        properties: Optional[List[str]] = None,
     ) -> Dict[str, dict]:
         """The static method to calculate a difference between two dictionaries.
 
         By default dictionaries are compared by going down all nested levels, to the point where key-value pairs are just strings or numbers. It is possible to configure which keys from these pairs should be compared (by default we compare all available keys). This is done using the `properties` parameter. It's a list of the bottom most level keys. For example, when comparing route tables snapshots are formatted like:
 
         ```yaml
         {
@@ -232,23 +262,23 @@
                     "route-table": "unicast"
                 },
                 ...
             }
         }
         ```
 
-        The bottom most level keys are: `virtual-router`, `destination`, `nexthop`, `metric`, `flags`, `age`, `interface`, `route-table`. This list follows [`ConfigParser`](/panos-upgrade-assurance/docs/api/utils#class-configparser) [`dialect`](/panos-upgrade-assurance/docs/dialect).
+        The bottom most level keys are: `virtual-router`, `destination`, `nexthop`, `metric`, `flags`, `age`, `interface`, `route-table`. This list follows [`ConfigParser`](/panos/docs/panos-upgrade-assurance/api/utils#class-configparser) [`dialect`](/panos/docs/panos-upgrade-assurance/dialect).
 
         The difference between dictionaries is calculated from three perspectives:
 
         1. are there any keys missing in the 2nd (right) dictionary that are present in the 1st (left) - this is represented under the `missing` key in the results.
         2. are there any keys in the 2nd (right) dictionary that are not present in the 1st (left) - this is represented under the `added` key in the results.
         3. for the keys that are present in both dictionaries, are values for these keys the same or different - this is represented under the `changed` key in the results.
 
-        This is a **recursive** method. When calculating changed values, if a value for the key is `dict`, we run the method again on that dictionary - we go down one level in the nested structure. We do that to a point where the value is of the `str` type. 
+        This is a **recursive** method. When calculating changed values, if a value for the key is `dict`, we run the method again on that dictionary - we go down one level in the nested structure. We do that to a point where the value is of the `str` type.
         Therefore, when the final comparison results are presented, the `changed` key usually contains a nested results structure. This means it contains a dictionary with the `missing`, `added`, and `changed` keys.
         Each comparison perspective contains the `passed` property that immediately informs if this comparison gave any results (`False`) or not (`True`).
 
         **Example.**
 
         Let's assume we want to compare two dictionaries of the following structure:
 
@@ -266,15 +296,15 @@
             'root_key2'= {
                 'key'= 'other_value'
             }
         }
         ```
 
         The result of this comparison would look like this:
-            
+
         ```json
         {
             "missing": {
                 "passed": false,
                 "missing_keys": [
                     "root_key1"
                 ]
@@ -343,77 +373,79 @@
 
         """
 
         if not (left_side_to_compare and right_side_to_compare):
             return {}
 
         result = dict(
-            missing=dict(
-                passed=True,
-                missing_keys=[]
-            ),
-            added=dict(
-                passed=True,
-                added_keys=[]
-            ),
-            changed=dict(
-                passed=True,
-                changed_raw={}
-            )
+            missing=dict(passed=True, missing_keys=[]),
+            added=dict(passed=True, added_keys=[]),
+            changed=dict(passed=True, changed_raw={}),
         )
 
         missing = left_side_to_compare.keys() - right_side_to_compare.keys()
         if missing:
-            result['missing']['passed'] = False
+            result["missing"]["passed"] = False
             for key in missing:
-                result['missing']['missing_keys'].append(key)
+                result["missing"]["missing_keys"].append(key)
 
         added = right_side_to_compare.keys() - left_side_to_compare.keys()
         if added:
-            result['added']['passed'] = False
+            result["added"]["passed"] = False
             for key in added:
-                result['added']['added_keys'].append(key)
+                result["added"]["added_keys"].append(key)
 
         common_keys = left_side_to_compare.keys() & right_side_to_compare.keys()
-        at_lowest_level = True if isinstance(right_side_to_compare[list(common_keys)[0]], str) else False
-        keys_to_check = ConfigParser(valid_elements=set(common_keys), requested_config=properties).prepare_config() if at_lowest_level else common_keys
+        at_lowest_level = (
+            True
+            if isinstance(right_side_to_compare[list(common_keys)[0]], str)
+            else False
+        )
+        keys_to_check = (
+            ConfigParser(
+                valid_elements=set(common_keys), requested_config=properties
+            ).prepare_config()
+            if at_lowest_level
+            else common_keys
+        )
 
         item_changed = False
         for key in keys_to_check:
             if right_side_to_compare[key] != left_side_to_compare[key]:
                 if isinstance(left_side_to_compare[key], str):
-                    result['changed']['changed_raw'][key] = dict(
+                    result["changed"]["changed_raw"][key] = dict(
                         left_snap=left_side_to_compare[key],
-                        right_snap=right_side_to_compare[key]
+                        right_snap=right_side_to_compare[key],
                     )
                     item_changed = True
                 elif isinstance(left_side_to_compare[key], dict):
                     nested_results = SnapshotCompare.calculate_diff_on_dicts(
                         left_side_to_compare=left_side_to_compare[key],
                         right_side_to_compare=right_side_to_compare[key],
-                        properties=properties)
+                        properties=properties,
+                    )
 
                     SnapshotCompare.calculate_passed(nested_results)
                     if not nested_results["passed"]:
-                        result['changed']['changed_raw'][key] = nested_results
+                        result["changed"]["changed_raw"][key] = nested_results
                         item_changed = True
                 else:
-                    raise WrongDataTypeException(f'Unknown value format for key {key}.')
-            result['changed']['passed'] = not item_changed
+                    raise WrongDataTypeException(f"Unknown value format for key {key}.")
+            result["changed"]["passed"] = not item_changed
 
         return result
 
     @staticmethod
     def calculate_passed(result: Dict[str, Union[dict, str]]) -> None:
         """The static method to calculate the upper level `passed` value.
 
         When two snapshots are compared, a dictionary that is the result of this comparison is structured as in the following [`get_diff_and_threshold()`](#snapshotcompareget_diff_and_threshold) method: each root key contains a dictionary that has a structure returned by the [`calculate_diff_on_dicts()`](#snapshotcomparecalculate_diff_on_dicts) method.
-        
-        This method takes a dictionary under the root key and calculates the `passed` flag based on the all `passed` flags in that dictionary. This provides a quick way of finding out if any comparison made on data under a root key failed or not. 
-        
+
+        This method takes a dictionary under the root key and calculates the `passed` flag based on the all `passed` flags in that dictionary. This provides a quick way of finding out if any comparison made on data under a root key failed or not.
+
         To illustrate that, the `passed` flag added by this method is marked with an arrow:
 
         ```yaml
         {
             'added': {
                 'added_keys': [],
                 'passed': True
@@ -437,33 +469,34 @@
         # Parameters
 
         result (dict): A dictionary for which the `passed` property should be calculated.
 
         """
         passed = True
         for value in result.values():
-            if isinstance(value, dict) and not value['passed']:
+            if isinstance(value, dict) and not value["passed"]:
                 passed = False
-        result['passed'] = passed
+        result["passed"] = passed
 
-    def get_diff_and_threshold(self,
-            report_type: str,
-            properties: Optional[List[str]] = None,
-            count_change_threshold: Optional[Union[int, float]] = None
+    def get_diff_and_threshold(
+        self,
+        report_type: str,
+        properties: Optional[List[str]] = None,
+        count_change_threshold: Optional[Union[int, float]] = None,
     ) -> Optional[Dict[str, Optional[Union[bool, dict]]]]:
         """The generic snapshot comparison method.
 
         The generic method to compare two snapshots of a given type. It is meant to fit most of the comparison cases.
         It is capable of calculating both - a difference between two snapshots and the change count in the elements against a given threshold. The 1<sup>st</sup> calculation is done by the [`calculate_diff_on_dicts()`](#snapshotcomparecalculate_diff_on_dicts) method, the 2<sup>nd</sup> - internally.
 
-        The changed elements count does not compare the count of elements in each snapshot. This value represents the number of actual changes, so elements added, missing and changed. This is compared against the number of elements in the left snapshot as this one is usually the 1st one taken and it's treated as a source of truth. 
+        The changed elements count does not compare the count of elements in each snapshot. This value represents the number of actual changes, so elements added, missing and changed. This is compared against the number of elements in the left snapshot as this one is usually the 1st one taken and it's treated as a source of truth.
 
         The changed elements count is presented as a percentage. In scenarios where the right snapshot has more elements then the left one, it can give values greater than 100%.
 
-        This method produces a complex set of nested dictionaries. Each level contains the `passed` flag indicating if the comparison of a particular type or for a particular level failed or not, and the actual comparison results. 
+        This method produces a complex set of nested dictionaries. Each level contains the `passed` flag indicating if the comparison of a particular type or for a particular level failed or not, and the actual comparison results.
 
         An example for the route tables, crafted in a way that almost each level fails:
 
         ```json
         {
             "added": {
                 "added_keys": [
@@ -508,15 +541,15 @@
                 "change_threshold": 1,
                 "passed": "False"
             },
             "passed": "False"
         }
         ```
 
-        In the example above, you can also see a nested dictionary produced by the [`calculate_diff_on_dicts()`](#snapshotcomparecalculate_diff_on_dicts) method under `changed.changed_raw`. 
+        In the example above, you can also see a nested dictionary produced by the [`calculate_diff_on_dicts()`](#snapshotcomparecalculate_diff_on_dicts) method under `changed.changed_raw`.
 
         # Parameters
 
         report_type (str): Name of report (type) that has to be compared. Basically this is a snapshot state area, for example `nics`, `routes`, etc.
 
         properties (list(str), optional): (defaults to `None`) An optional list of properties to include or exclude when comparing snapshots. This parameter is passed directly to the [`calculate_diff_on_dicts()`](#snapshotcomparecalculate_diff_on_dicts) method. For details on this method parameters, see the [documentation](#snapshotcomparecalculate_diff_on_dicts) for this method.
 
@@ -534,48 +567,57 @@
             right_side_to_compare=self.right_snap[report_type],
             properties=properties,
         )
         result.update(diff)
 
         if count_change_threshold and result:
             if count_change_threshold < 0 or count_change_threshold > 100:
-                raise WrongDataTypeException('The threshold should be a percentage value between 0 and 100.')
+                raise WrongDataTypeException(
+                    "The threshold should be a percentage value between 0 and 100."
+                )
 
-            added_count = len(result['added']['added_keys'])
-            missing_count = len(result['missing']['missing_keys'])
-            changed_count = len(result['changed']['changed_raw'])
+            added_count = len(result["added"]["added_keys"])
+            missing_count = len(result["missing"]["missing_keys"])
+            changed_count = len(result["changed"]["changed_raw"])
             left_total_count = len(self.left_snap[report_type].keys())
-            right_total_count = len(self.right_snap[report_type].keys())
 
-            diff = 1 if left_total_count == 0 else (added_count + missing_count + changed_count)/left_total_count
-            diff_percentage = round(float(diff)*100,2)
+            diff = (
+                1
+                if left_total_count == 0
+                else (added_count + missing_count + changed_count) / left_total_count
+            )
+            diff_percentage = round(float(diff) * 100, 2)
 
             passed = diff_percentage <= count_change_threshold
 
-            result.update({'count_change_percentage': dict(
-                passed=passed,
-                change_percentage=diff_percentage,
-                change_threshold=float(count_change_threshold)
-            )})
+            result.update(
+                {
+                    "count_change_percentage": dict(
+                        passed=passed,
+                        change_percentage=diff_percentage,
+                        change_threshold=float(count_change_threshold),
+                    )
+                }
+            )
 
         if result:
             SnapshotCompare.calculate_passed(result)
         else:
             result = None
         return result
 
     # custom compare methods
     def get_count_change_percentage(
         self,
         report_type: str,
-        thresholds: Optional[List[Dict[str, Union[int, float]]]] = None
+        thresholds: Optional[List[Dict[str, Union[int, float]]]] = None,
     ) -> Optional[Dict[str, Union[bool, dict]]]:
         """Generic method to calculate the change on values and compare them against a given threshold.
 
-        In opposition to the [`get_diff_and_threshold()`](#snapshotcompareget_diff_and_threshold) method, this one does not calculate the count change but the actual difference between the numerical values. 
+        In opposition to the [`get_diff_and_threshold()`](#snapshotcompareget_diff_and_threshold) method, this one does not calculate the count change but the actual difference between the numerical values.
         A good example is a change in the session count. The snapshot for this area is a dictionary with the keys taking values of different session types and values containing the actual session count:
 
         ```yaml
         {
             "session_stats": {
                 "tmo-5gcdelete": "15",
                 "tmo-sctpshutdown": "60",
@@ -593,51 +635,51 @@
                 "num-udp": "0",
                 ...
             }
         }
         ```
 
         This method:
-        
+
         - sweeps through all the session types provided in the `thresholds` variable,
-        - calculates the actual difference, 
+        - calculates the actual difference,
         - compares the actual difference with the threshold value (percentage) for a particular session type.
 
         It takes as parameter a list of dictionaries describing elements to compare, in a form of:
 
         ```json
         {
             "element_type": threshold_value
         }
         ```
 
         Where:
-        
+
         - `element_type` is a key which value we are going to compare,
         - `threshold_value` is a percentage value provided as either `int` or `float`. If the list is empty, the method will return `None`.
-        
-        :::warning
-        This list **does not support** [`ConfigParser`](/panos-upgrade-assurance/docs/api/utils#class-configparser) [`dialect`](/panos-upgrade-assurance/docs/dialect).
+
+        :::caution
+        This list **does not support** [`ConfigParser`](/panos/docs/panos-upgrade-assurance/api/utils#class-configparser) [`dialect`](/panos/docs/panos-upgrade-assurance/dialect).
         :::
 
         Below there is a sample list for the `sessions_stat` dictionary shown above that would calculate differences for the TCP and UDP sessions:
 
         ```json
         [
             { "num-tcp": 1.5 },
             { "num-udp": 15 },
         ]
         ```
 
         # Parameters
 
         thresholds (list): (defaults to `None`) The list of elements to compare with thresholds.
-                
+
         # Raises
-                
+
         SnapshotSchemeMismatchException: Thrown when a snapshot element has a different set of properties in both snapshots.
 
         # Returns
 
         dict: The result of difference compared against a threshold. The result for each value is in the same form as returned by the [`calculate_change_percentage()`](#snapshotcomparecalculate_change_percentage) method. For the examples above, the return value would be:
 
         ```yaml
@@ -661,28 +703,40 @@
         if not thresholds:
             return None
 
         result = dict(
             passed=True,
         )
 
-        if self.left_snap[report_type].keys() != self.right_snap[report_type].keys():
-            raise SnapshotSchemeMismatchException(f'Snapshots contain different set of data for {report_type} report.')
+        requested_elements = set(next(iter(unary_dict)) for unary_dict in thresholds)
+        try:
+            self.key_checker(
+                self.left_snap[report_type],
+                self.right_snap[report_type],
+                requested_elements,
+            )
+        except (
+            MissingKeyException
+        ) as exc:  # raised when any requested key is missing in one of the snapshots
+            raise SnapshotSchemeMismatchException(
+                f"Snapshots have missing keys in {requested_elements} for {report_type} report."
+            ) from exc
 
         elements = ConfigParser(
-                                    valid_elements=set(self.left_snap[report_type].keys()),
-                                    requested_config=thresholds,
-                        ).prepare_config()
+            valid_elements=set(self.left_snap[report_type].keys()),
+            requested_config=thresholds,
+        ).prepare_config()
 
         for element in elements:
             element_type, threshold_value = list(element.items())[0]
-            self.key_checker(self.left_snap[report_type], self.right_snap[report_type], element_type)
-            result.update({
-                element_type: SnapshotCompare.calculate_change_percentage(
-                    first_value=self.left_snap[report_type][element_type],
-                    second_value=self.right_snap[report_type][element_type],
-                    threshold=threshold_value
-                )
-            })
+            result.update(
+                {
+                    element_type: SnapshotCompare.calculate_change_percentage(
+                        first_value=self.left_snap[report_type][element_type],
+                        second_value=self.right_snap[report_type][element_type],
+                        threshold=threshold_value,
+                    )
+                }
+            )
 
         SnapshotCompare.calculate_passed(result)
         return result
```

### Comparing `panos_upgrade_assurance-0.0.1/panos_upgrade_assurance/utils.py` & `panos_upgrade_assurance-0.0.2/panos_upgrade_assurance/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,170 +1,196 @@
 from dataclasses import dataclass
 from copy import deepcopy
-from typing import Optional, Union, List, Dict, Iterable
+from typing import Optional, Union, List, Iterable
 from enum import Enum
 
+
 class UnknownParameterException(Exception):
     """Used when one of the requested configuration parameters processed by [`ConfigParser`](#class-configparser) is not a valid parameter."""
+
     pass
 
+
 class WrongDataTypeException(Exception):
     """Used when a variable does not meet data type requirements."""
+
     pass
 
+
 class CheckType:
     """Class mapping check configuration strings for commonly used variables.
 
-    Readiness checks configuration passed to the [`CheckFirewall`](/panos-upgrade-assurance/docs/api/check-firewall#class-checkfirewall) class is in a form of a list of strings. These strings are compared in several places to parse the configuration and set the proper checks. This class is used to avoid hardcoding these strings. It maps the actual configuration string to a variable that can be referenced in the code.
+    Readiness checks configuration passed to the [`CheckFirewall`](/panos/docs/panos-upgrade-assurance/api/check_firewall#class-checkfirewall) class is in a form of a list of strings. These strings are compared in several places to parse the configuration and set the proper checks. This class is used to avoid hardcoding these strings. It maps the actual configuration string to a variable that can be referenced in the code.
     """
+
     PANORAMA = "panorama"
     HA = "ha"
     NTP_SYNC = "ntp_sync"
     CANDIDATE_CONFIG = "candidate_config"
     EXPIRED_LICENSES = "expired_licenses"
     ACTIVE_SUPPORT = "active_support"
     CONTENT_VERSION = "content_version"
     SESSION_EXIST = "session_exist"
     ARP_ENTRY_EXIST = "arp_entry_exist"
     IPSEC_TUNNEL_STATUS = "ip_sec_tunnel_status"
     FREE_DISK_SPACE = "free_disk_space"
     MP_DP_CLOCK_SYNC = "planes_clock_sync"
 
+
 class SnapType:
     """Class mapping the snapshot configuration strings to the commonly used variables.
 
-    Snapshot configuration passed to the [`CheckFirewall`](/panos-upgrade-assurance/docs/api/check-firewall#class-checkfirewall) class is in a form of a list of strings. These strings are compared in several places to parse the configuration and set proper snapshots.
+    Snapshot configuration passed to the [`CheckFirewall`](/panos/docs/panos-upgrade-assurance/api/check_firewall#class-checkfirewall) class is in a form of a list of strings. These strings are compared in several places to parse the configuration and set proper snapshots.
     This class is used to avoid hardcoding these strings. It maps the actual configuration string to a variable that can be referenced in the code.
     """
+
     NICS = "nics"
     ROUTES = "routes"
     LICENSE = "license"
     ARP_TABLE = "arp_table"
     CONTENT_VERSION = "content_version"
     SESSION_STATS = "session_stats"
     IPSEC_TUNNELS = "ip_sec_tunnels"
 
+
 class CheckStatus(Enum):
     """Class containing possible statuses for the check results.
 
     Its main purpose is to extend the simple `True`/`False` logic in a way that would provide more details/explanation in case a check fails. It provides the following statuses:
 
     * `SUCCESS`
     * `FAIL`
     * `ERROR`
     * `SKIPPED`
 
     """
+
     SUCCESS = 0
     FAIL = 1
     ERROR = 2
     SKIPPED = 3
 
+
 @dataclass
 class CheckResult:
     """Class representing the readiness check results.
 
     It provides two types of information:
 
     * `status` which represents information about the check outcome,
     * `reason` a reason behind the particular outcome, this comes in handy when a check fails.
 
-    Most of the [`CheckFirewall`](/panos-upgrade-assurance/docs/api/check-firewall#class-checkfirewall) methods use this class to store the return values, but mostly internally. The [`CheckFirewall.run_readiness_checks()`](/panos-upgrade-assurance/docs/api/check-firewall#checkfirewallrun_readiness_checks) method translates this class into the python primitives: `str` and `bool`.
+    Most of the [`CheckFirewall`](/panos/docs/panos-upgrade-assurance/api/check_firewall#class-checkfirewall) methods use this class to store the return values, but mostly internally. The [`CheckFirewall.run_readiness_checks()`](/panos/docs/panos-upgrade-assurance/api/check_firewall#checkfirewallrun_readiness_checks) method translates this class into the python primitives: `str` and `bool`.
 
     # Attributes
 
     status (CheckStatus): Holds the status of a check. See [`CheckStatus`](#class-checkstatus) class for details.
-    reason (str): Holds a reason explaining why a check fails. Provides no value if the check is successful. 
-    
+    reason (str): Holds a reason explaining why a check fails. Provides no value if the check is successful.
+
     """
+
     status: CheckStatus = CheckStatus.FAIL
     reason: str = ""
 
     def __str__(self):
         """This class' string representation.
 
         # Returns
 
         str: a string combined from the `self.status` and `self.reason` variables. Provides a human readable representation of the class. Perfect to provide a reason for a particular check outcome.
 
         """
-        return f'[{self.status.name}] {self.reason}'
+        return f"[{self.status.name}] {self.reason}"
 
     def __bool__(self):
         """Class' boolean representation.
 
         # Returns
 
-        bool: a boolean value interpreting the value of the current `state`: 
+        bool: a boolean value interpreting the value of the current `state`:
 
         * `True` when `status` [`CheckStatus.SUCCESS`](#class-checkstatus)
         * `False` otherwise.
 
         """
         return True if self.status == CheckStatus.SUCCESS else False
 
+
 class ConfigParser:
     """Class responsible for parsing the provided configuration.
-    
-    This class is universal, meaning it parses configuration provided as the list of strings or dictionaries and verifies it against the list of valid configuration items. 
-    There are no hardcoded items against which the configuration is checked. This class is used in many places in this package and it uses a specific [`dialect`](/panos-upgrade-assurance/docs/dialect).
+
+    This class is universal, meaning it parses configuration provided as the list of strings or dictionaries and verifies it against the list of valid configuration items.
+    There are no hardcoded items against which the configuration is checked. This class is used in many places in this package and it uses a specific [`dialect`](/panos/docs/panos-upgrade-assurance/dialect).
 
     # Attributes
 
     _requested_config_names (set): Contains only element names of the requested configuration. When no requested configuration is passed (implicit `'all'`), this is equal to `self.valid_elements`.
 
     """
 
-    def __init__(self, valid_elements: Iterable, requested_config: Optional[List[Union[str, dict]]] = None):
+    def __init__(
+        self,
+        valid_elements: Iterable,
+        requested_config: Optional[List[Union[str, dict]]] = None,
+    ):
         """ConfigParser constructor.
 
         Introduces some initial verification logic:
 
         * `valid_elements` is converted to `set` - this way we get rid of all duplicates,
-        * if `requested_config` is `None` we immediately treat it as if `all`  was passed implicitly (see [`dialect`](/panos-upgrade-assurance/docs/dialect)) - it's expanded to `valid_elements`
+        * if `requested_config` is `None` we immediately treat it as if `all`  was passed implicitly (see [`dialect`](/panos/docs/panos-upgrade-assurance/dialect)) - it's expanded to `valid_elements`
         * `_requested_config_names` is introduced as `requested_config` stripped of any element configurations. Additionally, we do verification if elements of this variable match `valid_elements`. An exception is thrown if not.
 
         # Parameters
 
         valid_elements (iterable): Valid elements against which we check the requested config.
         requested_config (list, optional): (defaults to `None`) A list of requested configuration items with an optional configuration.
 
         # Raises
 
         UnknownParameterException: An exception is raised when a requested configuration element is not one of the valid elements.
-        
+
         """
         self.valid_elements = set(valid_elements)
 
-        if requested_config:    # if not None or not empty list
+        if requested_config:  # if not None or not empty list
             self.requested_config = deepcopy(requested_config)
-            self._requested_config_names = set([ ConfigParser._extract_element_name(config_keyword) for config_keyword in self.requested_config ])
+            self._requested_config_names = set(
+                [
+                    ConfigParser._extract_element_name(config_keyword)
+                    for config_keyword in self.requested_config
+                ]
+            )
             for config_name in self._requested_config_names:
                 if not self._is_element_included(element=config_name):
-                    raise UnknownParameterException(f'Unknown configuration parameter passed: {config_name}.')
+                    raise UnknownParameterException(
+                        f"Unknown configuration parameter passed: {config_name}."
+                    )
         else:
             self._requested_config_names = set(valid_elements)
             self.requested_config = list(valid_elements)  # Meaning 'all' valid tests
 
     def _is_element_included(self, element: str) -> bool:
         """Method verifying if a config element is a correct (supported) value.
 
-        This method can also handle `not-elements` (see [`dialect`](/panos-upgrade-assurance/docs/dialect)).
+        This method can also handle `not-elements` (see [`dialect`](/panos/docs/panos-upgrade-assurance/dialect)).
 
         # Parameters
 
         element (str): The config element to verify. This can be a `not-element`. This parameter is verified against `self.valid_elements` `set`. Key word `'all'` is also accepted.
 
         # Returns
         bool: `True` if the value is correct, `False` otherwise.
 
         """
-        if element in self.valid_elements or (element.startswith('!') and element[1:] in self.valid_elements):
+        if element in self.valid_elements or (
+            element.startswith("!") and element[1:] in self.valid_elements
+        ):
             return True
-        elif element == 'all' and 'all' in self.requested_config:
+        elif element == "all" and "all" in self.requested_config:
             return True
         else:
             return False
 
     @staticmethod
     def _extract_element_name(config: Union[str, dict]) -> str:
         """Method that extracts the name from a config element.
@@ -187,96 +213,109 @@
         if isinstance(config, str):
             return config
         elif isinstance(config, dict):
             if len(config) == 1:
                 return list(config.keys())[0]
             else:
                 raise WrongDataTypeException(
-                    'Dict provided as config definition has incorrect format, it is supposed to have only one key {key:[]}')
+                    "Dict provided as config definition has incorrect format, it is supposed to have only one key {key:[]}"
+                )
         else:
-            raise WrongDataTypeException('Config definition is neither string or dict')
+            raise WrongDataTypeException("Config definition is neither string or dict")
 
     def _expand_all(self) -> None:
         """Expand key word `'all'` to  `self.valid_elements`.
-        
-        During expansion, elements from `self.valid_elements` which are already available in `self.requested_config` are skipped. This way we do not introduce duplicates for elements that were provided explicitly. 
+
+        During expansion, elements from `self.valid_elements` which are already available in `self.requested_config` are skipped. This way we do not introduce duplicates for elements that were provided explicitly.
 
         This method directly operates on `self.requested_config`.
         """
-        pure_names = set([
-            (name[1:] if name.startswith('!') else name) for name in self._requested_config_names if name != 'all'
-        ])
+        pure_names = set(
+            [
+                (name[1:] if name.startswith("!") else name)
+                for name in self._requested_config_names
+                if name != "all"
+            ]
+        )
         self.requested_config.extend(list(self.valid_elements - pure_names))
         self.requested_config.remove("all")
 
-    def prepare_config(self) -> List[Union[str,dict]]:
+    def prepare_config(self) -> List[Union[str, dict]]:
         """Parse the input config and return a machine-usable configuration.
 
         The parsed configuration retains element types. This means that an element of a dictionary type will remain a dictionary in the parsed config.
 
-        This method handles most of the [`dialect`](/panos-upgrade-assurance/docs/dialect)'s logic.
+        This method handles most of the [`dialect`](/panos/docs/panos-upgrade-assurance/dialect)'s logic.
 
         # Returns
         list: The parsed configuration.
 
         """
-        if all( (config_name.startswith('!') for config_name in self._requested_config_names) ):
-                self.requested_config.insert(0, "all")
+        if all(
+            (
+                config_name.startswith("!")
+                for config_name in self._requested_config_names
+            )
+        ):
+            self.requested_config.insert(0, "all")
 
         if "all" in self.requested_config:
             self._expand_all()
 
         final_configs = []
 
         for config_element in self.requested_config:
-            if not ConfigParser._extract_element_name(config_element).startswith('!'):
+            if not ConfigParser._extract_element_name(config_element).startswith("!"):
                 final_configs.append(config_element)
 
         return final_configs
 
 
 def interpret_yes_no(boolstr: str) -> bool:
-        """Interpret `yes`/`no` as booleans.
-        
-        # Parameters
+    """Interpret `yes`/`no` as booleans.
+
+    # Parameters
 
-        boolstr (str): `yes` or `no`, a typical device response for simple boolean-like queries.
+    boolstr (str): `yes` or `no`, a typical device response for simple boolean-like queries.
 
-        # Raises
+    # Raises
 
-        WrongDataTypeException: An exception is raised when `boolstr` is neither `yes` or `no`.
+    WrongDataTypeException: An exception is raised when `boolstr` is neither `yes` or `no`.
 
-        # Returns
+    # Returns
 
-        bool: `True` for *yes*, `False` for *no*.
+    bool: `True` for *yes*, `False` for *no*.
 
-        """
-        if not boolstr in ['yes', 'no']:
-            raise WrongDataTypeException(f'Cannot interpret following string as boolean: {boolstr}.')
+    """
+    if boolstr not in ["yes", "no"]:
+        raise WrongDataTypeException(
+            f"Cannot interpret following string as boolean: {boolstr}."
+        )
+
+    return True if boolstr == "yes" else False
 
-        return True if boolstr == 'yes' else False
 
 def printer(report: dict, indent_level: int = 0) -> None:
     """Print reports in human friendly format.
 
     # Parameters
 
     report (dict): Dict with reports from tests.
     indent_level (int): Indentation level.
 
     """
-    delim = '   |'
-    if 'passed' in report:
+    delim = "   |"
+    if "passed" in report:
         print(f'{delim*indent_level} passed: {report["passed"]}')
-        if report['passed']:
+        if report["passed"]:
             return
     for k, v in report.items():
-        if k != 'passed':
+        if k != "passed":
             if isinstance(v, list):
-                print(f'{delim*indent_level} {k}:')
+                print(f"{delim*indent_level} {k}:")
                 for element in v:
-                    print(f'{delim*(indent_level +1)}- {element}')
+                    print(f"{delim*(indent_level +1)}- {element}")
             elif isinstance(v, dict):
-                print(f'{delim * indent_level} {k}:')
+                print(f"{delim * indent_level} {k}:")
                 printer(v, indent_level + 1)
             else:
-                print(f'{delim * indent_level} {k}: {v}')
+                print(f"{delim * indent_level} {k}: {v}")
```

### Comparing `panos_upgrade_assurance-0.0.1/PKG-INFO` & `panos_upgrade_assurance-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: panos-upgrade-assurance
-Version: 0.0.1
+Version: 0.0.2
 Summary: 
 Author: Palo Alto Networks
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: pan-os-python (>=1.8,<2.0)
 Requires-Dist: pan-python (>=0.17,<0.18)
 Requires-Dist: xmltodict (>=0.13,<0.14)
@@ -23,17 +22,17 @@
 
 The `panos-upgrade-assurance` package includes the set of classes written in `Python` to ease the process of writing checks and state snapshots during PanOS upgrade on the Next Generation Firewall.
 
 Both checks and snapshots can be used to verify the state of a device during an upgrade process. What more, it is possible to generate a report for these checks.
 
 The libraries were written to support Ansible and XSOAR integrations. They depend on [pan-os-python](https://pan.dev/panos/docs/panospython/) libraries and therefore are quite easy to fit into the [PanOS Ansible modules collection](https://galaxy.ansible.com/paloaltonetworks/panos).
 
-For more detailed documentation please refer to [PAN.DEV](https://pan.dev/panos-upgrade-assurance/docs/) portal.
+For more detailed documentation please refer to [PAN.DEV](https://pan.dev/panos/docs/panos-upgrade-assurance/) portal.
 
 ## Installation
 
 To install the package you can use `pip`:
 
 ``` console
-python -m pip install 'git+https://github.com/PaloAltoNetworks/pan-os-upgrade-assurance'
+python -m pip install panos-upgrade-assurance
 ```
```

