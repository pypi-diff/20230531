# Comparing `tmp/chainbench-0.2.0.tar.gz` & `tmp/chainbench-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chainbench-0.2.0.tar", max compression
+gzip compressed data, was "chainbench-0.3.0.tar", max compression
```

## Comparing `chainbench-0.2.0.tar` & `chainbench-0.3.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0    11357 2023-05-11 11:14:19.492029 chainbench-0.2.0/LICENSE
--rw-r--r--   0        0        0     7622 2023-05-11 11:14:19.496029 chainbench-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-05-11 11:14:19.496029 chainbench-0.2.0/chainbench/__init__.py
--rw-r--r--   0        0        0       39 2023-05-11 11:14:19.496029 chainbench-0.2.0/chainbench/__main__.py
--rw-r--r--   0        0        0     5735 2023-05-11 11:14:19.496029 chainbench-0.2.0/chainbench/main.py
--rw-r--r--   0        0        0        0 2023-05-11 11:14:19.496029 chainbench-0.2.0/chainbench/profile/__init__.py
--rw-r--r--   0        0        0     3417 2023-05-11 11:14:19.496029 chainbench-0.2.0/chainbench/profile/avalanche.py
--rw-r--r--   0        0        0     2512 2023-05-11 11:14:19.496029 chainbench-0.2.0/chainbench/profile/bsc.py
--rw-r--r--   0        0        0     2734 2023-05-11 11:14:19.496029 chainbench-0.2.0/chainbench/profile/ethereum.py
--rw-r--r--   0        0        0      723 2023-05-11 11:14:19.496029 chainbench-0.2.0/chainbench/profile/evm/heavy.py
--rw-r--r--   0        0        0     1592 2023-05-11 11:14:19.496029 chainbench-0.2.0/chainbench/profile/evm/light.py
--rw-r--r--   0        0        0     1829 2023-05-11 11:14:19.496029 chainbench-0.2.0/chainbench/profile/oasis.py
--rw-r--r--   0        0        0     2670 2023-05-11 11:14:19.496029 chainbench-0.2.0/chainbench/profile/polygon.py
--rw-r--r--   0        0        0      168 2023-05-11 11:14:19.496029 chainbench-0.2.0/chainbench/test_data/__init__.py
--rw-r--r--   0        0        0     4705 2023-05-11 11:14:19.496029 chainbench-0.2.0/chainbench/test_data/base.py
--rw-r--r--   0        0        0      166 2023-05-11 11:14:19.496029 chainbench-0.2.0/chainbench/test_data/dummy.py
--rw-r--r--   0        0        0     2596 2023-05-11 11:14:19.496029 chainbench-0.2.0/chainbench/test_data/evm.py
--rw-r--r--   0        0        0        0 2023-05-11 11:14:19.496029 chainbench-0.2.0/chainbench/user/__init__.py
--rw-r--r--   0        0        0     3410 2023-05-11 11:14:19.496029 chainbench-0.2.0/chainbench/user/base.py
--rw-r--r--   0        0        0     1225 2023-05-11 11:14:19.496029 chainbench-0.2.0/chainbench/user/evm.py
--rw-r--r--   0        0        0        0 2023-05-11 11:14:19.496029 chainbench-0.2.0/chainbench/util/__init__.py
--rw-r--r--   0        0        0     3015 2023-05-11 11:14:19.496029 chainbench-0.2.0/chainbench/util/cli.py
--rw-r--r--   0        0        0     2512 2023-05-11 11:14:19.496029 chainbench-0.2.0/chainbench/util/event.py
--rw-r--r--   0        0        0     3463 2023-05-11 11:14:19.496029 chainbench-0.2.0/chainbench/util/notify.py
--rw-r--r--   0        0        0      320 2023-05-11 11:14:19.496029 chainbench-0.2.0/chainbench/util/rpc.py
--rw-r--r--   0        0        0      438 2023-05-11 11:14:19.496029 chainbench-0.2.0/chainbench/util/timer.py
--rw-r--r--   0        0        0      746 2023-05-11 11:14:19.496029 chainbench-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     8088 1970-01-01 00:00:00.000000 chainbench-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-31 16:05:21.018361 chainbench-0.3.0/LICENSE
+-rw-r--r--   0        0        0     7715 2023-05-31 16:05:21.018361 chainbench-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 16:05:21.018361 chainbench-0.3.0/chainbench/__init__.py
+-rw-r--r--   0        0        0       39 2023-05-31 16:05:21.018361 chainbench-0.3.0/chainbench/__main__.py
+-rw-r--r--   0        0        0     7638 2023-05-31 16:05:21.018361 chainbench-0.3.0/chainbench/main.py
+-rw-r--r--   0        0        0        0 2023-05-31 16:05:21.018361 chainbench-0.3.0/chainbench/profile/__init__.py
+-rw-r--r--   0        0        0     3597 2023-05-31 16:05:21.018361 chainbench-0.3.0/chainbench/profile/avalanche/general.py
+-rw-r--r--   0        0        0     2693 2023-05-31 16:05:21.018361 chainbench-0.3.0/chainbench/profile/bsc/general.py
+-rw-r--r--   0        0        0     2912 2023-05-31 16:05:21.018361 chainbench-0.3.0/chainbench/profile/ethereum/general.py
+-rw-r--r--   0        0        0      361 2023-05-31 16:05:21.018361 chainbench-0.3.0/chainbench/profile/evm/get_logs.py
+-rw-r--r--   0        0        0      803 2023-05-31 16:05:21.018361 chainbench-0.3.0/chainbench/profile/evm/heavy.py
+-rw-r--r--   0        0        0     1645 2023-05-31 16:05:21.018361 chainbench-0.3.0/chainbench/profile/evm/light.py
+-rw-r--r--   0        0        0     1838 2023-05-31 16:05:21.018361 chainbench-0.3.0/chainbench/profile/oasis/general.py
+-rw-r--r--   0        0        0     2845 2023-05-31 16:05:21.018361 chainbench-0.3.0/chainbench/profile/polygon/general.py
+-rw-r--r--   0        0        0      168 2023-05-31 16:05:21.018361 chainbench-0.3.0/chainbench/test_data/__init__.py
+-rw-r--r--   0        0        0     4705 2023-05-31 16:05:21.018361 chainbench-0.3.0/chainbench/test_data/base.py
+-rw-r--r--   0        0        0      166 2023-05-31 16:05:21.018361 chainbench-0.3.0/chainbench/test_data/dummy.py
+-rw-r--r--   0        0        0     2979 2023-05-31 16:05:21.018361 chainbench-0.3.0/chainbench/test_data/evm.py
+-rw-r--r--   0        0        0        0 2023-05-31 16:05:21.018361 chainbench-0.3.0/chainbench/user/__init__.py
+-rw-r--r--   0        0        0     3511 2023-05-31 16:05:21.018361 chainbench-0.3.0/chainbench/user/base.py
+-rw-r--r--   0        0        0     1225 2023-05-31 16:05:21.018361 chainbench-0.3.0/chainbench/user/evm.py
+-rw-r--r--   0        0        0        0 2023-05-31 16:05:21.018361 chainbench-0.3.0/chainbench/util/__init__.py
+-rw-r--r--   0        0        0     3840 2023-05-31 16:05:21.018361 chainbench-0.3.0/chainbench/util/cli.py
+-rw-r--r--   0        0        0     2512 2023-05-31 16:05:21.018361 chainbench-0.3.0/chainbench/util/event.py
+-rw-r--r--   0        0        0     3463 2023-05-31 16:05:21.018361 chainbench-0.3.0/chainbench/util/notify.py
+-rw-r--r--   0        0        0      320 2023-05-31 16:05:21.018361 chainbench-0.3.0/chainbench/util/rpc.py
+-rw-r--r--   0        0        0      438 2023-05-31 16:05:21.018361 chainbench-0.3.0/chainbench/util/timer.py
+-rw-r--r--   0        0        0      772 2023-05-31 16:05:21.022361 chainbench-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     8228 1970-01-01 00:00:00.000000 chainbench-0.3.0/PKG-INFO
```

### Comparing `chainbench-0.2.0/LICENSE` & `chainbench-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chainbench-0.2.0/README.md` & `chainbench-0.3.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -90,31 +90,31 @@
 chainbench start --profile bsc --users 50 --workers 2 --test-time 12h --target https://node-url --headless --autoquit
 ```
 
 This will run a load test for BSC with 2 workers, 50 users and 12 hours test time in headless mode.
 After the test is finished, the tool will automatically quit.
 
 ### Parameters and Flags
-- `--profile`: This flag specifies the profile to use for the benchmark. Available profiles are `ethereum`, `bsc`, `polygon`, `oasis`, and `avalanche`.
-- `--users`: This flag sets the number of simulated users to use for the benchmark.
-- `--workers`: This flag sets the number of worker threads to use for the benchmark.
-- `--test-time`: This flag sets the duration of the test to run.
-- `--target`: This flag specifies the target blockchain node URL that the benchmark will connect to.
-- `--headless`: This flag runs the benchmark in headless mode, meaning that no graphical user interface (GUI) will be displayed during the test. This is useful for running the test on a remote server or when the GUI is not needed.
-- `--autoquit`: This flag tells the Chainbench tool to automatically quit after the test has finished. This is useful for running the benchmark in an automated environment where manual intervention is not desired.
-- `--help`: This flag displays the help message.
-
-By default, Chainbench uses `constant_pacing` wait time with a value of 10 seconds. 
-This means a load test with 100 users will have a theoretical maximum of 10 rps. This allows us to have a target rps in a test, 
-and the result rps lower than the target rps means performance deterioration.
+- `-p, --profile`: Specifies the profile to use for the benchmark. Available profiles can be found in the profile directory. Sample usage `-p bsc.general`
+- `-u, --users`: Sets the number of simulated users to use for the benchmark.
+- `-w, --workers`: Sets the number of worker threads to use for the benchmark.
+- `-t, --test-time`: Sets the duration of the test to run.
+- `--target`: Specifies the target blockchain node URL that the benchmark will connect to.
+- `--headless`: Runs the benchmark in headless mode, meaning that no graphical user interface (GUI) will be displayed during the test. This is useful for running the test on a remote server or when the GUI is not needed.
+- `--autoquit`: Tells the Chainbench tool to automatically quit after the test has finished. This is useful for running the benchmark in an automated environment where manual intervention is not desired.
+- `--help`: Displays the help message.
+- `--debug-trace-methods`: Enables tasks tagged with debug or trace to be executed
+- `-E, --exclude-tags`: Exclude tasks tagged with custom tags from the test. You may specify this option multiple times --help Show this message and exit.
+
+You may also run `chainbench start --help` for the full list of parameters and flags.
 
 ### Profiles
 Default profiles are located in the [`profile`](chainbench/profile) directory. For a tutorial on how to create custom profiles, please refer to [this document](docs/PROFILE.md).
 
-You can also use the `--profile-dir` flag to specify a custom directory with profiles. For example:
+You can also use the `-d` or `--profile-dir` flag to specify a custom directory with profiles. For example:
 ```shell
 chainbench start --profile-dir /path/to/profiles --profile my-profile --users 50 --workers 2 --test-time 12h --target https://node-url --headless --autoquit
 ```
 This will run a load test using `/path/to/profiles/my-profile.py` profile.
 
 It's possible to group profiles into directories. For example, you can create a directory called `bsc` and put all the BSC profiles there. Then you can run a load test using the following command:
 ```shell
