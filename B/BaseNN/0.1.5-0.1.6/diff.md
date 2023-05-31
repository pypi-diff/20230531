# Comparing `tmp/BaseNN-0.1.5.tar.gz` & `tmp/BaseNN-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/BaseNN-0.1.5.tar", last modified: Fri May 26 06:31:28 2023, max compression
+gzip compressed data, was "dist/BaseNN-0.1.6.tar", last modified: Wed May 31 09:49:51 2023, max compression
```

## Comparing `BaseNN-0.1.5.tar` & `BaseNN-0.1.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-05-26 06:31:28.000000 BaseNN-0.1.5/
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-05-26 06:31:28.000000 BaseNN-0.1.5/BaseNN/
--rw-rw-r--   0 user      (1001) user      (1001)    38762 2023-05-26 06:29:57.000000 BaseNN-0.1.5/BaseNN/BaseNN.py
--rw-rw-r--   0 user      (1001) user      (1001)      270 2023-05-24 09:07:14.000000 BaseNN-0.1.5/BaseNN/__init__.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-05-26 06:31:28.000000 BaseNN-0.1.5/BaseNN/examples/
--rw-rw-r--   0 user      (1001) user      (1001)    22843 2023-05-25 09:05:57.000000 BaseNN-0.1.5/BaseNN/examples/BaseNN_demo.py
--rw-rw-r--   0 user      (1001) user      (1001)        0 2022-08-26 07:13:38.000000 BaseNN-0.1.5/BaseNN/examples/__init__.py
--rw-rw-r--   0 user      (1001) user      (1001)     3059 2023-04-13 07:47:30.000000 BaseNN-0.1.5/BaseNN/examples/pkl2pth.py
--rw-r--r--   0 user      (1001) user      (1001)     4409 2023-05-22 08:15:12.000000 BaseNN-0.1.5/BaseNN/load_data.py
--rw-rw-r--   0 user      (1001) user      (1001)     1256 2023-05-26 06:30:24.000000 BaseNN-0.1.5/BaseNN/version.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-05-26 06:31:28.000000 BaseNN-0.1.5/BaseNN.egg-info/
--rw-rw-r--   0 user      (1001) user      (1001)      346 2023-05-26 06:31:28.000000 BaseNN-0.1.5/BaseNN.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1001) user      (1001)      375 2023-05-26 06:31:28.000000 BaseNN-0.1.5/BaseNN.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1001) user      (1001)        1 2023-05-26 06:31:28.000000 BaseNN-0.1.5/BaseNN.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1001) user      (1001)       49 2023-05-26 06:31:28.000000 BaseNN-0.1.5/BaseNN.egg-info/entry_points.txt
--rw-rw-r--   0 user      (1001) user      (1001)       80 2023-05-26 06:31:28.000000 BaseNN-0.1.5/BaseNN.egg-info/requires.txt
--rw-rw-r--   0 user      (1001) user      (1001)        7 2023-05-26 06:31:28.000000 BaseNN-0.1.5/BaseNN.egg-info/top_level.txt
--rw-rw-r--   0 user      (1001) user      (1001)        1 2022-11-18 03:21:26.000000 BaseNN-0.1.5/BaseNN.egg-info/zip-safe
--rw-rw-r--   0 user      (1001) user      (1001)      346 2023-05-26 06:31:28.000000 BaseNN-0.1.5/PKG-INFO
--rw-rw-r--   0 user      (1001) user      (1001)       38 2023-05-26 06:31:28.000000 BaseNN-0.1.5/setup.cfg
--rw-rw-r--   0 user      (1001) user      (1001)     3827 2023-05-26 06:30:17.000000 BaseNN-0.1.5/setup.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-05-31 09:49:51.000000 BaseNN-0.1.6/
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-05-31 09:49:51.000000 BaseNN-0.1.6/BaseNN/
+-rw-rw-r--   0 user      (1001) user      (1001)    38906 2023-05-31 09:49:11.000000 BaseNN-0.1.6/BaseNN/BaseNN.py
+-rw-rw-r--   0 user      (1001) user      (1001)      270 2023-05-24 09:07:14.000000 BaseNN-0.1.6/BaseNN/__init__.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-05-31 09:49:51.000000 BaseNN-0.1.6/BaseNN/examples/
+-rw-rw-r--   0 user      (1001) user      (1001)    22901 2023-05-29 09:42:57.000000 BaseNN-0.1.6/BaseNN/examples/BaseNN_demo.py
+-rw-rw-r--   0 user      (1001) user      (1001)        0 2022-08-26 07:13:38.000000 BaseNN-0.1.6/BaseNN/examples/__init__.py
+-rw-rw-r--   0 user      (1001) user      (1001)     3059 2023-04-13 07:47:30.000000 BaseNN-0.1.6/BaseNN/examples/pkl2pth.py
+-rw-r--r--   0 user      (1001) user      (1001)     4409 2023-05-22 08:15:12.000000 BaseNN-0.1.6/BaseNN/load_data.py
+-rw-rw-r--   0 user      (1001) user      (1001)     1256 2023-05-31 09:49:28.000000 BaseNN-0.1.6/BaseNN/version.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-05-31 09:49:51.000000 BaseNN-0.1.6/BaseNN.egg-info/
+-rw-rw-r--   0 user      (1001) user      (1001)      346 2023-05-31 09:49:51.000000 BaseNN-0.1.6/BaseNN.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1001) user      (1001)      375 2023-05-31 09:49:51.000000 BaseNN-0.1.6/BaseNN.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1001) user      (1001)        1 2023-05-31 09:49:51.000000 BaseNN-0.1.6/BaseNN.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1001) user      (1001)       49 2023-05-31 09:49:51.000000 BaseNN-0.1.6/BaseNN.egg-info/entry_points.txt
+-rw-rw-r--   0 user      (1001) user      (1001)       80 2023-05-31 09:49:51.000000 BaseNN-0.1.6/BaseNN.egg-info/requires.txt
+-rw-rw-r--   0 user      (1001) user      (1001)        7 2023-05-31 09:49:51.000000 BaseNN-0.1.6/BaseNN.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1001) user      (1001)        1 2022-11-18 03:21:26.000000 BaseNN-0.1.6/BaseNN.egg-info/zip-safe
+-rw-rw-r--   0 user      (1001) user      (1001)      346 2023-05-31 09:49:51.000000 BaseNN-0.1.6/PKG-INFO
+-rw-rw-r--   0 user      (1001) user      (1001)       38 2023-05-31 09:49:51.000000 BaseNN-0.1.6/setup.cfg
+-rw-rw-r--   0 user      (1001) user      (1001)     3827 2023-05-31 09:49:24.000000 BaseNN-0.1.6/setup.py
```

### Comparing `BaseNN-0.1.5/BaseNN/BaseNN.py` & `BaseNN-0.1.6/BaseNN/BaseNN.py`

 * *Files 1% similar despite different names*

```diff
@@ -380,20 +380,20 @@
         self.img_classes = classes
         self.transform = transform
         if 0 < train_val_ratio < 1:
             train_size =  int(train_val_ratio * self.dataset_size)
             val_size =  self.dataset_size - train_size
 
             train_dataset, val_dataset = torch.utils.data.random_split(dataset, [train_size, val_size])
