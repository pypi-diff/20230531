# Comparing `tmp/tiny_ai_helper-0.1.8.tar.gz` & `tmp/tiny_ai_helper-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiny_ai_helper-0.1.8.tar", last modified: Tue May 23 17:26:19 2023, max compression
+gzip compressed data, was "tiny_ai_helper-0.1.9.tar", last modified: Wed May 31 16:25:58 2023, max compression
```

## Comparing `tiny_ai_helper-0.1.8.tar` & `tiny_ai_helper-0.1.9.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxrwxr-x   0 www-data  (1000) www-data  (1000)        0 2023-05-23 17:26:19.861100 tiny_ai_helper-0.1.8/
--rw-rw-r--   0 www-data  (1000) www-data  (1000)     1103 2023-03-09 17:46:27.000000 tiny_ai_helper-0.1.8/LICENSE
--rw-rw-r--   0 www-data  (1000) www-data  (1000)      784 2023-05-23 17:26:19.861100 tiny_ai_helper-0.1.8/PKG-INFO
--rw-rw-r--   0 www-data  (1000) www-data  (1000)       74 2022-09-27 15:48:25.000000 tiny_ai_helper-0.1.8/README.md
--rw-rw-r--   0 www-data  (1000) www-data  (1000)       38 2023-05-23 17:26:19.861100 tiny_ai_helper-0.1.8/setup.cfg
--rw-rw-r--   0 www-data  (1000) www-data  (1000)     1029 2023-05-23 16:45:08.000000 tiny_ai_helper-0.1.8/setup.py
-drwxrwxr-x   0 www-data  (1000) www-data  (1000)        0 2023-05-23 17:26:19.857100 tiny_ai_helper-0.1.8/tiny_ai_helper/
--rw-rw-r--   0 www-data  (1000) www-data  (1000)    16082 2023-05-23 17:23:20.000000 tiny_ai_helper-0.1.8/tiny_ai_helper/Model.py
--rw-rw-r--   0 www-data  (1000) www-data  (1000)    10452 2023-04-30 10:47:53.000000 tiny_ai_helper-0.1.8/tiny_ai_helper/Trainer.py
--rw-rw-r--   0 www-data  (1000) www-data  (1000)      310 2023-05-23 16:45:14.000000 tiny_ai_helper-0.1.8/tiny_ai_helper/__init__.py
--rw-rw-r--   0 www-data  (1000) www-data  (1000)     6522 2023-05-23 10:24:05.000000 tiny_ai_helper-0.1.8/tiny_ai_helper/layers.py
--rw-rw-r--   0 www-data  (1000) www-data  (1000)     9071 2023-03-15 18:42:46.000000 tiny_ai_helper-0.1.8/tiny_ai_helper/mp.py
--rw-rw-r--   0 www-data  (1000) www-data  (1000)    21782 2023-05-23 14:05:17.000000 tiny_ai_helper-0.1.8/tiny_ai_helper/utils.py
-drwxrwxr-x   0 www-data  (1000) www-data  (1000)        0 2023-05-23 17:26:19.861100 tiny_ai_helper-0.1.8/tiny_ai_helper.egg-info/
--rw-rw-r--   0 www-data  (1000) www-data  (1000)      784 2023-05-23 17:26:19.000000 tiny_ai_helper-0.1.8/tiny_ai_helper.egg-info/PKG-INFO
--rw-rw-r--   0 www-data  (1000) www-data  (1000)      325 2023-05-23 17:26:19.000000 tiny_ai_helper-0.1.8/tiny_ai_helper.egg-info/SOURCES.txt
--rw-rw-r--   0 www-data  (1000) www-data  (1000)        1 2023-05-23 17:26:19.000000 tiny_ai_helper-0.1.8/tiny_ai_helper.egg-info/dependency_links.txt
--rw-rw-r--   0 www-data  (1000) www-data  (1000)       15 2023-05-23 17:26:19.000000 tiny_ai_helper-0.1.8/tiny_ai_helper.egg-info/top_level.txt
+drwxrwxr-x   0 www-data  (1000) www-data  (1000)        0 2023-05-31 16:25:58.924731 tiny_ai_helper-0.1.9/
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)     1103 2023-03-09 17:46:27.000000 tiny_ai_helper-0.1.9/LICENSE
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)      784 2023-05-31 16:25:58.924731 tiny_ai_helper-0.1.9/PKG-INFO
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)       74 2022-09-27 15:48:25.000000 tiny_ai_helper-0.1.9/README.md
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)       38 2023-05-31 16:25:58.924731 tiny_ai_helper-0.1.9/setup.cfg
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)     1029 2023-05-28 14:39:06.000000 tiny_ai_helper-0.1.9/setup.py
+drwxrwxr-x   0 www-data  (1000) www-data  (1000)        0 2023-05-31 16:25:58.920731 tiny_ai_helper-0.1.9/tiny_ai_helper/
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)    20652 2023-05-31 13:15:28.000000 tiny_ai_helper-0.1.9/tiny_ai_helper/Model.py
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)      266 2023-05-30 14:06:48.000000 tiny_ai_helper-0.1.9/tiny_ai_helper/__init__.py
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)     6668 2023-05-31 13:29:08.000000 tiny_ai_helper-0.1.9/tiny_ai_helper/layers.py
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)     9071 2023-03-15 18:42:46.000000 tiny_ai_helper-0.1.9/tiny_ai_helper/mp.py
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)    23364 2023-05-31 13:27:35.000000 tiny_ai_helper-0.1.9/tiny_ai_helper/utils.py
+drwxrwxr-x   0 www-data  (1000) www-data  (1000)        0 2023-05-31 16:25:58.924731 tiny_ai_helper-0.1.9/tiny_ai_helper.egg-info/
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)      784 2023-05-31 16:25:58.000000 tiny_ai_helper-0.1.9/tiny_ai_helper.egg-info/PKG-INFO
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)      299 2023-05-31 16:25:58.000000 tiny_ai_helper-0.1.9/tiny_ai_helper.egg-info/SOURCES.txt
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)        1 2023-05-31 16:25:58.000000 tiny_ai_helper-0.1.9/tiny_ai_helper.egg-info/dependency_links.txt
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)       15 2023-05-31 16:25:58.000000 tiny_ai_helper-0.1.9/tiny_ai_helper.egg-info/top_level.txt
```

### Comparing `tiny_ai_helper-0.1.8/LICENSE` & `tiny_ai_helper-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tiny_ai_helper-0.1.8/PKG-INFO` & `tiny_ai_helper-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiny_ai_helper
-Version: 0.1.8
+Version: 0.1.9
 Summary: Tiny AI Helper for PyTorch
 Home-page: https://github.com/bayrell/ai_helper
 Author: Ildar Bikmamatov
 Author-email: support@bayrell.org
 License: MIT License
 Keywords: ai helper,pytorch
 Platform: UNKNOWN
