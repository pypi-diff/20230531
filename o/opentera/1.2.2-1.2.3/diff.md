# Comparing `tmp/opentera-1.2.2.tar.gz` & `tmp/opentera-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opentera-1.2.2.tar", last modified: Tue May 23 18:48:14 2023, max compression
+gzip compressed data, was "opentera-1.2.3.tar", last modified: Wed May 31 15:42:52 2023, max compression
```

## Comparing `opentera-1.2.2.tar` & `opentera-1.2.3.tar`

### file list

```diff
@@ -1,155 +1,155 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:48:14.655590 opentera-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-23 18:46:51.000000 opentera-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-23 18:46:51.000000 opentera-1.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-05-23 18:48:14.655590 opentera-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-05-23 18:46:51.000000 opentera-1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:48:14.639589 opentera-1.2.2/opentera/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-23 18:47:25.000000 opentera-1.2.2/opentera/OpenTeraServerVersion.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       17 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:48:14.639589 opentera-1.2.2/opentera/config/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4321 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/config/ConfigManager.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:48:14.639589 opentera-1.2.2/opentera/crypto/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/crypto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12448 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/crypto/crypto_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:48:14.643590 opentera-1.2.2/opentera/db/
--rwxr-xr-x   0 runner    (1001) docker     (123)    12396 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/Base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/SoftDeleteMixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/SoftDeleteQueryRewriter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/SoftInsertMixin.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       17 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:48:14.647590 opentera-1.2.2/opentera/db/models/
--rw-r--r--   0 runner    (1001) docker     (123)     9183 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/models/TeraAsset.py
--rw-r--r--   0 runner    (1001) docker     (123)    11579 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/models/TeraDevice.py
--rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/models/TeraDeviceParticipant.py
--rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/models/TeraDeviceProject.py
--rw-r--r--   0 runner    (1001) docker     (123)     6465 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/models/TeraDeviceSite.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/models/TeraDeviceSubType.py
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/models/TeraDeviceType.py
--rw-r--r--   0 runner    (1001) docker     (123)    17755 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/models/TeraParticipant.py
--rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/models/TeraParticipantGroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     8844 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/models/TeraProject.py
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/models/TeraServerSettings.py
--rw-r--r--   0 runner    (1001) docker     (123)    10286 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/models/TeraService.py
--rw-r--r--   0 runner    (1001) docker     (123)    11408 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/models/TeraServiceAccess.py
--rw-r--r--   0 runner    (1001) docker     (123)    12119 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/models/TeraServiceConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/models/TeraServiceConfigSpecific.py
--rw-r--r--   0 runner    (1001) docker     (123)     7890 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/models/TeraServiceProject.py
--rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/models/TeraServiceRole.py
--rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/models/TeraServiceSite.py
--rw-r--r--   0 runner    (1001) docker     (123)    23587 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/models/TeraSession.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/models/TeraSessionDevices.py
--rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/models/TeraSessionEvent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/models/TeraSessionParticipants.py
--rw-r--r--   0 runner    (1001) docker     (123)     8719 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/models/TeraSessionType.py
--rw-r--r--   0 runner    (1001) docker     (123)     7959 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/models/TeraSessionTypeProject.py
--rw-r--r--   0 runner    (1001) docker     (123)     9118 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/models/TeraSessionTypeSite.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/models/TeraSessionUsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/models/TeraSite.py
--rw-r--r--   0 runner    (1001) docker     (123)     9504 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/models/TeraTest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/models/TeraTestType.py
--rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/models/TeraTestTypeProject.py
--rw-r--r--   0 runner    (1001) docker     (123)     6994 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/models/TeraTestTypeSite.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17164 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/models/TeraUser.py
--rw-r--r--   0 runner    (1001) docker     (123)     9339 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/models/TeraUserGroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/models/TeraUserPreference.py
--rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/models/TeraUserUserGroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:48:14.647590 opentera-1.2.2/opentera/events/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/events/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:48:14.647590 opentera-1.2.2/opentera/forms/
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/forms/TeraDeviceForm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/forms/TeraDeviceSubTypeForm.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/forms/TeraDeviceTypeForm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/forms/TeraForm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/forms/TeraParticipantForm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/forms/TeraParticipantGroupForm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/forms/TeraProjectForm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/forms/TeraServiceConfigForm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/forms/TeraServiceForm.py
--rw-r--r--   0 runner    (1001) docker     (123)     9901 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/forms/TeraSessionForm.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/forms/TeraSessionTypeConfigForm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/forms/TeraSessionTypeForm.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/forms/TeraSiteForm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/forms/TeraTestTypeForm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/forms/TeraUserForm.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/forms/TeraUserGroupForm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/forms/TeraVersionsForm.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/forms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:48:14.647590 opentera-1.2.2/opentera/logging/
--rw-r--r--   0 runner    (1001) docker     (123)     9627 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/logging/LoggingClient.py
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/logging/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:48:14.647590 opentera-1.2.2/opentera/messages/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/messages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:48:14.651589 opentera-1.2.2/opentera/messages/python/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-23 18:48:06.000000 opentera-1.2.2/opentera/messages/python/CreateSession_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-05-23 18:48:06.000000 opentera-1.2.2/opentera/messages/python/DatabaseEvent_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-05-23 18:48:06.000000 opentera-1.2.2/opentera/messages/python/DeviceEvent_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-23 18:48:06.000000 opentera-1.2.2/opentera/messages/python/JoinSessionEvent_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-23 18:48:07.000000 opentera-1.2.2/opentera/messages/python/JoinSessionReplyEvent_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-23 18:48:07.000000 opentera-1.2.2/opentera/messages/python/LeaveSessionEvent_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-05-23 18:48:07.000000 opentera-1.2.2/opentera/messages/python/LogEvent_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-05-23 18:48:07.000000 opentera-1.2.2/opentera/messages/python/LoginEvent_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-05-23 18:48:07.000000 opentera-1.2.2/opentera/messages/python/ParticipantEvent_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-05-23 18:48:07.000000 opentera-1.2.2/opentera/messages/python/RPCMessage_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-23 18:48:07.000000 opentera-1.2.2/opentera/messages/python/Result_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-23 18:48:07.000000 opentera-1.2.2/opentera/messages/python/ServerCommand_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-23 18:48:07.000000 opentera-1.2.2/opentera/messages/python/StopSessionEvent_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-23 18:48:07.000000 opentera-1.2.2/opentera/messages/python/TeraEvent_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-23 18:48:07.000000 opentera-1.2.2/opentera/messages/python/TeraMessage_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-05-23 18:48:07.000000 opentera-1.2.2/opentera/messages/python/TeraModuleMessage_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-23 18:48:07.000000 opentera-1.2.2/opentera/messages/python/UserEvent_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-05-23 18:48:06.000000 opentera-1.2.2/opentera/messages/python/UserRegisterToEvent_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/messages/python/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:48:14.651589 opentera-1.2.2/opentera/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     7687 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/modules/BaseModule.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:48:14.651589 opentera-1.2.2/opentera/redis/
--rwxr-xr-x   0 runner    (1001) docker     (123)     5734 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/redis/RedisClient.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2896 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/redis/RedisProtocolFactory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/redis/RedisRPCClient.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/redis/RedisVars.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/redis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:48:14.655590 opentera-1.2.2/opentera/services/
--rw-r--r--   0 runner    (1001) docker     (123)    38393 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/services/BaseWebRTCService.py
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/services/DisabledTokenStorage.py
--rw-r--r--   0 runner    (1001) docker     (123)    21672 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/services/ServiceAccessManager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/services/ServiceConfigManager.py
--rw-r--r--   0 runner    (1001) docker     (123)     8009 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/services/ServiceOpenTera.py
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/services/ServiceOpenTeraWithAssets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/services/ServiceOpenTeraWithTests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/services/TeraDeviceClient.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/services/TeraParticipantClient.py
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/services/TeraServiceClient.py
--rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/services/TeraUserClient.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:48:14.655590 opentera-1.2.2/opentera/services/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     7528 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/services/modules/WebRTCModule.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/services/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:48:14.655590 opentera-1.2.2/opentera/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/utils/Metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     8494 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/utils/TeraVersions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/utils/UserAgentParser.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:48:14.655590 opentera-1.2.2/opentera/utils/assets/
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/utils/assets/AssetFile.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/utils/assets/AssetVideoFile.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/utils/assets/BaseAsset.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/utils/assets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:48:14.639589 opentera-1.2.2/opentera.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-05-23 18:48:14.000000 opentera-1.2.2/opentera.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-05-23 18:48:14.000000 opentera-1.2.2/opentera.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 18:48:14.000000 opentera-1.2.2/opentera.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-23 18:48:14.000000 opentera-1.2.2/opentera.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-23 18:48:14.000000 opentera-1.2.2/opentera.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 18:48:14.655590 opentera-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-23 18:46:51.000000 opentera-1.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:48:14.639589 opentera-1.2.2/translations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:48:14.639589 opentera-1.2.2/translations/en/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:48:14.655590 opentera-1.2.2/translations/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-23 18:48:10.000000 opentera-1.2.2/translations/en/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    76833 2023-05-23 18:46:51.000000 opentera-1.2.2/translations/en/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:48:14.639589 opentera-1.2.2/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:48:14.655590 opentera-1.2.2/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    39138 2023-05-23 18:48:10.000000 opentera-1.2.2/translations/fr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    94200 2023-05-23 18:46:51.000000 opentera-1.2.2/translations/fr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:42:52.703375 opentera-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-31 15:41:12.000000 opentera-1.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-31 15:41:12.000000 opentera-1.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-05-31 15:42:52.703375 opentera-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-05-31 15:41:12.000000 opentera-1.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:42:52.687375 opentera-1.2.3/opentera/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-31 15:41:59.000000 opentera-1.2.3/opentera/OpenTeraServerVersion.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       17 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:42:52.687375 opentera-1.2.3/opentera/config/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4321 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/config/ConfigManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:42:52.687375 opentera-1.2.3/opentera/crypto/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/crypto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12448 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/crypto/crypto_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:42:52.687375 opentera-1.2.3/opentera/db/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12494 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/db/Base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/db/SoftDeleteMixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/db/SoftDeleteQueryRewriter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/db/SoftInsertMixin.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       17 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:42:52.691375 opentera-1.2.3/opentera/db/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     9183 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/db/models/TeraAsset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11579 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/db/models/TeraDevice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/db/models/TeraDeviceParticipant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/db/models/TeraDeviceProject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6465 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/db/models/TeraDeviceSite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/db/models/TeraDeviceSubType.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/db/models/TeraDeviceType.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17755 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/db/models/TeraParticipant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/db/models/TeraParticipantGroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8844 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/db/models/TeraProject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/db/models/TeraServerSettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10404 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/db/models/TeraService.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10411 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/db/models/TeraServiceAccess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12119 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/db/models/TeraServiceConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/db/models/TeraServiceConfigSpecific.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7890 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/db/models/TeraServiceProject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/db/models/TeraServiceRole.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/db/models/TeraServiceSite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23587 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/db/models/TeraSession.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/db/models/TeraSessionDevices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/db/models/TeraSessionEvent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/db/models/TeraSessionParticipants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8759 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/db/models/TeraSessionType.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8730 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/db/models/TeraSessionTypeProject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9880 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/db/models/TeraSessionTypeSite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/db/models/TeraSessionUsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/db/models/TeraSite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9504 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/db/models/TeraTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/db/models/TeraTestType.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/db/models/TeraTestTypeProject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6994 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/db/models/TeraTestTypeSite.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17164 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/db/models/TeraUser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9339 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/db/models/TeraUserGroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/db/models/TeraUserPreference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/db/models/TeraUserUserGroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/db/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:42:52.691375 opentera-1.2.3/opentera/events/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/events/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:42:52.695375 opentera-1.2.3/opentera/forms/
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/forms/TeraDeviceForm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/forms/TeraDeviceSubTypeForm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/forms/TeraDeviceTypeForm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/forms/TeraForm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/forms/TeraParticipantForm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/forms/TeraParticipantGroupForm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/forms/TeraProjectForm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/forms/TeraServiceConfigForm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/forms/TeraServiceForm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9901 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/forms/TeraSessionForm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/forms/TeraSessionTypeConfigForm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/forms/TeraSessionTypeForm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/forms/TeraSiteForm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/forms/TeraTestTypeForm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/forms/TeraUserForm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/forms/TeraUserGroupForm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/forms/TeraVersionsForm.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/forms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:42:52.695375 opentera-1.2.3/opentera/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)     9627 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/logging/LoggingClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/logging/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:42:52.695375 opentera-1.2.3/opentera/messages/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/messages/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:42:52.695375 opentera-1.2.3/opentera/messages/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-31 15:42:44.000000 opentera-1.2.3/opentera/messages/python/CreateSession_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-05-31 15:42:44.000000 opentera-1.2.3/opentera/messages/python/DatabaseEvent_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-05-31 15:42:44.000000 opentera-1.2.3/opentera/messages/python/DeviceEvent_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-31 15:42:44.000000 opentera-1.2.3/opentera/messages/python/JoinSessionEvent_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-31 15:42:44.000000 opentera-1.2.3/opentera/messages/python/JoinSessionReplyEvent_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-31 15:42:44.000000 opentera-1.2.3/opentera/messages/python/LeaveSessionEvent_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-05-31 15:42:44.000000 opentera-1.2.3/opentera/messages/python/LogEvent_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-05-31 15:42:44.000000 opentera-1.2.3/opentera/messages/python/LoginEvent_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-05-31 15:42:44.000000 opentera-1.2.3/opentera/messages/python/ParticipantEvent_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-05-31 15:42:44.000000 opentera-1.2.3/opentera/messages/python/RPCMessage_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-31 15:42:44.000000 opentera-1.2.3/opentera/messages/python/Result_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-31 15:42:44.000000 opentera-1.2.3/opentera/messages/python/ServerCommand_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-31 15:42:44.000000 opentera-1.2.3/opentera/messages/python/StopSessionEvent_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-31 15:42:44.000000 opentera-1.2.3/opentera/messages/python/TeraEvent_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-31 15:42:44.000000 opentera-1.2.3/opentera/messages/python/TeraMessage_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-05-31 15:42:44.000000 opentera-1.2.3/opentera/messages/python/TeraModuleMessage_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-31 15:42:44.000000 opentera-1.2.3/opentera/messages/python/UserEvent_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-05-31 15:42:44.000000 opentera-1.2.3/opentera/messages/python/UserRegisterToEvent_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/messages/python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:42:52.699375 opentera-1.2.3/opentera/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     7687 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/modules/BaseModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:42:52.699375 opentera-1.2.3/opentera/redis/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5734 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/redis/RedisClient.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2896 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/redis/RedisProtocolFactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/redis/RedisRPCClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/redis/RedisVars.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/redis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:42:52.699375 opentera-1.2.3/opentera/services/
+-rw-r--r--   0 runner    (1001) docker     (123)    38393 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/services/BaseWebRTCService.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/services/DisabledTokenStorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21672 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/services/ServiceAccessManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/services/ServiceConfigManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8009 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/services/ServiceOpenTera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/services/ServiceOpenTeraWithAssets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/services/ServiceOpenTeraWithTests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/services/TeraDeviceClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/services/TeraParticipantClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/services/TeraServiceClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/services/TeraUserClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:42:52.699375 opentera-1.2.3/opentera/services/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     7528 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/services/modules/WebRTCModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/services/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:42:52.699375 opentera-1.2.3/opentera/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/utils/Metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8494 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/utils/TeraVersions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/utils/UserAgentParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:42:52.699375 opentera-1.2.3/opentera/utils/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/utils/assets/AssetFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/utils/assets/AssetVideoFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/utils/assets/BaseAsset.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:12.000000 opentera-1.2.3/opentera/utils/assets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:42:52.687375 opentera-1.2.3/opentera.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-05-31 15:42:52.000000 opentera-1.2.3/opentera.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-05-31 15:42:52.000000 opentera-1.2.3/opentera.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 15:42:52.000000 opentera-1.2.3/opentera.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-31 15:42:52.000000 opentera-1.2.3/opentera.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-31 15:42:52.000000 opentera-1.2.3/opentera.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 15:42:52.703375 opentera-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-31 15:41:12.000000 opentera-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:42:52.683375 opentera-1.2.3/translations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:42:52.683375 opentera-1.2.3/translations/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:42:52.699375 opentera-1.2.3/translations/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-31 15:42:48.000000 opentera-1.2.3/translations/en/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    76833 2023-05-31 15:41:12.000000 opentera-1.2.3/translations/en/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:42:52.683375 opentera-1.2.3/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:42:52.703375 opentera-1.2.3/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    39138 2023-05-31 15:42:48.000000 opentera-1.2.3/translations/fr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    94200 2023-05-31 15:41:12.000000 opentera-1.2.3/translations/fr/LC_MESSAGES/messages.po
```

### Comparing `opentera-1.2.2/LICENSE` & `opentera-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/PKG-INFO` & `opentera-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentera
-Version: 1.2.2
+Version: 1.2.3
 Summary: OpenTera base package
 Home-page: https://github.com/introlab/opentera
 Author: Dominic Létourneau, Simon Brière
 Author-email: dominic.letourneau@usherbrooke.ca, simon.briere@usherbrooke.ca
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `opentera-1.2.2/README.md` & `opentera-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/config/ConfigManager.py` & `opentera-1.2.3/opentera/config/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/crypto/crypto_utils.py` & `opentera-1.2.3/opentera/crypto/crypto_utils.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/db/Base.py` & `opentera-1.2.3/opentera/db/Base.py`

 * *Files 2% similar despite different names*

