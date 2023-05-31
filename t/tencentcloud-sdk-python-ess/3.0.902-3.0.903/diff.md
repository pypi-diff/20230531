# Comparing `tmp/tencentcloud-sdk-python-ess-3.0.902.tar.gz` & `tmp/tencentcloud-sdk-python-ess-3.0.903.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.902.tar", last modified: Tue May 30 00:23:14 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.903.tar", last modified: Wed May 31 02:11:28 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ess-3.0.902.tar` & `tencentcloud-sdk-python-ess-3.0.903.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:23:14.000000 tencentcloud-sdk-python-ess-3.0.902/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-30 00:23:14.000000 tencentcloud-sdk-python-ess-3.0.902/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:23:14.000000 tencentcloud-sdk-python-ess-3.0.902/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-30 00:23:14.000000 tencentcloud-sdk-python-ess-3.0.902/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:23:14.000000 tencentcloud-sdk-python-ess-3.0.902/tencentcloud/ess/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 00:23:14.000000 tencentcloud-sdk-python-ess-3.0.902/tencentcloud/ess/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:23:14.000000 tencentcloud-sdk-python-ess-3.0.902/tencentcloud/ess/v20201111/
--rw-r--r--   0 root         (0) root         (0)    51121 2023-05-30 00:23:14.000000 tencentcloud-sdk-python-ess-3.0.902/tencentcloud/ess/v20201111/ess_client.py
--rw-r--r--   0 root         (0) root         (0)    23981 2023-05-30 00:23:14.000000 tencentcloud-sdk-python-ess-3.0.902/tencentcloud/ess/v20201111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 00:23:14.000000 tencentcloud-sdk-python-ess-3.0.902/tencentcloud/ess/v20201111/__init__.py
--rw-r--r--   0 root         (0) root         (0)   223871 2023-05-30 00:23:14.000000 tencentcloud-sdk-python-ess-3.0.902/tencentcloud/ess/v20201111/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:23:14.000000 tencentcloud-sdk-python-ess-3.0.902/tencentcloud_sdk_python_ess.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 00:23:14.000000 tencentcloud-sdk-python-ess-3.0.902/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-30 00:23:14.000000 tencentcloud-sdk-python-ess-3.0.902/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-30 00:23:14.000000 tencentcloud-sdk-python-ess-3.0.902/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-30 00:23:14.000000 tencentcloud-sdk-python-ess-3.0.902/tencentcloud_sdk_python_ess.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-30 00:23:14.000000 tencentcloud-sdk-python-ess-3.0.902/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-30 00:23:14.000000 tencentcloud-sdk-python-ess-3.0.902/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-30 00:23:14.000000 tencentcloud-sdk-python-ess-3.0.902/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:11:28.000000 tencentcloud-sdk-python-ess-3.0.903/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-31 02:11:27.000000 tencentcloud-sdk-python-ess-3.0.903/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:11:28.000000 tencentcloud-sdk-python-ess-3.0.903/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-31 02:11:27.000000 tencentcloud-sdk-python-ess-3.0.903/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:11:28.000000 tencentcloud-sdk-python-ess-3.0.903/tencentcloud/ess/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 02:11:27.000000 tencentcloud-sdk-python-ess-3.0.903/tencentcloud/ess/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:11:28.000000 tencentcloud-sdk-python-ess-3.0.903/tencentcloud/ess/v20201111/
+-rw-r--r--   0 root         (0) root         (0)    51121 2023-05-31 02:11:27.000000 tencentcloud-sdk-python-ess-3.0.903/tencentcloud/ess/v20201111/ess_client.py
+-rw-r--r--   0 root         (0) root         (0)    24243 2023-05-31 02:11:27.000000 tencentcloud-sdk-python-ess-3.0.903/tencentcloud/ess/v20201111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 02:11:27.000000 tencentcloud-sdk-python-ess-3.0.903/tencentcloud/ess/v20201111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   225454 2023-05-31 02:11:27.000000 tencentcloud-sdk-python-ess-3.0.903/tencentcloud/ess/v20201111/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:11:28.000000 tencentcloud-sdk-python-ess-3.0.903/tencentcloud_sdk_python_ess.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 02:11:28.000000 tencentcloud-sdk-python-ess-3.0.903/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-31 02:11:28.000000 tencentcloud-sdk-python-ess-3.0.903/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-31 02:11:28.000000 tencentcloud-sdk-python-ess-3.0.903/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-31 02:11:28.000000 tencentcloud-sdk-python-ess-3.0.903/tencentcloud_sdk_python_ess.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-31 02:11:28.000000 tencentcloud-sdk-python-ess-3.0.903/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-31 02:11:27.000000 tencentcloud-sdk-python-ess-3.0.903/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-31 02:11:28.000000 tencentcloud-sdk-python-ess-3.0.903/setup.cfg
```

### Comparing `tencentcloud-sdk-python-ess-3.0.902/README.rst` & `tencentcloud-sdk-python-ess-3.0.903/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.902/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ess-3.0.903/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.902'
+__version__ = '3.0.903'
```

### Comparing `tencentcloud-sdk-python-ess-3.0.902/tencentcloud/ess/v20201111/ess_client.py` & `tencentcloud-sdk-python-ess-3.0.903/tencentcloud/ess/v20201111/ess_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.902/tencentcloud/ess/v20201111/errorcodes.py` & `tencentcloud-sdk-python-ess-3.0.903/tencentcloud/ess/v20201111/errorcodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,14 +175,17 @@
 
 # 数据已存在。
 INVALIDPARAMETER_DATAEXISTS = 'InvalidParameter.DataExists'
 
 # 数据不存在。
 INVALIDPARAMETER_DATANOTFOUND = 'InvalidParameter.DataNotFound'
 
