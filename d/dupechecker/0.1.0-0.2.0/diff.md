# Comparing `tmp/dupechecker-0.1.0.tar.gz` & `tmp/dupechecker-0.2.0.tar.gz`

## Comparing `dupechecker-0.1.0.tar` & `dupechecker-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0    33570 2020-02-02 00:00:00.000000 dupechecker-0.1.0/docs/dupechecker.html
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 dupechecker-0.1.0/docs/index.html
--rw-r--r--   0        0        0    23348 2020-02-02 00:00:00.000000 dupechecker-0.1.0/docs/search.js
--rw-r--r--   0        0        0    99179 2020-02-02 00:00:00.000000 dupechecker-0.1.0/docs/dupechecker/dupechecker.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dupechecker-0.1.0/src/dupechecker/__init__.py
--rw-r--r--   0        0        0     4369 2020-02-02 00:00:00.000000 dupechecker-0.1.0/src/dupechecker/dupechecker.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 dupechecker-0.1.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 dupechecker-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 dupechecker-0.1.0/README.md
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 dupechecker-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 dupechecker-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 dupechecker-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0    33570 2020-02-02 00:00:00.000000 dupechecker-0.2.0/docs/dupechecker.html
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 dupechecker-0.2.0/docs/index.html
+-rw-r--r--   0        0        0    23051 2020-02-02 00:00:00.000000 dupechecker-0.2.0/docs/search.js
+-rw-r--r--   0        0        0   107454 2020-02-02 00:00:00.000000 dupechecker-0.2.0/docs/dupechecker/dupechecker.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dupechecker-0.2.0/src/dupechecker/__init__.py
+-rw-r--r--   0        0        0     4920 2020-02-02 00:00:00.000000 dupechecker-0.2.0/src/dupechecker/dupechecker.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 dupechecker-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 dupechecker-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 dupechecker-0.2.0/README.md
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 dupechecker-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 dupechecker-0.2.0/PKG-INFO
```

### Comparing `dupechecker-0.1.0/docs/dupechecker.html` & `dupechecker-0.2.0/docs/dupechecker.html`

 * *Files identical despite different names*

### Comparing `dupechecker-0.1.0/docs/search.js` & `dupechecker-0.2.0/docs/search.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -693,16 +693,16 @@
         "kind": "module",
         "doc": "<p></p>\n"
     }, {
         "fullname": "dupechecker.dupechecker.get_duplicates",
         "modulename": "dupechecker.dupechecker",
         "qualname": "get_duplicates",
         "kind": "function",
-        "doc": "<p>Return a list of lists for duplicate files in <code>path</code>.\nEach sub-list will contain 2 or more files determined to be equivalent files.\nIf <code>recursive</code> is <code>True</code>, files from <code>path</code> and it's subdirectories will be compared.</p>\n",
-        "signature": "<span class=\"signature pdoc-code multiline\">(<span class=\"param\">\t<span class=\"n\">path</span><span class=\"p\">:</span> <span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">Pathier</span>,</span><span class=\"param\">\t<span class=\"n\">recursive</span><span class=\"p\">:</span> <span class=\"nb\">bool</span> <span class=\"o\">=</span> <span class=\"kc\">False</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">Pathier</span><span class=\"p\">]]</span>:</span></span>",
+        "doc": "<p>Return a list of lists for duplicate files in <code>paths</code>.</p>\n",
+        "signature": "<span class=\"signature pdoc-code multiline\">(<span class=\"param\">\t<span class=\"n\">paths</span><span class=\"p\">:</span> <span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">Pathier</span><span class=\"p\">]</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">Pathier</span><span class=\"p\">]]</span>:</span></span>",
         "funcdef": "def"
     }, {
         "fullname": "dupechecker.dupechecker.get_args",
         "modulename": "dupechecker.dupechecker",
         "qualname": "get_args",
         "kind": "function",
         "doc": "<p></p>\n",
```

### Comparing `dupechecker-0.1.0/docs/dupechecker/dupechecker.html` & `dupechecker-0.2.0/docs/dupechecker/dupechecker.html`

 * *Files 1% similar despite different names*

```diff
@@ -66,175 +66,188 @@
 
                         <label class="view-source-button" for="mod-dupechecker-view-source"><span>View Source</span></label>
 
                         <div class="pdoc-code codehilite"><pre><span></span><span id="L-1"><a href="#L-1"><span class="linenos">  1</span></a><span class="kn">import</span> <span class="nn">argparse</span>
 </span><span id="L-2"><a href="#L-2"><span class="linenos">  2</span></a><span class="kn">import</span> <span class="nn">filecmp</span>
 </span><span id="L-3"><a href="#L-3"><span class="linenos">  3</span></a><span class="kn">import</span> <span class="nn">time</span>
 </span><span id="L-4"><a href="#L-4"><span class="linenos">  4</span></a><span class="kn">from</span> <span class="nn">concurrent.futures</span> <span class="kn">import</span> <span class="n">ThreadPoolExecutor</span>
-</span><span id="L-5"><a href="#L-5"><span class="linenos">  5</span></a>
-</span><span id="L-6"><a href="#L-6"><span class="linenos">  6</span></a><span class="kn">from</span> <span class="nn">griddle</span> <span class="kn">import</span> <span class="n">griddy</span>
-</span><span id="L-7"><a href="#L-7"><span class="linenos">  7</span></a><span class="kn">from</span> <span class="nn">pathier</span> <span class="kn">import</span> <span class="n">Pathier</span>
-</span><span id="L-8"><a href="#L-8"><span class="linenos">  8</span></a><span class="kn">from</span> <span class="nn">printbuddies</span> <span class="kn">import</span> <span class="n">Spinner</span>
-</span><span id="L-9"><a href="#L-9"><span class="linenos">  9</span></a>
-</span><span id="L-10"><a href="#L-10"><span class="linenos"> 10</span></a>
-</span><span id="L-11"><a href="#L-11"><span class="linenos"> 11</span></a><span class="k">def</span> <span class="nf">get_duplicates</span><span class="p">(</span><span class="n">path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">,</span> <span class="n">recursive</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">Pathier</span><span class="p">]]:</span>
-</span><span id="L-12"><a href="#L-12"><span class="linenos"> 12</span></a>    <span class="sd">&quot;&quot;&quot;Return a list of lists for duplicate files in `path`.</span>
-</span><span id="L-13"><a href="#L-13"><span class="linenos"> 13</span></a><span class="sd">    Each sub-list will contain 2 or more files determined to be equivalent files.</span>
-</span><span id="L-14"><a href="#L-14"><span class="linenos"> 14</span></a><span class="sd">    If `recursive` is `True`, files from `path` and it&#39;s subdirectories will be compared.&quot;&quot;&quot;</span>
-</span><span id="L-15"><a href="#L-15"><span class="linenos"> 15</span></a>    <span class="n">files</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="n">path</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.*&quot;</span><span class="p">))</span> <span class="k">if</span> <span class="n">recursive</span> <span class="k">else</span> <span class="nb">list</span><span class="p">(</span><span class="n">path</span><span class="o">.</span><span class="n">glob</span><span class="p">(</span><span class="s2">&quot;*.*&quot;</span><span class="p">))</span>
-</span><span id="L-16"><a href="#L-16"><span class="linenos"> 16</span></a>    <span class="n">matching_sets</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="L-17"><a href="#L-17"><span class="linenos"> 17</span></a>    <span class="k">while</span> <span class="nb">len</span><span class="p">(</span><span class="n">files</span><span class="p">)</span> <span class="o">&gt;</span> <span class="mi">0</span><span class="p">:</span>
-</span><span id="L-18"><a href="#L-18"><span class="linenos"> 18</span></a>        <span class="n">comparee</span> <span class="o">=</span> <span class="n">files</span><span class="o">.</span><span class="n">pop</span><span class="p">()</span>
-</span><span id="L-19"><a href="#L-19"><span class="linenos"> 19</span></a>        <span class="n">matching_files</span> <span class="o">=</span> <span class="p">[</span><span class="n">file</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">files</span> <span class="k">if</span> <span class="n">filecmp</span><span class="o">.</span><span class="n">cmp</span><span class="p">(</span><span class="n">comparee</span><span class="p">,</span> <span class="n">file</span><span class="p">,</span> <span class="kc">False</span><span class="p">)]</span>
-</span><span id="L-20"><a href="#L-20"><span class="linenos"> 20</span></a>        <span class="k">if</span> <span class="n">matching_files</span><span class="p">:</span>
-</span><span id="L-21"><a href="#L-21"><span class="linenos"> 21</span></a>            <span class="p">[</span><span class="n">files</span><span class="o">.</span><span class="n">pop</span><span class="p">(</span><span class="n">files</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="n">file</span><span class="p">))</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">matching_files</span><span class="p">]</span>
-</span><span id="L-22"><a href="#L-22"><span class="linenos"> 22</span></a>            <span class="n">matching_files</span><span class="o">.</span><span class="n">insert</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="n">comparee</span><span class="p">)</span>
-</span><span id="L-23"><a href="#L-23"><span class="linenos"> 23</span></a>            <span class="n">matching_sets</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">matching_files</span><span class="p">)</span>
-</span><span id="L-24"><a href="#L-24"><span class="linenos"> 24</span></a>    <span class="k">return</span> <span class="n">matching_sets</span>
+</span><span id="L-5"><a href="#L-5"><span class="linenos">  5</span></a><span class="kn">from</span> <span class="nn">itertools</span> <span class="kn">import</span> <span class="n">combinations</span>
+</span><span id="L-6"><a href="#L-6"><span class="linenos">  6</span></a>
+</span><span id="L-7"><a href="#L-7"><span class="linenos">  7</span></a><span class="kn">from</span> <span class="nn">griddle</span> <span class="kn">import</span> <span class="n">griddy</span>
+</span><span id="L-8"><a href="#L-8"><span class="linenos">  8</span></a><span class="kn">from</span> <span class="nn">pathier</span> <span class="kn">import</span> <span class="n">Pathier</span>
+</span><span id="L-9"><a href="#L-9"><span class="linenos">  9</span></a><span class="kn">from</span> <span class="nn">printbuddies</span> <span class="kn">import</span> <span class="n">Spinner</span>
+</span><span id="L-10"><a href="#L-10"><span class="linenos"> 10</span></a><span class="kn">from</span> <span class="nn">younotyou</span> <span class="kn">import</span> <span class="n">younotyou</span>
+</span><span id="L-11"><a href="#L-11"><span class="linenos"> 11</span></a>
+</span><span id="L-12"><a href="#L-12"><span class="linenos"> 12</span></a>
+</span><span id="L-13"><a href="#L-13"><span class="linenos"> 13</span></a><span class="k">def</span> <span class="nf">get_duplicates</span><span class="p">(</span><span class="n">paths</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">Pathier</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">Pathier</span><span class="p">]]:</span>
+</span><span id="L-14"><a href="#L-14"><span class="linenos"> 14</span></a>    <span class="sd">&quot;&quot;&quot;Return a list of lists for duplicate files in `paths`.&quot;&quot;&quot;</span>
+</span><span id="L-15"><a href="#L-15"><span class="linenos"> 15</span></a>    <span class="n">matching_sets</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="L-16"><a href="#L-16"><span class="linenos"> 16</span></a>    <span class="k">while</span> <span class="nb">len</span><span class="p">(</span><span class="n">paths</span><span class="p">)</span> <span class="o">&gt;</span> <span class="mi">0</span><span class="p">:</span>
+</span><span id="L-17"><a href="#L-17"><span class="linenos"> 17</span></a>        <span class="n">comparee</span> <span class="o">=</span> <span class="n">paths</span><span class="o">.</span><span class="n">pop</span><span class="p">()</span>
+</span><span id="L-18"><a href="#L-18"><span class="linenos"> 18</span></a>        <span class="n">matching_files</span> <span class="o">=</span> <span class="p">[</span><span class="n">file</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">paths</span> <span class="k">if</span> <span class="n">filecmp</span><span class="o">.</span><span class="n">cmp</span><span class="p">(</span><span class="n">comparee</span><span class="p">,</span> <span class="n">file</span><span class="p">,</span> <span class="kc">False</span><span class="p">)]</span>
+</span><span id="L-19"><a href="#L-19"><span class="linenos"> 19</span></a>        <span class="k">if</span> <span class="n">matching_files</span><span class="p">:</span>
+</span><span id="L-20"><a href="#L-20"><span class="linenos"> 20</span></a>            <span class="p">[</span><span class="n">paths</span><span class="o">.</span><span class="n">pop</span><span class="p">(</span><span class="n">paths</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="n">file</span><span class="p">))</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">matching_files</span><span class="p">]</span>
+</span><span id="L-21"><a href="#L-21"><span class="linenos"> 21</span></a>            <span class="n">matching_files</span><span class="o">.</span><span class="n">insert</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="n">comparee</span><span class="p">)</span>
+</span><span id="L-22"><a href="#L-22"><span class="linenos"> 22</span></a>            <span class="n">matching_sets</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">matching_files</span><span class="p">)</span>
+</span><span id="L-23"><a href="#L-23"><span class="linenos"> 23</span></a>    <span class="k">return</span> <span class="n">matching_sets</span>
+</span><span id="L-24"><a href="#L-24"><span class="linenos"> 24</span></a>
 </span><span id="L-25"><a href="#L-25"><span class="linenos"> 25</span></a>
-</span><span id="L-26"><a href="#L-26"><span class="linenos"> 26</span></a>
-</span><span id="L-27"><a href="#L-27"><span class="linenos"> 27</span></a><span class="k">def</span> <span class="nf">get_args</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">:</span>
-</span><span id="L-28"><a href="#L-28"><span class="linenos"> 28</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
-</span><span id="L-29"><a href="#L-29"><span class="linenos"> 29</span></a>
-</span><span id="L-30"><a href="#L-30"><span class="linenos"> 30</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-31"><a href="#L-31"><span class="linenos"> 31</span></a>        <span class="s2">&quot;-r&quot;</span><span class="p">,</span>
-</span><span id="L-32"><a href="#L-32"><span class="linenos"> 32</span></a>        <span class="s2">&quot;--recursive&quot;</span><span class="p">,</span>
-</span><span id="L-33"><a href="#L-33"><span class="linenos"> 33</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="L-34"><a href="#L-34"><span class="linenos"> 34</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Glob files to compare recursively. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-35"><a href="#L-35"><span class="linenos"> 35</span></a>    <span class="p">)</span>
-</span><span id="L-36"><a href="#L-36"><span class="linenos"> 36</span></a>
-</span><span id="L-37"><a href="#L-37"><span class="linenos"> 37</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-38"><a href="#L-38"><span class="linenos"> 38</span></a>        <span class="s2">&quot;-d&quot;</span><span class="p">,</span>
-</span><span id="L-39"><a href="#L-39"><span class="linenos"> 39</span></a>        <span class="s2">&quot;--delete_dupes&quot;</span><span class="p">,</span>
-</span><span id="L-40"><a href="#L-40"><span class="linenos"> 40</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="L-41"><a href="#L-41"><span class="linenos"> 41</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; After finding duplicates, delete all but one copy.</span>
-</span><span id="L-42"><a href="#L-42"><span class="linenos"> 42</span></a><span class="s2">        For each set of duplicates, the tool will ask you to enter the number corresponding to the copy you want to keep.</span>
-</span><span id="L-43"><a href="#L-43"><span class="linenos"> 43</span></a><span class="s2">        Pressing &#39;enter&#39; without entering a number will skip that set without deleting anything.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-26"><a href="#L-26"><span class="linenos"> 26</span></a><span class="k">def</span> <span class="nf">get_args</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">:</span>
+</span><span id="L-27"><a href="#L-27"><span class="linenos"> 27</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
+</span><span id="L-28"><a href="#L-28"><span class="linenos"> 28</span></a>
+</span><span id="L-29"><a href="#L-29"><span class="linenos"> 29</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-30"><a href="#L-30"><span class="linenos"> 30</span></a>        <span class="s2">&quot;-r&quot;</span><span class="p">,</span>
+</span><span id="L-31"><a href="#L-31"><span class="linenos"> 31</span></a>        <span class="s2">&quot;--recursive&quot;</span><span class="p">,</span>
+</span><span id="L-32"><a href="#L-32"><span class="linenos"> 32</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="L-33"><a href="#L-33"><span class="linenos"> 33</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Glob files to compare recursively. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-34"><a href="#L-34"><span class="linenos"> 34</span></a>    <span class="p">)</span>
+</span><span id="L-35"><a href="#L-35"><span class="linenos"> 35</span></a>
+</span><span id="L-36"><a href="#L-36"><span class="linenos"> 36</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-37"><a href="#L-37"><span class="linenos"> 37</span></a>        <span class="s2">&quot;-i&quot;</span><span class="p">,</span>
+</span><span id="L-38"><a href="#L-38"><span class="linenos"> 38</span></a>        <span class="s2">&quot;--ignores&quot;</span><span class="p">,</span>
+</span><span id="L-39"><a href="#L-39"><span class="linenos"> 39</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="L-40"><a href="#L-40"><span class="linenos"> 40</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;*&quot;</span><span class="p">,</span>
+</span><span id="L-41"><a href="#L-41"><span class="linenos"> 41</span></a>        <span class="n">default</span><span class="o">=</span><span class="p">[],</span>
+</span><span id="L-42"><a href="#L-42"><span class="linenos"> 42</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Ignore files matching these patterns.</span>
+</span><span id="L-43"><a href="#L-43"><span class="linenos"> 43</span></a><span class="s2">        e.g. `dupechecker -i *.wav` will compare all files in the current working directory except .wav files.&quot;&quot;&quot;</span><span class="p">,</span>
 </span><span id="L-44"><a href="#L-44"><span class="linenos"> 44</span></a>    <span class="p">)</span>
 </span><span id="L-45"><a href="#L-45"><span class="linenos"> 45</span></a>
 </span><span id="L-46"><a href="#L-46"><span class="linenos"> 46</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-47"><a href="#L-47"><span class="linenos"> 47</span></a>        <span class="s2">&quot;-ad&quot;</span><span class="p">,</span>
