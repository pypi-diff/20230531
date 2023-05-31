# Comparing `tmp/lifetimefitting-0.0.20.tar.gz` & `tmp/lifetimefitting-0.0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lifetimefitting-0.0.20.tar", last modified: Sun May 28 14:58:51 2023, max compression
+gzip compressed data, was "lifetimefitting-0.0.21.tar", last modified: Wed May 31 01:00:00 2023, max compression
```

## Comparing `lifetimefitting-0.0.20.tar` & `lifetimefitting-0.0.21.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:58:51.078610 lifetimefitting-0.0.20/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-28 14:58:37.000000 lifetimefitting-0.0.20/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-28 14:58:51.078610 lifetimefitting-0.0.20/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-05-28 14:58:37.000000 lifetimefitting-0.0.20/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:58:51.074610 lifetimefitting-0.0.20/app/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:58:51.078610 lifetimefitting-0.0.20/app/funcs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 14:58:37.000000 lifetimefitting-0.0.20/app/funcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-05-28 14:58:37.000000 lifetimefitting-0.0.20/app/funcs/expFuncs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7060 2023-05-28 14:58:37.000000 lifetimefitting-0.0.20/app/funcs/fittingFuncs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12992 2023-05-28 14:58:37.000000 lifetimefitting-0.0.20/app/funcs/gui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:58:51.078610 lifetimefitting-0.0.20/app/lifetimefitting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 14:58:37.000000 lifetimefitting-0.0.20/app/lifetimefitting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-05-28 14:58:37.000000 lifetimefitting-0.0.20/app/lifetimefitting/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:58:51.078610 lifetimefitting-0.0.20/app/lifetimefitting.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-28 14:58:51.000000 lifetimefitting-0.0.20/app/lifetimefitting.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-28 14:58:51.000000 lifetimefitting-0.0.20/app/lifetimefitting.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 14:58:51.000000 lifetimefitting-0.0.20/app/lifetimefitting.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-28 14:58:51.000000 lifetimefitting-0.0.20/app/lifetimefitting.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-28 14:58:51.000000 lifetimefitting-0.0.20/app/lifetimefitting.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 14:58:51.078610 lifetimefitting-0.0.20/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-28 14:58:37.000000 lifetimefitting-0.0.20/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 01:00:00.218952 lifetimefitting-0.0.21/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-31 00:59:44.000000 lifetimefitting-0.0.21/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-31 01:00:00.218952 lifetimefitting-0.0.21/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-05-31 00:59:44.000000 lifetimefitting-0.0.21/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 01:00:00.214952 lifetimefitting-0.0.21/app/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 01:00:00.214952 lifetimefitting-0.0.21/app/lifetimefitting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 00:59:44.000000 lifetimefitting-0.0.21/app/lifetimefitting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-05-31 00:59:44.000000 lifetimefitting-0.0.21/app/lifetimefitting/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 01:00:00.218952 lifetimefitting-0.0.21/app/lifetimefitting/funcs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 00:59:44.000000 lifetimefitting-0.0.21/app/lifetimefitting/funcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-05-31 00:59:44.000000 lifetimefitting-0.0.21/app/lifetimefitting/funcs/expFuncs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7045 2023-05-31 00:59:44.000000 lifetimefitting-0.0.21/app/lifetimefitting/funcs/fittingFuncs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12705 2023-05-31 00:59:44.000000 lifetimefitting-0.0.21/app/lifetimefitting/funcs/gui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 01:00:00.218952 lifetimefitting-0.0.21/app/lifetimefitting.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-31 01:00:00.000000 lifetimefitting-0.0.21/app/lifetimefitting.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-31 01:00:00.000000 lifetimefitting-0.0.21/app/lifetimefitting.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 01:00:00.000000 lifetimefitting-0.0.21/app/lifetimefitting.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-31 01:00:00.000000 lifetimefitting-0.0.21/app/lifetimefitting.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-31 01:00:00.000000 lifetimefitting-0.0.21/app/lifetimefitting.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 01:00:00.218952 lifetimefitting-0.0.21/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-31 00:59:44.000000 lifetimefitting-0.0.21/setup.py
```

### Comparing `lifetimefitting-0.0.20/LICENSE.md` & `lifetimefitting-0.0.21/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lifetimefitting-0.0.20/PKG-INFO` & `lifetimefitting-0.0.21/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lifetimefitting
-Version: 0.0.20
+Version: 0.0.21
 Summary: PicoHarp TCSPC lifetime fitting tool
 Home-page: https://github.com/adreasnow/LifetimeFittingTool
 Author: Adrea Snow
 Author-email: adrea.snow@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lifetimefitting-0.0.20/README.md` & `lifetimefitting-0.0.21/README.md`

 * *Files identical despite different names*

### Comparing `lifetimefitting-0.0.20/app/funcs/expFuncs.py` & `lifetimefitting-0.0.21/app/lifetimefitting/funcs/expFuncs.py`

 * *Files identical despite different names*

### Comparing `lifetimefitting-0.0.20/app/funcs/fittingFuncs.py` & `lifetimefitting-0.0.21/app/lifetimefitting/funcs/fittingFuncs.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     minbounds = [max(y) - 500]
     maxbounds = [max(y) + 500]
 
     fitFunc = FLFuncList[expCount]
     if ui.logFit_widg.isChecked():
         y = np.log(y)
         fitFunc = FLLinFuncList[expCount]