-            self.dataloader = DataLoader(train_dataset,batch_size=batch_size, shuffle=shuffle,num_workers=1)
-            self.val_dataloader = DataLoader(val_dataset,batch_size=batch_size, shuffle=shuffle,num_workers=1)
+            self.dataloader = DataLoader(train_dataset,batch_size=batch_size, shuffle=shuffle,num_workers=0)
+            self.val_dataloader = DataLoader(val_dataset,batch_size=batch_size, shuffle=shuffle,num_workers=0)
             return self.dataloader, self.val_dataloader
 
         else:
-            self.dataloader = DataLoader(dataset,batch_size=batch_size, shuffle=shuffle,num_workers=1)
+            self.dataloader = DataLoader(dataset,batch_size=batch_size, shuffle=shuffle,num_workers=0)
             self.label = torch.Tensor()
             for train_x, train_y in self.dataloader:
                 # test_x = test_x.to(self.device)
                 # test_y = test_y.to(self.device)
                 # batch_res = self.model(test_x)
                 self.label = torch.cat([self.label, train_y], dim=0)
             self.label = self.label.cpu().detach().numpy()
@@ -406,39 +406,39 @@
         # print(self.dataset_size)
         # self.dataloader = DataLoader(dataset,batch_size=batch_size, shuffle=shuffle,num_workers=1)
         if 0 < train_val_ratio < 1:
             train_size =  int(train_val_ratio * self.dataset_size)
             val_size =  self.dataset_size - train_size
 
             train_dataset, val_dataset = torch.utils.data.random_split(dataset, [train_size, val_size])
-            self.dataloader = DataLoader(train_dataset,batch_size=batch_size, shuffle=shuffle,num_workers=1)
-            self.val_dataloader = DataLoader(val_dataset,batch_size=batch_size, shuffle=shuffle,num_workers=1)
+            self.dataloader = DataLoader(train_dataset,batch_size=batch_size, shuffle=shuffle,num_workers=0)
+            self.val_dataloader = DataLoader(val_dataset,batch_size=batch_size, shuffle=shuffle,num_workers=0)
             return self.dataloader, self.val_dataloader
         else:
