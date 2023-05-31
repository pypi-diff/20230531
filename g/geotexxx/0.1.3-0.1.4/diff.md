# Comparing `tmp/geotexxx-0.1.3.tar.gz` & `tmp/geotexxx-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geotexxx-0.1.3.tar", last modified: Tue May 30 09:32:45 2023, max compression
+gzip compressed data, was "geotexxx-0.1.4.tar", last modified: Wed May 31 11:27:11 2023, max compression
```

## Comparing `geotexxx-0.1.3.tar` & `geotexxx-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 09:32:45.236550 geotexxx-0.1.3/
--rw-rw-rw-   0        0        0    13954 2022-04-20 15:29:56.000000 geotexxx-0.1.3/LICENSE.txt
--rw-rw-rw-   0        0        0     3831 2023-05-30 09:32:45.235548 geotexxx-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     3573 2023-04-04 15:09:05.000000 geotexxx-0.1.3/README.md
--rw-rw-rw-   0        0        0      405 2023-05-30 09:32:28.000000 geotexxx-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-30 09:32:45.237552 geotexxx-0.1.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-30 09:32:45.200669 geotexxx-0.1.3/src/
-drwxrwxrwx   0        0        0        0 2023-05-30 09:32:45.213048 geotexxx-0.1.3/src/geotexxx/
--rw-rw-rw-   0        0        0        0 2023-02-24 15:44:18.000000 geotexxx-0.1.3/src/geotexxx/__init__.py
--rw-rw-rw-   0        0        0   101264 2023-05-30 09:31:50.000000 geotexxx-0.1.3/src/geotexxx/gefxml_reader.py
-drwxrwxrwx   0        0        0        0 2023-05-30 09:32:45.233170 geotexxx-0.1.3/src/geotexxx.egg-info/
--rw-rw-rw-   0        0        0     3831 2023-05-30 09:32:45.000000 geotexxx-0.1.3/src/geotexxx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-05-30 09:32:45.000000 geotexxx-0.1.3/src/geotexxx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 09:32:45.000000 geotexxx-0.1.3/src/geotexxx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-05-30 09:32:45.000000 geotexxx-0.1.3/src/geotexxx.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-30 09:32:45.000000 geotexxx-0.1.3/src/geotexxx.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-31 11:27:11.682188 geotexxx-0.1.4/
+-rw-rw-rw-   0        0        0    13954 2022-04-20 15:29:56.000000 geotexxx-0.1.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     3831 2023-05-31 11:27:11.681188 geotexxx-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3573 2023-04-04 15:09:05.000000 geotexxx-0.1.4/README.md
+-rw-rw-rw-   0        0        0      405 2023-05-31 11:26:31.000000 geotexxx-0.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-31 11:27:11.682188 geotexxx-0.1.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-31 11:27:11.660220 geotexxx-0.1.4/src/
+drwxrwxrwx   0        0        0        0 2023-05-31 11:27:11.668915 geotexxx-0.1.4/src/geotexxx/
+-rw-rw-rw-   0        0        0        0 2023-02-24 15:44:18.000000 geotexxx-0.1.4/src/geotexxx/__init__.py
+-rw-rw-rw-   0        0        0   103525 2023-05-31 10:28:47.000000 geotexxx-0.1.4/src/geotexxx/gefxml_reader.py
+drwxrwxrwx   0        0        0        0 2023-05-31 11:27:11.679181 geotexxx-0.1.4/src/geotexxx.egg-info/
+-rw-rw-rw-   0        0        0     3831 2023-05-31 11:27:11.000000 geotexxx-0.1.4/src/geotexxx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-05-31 11:27:11.000000 geotexxx-0.1.4/src/geotexxx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 11:27:11.000000 geotexxx-0.1.4/src/geotexxx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-05-31 11:27:11.000000 geotexxx-0.1.4/src/geotexxx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-31 11:27:11.000000 geotexxx-0.1.4/src/geotexxx.egg-info/top_level.txt
```

### Comparing `geotexxx-0.1.3/LICENSE.txt` & `geotexxx-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `geotexxx-0.1.3/PKG-INFO` & `geotexxx-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geotexxx
-Version: 0.1.3
+Version: 0.1.4
 Summary: Package om geotechnisch grondonderzoek te verwerken
 Author-email: Thomas van der Linden <t.van.der.linden@amsterdam.nl>
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # gefxml_reader
```

### Comparing `geotexxx-0.1.3/README.md` & `geotexxx-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `geotexxx-0.1.3/src/geotexxx/gefxml_reader.py` & `geotexxx-0.1.4/src/geotexxx/gefxml_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1422,15 +1422,15 @@
     def plot_samendrukkingsproeven(self, saveFigs=False):
         figs = []
         for sampleNumber, complexAnalysis in self.complexAnalyses.items():
             if self.analyses.loc[sampleNumber, 'analysisType'] == 'zetting':
                 fig = self.plot_samendrukkingsproef(sampleNumber, complexAnalysis, tijdIn='min', saveFig=False, saveData=False)
                 figs.append(fig)
                 if saveFigs:
-                    plt.savefig(f'./samendrukkingsproef_{self.testid}_{sampleNumber}.png')
+                    plt.savefig(f'./output/samendrukkingsproef_{self.testid}_{sampleNumber}.png')
                     plt.close('all')
         return figs
     
     def plot_samendrukkingsproef(self, sampleNumber, complexAnalysis, tijdIn='min', saveFig=False, saveData=False):
         testdf = [] # dataframe om proefresultaten in tabel weg te schrijven
         # bepaal de monsterhoogte
         sampleHeight = float(self.analyses.loc[sampleNumber, 'endDepth']) - float(self.analyses.loc[sampleNumber, 'beginDepth'])