@@ -129,18 +129,18 @@
 ```shell
 chainbench start --profile evm.light --users 50 --workers 2 --test-time 12h --target https://node-url --headless --autoquit
 ```
 
 ### Web UI Mode
 
 Run the following command to run a load test for BSC in UI mode. It will start a web server on port 8089. 
-Target is not required as you can specify it in the UI along with the number of users, spawn rate and test time.
+Target is required to initialize the test data, however you may change the target endpoint later in the UI, along with the number of users, spawn rate and test time.
 
 ```shell
-chainbench start --profile bsc --workers 1
+chainbench start --profile bsc.general --workers 1 --target https://any-working-node-endpoint.com
 ```
 
 ### Headless Mode
 
 If you want to run a load test for BSC in headless mode, run the following command:
 
 ```shell
```

### Comparing `chainbench-0.2.0/chainbench/profile/avalanche.py` & `chainbench-0.3.0/chainbench/profile/avalanche/general.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,20 +11,23 @@
     "eth_getTransactionReceipt" : 17
     "eth_chainId" : 15
     "eth_blockNumber" : 15
     "eth_getBalance" : 11
     "Others" : 28
 ```
 """
-from locust import task
+from locust import constant_pacing, tag, task
 
 from chainbench.user.evm import EVMBenchUser
 
 
 class AvalancheProfile(EVMBenchUser):
+    wait_time = constant_pacing(2)
+    weight = 91
+
     @task(100)
     def call_task(self):
         self.make_call(
             name="call",
             method="eth_call",
             params=[
                 {
@@ -39,22 +42,14 @@
     def get_block_by_number_task(self):
         self.make_call(
             name="get_block_by_number",
             method="eth_getBlockByNumber",
             params=self._block_by_number_params_factory(),
         ),
 
-    @task(24)
-    def get_logs_task(self):
-        self.make_call(
-            name="get_logs",
-            method="eth_getLogs",
-            params=self._get_logs_params_factory(),
-        ),
-
     @task(17)
     def get_transaction_receipt_task(self):
         self.make_call(
             name="get_transaction_receipt",
             method="eth_getTransactionReceipt",
             params=self._transaction_by_hash_params_factory(),
         ),
@@ -127,7 +122,21 @@
 
     @task(3)
     def max_priority_fee_per_gas_task(self):
         self.make_call(
             name="max_priority_fee_per_gas",
             method="eth_maxPriorityFeePerGas",
         ),
+
+
+class GetLogsProfile(EVMBenchUser):
+    wait_time = constant_pacing(10)
+    weight = 9
+
+    @tag("get-logs")
+    @task
+    def get_logs_task(self):
+        self.make_call(
+            name="get_logs",
+            method="eth_getLogs",
+            params=self._get_logs_params_factory(),
+        ),
```

