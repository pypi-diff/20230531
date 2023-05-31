# Comparing `tmp/bubble-aide-0.1.1.tar.gz` & `tmp/bubble-aide-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bubble-aide-0.1.1.tar", last modified: Mon May 29 01:45:26 2023, max compression
+gzip compressed data, was "bubble-aide-0.1.2.tar", last modified: Wed May 31 07:54:50 2023, max compression
```

## Comparing `bubble-aide-0.1.1.tar` & `bubble-aide-0.1.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 01:45:26.739841 bubble-aide-0.1.1/
--rw-rw-rw-   0        0        0     1083 2023-05-24 02:42:32.000000 bubble-aide-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      707 2023-05-29 01:45:26.739004 bubble-aide-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2419 2023-05-29 01:45:12.000000 bubble-aide-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-29 01:45:26.722418 bubble-aide-0.1.1/bubble_aide/
--rw-rw-rw-   0        0        0       66 2023-05-25 01:55:47.000000 bubble-aide-0.1.1/bubble_aide/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 01:45:26.734998 bubble-aide-0.1.1/bubble_aide/abc/
--rw-rw-rw-   0        0        0       55 2023-05-26 09:57:09.000000 bubble-aide-0.1.1/bubble_aide/abc/__init__.py
--rw-rw-rw-   0        0        0      191 2023-05-26 09:38:15.000000 bubble-aide-0.1.1/bubble_aide/abc/module.py
--rw-rw-rw-   0        0        0     4879 2023-05-26 09:35:12.000000 bubble-aide-0.1.1/bubble_aide/delegate.py
--rw-rw-rw-   0        0        0    10020 2023-05-26 09:35:12.000000 bubble-aide-0.1.1/bubble_aide/govern.py
--rw-rw-rw-   0        0        0    10036 2023-05-26 10:28:31.000000 bubble-aide-0.1.1/bubble_aide/main.py
--rw-rw-rw-   0        0        0      794 2023-05-26 09:35:12.000000 bubble-aide-0.1.1/bubble_aide/restricting.py
--rw-rw-rw-   0        0        0     1720 2023-05-26 09:35:12.000000 bubble-aide-0.1.1/bubble_aide/reward.py
--rw-rw-rw-   0        0        0     1112 2023-05-26 09:35:12.000000 bubble-aide-0.1.1/bubble_aide/slashing.py
--rw-rw-rw-   0        0        0     5769 2023-05-26 09:35:12.000000 bubble-aide-0.1.1/bubble_aide/staking.py
-drwxrwxrwx   0        0        0        0 2023-05-29 01:45:26.738006 bubble-aide-0.1.1/bubble_aide/statics/
--rw-rw-rw-   0        0        0        0 2023-05-26 06:36:53.000000 bubble-aide-0.1.1/bubble_aide/statics/__init__.py
--rw-rw-rw-   0        0        0    12509 2023-05-26 09:04:44.000000 bubble-aide-0.1.1/bubble_aide/statics/calculator.py
--rw-rw-rw-   0        0        0     3393 2023-05-26 09:37:06.000000 bubble-aide-0.1.1/bubble_aide/statics/contract.py
--rw-rw-rw-   0        0        0     5783 2023-05-25 09:07:03.000000 bubble-aide-0.1.1/bubble_aide/statics/economic.py
--rw-rw-rw-   0        0        0      312 2023-05-26 07:31:21.000000 bubble-aide-0.1.1/bubble_aide/statics/graphqls.py
--rw-rw-rw-   0        0        0      911 2023-05-26 09:05:19.000000 bubble-aide-0.1.1/bubble_aide/statics/node.py
-drwxrwxrwx   0        0        0        0 2023-05-29 01:45:26.739004 bubble-aide-0.1.1/bubble_aide/utils/
--rw-rw-rw-   0        0        0        0 2023-05-26 07:29:33.000000 bubble-aide-0.1.1/bubble_aide/utils/__init__.py
--rw-rw-rw-   0        0        0     3326 2023-05-26 10:03:16.000000 bubble-aide-0.1.1/bubble_aide/utils/utils.py
--rw-rw-rw-   0        0        0      986 2023-05-26 09:37:35.000000 bubble-aide-0.1.1/bubble_aide/utils/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-05-29 01:45:26.734998 bubble-aide-0.1.1/bubble_aide.egg-info/
--rw-rw-rw-   0        0        0      707 2023-05-29 01:45:26.000000 bubble-aide-0.1.1/bubble_aide.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      750 2023-05-29 01:45:26.000000 bubble-aide-0.1.1/bubble_aide.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 01:45:26.000000 bubble-aide-0.1.1/bubble_aide.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-29 01:43:56.000000 bubble-aide-0.1.1/bubble_aide.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      161 2023-05-29 01:45:26.000000 bubble-aide-0.1.1/bubble_aide.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-29 01:45:26.000000 bubble-aide-0.1.1/bubble_aide.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-29 01:45:26.739841 bubble-aide-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1591 2023-05-29 01:45:23.000000 bubble-aide-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 07:54:50.110802 bubble-aide-0.1.2/
+-rw-rw-rw-   0        0        0     1083 2023-05-24 02:42:32.000000 bubble-aide-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      707 2023-05-31 07:54:50.110802 bubble-aide-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2419 2023-05-29 01:45:12.000000 bubble-aide-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-31 07:54:50.101793 bubble-aide-0.1.2/bubble_aide/
+-rw-rw-rw-   0        0        0       66 2023-05-25 01:55:47.000000 bubble-aide-0.1.2/bubble_aide/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 07:54:50.110802 bubble-aide-0.1.2/bubble_aide/abc/
+-rw-rw-rw-   0        0        0       55 2023-05-26 09:57:09.000000 bubble-aide-0.1.2/bubble_aide/abc/__init__.py
+-rw-rw-rw-   0        0        0      191 2023-05-26 09:38:15.000000 bubble-aide-0.1.2/bubble_aide/abc/module.py
+-rw-rw-rw-   0        0        0     4891 2023-05-31 03:07:24.000000 bubble-aide-0.1.2/bubble_aide/delegate.py
+-rw-rw-rw-   0        0        0    10060 2023-05-31 03:07:23.000000 bubble-aide-0.1.2/bubble_aide/govern.py
+-rw-rw-rw-   0        0        0    10064 2023-05-31 03:08:14.000000 bubble-aide-0.1.2/bubble_aide/main.py
+-rw-rw-rw-   0        0        0      794 2023-05-26 09:35:12.000000 bubble-aide-0.1.2/bubble_aide/restricting.py
+-rw-rw-rw-   0        0        0     1720 2023-05-26 09:35:12.000000 bubble-aide-0.1.2/bubble_aide/reward.py
+-rw-rw-rw-   0        0        0     1116 2023-05-31 03:07:23.000000 bubble-aide-0.1.2/bubble_aide/slashing.py
+-rw-rw-rw-   0        0        0     5813 2023-05-31 03:07:23.000000 bubble-aide-0.1.2/bubble_aide/staking.py
+drwxrwxrwx   0        0        0        0 2023-05-31 07:54:50.110802 bubble-aide-0.1.2/bubble_aide/statics/
+-rw-rw-rw-   0        0        0        0 2023-05-26 06:36:53.000000 bubble-aide-0.1.2/bubble_aide/statics/__init__.py
+-rw-rw-rw-   0        0        0    12509 2023-05-26 09:04:44.000000 bubble-aide-0.1.2/bubble_aide/statics/calculator.py
+-rw-rw-rw-   0        0        0      915 2023-05-31 03:08:14.000000 bubble-aide-0.1.2/bubble_aide/statics/constant.py
+-rw-rw-rw-   0        0        0     3393 2023-05-26 09:37:06.000000 bubble-aide-0.1.2/bubble_aide/statics/contract.py
+-rw-rw-rw-   0        0        0     5783 2023-05-25 09:07:03.000000 bubble-aide-0.1.2/bubble_aide/statics/economic.py
+-rw-rw-rw-   0        0        0      312 2023-05-26 07:31:21.000000 bubble-aide-0.1.2/bubble_aide/statics/graphqls.py
+drwxrwxrwx   0        0        0        0 2023-05-31 07:54:50.110802 bubble-aide-0.1.2/bubble_aide/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-26 07:29:33.000000 bubble-aide-0.1.2/bubble_aide/utils/__init__.py
+-rw-rw-rw-   0        0        0     3453 2023-05-30 02:55:03.000000 bubble-aide-0.1.2/bubble_aide/utils/utils.py
+-rw-rw-rw-   0        0        0      986 2023-05-26 09:37:35.000000 bubble-aide-0.1.2/bubble_aide/utils/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-05-31 07:54:50.110802 bubble-aide-0.1.2/bubble_aide.egg-info/
+-rw-rw-rw-   0        0        0      707 2023-05-31 07:54:50.000000 bubble-aide-0.1.2/bubble_aide.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      754 2023-05-31 07:54:50.000000 bubble-aide-0.1.2/bubble_aide.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 07:54:50.000000 bubble-aide-0.1.2/bubble_aide.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-31 07:44:08.000000 bubble-aide-0.1.2/bubble_aide.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      161 2023-05-31 07:54:50.000000 bubble-aide-0.1.2/bubble_aide.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-31 07:54:50.000000 bubble-aide-0.1.2/bubble_aide.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-31 07:54:50.110802 bubble-aide-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1591 2023-05-31 07:53:08.000000 bubble-aide-0.1.2/setup.py
```

### Comparing `bubble-aide-0.1.1/LICENSE` & `bubble-aide-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bubble-aide-0.1.1/PKG-INFO` & `bubble-aide-0.1.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bubble-aide
-Version: 0.1.1
+Version: 0.1.2
 Summary: bubble aide
 Home-page: https://github.com/shinnng/bubble-aide
 Author: Shing
 Author-email: shinnng@outlook.com
 License: MIT
 Keywords: bubble-aide
 Classifier: Development Status :: 4 - Beta
