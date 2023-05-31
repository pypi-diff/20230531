# Comparing `tmp/afscgap-0.0.9.tar.gz` & `tmp/afscgap-1.0.0.tar.gz`

## Comparing `afscgap-0.0.9.tar` & `afscgap-1.0.0.tar`

### file list

```diff
@@ -1,31 +1,39 @@
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 afscgap-0.0.9/.gitattributes
--rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 afscgap-0.0.9/CONDUCT.md
--rw-r--r--   0        0        0     7583 2020-02-02 00:00:00.000000 afscgap-0.0.9/CONTRIBUTING.md
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 afscgap-0.0.9/gruntfile.js
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 afscgap-0.0.9/install_browser.sh
--rw-r--r--   0        0        0   178220 2020-02-02 00:00:00.000000 afscgap-0.0.9/package-lock.json
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 afscgap-0.0.9/package.json
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 afscgap-0.0.9/setup.cfg
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 afscgap-0.0.9/afscgap/README.md
--rw-r--r--   0        0        0    58952 2020-02-02 00:00:00.000000 afscgap-0.0.9/afscgap/__init__.py
--rw-r--r--   0        0        0    42895 2020-02-02 00:00:00.000000 afscgap-0.0.9/afscgap/client.py
--rw-r--r--   0        0        0     9440 2020-02-02 00:00:00.000000 afscgap-0.0.9/afscgap/convert.py
--rw-r--r--   0        0        0     5132 2020-02-02 00:00:00.000000 afscgap-0.0.9/afscgap/cursor.py
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 afscgap-0.0.9/afscgap/http_util.py
--rw-r--r--   0        0        0    37009 2020-02-02 00:00:00.000000 afscgap-0.0.9/afscgap/inference.py
--rw-r--r--   0        0        0    37762 2020-02-02 00:00:00.000000 afscgap-0.0.9/afscgap/model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 afscgap-0.0.9/afscgap/py.typed
--rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 afscgap-0.0.9/afscgap/query_util.py
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 afscgap-0.0.9/afscgap/typesdef.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 afscgap-0.0.9/inst/README.md
--rw-r--r--   0        0        0    13278 2020-02-02 00:00:00.000000 afscgap-0.0.9/inst/architecture.drawio
--rw-r--r--   0        0        0    87762 2020-02-02 00:00:00.000000 afscgap-0.0.9/inst/library.png
--rw-r--r--   0        0        0     5648 2020-02-02 00:00:00.000000 afscgap-0.0.9/inst/paper.bib
--rw-r--r--   0        0        0     7867 2020-02-02 00:00:00.000000 afscgap-0.0.9/inst/paper.md
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 afscgap-0.0.9/inst/preview_paper.sh
--rw-r--r--   0        0        0   176314 2020-02-02 00:00:00.000000 afscgap-0.0.9/inst/viz.png
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 afscgap-0.0.9/.gitignore
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 afscgap-0.0.9/LICENSE.md
--rw-r--r--   0        0        0    43240 2020-02-02 00:00:00.000000 afscgap-0.0.9/README.md
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 afscgap-0.0.9/pyproject.toml
--rw-r--r--   0        0        0    44624 2020-02-02 00:00:00.000000 afscgap-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 afscgap-1.0.0/.gitattributes
+-rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 afscgap-1.0.0/CONDUCT.md
+-rw-r--r--   0        0        0     7583 2020-02-02 00:00:00.000000 afscgap-1.0.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 afscgap-1.0.0/build_docs.sh
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 afscgap-1.0.0/gruntfile.js
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 afscgap-1.0.0/install_browser.sh
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 afscgap-1.0.0/mkdocs.yml
+-rw-r--r--   0        0        0   178220 2020-02-02 00:00:00.000000 afscgap-1.0.0/package-lock.json
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 afscgap-1.0.0/package.json
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 afscgap-1.0.0/setup.cfg
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 afscgap-1.0.0/afscgap/README.md
+-rw-r--r--   0        0        0    58901 2020-02-02 00:00:00.000000 afscgap-1.0.0/afscgap/__init__.py
+-rw-r--r--   0        0        0    42895 2020-02-02 00:00:00.000000 afscgap-1.0.0/afscgap/client.py
+-rw-r--r--   0        0        0     9440 2020-02-02 00:00:00.000000 afscgap-1.0.0/afscgap/convert.py
+-rw-r--r--   0        0        0     5132 2020-02-02 00:00:00.000000 afscgap-1.0.0/afscgap/cursor.py
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 afscgap-1.0.0/afscgap/http_util.py
+-rw-r--r--   0        0        0    37009 2020-02-02 00:00:00.000000 afscgap-1.0.0/afscgap/inference.py
+-rw-r--r--   0        0        0    37762 2020-02-02 00:00:00.000000 afscgap-1.0.0/afscgap/model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 afscgap-1.0.0/afscgap/py.typed
+-rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 afscgap-1.0.0/afscgap/query_util.py
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 afscgap-1.0.0/afscgap/typesdef.py
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 afscgap-1.0.0/docs/building.md
+-rw-r--r--   0        0        0     5761 2020-02-02 00:00:00.000000 afscgap-1.0.0/docs/inference.md
+-rw-r--r--   0        0        0     3686 2020-02-02 00:00:00.000000 afscgap-1.0.0/docs/limitations.md
+-rw-r--r--   0        0        0    12988 2020-02-02 00:00:00.000000 afscgap-1.0.0/docs/model.md
+-rw-r--r--   0        0        0     3063 2020-02-02 00:00:00.000000 afscgap-1.0.0/docs/objectives.md
+-rw-r--r--   0        0        0    10255 2020-02-02 00:00:00.000000 afscgap-1.0.0/docs/usage.md
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 afscgap-1.0.0/inst/README.md
+-rw-r--r--   0        0        0    13278 2020-02-02 00:00:00.000000 afscgap-1.0.0/inst/architecture.drawio
+-rw-r--r--   0        0        0    87762 2020-02-02 00:00:00.000000 afscgap-1.0.0/inst/library.png
+-rw-r--r--   0        0        0     5641 2020-02-02 00:00:00.000000 afscgap-1.0.0/inst/paper.bib
+-rw-r--r--   0        0        0     7572 2020-02-02 00:00:00.000000 afscgap-1.0.0/inst/paper.md
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 afscgap-1.0.0/inst/preview_paper.sh
+-rw-r--r--   0        0        0   173860 2020-02-02 00:00:00.000000 afscgap-1.0.0/inst/viz.png
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 afscgap-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 afscgap-1.0.0/LICENSE.md
+-rw-r--r--   0        0        0    11171 2020-02-02 00:00:00.000000 afscgap-1.0.0/README.md
+-rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 afscgap-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0    12640 2020-02-02 00:00:00.000000 afscgap-1.0.0/PKG-INFO
```