```

### Comparing `tiny_ai_helper-0.1.8/setup.py` & `tiny_ai_helper-0.1.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 """
 
 from setuptools import setup, find_packages
 from os.path import abspath, dirname, join
 
 setup(
 	name="tiny_ai_helper",
-	version="0.1.8",
+	version="0.1.9",
 	description="Tiny AI Helper for PyTorch",
 	long_description=open(join(abspath(dirname(__file__)), 'README.md'), encoding='utf-8').read(),
 	long_description_content_type='text/markdown',
 	author="Ildar Bikmamatov",
 	author_email="support@bayrell.org",
 	license="MIT License",
 	url = "https://github.com/bayrell/ai_helper",
```

### Comparing `tiny_ai_helper-0.1.8/tiny_ai_helper/Model.py` & `tiny_ai_helper-0.1.9/tiny_ai_helper/Model.py`

 * *Files 12% similar despite different names*

```diff
@@ -93,16 +93,16 @@
         
         if self.optimizer is None:
             try:
                 self.optimizer = torch.optim.Adam(self.module.parameters(), lr=1e-3)
             except:
                 pass
         
-        if self.scheduler is None and self.optimizer is not None:
-            self.scheduler = torch.optim.lr_scheduler.ReduceLROnPlateau( self.optimizer )
+        #if self.scheduler is None and self.optimizer is not None:
+        #    self.scheduler = torch.optim.lr_scheduler.ReduceLROnPlateau( self.optimizer )
         
         return self
     
     
     def to(self, device):
         self.module = self.module.to(device)
         self.device = device
@@ -122,46 +122,62 @@
         return self
     
     def eval(self):
         self.module.eval()
         return self
     
     
+    def load_weights(self, file_path):
+        
+        """
+        Load weights
+        """
+        
+        state_dict = torch.load(file_path)
+        self.module.load_state_dict(state_dict, strict=False)
+        
+        
     def load_file(self, file_path):
         
         """
         Load model from file
         """
         
         save_metrics = torch.load(file_path)
-        self.epoch = save_metrics["epoch"]
         
-        # Load history
-        if "history" in save_metrics:
-            self.history = save_metrics["history"].copy()
-        
-        # Load module
-        if "module" in save_metrics:
-            state_dict = save_metrics["module"]
-            self.module.load_state_dict(state_dict, strict=False)
-        
-        # Load optimizer
-        if "optimizer" in save_metrics:
-            state_dict = save_metrics["optimizer"]
-            self.optimizer.load_state_dict(state_dict)
-        
-        # Load scheduler
-        if "scheduler" in save_metrics:
-            state_dict = save_metrics["scheduler"]
-            self.scheduler.load_state_dict(state_dict)
-        
-        # Load loss
-        if "loss" in save_metrics:
-            state_dict = save_metrics["loss"]
-            self.loss.load_state_dict(state_dict)
+        if "epoch" in save_metrics:
+            
+            self.epoch = save_metrics["epoch"]
+            
+            # Load history
+            if "history" in save_metrics:
+                self.history = save_metrics["history"].copy()
+            
+            # Load module
+            if "module" in save_metrics:
+                state_dict = save_metrics["module"]
+                self.module.load_state_dict(state_dict, strict=False)
+            
+            # Load optimizer
+            if "optimizer" in save_metrics:
+                state_dict = save_metrics["optimizer"]
+                self.optimizer.load_state_dict(state_dict)
+            
+            # Load scheduler
+            if "scheduler" in save_metrics:
+                state_dict = save_metrics["scheduler"]
+                self.scheduler.load_state_dict(state_dict)
+            
+            # Load loss
+            if "loss" in save_metrics:
+                state_dict = save_metrics["loss"]
+                self.loss.load_state_dict(state_dict)
+        
+        else:
+            self.module.load_state_dict(save_metrics, strict=False)
         
     
     def load(self, file_name):
         
         """
         Load model by file name
         """
@@ -210,31 +226,53 @@
             return
         
         obj = load_json(file_name)
         
         if obj is not None:
             best_epoch = obj["best_epoch"]
             self.load_epoch(best_epoch)
+    
+    
+    def save_weights(self, file_path=None):
+        
+        """
+        Save weights
+        """
         
+        if file_path is None:
+            model_name = self.get_full_name() + "-" + str(self.epoch) + ".pth"
+            file_path = os.path.join(
+                self.model_path,
+                model_name
+            )
+        
+        torch.save(self.module.state_dict(), file_path)
+    
     
-    def save_epoch(self):
+    def save_model(self):
         
         """
         Save train status
         """
         
         # Get metrics
         save_metrics = {}
         save_metrics["name"] = self.get_full_name()
         save_metrics["epoch"] = self.epoch
         save_metrics["history"] = self.history.copy()
         save_metrics["module"] = self.module.state_dict()
-        save_metrics["optimizer"] = self.optimizer.state_dict()
-        save_metrics["scheduler"] = self.scheduler.state_dict()
-        save_metrics["loss"] = self.loss.state_dict()
+        
+        if self.optimizer is not None:
+            save_metrics["optimizer"] = self.optimizer.state_dict()
+        
+        if self.scheduler is not None:
+            save_metrics["scheduler"] = self.scheduler.state_dict()
+        
+        if self.loss is not None:
+            save_metrics["loss"] = self.loss.state_dict()
         
         # Create folder
         if not os.path.isdir(self.model_path):
             os.makedirs(self.model_path)
         
         # Save model to file
         file_name = os.path.join(self.model_path, "model-" + str(self.epoch) + ".data")
@@ -274,19 +312,16 @@
         
         if self.optimizer.param_groups[0]["lr"] < self.min_lr:
             return False
         
         return True
     
     
-    def fit(self, train_dataset, val_dataset,
-        batch_size=32, epochs=10
-    ):
-        fit(self, train_dataset, val_dataset,
-            batch_size=batch_size, epochs=epochs)
+    def __call__(self, x):
+        return self.module(x)
     
     
     def predict(self, x):
         
         """
         Predict
         """
@@ -396,14 +431,34 @@
                 res2.append( value )
             
             res.append(res2)
             
         return res
     
     
+    def get_metric(self, metric_name, convert=False):
+        
+        """
+        Returns metrics by name
+        """
+        
+        res = []
+        epochs = list(self.history.keys())
+        for index in epochs:
+            
+            epoch = self.history[index]
+                        
+            value = epoch[metric_name] if metric_name in epoch else 0
+            if convert:
+                value = convert_value(value, metric_name)
+            res.append( value )
+            
+        return res
+    
+    
     def get_the_best_epoch(self):
         
         """
         Returns the best epoch
         """
         
         epoch_indexes = self.get_the_best_epochs_indexes(1)
@@ -488,15 +543,15 @@
         """
         
         summary(self.module, x, y,
             device=self.device,
             model_name=self.get_full_name()
         )
     
