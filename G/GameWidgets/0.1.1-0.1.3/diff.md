# Comparing `tmp/GameWidgets-0.1.1.tar.gz` & `tmp/GameWidgets-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GameWidgets-0.1.1.tar", last modified: Fri Sep 23 23:25:30 2022, max compression
+gzip compressed data, was "GameWidgets-0.1.3.tar", last modified: Wed May 31 01:46:19 2023, max compression
```

## Comparing `GameWidgets-0.1.1.tar` & `GameWidgets-0.1.3.tar`

### file list

```diff
@@ -1,38 +1,49 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2022-09-23 23:25:30.521741 GameWidgets-0.1.1/
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2022-09-23 23:25:30.513741 GameWidgets-0.1.1/GameWidgets/
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2022-09-23 23:25:30.517741 GameWidgets-0.1.1/GameWidgets/GameWidgets/
--rw-------   0 runner    (1000) runner    (1000)     1421 2022-09-11 20:52:52.000000 GameWidgets-0.1.1/GameWidgets/GameWidgets/Animatrix.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2022-09-23 23:25:30.517741 GameWidgets-0.1.1/GameWidgets/GameWidgets/Controller/
--rw-------   0 runner    (1000) runner    (1000)       13 2022-09-11 20:52:52.000000 GameWidgets-0.1.1/GameWidgets/GameWidgets/Controller/Hat.py
--rw-------   0 runner    (1000) runner    (1000)     1404 2022-09-11 20:52:52.000000 GameWidgets-0.1.1/GameWidgets/GameWidgets/Controller/Joystick.py
--rw-------   0 runner    (1000) runner    (1000)       13 2022-09-11 20:52:52.000000 GameWidgets-0.1.1/GameWidgets/GameWidgets/Controller/R1_R2.py
--rw-------   0 runner    (1000) runner    (1000)      145 2022-09-11 20:52:52.000000 GameWidgets-0.1.1/GameWidgets/GameWidgets/Controller/__init__.py
--rw-------   0 runner    (1000) runner    (1000)      735 2022-09-11 20:52:52.000000 GameWidgets-0.1.1/GameWidgets/GameWidgets/Draw.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2022-09-23 23:25:30.517741 GameWidgets-0.1.1/GameWidgets/GameWidgets/TileMaps/
--rw-------   0 runner    (1000) runner    (1000)      569 2022-09-11 20:52:52.000000 GameWidgets-0.1.1/GameWidgets/GameWidgets/TileMaps/Sprite.py
--rw-------   0 runner    (1000) runner    (1000)      703 2022-09-22 23:13:44.000000 GameWidgets-0.1.1/GameWidgets/GameWidgets/TileMaps/Tile.py
--rw-------   0 runner    (1000) runner    (1000)      124 2022-09-11 20:52:52.000000 GameWidgets-0.1.1/GameWidgets/GameWidgets/TileMaps/__init__.py
--rw-------   0 runner    (1000) runner    (1000)      121 2022-09-11 20:52:52.000000 GameWidgets-0.1.1/GameWidgets/GameWidgets/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2022-09-23 23:25:30.517741 GameWidgets-0.1.1/GameWidgets/SetUp/
--rw-------   0 runner    (1000) runner    (1000)     1449 2022-09-11 20:52:52.000000 GameWidgets-0.1.1/GameWidgets/SetUp/ScreenCommands.py
--rw-------   0 runner    (1000) runner    (1000)      109 2022-09-11 20:52:52.000000 GameWidgets-0.1.1/GameWidgets/SetUp/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2022-09-23 23:25:30.521741 GameWidgets-0.1.1/GameWidgets/Widgets/
--rw-------   0 runner    (1000) runner    (1000)     2989 2022-09-23 23:24:26.000000 GameWidgets-0.1.1/GameWidgets/Widgets/Btn.py
--rw-------   0 runner    (1000) runner    (1000)      626 2022-09-11 20:52:52.000000 GameWidgets-0.1.1/GameWidgets/Widgets/Clock.py
--rw-------   0 runner    (1000) runner    (1000)     3644 2022-09-11 20:52:52.000000 GameWidgets-0.1.1/GameWidgets/Widgets/Colors.py
--rw-------   0 runner    (1000) runner    (1000)     1039 2022-09-11 20:52:52.000000 GameWidgets-0.1.1/GameWidgets/Widgets/Cursor.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2761 2022-09-23 00:16:45.000000 GameWidgets-0.1.1/GameWidgets/Widgets/DialogeBox.py
--rw-r--r--   0 runner    (1000) runner    (1000)      718 2022-09-17 03:23:10.000000 GameWidgets-0.1.1/GameWidgets/Widgets/ScreenSlide.py
--rw-------   0 runner    (1000) runner    (1000)      246 2022-09-11 20:52:52.000000 GameWidgets-0.1.1/GameWidgets/Widgets/Sound.py
--rw-------   0 runner    (1000) runner    (1000)      152 2022-09-22 23:47:55.000000 GameWidgets-0.1.1/GameWidgets/Widgets/__init__.py
--rw-------   0 runner    (1000) runner    (1000)      614 2022-09-23 00:30:55.000000 GameWidgets-0.1.1/GameWidgets/__init__.py
--rw-------   0 runner    (1000) runner    (1000)      544 2022-09-23 23:25:02.000000 GameWidgets-0.1.1/GameWidgets/setup.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2022-09-23 23:25:30.513741 GameWidgets-0.1.1/GameWidgets.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)      709 2022-09-23 23:25:30.000000 GameWidgets-0.1.1/GameWidgets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      959 2022-09-23 23:25:30.000000 GameWidgets-0.1.1/GameWidgets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2022-09-23 23:25:30.000000 GameWidgets-0.1.1/GameWidgets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        7 2022-09-23 23:25:30.000000 GameWidgets-0.1.1/GameWidgets.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       12 2022-09-23 23:25:30.000000 GameWidgets-0.1.1/GameWidgets.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      709 2022-09-23 23:25:30.521741 GameWidgets-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      385 2022-09-11 21:19:38.000000 GameWidgets-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2022-09-23 23:25:30.521741 GameWidgets-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-31 01:46:19.313480 GameWidgets-0.1.3/
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-31 01:46:19.289480 GameWidgets-0.1.3/GameWidgets/
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-31 01:46:19.301479 GameWidgets-0.1.3/GameWidgets/Examples/
+-rw-------   0 runner    (1000) runner    (1000)     1864 2023-05-31 01:38:09.000000 GameWidgets-0.1.3/GameWidgets/Examples/Widget_Screen_GameWidgets_Example.py
+-rw-------   0 runner    (1000) runner    (1000)        4 2023-05-31 01:38:09.000000 GameWidgets-0.1.3/GameWidgets/Examples/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-31 01:46:19.301479 GameWidgets-0.1.3/GameWidgets/GameWidgets/
+-rw-------   0 runner    (1000) runner    (1000)     1422 2023-05-31 01:38:09.000000 GameWidgets-0.1.3/GameWidgets/GameWidgets/Animatrix.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-31 01:46:19.305480 GameWidgets-0.1.3/GameWidgets/GameWidgets/Controller/
+-rw-------   0 runner    (1000) runner    (1000)     1497 2023-05-31 01:38:09.000000 GameWidgets-0.1.3/GameWidgets/GameWidgets/Controller/Button.py
+-rw-------   0 runner    (1000) runner    (1000)     1404 2023-05-31 01:38:09.000000 GameWidgets-0.1.3/GameWidgets/GameWidgets/Controller/Joystick.py
+-rw-------   0 runner    (1000) runner    (1000)       13 2023-05-31 01:38:09.000000 GameWidgets-0.1.3/GameWidgets/GameWidgets/Controller/R1_R2.py
+-rw-------   0 runner    (1000) runner    (1000)      148 2023-05-31 01:38:09.000000 GameWidgets-0.1.3/GameWidgets/GameWidgets/Controller/__init__.py
+-rw-------   0 runner    (1000) runner    (1000)      735 2023-05-31 01:38:09.000000 GameWidgets-0.1.3/GameWidgets/GameWidgets/Draw.py
+-rw-------   0 runner    (1000) runner    (1000)      652 2023-05-31 01:38:09.000000 GameWidgets-0.1.3/GameWidgets/GameWidgets/ScreenSlide.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-31 01:46:19.305480 GameWidgets-0.1.3/GameWidgets/GameWidgets/TileMaps/
+-rw-------   0 runner    (1000) runner    (1000)      569 2023-05-31 01:38:09.000000 GameWidgets-0.1.3/GameWidgets/GameWidgets/TileMaps/Sprite.py
+-rw-------   0 runner    (1000) runner    (1000)      703 2023-05-31 01:38:09.000000 GameWidgets-0.1.3/GameWidgets/GameWidgets/TileMaps/Tile.py
+-rw-------   0 runner    (1000) runner    (1000)      124 2023-05-31 01:38:09.000000 GameWidgets-0.1.3/GameWidgets/GameWidgets/TileMaps/__init__.py
+-rw-------   0 runner    (1000) runner    (1000)      121 2023-05-31 01:38:09.000000 GameWidgets-0.1.3/GameWidgets/GameWidgets/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-31 01:46:19.309480 GameWidgets-0.1.3/GameWidgets/RuntimeTests/
+-rw-------   0 runner    (1000) runner    (1000)      649 2023-05-31 01:38:09.000000 GameWidgets-0.1.3/GameWidgets/RuntimeTests/AllTest.py
+-rw-------   0 runner    (1000) runner    (1000)      397 2023-05-31 01:38:09.000000 GameWidgets-0.1.3/GameWidgets/RuntimeTests/GameWidgetTest.py
+-rw-------   0 runner    (1000) runner    (1000)      359 2023-05-31 01:38:09.000000 GameWidgets-0.1.3/GameWidgets/RuntimeTests/SetUpTest.py
+-rw-------   0 runner    (1000) runner    (1000)      369 2023-05-31 01:38:09.000000 GameWidgets-0.1.3/GameWidgets/RuntimeTests/WidgetTest.py
+-rw-------   0 runner    (1000) runner    (1000)        4 2023-05-31 01:38:09.000000 GameWidgets-0.1.3/GameWidgets/RuntimeTests/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-31 01:46:19.309480 GameWidgets-0.1.3/GameWidgets/SetUp/
+-rw-------   0 runner    (1000) runner    (1000)     1689 2023-05-31 01:38:09.000000 GameWidgets-0.1.3/GameWidgets/SetUp/ScreenCommands.py
+-rw-------   0 runner    (1000) runner    (1000)      109 2023-05-31 01:38:09.000000 GameWidgets-0.1.3/GameWidgets/SetUp/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-31 01:46:19.313480 GameWidgets-0.1.3/GameWidgets/Widgets/
+-rw-------   0 runner    (1000) runner    (1000)     2980 2023-05-31 01:38:09.000000 GameWidgets-0.1.3/GameWidgets/Widgets/Btn.py
+-rw-------   0 runner    (1000) runner    (1000)      597 2023-05-31 01:38:09.000000 GameWidgets-0.1.3/GameWidgets/Widgets/Clock.py
+-rw-------   0 runner    (1000) runner    (1000)     3643 2023-05-31 01:38:09.000000 GameWidgets-0.1.3/GameWidgets/Widgets/Colors.py
+-rw-------   0 runner    (1000) runner    (1000)     1522 2023-05-31 01:38:09.000000 GameWidgets-0.1.3/GameWidgets/Widgets/Cursor.py
+-rw-------   0 runner    (1000) runner    (1000)     2761 2023-05-31 01:38:09.000000 GameWidgets-0.1.3/GameWidgets/Widgets/DialogeBox.py
+-rw-------   0 runner    (1000) runner    (1000)     1574 2023-05-31 01:38:09.000000 GameWidgets-0.1.3/GameWidgets/Widgets/ImgDecoder.py
+-rw-------   0 runner    (1000) runner    (1000)      246 2023-05-31 01:38:09.000000 GameWidgets-0.1.3/GameWidgets/Widgets/Sound.py
+-rw-------   0 runner    (1000) runner    (1000)     1914 2023-05-31 01:38:09.000000 GameWidgets-0.1.3/GameWidgets/Widgets/TextInp.py
+-rw-------   0 runner    (1000) runner    (1000)      159 2023-05-31 01:38:09.000000 GameWidgets-0.1.3/GameWidgets/Widgets/__init__.py
+-rw-------   0 runner    (1000) runner    (1000)      620 2023-05-31 01:38:09.000000 GameWidgets-0.1.3/GameWidgets/__init__.py
+-rw-------   0 runner    (1000) runner    (1000)      558 2023-05-31 01:45:49.000000 GameWidgets-0.1.3/GameWidgets/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-31 01:46:19.297479 GameWidgets-0.1.3/GameWidgets.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)      580 2023-05-31 01:46:19.000000 GameWidgets-0.1.3/GameWidgets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     1315 2023-05-31 01:46:19.000000 GameWidgets-0.1.3/GameWidgets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-05-31 01:46:19.000000 GameWidgets-0.1.3/GameWidgets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        7 2023-05-31 01:46:19.000000 GameWidgets-0.1.3/GameWidgets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       12 2023-05-31 01:46:19.000000 GameWidgets-0.1.3/GameWidgets.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      580 2023-05-31 01:46:19.313480 GameWidgets-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      385 2022-09-11 21:19:38.000000 GameWidgets-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-05-31 01:46:19.313480 GameWidgets-0.1.3/setup.cfg
```

### Comparing `GameWidgets-0.1.1/GameWidgets/GameWidgets/Animatrix.py` & `GameWidgets-0.1.3/GameWidgets/GameWidgets/Animatrix.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pygame
 import time
 class Animation:
-    def __init__(self,screen,Location=(0,0),Pictures=(),S_Per_Frame=0.1,FSize=()):
+    def __init__(self,screen,Location=(0,0),Pictures=(),S_Per_Frame=1000,FSize=()):
         self.S=screen
         #self.loc=Location
         self.rects=[]
         self.images=[]
         iteration=0
         for path in Pictures:
             image=pygame.image.load(path)
```

### Comparing `GameWidgets-0.1.1/GameWidgets/GameWidgets/Controller/Joystick.py` & `GameWidgets-0.1.3/GameWidgets/GameWidgets/Controller/Joystick.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.1/GameWidgets/GameWidgets/Draw.py` & `GameWidgets-0.1.3/GameWidgets/GameWidgets/Draw.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.1/GameWidgets/GameWidgets/TileMaps/Sprite.py` & `GameWidgets-0.1.3/GameWidgets/GameWidgets/TileMaps/Sprite.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.1/GameWidgets/GameWidgets/TileMaps/Tile.py` & `GameWidgets-0.1.3/GameWidgets/GameWidgets/TileMaps/Tile.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.1/GameWidgets/SetUp/ScreenCommands.py` & `GameWidgets-0.1.3/GameWidgets/SetUp/ScreenCommands.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,44 +3,50 @@
 class Screen:
     def __init__(self,**kwarg):
         self.Color=(0,0,0)
         self.Xsize=500
         self.Ysize=500
         self.Icon=''
         self.Title='    Pygame Window'