### Comparing `afscgap-0.0.9/CONDUCT.md` & `afscgap-1.0.0/CONDUCT.md`

 * *Files identical despite different names*

### Comparing `afscgap-0.0.9/CONTRIBUTING.md` & `afscgap-1.0.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `afscgap-0.0.9/gruntfile.js` & `afscgap-1.0.0/gruntfile.js`

 * *Files identical despite different names*

### Comparing `afscgap-0.0.9/package-lock.json` & `afscgap-1.0.0/package-lock.json`

 * *Files identical despite different names*

### Comparing `afscgap-0.0.9/afscgap/__init__.py` & `afscgap-1.0.0/afscgap/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,8 @@
-"""
-.. include:: ../README.md
-
-<br>
-<br>
-
-# API docs
-
-Library which allows for Pythonic access to the interacting with AFSC GAP.
+"""Library which allows for Pythonic access to the interacting with AFSC GAP.
 
 This library supports Pythonic utilization of the API for the Ground
 Fish Assessment Program (GAP), a dataset produced by the Resource Assessment
 and Conservation Engineering (RACE) Division of the Alaska Fisheries Science
 Center (AFSC) as part of the National Oceanic and Atmospheric Administration
 (NOAA Fisheries). Note that this is a community-provided library and is not
 officially endorsed by NOAA.