-    
+        
     def draw_history_ax(self, ax, metrics=[], label=None, legend=True, convert=None):
         
         """
         Draw history to axes
         """
         
         metrics_values = self.get_metrics(metrics)
@@ -540,42 +595,146 @@
         h.sort()
         
         for epoch in h:
             s = self.get_epoch_string(epoch)
             print(s)
     
     
+    def add_epoch(self,
+        train_batch_iter=None, train_batch_count=None,
+        train_acc=None, train_loss=None,
+        val_batch_iter=None, val_batch_count=None,
+        val_acc=None, val_loss=None,
+        t=None, **kwargs
+    ):
+    
+        lr = []
+        for param_group in self.optimizer.param_groups:
+            lr.append( round(param_group['lr'], 7) )
+        
+        h = {
+            "epoch": self.epoch,
+            "train_batch_iter": train_batch_iter,
+            "train_batch_count": train_batch_count,
+            "train_acc_total": train_acc,
+            "train_loss_total": train_loss,
+            "val_batch_iter": val_batch_iter,
+            "val_batch_count": val_batch_count,
+            "val_acc_total": val_acc,
+            "val_loss_total": val_loss,
+            "train_loss": None,
+            "train_acc": None,
+            "val_loss": None,
+            "val_acc": None,
+            "rel": None,
+            "lr": lr,
+            "t": t,
+            **kwargs
+        }
+        
+        if self.loss_reduction == "mean":
+            
+            if train_batch_iter is not None:
+                h["train_loss"] = train_loss / train_batch_iter
+            
+            if val_batch_iter is not None:
+                h["val_loss"] = val_loss / val_batch_iter
+        
+        elif self.loss_reduction == "sum":
+            
+            if train_batch_count is not None:
+                h["train_loss"] = train_loss / train_batch_count
+            
+            if val_batch_count is not None:
+                h["val_loss"] = val_loss / val_batch_count
+        
+        if train_acc is not None:
+            h["train_acc"] = (train_acc / train_batch_count) if train_batch_count > 0 else 0
+        
+        if val_acc is not None:
+            h["val_acc"] = (val_acc / val_batch_count) if val_batch_count > 0 else 0
+        
+        if h["train_acc"] is not None and h["val_acc"] is not None:
+            h["rel"] = (h["train_acc"] / h["val_acc"]) if h["val_acc"] > 0 else 0
+        
+        self.history[self.epoch] = h
+    
+    
     def get_epoch_string(self, epoch):
         
         res = self.history[epoch]
         
         # Get epoch status
         t = res["time"] if "time" in res else 0
         train_acc = res["train_acc"] if "train_acc" in res else 0
         train_loss = res["train_loss"] if "train_loss" in res else 0
         train_count = res["train_count"] if "train_count" in res else 0
         val_acc = res["val_acc"] if "val_acc" in res else 0
         val_loss = res["val_loss"] if "val_loss" in res else 0
         val_count = res["val_count"] if "val_count" in res else 0