+        self.resizable = False
         for key,val in kwarg.items():
             if key=='Color':
                 self.Color=val
             elif key=='Xsize':
                 self.Xsize=val
             elif key=='Ysize':
                 self.Ysize=val
             elif key=='Icon':
                 self.Icon=val
             elif key=='Title':
                 self.Title=val
+            elif key=='Resizable':
+                self.resizable = True
             else:
                 print(f'Value Error! No Attribute to {key}')
                 quit()
         self.Master=None
         if self.Icon=='':
             self.img=pygame.Surface((100,100))
             self.img.fill((0,0,0))
         else:
             self.img=pygame.image.load(self.Icon)
         
     def Return(self):
-        return pygame.display.set_mode((self.Xsize,self.Ysize))
+        if self.resizable!=True:
+            return pygame.display.set_mode((self.Xsize,self.Ysize))
+        else:
+            return pygame.display.set_mode((self.Xsize,self.Ysize),pygame.RESIZABLE)
     def Register_Master(self,master):
         self.Master=master
     def Return_HW(self,Type='List'):
         if Type=='List':
             return [self.Xsize,self.Ysize]
         if Type=='Dictionary':
-            return {'Hieght':self.Xsize,'Width':self.Ysize}
+            return {'Height':self.Xsize,'Width':self.Ysize}
         if Type=='Tuple':
             return (self.Xsize,self.Ysize)
     def Fill(self):
         self.Master.fill(self.Color)
     def Set_Icon(self):
         pygame.display.set_icon(self.img)
         pygame.display.set_caption(self.Title)