```diff
@@ -297,18 +297,19 @@
         missing_fields = []
 
         # Browse each
         pr_dict = dict()
         for name in dir(cls):
             value = getattr(cls, name)
             if cls.is_valid_property_name(name) and cls.is_valid_property_value(value) and \
-                    (name.startswith(model_name) or name.startswith('id')):
+                    (name.startswith(model_name) or name.startswith('id')) and not name.endswith('uuid'):
                 # Ok so far, check if column is required or not
                 if 'ColumnProperty' in str(type(value.prop)):
-                    if not value.prop.columns[0].nullable and name not in json_data and name not in ignore_fields:
+                    if not value.prop.columns[0].nullable and name not in json_data and name not in ignore_fields and \
+                            not value.prop.columns[0].default:
                         missing_fields.append(name)
 
         return missing_fields
 
 
 # Declarative base, inherit from Base for all models
 BaseModel = declarative_base(cls=BaseMixin)
```

### Comparing `opentera-1.2.2/opentera/db/SoftDeleteMixin.py` & `opentera-1.2.3/opentera/db/SoftDeleteMixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     #     state.statement = adapted
     @listens_for(Engine, "before_execute", retval=True)
     def soft_delete_execute(conn: Connection, clauseelement, multiparams, params, execution_options):
         if not isinstance(clauseelement, Select):
             return clauseelement, multiparams, params
 
         if disable_soft_delete_option_name in execution_options and execution_options[disable_soft_delete_option_name]:
-            print('test_include_deleted')
+            # print('test_include_deleted')
             return clauseelement, multiparams, params
 
         adapted = SoftDeleteQueryRewriter(deleted_field_name, disable_soft_delete_option_name).rewrite_statement(
             clauseelement
         )
         return adapted, multiparams, params
```

### Comparing `opentera-1.2.2/opentera/db/SoftDeleteQueryRewriter.py` & `opentera-1.2.3/opentera/db/SoftDeleteQueryRewriter.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/db/SoftInsertMixin.py` & `opentera-1.2.3/opentera/db/SoftInsertMixin.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/db/models/TeraAsset.py` & `opentera-1.2.3/opentera/db/models/TeraAsset.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/db/models/TeraDevice.py` & `opentera-1.2.3/opentera/db/models/TeraDevice.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/db/models/TeraDeviceParticipant.py` & `opentera-1.2.3/opentera/db/models/TeraDeviceParticipant.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/db/models/TeraDeviceProject.py` & `opentera-1.2.3/opentera/db/models/TeraDeviceProject.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/db/models/TeraDeviceSite.py` & `opentera-1.2.3/opentera/db/models/TeraDeviceSite.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/db/models/TeraDeviceSubType.py` & `opentera-1.2.3/opentera/db/models/TeraDeviceSubType.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/db/models/TeraDeviceType.py` & `opentera-1.2.3/opentera/db/models/TeraDeviceType.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,14 +22,16 @@
         return device_type_json
 
     def get_name(self) -> str:
         return self.device_type_name
 
     @staticmethod
     def create_defaults(test=False):