+# 部门用户Id不正确
+INVALIDPARAMETER_DEPARTUSERID = 'InvalidParameter.DepartUserId'
+
 # 参数为空，请检查参数修改后重试。
 INVALIDPARAMETER_EMPTYPARAMS = 'InvalidParameter.EmptyParams'
 
 # 不合法的EndPoint，请检查修改后重试。
 INVALIDPARAMETER_ENDPOINT = 'InvalidParameter.EndPoint'
 
 # 不合法的签署流程回调链接，请修改后重试。
@@ -277,23 +280,26 @@
 
 # 个人静默签Tag未设置，请检查后重试。
 INVALIDPARAMETER_PERSONAUTOSIGNTAG = 'InvalidParameter.PersonAutoSignTag'
 
 # 不合法的阅读时长限制，请联系客服了解阅读时长设置规则，修改后重试。
 INVALIDPARAMETER_PREREADTIME = 'InvalidParameter.PreReadTime'
 
-# 签署二维码的有效期不合法，请联系客服了解规则，并修稿后重试。
+# 签署二维码的有效期不合法，请联系客服了解规则，并修改后重试。
 INVALIDPARAMETER_QREFFECTDAY = 'InvalidParameter.QrEffectDay'
 
-# 二维码合同的有效期不合法，请联系客服了解规则，并修稿后重试。
+# 二维码合同的有效期不合法，请联系客服了解规则，并修改后重试。
 INVALIDPARAMETER_QRFLOWEFFECTDAY = 'InvalidParameter.QrFlowEffectDay'
 
 # 不合法的资源类型，请联系客服了解，并在修改后重试。
 INVALIDPARAMETER_RESOURCETYPE = 'InvalidParameter.ResourceType'
 
+# 角色ID不正确
+INVALIDPARAMETER_ROLEID = 'InvalidParameter.RoleId'
+
 # 不合法的印章id，请检查印章id是够正确，并在修改后重试。
 INVALIDPARAMETER_SEALID = 'InvalidParameter.SealId'
 
 # 参数包含有敏感词
 INVALIDPARAMETER_SENSITIVE = 'InvalidParameter.Sensitive'
 
 # 签署控件参数不合法，请检查后重试。