```

### Comparing `GameWidgets-0.1.1/GameWidgets/Widgets/Btn.py` & `GameWidgets-0.1.3/GameWidgets/Widgets/Btn.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import pygame
 pygame.init()
 class Normal_Btn:
-    def __init__(self,screen,fgcolor=(255,255,255),xy=(0,0),font='freesansbold.ttf',size=20,text='Custom Button',Outline=(255,255,255),Thickness=5):
+    def __init__(self,screen,fgcolor=(255,255,255),xy=(0,0),font='freesansbold.ttf',size=20,text='Normal Btn',Outline=(255,255,255),Thickness=5):
         self.screen=screen
-        self.BG=(0,255,0)
+        self.BG=(0,0,0)
         self.FG=fgcolor
         self.xy=xy
         self.size=size
         self.font=font
         self.text=text
         self.TH=Thickness
         TextFont=pygame.font.SysFont(self.font,self.size)
         self.text=TextFont.render(self.text,self.BG,self.FG)
         self.ROutline=self.text.get_rect(topleft=self.xy)
         self.COutline=Outline
         
     def Draw(self):
+        pygame.draw.rect(self.screen, self.COutline, self.ROutline, self.TH)
         self.screen.blit(self.text,self.xy)
-        pygame.draw.rect(self.screen,self.COutline,self.ROutline,self.TH)
     def Detect(self,mousexy,event):
         x=mousexy[0]
         y=mousexy[1]
         if ((x>=self.ROutline.topleft[0]) and (x<=self.ROutline.bottomright[0])) and ((y>=self.ROutline.topleft[1]) and (y<=self.ROutline.bottomright[1])):
             
             if event.type==pygame.MOUSEBUTTONDOWN:
                 return True