```

### Comparing `afscgap-0.0.9/afscgap/client.py` & `afscgap-1.0.0/afscgap/client.py`

 * *Files identical despite different names*

### Comparing `afscgap-0.0.9/afscgap/convert.py` & `afscgap-1.0.0/afscgap/convert.py`

 * *Files identical despite different names*

### Comparing `afscgap-0.0.9/afscgap/cursor.py` & `afscgap-1.0.0/afscgap/cursor.py`

 * *Files identical despite different names*

### Comparing `afscgap-0.0.9/afscgap/http_util.py` & `afscgap-1.0.0/afscgap/http_util.py`

 * *Files identical despite different names*

### Comparing `afscgap-0.0.9/afscgap/inference.py` & `afscgap-1.0.0/afscgap/inference.py`

 * *Files identical despite different names*

### Comparing `afscgap-0.0.9/afscgap/model.py` & `afscgap-1.0.0/afscgap/model.py`

 * *Files identical despite different names*

### Comparing `afscgap-0.0.9/afscgap/query_util.py` & `afscgap-1.0.0/afscgap/query_util.py`

 * *Files identical despite different names*

### Comparing `afscgap-0.0.9/afscgap/typesdef.py` & `afscgap-1.0.0/afscgap/typesdef.py`

 * *Files identical despite different names*

### Comparing `afscgap-0.0.9/inst/README.md` & `afscgap-1.0.0/inst/README.md`

 * *Files identical despite different names*

### Comparing `afscgap-0.0.9/inst/architecture.drawio` & `afscgap-1.0.0/inst/architecture.drawio`

 * *Files identical despite different names*

### Comparing `afscgap-0.0.9/inst/library.png` & `afscgap-1.0.0/inst/library.png`

 * *Files identical despite different names*

### Comparing `afscgap-0.0.9/inst/paper.bib` & `afscgap-1.0.0/inst/paper.bib`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 }
 
 @misc{diagrams,
   title={Jgraph/Drawio: Draw.io is a JavaScript, client-side editor for general diagramming and whiteboarding},
   url={https://github.com/jgraph/drawio},
   journal={GitHub},
   publisher={GitHub, Inc}, 
-  author={JGraph Ltd and draw.io AG},
+  author={JGraph and draw.io},
   year={2023}
 }
 
 @misc{d3,
   title={Data-Driven Documents 7.8.2},
   url={https://d3js.org/},
   journal={D3.js},
```

### Comparing `afscgap-0.0.9/inst/paper.md` & `afscgap-1.0.0/inst/paper.md`

 * *Files 19% similar despite different names*