+        if not test:
+            return
         # For now Defaults are hard coded
         VIDEOCONFERENCE = TeraDeviceType()
         VIDEOCONFERENCE.device_type_name = 'Vidéoconférence'
         VIDEOCONFERENCE.device_type_key = 'videoconference'
         TeraDeviceType.db().session.add(VIDEOCONFERENCE)
 
         CAPTEUR = TeraDeviceType()
```

### Comparing `opentera-1.2.2/opentera/db/models/TeraParticipant.py` & `opentera-1.2.3/opentera/db/models/TeraParticipant.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/db/models/TeraParticipantGroup.py` & `opentera-1.2.3/opentera/db/models/TeraParticipantGroup.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/db/models/TeraProject.py` & `opentera-1.2.3/opentera/db/models/TeraProject.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/db/models/TeraServerSettings.py` & `opentera-1.2.3/opentera/db/models/TeraServerSettings.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/db/models/TeraService.py` & `opentera-1.2.3/opentera/db/models/TeraService.py`

 * *Files 0% similar despite different names*

```diff
@@ -166,24 +166,25 @@
         new_service.service_port = 4042
         new_service.service_endpoint = '/'
         new_service.service_clientendpoint = '/file'
         new_service.service_enabled = True
         new_service.service_system = True
         TeraService.db().session.add(new_service)
 