- 
+
     for i in range(expCount):
         minbounds += [0,     0]
         maxbounds += [99999999, 1]
 
     popt, pcov = curve_fit(fitFunc, x, y,
                            bounds=(minbounds, maxbounds), 
                            # maxfev=maxIter,
@@ -61,15 +61,14 @@
                            )
 
     residual = np.sum(np.subtract(y, FLFuncList[expCount](x, *popt)))
 
     return popt, residual
 
 def fitFL(ui, plot=True, x_in=None, y_in=None, irf_in=None) -> None:
-    
     csv = 'x,y_lin,y_log\n'
     csvTail = '\n'
     outPrint = ''
     maxIter = ui.maxIter_widg.value()
     binSize = ui.binSize_widg.value()
     expCount = ui.expCount_widg.value()
 
@@ -194,15 +193,14 @@
         ui.axList += ui.ax1.plot(x_func, FLFuncList[expCount](x_func, *popt), 'k--', lw=1)
         ui.axList += ui.ax3.plot(x_func, FLFuncList[expCount](x_func, *popt), 'k--', lw=1)
 
         residualList = np.subtract(FLLinFuncList[expCount](x, *popt), np.log(y))
         ui.axList += [ui.ax2.scatter(x, residualList, s=0.1, c='b')]
         residualList = np.subtract(FLFuncList[expCount](x, *popt), y,)
         ui.axList += [ui.ax4.scatter(x, residualList, s=0.1, c='b')]
-        
 
         ui.canvas.draw()
         ui.text_output.setText(outPrint)
 
         for x, y_lin, y_log in zip(x_in, FLFuncList[expCount](x_raw, *popt), FLLinFuncList[expCount](x_raw, *popt)):
             csv += f'{x},{y_lin},{y_log}\n'
         csv += f'\n{csvTail}'
```

### Comparing `lifetimefitting-0.0.20/app/funcs/gui.py` & `lifetimefitting-0.0.21/app/lifetimefitting/funcs/gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from PyQt6 import QtCore, QtWidgets
+from PyQt6 import QtCore, QtGui, QtWidgets
 
 
 class Ui_Form(object):
     def setupUi(self, Form):
         Form.setObjectName("Form")
         Form.setEnabled(True)
         Form.resize(1024, 900)
@@ -117,28 +117,28 @@
         self.verticalLayout_5.addLayout(self.horizontalLayout)
         self.label_3 = QtWidgets.QLabel(parent=self.verticalGroupBox)
         self.label_3.setObjectName("label_3")
         self.verticalLayout_5.addWidget(self.label_3)
         self.horizontalLayout_6 = QtWidgets.QHBoxLayout()
         self.horizontalLayout_6.setObjectName("horizontalLayout_6")
         self.max_x = QtWidgets.QSlider(parent=self.verticalGroupBox)