```diff
@@ -30,70 +30,88 @@
 institute:
   - ucberkeley: University of California, Berkeley
 date: 4 April 2023
 bibliography: paper.bib
 ---
 
 # Summary
-The Resource Assessment and Conservation Engineering Division of the National Oceanic and Atmospheric Administration's Alaska Fisheries Science Center (NOAA AFSC RACE) runs the [Groundfish Assessment Program](https://www.fisheries.noaa.gov/contact/groundfish-assessment-program) (GAP) which produces longitudinal catch data [@afscgap]. These "hauls" report where marine species are found during bottom trawl surveys and in what quantities, empowering ocean health research and fisheries management [@example]. Increasing accessibility of these important data through tools for individuals of diverse programming experience, Pyafscgap.org offers not just easier access to the dataset's REST API through query compilation but provides both memory-efficient algorithms for "zero-catch inference" and interactive visual analytics tools [@inport]. Altogether, this toolset supports investigatory tasks not easily executable using the API service alone and, leveraging game and information design, offers these data to a broader audience.
+The Groundfish Assessment Program within NOAA's Alaska Fisheries Science Center produces longitudinal catch data for the region [@afscgap]. Supporting ocean health research and fisheries management, these "hauls" report where marine species are found during bottom trawl surveys and in what quantities [@example]. Increasing data usability for communities of diverse programming experience, Pyafscgap.org offers not just friendlier REST API operation for this economically and scientifically important dataset but query language compliation, memory-efficient algorithms for "zero-catch" inference, and interactive visual analytics. Altogether, this research toolset supports investigatory tasks not easily executable using the API service alone and broadens access through game and information design.
 
 # Statement of need
-Pyafscgap.org reduces barriers for use of GAP data, offering open source solutions for addressing the dataset's use of proprietary technology, presence-only nature, and size / complexity [@inport].
+Pyafscgap.org reduces barriers for use of NOAA AFSC RACE GAP^[Groundfish Assessment Program in the Resource Assessment and Conservation Engineering Division of the National Oceanic and Atmospheric Administration's Alaska Fisheries Science Center] data, offering:
 
-## Developer accessibility
-Working with these data requires knowledge of tools ouside the Python "standard toolchest" like the closed-source Oracle REST Data Services (ORDS) [@ords]. The `afscgap` package offers easier open source-based developer access to the official REST service with automated pagination, Python to ORDS syntax compilation, and documented types. Together, these tools enable Python developers to use familiar patterns to interact with these data like type checking, standard documentation, and other Python data-related libraries.
+ - Improved developer usability.
+ - Memory-efficient algorithms for analysis requiring zero catch inference.
+ - Tools for those with less developer experience.
 
-## Common analysis
-Access to the API alone cannot support some investigations as the API provides "presence-only" data [@inport]. Many types of analysis require information not just about where a species was present but also where it was not. For example, consider geohash-aggregated species catch per unit effort: while the presence-only dataset may provide a total weight or count, the total area swept for a region may not necessarily be easily available but required [@geohash; @notebook]. The `afscgap` Python package can, with memory efficiency, algorithmically infer those needed "zero catch" records.
+Altogether, these open source tools extend the dataset's reach and approachability.
 
-## General public accessibility
-Though the `afscgap` Python package makes GAP catch data more accessible to developers, the size and complexity of this dataset requires non-trivial engineering for comparative analysis between species, years, and/or geographic areas [@notebook]. Without deep developer experience, it can be difficult to get started. To address a broader audience, this project also offers a no-code visualization tool sitting on top of `afscgap` to begin investigations with CSV and Python code export as a bridge to further analysis.
+## Developer usability
+Working with these data requires knowledge of tools ouside the Python "standard toolset" like the closed-source Oracle REST Data Services (ORDS) [@ords]. The `afscgap` package offers easier access to the official REST service with automated pagination, ORDS compilation, and documented types. Together, these tools enable Python developers to use familiar patterns to interact with these data: type checking, standard documentation, and compatability with common Python data-related libraries.
+
+## Record inference
+The API struggles supporting some investigations as it provides "presence-only" data [@inport]. For example, the API may readily yield total mass of Pacific cod but not its geohash-aggregated catch per unit effort [@geohash].
+
+$$CPUE_{species} = \frac{m_{species}}{A_{swept}}$$
+
+Knowing CPUE (kg/ha) must also include "absence data" or hauls in which the speices was not recorded, this package can efficiently infer those hauls not easily returned from the API service [@notebook].
+
+## Broad accessibility
+Though the `afscgap` Python package makes GAP catch data more accessible, the size and complexity of this dataset complicates comparative analysis between species, years, and/or geographic areas [@notebook]. Without deep developer experience, it may still be difficult to get started even with scientific background. To address a broader audience, this project also offers a no-code visualization tool sitting on top of `afscgap` with CSV and Python code export as a bridge to further analysis.
 
 # Functions
-This project aims to improve accessibility of GAP catch data, democratizing developer access and offering inclusive approachable tools to kickstart analysis.
+This project aims to improve accessibility of GAP catch data and offer approachable tools to kickstart analysis.
 
 ## Lazy querying facade
-The `afscgap` library manages significant data structure complexity to offer a simple familiar interface to Python developers. First, lazy "generator iterables" increase accessibility by encapsulating logic for memory-efficient pagination and "data munging" behind Python-standard iterators [@lazy]. Furthermore, to support zero catch data, decorators adapt diverse structures to common interfaces, offering polymorphism [@decorators]. Finally, offering a single object entry-point into the library, a "facade" approach allows the user to interact with these systems without requiring deep understanding of the library's types, a goal furthered by compilation of "standard" Python types to Oracle REST Data Service queries [@facade].
+The `afscgap` library manages significant complexity to offer a simple familiar interface to Python developers:
+
+ - Lazy "generator iterables" increase accessibility by encapsulating logic for memory-efficient pagination and "data munging" behind Python-standard iterators [@lazy].
+ - To support zero catch data, decorators adapt diverse structures to common interfaces, offering polymorphism [@decorators].
+ - Offering a single object entry-point into the library, a "facade" frees users from needing deep understanding of the library's types, a goal furthered by compilation of "standard" Python types to Oracle REST Data Service queries [@facade].
 
-![Diagram of simplified afscgap operation [@diagrams].\label{fig:library}](library.png)
+![Diagram of afscgap.\label{fig:library}](library.png)
 
 ## Zero catch inference
-"Negative" or "zero catch" inference enables scientists to conduct a broader range of analysis. To achieve this, the package uses the following algorithm:
+"Zero catch" inference enables a broader range of analysis with the following algorithm:
 
  - Paginate while records remain available from the API service.
    - Record species and hauls observed from API-returned results.
    - Return records as available.
  - Generate inferred records after API exhaustion.
    - For each species observed in API results, check if it had a record for each haul in a hauls flat file [@flatfile].
-   - For any hauls without the species, produce an 0 catch record from the iterator.
+   - For any hauls without the species, produce a record from the iterator.
 
-Note that, this library offers Python-emaultion of ORDS-compiled fitlers for inferred records.
+This library offers Python-emulation of ORDS filters for inferred records.
 
 ## Visualization
-Despite these developer-focused tools, zero catch inference's millions of records requires technical sophistication to navigate. To further increase accessibility, this project offers a visualization tool for starting temporal, spatial, and species comparisons with coordinated highlighting, separated color channels, summary statistics, and side-by-side display [@few].
+This complex dataset requires technical sophistication to navigate and, to further increase accessibility, visualization tools help start temporal, spatial, and species comparisons with deep linking, coordinated highlighting, separated color channels, summary statistics, and side-by-side display [@few]. To support learning this UI, an optional introduction sequence tutorializes a "real" analysis via Hayashida^[Uses Mark Brown's formalization [@brown].] level design [@hayashida; @brown]:
 
-![Screenshot of the visualization tool.\label{fig:viz}](viz.png)
+ - **Introduction**: The tool shows information about Pacific cod with pre-filled controls used to achieve that analysis gradually fading in, asking the user for minor modifications.
+ - **Development**: Using the mechanics introduced moments prior, the tool invites the user to change the analysis to compare different regions.
+ - **Twist**: Enabling overlays on the same display, the user leverages mechanics they just exercised in a now more complex interface.
+ - **Conclusion**: The visualization invites the user to demonstrate skills acquired in a new problem.
 
-Of course, building competency in a sophisticated interface like this presents user experience challenges and, to that end, this project interprets Hayashida level design via Mark Brown's formalization into an in-tool introduction sequence that directs the player through a "real" analysis [@hayashida; @brown]:
+Note that this visualization also serves as a starting point for continued analysis by generating either CSV or Python code to take work into other tools.
 
- - **Introduction**: The player sees information about Pacific cod with pre-filled elements used to achieve that analysis gradually fading in.
- - **Development**: Using the mechanics introduced moments prior, the tool invites the player to change the analysis to compare different regions with temperature data.
- - **Twist**: Overlays on the same display are enabled, allowing the player to leverage mechanics they just exercised in a now more complex interface.
- - **Conclusion**: End with giving the player an opportunity to demonstrate all of the skills acquired in a new problem.
+![Visualization screenshot.\label{fig:viz}](viz.png)
 
-While this interface uses game / information design techniques to offer an accessible on-ramp to quickly learn a sophisticated interface, it also serves as a starting point for continued analysis by generating either CSV or Python code to take work into other tools. Examined via Thinking-aloud Method [@thinkaloud].
+In addition to graduate classroom use, five individuals with relevant background offered detailed feedback on this open source visualization. Though sometimes aided by a think-aloud prompt, feedback was limited to needs assessment / quality improvement specific to this publicly accessible web service [@thinkaloud].
 
 ## Limitations
-Notable current limitations:
+As further documented in the repository [@readme], these tools:
 
- - Single-threaded and non-asynchoronous.
- - Due to dataset limitations, hauls are represeted by points not areas in visualization aggregation [@readme].
+ - Run single-threaded and synchoronous.
+ - Represents hauls as points not areas in visualization aggregation due to dataset limitation.
+ - Must exclude any hauls also excluded by NOAA from their dataset.
 
 # Acknowledgements
-Thanks to the following for feedback / testing on these components:
+Thanks to:
 
- - Library: Carl Boettiger and Fernando Perez
- - Visualization: Maya Weltman-Fahs, Brookie Guzder-Williams, and Magali de Bruyn.
+ - Runtime dependencies: ColorBrewer, D3, Flask, Geolib, Requests, Toolz, and Papa Parse [@colorbrewer; @d3; @flask; @geolib; @requests; @toolz; @papa].
+ - Library advice: Carl Boettiger, Fernando Perez, and PyOpenSci reviewers.
+ - Visualization advice: Lewis Barnett, Magali de Bruyn, Brookie Guzder-Williams, Angela Hayes, David Joy, Emily Markowitz, and Maya Weltman-Fahs.
+ - Ciera Martinez for general guidance.
+ - Draw.io for diagrams [@diagrams].
 
-Project of the The Eric and Wendy Schmidt Center for Data Science and the Environment at University of California Berkeley. Though the README lists full library credits, thanks to runtime dependencies ColorBrewer, D3, Flask, Geolib, Requests, Toolz, and Papa Parse [@colorbrewer; @d3; @flask; @geolib; @requests; @toolz; @papa].
+Project of The Eric and Wendy Schmidt Center for Data Science and the Environment at UC Berkeley.
 
-# References
+# References
```

### Comparing `afscgap-0.0.9/LICENSE.md` & `afscgap-1.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `afscgap-0.0.9/pyproject.toml` & `afscgap-1.0.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "afscgap"
-version = "0.0.9"
+version = "1.0.0"
 authors = [
   { name="A Samuel Pottinger", email="sam.pottinger@berkeley.edu" },
 ]
 description = "Tools for interacting with the public bottom trawl surveys data from the NOAA AFSC GAP."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -34,15 +34,17 @@
   "build",
   "nose2",
   "mypy",
   "pyflakes",
   "pycodestyle",
   "pdoc",
   "twine",
-  "types-requests"
+  "types-requests",
+  "mkdocs",
+  "mkdocs-windmill"
 ]
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.hatch.build]
```