@@ -307,14 +313,17 @@
 
 # 不合法的认证渠道，请联系客户了解电子签支持的认证渠道，并在修改后重试。
 INVALIDPARAMETER_VERIFYCHANNEL = 'InvalidParameter.VerifyChannel'
 
 # 参数取值错误。
 INVALIDPARAMETERVALUE = 'InvalidParameterValue'
 
+# 无效的手机号
+INVALIDPARAMETERVALUE_INVALIDMOBILE = 'InvalidParameterValue.InvalidMobile'
+
 # 需要屏蔽的告警。
 INVALIDPARAMETERVALUE_MASK = 'InvalidParameterValue.Mask'
 
 # 超过配额限制。
 LIMITEXCEEDED = 'LimitExceeded'
 
 # 缺少参数错误。
```

### Comparing `tencentcloud-sdk-python-ess-3.0.902/tencentcloud/ess/v20201111/models.py` & `tencentcloud-sdk-python-ess-3.0.903/tencentcloud/ess/v20201111/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,40 +93,40 @@
         r"""
         :param ApproverType: 参与者类型：
 0：企业
 1：个人
 3：企业静默签署
 注：类型为3（企业静默签署）时，此接口会默认完成该签署方的签署。静默签署仅进行盖章操作，不能自动签名。
         :type ApproverType: int
-        :param ApproverName: 本环节需要操作人的名字
+        :param ApproverName: 签署人的姓名
         :type ApproverName: str
-        :param ApproverMobile: 本环节需要操作人的手机号
+        :param ApproverMobile: 签署人的手机号，11位数字
         :type ApproverMobile: str
-        :param SignComponents: 本环节操作人签署控件配置
+        :param SignComponents: 签署人的签署控件列表
         :type SignComponents: list of Component
-        :param OrganizationName: 如果是企业,则为企业的名字
+        :param OrganizationName: 如果签署方是企业签署方，则为企业名
         :type OrganizationName: str
-        :param ApproverIdCardNumber: 身份证号
+        :param ApproverIdCardNumber: 签署人的身份证号
         :type ApproverIdCardNumber: str
-        :param ApproverIdCardType: 证件类型 
+        :param ApproverIdCardType: 签署人的身份证件类型 
 ID_CARD 身份证
 HONGKONG_AND_MACAO 港澳居民来往内地通行证
 HONGKONG_MACAO_AND_TAIWAN 港澳台居民居住证(格式同居民身份证)
         :type ApproverIdCardType: str
-        :param NotifyType: sms--短信，none--不通知
+        :param NotifyType: 签署通知类型：sms--短信，none--不通知
         :type NotifyType: str
-        :param ApproverRole: 1--收款人、2--开具人、3--见证人
+        :param ApproverRole: 签署人角色类型：1--收款人、2--开具人、3--见证人
         :type ApproverRole: int
-        :param VerifyChannel: 签署意愿确认渠道,WEIXINAPP:人脸识别
+        :param VerifyChannel: 签署意愿确认渠道，默认为WEIXINAPP:人脸识别
         :type VerifyChannel: list of str
         :param PreReadTime: 合同的强制预览时间：3~300s，未指定则按合同页数计算
         :type PreReadTime: int
         :param UserId: 签署人userId，传此字段则不用传姓名、手机号
         :type UserId: str
-        :param ApproverSource: 签署人用户来源,企微侧用户请传入：WEWORKAPP
+        :param ApproverSource: 签署人用户来源，企微侧用户请传入：WEWORKAPP
         :type ApproverSource: str
         :param CustomApproverTag: 客户自定义签署人标识，64位长度，保证唯一，非企微场景不使用此字段
         :type CustomApproverTag: str
         :param ApproverOption: 签署人个性化能力值
         :type ApproverOption: :class:`tencentcloud.ess.v20201111.models.ApproverOption`
         :param ApproverVerifyTypes: 签署人查看合同时认证方式, 
 1-实名查看 2-短信验证码查看(企业签署方不支持该方式)
@@ -223,19 +223,19 @@
 
     """
 
     def __init__(self):
         r"""
         :param Name: 指定签署人名字
         :type Name: str
-        :param Mobile: 指定签署人手机号
+        :param Mobile: 指定签署人手机号，11位数字
         :type Mobile: str
-        :param IdCardType: 指定签署人证件类型
+        :param IdCardType: 指定签署人证件类型，ID_CARD-身份证
         :type IdCardType: str
-        :param IdCardNumber: 指定签署人证件号码
+        :param IdCardNumber: 指定签署人证件号码，字母大写
         :type IdCardNumber: str
         """
         self.Name = None
         self.Mobile = None
         self.IdCardType = None
         self.IdCardNumber = None
 