```

### Comparing `bubble-aide-0.1.1/README.md` & `bubble-aide-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `bubble-aide-0.1.1/bubble_aide/delegate.py` & `bubble-aide-0.1.2/bubble_aide/delegate.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,30 +25,30 @@
                  node_id=None,
                  txn=None,
                  private_key=None,
                  ):
         """ 委托节点，以获取节点的奖励分红
         """
         amount = amount or self.aide.economic.delegate_limit
-        node_id = node_id or self.aide.node.node_id
+        node_id = node_id or self.aide.constant.node_id
         return self.aide.web3.dpos.delegate.delegate(node_id, balance_type, amount)
 
     @contract_transaction(1005)
     def withdrew_delegate(self,
                           amount=0,
                           staking_block_identifier=None,
                           node_id=None,
                           txn=None,
                           private_key=None,
                           ):
         """
         撤回对节点的委托，可以撤回部分委托
         注意：因为节点可能进行过多次质押/撤销质押，会使得委托信息遗留，因此撤回委托时必须指定节点质押区块
         """
-        node_id = node_id or self.aide.node.node_id
+        node_id = node_id or self.aide.constant.node_id
         amount = amount or self.aide.economic.delegate_limit
         staking_block_identifier = staking_block_identifier or self.aide.staking.staking_info.StakingBlockNum
 
         return self.aide.web3.dpos.delegate.withdrew_delegate(node_id,
                                                               staking_block_identifier,
                                                               amount,
                                                               )
@@ -69,15 +69,15 @@
                           staking_block_identifier=None,
                           ):
         """ 获取地址对某个节点的某次质押的委托信息
         注意：因为节点可能进行过多次质押/撤销质押，会使得委托信息遗留，因此获取委托信息时必须指定节点质押区块
         """
         if self.aide.account:
             address = address or self.aide.account.address
-        node_id = node_id or self.aide.node.node_id
+        node_id = node_id or self.aide.constant.node_id
         staking_block_identifier = staking_block_identifier or self.aide.staking.staking_info.staking_block_number
 
         delegate_info = self.aide.web3.dpos.delegate.get_delegate_info(address, node_id, staking_block_identifier).call()
         if delegate_info == 'Query delegate info failed:Delegate info is not found':
             return None
         else:
             return DelegateInfo(delegate_info)
```