-</span><span id="L-48"><a href="#L-48"><span class="linenos"> 48</span></a>        <span class="s2">&quot;--autodelete&quot;</span><span class="p">,</span>
+</span><span id="L-47"><a href="#L-47"><span class="linenos"> 47</span></a>        <span class="s2">&quot;-d&quot;</span><span class="p">,</span>
+</span><span id="L-48"><a href="#L-48"><span class="linenos"> 48</span></a>        <span class="s2">&quot;--delete_dupes&quot;</span><span class="p">,</span>
 </span><span id="L-49"><a href="#L-49"><span class="linenos"> 49</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="L-50"><a href="#L-50"><span class="linenos"> 50</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Automatically decide which file to keep and which to delete from each set of duplicate files instead of asking which to keep. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-51"><a href="#L-51"><span class="linenos"> 51</span></a>    <span class="p">)</span>
-</span><span id="L-52"><a href="#L-52"><span class="linenos"> 52</span></a>
-</span><span id="L-53"><a href="#L-53"><span class="linenos"> 53</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-54"><a href="#L-54"><span class="linenos"> 54</span></a>        <span class="s2">&quot;-ns&quot;</span><span class="p">,</span>
-</span><span id="L-55"><a href="#L-55"><span class="linenos"> 55</span></a>        <span class="s2">&quot;--no_show&quot;</span><span class="p">,</span>
-</span><span id="L-56"><a href="#L-56"><span class="linenos"> 56</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="L-57"><a href="#L-57"><span class="linenos"> 57</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Don&#39;t show printout of matching files. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-58"><a href="#L-58"><span class="linenos"> 58</span></a>    <span class="p">)</span>
-</span><span id="L-59"><a href="#L-59"><span class="linenos"> 59</span></a>
-</span><span id="L-60"><a href="#L-60"><span class="linenos"> 60</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-61"><a href="#L-61"><span class="linenos"> 61</span></a>        <span class="s2">&quot;path&quot;</span><span class="p">,</span>
-</span><span id="L-62"><a href="#L-62"><span class="linenos"> 62</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="L-63"><a href="#L-63"><span class="linenos"> 63</span></a>        <span class="n">default</span><span class="o">=</span><span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">(),</span>
-</span><span id="L-64"><a href="#L-64"><span class="linenos"> 64</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;?&quot;</span><span class="p">,</span>
-</span><span id="L-65"><a href="#L-65"><span class="linenos"> 65</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The path to compare files in. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-66"><a href="#L-66"><span class="linenos"> 66</span></a>    <span class="p">)</span>
-</span><span id="L-67"><a href="#L-67"><span class="linenos"> 67</span></a>
-</span><span id="L-68"><a href="#L-68"><span class="linenos"> 68</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
-</span><span id="L-69"><a href="#L-69"><span class="linenos"> 69</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">path</span> <span class="o">==</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">():</span>
-</span><span id="L-70"><a href="#L-70"><span class="linenos"> 70</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">path</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">path</span><span class="p">)</span>
-</span><span id="L-71"><a href="#L-71"><span class="linenos"> 71</span></a>
-</span><span id="L-72"><a href="#L-72"><span class="linenos"> 72</span></a>    <span class="k">return</span> <span class="n">args</span>
-</span><span id="L-73"><a href="#L-73"><span class="linenos"> 73</span></a>
-</span><span id="L-74"><a href="#L-74"><span class="linenos"> 74</span></a>
-</span><span id="L-75"><a href="#L-75"><span class="linenos"> 75</span></a><span class="k">def</span> <span class="nf">delete_wizard</span><span class="p">(</span><span class="n">matches</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">Pathier</span><span class="p">]]):</span>
-</span><span id="L-76"><a href="#L-76"><span class="linenos"> 76</span></a>    <span class="sd">&quot;&quot;&quot;Ask which file to keep for each set.&quot;&quot;&quot;</span>
-</span><span id="L-77"><a href="#L-77"><span class="linenos"> 77</span></a>    <span class="nb">print</span><span class="p">()</span>
-</span><span id="L-78"><a href="#L-78"><span class="linenos"> 78</span></a>    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Enter the corresponding number of the file to keep.&quot;</span><span class="p">)</span>
-</span><span id="L-79"><a href="#L-79"><span class="linenos"> 79</span></a>    <span class="nb">print</span><span class="p">(</span>
-</span><span id="L-80"><a href="#L-80"><span class="linenos"> 80</span></a>        <span class="s2">&quot;Press &#39;Enter&#39; without giving a number to skip deleting any files for the given set.&quot;</span>
-</span><span id="L-81"><a href="#L-81"><span class="linenos"> 81</span></a>    <span class="p">)</span>
-</span><span id="L-82"><a href="#L-82"><span class="linenos"> 82</span></a>    <span class="nb">print</span><span class="p">()</span>
-</span><span id="L-83"><a href="#L-83"><span class="linenos"> 83</span></a>    <span class="k">for</span> <span class="n">match</span> <span class="ow">in</span> <span class="n">matches</span><span class="p">:</span>
-</span><span id="L-84"><a href="#L-84"><span class="linenos"> 84</span></a>        <span class="n">map_</span> <span class="o">=</span> <span class="p">{</span><span class="nb">str</span><span class="p">(</span><span class="n">i</span><span class="p">):</span> <span class="n">file</span> <span class="k">for</span> <span class="n">i</span><span class="p">,</span> <span class="n">file</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">match</span><span class="p">,</span> <span class="mi">1</span><span class="p">)}</span>
-</span><span id="L-85"><a href="#L-85"><span class="linenos"> 85</span></a>        <span class="n">options</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;(</span><span class="si">{</span><span class="n">i</span><span class="si">}</span><span class="s2">) </span><span class="si">{</span><span class="n">file</span><span class="si">}</span><span class="s2">&quot;</span> <span class="k">for</span> <span class="n">i</span><span class="p">,</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">map_</span><span class="o">.</span><span class="n">items</span><span class="p">())</span> <span class="o">+</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span>
-</span><span id="L-86"><a href="#L-86"><span class="linenos"> 86</span></a>        <span class="nb">print</span><span class="p">(</span><span class="n">options</span><span class="p">)</span>
-</span><span id="L-87"><a href="#L-87"><span class="linenos"> 87</span></a>        <span class="n">keeper</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Enter number of file to keep (</span><span class="si">{</span><span class="s1">&#39;, &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">map_</span><span class="o">.</span><span class="n">keys</span><span class="p">())</span><span class="si">}</span><span class="s2">): &quot;</span><span class="p">)</span>
-</span><span id="L-88"><a href="#L-88"><span class="linenos"> 88</span></a>        <span class="k">if</span> <span class="n">keeper</span><span class="p">:</span>
-</span><span id="L-89"><a href="#L-89"><span class="linenos"> 89</span></a>            <span class="p">[</span><span class="n">map_</span><span class="p">[</span><span class="n">num</span><span class="p">]</span><span class="o">.</span><span class="n">delete</span><span class="p">()</span> <span class="k">for</span> <span class="n">num</span> <span class="ow">in</span> <span class="n">map_</span> <span class="k">if</span> <span class="n">num</span> <span class="o">!=</span> <span class="n">keeper</span><span class="p">]</span>
-</span><span id="L-90"><a href="#L-90"><span class="linenos"> 90</span></a>
+</span><span id="L-50"><a href="#L-50"><span class="linenos"> 50</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; After finding duplicates, delete all but one copy.</span>
+</span><span id="L-51"><a href="#L-51"><span class="linenos"> 51</span></a><span class="s2">        For each set of duplicates, the tool will ask you to enter the number corresponding to the copy you want to keep.</span>
+</span><span id="L-52"><a href="#L-52"><span class="linenos"> 52</span></a><span class="s2">        Pressing &#39;enter&#39; without entering a number will skip that set without deleting anything.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-53"><a href="#L-53"><span class="linenos"> 53</span></a>    <span class="p">)</span>
+</span><span id="L-54"><a href="#L-54"><span class="linenos"> 54</span></a>
+</span><span id="L-55"><a href="#L-55"><span class="linenos"> 55</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-56"><a href="#L-56"><span class="linenos"> 56</span></a>        <span class="s2">&quot;-ad&quot;</span><span class="p">,</span>
+</span><span id="L-57"><a href="#L-57"><span class="linenos"> 57</span></a>        <span class="s2">&quot;--autodelete&quot;</span><span class="p">,</span>
+</span><span id="L-58"><a href="#L-58"><span class="linenos"> 58</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="L-59"><a href="#L-59"><span class="linenos"> 59</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Automatically decide which file to keep and which to delete from each set of duplicate files instead of asking which to keep. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-60"><a href="#L-60"><span class="linenos"> 60</span></a>    <span class="p">)</span>
+</span><span id="L-61"><a href="#L-61"><span class="linenos"> 61</span></a>
+</span><span id="L-62"><a href="#L-62"><span class="linenos"> 62</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-63"><a href="#L-63"><span class="linenos"> 63</span></a>        <span class="s2">&quot;-ns&quot;</span><span class="p">,</span>
+</span><span id="L-64"><a href="#L-64"><span class="linenos"> 64</span></a>        <span class="s2">&quot;--no_show&quot;</span><span class="p">,</span>
+</span><span id="L-65"><a href="#L-65"><span class="linenos"> 65</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="L-66"><a href="#L-66"><span class="linenos"> 66</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Don&#39;t show printout of matching files. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-67"><a href="#L-67"><span class="linenos"> 67</span></a>    <span class="p">)</span>
+</span><span id="L-68"><a href="#L-68"><span class="linenos"> 68</span></a>
+</span><span id="L-69"><a href="#L-69"><span class="linenos"> 69</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-70"><a href="#L-70"><span class="linenos"> 70</span></a>        <span class="s2">&quot;paths&quot;</span><span class="p">,</span>
+</span><span id="L-71"><a href="#L-71"><span class="linenos"> 71</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="L-72"><a href="#L-72"><span class="linenos"> 72</span></a>        <span class="n">default</span><span class="o">=</span><span class="p">[</span><span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()],</span>
+</span><span id="L-73"><a href="#L-73"><span class="linenos"> 73</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;*&quot;</span><span class="p">,</span>
+</span><span id="L-74"><a href="#L-74"><span class="linenos"> 74</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The paths to compare files in. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-75"><a href="#L-75"><span class="linenos"> 75</span></a>    <span class="p">)</span>
+</span><span id="L-76"><a href="#L-76"><span class="linenos"> 76</span></a>
+</span><span id="L-77"><a href="#L-77"><span class="linenos"> 77</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
+</span><span id="L-78"><a href="#L-78"><span class="linenos"> 78</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">paths</span> <span class="o">==</span> <span class="p">[</span><span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()]:</span>
+</span><span id="L-79"><a href="#L-79"><span class="linenos"> 79</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">paths</span> <span class="o">=</span> <span class="p">[</span><span class="n">Pathier</span><span class="p">(</span><span class="n">path</span><span class="p">)</span> <span class="k">for</span> <span class="n">path</span> <span class="ow">in</span> <span class="n">args</span><span class="o">.</span><span class="n">paths</span><span class="p">]</span>
+</span><span id="L-80"><a href="#L-80"><span class="linenos"> 80</span></a>    <span class="n">files</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="L-81"><a href="#L-81"><span class="linenos"> 81</span></a>    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Gathering files...&quot;</span><span class="p">)</span>
+</span><span id="L-82"><a href="#L-82"><span class="linenos"> 82</span></a>    <span class="k">for</span> <span class="n">path</span> <span class="ow">in</span> <span class="n">args</span><span class="o">.</span><span class="n">paths</span><span class="p">:</span>
+</span><span id="L-83"><a href="#L-83"><span class="linenos"> 83</span></a>        <span class="n">files</span><span class="o">.</span><span class="n">extend</span><span class="p">(</span>
+</span><span id="L-84"><a href="#L-84"><span class="linenos"> 84</span></a>            <span class="nb">list</span><span class="p">(</span><span class="n">path</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.*&quot;</span><span class="p">))</span> <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">recursive</span> <span class="k">else</span> <span class="nb">list</span><span class="p">(</span><span class="n">path</span><span class="o">.</span><span class="n">glob</span><span class="p">(</span><span class="s2">&quot;*.*&quot;</span><span class="p">))</span>
+</span><span id="L-85"><a href="#L-85"><span class="linenos"> 85</span></a>        <span class="p">)</span>
+</span><span id="L-86"><a href="#L-86"><span class="linenos"> 86</span></a>    <span class="n">args</span><span class="o">.</span><span class="n">paths</span> <span class="o">=</span> <span class="n">younotyou</span><span class="p">([</span><span class="nb">str</span><span class="p">(</span><span class="n">file</span><span class="p">)</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">files</span><span class="p">],</span> <span class="n">exclude_patterns</span><span class="o">=</span><span class="n">args</span><span class="o">.</span><span class="n">ignores</span><span class="p">)</span>
+</span><span id="L-87"><a href="#L-87"><span class="linenos"> 87</span></a>    <span class="n">num_comparisons</span> <span class="o">=</span> <span class="nb">len</span><span class="p">(</span><span class="nb">list</span><span class="p">(</span><span class="n">combinations</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">paths</span><span class="p">,</span> <span class="mi">2</span><span class="p">)))</span>
+</span><span id="L-88"><a href="#L-88"><span class="linenos"> 88</span></a>    <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Making </span><span class="si">{</span><span class="n">num_comparisons</span><span class="si">}</span><span class="s2"> comparisons between </span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">paths</span><span class="p">)</span><span class="si">}</span><span class="s2"> files...&quot;</span><span class="p">)</span>
+</span><span id="L-89"><a href="#L-89"><span class="linenos"> 89</span></a>
+</span><span id="L-90"><a href="#L-90"><span class="linenos"> 90</span></a>    <span class="k">return</span> <span class="n">args</span>
 </span><span id="L-91"><a href="#L-91"><span class="linenos"> 91</span></a>
-</span><span id="L-92"><a href="#L-92"><span class="linenos"> 92</span></a><span class="k">def</span> <span class="nf">autodelete</span><span class="p">(</span><span class="n">matches</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">Pathier</span><span class="p">]]):</span>
-</span><span id="L-93"><a href="#L-93"><span class="linenos"> 93</span></a>    <span class="sd">&quot;&quot;&quot;Keep one of each set in `matches` and delete the others.&quot;&quot;&quot;</span>
-</span><span id="L-94"><a href="#L-94"><span class="linenos"> 94</span></a>    <span class="k">for</span> <span class="n">match</span> <span class="ow">in</span> <span class="n">matches</span><span class="p">:</span>
-</span><span id="L-95"><a href="#L-95"><span class="linenos"> 95</span></a>        <span class="k">match</span><span class="o">.</span><span class="n">pop</span><span class="p">()</span>
-</span><span id="L-96"><a href="#L-96"><span class="linenos"> 96</span></a>        <span class="p">[</span><span class="n">file</span><span class="o">.</span><span class="n">delete</span><span class="p">()</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">match</span><span class="p">]</span>
-</span><span id="L-97"><a href="#L-97"><span class="linenos"> 97</span></a>
-</span><span id="L-98"><a href="#L-98"><span class="linenos"> 98</span></a>
-</span><span id="L-99"><a href="#L-99"><span class="linenos"> 99</span></a><span class="k">def</span> <span class="nf">dupechecker</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
+</span><span id="L-92"><a href="#L-92"><span class="linenos"> 92</span></a>
+</span><span id="L-93"><a href="#L-93"><span class="linenos"> 93</span></a><span class="k">def</span> <span class="nf">delete_wizard</span><span class="p">(</span><span class="n">matches</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">Pathier</span><span class="p">]]):</span>
+</span><span id="L-94"><a href="#L-94"><span class="linenos"> 94</span></a>    <span class="sd">&quot;&quot;&quot;Ask which file to keep for each set.&quot;&quot;&quot;</span>
+</span><span id="L-95"><a href="#L-95"><span class="linenos"> 95</span></a>    <span class="nb">print</span><span class="p">()</span>
+</span><span id="L-96"><a href="#L-96"><span class="linenos"> 96</span></a>    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Enter the corresponding number of the file to keep.&quot;</span><span class="p">)</span>
+</span><span id="L-97"><a href="#L-97"><span class="linenos"> 97</span></a>    <span class="nb">print</span><span class="p">(</span>
+</span><span id="L-98"><a href="#L-98"><span class="linenos"> 98</span></a>        <span class="s2">&quot;Press &#39;Enter&#39; without giving a number to skip deleting any files for the given set.&quot;</span>
+</span><span id="L-99"><a href="#L-99"><span class="linenos"> 99</span></a>    <span class="p">)</span>
 </span><span id="L-100"><a href="#L-100"><span class="linenos">100</span></a>    <span class="nb">print</span><span class="p">()</span>
-</span><span id="L-101"><a href="#L-101"><span class="linenos">101</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
-</span><span id="L-102"><a href="#L-102"><span class="linenos">102</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
-</span><span id="L-103"><a href="#L-103"><span class="linenos">103</span></a>    <span class="n">s</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="L-104"><a href="#L-104"><span class="linenos">104</span></a>        <span class="n">ch</span><span class="o">.</span><span class="n">rjust</span><span class="p">(</span><span class="n">i</span> <span class="o">+</span> <span class="n">j</span><span class="p">)</span>
-</span><span id="L-105"><a href="#L-105"><span class="linenos">105</span></a>        <span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="mi">1</span><span class="p">,</span> <span class="mi">25</span><span class="p">,</span> <span class="mi">3</span><span class="p">)</span>
-</span><span id="L-106"><a href="#L-106"><span class="linenos">106</span></a>        <span class="k">for</span> <span class="n">j</span><span class="p">,</span> <span class="n">ch</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">([</span><span class="s2">&quot;/&quot;</span><span class="p">,</span> <span class="s2">&quot;-&quot;</span><span class="p">,</span> <span class="s2">&quot;</span><span class="se">\\</span><span class="s2">&quot;</span><span class="p">])</span>
-</span><span id="L-107"><a href="#L-107"><span class="linenos">107</span></a>    <span class="p">]</span>
-</span><span id="L-108"><a href="#L-108"><span class="linenos">108</span></a>    <span class="n">s</span> <span class="o">+=</span> <span class="n">s</span><span class="p">[::</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span>
-</span><span id="L-109"><a href="#L-109"><span class="linenos">109</span></a>    <span class="k">with</span> <span class="n">Spinner</span><span class="p">(</span><span class="n">s</span><span class="p">)</span> <span class="k">as</span> <span class="n">spinner</span><span class="p">:</span>
-</span><span id="L-110"><a href="#L-110"><span class="linenos">110</span></a>        <span class="k">with</span> <span class="n">ThreadPoolExecutor</span><span class="p">()</span> <span class="k">as</span> <span class="n">exc</span><span class="p">:</span>
-</span><span id="L-111"><a href="#L-111"><span class="linenos">111</span></a>            <span class="n">thread</span> <span class="o">=</span> <span class="n">exc</span><span class="o">.</span><span class="n">submit</span><span class="p">(</span><span class="n">get_duplicates</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">path</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">recursive</span><span class="p">)</span>
-</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a>            <span class="k">while</span> <span class="ow">not</span> <span class="n">thread</span><span class="o">.</span><span class="n">done</span><span class="p">():</span>
-</span><span id="L-113"><a href="#L-113"><span class="linenos">113</span></a>                <span class="n">spinner</span><span class="o">.</span><span class="n">display</span><span class="p">()</span>
-</span><span id="L-114"><a href="#L-114"><span class="linenos">114</span></a>                <span class="n">time</span><span class="o">.</span><span class="n">sleep</span><span class="p">(</span><span class="mf">0.025</span><span class="p">)</span>
-</span><span id="L-115"><a href="#L-115"><span class="linenos">115</span></a>            <span class="n">matches</span> <span class="o">=</span> <span class="n">thread</span><span class="o">.</span><span class="n">result</span><span class="p">()</span>
-</span><span id="L-116"><a href="#L-116"><span class="linenos">116</span></a>    <span class="k">if</span> <span class="n">matches</span><span class="p">:</span>
-</span><span id="L-117"><a href="#L-117"><span class="linenos">117</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Found </span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="n">matches</span><span class="p">)</span><span class="si">}</span><span class="s2"> duplicate sets of files.&quot;</span><span class="p">)</span>
-</span><span id="L-118"><a href="#L-118"><span class="linenos">118</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">no_show</span><span class="p">:</span>
-</span><span id="L-119"><a href="#L-119"><span class="linenos">119</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">griddy</span><span class="p">(</span><span class="n">matches</span><span class="p">))</span>
-</span><span id="L-120"><a href="#L-120"><span class="linenos">120</span></a>        <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">delete_dupes</span> <span class="ow">or</span> <span class="n">args</span><span class="o">.</span><span class="n">autodelete</span><span class="p">:</span>
-</span><span id="L-121"><a href="#L-121"><span class="linenos">121</span></a>            <span class="n">size</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">size</span><span class="p">()</span>
-</span><span id="L-122"><a href="#L-122"><span class="linenos">122</span></a>            <span class="n">delete_wizard</span><span class="p">(</span><span class="n">matches</span><span class="p">)</span> <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">delete_dupes</span> <span class="k">else</span> <span class="n">autodelete</span><span class="p">(</span><span class="n">matches</span><span class="p">)</span>
-</span><span id="L-123"><a href="#L-123"><span class="linenos">123</span></a>            <span class="n">deleted_size</span> <span class="o">=</span> <span class="n">size</span> <span class="o">-</span> <span class="n">args</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">size</span><span class="p">()</span>
-</span><span id="L-124"><a href="#L-124"><span class="linenos">124</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Deleted </span><span class="si">{</span><span class="n">Pathier</span><span class="o">.</span><span class="n">format_size</span><span class="p">(</span><span class="n">deleted_size</span><span class="p">)</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
-</span><span id="L-125"><a href="#L-125"><span class="linenos">125</span></a>    <span class="k">else</span><span class="p">:</span>
-</span><span id="L-126"><a href="#L-126"><span class="linenos">126</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;No duplicates detected.&quot;</span><span class="p">)</span>
-</span><span id="L-127"><a href="#L-127"><span class="linenos">127</span></a>
-</span><span id="L-128"><a href="#L-128"><span class="linenos">128</span></a>
-</span><span id="L-129"><a href="#L-129"><span class="linenos">129</span></a><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
-</span><span id="L-130"><a href="#L-130"><span class="linenos">130</span></a>    <span class="n">dupechecker</span><span class="p">(</span><span class="n">get_args</span><span class="p">())</span>
+</span><span id="L-101"><a href="#L-101"><span class="linenos">101</span></a>    <span class="k">for</span> <span class="n">match</span> <span class="ow">in</span> <span class="n">matches</span><span class="p">:</span>
+</span><span id="L-102"><a href="#L-102"><span class="linenos">102</span></a>        <span class="n">map_</span> <span class="o">=</span> <span class="p">{</span><span class="nb">str</span><span class="p">(</span><span class="n">i</span><span class="p">):</span> <span class="n">file</span> <span class="k">for</span> <span class="n">i</span><span class="p">,</span> <span class="n">file</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">match</span><span class="p">,</span> <span class="mi">1</span><span class="p">)}</span>
+</span><span id="L-103"><a href="#L-103"><span class="linenos">103</span></a>        <span class="n">options</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;(</span><span class="si">{</span><span class="n">i</span><span class="si">}</span><span class="s2">) </span><span class="si">{</span><span class="n">file</span><span class="si">}</span><span class="s2">&quot;</span> <span class="k">for</span> <span class="n">i</span><span class="p">,</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">map_</span><span class="o">.</span><span class="n">items</span><span class="p">())</span> <span class="o">+</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span>
+</span><span id="L-104"><a href="#L-104"><span class="linenos">104</span></a>        <span class="nb">print</span><span class="p">(</span><span class="n">options</span><span class="p">)</span>
+</span><span id="L-105"><a href="#L-105"><span class="linenos">105</span></a>        <span class="n">keeper</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Enter number of file to keep (</span><span class="si">{</span><span class="s1">&#39;, &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">map_</span><span class="o">.</span><span class="n">keys</span><span class="p">())</span><span class="si">}</span><span class="s2">): &quot;</span><span class="p">)</span>
+</span><span id="L-106"><a href="#L-106"><span class="linenos">106</span></a>        <span class="k">if</span> <span class="n">keeper</span><span class="p">:</span>
+</span><span id="L-107"><a href="#L-107"><span class="linenos">107</span></a>            <span class="p">[</span><span class="n">map_</span><span class="p">[</span><span class="n">num</span><span class="p">]</span><span class="o">.</span><span class="n">delete</span><span class="p">()</span> <span class="k">for</span> <span class="n">num</span> <span class="ow">in</span> <span class="n">map_</span> <span class="k">if</span> <span class="n">num</span> <span class="o">!=</span> <span class="n">keeper</span><span class="p">]</span>
+</span><span id="L-108"><a href="#L-108"><span class="linenos">108</span></a>
+</span><span id="L-109"><a href="#L-109"><span class="linenos">109</span></a>
+</span><span id="L-110"><a href="#L-110"><span class="linenos">110</span></a><span class="k">def</span> <span class="nf">autodelete</span><span class="p">(</span><span class="n">matches</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">Pathier</span><span class="p">]]):</span>
+</span><span id="L-111"><a href="#L-111"><span class="linenos">111</span></a>    <span class="sd">&quot;&quot;&quot;Keep one of each set in `matches` and delete the others.&quot;&quot;&quot;</span>
+</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a>    <span class="k">for</span> <span class="n">match</span> <span class="ow">in</span> <span class="n">matches</span><span class="p">:</span>
+</span><span id="L-113"><a href="#L-113"><span class="linenos">113</span></a>        <span class="k">match</span><span class="o">.</span><span class="n">pop</span><span class="p">()</span>
+</span><span id="L-114"><a href="#L-114"><span class="linenos">114</span></a>        <span class="p">[</span><span class="n">file</span><span class="o">.</span><span class="n">delete</span><span class="p">()</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">match</span><span class="p">]</span>
+</span><span id="L-115"><a href="#L-115"><span class="linenos">115</span></a>
+</span><span id="L-116"><a href="#L-116"><span class="linenos">116</span></a>
+</span><span id="L-117"><a href="#L-117"><span class="linenos">117</span></a><span class="k">def</span> <span class="nf">dupechecker</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
+</span><span id="L-118"><a href="#L-118"><span class="linenos">118</span></a>    <span class="nb">print</span><span class="p">()</span>
+</span><span id="L-119"><a href="#L-119"><span class="linenos">119</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
+</span><span id="L-120"><a href="#L-120"><span class="linenos">120</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
+</span><span id="L-121"><a href="#L-121"><span class="linenos">121</span></a>    <span class="n">s</span> <span class="o">=</span> <span class="p">[</span>
+</span><span id="L-122"><a href="#L-122"><span class="linenos">122</span></a>        <span class="n">ch</span><span class="o">.</span><span class="n">rjust</span><span class="p">(</span><span class="n">i</span> <span class="o">+</span> <span class="n">j</span><span class="p">)</span>
+</span><span id="L-123"><a href="#L-123"><span class="linenos">123</span></a>        <span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="mi">1</span><span class="p">,</span> <span class="mi">25</span><span class="p">,</span> <span class="mi">3</span><span class="p">)</span>
+</span><span id="L-124"><a href="#L-124"><span class="linenos">124</span></a>        <span class="k">for</span> <span class="n">j</span><span class="p">,</span> <span class="n">ch</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">([</span><span class="s2">&quot;/&quot;</span><span class="p">,</span> <span class="s2">&quot;-&quot;</span><span class="p">,</span> <span class="s2">&quot;</span><span class="se">\\</span><span class="s2">&quot;</span><span class="p">])</span>
+</span><span id="L-125"><a href="#L-125"><span class="linenos">125</span></a>    <span class="p">]</span>
+</span><span id="L-126"><a href="#L-126"><span class="linenos">126</span></a>    <span class="n">s</span> <span class="o">+=</span> <span class="n">s</span><span class="p">[::</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span>
+</span><span id="L-127"><a href="#L-127"><span class="linenos">127</span></a>    <span class="k">with</span> <span class="n">Spinner</span><span class="p">(</span><span class="n">s</span><span class="p">)</span> <span class="k">as</span> <span class="n">spinner</span><span class="p">:</span>
+</span><span id="L-128"><a href="#L-128"><span class="linenos">128</span></a>        <span class="k">with</span> <span class="n">ThreadPoolExecutor</span><span class="p">()</span> <span class="k">as</span> <span class="n">exc</span><span class="p">:</span>
+</span><span id="L-129"><a href="#L-129"><span class="linenos">129</span></a>            <span class="n">thread</span> <span class="o">=</span> <span class="n">exc</span><span class="o">.</span><span class="n">submit</span><span class="p">(</span><span class="n">get_duplicates</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">paths</span><span class="p">)</span>
+</span><span id="L-130"><a href="#L-130"><span class="linenos">130</span></a>            <span class="k">while</span> <span class="ow">not</span> <span class="n">thread</span><span class="o">.</span><span class="n">done</span><span class="p">():</span>
+</span><span id="L-131"><a href="#L-131"><span class="linenos">131</span></a>                <span class="n">spinner</span><span class="o">.</span><span class="n">display</span><span class="p">()</span>
+</span><span id="L-132"><a href="#L-132"><span class="linenos">132</span></a>                <span class="n">time</span><span class="o">.</span><span class="n">sleep</span><span class="p">(</span><span class="mf">0.025</span><span class="p">)</span>
+</span><span id="L-133"><a href="#L-133"><span class="linenos">133</span></a>            <span class="n">matches</span> <span class="o">=</span> <span class="n">thread</span><span class="o">.</span><span class="n">result</span><span class="p">()</span>
+</span><span id="L-134"><a href="#L-134"><span class="linenos">134</span></a>    <span class="k">if</span> <span class="n">matches</span><span class="p">:</span>
+</span><span id="L-135"><a href="#L-135"><span class="linenos">135</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Found </span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="n">matches</span><span class="p">)</span><span class="si">}</span><span class="s2"> duplicate sets of files.&quot;</span><span class="p">)</span>
+</span><span id="L-136"><a href="#L-136"><span class="linenos">136</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">no_show</span><span class="p">:</span>
+</span><span id="L-137"><a href="#L-137"><span class="linenos">137</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">griddy</span><span class="p">(</span><span class="n">matches</span><span class="p">))</span>
+</span><span id="L-138"><a href="#L-138"><span class="linenos">138</span></a>        <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">delete_dupes</span> <span class="ow">or</span> <span class="n">args</span><span class="o">.</span><span class="n">autodelete</span><span class="p">:</span>
+</span><span id="L-139"><a href="#L-139"><span class="linenos">139</span></a>            <span class="n">size</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">size</span><span class="p">()</span>
+</span><span id="L-140"><a href="#L-140"><span class="linenos">140</span></a>            <span class="n">delete_wizard</span><span class="p">(</span><span class="n">matches</span><span class="p">)</span> <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">delete_dupes</span> <span class="k">else</span> <span class="n">autodelete</span><span class="p">(</span><span class="n">matches</span><span class="p">)</span>
+</span><span id="L-141"><a href="#L-141"><span class="linenos">141</span></a>            <span class="n">deleted_size</span> <span class="o">=</span> <span class="n">size</span> <span class="o">-</span> <span class="n">args</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">size</span><span class="p">()</span>
+</span><span id="L-142"><a href="#L-142"><span class="linenos">142</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Deleted </span><span class="si">{</span><span class="n">Pathier</span><span class="o">.</span><span class="n">format_size</span><span class="p">(</span><span class="n">deleted_size</span><span class="p">)</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+</span><span id="L-143"><a href="#L-143"><span class="linenos">143</span></a>    <span class="k">else</span><span class="p">:</span>
+</span><span id="L-144"><a href="#L-144"><span class="linenos">144</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;No duplicates detected.&quot;</span><span class="p">)</span>
+</span><span id="L-145"><a href="#L-145"><span class="linenos">145</span></a>
+</span><span id="L-146"><a href="#L-146"><span class="linenos">146</span></a>
+</span><span id="L-147"><a href="#L-147"><span class="linenos">147</span></a><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
+</span><span id="L-148"><a href="#L-148"><span class="linenos">148</span></a>    <span class="n">dupechecker</span><span class="p">(</span><span class="n">get_args</span><span class="p">())</span>
 </span></pre></div>
 
 
             </section>
                 <section id="get_duplicates">
                             <input id="get_duplicates-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
-        <span class="name">get_duplicates</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="n">path</span><span class="p">:</span> <span class="n">pathier</span><span class="o">.</span><span class="n">pathier</span><span class="o">.</span><span class="n">Pathier</span>,</span><span class="param">	<span class="n">recursive</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span></span><span class="return-annotation">) -> <span class="nb">list</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">pathier</span><span class="o">.</span><span class="n">pathier</span><span class="o">.</span><span class="n">Pathier</span><span class="p">]]</span>:</span></span>
+        <span class="name">get_duplicates</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="n">paths</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">pathier</span><span class="o">.</span><span class="n">pathier</span><span class="o">.</span><span class="n">Pathier</span><span class="p">]</span></span><span class="return-annotation">) -> <span class="nb">list</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">pathier</span><span class="o">.</span><span class="n">pathier</span><span class="o">.</span><span class="n">Pathier</span><span class="p">]]</span>:</span></span>
 
                 <label class="view-source-button" for="get_duplicates-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#get_duplicates"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="get_duplicates-12"><a href="#get_duplicates-12"><span class="linenos">12</span></a><span class="k">def</span> <span class="nf">get_duplicates</span><span class="p">(</span><span class="n">path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">,</span> <span class="n">recursive</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">Pathier</span><span class="p">]]:</span>
-</span><span id="get_duplicates-13"><a href="#get_duplicates-13"><span class="linenos">13</span></a>    <span class="sd">&quot;&quot;&quot;Return a list of lists for duplicate files in `path`.</span>
-</span><span id="get_duplicates-14"><a href="#get_duplicates-14"><span class="linenos">14</span></a><span class="sd">    Each sub-list will contain 2 or more files determined to be equivalent files.</span>
-</span><span id="get_duplicates-15"><a href="#get_duplicates-15"><span class="linenos">15</span></a><span class="sd">    If `recursive` is `True`, files from `path` and it&#39;s subdirectories will be compared.&quot;&quot;&quot;</span>
-</span><span id="get_duplicates-16"><a href="#get_duplicates-16"><span class="linenos">16</span></a>    <span class="n">files</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="n">path</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.*&quot;</span><span class="p">))</span> <span class="k">if</span> <span class="n">recursive</span> <span class="k">else</span> <span class="nb">list</span><span class="p">(</span><span class="n">path</span><span class="o">.</span><span class="n">glob</span><span class="p">(</span><span class="s2">&quot;*.*&quot;</span><span class="p">))</span>
-</span><span id="get_duplicates-17"><a href="#get_duplicates-17"><span class="linenos">17</span></a>    <span class="n">matching_sets</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="get_duplicates-18"><a href="#get_duplicates-18"><span class="linenos">18</span></a>    <span class="k">while</span> <span class="nb">len</span><span class="p">(</span><span class="n">files</span><span class="p">)</span> <span class="o">&gt;</span> <span class="mi">0</span><span class="p">:</span>
-</span><span id="get_duplicates-19"><a href="#get_duplicates-19"><span class="linenos">19</span></a>        <span class="n">comparee</span> <span class="o">=</span> <span class="n">files</span><span class="o">.</span><span class="n">pop</span><span class="p">()</span>
-</span><span id="get_duplicates-20"><a href="#get_duplicates-20"><span class="linenos">20</span></a>        <span class="n">matching_files</span> <span class="o">=</span> <span class="p">[</span><span class="n">file</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">files</span> <span class="k">if</span> <span class="n">filecmp</span><span class="o">.</span><span class="n">cmp</span><span class="p">(</span><span class="n">comparee</span><span class="p">,</span> <span class="n">file</span><span class="p">,</span> <span class="kc">False</span><span class="p">)]</span>
-</span><span id="get_duplicates-21"><a href="#get_duplicates-21"><span class="linenos">21</span></a>        <span class="k">if</span> <span class="n">matching_files</span><span class="p">:</span>
-</span><span id="get_duplicates-22"><a href="#get_duplicates-22"><span class="linenos">22</span></a>            <span class="p">[</span><span class="n">files</span><span class="o">.</span><span class="n">pop</span><span class="p">(</span><span class="n">files</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="n">file</span><span class="p">))</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">matching_files</span><span class="p">]</span>
-</span><span id="get_duplicates-23"><a href="#get_duplicates-23"><span class="linenos">23</span></a>            <span class="n">matching_files</span><span class="o">.</span><span class="n">insert</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="n">comparee</span><span class="p">)</span>
-</span><span id="get_duplicates-24"><a href="#get_duplicates-24"><span class="linenos">24</span></a>            <span class="n">matching_sets</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">matching_files</span><span class="p">)</span>
-</span><span id="get_duplicates-25"><a href="#get_duplicates-25"><span class="linenos">25</span></a>    <span class="k">return</span> <span class="n">matching_sets</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="get_duplicates-14"><a href="#get_duplicates-14"><span class="linenos">14</span></a><span class="k">def</span> <span class="nf">get_duplicates</span><span class="p">(</span><span class="n">paths</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">Pathier</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">Pathier</span><span class="p">]]:</span>
+</span><span id="get_duplicates-15"><a href="#get_duplicates-15"><span class="linenos">15</span></a>    <span class="sd">&quot;&quot;&quot;Return a list of lists for duplicate files in `paths`.&quot;&quot;&quot;</span>
+</span><span id="get_duplicates-16"><a href="#get_duplicates-16"><span class="linenos">16</span></a>    <span class="n">matching_sets</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="get_duplicates-17"><a href="#get_duplicates-17"><span class="linenos">17</span></a>    <span class="k">while</span> <span class="nb">len</span><span class="p">(</span><span class="n">paths</span><span class="p">)</span> <span class="o">&gt;</span> <span class="mi">0</span><span class="p">:</span>
+</span><span id="get_duplicates-18"><a href="#get_duplicates-18"><span class="linenos">18</span></a>        <span class="n">comparee</span> <span class="o">=</span> <span class="n">paths</span><span class="o">.</span><span class="n">pop</span><span class="p">()</span>
+</span><span id="get_duplicates-19"><a href="#get_duplicates-19"><span class="linenos">19</span></a>        <span class="n">matching_files</span> <span class="o">=</span> <span class="p">[</span><span class="n">file</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">paths</span> <span class="k">if</span> <span class="n">filecmp</span><span class="o">.</span><span class="n">cmp</span><span class="p">(</span><span class="n">comparee</span><span class="p">,</span> <span class="n">file</span><span class="p">,</span> <span class="kc">False</span><span class="p">)]</span>
+</span><span id="get_duplicates-20"><a href="#get_duplicates-20"><span class="linenos">20</span></a>        <span class="k">if</span> <span class="n">matching_files</span><span class="p">:</span>
+</span><span id="get_duplicates-21"><a href="#get_duplicates-21"><span class="linenos">21</span></a>            <span class="p">[</span><span class="n">paths</span><span class="o">.</span><span class="n">pop</span><span class="p">(</span><span class="n">paths</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="n">file</span><span class="p">))</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">matching_files</span><span class="p">]</span>
+</span><span id="get_duplicates-22"><a href="#get_duplicates-22"><span class="linenos">22</span></a>            <span class="n">matching_files</span><span class="o">.</span><span class="n">insert</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="n">comparee</span><span class="p">)</span>
+</span><span id="get_duplicates-23"><a href="#get_duplicates-23"><span class="linenos">23</span></a>            <span class="n">matching_sets</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">matching_files</span><span class="p">)</span>
+</span><span id="get_duplicates-24"><a href="#get_duplicates-24"><span class="linenos">24</span></a>    <span class="k">return</span> <span class="n">matching_sets</span>
 </span></pre></div>
 
 