-        res_lr = res["res_lr"] if "res_lr" in res else []
+        res_lr = res["lr"] if "lr" in res else []
         res_lr_str = str(res_lr)
         
         # Get result
         f = "{:."+str(self.loss_precision)+"f}"
         train_loss = f.format(train_loss)
         val_loss = f.format(val_loss)
-        train_acc = round(train_acc / train_count * 10000) / 100
-        val_acc = round(val_acc / val_count * 10000) / 100
+        train_acc = round(train_acc * 10000) / 100
+        val_acc = round(val_acc * 10000) / 100
         
         msg = []
         msg.append(f'\rEpoch: {epoch}')
         
         if self.acc_fn is not None:
-            acc_rel = "{:.4f}".format(train_acc / val_acc) if val_acc > 0 else 0
+            acc_rel = res["rel"] if "rel" in res else 0
             msg.append(f'train_acc: {train_acc}%, val_acc: {val_acc}%, rel: {acc_rel}')
         
         msg.append(f'train_loss: {train_loss}, val_loss: {val_loss}')
         msg.append(f'lr: {res_lr_str}, t: {t}s')
         
         return ", ".join(msg)
         
+    
+    def get_train_loss(self, epoch=None):
+        if epoch is None:
+            epoch = self.epoch
+        value = self.history[epoch]["train_loss"]
+        if value is None:
+            value = 0
+        return value
+    
+    
+    def get_val_loss(self, epoch=None):
+        if epoch is None:
+            epoch = self.epoch
+        value = self.history[epoch]["train_loss"]
+        if value is None:
+            value = 0
+        return value
+    
+    
+    def get_train_acc(self, epoch=None):
+        if epoch is None:
+            epoch = self.epoch
+        value = self.history[epoch]["train_acc"]
+        if value is None:
+            value = 0
+        return value
+    
+    
+    def get_val_acc(self, epoch=None):
+        if epoch is None:
+            epoch = self.epoch
+        value = self.history[epoch]["train_acc"]
+        if value is None:
+            value = 0
+        return value
+    
+    
+    def get_epoch_metric(self, metric_name, epoch=None):
+        if epoch is None:
+            epoch = self.epoch
+        value = self.history[epoch][metric_name]
+        if value is None:
+            value = 0
+        return value
```

### Comparing `tiny_ai_helper-0.1.8/tiny_ai_helper/layers.py` & `tiny_ai_helper-0.1.9/tiny_ai_helper/layers.py`

 * *Files 4% similar despite different names*

```diff
@@ -172,24 +172,25 @@
         return 'mean={}, std={}, inplace={}'.format(
             self.mean, self.std, self.inplace
         )
 
 
 class PreparedModule(torch.nn.Module):
     