### Comparing `bubble-aide-0.1.1/bubble_aide/govern.py` & `bubble-aide-0.1.2/bubble_aide/govern.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,15 +68,15 @@
                          node_id: Union[NodeID, HexStr] = None,
                          txn=None,
                          private_key=None,
                          ):
         """ 提交版本提案，实现链上共识硬分叉版本的升级
         """
         pip_number = pip_number or str(time())
-        node_id = node_id or self.aide.node.node_id
+        node_id = node_id or self.aide.constant.node_id
         return self.aide.web3.proposal.submit_version_proposal(node_id, pip_number, version, voting_rounds)
 
     @contract_transaction(default_txn={'gasPrice': paramGasPrice})
     def param_proposal(self,
                        module: str,
                        name: str,
                        value: str,
@@ -84,75 +84,75 @@
                        node_id: Union[NodeID, HexStr] = None,
                        txn=None,
                        private_key=None,
                        ):
         """ 提交参数提案，修改链上可治理参数
         """
         pip_number = pip_number or str(time())
-        node_id = node_id or self.aide.node.node_id
+        node_id = node_id or self.aide.constant.node_id
         return self.aide.web3.proposal.submit_param_proposal(node_id, pip_number, module, name, value)
 
     @contract_transaction(default_txn={'gasPrice': cancelGasPrice})
     def cancel_proposal(self,
                         proposal_id: str,
                         voting_rounds: int = 4,
                         node_id: Union[NodeID, HexStr] = None,
                         pip_number: str = None,
                         txn=None,
                         private_key=None,
                         ):
         """ 提交取消提案
         """
         pip_number = pip_number or str(time())