### Comparing `chainbench-0.2.0/chainbench/profile/bsc.py` & `chainbench-0.3.0/chainbench/profile/ethereum/general.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,99 +1,118 @@
 """
-Bsc profile.
+Ethereum profile.
 
 Chart:
 ```mermaid
 %%{init: {'theme':'forest'}}%%
 pie title Methods Distribution
     "eth_call" : 100
-    "eth_getTransactionReceipt" : 93
-    "eth_getLogs" : 36
-    "eth_blockNumber" : 28
-    "eth_chainId" : 18
-    "eth_getBlockByNumber" : 13
-    "Others" : 20
+    "eth_getTransactionReceipt" : 24
+    "eth_blockNumber" : 19
+    "eth_getBalance" : 12
+    "eth_chainId" : 11
+    "eth_getBlockByNumber" : 9
+    "eth_getTransactionByHash" : 8
+    "Others" : 12
 ```
 """
-from locust import task
+from locust import constant_pacing, tag, task
 
 from chainbench.user.evm import EVMBenchUser
 
 
-class BscProfile(EVMBenchUser):
+class EthereumProfile(EVMBenchUser):
+    wait_time = constant_pacing(2)
+    weight = 487
+
     @task(100)
     def call_task(self):
         self.make_call(
             name="call",
             method="eth_call",
             params=[
                 {
-                    "to": "0x55d398326f99059fF775485246999027B3197955",
-                    "data": "0x70a08231000000000000000000000000f977814e90da44bfa03b6295a0616a897441acec",  # noqa: E501
+                    "to": "0xdAC17F958D2ee523a2206206994597C13D831ec7",
+                    "data": "0x70a082310000000000000000000000009696f59E4d72E237BE84fFD425DCaD154Bf96976",  # noqa: E501
                 },
                 "latest",
             ],
         ),
 