-    def __init__(self, module, weight_path=None, forward=None, *args, **kwargs):
+    def __init__(self, module, weight_path=None, forward=None, requires_grad=False, *args, **kwargs):
         
         torch.nn.Module.__init__(self)
         
         self.module = module
         self.weight_path = weight_path
         self._forward = forward
         
-        for param in self.module.parameters():
-            param.requires_grad = False
+        if not requires_grad:
+            for param in self.module.parameters():
+                param.requires_grad = False
         
         self.load_weight()
     
     def forward(self, x):
         
         if self._forward:
             x = self._forward(self, x)
@@ -250,39 +251,39 @@
                 module.state_dict(
                     destination=destination,
                     prefix=prefix + m + '.',
                     keep_vars=keep_vars
                 )
 
 
-class Pipe():
+class Pipe(torch.nn.Module):
     def __init__(self, *args):
         torch.nn.Module.__init__(self)
         self.pipe = args
     
     def forward(self, value):
         for fn in self.pipe:
             value = fn(value)
         return value
 
 
 class ModuleRemoveLastClassifier(PreparedModule):
     
-    def __init__(self, module, weight_path=None, *args, **kwargs):
+    def __init__(self, module, weight_path=None, requires_grad=False, *args, **kwargs):
         
-        PreparedModule.__init__(self, module, weight_path, *args, **kwargs)
+        PreparedModule.__init__(self, module, weight_path, requires_grad, *args, **kwargs)
         
         # Remove last layer
         classifier = list(self.module.classifier.children())
         classifier = classifier[:-1]
         self.module.classifier = torch.nn.Sequential(*classifier)
 
 
 class ModuleRemoveAllClassifier(PreparedModule):
     