-            self.dataloader = DataLoader(dataset,batch_size=batch_size, shuffle=shuffle,num_workers=1)
+            self.dataloader = DataLoader(dataset,batch_size=batch_size, shuffle=shuffle,num_workers=0,pin_memory=True)
 
             return self.dataloader
 
     def load_npz_data(self, data_path, batch_size=32, shuffle=True, classes=None,train_val_ratio=1.0):
         from .load_data import NpzDataset
         dataset = NpzDataset(data_path)
         self.dataset_size = int(len(dataset))
         self.img_classes = classes
 
         # print(self.dataset_size)
-        self.dataloader = DataLoader(dataset,batch_size=batch_size, shuffle=shuffle,num_workers=1)
+        # self.dataloader = DataLoader(dataset,batch_size=batch_size, shuffle=shuffle,num_workers=1)
         if 0 < train_val_ratio < 1:
             train_size =  int(train_val_ratio * self.dataset_size)
             val_size =  self.dataset_size - train_size
 
             train_dataset, val_dataset = torch.utils.data.random_split(dataset, [train_size, val_size])
-            self.dataloader = DataLoader(train_dataset,batch_size=batch_size, shuffle=shuffle,num_workers=1)
-            self.val_dataloader = DataLoader(val_dataset,batch_size=batch_size, shuffle=shuffle,num_workers=1)
+            self.dataloader = DataLoader(train_dataset,batch_size=batch_size, shuffle=shuffle,num_workers=0)
+            self.val_dataloader = DataLoader(val_dataset,batch_size=batch_size, shuffle=shuffle,num_workers=0)
         else:
-            self.dataloader = DataLoader(dataset,batch_size=batch_size, shuffle=shuffle,num_workers=1)
+            self.dataloader = DataLoader(dataset,batch_size=batch_size, shuffle=shuffle,num_workers=0)
         return self.dataloader
 
     # def load_dataset(self, data_path, batch_size=32,shuffle=True,batch_mode=False,label_column=-1,transform=None,color="RGB",**kw ):
         # from .load_data import ImageFolderDataset
         # from torch.utils.data import DataLoader
 
         # if data_type == 'tabular':
@@ -613,14 +613,16 @@
             # scheduler = torch.optim.lr_scheduler.ReduceLROnPlateau(optimizer, mode='min', factor=0.1, patience=10,verbose=False, threshold=0.0001, threshold_mode='rel', cooldown=0, min_lr=0, eps=1e-08)
             self.model.to(self.device)
             log = []
             for epoch in range(epochs):  
                 # b_loss = 0
                 # b_acc = 0
                 for batch_x, batch_y in self.loader:
+                    # a = time.time()
+                    # print("1", a)
                     # print("iter ", iter, np.squeeze(batch_x[0]).shape, batch_y[0])
                     # import cv2
                     # cv2.imshow("asd", np.array(np.squeeze(batch_x[0])))
                     # print("batch_y[0]",np.squeeze(batch_y[0]))
                     # y_pred = self.model(self.x)
                     batch_x = batch_x.to(self.device)
                     batch_y = batch_y.to(self.device)
@@ -631,14 +633,16 @@
                     # print(batch_y[0],y_pred[0])
                     # cv2.waitKey(0)
 
                     loss = loss_fun(y_pred, batch_y)
                     loss.backward()  # 反向传播，计算当前梯度
                     optimizer.step()  # 根据梯度更新网络参数\
                     # scheduler.step()
+                    # print("2", a - time.time())
+
                     log_info = "{epoch:%d  Loss:%.4f}" % (epoch, loss)
                     log_dict = {"epoch":epoch, "loss":loss.item()}
                     if "acc" in metrics:
                         acc = cal_accuracy(batch_y, y_pred)
                         log_info = log_info[:-1] # 去掉句末大括号
                         log_info+= "  Accuracy:%.4f}"%acc # 加入acc信息
                         log_dict['acc'] = acc
@@ -654,14 +658,15 @@
                         log_info = log_info[:-1] # 去掉句末大括号
                         log_info+= "  MSE:%.4f}"%mse # 加入acc信息
                         log_dict['mse'] = mse
                     print(log_info)
                     log.append(log_dict)
                     # b_acc += acc
                     # b_loss+= loss
+
                 # step+=1
                 # print("{epoch:%d  Loss:%.4f  Accuracy:%.4f}" % (epoch, b_loss/step, b_acc/step),step)
 
             if save_fold:
                 self.save_fold = save_fold
                 # print(self.save_fold)
             if not os.path.exists(self.save_fold):