-        self.max_x.setMaximum(500)
+        self.max_x.setMaximum(300)
         self.max_x.setProperty("value", 20)
         self.max_x.setSliderPosition(20)
         self.max_x.setOrientation(QtCore.Qt.Orientation.Horizontal)
         self.max_x.setInvertedAppearance(False)
         self.max_x.setInvertedControls(False)
         self.max_x.setTickPosition(QtWidgets.QSlider.TickPosition.TicksBelow)
         self.max_x.setTickInterval(100)
         self.max_x.setObjectName("max_x")
         self.horizontalLayout_6.addWidget(self.max_x)
         self.max_x_out = QtWidgets.QSpinBox(parent=self.verticalGroupBox)
         self.max_x_out.setButtonSymbols(QtWidgets.QAbstractSpinBox.ButtonSymbols.NoButtons)
-        self.max_x_out.setMaximum(500)
-        self.max_x_out.setValue(20)
+        self.max_x_out.setMaximum(300)
+        self.max_x_out.setProperty("value", 20)
         self.max_x_out.setObjectName("max_x_out")
         self.horizontalLayout_6.addWidget(self.max_x_out)
         self.verticalLayout_5.addLayout(self.horizontalLayout_6)
         self.logFit_widg = QtWidgets.QCheckBox(parent=self.verticalGroupBox)
         self.logFit_widg.setEnabled(True)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Fixed, QtWidgets.QSizePolicy.Policy.Fixed)
         sizePolicy.setHorizontalStretch(0)
@@ -171,18 +171,14 @@
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.text_output.sizePolicy().hasHeightForWidth())
         self.text_output.setSizePolicy(sizePolicy)
         self.text_output.setObjectName("text_output")
         self.verticalLayout_5.addWidget(self.text_output)
         self.horizontalLayout_3 = QtWidgets.QHBoxLayout()
         self.horizontalLayout_3.setObjectName("horizontalLayout_3")
-        self.plot_browse = QtWidgets.QPushButton(parent=self.verticalGroupBox)
-        self.plot_browse.setAcceptDrops(True)
-        self.plot_browse.setObjectName("plot_browse")
-        self.horizontalLayout_3.addWidget(self.plot_browse)
         self.csv_browse = QtWidgets.QPushButton(parent=self.verticalGroupBox)
         self.csv_browse.setAcceptDrops(True)
         self.csv_browse.setObjectName("csv_browse")
         self.horizontalLayout_3.addWidget(self.csv_browse)
         self.verticalLayout_5.addLayout(self.horizontalLayout_3)
         self.horizontalLayout_4.addWidget(self.verticalGroupBox)
         self.frame = QtWidgets.QFrame(parent=self.groupBox)
@@ -214,9 +210,8 @@
         self.label_24.setText(_translate("Form", "Number of Decays to fit"))
         self.label_3.setText(_translate("Form", "Maximum Time to Plot (ns)"))
         self.logFit_widg.setText(_translate("Form", "Fit in Log Space"))
         self.plotIRF_widg.setText(_translate("Form", "Plot the IRF"))
         self.scaled_widg.setText(_translate("Form", "Plot the Decays scaled by Their Coefficients"))
         self.fit_button.setText(_translate("Form", "Fit"))
         self.label_4.setText(_translate("Form", "Output"))
-        self.plot_browse.setText(_translate("Form", "Save Image"))
         self.csv_browse.setText(_translate("Form", "Save CSV"))
```

### Comparing `lifetimefitting-0.0.20/app/lifetimefitting/__main__.py` & `lifetimefitting-0.0.21/app/lifetimefitting/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import matplotlib.pyplot as plt
 from PyQt6 import QtWidgets
 from PyQt6.QtWidgets import QFileDialog
 from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg as FigureCanvas