-    def __init__(self, module, weight_path=None, *args, **kwargs):
-        PreparedModule.__init__(self, module, weight_path, *args, **kwargs)
+    def __init__(self, module, weight_path=None, requires_grad=False, *args, **kwargs):
+        PreparedModule.__init__(self, module, weight_path, requires_grad, *args, **kwargs)
     
     def forward(self, x):
         x = self.module.features(x)
         x = self.module.avgpool(x)
         return x
```

### Comparing `tiny_ai_helper-0.1.8/tiny_ai_helper/mp.py` & `tiny_ai_helper-0.1.9/tiny_ai_helper/mp.py`

 * *Files identical despite different names*

### Comparing `tiny_ai_helper-0.1.8/tiny_ai_helper/utils.py` & `tiny_ai_helper-0.1.9/tiny_ai_helper/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -306,15 +306,15 @@
     
     width, height = size
     
     if color == None:
         pixels = image.load()
         color = pixels[0, 0]
         del pixels
-        
+    
     image_new = Image.new(image.mode, (width, height), color = color)
     
     position = (
         math.ceil((width - image.size[0]) / 2),
         math.ceil((height - image.size[1]) / 2),
     )
     
@@ -341,15 +341,15 @@
     
     import matplotlib.pyplot as plt
     
     plt.imshow(image, cmap)
     plt.show()
 
 
-def list_files(path="", recursive=True):
+def list_files(path="", recursive=True, full_path=False):
     
     """
         Returns files in folder
     """
     
     def read_dir(path, recursive=True):
         res = []
@@ -376,14 +376,17 @@
             return item[len(path + "/"):]
         
         items = list( map(f, items) )
     
     except Exception:
         items = []
     