@@ -1461,15 +1461,15 @@
         ax1.set_xlabel(f'Tijd [{tijdIn}]')
         ax1.set_ylabel('Zetting [mm]')
         ax1.set_title(f'Tijd-Zetting Boring: {self.testid} Monster: {sampleNumber} Niveau: {float(self.analyses.loc[sampleNumber, "endDepth"]):.2f} - {float(self.analyses.loc[sampleNumber, "beginDepth"]):.2f}')
 
         # tabel met proefresultaten wegschrijven
         if saveData:
             testdf = pd.concat(testdf)
-            testdf.to_csv(f'./tijdzetting_{sampleNumber}.csv', sep=';', decimal=',')
+            testdf.to_csv(f'./output/tijdzetting_{sampleNumber}.csv', sep=';', decimal=',')
 
         # maak een belasting-rek plot
         x, y = [], []
         # doorloop de stappen
         for stepNumber in complexAnalysis.loc['values'].index:
 
             xy = pd.read_csv(StringIO(complexAnalysis.loc['values', stepNumber]), sep=',', lineterminator=';', header=None)
@@ -1484,18 +1484,71 @@
         ax2.set_xlim([1, 1000])
         ax2.invert_yaxis()
         ax2.set_xlabel('belasting [kPa]')
         ax2.set_ylabel('lineaire rek [-]')
         ax2.set_title(f'Belasting-Rek Boring: {self.testid} Monster: {sampleNumber} Niveau: {float(self.analyses.loc[sampleNumber, "endDepth"]):.2f} - {float(self.analyses.loc[sampleNumber, "beginDepth"]):.2f}')
 
         if saveFig:
-            plt.savefig(f'./samendrukkingsproef_{self.testid}_{sampleNumber}.png')
+            plt.savefig(f'./output/samendrukkingsproef_{self.testid}_{sampleNumber}.png')
 
         return fig
 
+    def plot_korrelgrootte_verdeling(self, grainsizeData, monster, saveFig=False, saveData=False):
+        fig = plt.figure()
+        ax = fig.add_subplot()
+        ax.semilogx(grainsizeData.columns, pd.to_numeric(grainsizeData.loc[monster]).cumsum())
+        ax.set_xlabel('korrelgrootte [mm]')
+        ax.set_ylabel('[%]')
+
+        if saveFig:
+            plt.savefig(f'./output/korrelgrootte_{self.testid}_{monster}.png')
+
+        if saveData:
+            grainsizeData.to_csv(f'./output/korrelgrootte_{self.testid}_{monster}.csv', sep=';', decimal=',')
+
+        return fig
+
+
+    def plot_korrelgrootte_verdelingen(self, saveFigs=False):
+        figs = []
+
+        grainsize_pattern = re.compile(r'fraction(?P<from>\d+_?\d*)u*m*to(?P<to>\d+_?\d*)(?P<unit>[um]m)')
+
+        if isinstance(self.analyses, pd.DataFrame) and 'korrelgrootteverdeling' in self.analyses['analysisType'].unique():
+            # filter kolommen zodat ze fraction ... to bevatten
+            grainsizeData = self.analyses[self.analyses['analysisType'] == 'korrelgrootteverdeling']
+
+            grainsizeCols = []
+            for col in self.analyses.columns:
+                if 'fraction' in col and 'to' in col:
+                    grainsizeCols.append(col)
+            grainsizeData = grainsizeData[grainsizeCols]
+
+            # doorloop de kolomnamen om deze numeriek te maken'
+            grainsizeData.columns = grainsizeData.columns.str.extract(grainsize_pattern)
+            
+            # maak van de waarden alles mm
+            colsMm = []
+            for col in grainsizeData.columns:
+                if col[2] == 'um':
+                    colsMm.append(float(col[1].replace('_', '.')) / 1000)
+                elif col[2] == 'mm':
+                    colsMm.append(float(col[1].replace('_', '.')))
+            grainsizeData.columns = colsMm
+
+            # maak een plot
+            for monster in grainsizeData.index:
+                fig = self.plot_korrelgrootte_verdeling(grainsizeData, monster, saveFig=False, saveData=False)
+                figs.append(fig)
+                if saveFigs:
+                    plt.savefig(f'./output/korrelgrootte_{self.testid}_{monster}.png')
+
+        return figs
+
+
     def from_cpt(self, cpt, interpretationModel='Robertson'):
 
         # maak een object alsof het een boring is
         self.soillayers['cpt']= pd.DataFrame(columns=['geotechnicalSoilName', 'frictionRatio', 'coneResistance', 'upper_NAP', 'lower_NAP'])
         self.soillayers['cpt']['geotechnicalSoilName'] = cpt.data[interpretationModel]
         # TODO frictionRatio en coneResistance horen er eigenlijk niet in thuis, maar zijn handig als referentie
         self.soillayers['cpt'][['frictionRatio', 'coneResistance']] = cpt.data[['frictionRatio', 'coneResistance']]
```

### Comparing `geotexxx-0.1.3/src/geotexxx.egg-info/PKG-INFO` & `geotexxx-0.1.4/src/geotexxx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geotexxx
-Version: 0.1.3
+Version: 0.1.4
 Summary: Package om geotechnisch grondonderzoek te verwerken
 Author-email: Thomas van der Linden <t.van.der.linden@amsterdam.nl>
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # gefxml_reader
```