@@ -55,15 +55,15 @@
                 self.x=val
             elif key=='Y':
                 self.y=val
             else:
                 print('Btn.py')
                 print(f'Value Error! No Attribute to {key}')
         self.font=pygame.font.SysFont(self.font,self.size)
-        self.label=self.font.render(self.text,self.Colors[3],self.Colors[4])
+        self.label=self.font.render(self.text,(0,0,0),self.Colors[3])
         self.rect=self.label.get_rect(topleft=(self.x,self.y))
         self.surf=pygame.Surface((self.rect.width,self.rect.height))
         self.state=0
         self.screen=screen
     def Detect(self,mousexy,event):
         x=mousexy[0]
         y=mousexy[1]
```

### Comparing `GameWidgets-0.1.1/GameWidgets/Widgets/Clock.py` & `GameWidgets-0.1.3/GameWidgets/Widgets/Clock.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import pygame
 pygame.init()
 class Clock:
     def __init__(self,FPS=60):
         self.FPS=FPS
-    def Set_Up_Clock(self):
-        self.clock=pygame.time.Clock()
-    def Set_FPS(self):
+        self.clock = pygame.time.Clock()
+    def Tick(self):
         self.clock.tick(self.FPS)
     def Set_Delay(self,TIME=1,**kwarg):
         time=TIME
         Unit=1
         for key,val in kwarg.items():
             if key=='Milli':
                 Unit=1000
```

### Comparing `GameWidgets-0.1.1/GameWidgets/Widgets/Colors.py` & `GameWidgets-0.1.3/GameWidgets/Widgets/Colors.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -148,8 +148,8 @@
 dim_gray_dim_grey=(105,105,105)
 gray_grey=(128,128,128)
 dark_gray_dark_grey=(169,169,169)
 silver=(192,192,192)
 light_gray_light_grey=(211,211,211)
 gainsboro=(220,220,220)
 white_smoke=(245,245,245)
-white=(255,255,255)
+white=(255,255,255)
```

### Comparing `GameWidgets-0.1.1/GameWidgets/Widgets/DialogeBox.py` & `GameWidgets-0.1.3/GameWidgets/Widgets/DialogeBox.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.1/GameWidgets/Widgets/ScreenSlide.py` & `GameWidgets-0.1.3/GameWidgets/GameWidgets/ScreenSlide.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import pygame
 pygame.init()
 class Slide:
-    def __init__(self,screen,Color=(0,0,0),Vertical=(0,500),Horizontal=-500,Per_Frame=2,Width=500,height=600):
+    def __init__(self,screen,Color=(0,0,0),y=0,x=-500,Per_Frame=2,Width=500,height=600):
         self.screen=screen
         self.Color=Color
-        self.Vertical=Vertical
-        self.Horizontal=Horizontal
+        self.Vertical=y
+        self.Horizontal=x
         self.PF=Per_Frame
         self.Width=Width
         self.height=height
-        self.rect=pygame.Rect(self.Horizontal,self.Vertical[0],self.Width,self.Vertical[0]-self.Vertical[1])
+        self.rect=pygame.Rect(self.Horizontal,self.Vertical,self.Width,self.height)
         
     def Update(self):
         #print(self.Horizontal)
         self.Horizontal+=self.PF