-        new_service = TeraService()
-        new_service.service_uuid = str(uuid.uuid4())
-        new_service.service_key = 'BureauActif'
-        new_service.service_name = 'Bureau Actif'
-        new_service.service_hostname = '127.0.0.1'
-        new_service.service_port = 4050
-        new_service.service_endpoint = '/'
-        new_service.service_clientendpoint = '/bureau'
-        new_service.service_enabled = True
-        TeraService.db().session.add(new_service)
+        if test:
+            new_service = TeraService()
+            new_service.service_uuid = str(uuid.uuid4())
+            new_service.service_key = 'BureauActif'
+            new_service.service_name = 'Bureau Actif'
+            new_service.service_hostname = '127.0.0.1'
+            new_service.service_port = 4050
+            new_service.service_endpoint = '/'
+            new_service.service_clientendpoint = '/bureau'
+            new_service.service_enabled = True
+            TeraService.db().session.add(new_service)
 
         new_service = TeraService()
         new_service.service_uuid = str(uuid.uuid4())
         new_service.service_key = 'VideoRehabService'
         new_service.service_name = 'Télé-réadaptation vidéo'
         new_service.service_hostname = '127.0.0.1'
         new_service.service_port = 4070
@@ -194,25 +195,26 @@
         # new_service.service_endpoint_user = '/user'
         # new_service.service_endpoint_device = '/device'
         new_service.service_enabled = True
         new_service.service_editable_config = True
         new_service.service_system = True
         TeraService.db().session.add(new_service)
 
-        new_service = TeraService()
-        new_service.service_uuid = str(uuid.uuid4())
-        new_service.service_key = 'RobotTeleOperationService'
-        new_service.service_name = 'Robot Teleoperation Service'
-        new_service.service_hostname = '127.0.0.1'
-        new_service.service_port = 4080
-        new_service.service_endpoint = '/'
-        new_service.service_clientendpoint = '/robot'
-        new_service.service_enabled = True
-        TeraService.db().session.add(new_service)
-        TeraService.db().session.commit()
+        if test:
+            new_service = TeraService()
+            new_service.service_uuid = str(uuid.uuid4())
+            new_service.service_key = 'RobotTeleOperationService'
+            new_service.service_name = 'Robot Teleoperation Service'
+            new_service.service_hostname = '127.0.0.1'
+            new_service.service_port = 4080
+            new_service.service_endpoint = '/'
+            new_service.service_clientendpoint = '/robot'
+            new_service.service_enabled = True
+            TeraService.db().session.add(new_service)
+            TeraService.db().session.commit()
 
     def to_json_create_event(self):
         return self.to_json(minimal=False)
 
     def to_json_update_event(self):
         return self.to_json(minimal=False)
```

### Comparing `opentera-1.2.2/opentera/db/models/TeraServiceAccess.py` & `opentera-1.2.3/opentera/db/models/TeraServiceAccess.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from opentera.db.Base import BaseModel
 from opentera.db.SoftDeleteMixin import SoftDeleteMixin
 from opentera.db.SoftInsertMixin import SoftInsertMixin
 from sqlalchemy import Column, ForeignKey, Integer, Sequence
 from sqlalchemy.orm import relationship
 from opentera.db.models.TeraServiceRole import TeraServiceRole