-        node_id = node_id or self.aide.node.node_id
+        node_id = node_id or self.aide.constant.node_id
         return self.aide.web3.proposal.submit_cancel_proposal(node_id, pip_number, voting_rounds, proposal_id)
 
     @contract_transaction(default_txn={'gasPrice': textGasPrice})
     def text_proposal(self,
                       pip_number: str = None,
                       node_id: Union[NodeID, HexStr] = None,
                       txn=None,
                       private_key=None,
                       ):
         """ 提交文本提案，文本提案不对链上产生影响，仅做pip投票意见收集作用
         """
         pip_number = pip_number or str(time())
-        node_id = node_id or self.aide.node.node_id
+        node_id = node_id or self.aide.constant.node_id
         return self.aide.web3.proposal.submit_text_proposal(node_id, pip_number)
 
     @contract_transaction()
     def vote(self,
              proposal_id: Union[bytes, HexStr],
              option: int,
              node_id: Union[NodeID, HexStr] = None,
              version: int = None,
              version_sign: Union[bytes, HexStr] = None,
              txn=None,
              private_key=None,
              ):
         """ 对提案进行投票
         """
-        node_id = node_id or self.aide.node.node_id
-        version = version or self.aide.node.node_version
-        version_sign = version_sign or self.aide.node.version_sign
+        node_id = node_id or self.aide.constant.node_id
+        version = version or self.aide.constant.node_version
+        version_sign = version_sign or self.aide.constant.version_sign
         return self.aide.web3.proposal.vote(node_id, proposal_id, option, version, version_sign)
 
     @contract_transaction()
     def declare_version(self,
                         node_id: Union[NodeID, HexStr] = None,
                         version: int = None,
                         version_sign: Union[bytes, HexStr] = None,
                         txn=None,
                         private_key=None,
                         ):
         """ 向链上声明节点版本，以获得参与共识出块的资格
         """