+from matplotlib.backends.backend_qt5agg import NavigationToolbar2QT as NavigationToolbar
 from phdimporter import TRF
 from funcs.gui import Ui_Form
 from funcs.fittingFuncs import loadAndCull, fitFL
 import sys
 
 def plotFL():
     global csv
@@ -35,19 +36,21 @@
 def update_max_x():
     ui.max_x_out.setValue(ui.max_x.value())
 
 def update_max_x_from_out():
     ui.max_x.setValue(ui.max_x_out.value())
 
 def setupPlot():
-    ui.horizontalLayout_plot = QtWidgets.QHBoxLayout(ui.frame)
-    ui.horizontalLayout_plot.setObjectName("horizontalLayout_plot")
+    ui.verticalLayout_plot = QtWidgets.QVBoxLayout(ui.frame)
+    ui.verticalLayout_plot.setObjectName("verticalLayout_plot")
     ui.figure, (ui.ax1, ui.ax3, ui.ax2, ui.ax4) = plt.subplots(4, 1, figsize=(8, 10), sharex=True, height_ratios=[3, 3, 1, 1])
     ui.canvas = FigureCanvas(ui.figure)
-    ui.horizontalLayout_plot.addWidget(ui.canvas)
+    ui.toolbar = NavigationToolbar(ui.canvas)
+    ui.verticalLayout_plot.addWidget(ui.canvas)
+    ui.verticalLayout_plot.addWidget(ui.toolbar)
     ui.axList = []
 
     # log plot
     ui.ax1.set_yscale('log')
     ui.ax1.set_ylim(1e-1, 1e5, auto=False)
     ui.ax1.axhline(0, c='k', lw=0.5)
     ui.ax1.axvline(0, c='k', lw=0.5)
@@ -61,20 +64,14 @@
     ui.ax2.axhline(0, c='k', lw=0.5)
     # linear residuals
     ui.ax4.set_xlabel('Time (ns)')
     ui.ax4.set_ylabel('Residuals\n(lin)')
     ui.ax4.axvline(0, c='k', lw=0.5)
     ui.ax4.axhline(0, c='k', lw=0.5)
 
-def savePlot():
-    save_plot_dialog = QFileDialog()
-    name = save_plot_dialog.getSaveFileName(filter="PNG Image (*.png);;SVG Image (*.svg);;PDF Document (*.pdf)")[0]
-    if name != '':
-        plt.savefig(name, dpi=900)
-
 def saveCSV():
     global csv
     if 'csv' in globals():
         save_csv_dialog = QFileDialog()
         name = save_csv_dialog.getSaveFileName(filter="CSV Sheet (*.csv)")[0]
         if name != '':
             with open(name, 'w+') as f:
@@ -87,15 +84,14 @@
     ui.setupUi(Form)
     setupPlot()
 
     # file loading
     file_dialog = QFileDialog()
     ui.trf_browse.clicked.connect(trf_browse)
     ui.irf_browse.clicked.connect(irf_browse)
-    ui.plot_browse.clicked.connect(savePlot)
     ui.csv_browse.clicked.connect(saveCSV)
     ui.max_x.sliderMoved.connect(update_max_x)
     ui.max_x_out.valueChanged.connect(update_max_x_from_out)
 
     ui.fit_button.clicked.connect(plotFL)
 
     Form.show()
```

### Comparing `lifetimefitting-0.0.20/app/lifetimefitting.egg-info/PKG-INFO` & `lifetimefitting-0.0.21/app/lifetimefitting.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lifetimefitting
-Version: 0.0.20
+Version: 0.0.21
 Summary: PicoHarp TCSPC lifetime fitting tool
 Home-page: https://github.com/adreasnow/LifetimeFittingTool
 Author: Adrea Snow
 Author-email: adrea.snow@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lifetimefitting-0.0.20/setup.py` & `lifetimefitting-0.0.21/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name = "lifetimefitting",
-    version = "0.0.20",
+    version = "0.0.21",
     author = "Adrea Snow",
     author_email = "adrea.snow@gmail.com",
     description = "PicoHarp TCSPC lifetime fitting tool",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/adreasnow/LifetimeFittingTool",
     classifiers = [
```