-    @task(93)
+    @task(24)
     def get_transaction_receipt_task(self):
         self.make_call(
             name="get_transaction_receipt",
             method="eth_getTransactionReceipt",
             params=self._transaction_by_hash_params_factory(),
         ),
 
-    @task(36)
-    def get_logs_task(self):
-        self.make_call(
-            name="get_logs",
-            method="eth_getLogs",
-            params=self._get_logs_params_factory(),
-        ),
-
-    @task(28)
+    @task(19)
     def block_number_task(self):
         self.make_call(
             name="block_number",
             method="eth_blockNumber",
             params=[],
         ),
 
-    @task(18)
+    @task(12)
+    def get_balance_task(self):
+        self.make_call(
+            name="get_balance",
+            method="eth_getBalance",
+            params=self._get_balance_params_factory_latest(),
+        ),
+
+    @task(11)
     def chain_id_task(self):
         self.make_call(
             name="chain_id",
             method="eth_chainId",
             params=[],
         ),
 
-    @task(13)
+    @task(9)
     def get_block_by_number_task(self):
         self.make_call(
             name="get_block_by_number",
             method="eth_getBlockByNumber",
             params=self._block_by_number_params_factory(),
         ),
 
-    @task(9)
+    @task(8)
     def get_transaction_by_hash_task(self):
         self.make_call(
             name="get_transaction_by_hash",
             method="eth_getTransactionByHash",
             params=self._transaction_by_hash_params_factory(),
         ),
 
-    @task(5)
-    def get_balance_task(self):
+    @tag("debug")
+    @task(3)
+    def trace_transaction_task(self):
         self.make_call(
-            name="get_balance",
-            method="eth_getBalance",
-            params=self._get_balance_params_factory_latest(),
+            name="trace_transaction",
+            method="debug_traceTransaction",
+            params=[],
         ),
 
-    @task(3)
-    def get_block_by_hash_task(self):
+    @task(2)
+    def client_version_task(self):
         self.make_call(
-            name="get_block_by_hash",
-            method="eth_getBlockByHash",
-            params=self._block_by_hash_params_factory(),
+            name="client_version",
+            method="web3_clientVersion",
+            params=[],
+        ),
+
+
+class GetLogsProfile(EVMBenchUser):
+    wait_time = constant_pacing(10)
+    weight = 13
+
+    @tag("get-logs")
+    @task
+    def get_logs_task(self):
+        self.make_call(
+            name="get_logs",
+            method="eth_getLogs",
+            params=self._get_logs_params_factory(),
         ),
```

### Comparing `chainbench-0.2.0/chainbench/profile/ethereum.py` & `chainbench-0.3.0/chainbench/profile/polygon/general.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,109 +1,113 @@
 """
-Ethereum profile.
+Polygon profile.
+
+Note, that eth_sendRawTransaction is excluded from the test because it requires
+building a transaction and signing it.
 
 Chart:
 ```mermaid
 %%{init: {'theme':'forest'}}%%
 pie title Methods Distribution
     "eth_call" : 100
-    "eth_getTransactionReceipt" : 24
-    "eth_blockNumber" : 19
-    "eth_getBalance" : 12
-    "eth_chainId" : 11
-    "eth_getBlockByNumber" : 9
-    "eth_getTransactionByHash" : 8
-    "Others" : 12
+    "eth_getTransactionReceipt" : 64
+    "eth_chainId" : 20
+    "eth_getBlockByNumber" : 17
+    "eth_blockNumber" : 16
+    "eth_getTransactionByHash" : 11
+    "eth_getLogs" : 11
+    "Others" : 9
 ```
 """