-        node_id = node_id or self.aide.node.node_id
-        version = version or self.aide.node.node_version
-        version_sign = version_sign or self.aide.node.version_sign
+        node_id = node_id or self.aide.constant.node_id
+        version = version or self.aide.constant.node_version
+        version_sign = version_sign or self.aide.constant.version_sign
         return self.aide.web3.proposal.declare_version(node_id, version, version_sign)
 
     def get_proposal(self, proposal_id: Union[bytes, HexStr]):
         """ 获取提案信息
         """
         proposal = self.aide.web3.proposal.get_proposal(proposal_id).call()
         return to_attribute_proposal(proposal)
```

### Comparing `bubble-aide-0.1.1/bubble_aide/main.py` & `bubble-aide-0.1.2/bubble_aide/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from bubble_aide.statics.contract import Contract
 from bubble_aide.staking import Staking
 from bubble_aide.delegate import Delegate
 from bubble_aide.slashing import Slashing
 from bubble_aide.reward import Reward
 from bubble_aide.govern import Govern
 from bubble_aide.statics.graphqls import Graphql
-from bubble_aide.statics.node import Node
+from bubble_aide.statics.constant import Constant
 from bubble_aide.utils.utils import get_web3, get_economic, precompile_contracts
 from eth_account._utils.signing import to_standard_signature_bytes
 from eth_hash.auto import keccak
 from eth_keys.datatypes import Signature
 from eth_typing import HexStr
 from eth_utils import remove_0x_prefix, to_canonical_address
 
@@ -51,24 +51,24 @@
         self.__init_modules__()
 
     def __init_web3__(self):
         """ 设置web相关模块
         """
         self.web3 = get_web3(self.uri)
         self.bub = self.web3.bub
-        self.txpool = self.web3.node.txpool
-        self.personal = self.web3.node.personal
-        self.admin = self.web3.node.admin
+        self.txpool = self.web3.constant.txpool
+        self.personal = self.web3.constant.personal
+        self.admin = self.web3.constant.admin
         self.debug = self.web3.debug
 
     def __init_modules__(self):
         """ 设置bubble内置合约相关模块
         """
         self.economic = get_economic(self)
-        self.node = Node(self)
+        self.constant = Constant(self)
         self.graphql = Graphql(f'{self.uri}/bubble/graphql')
         self.calculator = Calculator(self)
         self.restricting = Restricting(self)
         self.staking = Staking(self)
         self.delegate = Delegate(self)
         self.slashing = Slashing(self)
         self.reward = Reward(self)
```

### Comparing `bubble-aide-0.1.1/bubble_aide/restricting.py` & `bubble-aide-0.1.2/bubble_aide/restricting.py`

 * *Files identical despite different names*

### Comparing `bubble-aide-0.1.1/bubble_aide/reward.py` & `bubble-aide-0.1.2/bubble_aide/reward.py`

 * *Files identical despite different names*

### Comparing `bubble-aide-0.1.1/bubble_aide/slashing.py` & `bubble-aide-0.1.2/bubble_aide/slashing.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,9 +23,9 @@
         return self.aide.web3.dpos.slashing.report_duplicate_sign(report_type, data)
 
     def check_duplicate_sign(self,
                              report_type,
                              block_identifier,
                              node_id=None,
                              ):
-        node_id = node_id or self.aide.node.node_id
+        node_id = node_id or self.aide.constant.node_id
         return self.aide.web3.dpos.slashing.check_duplicate_sign(report_type, node_id, block_identifier).call()
```

### Comparing `bubble-aide-0.1.1/bubble_aide/staking.py` & `bubble-aide-0.1.2/bubble_aide/staking.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 
     def __init__(self, aide: "Aide"):
         super().__init__(aide)
         self.address = self.aide.web3.dpos.staking.ADDRESS
 
     @property
     def staking_info(self):
-        candidate_info = self.get_candidate_info(self.aide.node.node_id)
+        candidate_info = self.get_candidate_info(self.aide.constant.node_id)
         if candidate_info:
             return candidate_info