-            <div class="docstring"><p>Return a list of lists for duplicate files in <code>path</code>.
-Each sub-list will contain 2 or more files determined to be equivalent files.
-If <code>recursive</code> is <code>True</code>, files from <code>path</code> and it's subdirectories will be compared.</p>
+            <div class="docstring"><p>Return a list of lists for duplicate files in <code>paths</code>.</p>
 </div>
 
 
                 </section>
                 <section id="get_args">
                             <input id="get_args-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -242,60 +255,79 @@
         <span class="def">def</span>
         <span class="name">get_args</span><span class="signature pdoc-code condensed">(<span class="return-annotation">) -> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span>:</span></span>
 
                 <label class="view-source-button" for="get_args-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#get_args"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="get_args-28"><a href="#get_args-28"><span class="linenos">28</span></a><span class="k">def</span> <span class="nf">get_args</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">:</span>
-</span><span id="get_args-29"><a href="#get_args-29"><span class="linenos">29</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
-</span><span id="get_args-30"><a href="#get_args-30"><span class="linenos">30</span></a>
-</span><span id="get_args-31"><a href="#get_args-31"><span class="linenos">31</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-32"><a href="#get_args-32"><span class="linenos">32</span></a>        <span class="s2">&quot;-r&quot;</span><span class="p">,</span>
-</span><span id="get_args-33"><a href="#get_args-33"><span class="linenos">33</span></a>        <span class="s2">&quot;--recursive&quot;</span><span class="p">,</span>
-</span><span id="get_args-34"><a href="#get_args-34"><span class="linenos">34</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="get_args-35"><a href="#get_args-35"><span class="linenos">35</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Glob files to compare recursively. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-36"><a href="#get_args-36"><span class="linenos">36</span></a>    <span class="p">)</span>
-</span><span id="get_args-37"><a href="#get_args-37"><span class="linenos">37</span></a>
-</span><span id="get_args-38"><a href="#get_args-38"><span class="linenos">38</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-39"><a href="#get_args-39"><span class="linenos">39</span></a>        <span class="s2">&quot;-d&quot;</span><span class="p">,</span>
-</span><span id="get_args-40"><a href="#get_args-40"><span class="linenos">40</span></a>        <span class="s2">&quot;--delete_dupes&quot;</span><span class="p">,</span>
-</span><span id="get_args-41"><a href="#get_args-41"><span class="linenos">41</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="get_args-42"><a href="#get_args-42"><span class="linenos">42</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; After finding duplicates, delete all but one copy.</span>
-</span><span id="get_args-43"><a href="#get_args-43"><span class="linenos">43</span></a><span class="s2">        For each set of duplicates, the tool will ask you to enter the number corresponding to the copy you want to keep.</span>
-</span><span id="get_args-44"><a href="#get_args-44"><span class="linenos">44</span></a><span class="s2">        Pressing &#39;enter&#39; without entering a number will skip that set without deleting anything.&quot;&quot;&quot;</span><span class="p">,</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="get_args-27"><a href="#get_args-27"><span class="linenos">27</span></a><span class="k">def</span> <span class="nf">get_args</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">:</span>
+</span><span id="get_args-28"><a href="#get_args-28"><span class="linenos">28</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
+</span><span id="get_args-29"><a href="#get_args-29"><span class="linenos">29</span></a>
+</span><span id="get_args-30"><a href="#get_args-30"><span class="linenos">30</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-31"><a href="#get_args-31"><span class="linenos">31</span></a>        <span class="s2">&quot;-r&quot;</span><span class="p">,</span>
+</span><span id="get_args-32"><a href="#get_args-32"><span class="linenos">32</span></a>        <span class="s2">&quot;--recursive&quot;</span><span class="p">,</span>
+</span><span id="get_args-33"><a href="#get_args-33"><span class="linenos">33</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="get_args-34"><a href="#get_args-34"><span class="linenos">34</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Glob files to compare recursively. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-35"><a href="#get_args-35"><span class="linenos">35</span></a>    <span class="p">)</span>
+</span><span id="get_args-36"><a href="#get_args-36"><span class="linenos">36</span></a>
+</span><span id="get_args-37"><a href="#get_args-37"><span class="linenos">37</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-38"><a href="#get_args-38"><span class="linenos">38</span></a>        <span class="s2">&quot;-i&quot;</span><span class="p">,</span>
+</span><span id="get_args-39"><a href="#get_args-39"><span class="linenos">39</span></a>        <span class="s2">&quot;--ignores&quot;</span><span class="p">,</span>
+</span><span id="get_args-40"><a href="#get_args-40"><span class="linenos">40</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="get_args-41"><a href="#get_args-41"><span class="linenos">41</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;*&quot;</span><span class="p">,</span>
+</span><span id="get_args-42"><a href="#get_args-42"><span class="linenos">42</span></a>        <span class="n">default</span><span class="o">=</span><span class="p">[],</span>
+</span><span id="get_args-43"><a href="#get_args-43"><span class="linenos">43</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Ignore files matching these patterns.</span>
+</span><span id="get_args-44"><a href="#get_args-44"><span class="linenos">44</span></a><span class="s2">        e.g. `dupechecker -i *.wav` will compare all files in the current working directory except .wav files.&quot;&quot;&quot;</span><span class="p">,</span>
 </span><span id="get_args-45"><a href="#get_args-45"><span class="linenos">45</span></a>    <span class="p">)</span>
 </span><span id="get_args-46"><a href="#get_args-46"><span class="linenos">46</span></a>
 </span><span id="get_args-47"><a href="#get_args-47"><span class="linenos">47</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-48"><a href="#get_args-48"><span class="linenos">48</span></a>        <span class="s2">&quot;-ad&quot;</span><span class="p">,</span>