-from locust import tag, task
+from locust import constant_pacing, tag, task
 
 from chainbench.user.evm import EVMBenchUser
 
 
-class EthereumProfile(EVMBenchUser):
+class PolygonGeneral(EVMBenchUser):
+    wait_time = constant_pacing(2)
+    weight = 19
+
     @task(100)
     def call_task(self):
         self.make_call(
             name="call",
             method="eth_call",
             params=[
                 {
-                    "to": "0xdAC17F958D2ee523a2206206994597C13D831ec7",
-                    "data": "0x70a082310000000000000000000000009696f59E4d72E237BE84fFD425DCaD154Bf96976",  # noqa: E501
+                    "to": "0xc2132D05D31c914a87C6611C10748AEb04B58e8F",
+                    "data": "0x70a08231000000000000000000000000F977814e90dA44bFA03b6295A0616a897441aceC",  # noqa: E501
                 },
                 "latest",
             ],
         ),
 
-    @task(24)
+    @task(64)
     def get_transaction_receipt_task(self):
         self.make_call(
             name="get_transaction_receipt",
             method="eth_getTransactionReceipt",
             params=self._transaction_by_hash_params_factory(),
         ),
 
-    @task(19)
-    def block_number_task(self):
-        self.make_call(
-            name="block_number",
-            method="eth_blockNumber",
-            params=[],
-        ),
-
-    @task(12)
-    def get_balance_task(self):
-        self.make_call(
-            name="get_balance",
-            method="eth_getBalance",
-            params=self._get_balance_params_factory_latest(),
-        ),
-
-    @task(11)
+    @task(20)
     def chain_id_task(self):
         self.make_call(
             name="chain_id",
             method="eth_chainId",
             params=[],
         ),
 
-    @task(9)
+    @task(17)
     def get_block_by_number_task(self):
         self.make_call(
             name="get_block_by_number",
             method="eth_getBlockByNumber",
             params=self._block_by_number_params_factory(),
         ),
 
-    @task(8)
+    @task(16)
+    def block_number_task(self):
+        self.make_call(
+            name="block_number",
+            method="eth_blockNumber",
+            params=[],
+        ),
+
+    @task(11)
     def get_transaction_by_hash_task(self):
         self.make_call(
             name="get_transaction_by_hash",
             method="eth_getTransactionByHash",
             params=self._transaction_by_hash_params_factory(),
         ),
 
-    @task(5)
-    def get_logs_task(self):
+    @task(4)
+    def get_balance_task(self):
         self.make_call(
-            name="get_logs",
-            method="eth_getLogs",
-            params=self._get_logs_params_factory(),
+            name="get_balance",
+            method="eth_getBalance",
+            params=self._get_balance_params_factory_latest(),
         ),
 
-    @tag("debug")
-    @task(3)
-    def trace_transaction_task(self):
+    @tag("trace")
+    @task(2)
+    def block_task(self):
         self.make_call(
-            name="trace_transaction",
-            method="debug_traceTransaction",
-            params=[],
+            name="block",
+            method="trace_block",
+            params=self._block_by_number_params_factory(),
         ),
 
-    @task(2)
-    def client_version_task(self):
+
+class GetLogsProfile(EVMBenchUser):
+    wait_time = constant_pacing(10)
+    weight = 1
+
+    @tag("get-logs")
+    @task
+    def get_logs_task(self):
         self.make_call(
-            name="client_version",
-            method="web3_clientVersion",
-            params=[],
+            name="get_logs",
+            method="eth_getLogs",
+            params=self._get_logs_params_factory(),
         ),
```

### Comparing `chainbench-0.2.0/chainbench/profile/evm/heavy.py` & `chainbench-0.3.0/chainbench/profile/evm/heavy.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """
 Ethereum profile (heavy mode).
 """
-from locust import task
+from locust import constant_pacing, tag, task
 
 from chainbench.user.evm import EVMBenchUser
 
 
 class EthereumHeavyProfile(EVMBenchUser):
+    wait_time = constant_pacing(10)
+
     @task
     def trace_transaction_task(self):
         self.make_call(
             name="trace_transaction",
             method="debug_traceTransaction",
             params=[],
         ),
@@ -19,14 +21,15 @@
     def block_task(self):
         self.make_call(
             name="block",
             method="trace_block",
             params=self._block_by_number_params_factory(),
         ),
 
+    @tag("get-logs")
     @task
     def get_logs_task(self):
         self.make_call(
             name="get_logs",
             method="eth_getLogs",
             params=self._get_logs_params_factory(),
         ),
```

### Comparing `chainbench-0.2.0/chainbench/profile/evm/light.py` & `chainbench-0.3.0/chainbench/profile/evm/light.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """
 Ethereum profile (light mode).
 """