@@ -257,15 +257,15 @@
 class AuthorizedUser(AbstractModel):
     """授权用户
 
     """
 
     def __init__(self):
         r"""
-        :param UserId: 用户id
+        :param UserId: 电子签系统中的用户id
         :type UserId: str
         """
         self.UserId = None
 
 
     def _deserialize(self, params):
         self.UserId = params.get("UserId")
@@ -283,21 +283,21 @@
 
     """
 
     def __init__(self):
         r"""
         :param UserInfo: 自动签开通个人用户的三要素
         :type UserInfo: :class:`tencentcloud.ess.v20201111.models.UserThreeFactor`
-        :param CallbackUrl: 回调链接
+        :param CallbackUrl: 接受自动签开启的回调地址。需要保证post返回200
         :type CallbackUrl: str
-        :param CertInfoCallback: 是否回调证书信息
+        :param CertInfoCallback: 是否回调证书信息，默认false-不需要
         :type CertInfoCallback: bool
-        :param UserDefineSeal: 是否支持用户自定义签名印章
+        :param UserDefineSeal: 是否支持用户自定义签名印章，默认false-不需要
         :type UserDefineSeal: bool
-        :param SealImgCallback: 是否需要回调的时候返回印章(签名) 图片的 base64
+        :param SealImgCallback: 是否需要回调的时候返回印章(签名) 图片的 base64，默认false-不需要
         :type SealImgCallback: bool
         :param VerifyChannels: 开通时候的验证方式，取值：WEIXINAPP（微信人脸识别），INSIGHT（慧眼人脸认别），TELECOM（运营商三要素验证）。如果是小程序开通链接，支持传 WEIXINAPP / TELECOM。如果是 H5 开通链接，支持传 INSIGHT / TELECOM。默认值 WEIXINAPP / INSIGHT。
         :type VerifyChannels: list of str
         """
         self.UserInfo = None
         self.CallbackUrl = None
         self.CertInfoCallback = None
@@ -556,15 +556,15 @@
 class CcInfo(AbstractModel):
     """抄送信息
 
     """
 
     def __init__(self):
         r"""
-        :param Mobile: 被抄送人手机号
+        :param Mobile: 被抄送人手机号，11位数字
         :type Mobile: str
         :param Name: 被抄送人姓名
         :type Name: str
         :param CcType: 被抄送人类型,
 0--个人
 1--员工
         :type CcType: int