+    if full_path:
+        items = list( map(lambda x: os.path.join(path, x), items) )
+    
     return items
 
 
 def get_sort_alphanum_key(name):
     
     """
     Returns sort alphanum key
@@ -623,15 +626,16 @@
         for _, value in enumerate(values):
             print( format_row(value, info_sizes) )
         
         print( "-" * width )
         if model_name is not None and model_name != module.__class__.__name__:
             print( f"Model name: {model_name}" )
         print( f"Total params: {res['params_count']:_}".replace('_', ' ') )
-        print( f"Trainable params: {res['params_train_count']:_}".replace('_', ' ') )
+        if res['params_count'] != res['params_train_count'] and res['params_train_count'] > 0:
+            print( f"Trainable params: {res['params_train_count']:_}".replace('_', ' ') )
         #print( f"Total size: {res['total_size']} MiB" )
         print( "=" * width )
 
 
 def compile(module):
     from .Model import Model
     return Model(module)
@@ -679,16 +683,15 @@
             val_count = 0
             val_loss = 0
             val_iter = 0
             val_acc = 0
             total_count = len(train_dataset) + len(val_dataset)
             pos = 0
             
-            model.epoch = model.epoch + 1
-            epoch = model.epoch
+            epoch = model.epoch + 1
             
             # train mode
             model.train()
             
             for x_batch, y_batch in train_loader:
                 
                 # data to device
@@ -775,64 +778,125 @@
                     iter_value = round(pos / total_count * 100)
                     if val_acc_val > 0:
                         print(f"\rEpoch: {epoch}, {iter_value}%, acc: " + str(val_acc_val), end="")
                     else:
                         print(f"\rEpoch: {epoch}, {iter_value}%", end="")
             
             
-            if model.loss_reduction == "mean":
-                train_loss = (train_loss / train_iter).item()
-                val_loss = (val_loss / val_iter).item()
-            
-            elif model.loss_reduction == "sum":
-                train_loss = (train_loss / train_count).item()
-                val_loss = (val_loss / val_count).item()
-            
-            if scheduler is not None:
-               scheduler.step(val_loss)
-            
-            # Current lr
-            res_lr = []
-            for param_group in optimizer.param_groups:
-                res_lr.append( round(param_group['lr'], 7) )
-            
+            # Add metricks
             time_end = time.time()
             t = round(time_end - time_start)
             
-            train_acc_value = (train_acc / train_count) if train_count > 0 else 0
-            val_acc_value = (val_acc / val_count) if train_count > 0 else 0
-            
-            h = {
-                "epoch": epoch,
-                "rel": (train_acc_value / val_acc_value) if val_acc_value > 0 else 0,
-                "res_lr": res_lr,
-                "time": t,
-                "train_acc": train_acc,
-                "train_acc_value": train_acc_value,
-                "train_count": train_count,
-                "train_loss": train_loss,
-                "val_acc": val_acc,
-                "val_acc_value": val_acc_value,
-                "val_count": val_count,
-                "val_loss": val_loss,
-            }
+            model.add_epoch(
+                train_acc = train_acc,
+                train_batch_count = train_count,
+                train_batch_iter = train_iter,
+                train_loss = train_loss,
+                val_acc = val_acc,
+                val_batch_count = val_count,
+                val_batch_iter = val_iter,
+                val_loss = val_loss,
+                t = t,
+            )
             
-            model.history[epoch] = h
             print( model.get_epoch_string(epoch) )
             
-            model.save_epoch()
+            model.epoch = epoch
+            model.save_model()
             model.save_the_best_models()
             
             if res_lr[0] < min_lr:
                 break
-
+        
         print ("Ok")
 
     except KeyboardInterrupt:
         
         print ("")
         print ("Stopped manually")
         print ("")
 
     if torch.cuda.is_available():
         torch.cuda.empty_cache()
+
+
+def colab_upload_file_to_google_drive(src, dest):
+    
+    import shutil
+    
+    if not os.path.exists('/content/drive'):
+        from google.colab import drive
+        drive.mount('/content/drive')
+    
+    dest_dir_path = os.path.dirname(dest)
+    if not os.path.exists(dest_dir_path):
+        os.makedirs(dest_dir_path)
+    
+    shutil.copy(src, dest)
+    
+
+def colab_upload_model_to_google_drive(model, path, epoch):
+    
+    import shutil
+    
+    if not os.path.exists('/content/drive'):
+        from google.colab import drive
+        drive.mount('/content/drive')
+    
+    if not os.path.exists(generator_path):
+        os.makedirs(generator_path)
+    
+    src_file_path = os.path.join(model.model_path, "model-" + str(epoch) + ".data")
+    dest_file_path = os.path.join(path, "model-" + str(epoch) + ".data")
+    
+    shutil.copy(src_file_path, dest_file_path)
+
+
+def colab_upload_history_to_google_drive(model, path):
+    
+    import shutil
+    
+    if not os.path.exists('/content/drive'):
+        from google.colab import drive
+        drive.mount('/content/drive')
+    
+    if not os.path.exists(generator_path):
+        os.makedirs(generator_path)
+    
+    src_file_path = os.path.join(model.model_path, "history.json")
+    dest_file_path = os.path.join(path, "history.json")
+    
+    shutil.copy(src_file_path, dest_file_path)
+
+
+def colab_download_model_from_google_drive(model, path, epoch):
+    
+    import shutil
+    
+    if not os.path.exists('/content/drive'):
+        from google.colab import drive
+        drive.mount('/content/drive')
+    
+    if not os.path.exists(model.model_path):
+        os.makedirs(model.model_path)
+    
+    src_file_path = os.path.join(path, "model-" + str(epoch) + ".data")
+    dest_file_path = os.path.join(model.model_path, "model-" + str(epoch) + ".data")
+    
+    shutil.copy(src_file_path, dest_file_path)
+
+
+def colab_download_history_from_google_drive(model, path):
+    
+    import shutil
+    
+    if not os.path.exists('/content/drive'):
+        from google.colab import drive
+        drive.mount('/content/drive')
+    
+    if not os.path.exists(model.model_path):
+        os.makedirs(model.model_path)
+    
+    src_file_path = os.path.join(path, "history.json")
+    dest_file_path = os.path.join(model.model_path, "history.json")
     
+    shutil.copy(src_file_path, dest_file_path)
```

### Comparing `tiny_ai_helper-0.1.8/tiny_ai_helper.egg-info/PKG-INFO` & `tiny_ai_helper-0.1.9/tiny_ai_helper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiny-ai-helper
-Version: 0.1.8
+Version: 0.1.9
 Summary: Tiny AI Helper for PyTorch
 Home-page: https://github.com/bayrell/ai_helper
 Author: Ildar Bikmamatov
 Author-email: support@bayrell.org
 License: MIT License
 Keywords: ai helper,pytorch
 Platform: UNKNOWN
```