-from locust import task
+from locust import constant_pacing, task
 
 from chainbench.user.evm import EVMBenchUser
 
 
 class EthereumLightProfile(EVMBenchUser):
+    wait_time = constant_pacing(2)
+
     @task
     def get_transaction_receipt_task(self):
         self.make_call(
             name="get_transaction_receipt",
             method="eth_getTransactionReceipt",
             params=self._transaction_by_hash_params_factory(),
         ),
```

### Comparing `chainbench-0.2.0/chainbench/profile/oasis.py` & `chainbench-0.3.0/chainbench/profile/oasis/general.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from locust import between, task
+from locust import constant_pacing, task
 
 from chainbench.user.evm import EVMBenchUser
 
 
 class OasisProfile(EVMBenchUser):
-    wait_time = between(0.1, 1.5)
+    wait_time = constant_pacing(2)
 
     @task
     def get_block_by_number_task(self):
         self.make_call(
             name="get_block_by_number",
             method="eth_getBlockByNumber",
             params=self._block_by_number_params_factory(),
```

### Comparing `chainbench-0.2.0/chainbench/profile/polygon.py` & `chainbench-0.3.0/chainbench/profile/bsc/general.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,104 +1,108 @@
 """
-Polygon profile.
-
-Note, that eth_sendRawTransaction is excluded from the test because it requires
-building a transaction and signing it.
+Bsc profile.
 
 Chart:
 ```mermaid
 %%{init: {'theme':'forest'}}%%
 pie title Methods Distribution
     "eth_call" : 100
-    "eth_getTransactionReceipt" : 64
-    "eth_chainId" : 20
-    "eth_getBlockByNumber" : 17
-    "eth_blockNumber" : 16
-    "eth_getTransactionByHash" : 11
-    "eth_getLogs" : 11
-    "Others" : 9
+    "eth_getTransactionReceipt" : 93
+    "eth_getLogs" : 36
+    "eth_blockNumber" : 28
+    "eth_chainId" : 18
+    "eth_getBlockByNumber" : 13
+    "Others" : 20
 ```
 """
-from locust import tag, task
+from locust import constant_pacing, tag, task
 
 from chainbench.user.evm import EVMBenchUser
 
 
-class PolygonProfile(EVMBenchUser):
+class BscProfile(EVMBenchUser):
+    wait_time = constant_pacing(2)
+    weight = 89
+
     @task(100)
     def call_task(self):
         self.make_call(
             name="call",
             method="eth_call",
             params=[
                 {
-                    "to": "0xc2132D05D31c914a87C6611C10748AEb04B58e8F",
-                    "data": "0x70a08231000000000000000000000000F977814e90dA44bFA03b6295A0616a897441aceC",  # noqa: E501
+                    "to": "0x55d398326f99059fF775485246999027B3197955",
+                    "data": "0x70a08231000000000000000000000000f977814e90da44bfa03b6295a0616a897441acec",  # noqa: E501
                 },
                 "latest",
             ],
         ),
 
-    @task(64)
+    @task(93)
     def get_transaction_receipt_task(self):
         self.make_call(
             name="get_transaction_receipt",
             method="eth_getTransactionReceipt",
             params=self._transaction_by_hash_params_factory(),
         ),
 
-    @task(20)
+    @task(28)
+    def block_number_task(self):
+        self.make_call(
+            name="block_number",
+            method="eth_blockNumber",
+            params=[],
+        ),
+
+    @task(18)
     def chain_id_task(self):
         self.make_call(
             name="chain_id",
             method="eth_chainId",
             params=[],
         ),
 
-    @task(17)
+    @task(13)
     def get_block_by_number_task(self):
         self.make_call(
             name="get_block_by_number",
             method="eth_getBlockByNumber",
             params=self._block_by_number_params_factory(),
         ),
 
-    @task(16)
-    def block_number_task(self):
-        self.make_call(
-            name="block_number",
-            method="eth_blockNumber",
-            params=[],
-        ),
-
-    @task(11)
+    @task(9)
     def get_transaction_by_hash_task(self):
         self.make_call(
             name="get_transaction_by_hash",
             method="eth_getTransactionByHash",
             params=self._transaction_by_hash_params_factory(),
         ),
 
-    @task(11)
-    def get_logs_task(self):
-        self.make_call(
-            name="get_logs",
-            method="eth_getLogs",
-            params=self._get_logs_params_factory(),
-        ),
-
-    @task(4)
+    @task(5)
     def get_balance_task(self):
         self.make_call(
             name="get_balance",
             method="eth_getBalance",
             params=self._get_balance_params_factory_latest(),
         ),
 
-    @tag("trace")
-    @task(2)
-    def block_task(self):
+    @task(3)
+    def get_block_by_hash_task(self):
         self.make_call(
-            name="block",
-            method="trace_block",
-            params=self._block_by_number_params_factory(),
+            name="get_block_by_hash",
+            method="eth_getBlockByHash",
+            params=self._block_by_hash_params_factory(),
+        ),
+
+
+class GetLogsProfile(EVMBenchUser):
+    wait_time = constant_pacing(10)
+    weight = 12
+
+    @tag("get-logs")
+    @task
+    def get_logs_task(self):
+        self.make_call(
+            name="get_logs",
+            method="eth_getLogs",
+            params=self._get_logs_params_factory(),
         ),
```

### Comparing `chainbench-0.2.0/chainbench/test_data/base.py` & `chainbench-0.3.0/chainbench/test_data/base.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.2.0/chainbench/test_data/evm.py` & `chainbench-0.3.0/chainbench/test_data/evm.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 import random
 
 from chainbench.test_data.base import BaseTestData, BlockchainData
 
 
 class EVMTestData(BaseTestData):
     TXS_REQUIRED = 50
+    ACCOUNTS_REQUIRED = 100
     SAVE_LAST_BLOCKS = 100
 
     @staticmethod
     def _parse_hex_to_int(value: str) -> int:
         return int(value, 16)
 
+    @staticmethod
+    def _append_if_not_none(data_list, val):
+        if val is not None:
+            data_list.append(val)
+
     def _fetch_block(
         self, block_number: int | str, return_txs: bool = True
     ) -> tuple[int, dict]:
         if isinstance(block_number, int):
             block_number = hex(block_number)
         elif (block_number := block_number.lower()) not in (
             "latest",
@@ -28,33 +34,33 @@
     def _fetch_random_block(self, start, end, return_txs=True) -> tuple[int, dict]:
         block_number = random.randint(start, end)
         return self._fetch_block(block_number, return_txs=return_txs)
 
     # get initial data from blockchain
     def _get_init_data(self) -> BlockchainData:
         latest_block_number, latest_block = self._fetch_block("latest")
-        txs = []
-        tx_hashes = []
-        accounts = []
+        txs: list[dict] = []
+        tx_hashes: list[str] = []
+        accounts: list[str] = []
         blocks = [(latest_block_number, latest_block["hash"])]
         # extract data from block
         for tx in latest_block["transactions"]:
-            txs.append(tx)
-            tx_hashes.append(tx["hash"])
-            accounts.append(tx["from"])
-            accounts.append(tx["to"])
+            self._append_if_not_none(txs, tx)
+            self._append_if_not_none(tx_hashes, tx["hash"])
+            self._append_if_not_none(accounts, tx["from"])
+            self._append_if_not_none(accounts, tx["to"])
 
-        while self.TXS_REQUIRED > len(txs):
+        while self.TXS_REQUIRED > len(txs) and self.ACCOUNTS_REQUIRED > len(accounts):
             block_number, block = self._fetch_random_block(0, latest_block_number)
             blocks.append((block_number, block["hash"]))
             for tx in block["transactions"]:
-                txs.append(tx)
-                tx_hashes.append(tx["hash"])
-                accounts.append(tx["from"])
-                accounts.append(tx["to"])
+                self._append_if_not_none(txs, tx)
+                self._append_if_not_none(tx_hashes, tx["hash"])
+                self._append_if_not_none(accounts, tx["from"])
+                self._append_if_not_none(accounts, tx["to"])
 
         return BlockchainData(
             latest_block_number=latest_block_number,
             latest_block=latest_block,
             first_block_number=0,
             blocks=blocks,
             txs=txs,
```

### Comparing `chainbench-0.2.0/chainbench/user/base.py` & `chainbench-0.3.0/chainbench/user/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 from locust.contrib.fasthttp import RestResponseContextManager
 from locust.exception import RescheduleTask
 
 from chainbench.test_data import BaseTestData, DummyTestData
 from chainbench.util.event import setup_event_listeners
 from chainbench.util.rpc import generate_request
 
+# importing plugins here as all profiles depend on it
+import locust_plugins  # isort: skip  # noqa
+
+
 setup_event_listeners()
 
 
 class BaseBenchUser(FastHttpUser):
     """Base class for all benchmark users."""
 
     abstract = True
```

### Comparing `chainbench-0.2.0/chainbench/user/evm.py` & `chainbench-0.3.0/chainbench/user/evm.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.2.0/chainbench/util/event.py` & `chainbench-0.3.0/chainbench/util/event.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.2.0/chainbench/util/notify.py` & `chainbench-0.3.0/chainbench/util/notify.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.2.0/pyproject.toml` & `chainbench-0.3.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [tool.poetry]
 name = "chainbench"
-version = "0.2.0"
+version = "0.3.0"
 description = ""
 authors = ["Egor Molodik <egor.molodik@chainstack.com>"]
 readme = "README.md"
 packages = [{include = "chainbench"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 httpx = "^0.24.0"
 locust = "^2.15.0"
 click = "^8.1.3"
+locust-plugins = "^3.3.0"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 mypy = "^1.2.0"
 pre-commit = "^3.2.2"
 flake8 = "^6.0.0"
```

### Comparing `chainbench-0.2.0/PKG-INFO` & `chainbench-0.3.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: chainbench
-Version: 0.2.0
+Version: 0.3.0
 Summary: 
 Author: Egor Molodik
 Author-email: egor.molodik@chainstack.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: httpx (>=0.24.0,<0.25.0)
 Requires-Dist: locust (>=2.15.0,<3.0.0)
+Requires-Dist: locust-plugins (>=3.3.0,<4.0.0)
 Description-Content-Type: text/markdown
 
 <img width="1200" alt="Labs" src="https://user-images.githubusercontent.com/99700157/213291931-5a822628-5b8a-4768-980d-65f324985d32.png">
 
 <p>
  <h3 align="center">Chainstack is the leading suite of services connecting developers with Web3 infrastructure</h3>
 </p>
@@ -105,31 +106,31 @@
 chainbench start --profile bsc --users 50 --workers 2 --test-time 12h --target https://node-url --headless --autoquit
 ```
 
 This will run a load test for BSC with 2 workers, 50 users and 12 hours test time in headless mode.
 After the test is finished, the tool will automatically quit.
 
 ### Parameters and Flags
-- `--profile`: This flag specifies the profile to use for the benchmark. Available profiles are `ethereum`, `bsc`, `polygon`, `oasis`, and `avalanche`.
-- `--users`: This flag sets the number of simulated users to use for the benchmark.
-- `--workers`: This flag sets the number of worker threads to use for the benchmark.
-- `--test-time`: This flag sets the duration of the test to run.
-- `--target`: This flag specifies the target blockchain node URL that the benchmark will connect to.
-- `--headless`: This flag runs the benchmark in headless mode, meaning that no graphical user interface (GUI) will be displayed during the test. This is useful for running the test on a remote server or when the GUI is not needed.
-- `--autoquit`: This flag tells the Chainbench tool to automatically quit after the test has finished. This is useful for running the benchmark in an automated environment where manual intervention is not desired.
-- `--help`: This flag displays the help message.
-
-By default, Chainbench uses `constant_pacing` wait time with a value of 10 seconds. 
-This means a load test with 100 users will have a theoretical maximum of 10 rps. This allows us to have a target rps in a test, 
-and the result rps lower than the target rps means performance deterioration.
+- `-p, --profile`: Specifies the profile to use for the benchmark. Available profiles can be found in the profile directory. Sample usage `-p bsc.general`
+- `-u, --users`: Sets the number of simulated users to use for the benchmark.
+- `-w, --workers`: Sets the number of worker threads to use for the benchmark.
+- `-t, --test-time`: Sets the duration of the test to run.
+- `--target`: Specifies the target blockchain node URL that the benchmark will connect to.
+- `--headless`: Runs the benchmark in headless mode, meaning that no graphical user interface (GUI) will be displayed during the test. This is useful for running the test on a remote server or when the GUI is not needed.
+- `--autoquit`: Tells the Chainbench tool to automatically quit after the test has finished. This is useful for running the benchmark in an automated environment where manual intervention is not desired.
+- `--help`: Displays the help message.
+- `--debug-trace-methods`: Enables tasks tagged with debug or trace to be executed
+- `-E, --exclude-tags`: Exclude tasks tagged with custom tags from the test. You may specify this option multiple times --help Show this message and exit.
+
+You may also run `chainbench start --help` for the full list of parameters and flags.
 
 ### Profiles
 Default profiles are located in the [`profile`](chainbench/profile) directory. For a tutorial on how to create custom profiles, please refer to [this document](docs/PROFILE.md).
 
-You can also use the `--profile-dir` flag to specify a custom directory with profiles. For example:
+You can also use the `-d` or `--profile-dir` flag to specify a custom directory with profiles. For example:
 ```shell
 chainbench start --profile-dir /path/to/profiles --profile my-profile --users 50 --workers 2 --test-time 12h --target https://node-url --headless --autoquit
 ```
 This will run a load test using `/path/to/profiles/my-profile.py` profile.
 
 It's possible to group profiles into directories. For example, you can create a directory called `bsc` and put all the BSC profiles there. Then you can run a load test using the following command:
 ```shell
@@ -144,18 +145,18 @@
 ```shell
 chainbench start --profile evm.light --users 50 --workers 2 --test-time 12h --target https://node-url --headless --autoquit
 ```
 
 ### Web UI Mode
 
 Run the following command to run a load test for BSC in UI mode. It will start a web server on port 8089. 
-Target is not required as you can specify it in the UI along with the number of users, spawn rate and test time.
+Target is required to initialize the test data, however you may change the target endpoint later in the UI, along with the number of users, spawn rate and test time.
 
 ```shell
-chainbench start --profile bsc --workers 1
+chainbench start --profile bsc.general --workers 1 --target https://any-working-node-endpoint.com
 ```
 
 ### Headless Mode
 
 If you want to run a load test for BSC in headless mode, run the following command:
 
 ```shell
```