@@ -596,51 +596,51 @@
 class Component(AbstractModel):
     """模板控件信息
 
     """
 
     def __init__(self):
         r"""
-        :param ComponentType: 如果是Component控件类型，则可选的字段为：
+        :param ComponentType: 如果是Component填写控件类型，则可选的字段为：
 TEXT - 普通文本控件，输入文本字符串；
 MULTI_LINE_TEXT - 多行文本控件，输入文本字符串；
 CHECK_BOX - 勾选框控件，若选中填写ComponentValue 填写 true或者 false 字符串；
 FILL_IMAGE - 图片控件，ComponentValue 填写图片的资源 ID；
 DYNAMIC_TABLE - 动态表格控件；
 ATTACHMENT - 附件控件,ComponentValue 填写附件图片的资源 ID列表，以逗号分割；
 SELECTOR - 选择器控件，ComponentValue填写选择的字符串内容；
 DATE - 日期控件；默认是格式化为xxxx年xx月xx日字符串；
 DISTRICT - 省市区行政区控件，ComponentValue填写省市区行政区字符串内容；
 
-如果是SignComponent控件类型，则可选的字段为
+如果是SignComponent签署控件类型，则可选的字段为
 SIGN_SEAL - 签署印章控件；
 SIGN_DATE - 签署日期控件；
 SIGN_SIGNATURE - 用户签名控件；
 SIGN_PERSONAL_SEAL - 个人签署印章控件（使用文件发起暂不支持此类型）；
 SIGN_PAGING_SEAL - 骑缝章；若文件发起，需要对应填充ComponentPosY、ComponentWidth、ComponentHeight
 SIGN_OPINION - 签署意见控件，用户需要根据配置的签署意见内容，完成对意见内容的确认；
 SIGN_LEGAL_PERSON_SEAL - 企业法定代表人控件。
 
 表单域的控件不能作为印章和签名控件
         :type ComponentType: str
-        :param FileIndex: 控件所属文件的序号（模板中的resourceId排列序号，取值为：0-N）
+        :param FileIndex: 控件所属文件的序号（取值为：0-N）。目前单文件的情况下，值是0
         :type FileIndex: int
         :param ComponentHeight: 参数控件高度，单位pt
         :type ComponentHeight: float
         :param ComponentWidth: 参数控件宽度，单位pt
         :type ComponentWidth: float
         :param ComponentPage: 参数控件所在页码，取值为：1-N
         :type ComponentPage: int
         :param ComponentPosX: 参数控件X位置，单位pt
         :type ComponentPosX: float
         :param ComponentPosY: 参数控件Y位置，单位pt
         :type ComponentPosY: float
-        :param ComponentId: GenerateMode==KEYWORD 指定关键字
+        :param ComponentId: 查询时返回控件唯一Id。使用文件发起合同时用于GenerateMode==KEYWORD 指定关键字
         :type ComponentId: str
-        :param ComponentName: GenerateMode==FIELD 指定表单域名称
+        :param ComponentName: 查询时返回控件名。使用文件发起合同时用于GenerateMode==FIELD 指定表单域名称
         :type ComponentName: str
         :param ComponentRequired: 是否必选，默认为false
         :type ComponentRequired: bool
         :param ComponentRecipientId: 控件关联的签署人ID
         :type ComponentRecipientId: str
         :param ComponentExtra: 扩展参数：
 为JSON格式。
@@ -665,15 +665,15 @@
 3 FontAlign： 字符串类型，可取Left/Right/Center，对应左对齐/居中/右对齐
 4 Format： 字符串类型，日期格式，必须是以下五种之一 “yyyy m d”，”yyyy年m月d日”，”yyyy/m/d”，”yyyy-m-d”，”yyyy.m.d”。
 5 Gaps:： 字符串类型，仅在Format为“yyyy m d”时起作用，格式为用逗号分开的两个整数，例如”2,2”，两个数字分别是日期格式的前后两个空隙钟的空格个数
 如果extra参数为空，默认为”yyyy年m月d日”格式的居中日期
 特别地，如果extra中Format字段为空或无法被识别，则extra参数会被当作默认值处理（Font，FontSize，Gaps和FontAlign都不会起效）
 参数样例：    "ComponentExtra": "{\"Format\":“yyyy m d”,\"FontSize\":12,\"Gaps\":\"2,2\", \"FontAlign\":\"Right\"}",
         :type ComponentExtra: str
-        :param IsFormType: 是否是表单域类型，默认不存在
+        :param IsFormType: 是否是表单域类型，默认不false-不是
         :type IsFormType: bool
         :param ComponentValue: 控件填充vaule，ComponentType和传入值类型对应关系：
 TEXT - 文本内容
 MULTI_LINE_TEXT - 文本内容
 CHECK_BOX - true/false
 FILL_IMAGE、ATTACHMENT - 附件的FileId，需要通过UploadFiles接口上传获取
 SELECTOR - 选项值
@@ -750,21 +750,21 @@
         :type ComponentValue: str
         :param GenerateMode: NORMAL 正常模式，使用坐标制定签署控件位置
 FIELD 表单域，需使用ComponentName指定表单域名称
 KEYWORD 关键字，使用ComponentId指定关键字
         :type GenerateMode: str
         :param ComponentDateFontSize: 日期签署控件的字号，默认为 12
         :type ComponentDateFontSize: int
-        :param ChannelComponentId: 平台模板控件 id 标识
+        :param ChannelComponentId: 第三方应用集成平台模板控件 id 标识
         :type ChannelComponentId: str
         :param OffsetX: 指定关键字时横坐标偏移量，单位pt
         :type OffsetX: float
         :param OffsetY: 指定关键字时纵坐标偏移量，单位pt
         :type OffsetY: float
-        :param ChannelComponentSource: //子客控件来源。0-平台指定；1-用户自定义
+        :param ChannelComponentSource: 第三方应用集成中子客企业控件来源。0-平台指定；1-用户自定义
         :type ChannelComponentSource: int
         :param KeywordOrder: 指定关键字排序规则，Positive-正序，Reverse-倒序。传入Positive时会根据关键字在PDF文件内的顺序进行排列。在指定KeywordIndexes时，0代表在PDF内查找内容时，查找到的第一个关键字。
 传入Reverse时会根据关键字在PDF文件内的反序进行排列。在指定KeywordIndexes时，0代表在PDF内查找内容时，查找到的最后一个关键字。
         :type KeywordOrder: str
         :param KeywordPage: 指定关键字页码，可选参数，指定页码后，将只在指定的页码内查找关键字，非该页码的关键字将不会查询出来
         :type KeywordPage: int
         :param RelativeLocation: 关键字位置模式，Middle-居中，Below-正下方，Right-正右方，LowerRight-右上角，UpperRight-右下角。示例：如果设置Middle的关键字盖章，则印章的中心会和关键字的中心重合，如果设置Below，则印章在关键字的正下方
@@ -2040,57 +2040,77 @@
 class CreatePreparedPersonalEsignRequest(AbstractModel):
     """CreatePreparedPersonalEsign请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param UserName: 个人用户名称