-import modules.Globals as Globals
 
 
 class TeraServiceAccess(BaseModel, SoftDeleteMixin, SoftInsertMixin):
     __tablename__ = 't_services_access'
     id_service_access = Column(Integer, Sequence('id_service_project_role_sequence'), primary_key=True,
                                autoincrement=True)
     id_user_group = Column(Integer, ForeignKey('t_users_groups.id_user_group', ondelete='cascade'),
@@ -155,31 +154,14 @@
                 TeraServiceAccess.delete(service_access.id_service_access)
                 return
 
             if id_project and service_access.service_access_role.id_project == id_project:
                 TeraServiceAccess.delete(service_access.id_service_access)
                 return
 
-    # TODO: Delete those methods (replaced by the generic one)
-    @staticmethod
-    def delete_service_access_for_user_group_for_site(id_site: int, id_user_group: int):
-        for service_access in TeraServiceAccess.get_service_access_for_user_group(
-                id_service=Globals.opentera_service_id, id_user_group=id_user_group):
-            if service_access.service_access_role.id_site == id_site:
-                TeraServiceAccess.delete(service_access.id_service_access)
-                break
-
-    @staticmethod
-    def delete_service_access_for_user_group_for_project(id_project: int, id_user_group: int):
-        for service_access in TeraServiceAccess.get_service_access_for_user_group(
-                id_service=Globals.opentera_service_id, id_user_group=id_user_group):
-            if service_access.service_access_role.id_project == id_project:
-                TeraServiceAccess.delete(service_access.id_service_access)
-                break
-
     @staticmethod
     def create_defaults(test=False):
         if test:
             from opentera.db.models.TeraService import TeraService
             from opentera.db.models.TeraUserGroup import TeraUserGroup
             from opentera.db.models.TeraDevice import TeraDevice
             from opentera.db.models.TeraParticipantGroup import TeraParticipantGroup
```

### Comparing `opentera-1.2.2/opentera/db/models/TeraServiceConfig.py` & `opentera-1.2.3/opentera/db/models/TeraServiceConfig.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/db/models/TeraServiceConfigSpecific.py` & `opentera-1.2.3/opentera/db/models/TeraServiceConfigSpecific.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/db/models/TeraServiceProject.py` & `opentera-1.2.3/opentera/db/models/TeraServiceProject.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/db/models/TeraServiceRole.py` & `opentera-1.2.3/opentera/db/models/TeraServiceRole.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/db/models/TeraServiceSite.py` & `opentera-1.2.3/opentera/db/models/TeraServiceSite.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/db/models/TeraSession.py` & `opentera-1.2.3/opentera/db/models/TeraSession.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/db/models/TeraSessionDevices.py` & `opentera-1.2.3/opentera/db/models/TeraSessionDevices.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/db/models/TeraSessionEvent.py` & `opentera-1.2.3/opentera/db/models/TeraSessionEvent.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/db/models/TeraSessionParticipants.py` & `opentera-1.2.3/opentera/db/models/TeraSessionParticipants.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/db/models/TeraSessionType.py` & `opentera-1.2.3/opentera/db/models/TeraSessionType.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,14 +66,16 @@
 
     def to_json_delete_event(self):
         # Minimal information, delete can not be filtered
         return {'id_session_type': self.id_session_type, 'id_service': self.id_service}
 
     @staticmethod
     def create_defaults(test=False):
+        if not test:
+            return
         # from opentera.db.models.TeraProject import TeraProject
         # from opentera.db.models.TeraDeviceType import TeraDeviceType
         from opentera.db.models.TeraService import TeraService
 
         # type_project = TeraProject.get_project_by_projectname('Default Project #1')
         video_session = TeraSessionType()
         video_session.session_type_name = "Suivi vidéo"
```

### Comparing `opentera-1.2.2/opentera/db/models/TeraSessionTypeProject.py` & `opentera-1.2.3/opentera/db/models/TeraSessionTypeProject.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from opentera.db.Base import BaseModel
 from opentera.db.models.TeraSession import TeraSession
+from opentera.db.models.TeraSessionType import TeraSessionType
 from opentera.db.SoftDeleteMixin import SoftDeleteMixin
 from opentera.db.SoftInsertMixin import SoftInsertMixin
 from sqlalchemy import Column, ForeignKey, Integer, Sequence
 from sqlalchemy.orm import relationship
 from sqlalchemy.exc import IntegrityError
 
 
@@ -25,14 +26,31 @@
         if minimal:
             ignore_fields.extend([])
 
         rval = super().to_json(ignore_fields=ignore_fields)
 
         return rval
 
+    def to_json_create_event(self):
+        json_data = self.to_json(minimal=True)
+        # Query session type information
+        session_type = TeraSessionType.get_session_type_by_id(self.id_session_type)
+        if session_type:
+            json_data['session_type_id_service'] = session_type.id_service
+        return json_data
+
+    def to_json_update_event(self):
+        json_data = self.to_json(minimal=True)
+        json_data['session_type_id_service'] = self.session_type_project_session_type.id_service
+        return json_data
+
+    def to_json_delete_event(self):
+        # Minimal information, delete can not be filtered
+        return {'id_session_type_project': self.id_session_type_project}
+
     @staticmethod
     def create_defaults(test=False):
         if test:
             from opentera.db.models.TeraSessionType import TeraSessionType
             from opentera.db.models.TeraProject import TeraProject
 
             video_session = TeraSessionType.get_session_type_by_id(1)
```

### Comparing `opentera-1.2.2/opentera/db/models/TeraSessionTypeSite.py` & `opentera-1.2.3/opentera/db/models/TeraSessionTypeSite.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from opentera.db.Base import BaseModel
 from opentera.db.models.TeraSessionTypeProject import TeraSessionTypeProject
+from opentera.db.models.TeraSessionType import TeraSessionType
 from opentera.db.SoftDeleteMixin import SoftDeleteMixin
 from opentera.db.SoftInsertMixin import SoftInsertMixin
 from sqlalchemy import Column, ForeignKey, Integer, Sequence
 from sqlalchemy.orm import relationship
 from sqlalchemy.exc import IntegrityError
 
 
@@ -24,14 +25,31 @@
         if minimal:
             ignore_fields.extend([])
 
         rval = super().to_json(ignore_fields=ignore_fields)
 
         return rval
 
+    def to_json_create_event(self):
+        json_data = self.to_json(minimal=True)
+        # Query session type information
+        session_type = TeraSessionType.get_session_type_by_id(self.id_session_type)
+        if session_type:
+            json_data['session_type_id_service'] = session_type.id_service
+        return json_data
+
+    def to_json_update_event(self):
+        json_data = self.to_json(minimal=True)
+        json_data['session_type_id_service'] = self.session_type_site_session_type.id_service
+        return json_data
+
+    def to_json_delete_event(self):
+        # Minimal information, delete can not be filtered
+        return {'id_session_type_site': self.id_session_type_site}
+
     @staticmethod
     def create_defaults(test=False):
         if test:
             from opentera.db.models.TeraSessionType import TeraSessionType
             from opentera.db.models.TeraSite import TeraSite
 
             video_session = TeraSessionType.get_session_type_by_id(1)
```

### Comparing `opentera-1.2.2/opentera/db/models/TeraSessionUsers.py` & `opentera-1.2.3/opentera/db/models/TeraSessionUsers.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/db/models/TeraSite.py` & `opentera-1.2.3/opentera/db/models/TeraSite.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/db/models/TeraTest.py` & `opentera-1.2.3/opentera/db/models/TeraTest.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/db/models/TeraTestType.py` & `opentera-1.2.3/opentera/db/models/TeraTestType.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/db/models/TeraTestTypeProject.py` & `opentera-1.2.3/opentera/db/models/TeraTestTypeProject.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/db/models/TeraTestTypeSite.py` & `opentera-1.2.3/opentera/db/models/TeraTestTypeSite.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/db/models/TeraUser.py` & `opentera-1.2.3/opentera/db/models/TeraUser.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/db/models/TeraUserGroup.py` & `opentera-1.2.3/opentera/db/models/TeraUserGroup.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/db/models/TeraUserPreference.py` & `opentera-1.2.3/opentera/db/models/TeraUserPreference.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/db/models/TeraUserUserGroup.py` & `opentera-1.2.3/opentera/db/models/TeraUserUserGroup.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/db/models/__init__.py` & `opentera-1.2.3/opentera/db/models/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -48,15 +48,17 @@
     TeraSession.get_model_name(): TeraSession,
     TeraSessionType.get_model_name(): TeraSessionType,
     TeraSite.get_model_name(): TeraSite,
     TeraUser.get_model_name(): TeraUser,
     TeraUserGroup.get_model_name(): TeraUserGroup,
     TeraTestType.get_model_name(): TeraTestType,
     TeraTest.get_model_name(): TeraTest,
-    TeraService.get_model_name(): TeraService
+    TeraService.get_model_name(): TeraService,
+    TeraSessionTypeSite.get_model_name(): TeraSessionTypeSite,
+    TeraSessionTypeProject.get_model_name(): TeraSessionTypeProject
 }
 
 # All exported symbols
 __all__ = ['TeraAsset',
            'TeraDevice',
            'TeraDeviceParticipant',
            'TeraDeviceProject',
```

### Comparing `opentera-1.2.2/opentera/forms/TeraDeviceForm.py` & `opentera-1.2.3/opentera/forms/TeraDeviceForm.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/forms/TeraDeviceSubTypeForm.py` & `opentera-1.2.3/opentera/forms/TeraDeviceSubTypeForm.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/forms/TeraDeviceTypeForm.py` & `opentera-1.2.3/opentera/forms/TeraDeviceTypeForm.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/forms/TeraForm.py` & `opentera-1.2.3/opentera/forms/TeraForm.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/forms/TeraParticipantForm.py` & `opentera-1.2.3/opentera/forms/TeraParticipantForm.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/forms/TeraParticipantGroupForm.py` & `opentera-1.2.3/opentera/forms/TeraParticipantGroupForm.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/forms/TeraProjectForm.py` & `opentera-1.2.3/opentera/forms/TeraProjectForm.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/forms/TeraServiceConfigForm.py` & `opentera-1.2.3/opentera/forms/TeraServiceConfigForm.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/forms/TeraServiceForm.py` & `opentera-1.2.3/opentera/forms/TeraServiceForm.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/forms/TeraSessionForm.py` & `opentera-1.2.3/opentera/forms/TeraSessionForm.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/forms/TeraSessionTypeForm.py` & `opentera-1.2.3/opentera/forms/TeraSessionTypeForm.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/forms/TeraSiteForm.py` & `opentera-1.2.3/opentera/forms/TeraSiteForm.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/forms/TeraTestTypeForm.py` & `opentera-1.2.3/opentera/forms/TeraTestTypeForm.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/forms/TeraUserForm.py` & `opentera-1.2.3/opentera/forms/TeraUserForm.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/forms/TeraUserGroupForm.py` & `opentera-1.2.3/opentera/forms/TeraUserGroupForm.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/forms/TeraVersionsForm.py` & `opentera-1.2.3/opentera/forms/TeraVersionsForm.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/logging/LoggingClient.py` & `opentera-1.2.3/opentera/logging/LoggingClient.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/messages/python/CreateSession_pb2.py` & `opentera-1.2.3/opentera/messages/python/CreateSession_pb2.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/messages/python/DatabaseEvent_pb2.py` & `opentera-1.2.3/opentera/messages/python/DatabaseEvent_pb2.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/messages/python/DeviceEvent_pb2.py` & `opentera-1.2.3/opentera/messages/python/DeviceEvent_pb2.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/messages/python/JoinSessionEvent_pb2.py` & `opentera-1.2.3/opentera/messages/python/JoinSessionEvent_pb2.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/messages/python/JoinSessionReplyEvent_pb2.py` & `opentera-1.2.3/opentera/messages/python/JoinSessionReplyEvent_pb2.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/messages/python/LeaveSessionEvent_pb2.py` & `opentera-1.2.3/opentera/messages/python/LeaveSessionEvent_pb2.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/messages/python/LogEvent_pb2.py` & `opentera-1.2.3/opentera/messages/python/LogEvent_pb2.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/messages/python/LoginEvent_pb2.py` & `opentera-1.2.3/opentera/messages/python/LoginEvent_pb2.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/messages/python/ParticipantEvent_pb2.py` & `opentera-1.2.3/opentera/messages/python/ParticipantEvent_pb2.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/messages/python/RPCMessage_pb2.py` & `opentera-1.2.3/opentera/messages/python/RPCMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/messages/python/Result_pb2.py` & `opentera-1.2.3/opentera/messages/python/Result_pb2.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/messages/python/ServerCommand_pb2.py` & `opentera-1.2.3/opentera/messages/python/ServerCommand_pb2.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/messages/python/StopSessionEvent_pb2.py` & `opentera-1.2.3/opentera/messages/python/StopSessionEvent_pb2.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/messages/python/TeraEvent_pb2.py` & `opentera-1.2.3/opentera/messages/python/TeraEvent_pb2.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/messages/python/TeraMessage_pb2.py` & `opentera-1.2.3/opentera/messages/python/TeraMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/messages/python/TeraModuleMessage_pb2.py` & `opentera-1.2.3/opentera/messages/python/TeraModuleMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/messages/python/UserEvent_pb2.py` & `opentera-1.2.3/opentera/messages/python/UserEvent_pb2.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/messages/python/UserRegisterToEvent_pb2.py` & `opentera-1.2.3/opentera/messages/python/UserRegisterToEvent_pb2.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/messages/python/__init__.py` & `opentera-1.2.3/opentera/messages/python/__init__.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/modules/BaseModule.py` & `opentera-1.2.3/opentera/modules/BaseModule.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/redis/RedisClient.py` & `opentera-1.2.3/opentera/redis/RedisClient.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/redis/RedisProtocolFactory.py` & `opentera-1.2.3/opentera/redis/RedisProtocolFactory.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/redis/RedisRPCClient.py` & `opentera-1.2.3/opentera/redis/RedisRPCClient.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/redis/RedisVars.py` & `opentera-1.2.3/opentera/redis/RedisVars.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/services/BaseWebRTCService.py` & `opentera-1.2.3/opentera/services/BaseWebRTCService.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/services/DisabledTokenStorage.py` & `opentera-1.2.3/opentera/services/DisabledTokenStorage.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/services/ServiceAccessManager.py` & `opentera-1.2.3/opentera/services/ServiceAccessManager.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/services/ServiceConfigManager.py` & `opentera-1.2.3/opentera/services/ServiceConfigManager.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/services/ServiceOpenTera.py` & `opentera-1.2.3/opentera/services/ServiceOpenTera.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/services/ServiceOpenTeraWithAssets.py` & `opentera-1.2.3/opentera/services/ServiceOpenTeraWithAssets.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/services/ServiceOpenTeraWithTests.py` & `opentera-1.2.3/opentera/services/ServiceOpenTeraWithTests.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/services/TeraDeviceClient.py` & `opentera-1.2.3/opentera/services/TeraDeviceClient.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/services/TeraParticipantClient.py` & `opentera-1.2.3/opentera/services/TeraParticipantClient.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/services/TeraServiceClient.py` & `opentera-1.2.3/opentera/services/TeraServiceClient.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/services/TeraUserClient.py` & `opentera-1.2.3/opentera/services/TeraUserClient.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/services/modules/WebRTCModule.py` & `opentera-1.2.3/opentera/services/modules/WebRTCModule.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/utils/Metrics.py` & `opentera-1.2.3/opentera/utils/Metrics.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/utils/TeraVersions.py` & `opentera-1.2.3/opentera/utils/TeraVersions.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/utils/UserAgentParser.py` & `opentera-1.2.3/opentera/utils/UserAgentParser.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera/utils/assets/BaseAsset.py` & `opentera-1.2.3/opentera/utils/assets/BaseAsset.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera.egg-info/PKG-INFO` & `opentera-1.2.3/opentera.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentera
-Version: 1.2.2
+Version: 1.2.3
 Summary: OpenTera base package
 Home-page: https://github.com/introlab/opentera
 Author: Dominic Létourneau, Simon Brière
 Author-email: dominic.letourneau@usherbrooke.ca, simon.briere@usherbrooke.ca
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `opentera-1.2.2/opentera.egg-info/SOURCES.txt` & `opentera-1.2.3/opentera.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/opentera.egg-info/requires.txt` & `opentera-1.2.3/opentera.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/setup.py` & `opentera-1.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open("env/requirements.txt", "r", encoding="utf-8") as f:
     requirements = f.readlines()
     requirements.append('protobuf==3.20.3')
 
 setuptools.setup(
     name="opentera",
-    version="1.2.2",
+    version="1.2.3",
     author="Dominic Létourneau, Simon Brière",
     author_email="dominic.letourneau@usherbrooke.ca, simon.briere@usherbrooke.ca",
     description="OpenTera base package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/introlab/opentera",
     packages=setuptools.find_packages(),
```

### Comparing `opentera-1.2.2/translations/en/LC_MESSAGES/messages.po` & `opentera-1.2.3/translations/en/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/translations/fr/LC_MESSAGES/messages.mo` & `opentera-1.2.3/translations/fr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `opentera-1.2.2/translations/fr/LC_MESSAGES/messages.po` & `opentera-1.2.3/translations/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