-        self.rect=pygame.Rect(self.Horizontal,self.Vertical[0],self.Width,self.height)
+        self.rect=pygame.Rect(self.Horizontal,self.Vertical,self.Width,self.height)
     def Draw(self):
         pygame.draw.rect(self.screen,self.Color,self.rect)
```

### Comparing `GameWidgets-0.1.1/GameWidgets/__init__.py` & `GameWidgets-0.1.3/GameWidgets/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-try:
+'''try:
     from GameWidgets.Widgets import *
 except:
     print('GameWidgets.Widgets File has been edited, moved, or deleted')
 try:
     from GameWidgets.GameWidgets import *
 except:
     print('GameWidgets.GameWidgets File has been edited, moved, or deleted')
 try:
     from GameWidgets.SetUp import *
 except:
-    print('GameWidgets.SetUp File has been edited, moved, or deleted')
+    print('GameWidgets.SetUp File has been edited, moved, or deleted')'''
 print('GameWidgets Active!')
 __author__='Manomay Tyagi'
 __credits__='Tyagi Family'
-__Widgets__='''Automatic Import:
+'''__Widgets__=Automatic Import:
 Btn
 Clock
 Colors
 Sound
 Cursor
 DialogeBox
 ScreenCommands
```

### Comparing `GameWidgets-0.1.1/GameWidgets/setup.py` & `GameWidgets-0.1.3/GameWidgets/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
   
 with open("GameWidgets/README.md", "r") as fh:
     description = fh.read()
   
 setup(
     name="GameWidgets",
-    version="0.1.1",
+    version="0.1.3",
     author="Manomay tyagi",
     author_email="tyagimanomay57@gmail.com",
-    description="Pygame becomes easier",
+    description="Make Games Easier with GameWidgets ",
     long_description=description,
     long_description_content_type="text/markdown",
     url="https://github.com/SuperGuy123456/GameWidgets",
     license='MIT',
     python_requires='>=3.8',
     install_requires=['pygame'],
     packages=find_packages()
```

### Comparing `GameWidgets-0.1.1/GameWidgets.egg-info/SOURCES.txt` & `GameWidgets-0.1.3/GameWidgets.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -2,27 +2,36 @@
 GameWidgets/__init__.py
 GameWidgets/setup.py
 GameWidgets.egg-info/PKG-INFO
 GameWidgets.egg-info/SOURCES.txt
 GameWidgets.egg-info/dependency_links.txt
 GameWidgets.egg-info/requires.txt
 GameWidgets.egg-info/top_level.txt
+GameWidgets/Examples/Widget_Screen_GameWidgets_Example.py
+GameWidgets/Examples/__init__.py
 GameWidgets/GameWidgets/Animatrix.py
 GameWidgets/GameWidgets/Draw.py
+GameWidgets/GameWidgets/ScreenSlide.py
 GameWidgets/GameWidgets/__init__.py
-GameWidgets/GameWidgets/Controller/Hat.py
+GameWidgets/GameWidgets/Controller/Button.py
 GameWidgets/GameWidgets/Controller/Joystick.py
 GameWidgets/GameWidgets/Controller/R1_R2.py
 GameWidgets/GameWidgets/Controller/__init__.py
 GameWidgets/GameWidgets/TileMaps/Sprite.py
 GameWidgets/GameWidgets/TileMaps/Tile.py
 GameWidgets/GameWidgets/TileMaps/__init__.py
+GameWidgets/RuntimeTests/AllTest.py
+GameWidgets/RuntimeTests/GameWidgetTest.py
+GameWidgets/RuntimeTests/SetUpTest.py
+GameWidgets/RuntimeTests/WidgetTest.py
+GameWidgets/RuntimeTests/__init__.py
 GameWidgets/SetUp/ScreenCommands.py
 GameWidgets/SetUp/__init__.py
 GameWidgets/Widgets/Btn.py
 GameWidgets/Widgets/Clock.py
 GameWidgets/Widgets/Colors.py
 GameWidgets/Widgets/Cursor.py
 GameWidgets/Widgets/DialogeBox.py
-GameWidgets/Widgets/ScreenSlide.py
+GameWidgets/Widgets/ImgDecoder.py
 GameWidgets/Widgets/Sound.py
+GameWidgets/Widgets/TextInp.py
 GameWidgets/Widgets/__init__.py
```