+        :param UserName: 个人用户姓名
         :type UserName: str
         :param IdCardNumber: 身份证件号码
         :type IdCardNumber: str
-        :param SealImage: 印章图片的base64
-        :type SealImage: str
         :param SealName: 印章名称
         :type SealName: str
+        :param SealImage: 印章图片的base64，最大不超过 8M
+        :type SealImage: str
         :param Operator: 调用方用户信息，userId 必填。支持填入集团子公司经办人 userId代发合同。
         :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
         :param IdCardType: 身份证件类型:
 ID_CARD 身份证
 PASSPORT 护照
 HONGKONG_AND_MACAO 中国香港
 FOREIGN_ID_CARD 境外身份
 HONGKONG_MACAO_AND_TAIWAN 中国台湾
         :type IdCardType: str
+        :param SealImageCompress: 是否开启印章图片压缩处理，默认不开启，如需开启请设置为 true。当印章超过 2M 时建议开启，开启后图片的 hash 将发生变化。
+        :type SealImageCompress: bool
         :param Mobile: 手机号码；当需要开通自动签时，该参数必传
         :type Mobile: str
         :param EnableAutoSign: 是否开通自动签，该功能需联系运营工作人员开通后使用
         :type EnableAutoSign: bool
+        :param SealColor: 印章颜色（参数ProcessSeal=true时生效）
+默认值：BLACK黑色
+取值: 
+BLACK 黑色,
+RED 红色,
+BLUE 蓝色。
+        :type SealColor: str
+        :param ProcessSeal: 是否处理印章
+默认不做印章处理。
+取值：false：不做任何处理；
+true：做透明化处理和颜色增强。
+        :type ProcessSeal: bool
         """
         self.UserName = None
         self.IdCardNumber = None
-        self.SealImage = None
         self.SealName = None
+        self.SealImage = None
         self.Operator = None
         self.IdCardType = None
+        self.SealImageCompress = None
         self.Mobile = None
         self.EnableAutoSign = None
+        self.SealColor = None
+        self.ProcessSeal = None
 
 
     def _deserialize(self, params):
         self.UserName = params.get("UserName")
         self.IdCardNumber = params.get("IdCardNumber")
-        self.SealImage = params.get("SealImage")
         self.SealName = params.get("SealName")
+        self.SealImage = params.get("SealImage")
         if params.get("Operator") is not None:
             self.Operator = UserInfo()
             self.Operator._deserialize(params.get("Operator"))
         self.IdCardType = params.get("IdCardType")
+        self.SealImageCompress = params.get("SealImageCompress")
         self.Mobile = params.get("Mobile")
         self.EnableAutoSign = params.get("EnableAutoSign")
+        self.SealColor = params.get("SealColor")
+        self.ProcessSeal = params.get("ProcessSeal")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -3813,15 +3833,15 @@
         :type DisplayName: str
         :param Mobile: 用户传入的手机号
         :type Mobile: str
         :param Reason: 失败原因
         :type Reason: str
         :param UserId: 用户Id
         :type UserId: str
-        :param OpenId: 用户OpenId
+        :param OpenId: 员工在第三方平台的openId
         :type OpenId: str
         """
         self.DisplayName = None
         self.Mobile = None
         self.Reason = None
         self.UserId = None
         self.OpenId = None