-        raise AttributeError('the node has no staking information.')
+        raise AttributeError('the constant has no staking information.')
 
     @contract_transaction()
     def create_staking(self,
                        amount=None,
                        balance_type=0,
                        node_id=None,
                        benefit_address=None,
@@ -43,55 +43,55 @@
         if not benefit_address:
             benefit_account = self.aide.bub.account.from_key(private_key) if private_key else self.aide.account
             if not benefit_account:
                 raise ValueError('the benefit address cannot be empty')
 
             benefit_address = benefit_account.address
 
-        node_id = node_id or self.aide.node.node_id
+        node_id = node_id or self.aide.constant.node_id
         amount = amount or self.aide.economic.staking_limit
-        version = version or self.aide.node.node_version
-        version_sign = version_sign or self.aide.node.version_sign
-        bls_pubkey = bls_pubkey or self.aide.node.bls_pubkey
-        bls_proof = bls_proof or self.aide.node.bls_proof
+        version = version or self.aide.constant.node_version
+        version_sign = version_sign or self.aide.constant.version_sign
+        bls_pubkey = bls_pubkey or self.aide.constant.bls_pubkey
+        bls_proof = bls_proof or self.aide.constant.bls_proof
         return self.aide.web3.dpos.staking.create_staking(balance_type, benefit_address, node_id, external_id,
                                                           node_name, website, details, amount, reward_per,
                                                           version, version_sign, bls_pubkey, bls_proof
                                                           )
 
     @contract_transaction()
     def increase_staking(self,
                          balance_type=0,
                          node_id=None,
                          amount=None,
                          txn=None,
                          private_key=None,
                          ):
-        node_id = node_id or self.aide.node.node_id
+        node_id = node_id or self.aide.constant.node_id
         amount = amount or self.aide.economic.add_staking_limit
         return self.aide.web3.dpos.staking.increase_staking(node_id, balance_type, amount)
 
     @contract_transaction()
     def withdrew_staking(self, node_id=None, txn=None, private_key=None):
-        node_id = node_id or self.aide.node.node_id
+        node_id = node_id or self.aide.constant.node_id
         return self.aide.web3.dpos.staking.withdrew_staking(node_id)
 
     @contract_transaction()
     def edit_candidate(self,
                        benifit_address=None,
                        node_id=None,
                        reward_per=None,
                        external_id=None,
                        node_name=None,
                        website=None,
                        details=None,
                        txn=None,
                        private_key=None,
                        ):
-        node_id = node_id or self.aide.node.node_id
+        node_id = node_id or self.aide.constant.node_id
         return self.aide.web3.dpos.staking.edit_staking(node_id, benifit_address, reward_per, external_id,
                                                         node_name, website, details
                                                         )
 
     def get_verifier_list(self):
         verifier_list = self.aide.web3.dpos.staking.get_verifier_list().call()
         return [StakingInfo(verifier) for verifier in verifier_list]
@@ -101,15 +101,15 @@
         return [StakingInfo(validator) for validator in validator_list]
 
     def get_candidate_list(self):
         candidate_list = self.aide.web3.dpos.staking.get_candidate_list().call()
         return [StakingInfo(candidate) for candidate in candidate_list]
 
     def get_candidate_info(self, node_id=None):
-        node_id = node_id or self.aide.node.node_id
+        node_id = node_id or self.aide.constant.node_id
         staking_info = self.aide.web3.dpos.staking.get_candidate_info(node_id).call()
         if staking_info == 'Query candidate info failed:Candidate info is not found':
             return None
         else:
             return StakingInfo(staking_info)
 
     def get_block_reward(self):
```

### Comparing `bubble-aide-0.1.1/bubble_aide/statics/calculator.py` & `bubble-aide-0.1.2/bubble_aide/statics/calculator.py`

 * *Files identical despite different names*

### Comparing `bubble-aide-0.1.1/bubble_aide/statics/contract.py` & `bubble-aide-0.1.2/bubble_aide/statics/contract.py`

 * *Files identical despite different names*

### Comparing `bubble-aide-0.1.1/bubble_aide/statics/economic.py` & `bubble-aide-0.1.2/bubble_aide/statics/economic.py`

 * *Files identical despite different names*

### Comparing `bubble-aide-0.1.1/bubble_aide/statics/node.py` & `bubble-aide-0.1.2/bubble_aide/statics/constant.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from bubble_aide import Aide
 
 
-class Node:
+class Constant:
 
     def __init__(self, aide: "Aide"):
         self.aide = aide
 
     @property
     def node_id(self):
         node_info = self.aide.admin.node_info()
```

### Comparing `bubble-aide-0.1.1/bubble_aide/utils/utils.py` & `bubble-aide-0.1.2/bubble_aide/utils/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from os.path import abspath
 from typing import cast
 
 from bubble import Web3, HTTPProvider, WebsocketProvider, IPCProvider
 from bubble._utils.threads import Timeout
 from bubble.datastructures import AttributeDict
 from bubble.exceptions import ContractLogicError
+from bubble.middleware import node_poa_middleware
 from bubble.types import RLPEventData
 
 from gql import Client
 from gql.transport.aiohttp import AIOHTTPTransport
 from gql.transport.websockets import WebsocketsTransport
 
 from bubble_aide.statics.economic import new_economic
@@ -40,14 +41,15 @@
     else:
         raise ValueError(f'unidentifiable uri {uri}')
 
     with Timeout(timeout) as t:
         while True:
             web3 = Web3(provider(uri), modules=modules)
             if web3.is_connected():
+                web3.middleware_onion.inject(node_poa_middleware, layer=0)
                 break
             t.sleep(1)
 
     return web3
 
 
 def get_economic(aide):
```

### Comparing `bubble-aide-0.1.1/bubble_aide/utils/wrapper.py` & `bubble-aide-0.1.2/bubble_aide/utils/wrapper.py`

 * *Files identical despite different names*

### Comparing `bubble-aide-0.1.1/bubble_aide.egg-info/PKG-INFO` & `bubble-aide-0.1.2/bubble_aide.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bubble-aide
-Version: 0.1.1
+Version: 0.1.2
 Summary: bubble aide
 Home-page: https://github.com/shinnng/bubble-aide
 Author: Shing
 Author-email: shinnng@outlook.com
 License: MIT
 Keywords: bubble-aide
 Classifier: Development Status :: 4 - Beta
```

### Comparing `bubble-aide-0.1.1/bubble_aide.egg-info/SOURCES.txt` & `bubble-aide-0.1.2/bubble_aide.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,14 @@
 bubble_aide.egg-info/not-zip-safe
 bubble_aide.egg-info/requires.txt
 bubble_aide.egg-info/top_level.txt
 bubble_aide/abc/__init__.py
 bubble_aide/abc/module.py
 bubble_aide/statics/__init__.py
 bubble_aide/statics/calculator.py
+bubble_aide/statics/constant.py
 bubble_aide/statics/contract.py
 bubble_aide/statics/economic.py
 bubble_aide/statics/graphqls.py
-bubble_aide/statics/node.py
 bubble_aide/utils/__init__.py
 bubble_aide/utils/utils.py
 bubble_aide/utils/wrapper.py
```

### Comparing `bubble-aide-0.1.1/setup.py` & `bubble-aide-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 with open('./README.md', encoding='utf-8') as readme:
     long_description = readme.read()
 
 setup(
     name='bubble-aide',
     # *IMPORTANT*: Don't manually change the version here. Use the 'bumpversion' utility.
-    version='0.1.1',
+    version='0.1.2',
     description="""bubble aide""",
     # long_description=long_description,
     # long_description_content_type='text/markdown',
     author='Shing',
     author_email='shinnng@outlook.com',
     url='https://github.com/shinnng/bubble-aide',
     include_package_data=True,
```