```

### Comparing `BaseNN-0.1.5/BaseNN/examples/BaseNN_demo.py` & `BaseNN-0.1.6/BaseNN/examples/BaseNN_demo.py`

 * *Files 1% similar despite different names*

```diff
@@ -378,36 +378,40 @@
     # print(y[1000:1100])
     a = "/home/user/桌面/BaseNN004/dataset/cls/cats_dogs_dataset/CatsDogs (1)/CatsDogs/val_set/dog"
     b = "/home/user/桌面/BaseNN004/dataset/cls/cats_dogs_dataset/CatsDogs (1)/CatsDogs/val_set/dog/dog0.jpg"
     result = model.inference(data=b, checkpoint="new_cd_ckpt/basenn.pth")
     model.print_result()
 
 def load_tab_data_iris():
+    import time
     model = nn()
     # 训练数据
     train_path = '../../dataset/iris/iris_training.csv'
     # x = np.loadtxt(train_path, dtype=float, delimiter=',',skiprows=1,usecols=range(0,4)) # [120, 4]
     # y = np.loadtxt(train_path, dtype=int, delimiter=',',skiprows=1,usecols=4)
-    train,val = model.load_tab_data(train_path, batch_size=2,train_val_ratio=0.8)
+    model.load_tab_data(train_path, batch_size=200000)
     # for x, y in dl:
     #     print(x,y)
 
-    # model.add(layer='Linear',size=(4, 10),activation='ReLU') # [120, 10]
-    # model.add(layer='Linear',size=(10, 5), activation='ReLU') # [120, 5]
-    # model.add(layer='Linear', size=(5, 3), activation='Softmax') # [120, 3]
-    # model.save_fold = 'iris_ckpt'
-    # model.train(lr=0.01, epochs=500)
+    model.add(layer='Linear',size=(4, 10),activation='ReLU') # [120, 10]
+    model.add(layer='Linear',size=(10, 5), activation='ReLU') # [120, 5]
+    model.add(layer='Linear', size=(5, 3), activation='Softmax') # [120, 3]
+    model.save_fold = 'iris_ckpt'
+    a = time.time()
+    model.train(lr=0.01, epochs=100)
+    print(time.time() - a)
+    print(model.device)
     # model.print_model()
     # test_path = '../../dataset/iris/iris_test.csv'
     # x = np.loadtxt(test_path, dtype=float, delimiter=',',skiprows=1,usecols=range(0,4)) # [120, 4]
     # y = np.loadtxt(test_path, dtype=int, delimiter=',',skiprows=1,usecols=4)
-    # print(y)
-    res = model.inference(val,label=True, checkpoint="iris_ckpt/basenn.pth")
-    model.print_result(res)
-    print(model.val_label)
+    # # print(y)
+    # res = model.inference(val,label=True, checkpoint="iris_ckpt/basenn.pth")
+    # model.print_result(res)
+    # print(model.val_label)
 
 def load_npz_data_action():
     # 读取数据
     X = np.load("/home/user/桌面/BaseNN004/BaseNN/examples/human_action_recognition-main/X1.npy",allow_pickle = True)
     y = np.load("/home/user/桌面/BaseNN004/BaseNN/examples/human_action_recognition-main/y1.npy", allow_pickle = True)    
     X = np.load("./conbined.npz")["data"]
 
@@ -460,11 +464,11 @@
     # visual_feature_demo()
     # extract_feature_demo()
 
     # lstm_train_demo()
     # pth_info('model_lstm.pth')
     # lstm_infer_demo()
 
-    load_image_data_mn()
+    # load_image_data_mn()
     # load_image_data_cd()
-    # load_tab_data_iris()
+    load_tab_data_iris()
     # load_npz_data_action()
```

### Comparing `BaseNN-0.1.5/BaseNN/examples/pkl2pth.py` & `BaseNN-0.1.6/BaseNN/examples/pkl2pth.py`

 * *Files identical despite different names*

### Comparing `BaseNN-0.1.5/BaseNN/load_data.py` & `BaseNN-0.1.6/BaseNN/load_data.py`

 * *Files identical despite different names*

### Comparing `BaseNN-0.1.5/BaseNN/version.py` & `BaseNN-0.1.6/BaseNN/version.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 
-__version__='0.1.5'
+__version__='0.1.6'
 __path__=os.path.abspath(os.getcwd())
 
 def parse_version_info(version_str):
     version_info = []
     for x in version_str.split('.'):
         if x.isdigit():
             version_info.append(int(x))
```

### Comparing `BaseNN-0.1.5/setup.py` & `BaseNN-0.1.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 
     packages = list(gen_packages_items())
     return packages
 
 
 setup(
     name='BaseNN',
-    version='0.1.5',
+    version='0.1.6',
     description='BaseNN can easily build neural networks layer by layer and deeply explore the neural network principle.',
     license='MIT License',
     author='OpenXLab',
     author_email='wangbolun@pjlab.org.cn',
     url='https://github.com/OpenXLab-Edu/OpenMMLab-Edu',
     packages=find_packages(),
     include_package_data=True,
```