@@ -3839,15 +3859,15 @@
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class FileInfo(AbstractModel):
-    """二期接口返回的模板中文件的信息结构
+    """模板中文件的信息结构
 
     """
 
     def __init__(self):
         r"""
         :param FileId: 文件Id
         :type FileId: str
@@ -5582,14 +5602,19 @@
         :type Status: int
         :param Creator: 模板的创建人
         :type Creator: str
         :param CreatedOn: 模板创建的时间戳（精确到秒）
         :type CreatedOn: int
         :param Promoter: 发起人角色信息
         :type Promoter: :class:`tencentcloud.ess.v20201111.models.Recipient`
+        :param TemplateType: 模板类型
+取值：
+1  静默签,
+3  普通模板
+        :type TemplateType: int
         :param Available: 模板可用状态，取值：1启用（默认），2停用
         :type Available: int
         :param OrganizationId: 模板创建组织id
         :type OrganizationId: str
         :param PreviewUrl: 模板预览链接
 注意：此字段可能返回 null，表示取不到有效值。
         :type PreviewUrl: str
@@ -5610,14 +5635,15 @@
         self.Recipients = None
         self.Components = None
         self.SignComponents = None
         self.Status = None
         self.Creator = None
         self.CreatedOn = None
         self.Promoter = None
+        self.TemplateType = None
         self.Available = None
         self.OrganizationId = None
         self.PreviewUrl = None
         self.TemplateVersion = None
         self.Published = None
 
 
@@ -5654,14 +5680,15 @@
                 self.SignComponents.append(obj)
         self.Status = params.get("Status")
         self.Creator = params.get("Creator")
         self.CreatedOn = params.get("CreatedOn")
         if params.get("Promoter") is not None:
             self.Promoter = Recipient()
             self.Promoter._deserialize(params.get("Promoter"))
+        self.TemplateType = params.get("TemplateType")
         self.Available = params.get("Available")
         self.OrganizationId = params.get("OrganizationId")
         self.PreviewUrl = params.get("PreviewUrl")
         self.TemplateVersion = params.get("TemplateVersion")
         self.Published = params.get("Published")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
```

### Comparing `tencentcloud-sdk-python-ess-3.0.902/tencentcloud_sdk_python_ess.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.903/tencentcloud_sdk_python_ess.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.902
+Version: 3.0.903
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.902/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.903/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.902
+Version: 3.0.903
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.902/setup.py` & `tencentcloud-sdk-python-ess-3.0.903/setup.py`

 * *Files identical despite different names*