-</span><span id="get_args-49"><a href="#get_args-49"><span class="linenos">49</span></a>        <span class="s2">&quot;--autodelete&quot;</span><span class="p">,</span>
+</span><span id="get_args-48"><a href="#get_args-48"><span class="linenos">48</span></a>        <span class="s2">&quot;-d&quot;</span><span class="p">,</span>
+</span><span id="get_args-49"><a href="#get_args-49"><span class="linenos">49</span></a>        <span class="s2">&quot;--delete_dupes&quot;</span><span class="p">,</span>
 </span><span id="get_args-50"><a href="#get_args-50"><span class="linenos">50</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="get_args-51"><a href="#get_args-51"><span class="linenos">51</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Automatically decide which file to keep and which to delete from each set of duplicate files instead of asking which to keep. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-52"><a href="#get_args-52"><span class="linenos">52</span></a>    <span class="p">)</span>
-</span><span id="get_args-53"><a href="#get_args-53"><span class="linenos">53</span></a>
-</span><span id="get_args-54"><a href="#get_args-54"><span class="linenos">54</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-55"><a href="#get_args-55"><span class="linenos">55</span></a>        <span class="s2">&quot;-ns&quot;</span><span class="p">,</span>
-</span><span id="get_args-56"><a href="#get_args-56"><span class="linenos">56</span></a>        <span class="s2">&quot;--no_show&quot;</span><span class="p">,</span>
-</span><span id="get_args-57"><a href="#get_args-57"><span class="linenos">57</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="get_args-58"><a href="#get_args-58"><span class="linenos">58</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Don&#39;t show printout of matching files. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-59"><a href="#get_args-59"><span class="linenos">59</span></a>    <span class="p">)</span>
-</span><span id="get_args-60"><a href="#get_args-60"><span class="linenos">60</span></a>
-</span><span id="get_args-61"><a href="#get_args-61"><span class="linenos">61</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-62"><a href="#get_args-62"><span class="linenos">62</span></a>        <span class="s2">&quot;path&quot;</span><span class="p">,</span>
-</span><span id="get_args-63"><a href="#get_args-63"><span class="linenos">63</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="get_args-64"><a href="#get_args-64"><span class="linenos">64</span></a>        <span class="n">default</span><span class="o">=</span><span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">(),</span>
-</span><span id="get_args-65"><a href="#get_args-65"><span class="linenos">65</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;?&quot;</span><span class="p">,</span>
-</span><span id="get_args-66"><a href="#get_args-66"><span class="linenos">66</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The path to compare files in. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-67"><a href="#get_args-67"><span class="linenos">67</span></a>    <span class="p">)</span>
-</span><span id="get_args-68"><a href="#get_args-68"><span class="linenos">68</span></a>
-</span><span id="get_args-69"><a href="#get_args-69"><span class="linenos">69</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
-</span><span id="get_args-70"><a href="#get_args-70"><span class="linenos">70</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">path</span> <span class="o">==</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">():</span>
-</span><span id="get_args-71"><a href="#get_args-71"><span class="linenos">71</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">path</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">path</span><span class="p">)</span>
-</span><span id="get_args-72"><a href="#get_args-72"><span class="linenos">72</span></a>
-</span><span id="get_args-73"><a href="#get_args-73"><span class="linenos">73</span></a>    <span class="k">return</span> <span class="n">args</span>
+</span><span id="get_args-51"><a href="#get_args-51"><span class="linenos">51</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; After finding duplicates, delete all but one copy.</span>
+</span><span id="get_args-52"><a href="#get_args-52"><span class="linenos">52</span></a><span class="s2">        For each set of duplicates, the tool will ask you to enter the number corresponding to the copy you want to keep.</span>
+</span><span id="get_args-53"><a href="#get_args-53"><span class="linenos">53</span></a><span class="s2">        Pressing &#39;enter&#39; without entering a number will skip that set without deleting anything.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-54"><a href="#get_args-54"><span class="linenos">54</span></a>    <span class="p">)</span>
+</span><span id="get_args-55"><a href="#get_args-55"><span class="linenos">55</span></a>
+</span><span id="get_args-56"><a href="#get_args-56"><span class="linenos">56</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-57"><a href="#get_args-57"><span class="linenos">57</span></a>        <span class="s2">&quot;-ad&quot;</span><span class="p">,</span>
+</span><span id="get_args-58"><a href="#get_args-58"><span class="linenos">58</span></a>        <span class="s2">&quot;--autodelete&quot;</span><span class="p">,</span>
+</span><span id="get_args-59"><a href="#get_args-59"><span class="linenos">59</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="get_args-60"><a href="#get_args-60"><span class="linenos">60</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Automatically decide which file to keep and which to delete from each set of duplicate files instead of asking which to keep. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-61"><a href="#get_args-61"><span class="linenos">61</span></a>    <span class="p">)</span>
+</span><span id="get_args-62"><a href="#get_args-62"><span class="linenos">62</span></a>
+</span><span id="get_args-63"><a href="#get_args-63"><span class="linenos">63</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-64"><a href="#get_args-64"><span class="linenos">64</span></a>        <span class="s2">&quot;-ns&quot;</span><span class="p">,</span>
+</span><span id="get_args-65"><a href="#get_args-65"><span class="linenos">65</span></a>        <span class="s2">&quot;--no_show&quot;</span><span class="p">,</span>
+</span><span id="get_args-66"><a href="#get_args-66"><span class="linenos">66</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="get_args-67"><a href="#get_args-67"><span class="linenos">67</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Don&#39;t show printout of matching files. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-68"><a href="#get_args-68"><span class="linenos">68</span></a>    <span class="p">)</span>
+</span><span id="get_args-69"><a href="#get_args-69"><span class="linenos">69</span></a>
+</span><span id="get_args-70"><a href="#get_args-70"><span class="linenos">70</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-71"><a href="#get_args-71"><span class="linenos">71</span></a>        <span class="s2">&quot;paths&quot;</span><span class="p">,</span>
+</span><span id="get_args-72"><a href="#get_args-72"><span class="linenos">72</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="get_args-73"><a href="#get_args-73"><span class="linenos">73</span></a>        <span class="n">default</span><span class="o">=</span><span class="p">[</span><span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()],</span>
+</span><span id="get_args-74"><a href="#get_args-74"><span class="linenos">74</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;*&quot;</span><span class="p">,</span>
+</span><span id="get_args-75"><a href="#get_args-75"><span class="linenos">75</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The paths to compare files in. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-76"><a href="#get_args-76"><span class="linenos">76</span></a>    <span class="p">)</span>
+</span><span id="get_args-77"><a href="#get_args-77"><span class="linenos">77</span></a>
+</span><span id="get_args-78"><a href="#get_args-78"><span class="linenos">78</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
+</span><span id="get_args-79"><a href="#get_args-79"><span class="linenos">79</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">paths</span> <span class="o">==</span> <span class="p">[</span><span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()]:</span>
+</span><span id="get_args-80"><a href="#get_args-80"><span class="linenos">80</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">paths</span> <span class="o">=</span> <span class="p">[</span><span class="n">Pathier</span><span class="p">(</span><span class="n">path</span><span class="p">)</span> <span class="k">for</span> <span class="n">path</span> <span class="ow">in</span> <span class="n">args</span><span class="o">.</span><span class="n">paths</span><span class="p">]</span>
+</span><span id="get_args-81"><a href="#get_args-81"><span class="linenos">81</span></a>    <span class="n">files</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="get_args-82"><a href="#get_args-82"><span class="linenos">82</span></a>    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Gathering files...&quot;</span><span class="p">)</span>
+</span><span id="get_args-83"><a href="#get_args-83"><span class="linenos">83</span></a>    <span class="k">for</span> <span class="n">path</span> <span class="ow">in</span> <span class="n">args</span><span class="o">.</span><span class="n">paths</span><span class="p">:</span>
+</span><span id="get_args-84"><a href="#get_args-84"><span class="linenos">84</span></a>        <span class="n">files</span><span class="o">.</span><span class="n">extend</span><span class="p">(</span>
+</span><span id="get_args-85"><a href="#get_args-85"><span class="linenos">85</span></a>            <span class="nb">list</span><span class="p">(</span><span class="n">path</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.*&quot;</span><span class="p">))</span> <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">recursive</span> <span class="k">else</span> <span class="nb">list</span><span class="p">(</span><span class="n">path</span><span class="o">.</span><span class="n">glob</span><span class="p">(</span><span class="s2">&quot;*.*&quot;</span><span class="p">))</span>
+</span><span id="get_args-86"><a href="#get_args-86"><span class="linenos">86</span></a>        <span class="p">)</span>
+</span><span id="get_args-87"><a href="#get_args-87"><span class="linenos">87</span></a>    <span class="n">args</span><span class="o">.</span><span class="n">paths</span> <span class="o">=</span> <span class="n">younotyou</span><span class="p">([</span><span class="nb">str</span><span class="p">(</span><span class="n">file</span><span class="p">)</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">files</span><span class="p">],</span> <span class="n">exclude_patterns</span><span class="o">=</span><span class="n">args</span><span class="o">.</span><span class="n">ignores</span><span class="p">)</span>
+</span><span id="get_args-88"><a href="#get_args-88"><span class="linenos">88</span></a>    <span class="n">num_comparisons</span> <span class="o">=</span> <span class="nb">len</span><span class="p">(</span><span class="nb">list</span><span class="p">(</span><span class="n">combinations</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">paths</span><span class="p">,</span> <span class="mi">2</span><span class="p">)))</span>
+</span><span id="get_args-89"><a href="#get_args-89"><span class="linenos">89</span></a>    <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Making </span><span class="si">{</span><span class="n">num_comparisons</span><span class="si">}</span><span class="s2"> comparisons between </span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">paths</span><span class="p">)</span><span class="si">}</span><span class="s2"> files...&quot;</span><span class="p">)</span>
+</span><span id="get_args-90"><a href="#get_args-90"><span class="linenos">90</span></a>
+</span><span id="get_args-91"><a href="#get_args-91"><span class="linenos">91</span></a>    <span class="k">return</span> <span class="n">args</span>
 </span></pre></div>
 
 
     
 
                 </section>
                 <section id="delete_wizard">
@@ -305,29 +337,29 @@
         <span class="def">def</span>
         <span class="name">delete_wizard</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">matches</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">pathier</span><span class="o">.</span><span class="n">pathier</span><span class="o">.</span><span class="n">Pathier</span><span class="p">]]</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="delete_wizard-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#delete_wizard"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="delete_wizard-76"><a href="#delete_wizard-76"><span class="linenos">76</span></a><span class="k">def</span> <span class="nf">delete_wizard</span><span class="p">(</span><span class="n">matches</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">Pathier</span><span class="p">]]):</span>
-</span><span id="delete_wizard-77"><a href="#delete_wizard-77"><span class="linenos">77</span></a>    <span class="sd">&quot;&quot;&quot;Ask which file to keep for each set.&quot;&quot;&quot;</span>
-</span><span id="delete_wizard-78"><a href="#delete_wizard-78"><span class="linenos">78</span></a>    <span class="nb">print</span><span class="p">()</span>
-</span><span id="delete_wizard-79"><a href="#delete_wizard-79"><span class="linenos">79</span></a>    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Enter the corresponding number of the file to keep.&quot;</span><span class="p">)</span>
-</span><span id="delete_wizard-80"><a href="#delete_wizard-80"><span class="linenos">80</span></a>    <span class="nb">print</span><span class="p">(</span>
-</span><span id="delete_wizard-81"><a href="#delete_wizard-81"><span class="linenos">81</span></a>        <span class="s2">&quot;Press &#39;Enter&#39; without giving a number to skip deleting any files for the given set.&quot;</span>
-</span><span id="delete_wizard-82"><a href="#delete_wizard-82"><span class="linenos">82</span></a>    <span class="p">)</span>
-</span><span id="delete_wizard-83"><a href="#delete_wizard-83"><span class="linenos">83</span></a>    <span class="nb">print</span><span class="p">()</span>
-</span><span id="delete_wizard-84"><a href="#delete_wizard-84"><span class="linenos">84</span></a>    <span class="k">for</span> <span class="n">match</span> <span class="ow">in</span> <span class="n">matches</span><span class="p">:</span>
-</span><span id="delete_wizard-85"><a href="#delete_wizard-85"><span class="linenos">85</span></a>        <span class="n">map_</span> <span class="o">=</span> <span class="p">{</span><span class="nb">str</span><span class="p">(</span><span class="n">i</span><span class="p">):</span> <span class="n">file</span> <span class="k">for</span> <span class="n">i</span><span class="p">,</span> <span class="n">file</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">match</span><span class="p">,</span> <span class="mi">1</span><span class="p">)}</span>
-</span><span id="delete_wizard-86"><a href="#delete_wizard-86"><span class="linenos">86</span></a>        <span class="n">options</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;(</span><span class="si">{</span><span class="n">i</span><span class="si">}</span><span class="s2">) </span><span class="si">{</span><span class="n">file</span><span class="si">}</span><span class="s2">&quot;</span> <span class="k">for</span> <span class="n">i</span><span class="p">,</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">map_</span><span class="o">.</span><span class="n">items</span><span class="p">())</span> <span class="o">+</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span>
-</span><span id="delete_wizard-87"><a href="#delete_wizard-87"><span class="linenos">87</span></a>        <span class="nb">print</span><span class="p">(</span><span class="n">options</span><span class="p">)</span>
-</span><span id="delete_wizard-88"><a href="#delete_wizard-88"><span class="linenos">88</span></a>        <span class="n">keeper</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Enter number of file to keep (</span><span class="si">{</span><span class="s1">&#39;, &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">map_</span><span class="o">.</span><span class="n">keys</span><span class="p">())</span><span class="si">}</span><span class="s2">): &quot;</span><span class="p">)</span>
-</span><span id="delete_wizard-89"><a href="#delete_wizard-89"><span class="linenos">89</span></a>        <span class="k">if</span> <span class="n">keeper</span><span class="p">:</span>
-</span><span id="delete_wizard-90"><a href="#delete_wizard-90"><span class="linenos">90</span></a>            <span class="p">[</span><span class="n">map_</span><span class="p">[</span><span class="n">num</span><span class="p">]</span><span class="o">.</span><span class="n">delete</span><span class="p">()</span> <span class="k">for</span> <span class="n">num</span> <span class="ow">in</span> <span class="n">map_</span> <span class="k">if</span> <span class="n">num</span> <span class="o">!=</span> <span class="n">keeper</span><span class="p">]</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="delete_wizard-94"><a href="#delete_wizard-94"><span class="linenos"> 94</span></a><span class="k">def</span> <span class="nf">delete_wizard</span><span class="p">(</span><span class="n">matches</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">Pathier</span><span class="p">]]):</span>
+</span><span id="delete_wizard-95"><a href="#delete_wizard-95"><span class="linenos"> 95</span></a>    <span class="sd">&quot;&quot;&quot;Ask which file to keep for each set.&quot;&quot;&quot;</span>
+</span><span id="delete_wizard-96"><a href="#delete_wizard-96"><span class="linenos"> 96</span></a>    <span class="nb">print</span><span class="p">()</span>
+</span><span id="delete_wizard-97"><a href="#delete_wizard-97"><span class="linenos"> 97</span></a>    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Enter the corresponding number of the file to keep.&quot;</span><span class="p">)</span>
+</span><span id="delete_wizard-98"><a href="#delete_wizard-98"><span class="linenos"> 98</span></a>    <span class="nb">print</span><span class="p">(</span>
+</span><span id="delete_wizard-99"><a href="#delete_wizard-99"><span class="linenos"> 99</span></a>        <span class="s2">&quot;Press &#39;Enter&#39; without giving a number to skip deleting any files for the given set.&quot;</span>
+</span><span id="delete_wizard-100"><a href="#delete_wizard-100"><span class="linenos">100</span></a>    <span class="p">)</span>
+</span><span id="delete_wizard-101"><a href="#delete_wizard-101"><span class="linenos">101</span></a>    <span class="nb">print</span><span class="p">()</span>
+</span><span id="delete_wizard-102"><a href="#delete_wizard-102"><span class="linenos">102</span></a>    <span class="k">for</span> <span class="n">match</span> <span class="ow">in</span> <span class="n">matches</span><span class="p">:</span>
+</span><span id="delete_wizard-103"><a href="#delete_wizard-103"><span class="linenos">103</span></a>        <span class="n">map_</span> <span class="o">=</span> <span class="p">{</span><span class="nb">str</span><span class="p">(</span><span class="n">i</span><span class="p">):</span> <span class="n">file</span> <span class="k">for</span> <span class="n">i</span><span class="p">,</span> <span class="n">file</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">match</span><span class="p">,</span> <span class="mi">1</span><span class="p">)}</span>
+</span><span id="delete_wizard-104"><a href="#delete_wizard-104"><span class="linenos">104</span></a>        <span class="n">options</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;(</span><span class="si">{</span><span class="n">i</span><span class="si">}</span><span class="s2">) </span><span class="si">{</span><span class="n">file</span><span class="si">}</span><span class="s2">&quot;</span> <span class="k">for</span> <span class="n">i</span><span class="p">,</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">map_</span><span class="o">.</span><span class="n">items</span><span class="p">())</span> <span class="o">+</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span>
+</span><span id="delete_wizard-105"><a href="#delete_wizard-105"><span class="linenos">105</span></a>        <span class="nb">print</span><span class="p">(</span><span class="n">options</span><span class="p">)</span>
+</span><span id="delete_wizard-106"><a href="#delete_wizard-106"><span class="linenos">106</span></a>        <span class="n">keeper</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Enter number of file to keep (</span><span class="si">{</span><span class="s1">&#39;, &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">map_</span><span class="o">.</span><span class="n">keys</span><span class="p">())</span><span class="si">}</span><span class="s2">): &quot;</span><span class="p">)</span>
+</span><span id="delete_wizard-107"><a href="#delete_wizard-107"><span class="linenos">107</span></a>        <span class="k">if</span> <span class="n">keeper</span><span class="p">:</span>
+</span><span id="delete_wizard-108"><a href="#delete_wizard-108"><span class="linenos">108</span></a>            <span class="p">[</span><span class="n">map_</span><span class="p">[</span><span class="n">num</span><span class="p">]</span><span class="o">.</span><span class="n">delete</span><span class="p">()</span> <span class="k">for</span> <span class="n">num</span> <span class="ow">in</span> <span class="n">map_</span> <span class="k">if</span> <span class="n">num</span> <span class="o">!=</span> <span class="n">keeper</span><span class="p">]</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Ask which file to keep for each set.</p>
 </div>
 
 
@@ -339,19 +371,19 @@
         <span class="def">def</span>
         <span class="name">autodelete</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">matches</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">pathier</span><span class="o">.</span><span class="n">pathier</span><span class="o">.</span><span class="n">Pathier</span><span class="p">]]</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="autodelete-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#autodelete"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="autodelete-93"><a href="#autodelete-93"><span class="linenos">93</span></a><span class="k">def</span> <span class="nf">autodelete</span><span class="p">(</span><span class="n">matches</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">Pathier</span><span class="p">]]):</span>
-</span><span id="autodelete-94"><a href="#autodelete-94"><span class="linenos">94</span></a>    <span class="sd">&quot;&quot;&quot;Keep one of each set in `matches` and delete the others.&quot;&quot;&quot;</span>
-</span><span id="autodelete-95"><a href="#autodelete-95"><span class="linenos">95</span></a>    <span class="k">for</span> <span class="n">match</span> <span class="ow">in</span> <span class="n">matches</span><span class="p">:</span>
-</span><span id="autodelete-96"><a href="#autodelete-96"><span class="linenos">96</span></a>        <span class="k">match</span><span class="o">.</span><span class="n">pop</span><span class="p">()</span>
-</span><span id="autodelete-97"><a href="#autodelete-97"><span class="linenos">97</span></a>        <span class="p">[</span><span class="n">file</span><span class="o">.</span><span class="n">delete</span><span class="p">()</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">match</span><span class="p">]</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="autodelete-111"><a href="#autodelete-111"><span class="linenos">111</span></a><span class="k">def</span> <span class="nf">autodelete</span><span class="p">(</span><span class="n">matches</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">Pathier</span><span class="p">]]):</span>
+</span><span id="autodelete-112"><a href="#autodelete-112"><span class="linenos">112</span></a>    <span class="sd">&quot;&quot;&quot;Keep one of each set in `matches` and delete the others.&quot;&quot;&quot;</span>
+</span><span id="autodelete-113"><a href="#autodelete-113"><span class="linenos">113</span></a>    <span class="k">for</span> <span class="n">match</span> <span class="ow">in</span> <span class="n">matches</span><span class="p">:</span>
+</span><span id="autodelete-114"><a href="#autodelete-114"><span class="linenos">114</span></a>        <span class="k">match</span><span class="o">.</span><span class="n">pop</span><span class="p">()</span>
+</span><span id="autodelete-115"><a href="#autodelete-115"><span class="linenos">115</span></a>        <span class="p">[</span><span class="n">file</span><span class="o">.</span><span class="n">delete</span><span class="p">()</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">match</span><span class="p">]</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Keep one of each set in <code>matches</code> and delete the others.</p>
 </div>
 
 
@@ -363,42 +395,42 @@
         <span class="def">def</span>
         <span class="name">dupechecker</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="dupechecker-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#dupechecker"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="dupechecker-100"><a href="#dupechecker-100"><span class="linenos">100</span></a><span class="k">def</span> <span class="nf">dupechecker</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
-</span><span id="dupechecker-101"><a href="#dupechecker-101"><span class="linenos">101</span></a>    <span class="nb">print</span><span class="p">()</span>
-</span><span id="dupechecker-102"><a href="#dupechecker-102"><span class="linenos">102</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
-</span><span id="dupechecker-103"><a href="#dupechecker-103"><span class="linenos">103</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
-</span><span id="dupechecker-104"><a href="#dupechecker-104"><span class="linenos">104</span></a>    <span class="n">s</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="dupechecker-105"><a href="#dupechecker-105"><span class="linenos">105</span></a>        <span class="n">ch</span><span class="o">.</span><span class="n">rjust</span><span class="p">(</span><span class="n">i</span> <span class="o">+</span> <span class="n">j</span><span class="p">)</span>
-</span><span id="dupechecker-106"><a href="#dupechecker-106"><span class="linenos">106</span></a>        <span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="mi">1</span><span class="p">,</span> <span class="mi">25</span><span class="p">,</span> <span class="mi">3</span><span class="p">)</span>
-</span><span id="dupechecker-107"><a href="#dupechecker-107"><span class="linenos">107</span></a>        <span class="k">for</span> <span class="n">j</span><span class="p">,</span> <span class="n">ch</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">([</span><span class="s2">&quot;/&quot;</span><span class="p">,</span> <span class="s2">&quot;-&quot;</span><span class="p">,</span> <span class="s2">&quot;</span><span class="se">\\</span><span class="s2">&quot;</span><span class="p">])</span>
-</span><span id="dupechecker-108"><a href="#dupechecker-108"><span class="linenos">108</span></a>    <span class="p">]</span>
-</span><span id="dupechecker-109"><a href="#dupechecker-109"><span class="linenos">109</span></a>    <span class="n">s</span> <span class="o">+=</span> <span class="n">s</span><span class="p">[::</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span>
-</span><span id="dupechecker-110"><a href="#dupechecker-110"><span class="linenos">110</span></a>    <span class="k">with</span> <span class="n">Spinner</span><span class="p">(</span><span class="n">s</span><span class="p">)</span> <span class="k">as</span> <span class="n">spinner</span><span class="p">:</span>
-</span><span id="dupechecker-111"><a href="#dupechecker-111"><span class="linenos">111</span></a>        <span class="k">with</span> <span class="n">ThreadPoolExecutor</span><span class="p">()</span> <span class="k">as</span> <span class="n">exc</span><span class="p">:</span>
-</span><span id="dupechecker-112"><a href="#dupechecker-112"><span class="linenos">112</span></a>            <span class="n">thread</span> <span class="o">=</span> <span class="n">exc</span><span class="o">.</span><span class="n">submit</span><span class="p">(</span><span class="n">get_duplicates</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">path</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">recursive</span><span class="p">)</span>
-</span><span id="dupechecker-113"><a href="#dupechecker-113"><span class="linenos">113</span></a>            <span class="k">while</span> <span class="ow">not</span> <span class="n">thread</span><span class="o">.</span><span class="n">done</span><span class="p">():</span>
-</span><span id="dupechecker-114"><a href="#dupechecker-114"><span class="linenos">114</span></a>                <span class="n">spinner</span><span class="o">.</span><span class="n">display</span><span class="p">()</span>
-</span><span id="dupechecker-115"><a href="#dupechecker-115"><span class="linenos">115</span></a>                <span class="n">time</span><span class="o">.</span><span class="n">sleep</span><span class="p">(</span><span class="mf">0.025</span><span class="p">)</span>
-</span><span id="dupechecker-116"><a href="#dupechecker-116"><span class="linenos">116</span></a>            <span class="n">matches</span> <span class="o">=</span> <span class="n">thread</span><span class="o">.</span><span class="n">result</span><span class="p">()</span>
-</span><span id="dupechecker-117"><a href="#dupechecker-117"><span class="linenos">117</span></a>    <span class="k">if</span> <span class="n">matches</span><span class="p">:</span>
-</span><span id="dupechecker-118"><a href="#dupechecker-118"><span class="linenos">118</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Found </span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="n">matches</span><span class="p">)</span><span class="si">}</span><span class="s2"> duplicate sets of files.&quot;</span><span class="p">)</span>
-</span><span id="dupechecker-119"><a href="#dupechecker-119"><span class="linenos">119</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">no_show</span><span class="p">:</span>
-</span><span id="dupechecker-120"><a href="#dupechecker-120"><span class="linenos">120</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">griddy</span><span class="p">(</span><span class="n">matches</span><span class="p">))</span>
-</span><span id="dupechecker-121"><a href="#dupechecker-121"><span class="linenos">121</span></a>        <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">delete_dupes</span> <span class="ow">or</span> <span class="n">args</span><span class="o">.</span><span class="n">autodelete</span><span class="p">:</span>
-</span><span id="dupechecker-122"><a href="#dupechecker-122"><span class="linenos">122</span></a>            <span class="n">size</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">size</span><span class="p">()</span>
-</span><span id="dupechecker-123"><a href="#dupechecker-123"><span class="linenos">123</span></a>            <span class="n">delete_wizard</span><span class="p">(</span><span class="n">matches</span><span class="p">)</span> <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">delete_dupes</span> <span class="k">else</span> <span class="n">autodelete</span><span class="p">(</span><span class="n">matches</span><span class="p">)</span>
-</span><span id="dupechecker-124"><a href="#dupechecker-124"><span class="linenos">124</span></a>            <span class="n">deleted_size</span> <span class="o">=</span> <span class="n">size</span> <span class="o">-</span> <span class="n">args</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">size</span><span class="p">()</span>
-</span><span id="dupechecker-125"><a href="#dupechecker-125"><span class="linenos">125</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Deleted </span><span class="si">{</span><span class="n">Pathier</span><span class="o">.</span><span class="n">format_size</span><span class="p">(</span><span class="n">deleted_size</span><span class="p">)</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
-</span><span id="dupechecker-126"><a href="#dupechecker-126"><span class="linenos">126</span></a>    <span class="k">else</span><span class="p">:</span>
-</span><span id="dupechecker-127"><a href="#dupechecker-127"><span class="linenos">127</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;No duplicates detected.&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="dupechecker-118"><a href="#dupechecker-118"><span class="linenos">118</span></a><span class="k">def</span> <span class="nf">dupechecker</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
+</span><span id="dupechecker-119"><a href="#dupechecker-119"><span class="linenos">119</span></a>    <span class="nb">print</span><span class="p">()</span>
+</span><span id="dupechecker-120"><a href="#dupechecker-120"><span class="linenos">120</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
+</span><span id="dupechecker-121"><a href="#dupechecker-121"><span class="linenos">121</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
+</span><span id="dupechecker-122"><a href="#dupechecker-122"><span class="linenos">122</span></a>    <span class="n">s</span> <span class="o">=</span> <span class="p">[</span>
+</span><span id="dupechecker-123"><a href="#dupechecker-123"><span class="linenos">123</span></a>        <span class="n">ch</span><span class="o">.</span><span class="n">rjust</span><span class="p">(</span><span class="n">i</span> <span class="o">+</span> <span class="n">j</span><span class="p">)</span>
+</span><span id="dupechecker-124"><a href="#dupechecker-124"><span class="linenos">124</span></a>        <span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="mi">1</span><span class="p">,</span> <span class="mi">25</span><span class="p">,</span> <span class="mi">3</span><span class="p">)</span>
+</span><span id="dupechecker-125"><a href="#dupechecker-125"><span class="linenos">125</span></a>        <span class="k">for</span> <span class="n">j</span><span class="p">,</span> <span class="n">ch</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">([</span><span class="s2">&quot;/&quot;</span><span class="p">,</span> <span class="s2">&quot;-&quot;</span><span class="p">,</span> <span class="s2">&quot;</span><span class="se">\\</span><span class="s2">&quot;</span><span class="p">])</span>
+</span><span id="dupechecker-126"><a href="#dupechecker-126"><span class="linenos">126</span></a>    <span class="p">]</span>
+</span><span id="dupechecker-127"><a href="#dupechecker-127"><span class="linenos">127</span></a>    <span class="n">s</span> <span class="o">+=</span> <span class="n">s</span><span class="p">[::</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span>
+</span><span id="dupechecker-128"><a href="#dupechecker-128"><span class="linenos">128</span></a>    <span class="k">with</span> <span class="n">Spinner</span><span class="p">(</span><span class="n">s</span><span class="p">)</span> <span class="k">as</span> <span class="n">spinner</span><span class="p">:</span>
+</span><span id="dupechecker-129"><a href="#dupechecker-129"><span class="linenos">129</span></a>        <span class="k">with</span> <span class="n">ThreadPoolExecutor</span><span class="p">()</span> <span class="k">as</span> <span class="n">exc</span><span class="p">:</span>
+</span><span id="dupechecker-130"><a href="#dupechecker-130"><span class="linenos">130</span></a>            <span class="n">thread</span> <span class="o">=</span> <span class="n">exc</span><span class="o">.</span><span class="n">submit</span><span class="p">(</span><span class="n">get_duplicates</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">paths</span><span class="p">)</span>
+</span><span id="dupechecker-131"><a href="#dupechecker-131"><span class="linenos">131</span></a>            <span class="k">while</span> <span class="ow">not</span> <span class="n">thread</span><span class="o">.</span><span class="n">done</span><span class="p">():</span>
+</span><span id="dupechecker-132"><a href="#dupechecker-132"><span class="linenos">132</span></a>                <span class="n">spinner</span><span class="o">.</span><span class="n">display</span><span class="p">()</span>
+</span><span id="dupechecker-133"><a href="#dupechecker-133"><span class="linenos">133</span></a>                <span class="n">time</span><span class="o">.</span><span class="n">sleep</span><span class="p">(</span><span class="mf">0.025</span><span class="p">)</span>
+</span><span id="dupechecker-134"><a href="#dupechecker-134"><span class="linenos">134</span></a>            <span class="n">matches</span> <span class="o">=</span> <span class="n">thread</span><span class="o">.</span><span class="n">result</span><span class="p">()</span>
+</span><span id="dupechecker-135"><a href="#dupechecker-135"><span class="linenos">135</span></a>    <span class="k">if</span> <span class="n">matches</span><span class="p">:</span>
+</span><span id="dupechecker-136"><a href="#dupechecker-136"><span class="linenos">136</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Found </span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="n">matches</span><span class="p">)</span><span class="si">}</span><span class="s2"> duplicate sets of files.&quot;</span><span class="p">)</span>
+</span><span id="dupechecker-137"><a href="#dupechecker-137"><span class="linenos">137</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">no_show</span><span class="p">:</span>
+</span><span id="dupechecker-138"><a href="#dupechecker-138"><span class="linenos">138</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">griddy</span><span class="p">(</span><span class="n">matches</span><span class="p">))</span>
+</span><span id="dupechecker-139"><a href="#dupechecker-139"><span class="linenos">139</span></a>        <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">delete_dupes</span> <span class="ow">or</span> <span class="n">args</span><span class="o">.</span><span class="n">autodelete</span><span class="p">:</span>
+</span><span id="dupechecker-140"><a href="#dupechecker-140"><span class="linenos">140</span></a>            <span class="n">size</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">size</span><span class="p">()</span>
+</span><span id="dupechecker-141"><a href="#dupechecker-141"><span class="linenos">141</span></a>            <span class="n">delete_wizard</span><span class="p">(</span><span class="n">matches</span><span class="p">)</span> <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">delete_dupes</span> <span class="k">else</span> <span class="n">autodelete</span><span class="p">(</span><span class="n">matches</span><span class="p">)</span>
+</span><span id="dupechecker-142"><a href="#dupechecker-142"><span class="linenos">142</span></a>            <span class="n">deleted_size</span> <span class="o">=</span> <span class="n">size</span> <span class="o">-</span> <span class="n">args</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">size</span><span class="p">()</span>
+</span><span id="dupechecker-143"><a href="#dupechecker-143"><span class="linenos">143</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Deleted </span><span class="si">{</span><span class="n">Pathier</span><span class="o">.</span><span class="n">format_size</span><span class="p">(</span><span class="n">deleted_size</span><span class="p">)</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+</span><span id="dupechecker-144"><a href="#dupechecker-144"><span class="linenos">144</span></a>    <span class="k">else</span><span class="p">:</span>
+</span><span id="dupechecker-145"><a href="#dupechecker-145"><span class="linenos">145</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;No duplicates detected.&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                 </section>
     </main>
```

#### html2text {}

```diff
@@ -12,281 +12,315 @@
 
 ****** dupechecker.dupechecker ******
 ⁰ View Source
 __1import argparse
 __2import filecmp
 __3import time
 __4from concurrent.futures import ThreadPoolExecutor
-__5
-__6from griddle import griddy
-__7from pathier import Pathier
-__8from printbuddies import Spinner
-__9
-_10
-_11def get_duplicates(path: Pathier, recursive: bool = False) -> list[list
-[Pathier]]:
-_12    """Return a list of lists for duplicate files in `path`.
-_13    Each sub-list will contain 2 or more files determined to be equivalent
-files.
-_14    If `recursive` is `True`, files from `path` and it's subdirectories will
-be compared."""
-_15    files = list(path.rglob("*.*")) if recursive else list(path.glob("*.*"))
-_16    matching_sets = []
-_17    while len(files) > 0:
-_18        comparee = files.pop()
-_19        matching_files = [file for file in files if filecmp.cmp(comparee,
+__5from itertools import combinations
+__6
+__7from griddle import griddy
+__8from pathier import Pathier
+__9from printbuddies import Spinner
+_10from younotyou import younotyou
+_11
+_12
+_13def get_duplicates(paths: list[Pathier]) -> list[list[Pathier]]:
+_14    """Return a list of lists for duplicate files in `paths`."""
+_15    matching_sets = []
+_16    while len(paths) > 0:
+_17        comparee = paths.pop()
+_18        matching_files = [file for file in paths if filecmp.cmp(comparee,
 file, False)]
-_20        if matching_files:
-_21            [files.pop(files.index(file)) for file in matching_files]
-_22            matching_files.insert(0, comparee)
-_23            matching_sets.append(matching_files)
-_24    return matching_sets
+_19        if matching_files:
+_20            [paths.pop(paths.index(file)) for file in matching_files]
+_21            matching_files.insert(0, comparee)
+_22            matching_sets.append(matching_files)
+_23    return matching_sets
+_24
 _25
-_26
-_27def get_args() -> argparse.Namespace:
-_28    parser = argparse.ArgumentParser()
-_29
-_30    parser.add_argument(
-_31        "-r",
-_32        "--recursive",
-_33        action="store_true",
-_34        help=""" Glob files to compare recursively. """,
-_35    )
-_36
-_37    parser.add_argument(
-_38        "-d",
-_39        "--delete_dupes",
-_40        action="store_true",
-_41        help=""" After finding duplicates, delete all but one copy.
-_42        For each set of duplicates, the tool will ask you to enter the
-number corresponding to the copy you want to keep.
-_43        Pressing 'enter' without entering a number will skip that set
-without deleting anything.""",
+_26def get_args() -> argparse.Namespace:
+_27    parser = argparse.ArgumentParser()
+_28
+_29    parser.add_argument(
+_30        "-r",
+_31        "--recursive",
+_32        action="store_true",
+_33        help=""" Glob files to compare recursively. """,
+_34    )
+_35
+_36    parser.add_argument(
+_37        "-i",
+_38        "--ignores",
+_39        type=str,
+_40        nargs="*",
+_41        default=[],
+_42        help=""" Ignore files matching these patterns.
+_43        e.g. `dupechecker -i *.wav` will compare all files in the current
+working directory except .wav files.""",
 _44    )
 _45
 _46    parser.add_argument(
-_47        "-ad",
-_48        "--autodelete",
+_47        "-d",
+_48        "--delete_dupes",
 _49        action="store_true",
-_50        help=""" Automatically decide which file to keep and which to delete
+_50        help=""" After finding duplicates, delete all but one copy.
+_51        For each set of duplicates, the tool will ask you to enter the
+number corresponding to the copy you want to keep.
+_52        Pressing 'enter' without entering a number will skip that set
+without deleting anything.""",
+_53    )
+_54
+_55    parser.add_argument(
+_56        "-ad",
+_57        "--autodelete",
+_58        action="store_true",
+_59        help=""" Automatically decide which file to keep and which to delete
 from each set of duplicate files instead of asking which to keep. """,
-_51    )
-_52
-_53    parser.add_argument(
-_54        "-ns",
-_55        "--no_show",
-_56        action="store_true",
-_57        help=""" Don't show printout of matching files. """,
-_58    )
-_59
-_60    parser.add_argument(
-_61        "path",
-_62        type=str,
-_63        default=Pathier.cwd(),
-_64        nargs="?",
-_65        help=""" The path to compare files in. """,
-_66    )
-_67
-_68    args = parser.parse_args()
-_69    if not args.path == Pathier.cwd():
-_70        args.path = Pathier(args.path)
-_71
-_72    return args
-_73
-_74
-_75def delete_wizard(matches: list[list[Pathier]]):
-_76    """Ask which file to keep for each set."""
-_77    print()
-_78    print("Enter the corresponding number of the file to keep.")
-_79    print(
-_80        "Press 'Enter' without giving a number to skip deleting any files
+_60    )
+_61
+_62    parser.add_argument(
+_63        "-ns",
+_64        "--no_show",
+_65        action="store_true",
+_66        help=""" Don't show printout of matching files. """,
+_67    )
+_68
+_69    parser.add_argument(
+_70        "paths",
+_71        type=str,
+_72        default=[Pathier.cwd()],
+_73        nargs="*",
+_74        help=""" The paths to compare files in. """,
+_75    )
+_76
+_77    args = parser.parse_args()
+_78    if not args.paths == [Pathier.cwd()]:
+_79        args.paths = [Pathier(path) for path in args.paths]
+_80    files = []
+_81    print("Gathering files...")
+_82    for path in args.paths:
+_83        files.extend(
+_84            list(path.rglob("*.*")) if args.recursive else list(path.glob
+("*.*"))
+_85        )
+_86    args.paths = younotyou([str(file) for file in files],
+exclude_patterns=args.ignores)
+_87    num_comparisons = len(list(combinations(args.paths, 2)))
+_88    print(f"Making {num_comparisons} comparisons between {len(args.paths)}
+files...")
+_89
+_90    return args
+_91
+_92
+_93def delete_wizard(matches: list[list[Pathier]]):
+_94    """Ask which file to keep for each set."""
+_95    print()
+_96    print("Enter the corresponding number of the file to keep.")
+_97    print(
+_98        "Press 'Enter' without giving a number to skip deleting any files
 for the given set."
-_81    )
-_82    print()
-_83    for match in matches:
-_84        map_ = {str(i): file for i, file in enumerate(match, 1)}
-_85        options = "\n".join(f"({i}) {file}" for i, file in map_.items()) +
+_99    )
+100    print()
+101    for match in matches:
+102        map_ = {str(i): file for i, file in enumerate(match, 1)}
+103        options = "\n".join(f"({i}) {file}" for i, file in map_.items()) +
 "\n"
-_86        print(options)
-_87        keeper = input(f"Enter number of file to keep ({', '.join(map_.keys
+104        print(options)
+105        keeper = input(f"Enter number of file to keep ({', '.join(map_.keys
 ())}): ")
-_88        if keeper:
-_89            [map_[num].delete() for num in map_ if num != keeper]
-_90
-_91
-_92def autodelete(matches: list[list[Pathier]]):
-_93    """Keep one of each set in `matches` and delete the others."""
-_94    for match in matches:
-_95        match.pop()
-_96        [file.delete() for file in match]
-_97
-_98
-_99def dupechecker(args: argparse.Namespace | None = None):
-100    print()
-101    if not args:
-102        args = get_args()
-103    s = [
-104        ch.rjust(i + j)
-105        for i in range(1, 25, 3)
-106        for j, ch in enumerate(["/", "-", "\\"])
-107    ]
-108    s += s[::-1]
-109    with Spinner(s) as spinner:
-110        with ThreadPoolExecutor() as exc:
-111            thread = exc.submit(get_duplicates, args.path, args.recursive)
-112            while not thread.done():
-113                spinner.display()
-114                time.sleep(0.025)
-115            matches = thread.result()
-116    if matches:
-117        print(f"Found {len(matches)} duplicate sets of files.")
-118        if not args.no_show:
-119            print(griddy(matches))
-120        if args.delete_dupes or args.autodelete:
-121            size = args.path.size()
-122            delete_wizard(matches) if args.delete_dupes else autodelete
+106        if keeper:
+107            [map_[num].delete() for num in map_ if num != keeper]
+108
+109
+110def autodelete(matches: list[list[Pathier]]):
+111    """Keep one of each set in `matches` and delete the others."""
+112    for match in matches:
+113        match.pop()
+114        [file.delete() for file in match]
+115
+116
+117def dupechecker(args: argparse.Namespace | None = None):
+118    print()
+119    if not args:
+120        args = get_args()
+121    s = [
+122        ch.rjust(i + j)
+123        for i in range(1, 25, 3)
+124        for j, ch in enumerate(["/", "-", "\\"])
+125    ]
+126    s += s[::-1]
+127    with Spinner(s) as spinner:
+128        with ThreadPoolExecutor() as exc:
+129            thread = exc.submit(get_duplicates, args.paths)
+130            while not thread.done():
+131                spinner.display()
+132                time.sleep(0.025)
+133            matches = thread.result()
+134    if matches:
+135        print(f"Found {len(matches)} duplicate sets of files.")
+136        if not args.no_show:
+137            print(griddy(matches))
+138        if args.delete_dupes or args.autodelete:
+139            size = args.path.size()
+140            delete_wizard(matches) if args.delete_dupes else autodelete
 (matches)
-123            deleted_size = size - args.path.size()
-124            print(f"Deleted {Pathier.format_size(deleted_size)}.")
-125    else:
-126        print("No duplicates detected.")
-127
-128
-129if __name__ == "__main__":
-130    dupechecker(get_args())
+141            deleted_size = size - args.path.size()
+142            print(f"Deleted {Pathier.format_size(deleted_size)}.")
+143    else:
+144        print("No duplicates detected.")
+145
+146
+147if __name__ == "__main__":
+148    dupechecker(get_args())
   ⁰
 def get_duplicates(
-path: pathier.pathier.Pathier,
-recursive: bool = False) -> list[list[pathier.pathier.Pathier]]: View Source
-12def get_duplicates(path: Pathier, recursive: bool = False) -> list[list
-[Pathier]]:
-13    """Return a list of lists for duplicate files in `path`.
-14    Each sub-list will contain 2 or more files determined to be equivalent
-files.
-15    If `recursive` is `True`, files from `path` and it's subdirectories will
-be compared."""
-16    files = list(path.rglob("*.*")) if recursive else list(path.glob("*.*"))
-17    matching_sets = []
-18    while len(files) > 0:
-19        comparee = files.pop()
-20        matching_files = [file for file in files if filecmp.cmp(comparee,
+paths: list[pathier.pathier.Pathier]) -> list[list[pathier.pathier.Pathier]]:
+View Source
+14def get_duplicates(paths: list[Pathier]) -> list[list[Pathier]]:
+15    """Return a list of lists for duplicate files in `paths`."""
+16    matching_sets = []
+17    while len(paths) > 0:
+18        comparee = paths.pop()
+19        matching_files = [file for file in paths if filecmp.cmp(comparee,
 file, False)]
-21        if matching_files:
-22            [files.pop(files.index(file)) for file in matching_files]
-23            matching_files.insert(0, comparee)
-24            matching_sets.append(matching_files)
-25    return matching_sets
-Return a list of lists for duplicate files in path. Each sub-list will contain
-2 or more files determined to be equivalent files. If recursive is True, files
-from path and it's subdirectories will be compared.
+20        if matching_files:
+21            [paths.pop(paths.index(file)) for file in matching_files]
+22            matching_files.insert(0, comparee)
+23            matching_sets.append(matching_files)
+24    return matching_sets
+Return a list of lists for duplicate files in paths.
   ⁰
 def get_args() -> argparse.Namespace: View Source
-28def get_args() -> argparse.Namespace:
-29    parser = argparse.ArgumentParser()
-30
-31    parser.add_argument(
-32        "-r",
-33        "--recursive",
-34        action="store_true",
-35        help=""" Glob files to compare recursively. """,
-36    )
-37
-38    parser.add_argument(
-39        "-d",
-40        "--delete_dupes",
-41        action="store_true",
-42        help=""" After finding duplicates, delete all but one copy.
-43        For each set of duplicates, the tool will ask you to enter the number
-corresponding to the copy you want to keep.
-44        Pressing 'enter' without entering a number will skip that set without
-deleting anything.""",
+27def get_args() -> argparse.Namespace:
+28    parser = argparse.ArgumentParser()
+29
+30    parser.add_argument(
+31        "-r",
+32        "--recursive",
+33        action="store_true",
+34        help=""" Glob files to compare recursively. """,
+35    )
+36
+37    parser.add_argument(
+38        "-i",
+39        "--ignores",
+40        type=str,
+41        nargs="*",
+42        default=[],
+43        help=""" Ignore files matching these patterns.
+44        e.g. `dupechecker -i *.wav` will compare all files in the current
+working directory except .wav files.""",
 45    )
 46
 47    parser.add_argument(
-48        "-ad",
-49        "--autodelete",
+48        "-d",
+49        "--delete_dupes",
 50        action="store_true",
-51        help=""" Automatically decide which file to keep and which to delete
+51        help=""" After finding duplicates, delete all but one copy.
+52        For each set of duplicates, the tool will ask you to enter the number
+corresponding to the copy you want to keep.
+53        Pressing 'enter' without entering a number will skip that set without
+deleting anything.""",
+54    )
+55
+56    parser.add_argument(
+57        "-ad",
+58        "--autodelete",
+59        action="store_true",
+60        help=""" Automatically decide which file to keep and which to delete
 from each set of duplicate files instead of asking which to keep. """,
-52    )
-53
-54    parser.add_argument(
-55        "-ns",
-56        "--no_show",
-57        action="store_true",
-58        help=""" Don't show printout of matching files. """,
-59    )
-60
-61    parser.add_argument(
-62        "path",
-63        type=str,
-64        default=Pathier.cwd(),
-65        nargs="?",
-66        help=""" The path to compare files in. """,
-67    )
-68
-69    args = parser.parse_args()
-70    if not args.path == Pathier.cwd():
-71        args.path = Pathier(args.path)
-72
-73    return args
+61    )
+62
+63    parser.add_argument(
+64        "-ns",
+65        "--no_show",
+66        action="store_true",
+67        help=""" Don't show printout of matching files. """,
+68    )
+69
+70    parser.add_argument(
+71        "paths",
+72        type=str,
+73        default=[Pathier.cwd()],
+74        nargs="*",
+75        help=""" The paths to compare files in. """,
+76    )
+77
+78    args = parser.parse_args()
+79    if not args.paths == [Pathier.cwd()]:
+80        args.paths = [Pathier(path) for path in args.paths]
+81    files = []
+82    print("Gathering files...")
+83    for path in args.paths:
+84        files.extend(
+85            list(path.rglob("*.*")) if args.recursive else list(path.glob
+("*.*"))
+86        )
+87    args.paths = younotyou([str(file) for file in files],
+exclude_patterns=args.ignores)
+88    num_comparisons = len(list(combinations(args.paths, 2)))
+89    print(f"Making {num_comparisons} comparisons between {len(args.paths)}
+files...")
+90
+91    return args
   ⁰
 def delete_wizard(matches: list[list[pathier.pathier.Pathier]]): View Source
-76def delete_wizard(matches: list[list[Pathier]]):
-77    """Ask which file to keep for each set."""
-78    print()
-79    print("Enter the corresponding number of the file to keep.")
-80    print(
-81        "Press 'Enter' without giving a number to skip deleting any files for
-the given set."
-82    )
-83    print()
-84    for match in matches:
-85        map_ = {str(i): file for i, file in enumerate(match, 1)}
-86        options = "\n".join(f"({i}) {file}" for i, file in map_.items()) +
+_94def delete_wizard(matches: list[list[Pathier]]):
+_95    """Ask which file to keep for each set."""
+_96    print()
+_97    print("Enter the corresponding number of the file to keep.")
+_98    print(
+_99        "Press 'Enter' without giving a number to skip deleting any files
+for the given set."
+100    )
+101    print()
+102    for match in matches:
+103        map_ = {str(i): file for i, file in enumerate(match, 1)}
+104        options = "\n".join(f"({i}) {file}" for i, file in map_.items()) +
 "\n"
-87        print(options)
-88        keeper = input(f"Enter number of file to keep ({', '.join(map_.keys
+105        print(options)
+106        keeper = input(f"Enter number of file to keep ({', '.join(map_.keys
 ())}): ")
-89        if keeper:
-90            [map_[num].delete() for num in map_ if num != keeper]
+107        if keeper:
+108            [map_[num].delete() for num in map_ if num != keeper]
 Ask which file to keep for each set.
   ⁰
 def autodelete(matches: list[list[pathier.pathier.Pathier]]): View Source
-93def autodelete(matches: list[list[Pathier]]):
-94    """Keep one of each set in `matches` and delete the others."""
-95    for match in matches:
-96        match.pop()
-97        [file.delete() for file in match]
+111def autodelete(matches: list[list[Pathier]]):
+112    """Keep one of each set in `matches` and delete the others."""
+113    for match in matches:
+114        match.pop()
+115        [file.delete() for file in match]
 Keep one of each set in matches and delete the others.
   ⁰
 def dupechecker(args: argparse.Namespace | None = None): View Source
-100def dupechecker(args: argparse.Namespace | None = None):
-101    print()
-102    if not args:
-103        args = get_args()
-104    s = [
-105        ch.rjust(i + j)
-106        for i in range(1, 25, 3)
-107        for j, ch in enumerate(["/", "-", "\\"])
-108    ]
-109    s += s[::-1]
-110    with Spinner(s) as spinner:
-111        with ThreadPoolExecutor() as exc:
-112            thread = exc.submit(get_duplicates, args.path, args.recursive)
-113            while not thread.done():
-114                spinner.display()
-115                time.sleep(0.025)
-116            matches = thread.result()
-117    if matches:
-118        print(f"Found {len(matches)} duplicate sets of files.")
-119        if not args.no_show:
-120            print(griddy(matches))
-121        if args.delete_dupes or args.autodelete:
-122            size = args.path.size()
-123            delete_wizard(matches) if args.delete_dupes else autodelete
+118def dupechecker(args: argparse.Namespace | None = None):
+119    print()
+120    if not args:
+121        args = get_args()
+122    s = [
+123        ch.rjust(i + j)
+124        for i in range(1, 25, 3)
+125        for j, ch in enumerate(["/", "-", "\\"])
+126    ]
+127    s += s[::-1]
+128    with Spinner(s) as spinner:
+129        with ThreadPoolExecutor() as exc:
+130            thread = exc.submit(get_duplicates, args.paths)
+131            while not thread.done():
+132                spinner.display()
+133                time.sleep(0.025)
+134            matches = thread.result()
+135    if matches:
+136        print(f"Found {len(matches)} duplicate sets of files.")
+137        if not args.no_show:
+138            print(griddy(matches))
+139        if args.delete_dupes or args.autodelete:
+140            size = args.path.size()
+141            delete_wizard(matches) if args.delete_dupes else autodelete
 (matches)
-124            deleted_size = size - args.path.size()
-125            print(f"Deleted {Pathier.format_size(deleted_size)}.")
-126    else:
-127        print("No duplicates detected.")
+142            deleted_size = size - args.path.size()
+143            print(f"Deleted {Pathier.format_size(deleted_size)}.")
+144    else:
+145        print("No duplicates detected.")
```

### Comparing `dupechecker-0.1.0/src/dupechecker/dupechecker.py` & `dupechecker-0.2.0/src/dupechecker/dupechecker.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 import argparse
 import filecmp
 import time
 from concurrent.futures import ThreadPoolExecutor
+from itertools import combinations
 
 from griddle import griddy
 from pathier import Pathier
 from printbuddies import Spinner
+from younotyou import younotyou
 
 
-def get_duplicates(path: Pathier, recursive: bool = False) -> list[list[Pathier]]:
-    """Return a list of lists for duplicate files in `path`.
-    Each sub-list will contain 2 or more files determined to be equivalent files.
-    If `recursive` is `True`, files from `path` and it's subdirectories will be compared."""
-    files = list(path.rglob("*.*")) if recursive else list(path.glob("*.*"))
+def get_duplicates(paths: list[Pathier]) -> list[list[Pathier]]:
+    """Return a list of lists for duplicate files in `paths`."""
     matching_sets = []
-    while len(files) > 0:
-        comparee = files.pop()
-        matching_files = [file for file in files if filecmp.cmp(comparee, file, False)]
+    while len(paths) > 0:
+        comparee = paths.pop()
+        matching_files = [file for file in paths if filecmp.cmp(comparee, file, False)]
         if matching_files:
-            [files.pop(files.index(file)) for file in matching_files]
+            [paths.pop(paths.index(file)) for file in matching_files]
             matching_files.insert(0, comparee)
             matching_sets.append(matching_files)
     return matching_sets
 
 
 def get_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser()
@@ -31,14 +30,24 @@
         "-r",
         "--recursive",
         action="store_true",
         help=""" Glob files to compare recursively. """,
     )
 
     parser.add_argument(
+        "-i",
+        "--ignores",
+        type=str,
+        nargs="*",
+        default=[],
+        help=""" Ignore files matching these patterns.
+        e.g. `dupechecker -i *.wav` will compare all files in the current working directory except .wav files.""",
+    )
+
+    parser.add_argument(
         "-d",
         "--delete_dupes",
         action="store_true",
         help=""" After finding duplicates, delete all but one copy.
         For each set of duplicates, the tool will ask you to enter the number corresponding to the copy you want to keep.
         Pressing 'enter' without entering a number will skip that set without deleting anything.""",
     )
@@ -54,24 +63,33 @@
         "-ns",
         "--no_show",
         action="store_true",
         help=""" Don't show printout of matching files. """,
     )
 
     parser.add_argument(
-        "path",
+        "paths",
         type=str,
-        default=Pathier.cwd(),
-        nargs="?",
-        help=""" The path to compare files in. """,
+        default=[Pathier.cwd()],
+        nargs="*",
+        help=""" The paths to compare files in. """,
     )
 
     args = parser.parse_args()
-    if not args.path == Pathier.cwd():
-        args.path = Pathier(args.path)
+    if not args.paths == [Pathier.cwd()]:
+        args.paths = [Pathier(path) for path in args.paths]
+    files = []
+    print("Gathering files...")
+    for path in args.paths:
+        files.extend(
+            list(path.rglob("*.*")) if args.recursive else list(path.glob("*.*"))
+        )
+    args.paths = younotyou([str(file) for file in files], exclude_patterns=args.ignores)
+    num_comparisons = len(list(combinations(args.paths, 2)))
+    print(f"Making {num_comparisons} comparisons between {len(args.paths)} files...")
 
     return args
 
 
 def delete_wizard(matches: list[list[Pathier]]):
     """Ask which file to keep for each set."""
     print()
@@ -104,15 +122,15 @@
         ch.rjust(i + j)
         for i in range(1, 25, 3)
         for j, ch in enumerate(["/", "-", "\\"])
     ]
     s += s[::-1]
     with Spinner(s) as spinner:
         with ThreadPoolExecutor() as exc:
-            thread = exc.submit(get_duplicates, args.path, args.recursive)
+            thread = exc.submit(get_duplicates, args.paths)
             while not thread.done():
                 spinner.display()
                 time.sleep(0.025)
             matches = thread.result()
     if matches:
         print(f"Found {len(matches)} duplicate sets of files.")
         if not args.no_show:
```

### Comparing `dupechecker-0.1.0/LICENSE.txt` & `dupechecker-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dupechecker-0.1.0/README.md` & `dupechecker-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `dupechecker-0.1.0/pyproject.toml` & `dupechecker-0.2.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -6,68 +6,68 @@
 00000050: 7072 6f6a 6563 745d 0d0a 6e61 6d65 203d  project]..name =
 00000060: 2022 6475 7065 6368 6563 6b65 7222 0d0a   "dupechecker"..
 00000070: 6465 7363 7269 7074 696f 6e20 3d20 2243  description = "C
 00000080: 6865 636b 2066 6f72 2061 6e64 2064 656c  heck for and del
 00000090: 6574 6520 6475 706c 6963 6174 6520 6669  ete duplicate fi
 000000a0: 6c65 7320 6672 6f6d 2074 6865 2063 6f6d  les from the com
 000000b0: 6d61 6e64 206c 696e 652e 220d 0a76 6572  mand line."..ver
-000000c0: 7369 6f6e 203d 2022 302e 312e 3022 0d0a  sion = "0.1.0"..
+000000c0: 7369 6f6e 203d 2022 302e 322e 3022 0d0a  sion = "0.2.0"..
 000000d0: 7265 7175 6972 6573 2d70 7974 686f 6e20  requires-python 
 000000e0: 3d20 223e 3d33 2e31 3022 0d0a 6465 7065  = ">=3.10"..depe
 000000f0: 6e64 656e 6369 6573 203d 205b 2267 7269  ndencies = ["gri
 00000100: 6464 6c65 222c 2022 7061 7468 6965 7222  ddle", "pathier"
 00000110: 2c20 2270 7269 6e74 6275 6464 6965 7322  , "printbuddies"
-00000120: 2c20 2270 7974 6573 7422 5d0d 0a72 6561  , "pytest"]..rea
-00000130: 646d 6520 3d20 2252 4541 444d 452e 6d64  dme = "README.md
-00000140: 220d 0a6b 6579 776f 7264 7320 3d20 5b22  "..keywords = ["
-00000150: 6669 6c65 636d 7022 2c20 2263 6c69 222c  filecmp", "cli",
-00000160: 2022 6669 6c65 7379 7374 656d 225d 0d0a   "filesystem"]..
-00000170: 636c 6173 7369 6669 6572 7320 3d20 5b0d  classifiers = [.
-00000180: 0a20 2020 2022 5072 6f67 7261 6d6d 696e  .    "Programmin
-00000190: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-000001a0: 7468 6f6e 203a 3a20 3322 2c0d 0a20 2020  thon :: 3",..   
-000001b0: 2022 4c69 6365 6e73 6520 3a3a 204f 5349   "License :: OSI
-000001c0: 2041 7070 726f 7665 6420 3a3a 204d 4954   Approved :: MIT
-000001d0: 204c 6963 656e 7365 222c 0d0a 2020 2020   License",..    
-000001e0: 224f 7065 7261 7469 6e67 2053 7973 7465  "Operating Syste
-000001f0: 6d20 3a3a 204f 5320 496e 6465 7065 6e64  m :: OS Independ
-00000200: 656e 7422 2c0d 0a20 2020 205d 0d0a 0d0a  ent",..    ]....
-00000210: 5b5b 7072 6f6a 6563 742e 6175 7468 6f72  [[project.author
-00000220: 735d 5d0d 0a6e 616d 6520 3d20 224d 6174  s]]..name = "Mat
-00000230: 7420 4d61 6e65 7322 0d0a 656d 6169 6c20  t Manes"..email 
-00000240: 3d20 226d 6174 746d 616e 6573 4070 6d2e  = "mattmanes@pm.
-00000250: 6d65 220d 0a0d 0a5b 7072 6f6a 6563 742e  me"....[project.
-00000260: 7572 6c73 5d0d 0a22 486f 6d65 7061 6765  urls].."Homepage
-00000270: 2220 3d20 2268 7474 7073 3a2f 2f67 6974  " = "https://git
-00000280: 6875 622e 636f 6d2f 6d61 7474 2d6d 616e  hub.com/matt-man
-00000290: 6573 2f64 7570 6563 6865 636b 6572 220d  es/dupechecker".
-000002a0: 0a22 446f 6375 6d65 6e74 6174 696f 6e22  ."Documentation"
-000002b0: 203d 2022 6874 7470 733a 2f2f 6769 7468   = "https://gith
-000002c0: 7562 2e63 6f6d 2f6d 6174 742d 6d61 6e65  ub.com/matt-mane
-000002d0: 732f 6475 7065 6368 6563 6b65 722f 7472  s/dupechecker/tr
-000002e0: 6565 2f6d 6169 6e2f 646f 6373 220d 0a22  ee/main/docs".."
-000002f0: 536f 7572 6365 2063 6f64 6522 203d 2022  Source code" = "
-00000300: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000310: 6f6d 2f6d 6174 742d 6d61 6e65 732f 6475  om/matt-manes/du
-00000320: 7065 6368 6563 6b65 722f 7472 6565 2f6d  pechecker/tree/m
-00000330: 6169 6e2f 7372 632f 6475 7065 6368 6563  ain/src/dupechec
-00000340: 6b65 7222 0d0a 0d0a 5b74 6f6f 6c2e 7079  ker"....[tool.py
-00000350: 7465 7374 2e69 6e69 5f6f 7074 696f 6e73  test.ini_options
-00000360: 5d0d 0a61 6464 6f70 7473 203d 205b 0d0a  ]..addopts = [..
-00000370: 2020 2020 222d 2d69 6d70 6f72 742d 6d6f      "--import-mo
-00000380: 6465 3d69 6d70 6f72 746c 6962 222c 0d0a  de=importlib",..
-00000390: 2020 2020 5d0d 0a70 7974 686f 6e70 6174      ]..pythonpat
-000003a0: 6820 3d20 2273 7263 220d 0a0d 0a5b 746f  h = "src"....[to
-000003b0: 6f6c 2e68 6174 6368 2e62 7569 6c64 2e74  ol.hatch.build.t
-000003c0: 6172 6765 7473 2e73 6469 7374 5d0d 0a65  argets.sdist]..e
-000003d0: 7863 6c75 6465 203d 205b 0d0a 2020 2020  xclude = [..    
-000003e0: 222e 636f 7665 7261 6765 222c 0d0a 2020  ".coverage",..  
-000003f0: 2020 222e 7079 7465 7374 5f63 6163 6865    ".pytest_cache
-00000400: 222c 0d0a 2020 2020 222e 7673 636f 6465  ",..    ".vscode
-00000410: 222c 0d0a 2020 2020 2274 6573 7473 222c  ",..    "tests",
-00000420: 0d0a 2020 2020 222e 6769 7469 676e 6f72  ..    ".gitignor
-00000430: 6522 0d0a 2020 2020 5d0d 0a5b 7072 6f6a  e"..    ]..[proj
-00000440: 6563 742e 7363 7269 7074 735d 0d0a 6475  ect.scripts]..du
-00000450: 7065 6368 6563 6b65 7220 3d20 2264 7570  pechecker = "dup
-00000460: 6563 6865 636b 6572 2e64 7570 6563 6865  echecker.dupeche
-00000470: 636b 6572 3a64 7570 6563 6865 636b 6572  cker:dupechecker
-00000480: 220d 0a                                  "..
+00000120: 2c20 2270 7974 6573 7422 2c20 2279 6f75  , "pytest", "you
+00000130: 6e6f 7479 6f75 225d 0d0a 7265 6164 6d65  notyou"]..readme
+00000140: 203d 2022 5245 4144 4d45 2e6d 6422 0d0a   = "README.md"..
+00000150: 6b65 7977 6f72 6473 203d 205b 2266 696c  keywords = ["fil
+00000160: 6563 6d70 222c 2022 636c 6922 2c20 2266  ecmp", "cli", "f
+00000170: 696c 6573 7973 7465 6d22 5d0d 0a63 6c61  ilesystem"]..cla
+00000180: 7373 6966 6965 7273 203d 205b 0d0a 2020  ssifiers = [..  
+00000190: 2020 2250 726f 6772 616d 6d69 6e67 204c    "Programming L
+000001a0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+000001b0: 6e20 3a3a 2033 222c 0d0a 2020 2020 224c  n :: 3",..    "L
+000001c0: 6963 656e 7365 203a 3a20 4f53 4920 4170  icense :: OSI Ap
+000001d0: 7072 6f76 6564 203a 3a20 4d49 5420 4c69  proved :: MIT Li
+000001e0: 6365 6e73 6522 2c0d 0a20 2020 2022 4f70  cense",..    "Op
+000001f0: 6572 6174 696e 6720 5379 7374 656d 203a  erating System :
+00000200: 3a20 4f53 2049 6e64 6570 656e 6465 6e74  : OS Independent
+00000210: 222c 0d0a 2020 2020 5d0d 0a0d 0a5b 5b70  ",..    ]....[[p
+00000220: 726f 6a65 6374 2e61 7574 686f 7273 5d5d  roject.authors]]
+00000230: 0d0a 6e61 6d65 203d 2022 4d61 7474 204d  ..name = "Matt M
+00000240: 616e 6573 220d 0a65 6d61 696c 203d 2022  anes"..email = "
+00000250: 6d61 7474 6d61 6e65 7340 706d 2e6d 6522  mattmanes@pm.me"
+00000260: 0d0a 0d0a 5b70 726f 6a65 6374 2e75 726c  ....[project.url
+00000270: 735d 0d0a 2248 6f6d 6570 6167 6522 203d  s].."Homepage" =
+00000280: 2022 6874 7470 733a 2f2f 6769 7468 7562   "https://github
+00000290: 2e63 6f6d 2f6d 6174 742d 6d61 6e65 732f  .com/matt-manes/
+000002a0: 6475 7065 6368 6563 6b65 7222 0d0a 2244  dupechecker".."D
+000002b0: 6f63 756d 656e 7461 7469 6f6e 2220 3d20  ocumentation" = 
+000002c0: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+000002d0: 636f 6d2f 6d61 7474 2d6d 616e 6573 2f64  com/matt-manes/d
+000002e0: 7570 6563 6865 636b 6572 2f74 7265 652f  upechecker/tree/
+000002f0: 6d61 696e 2f64 6f63 7322 0d0a 2253 6f75  main/docs".."Sou
+00000300: 7263 6520 636f 6465 2220 3d20 2268 7474  rce code" = "htt
+00000310: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000320: 6d61 7474 2d6d 616e 6573 2f64 7570 6563  matt-manes/dupec
+00000330: 6865 636b 6572 2f74 7265 652f 6d61 696e  hecker/tree/main
+00000340: 2f73 7263 2f64 7570 6563 6865 636b 6572  /src/dupechecker
+00000350: 220d 0a0d 0a5b 746f 6f6c 2e70 7974 6573  "....[tool.pytes
+00000360: 742e 696e 695f 6f70 7469 6f6e 735d 0d0a  t.ini_options]..
+00000370: 6164 646f 7074 7320 3d20 5b0d 0a20 2020  addopts = [..   
+00000380: 2022 2d2d 696d 706f 7274 2d6d 6f64 653d   "--import-mode=
+00000390: 696d 706f 7274 6c69 6222 2c0d 0a20 2020  importlib",..   
+000003a0: 205d 0d0a 7079 7468 6f6e 7061 7468 203d   ]..pythonpath =
+000003b0: 2022 7372 6322 0d0a 0d0a 5b74 6f6f 6c2e   "src"....[tool.
+000003c0: 6861 7463 682e 6275 696c 642e 7461 7267  hatch.build.targ
+000003d0: 6574 732e 7364 6973 745d 0d0a 6578 636c  ets.sdist]..excl
+000003e0: 7564 6520 3d20 5b0d 0a20 2020 2022 2e63  ude = [..    ".c
+000003f0: 6f76 6572 6167 6522 2c0d 0a20 2020 2022  overage",..    "
+00000400: 2e70 7974 6573 745f 6361 6368 6522 2c0d  .pytest_cache",.
+00000410: 0a20 2020 2022 2e76 7363 6f64 6522 2c0d  .    ".vscode",.
+00000420: 0a20 2020 2022 7465 7374 7322 2c0d 0a20  .    "tests",.. 
+00000430: 2020 2022 2e67 6974 6967 6e6f 7265 220d     ".gitignore".
+00000440: 0a20 2020 205d 0d0a 5b70 726f 6a65 6374  .    ]..[project
+00000450: 2e73 6372 6970 7473 5d0d 0a64 7570 6563  .scripts]..dupec
+00000460: 6865 636b 6572 203d 2022 6475 7065 6368  hecker = "dupech
+00000470: 6563 6b65 722e 6475 7065 6368 6563 6b65  ecker.dupechecke
+00000480: 723a 6475 7065 6368 6563 6b65 7222 0d0a  r:dupechecker"..
```

### Comparing `dupechecker-0.1.0/PKG-INFO` & `dupechecker-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dupechecker
-Version: 0.1.0
+Version: 0.2.0
 Summary: Check for and delete duplicate files from the command line.
 Project-URL: Homepage, https://github.com/matt-manes/dupechecker
 Project-URL: Documentation, https://github.com/matt-manes/dupechecker/tree/main/docs
 Project-URL: Source code, https://github.com/matt-manes/dupechecker/tree/main/src/dupechecker
 Author-email: Matt Manes <mattmanes@pm.me>
 License-File: LICENSE.txt
 Keywords: cli,filecmp,filesystem
@@ -12,14 +12,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: griddle
 Requires-Dist: pathier
 Requires-Dist: printbuddies
 Requires-Dist: pytest
+Requires-Dist: younotyou
 Description-Content-Type: text/markdown
 
 # dupechecker
 
 Check for and delete duplicate files from the command line.
 
 ## Installation
```

