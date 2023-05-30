# Comparing `tmp/gitbetter-1.1.0.tar.gz` & `tmp/gitbetter-1.2.0.tar.gz`

## Comparing `gitbetter-1.1.0.tar` & `gitbetter-1.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 gitbetter-1.1.0/CHANGELOG.md
--rw-r--r--   0        0        0    34128 2020-02-02 00:00:00.000000 gitbetter-1.1.0/docs/gitbetter.html
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 gitbetter-1.1.0/docs/index.html
--rw-r--r--   0        0        0    63347 2020-02-02 00:00:00.000000 gitbetter-1.1.0/docs/search.js
--rw-r--r--   0        0        0   226499 2020-02-02 00:00:00.000000 gitbetter-1.1.0/docs/gitbetter/git.html
--rw-r--r--   0        0        0   249963 2020-02-02 00:00:00.000000 gitbetter-1.1.0/docs/gitbetter/gitbetter.html
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 gitbetter-1.1.0/src/gitbetter/__init__.py
--rw-r--r--   0        0        0     8593 2020-02-02 00:00:00.000000 gitbetter-1.1.0/src/gitbetter/git.py
--rw-r--r--   0        0        0    10217 2020-02-02 00:00:00.000000 gitbetter-1.1.0/src/gitbetter/gitbetter.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 gitbetter-1.1.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 gitbetter-1.1.0/LICENSE.txt
--rw-r--r--   0        0        0     5091 2020-02-02 00:00:00.000000 gitbetter-1.1.0/README.md
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 gitbetter-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     5670 2020-02-02 00:00:00.000000 gitbetter-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 gitbetter-1.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0    34128 2020-02-02 00:00:00.000000 gitbetter-1.2.0/docs/gitbetter.html
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 gitbetter-1.2.0/docs/index.html
+-rw-r--r--   0        0        0    63693 2020-02-02 00:00:00.000000 gitbetter-1.2.0/docs/search.js
+-rw-r--r--   0        0        0   230942 2020-02-02 00:00:00.000000 gitbetter-1.2.0/docs/gitbetter/git.html
+-rw-r--r--   0        0        0   249963 2020-02-02 00:00:00.000000 gitbetter-1.2.0/docs/gitbetter/gitbetter.html
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 gitbetter-1.2.0/src/gitbetter/__init__.py
+-rw-r--r--   0        0        0     8779 2020-02-02 00:00:00.000000 gitbetter-1.2.0/src/gitbetter/git.py
+-rw-r--r--   0        0        0    10217 2020-02-02 00:00:00.000000 gitbetter-1.2.0/src/gitbetter/gitbetter.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 gitbetter-1.2.0/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 gitbetter-1.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     5825 2020-02-02 00:00:00.000000 gitbetter-1.2.0/README.md
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 gitbetter-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6382 2020-02-02 00:00:00.000000 gitbetter-1.2.0/PKG-INFO
```

### Comparing `gitbetter-1.1.0/CHANGELOG.md` & `gitbetter-1.2.0/CHANGELOG.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # Changelog
 
+## v1.1.0 (2023-05-26)
+
+#### Refactorings
+
+* change tag function parameter default and doc string
 ## v1.0.0 (2023-05-21)
 
 #### New Features
 
 * all git functions can return stdout as a string
 #### Fixes
```

### Comparing `gitbetter-1.1.0/docs/gitbetter.html` & `gitbetter-1.2.0/docs/gitbetter.html`

 * *Files identical despite different names*

### Comparing `gitbetter-1.1.0/docs/search.js` & `gitbetter-1.2.0/docs/search.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -709,14 +709,22 @@
         "fullname": "gitbetter.git.Git.capture_stdout",
         "modulename": "gitbetter.git",
         "qualname": "Git.capture_stdout",
         "kind": "variable",
         "doc": "<p>If <code>True</code>, member functions will return the generated <code>stdout</code> as a string,\notherwise they return the command's exit code.</p>\n",
         "annotation": ": bool"
     }, {
+        "fullname": "gitbetter.git.Git.capture_output",
+        "modulename": "gitbetter.git",
+        "qualname": "Git.capture_output",
+        "kind": "function",
+        "doc": "<p></p>\n",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span></span><span class=\"return-annotation\">):</span></span>",
+        "funcdef": "def"
+    }, {
         "fullname": "gitbetter.git.Git.execute",
         "modulename": "gitbetter.git",
         "qualname": "Git.execute",
         "kind": "function",
         "doc": "<p>Execute git command.</p>\n\n<p>Equivalent to executing <code>git {command}</code> in the shell.</p>\n",
         "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span>, </span><span class=\"param\"><span class=\"n\">command</span><span class=\"p\">:</span> <span class=\"nb\">str</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">str</span> <span class=\"o\">|</span> <span class=\"nb\">int</span>:</span></span>",
         "funcdef": "def"
```

### Comparing `gitbetter-1.1.0/docs/gitbetter/git.html` & `gitbetter-1.2.0/docs/gitbetter/git.html`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,17 @@
                         <li>
                                 <a class="function" href="#Git.__init__">Git</a>
                         </li>
                         <li>
                                 <a class="variable" href="#Git.capture_stdout">capture_stdout</a>
                         </li>
                         <li>
+                                <a class="function" href="#Git.capture_output">capture_output</a>
+                        </li>
+                        <li>
                                 <a class="function" href="#Git.execute">execute</a>
                         </li>
                         <li>
                                 <a class="function" href="#Git.new_repo">new_repo</a>
                         </li>
                         <li>
                                 <a class="function" href="#Git.loggy">loggy</a>
@@ -145,231 +148,238 @@
                 
                         <input id="mod-git-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 
                         <label class="view-source-button" for="mod-git-view-source"><span>View Source</span></label>
 
                         <div class="pdoc-code codehilite"><pre><span></span><span id="L-1"><a href="#L-1"><span class="linenos">  1</span></a><span class="kn">import</span> <span class="nn">shlex</span>
 </span><span id="L-2"><a href="#L-2"><span class="linenos">  2</span></a><span class="kn">import</span> <span class="nn">subprocess</span>
-</span><span id="L-3"><a href="#L-3"><span class="linenos">  3</span></a>
+</span><span id="L-3"><a href="#L-3"><span class="linenos">  3</span></a><span class="kn">from</span> <span class="nn">contextlib</span> <span class="kn">import</span> <span class="n">contextmanager</span>
 </span><span id="L-4"><a href="#L-4"><span class="linenos">  4</span></a>
-</span><span id="L-5"><a href="#L-5"><span class="linenos">  5</span></a><span class="k">class</span> <span class="nc">Git</span><span class="p">:</span>
-</span><span id="L-6"><a href="#L-6"><span class="linenos">  6</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">capture_stdout</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">):</span>
-</span><span id="L-7"><a href="#L-7"><span class="linenos">  7</span></a>        <span class="sd">&quot;&quot;&quot;If `capture_stdout` is `True`, all functions will return their generated `stdout` as a string.</span>
-</span><span id="L-8"><a href="#L-8"><span class="linenos">  8</span></a><span class="sd">        Otherwise, the functions return the call&#39;s exit code.&quot;&quot;&quot;</span>
-</span><span id="L-9"><a href="#L-9"><span class="linenos">  9</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">capture_stdout</span> <span class="o">=</span> <span class="n">capture_stdout</span>
-</span><span id="L-10"><a href="#L-10"><span class="linenos"> 10</span></a>
-</span><span id="L-11"><a href="#L-11"><span class="linenos"> 11</span></a>    <span class="nd">@property</span>
-</span><span id="L-12"><a href="#L-12"><span class="linenos"> 12</span></a>    <span class="k">def</span> <span class="nf">capture_stdout</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="L-13"><a href="#L-13"><span class="linenos"> 13</span></a>        <span class="sd">&quot;&quot;&quot;If `True`, member functions will return the generated `stdout` as a string,</span>
-</span><span id="L-14"><a href="#L-14"><span class="linenos"> 14</span></a><span class="sd">        otherwise they return the command&#39;s exit code.&quot;&quot;&quot;</span>
-</span><span id="L-15"><a href="#L-15"><span class="linenos"> 15</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_capture_stdout</span>
-</span><span id="L-16"><a href="#L-16"><span class="linenos"> 16</span></a>
-</span><span id="L-17"><a href="#L-17"><span class="linenos"> 17</span></a>    <span class="nd">@capture_stdout</span><span class="o">.</span><span class="n">setter</span>
-</span><span id="L-18"><a href="#L-18"><span class="linenos"> 18</span></a>    <span class="k">def</span> <span class="nf">capture_stdout</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">should_capture</span><span class="p">:</span> <span class="nb">bool</span><span class="p">):</span>
-</span><span id="L-19"><a href="#L-19"><span class="linenos"> 19</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_capture_stdout</span> <span class="o">=</span> <span class="n">should_capture</span>
-</span><span id="L-20"><a href="#L-20"><span class="linenos"> 20</span></a>
-</span><span id="L-21"><a href="#L-21"><span class="linenos"> 21</span></a>    <span class="k">def</span> <span class="nf">_run</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="L-22"><a href="#L-22"><span class="linenos"> 22</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_capture_stdout</span><span class="p">:</span>
-</span><span id="L-23"><a href="#L-23"><span class="linenos"> 23</span></a>            <span class="k">return</span> <span class="n">subprocess</span><span class="o">.</span><span class="n">run</span><span class="p">(</span><span class="n">args</span><span class="p">,</span> <span class="n">stdout</span><span class="o">=</span><span class="n">subprocess</span><span class="o">.</span><span class="n">PIPE</span><span class="p">,</span> <span class="n">text</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span><span class="o">.</span><span class="n">stdout</span>
-</span><span id="L-24"><a href="#L-24"><span class="linenos"> 24</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="L-25"><a href="#L-25"><span class="linenos"> 25</span></a>            <span class="k">return</span> <span class="n">subprocess</span><span class="o">.</span><span class="n">run</span><span class="p">(</span><span class="n">args</span><span class="p">)</span><span class="o">.</span><span class="n">returncode</span>
-</span><span id="L-26"><a href="#L-26"><span class="linenos"> 26</span></a>
-</span><span id="L-27"><a href="#L-27"><span class="linenos"> 27</span></a>    <span class="k">def</span> <span class="nf">execute</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">command</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="L-28"><a href="#L-28"><span class="linenos"> 28</span></a>        <span class="sd">&quot;&quot;&quot;Execute git command.</span>
-</span><span id="L-29"><a href="#L-29"><span class="linenos"> 29</span></a>
-</span><span id="L-30"><a href="#L-30"><span class="linenos"> 30</span></a><span class="sd">        Equivalent to executing `git {command}` in the shell.&quot;&quot;&quot;</span>
-</span><span id="L-31"><a href="#L-31"><span class="linenos"> 31</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="p">[</span><span class="s2">&quot;git&quot;</span><span class="p">]</span> <span class="o">+</span> <span class="n">shlex</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="n">command</span><span class="p">)</span>
-</span><span id="L-32"><a href="#L-32"><span class="linenos"> 32</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
+</span><span id="L-5"><a href="#L-5"><span class="linenos">  5</span></a>
+</span><span id="L-6"><a href="#L-6"><span class="linenos">  6</span></a><span class="k">class</span> <span class="nc">Git</span><span class="p">:</span>
+</span><span id="L-7"><a href="#L-7"><span class="linenos">  7</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">capture_stdout</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">):</span>
+</span><span id="L-8"><a href="#L-8"><span class="linenos">  8</span></a>        <span class="sd">&quot;&quot;&quot;If `capture_stdout` is `True`, all functions will return their generated `stdout` as a string.</span>
+</span><span id="L-9"><a href="#L-9"><span class="linenos">  9</span></a><span class="sd">        Otherwise, the functions return the call&#39;s exit code.&quot;&quot;&quot;</span>
+</span><span id="L-10"><a href="#L-10"><span class="linenos"> 10</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">capture_stdout</span> <span class="o">=</span> <span class="n">capture_stdout</span>
+</span><span id="L-11"><a href="#L-11"><span class="linenos"> 11</span></a>
+</span><span id="L-12"><a href="#L-12"><span class="linenos"> 12</span></a>    <span class="nd">@contextmanager</span>
+</span><span id="L-13"><a href="#L-13"><span class="linenos"> 13</span></a>    <span class="k">def</span> <span class="nf">capture_output</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="L-14"><a href="#L-14"><span class="linenos"> 14</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">capture_stdout</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="L-15"><a href="#L-15"><span class="linenos"> 15</span></a>        <span class="k">yield</span> <span class="bp">self</span>
+</span><span id="L-16"><a href="#L-16"><span class="linenos"> 16</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">capture_stdout</span> <span class="o">=</span> <span class="kc">False</span>
+</span><span id="L-17"><a href="#L-17"><span class="linenos"> 17</span></a>
+</span><span id="L-18"><a href="#L-18"><span class="linenos"> 18</span></a>    <span class="nd">@property</span>
+</span><span id="L-19"><a href="#L-19"><span class="linenos"> 19</span></a>    <span class="k">def</span> <span class="nf">capture_stdout</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="L-20"><a href="#L-20"><span class="linenos"> 20</span></a>        <span class="sd">&quot;&quot;&quot;If `True`, member functions will return the generated `stdout` as a string,</span>
+</span><span id="L-21"><a href="#L-21"><span class="linenos"> 21</span></a><span class="sd">        otherwise they return the command&#39;s exit code.&quot;&quot;&quot;</span>
+</span><span id="L-22"><a href="#L-22"><span class="linenos"> 22</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_capture_stdout</span>
+</span><span id="L-23"><a href="#L-23"><span class="linenos"> 23</span></a>
+</span><span id="L-24"><a href="#L-24"><span class="linenos"> 24</span></a>    <span class="nd">@capture_stdout</span><span class="o">.</span><span class="n">setter</span>
+</span><span id="L-25"><a href="#L-25"><span class="linenos"> 25</span></a>    <span class="k">def</span> <span class="nf">capture_stdout</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">should_capture</span><span class="p">:</span> <span class="nb">bool</span><span class="p">):</span>
+</span><span id="L-26"><a href="#L-26"><span class="linenos"> 26</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_capture_stdout</span> <span class="o">=</span> <span class="n">should_capture</span>
+</span><span id="L-27"><a href="#L-27"><span class="linenos"> 27</span></a>
+</span><span id="L-28"><a href="#L-28"><span class="linenos"> 28</span></a>    <span class="k">def</span> <span class="nf">_run</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="L-29"><a href="#L-29"><span class="linenos"> 29</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_capture_stdout</span><span class="p">:</span>
+</span><span id="L-30"><a href="#L-30"><span class="linenos"> 30</span></a>            <span class="k">return</span> <span class="n">subprocess</span><span class="o">.</span><span class="n">run</span><span class="p">(</span><span class="n">args</span><span class="p">,</span> <span class="n">stdout</span><span class="o">=</span><span class="n">subprocess</span><span class="o">.</span><span class="n">PIPE</span><span class="p">,</span> <span class="n">text</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span><span class="o">.</span><span class="n">stdout</span>
+</span><span id="L-31"><a href="#L-31"><span class="linenos"> 31</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="L-32"><a href="#L-32"><span class="linenos"> 32</span></a>            <span class="k">return</span> <span class="n">subprocess</span><span class="o">.</span><span class="n">run</span><span class="p">(</span><span class="n">args</span><span class="p">)</span><span class="o">.</span><span class="n">returncode</span>
 </span><span id="L-33"><a href="#L-33"><span class="linenos"> 33</span></a>
-</span><span id="L-34"><a href="#L-34"><span class="linenos"> 34</span></a>    <span class="k">def</span> <span class="nf">new_repo</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="L-35"><a href="#L-35"><span class="linenos"> 35</span></a>        <span class="sd">&quot;&quot;&quot;Executes `git init -b main`.&quot;&quot;&quot;</span>
-</span><span id="L-36"><a href="#L-36"><span class="linenos"> 36</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="s2">&quot;init -b main&quot;</span><span class="p">)</span>
-</span><span id="L-37"><a href="#L-37"><span class="linenos"> 37</span></a>
-</span><span id="L-38"><a href="#L-38"><span class="linenos"> 38</span></a>    <span class="k">def</span> <span class="nf">loggy</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="L-39"><a href="#L-39"><span class="linenos"> 39</span></a>        <span class="sd">&quot;&quot;&quot;Equivalent to `git log --oneline --name-only --abbrev-commit --graph`.&quot;&quot;&quot;</span>
-</span><span id="L-40"><a href="#L-40"><span class="linenos"> 40</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="s2">&quot;log --oneline --name-only --abbrev-commit --graph&quot;</span><span class="p">)</span>
-</span><span id="L-41"><a href="#L-41"><span class="linenos"> 41</span></a>
-</span><span id="L-42"><a href="#L-42"><span class="linenos"> 42</span></a>    <span class="k">def</span> <span class="nf">status</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="L-43"><a href="#L-43"><span class="linenos"> 43</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git status`.&quot;&quot;&quot;</span>
-</span><span id="L-44"><a href="#L-44"><span class="linenos"> 44</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="s2">&quot;status&quot;</span><span class="p">)</span>
-</span><span id="L-45"><a href="#L-45"><span class="linenos"> 45</span></a>
-</span><span id="L-46"><a href="#L-46"><span class="linenos"> 46</span></a>    <span class="c1"># ======================================Staging/Committing======================================</span>
-</span><span id="L-47"><a href="#L-47"><span class="linenos"> 47</span></a>    <span class="k">def</span> <span class="nf">commit</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="L-48"><a href="#L-48"><span class="linenos"> 48</span></a>        <span class="sd">&quot;&quot;&quot;&gt;&gt;&gt; git commit {args}&quot;&quot;&quot;</span>
-</span><span id="L-49"><a href="#L-49"><span class="linenos"> 49</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;commit </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-50"><a href="#L-50"><span class="linenos"> 50</span></a>
-</span><span id="L-51"><a href="#L-51"><span class="linenos"> 51</span></a>    <span class="k">def</span> <span class="nf">add</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">files</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="L-52"><a href="#L-52"><span class="linenos"> 52</span></a>        <span class="sd">&quot;&quot;&quot;Stage a list of files.</span>
-</span><span id="L-53"><a href="#L-53"><span class="linenos"> 53</span></a>
-</span><span id="L-54"><a href="#L-54"><span class="linenos"> 54</span></a><span class="sd">        If no files are given (`files=None`), all files will be staged.&quot;&quot;&quot;</span>
-</span><span id="L-55"><a href="#L-55"><span class="linenos"> 55</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">files</span><span class="p">:</span>
-</span><span id="L-56"><a href="#L-56"><span class="linenos"> 56</span></a>            <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="s2">&quot;add .&quot;</span><span class="p">)</span>
-</span><span id="L-57"><a href="#L-57"><span class="linenos"> 57</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="L-58"><a href="#L-58"><span class="linenos"> 58</span></a>            <span class="n">files</span> <span class="o">=</span> <span class="s2">&quot; &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;&quot;</span><span class="si">{</span><span class="n">file</span><span class="si">}</span><span class="s1">&quot;&#39;</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">files</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
-</span><span id="L-59"><a href="#L-59"><span class="linenos"> 59</span></a>            <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;add </span><span class="si">{</span><span class="n">files</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-34"><a href="#L-34"><span class="linenos"> 34</span></a>    <span class="k">def</span> <span class="nf">execute</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">command</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="L-35"><a href="#L-35"><span class="linenos"> 35</span></a>        <span class="sd">&quot;&quot;&quot;Execute git command.</span>
+</span><span id="L-36"><a href="#L-36"><span class="linenos"> 36</span></a>
+</span><span id="L-37"><a href="#L-37"><span class="linenos"> 37</span></a><span class="sd">        Equivalent to executing `git {command}` in the shell.&quot;&quot;&quot;</span>
+</span><span id="L-38"><a href="#L-38"><span class="linenos"> 38</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="p">[</span><span class="s2">&quot;git&quot;</span><span class="p">]</span> <span class="o">+</span> <span class="n">shlex</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="n">command</span><span class="p">)</span>
+</span><span id="L-39"><a href="#L-39"><span class="linenos"> 39</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
+</span><span id="L-40"><a href="#L-40"><span class="linenos"> 40</span></a>
+</span><span id="L-41"><a href="#L-41"><span class="linenos"> 41</span></a>    <span class="k">def</span> <span class="nf">new_repo</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="L-42"><a href="#L-42"><span class="linenos"> 42</span></a>        <span class="sd">&quot;&quot;&quot;Executes `git init -b main`.&quot;&quot;&quot;</span>
+</span><span id="L-43"><a href="#L-43"><span class="linenos"> 43</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="s2">&quot;init -b main&quot;</span><span class="p">)</span>
+</span><span id="L-44"><a href="#L-44"><span class="linenos"> 44</span></a>
+</span><span id="L-45"><a href="#L-45"><span class="linenos"> 45</span></a>    <span class="k">def</span> <span class="nf">loggy</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="L-46"><a href="#L-46"><span class="linenos"> 46</span></a>        <span class="sd">&quot;&quot;&quot;Equivalent to `git log --oneline --name-only --abbrev-commit --graph`.&quot;&quot;&quot;</span>
+</span><span id="L-47"><a href="#L-47"><span class="linenos"> 47</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="s2">&quot;log --oneline --name-only --abbrev-commit --graph&quot;</span><span class="p">)</span>
+</span><span id="L-48"><a href="#L-48"><span class="linenos"> 48</span></a>
+</span><span id="L-49"><a href="#L-49"><span class="linenos"> 49</span></a>    <span class="k">def</span> <span class="nf">status</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="L-50"><a href="#L-50"><span class="linenos"> 50</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git status`.&quot;&quot;&quot;</span>
+</span><span id="L-51"><a href="#L-51"><span class="linenos"> 51</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="s2">&quot;status&quot;</span><span class="p">)</span>
+</span><span id="L-52"><a href="#L-52"><span class="linenos"> 52</span></a>
+</span><span id="L-53"><a href="#L-53"><span class="linenos"> 53</span></a>    <span class="c1"># ======================================Staging/Committing======================================</span>
+</span><span id="L-54"><a href="#L-54"><span class="linenos"> 54</span></a>    <span class="k">def</span> <span class="nf">commit</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="L-55"><a href="#L-55"><span class="linenos"> 55</span></a>        <span class="sd">&quot;&quot;&quot;&gt;&gt;&gt; git commit {args}&quot;&quot;&quot;</span>
+</span><span id="L-56"><a href="#L-56"><span class="linenos"> 56</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;commit </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-57"><a href="#L-57"><span class="linenos"> 57</span></a>
+</span><span id="L-58"><a href="#L-58"><span class="linenos"> 58</span></a>    <span class="k">def</span> <span class="nf">add</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">files</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="L-59"><a href="#L-59"><span class="linenos"> 59</span></a>        <span class="sd">&quot;&quot;&quot;Stage a list of files.</span>
 </span><span id="L-60"><a href="#L-60"><span class="linenos"> 60</span></a>
-</span><span id="L-61"><a href="#L-61"><span class="linenos"> 61</span></a>    <span class="k">def</span> <span class="nf">commit_files</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">files</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">],</span> <span class="n">message</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="L-62"><a href="#L-62"><span class="linenos"> 62</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit a list of files with commit message `message`.&quot;&quot;&quot;</span>
-</span><span id="L-63"><a href="#L-63"><span class="linenos"> 63</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">add</span><span class="p">(</span><span class="n">files</span><span class="p">)</span> <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;-m &quot;</span><span class="si">{</span><span class="n">message</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
-</span><span id="L-64"><a href="#L-64"><span class="linenos"> 64</span></a>
-</span><span id="L-65"><a href="#L-65"><span class="linenos"> 65</span></a>    <span class="k">def</span> <span class="nf">initcommit</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="L-66"><a href="#L-66"><span class="linenos"> 66</span></a>        <span class="sd">&quot;&quot;&quot;Equivalent to</span>
-</span><span id="L-67"><a href="#L-67"><span class="linenos"> 67</span></a><span class="sd">        &gt;&gt;&gt; git add .</span>
-</span><span id="L-68"><a href="#L-68"><span class="linenos"> 68</span></a><span class="sd">        &gt;&gt;&gt; git commit -m &quot;Initial commit&quot; &quot;&quot;&quot;</span>
-</span><span id="L-69"><a href="#L-69"><span class="linenos"> 69</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">add</span><span class="p">()</span> <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="s1">&#39;-m &quot;Initial commit&quot;&#39;</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
-</span><span id="L-70"><a href="#L-70"><span class="linenos"> 70</span></a>
-</span><span id="L-71"><a href="#L-71"><span class="linenos"> 71</span></a>    <span class="k">def</span> <span class="nf">amend</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">files</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="L-72"><a href="#L-72"><span class="linenos"> 72</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit changes to the previous commit.</span>
-</span><span id="L-73"><a href="#L-73"><span class="linenos"> 73</span></a>
-</span><span id="L-74"><a href="#L-74"><span class="linenos"> 74</span></a><span class="sd">        If `files` is `None`, all files will be staged.</span>
-</span><span id="L-75"><a href="#L-75"><span class="linenos"> 75</span></a>
-</span><span id="L-76"><a href="#L-76"><span class="linenos"> 76</span></a><span class="sd">        Equivalent to:</span>
-</span><span id="L-77"><a href="#L-77"><span class="linenos"> 77</span></a><span class="sd">        &gt;&gt;&gt; git add {files}</span>
-</span><span id="L-78"><a href="#L-78"><span class="linenos"> 78</span></a><span class="sd">        &gt;&gt;&gt; git commit --amend --no-edit</span>
-</span><span id="L-79"><a href="#L-79"><span class="linenos"> 79</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="L-80"><a href="#L-80"><span class="linenos"> 80</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">add</span><span class="p">(</span><span class="n">files</span><span class="p">)</span> <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="s2">&quot;--amend --no-edit&quot;</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
-</span><span id="L-81"><a href="#L-81"><span class="linenos"> 81</span></a>
-</span><span id="L-82"><a href="#L-82"><span class="linenos"> 82</span></a>    <span class="k">def</span> <span class="nf">tag</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="L-83"><a href="#L-83"><span class="linenos"> 83</span></a>        <span class="sd">&quot;&quot;&quot;Execute the `tag` command with `args`.</span>
-</span><span id="L-84"><a href="#L-84"><span class="linenos"> 84</span></a>
-</span><span id="L-85"><a href="#L-85"><span class="linenos"> 85</span></a><span class="sd">        e.g.</span>
-</span><span id="L-86"><a href="#L-86"><span class="linenos"> 86</span></a>
-</span><span id="L-87"><a href="#L-87"><span class="linenos"> 87</span></a><span class="sd">        `self.tag(&quot;--sort=-committerdate&quot;)`</span>
+</span><span id="L-61"><a href="#L-61"><span class="linenos"> 61</span></a><span class="sd">        If no files are given (`files=None`), all files will be staged.&quot;&quot;&quot;</span>
+</span><span id="L-62"><a href="#L-62"><span class="linenos"> 62</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">files</span><span class="p">:</span>
+</span><span id="L-63"><a href="#L-63"><span class="linenos"> 63</span></a>            <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="s2">&quot;add .&quot;</span><span class="p">)</span>
+</span><span id="L-64"><a href="#L-64"><span class="linenos"> 64</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="L-65"><a href="#L-65"><span class="linenos"> 65</span></a>            <span class="n">files</span> <span class="o">=</span> <span class="s2">&quot; &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;&quot;</span><span class="si">{</span><span class="n">file</span><span class="si">}</span><span class="s1">&quot;&#39;</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">files</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
+</span><span id="L-66"><a href="#L-66"><span class="linenos"> 66</span></a>            <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;add </span><span class="si">{</span><span class="n">files</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-67"><a href="#L-67"><span class="linenos"> 67</span></a>
+</span><span id="L-68"><a href="#L-68"><span class="linenos"> 68</span></a>    <span class="k">def</span> <span class="nf">commit_files</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">files</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">],</span> <span class="n">message</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="L-69"><a href="#L-69"><span class="linenos"> 69</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit a list of files with commit message `message`.&quot;&quot;&quot;</span>
+</span><span id="L-70"><a href="#L-70"><span class="linenos"> 70</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">add</span><span class="p">(</span><span class="n">files</span><span class="p">)</span> <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;-m &quot;</span><span class="si">{</span><span class="n">message</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
+</span><span id="L-71"><a href="#L-71"><span class="linenos"> 71</span></a>
+</span><span id="L-72"><a href="#L-72"><span class="linenos"> 72</span></a>    <span class="k">def</span> <span class="nf">initcommit</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="L-73"><a href="#L-73"><span class="linenos"> 73</span></a>        <span class="sd">&quot;&quot;&quot;Equivalent to</span>
+</span><span id="L-74"><a href="#L-74"><span class="linenos"> 74</span></a><span class="sd">        &gt;&gt;&gt; git add .</span>
+</span><span id="L-75"><a href="#L-75"><span class="linenos"> 75</span></a><span class="sd">        &gt;&gt;&gt; git commit -m &quot;Initial commit&quot; &quot;&quot;&quot;</span>
+</span><span id="L-76"><a href="#L-76"><span class="linenos"> 76</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">add</span><span class="p">()</span> <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="s1">&#39;-m &quot;Initial commit&quot;&#39;</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
+</span><span id="L-77"><a href="#L-77"><span class="linenos"> 77</span></a>
+</span><span id="L-78"><a href="#L-78"><span class="linenos"> 78</span></a>    <span class="k">def</span> <span class="nf">amend</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">files</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="L-79"><a href="#L-79"><span class="linenos"> 79</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit changes to the previous commit.</span>
+</span><span id="L-80"><a href="#L-80"><span class="linenos"> 80</span></a>
+</span><span id="L-81"><a href="#L-81"><span class="linenos"> 81</span></a><span class="sd">        If `files` is `None`, all files will be staged.</span>
+</span><span id="L-82"><a href="#L-82"><span class="linenos"> 82</span></a>
+</span><span id="L-83"><a href="#L-83"><span class="linenos"> 83</span></a><span class="sd">        Equivalent to:</span>
+</span><span id="L-84"><a href="#L-84"><span class="linenos"> 84</span></a><span class="sd">        &gt;&gt;&gt; git add {files}</span>
+</span><span id="L-85"><a href="#L-85"><span class="linenos"> 85</span></a><span class="sd">        &gt;&gt;&gt; git commit --amend --no-edit</span>
+</span><span id="L-86"><a href="#L-86"><span class="linenos"> 86</span></a><span class="sd">        &quot;&quot;&quot;</span>
+</span><span id="L-87"><a href="#L-87"><span class="linenos"> 87</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">add</span><span class="p">(</span><span class="n">files</span><span class="p">)</span> <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="s2">&quot;--amend --no-edit&quot;</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
 </span><span id="L-88"><a href="#L-88"><span class="linenos"> 88</span></a>
-</span><span id="L-89"><a href="#L-89"><span class="linenos"> 89</span></a><span class="sd">        will list all the tags for this repository in descending commit date.&quot;&quot;&quot;</span>
-</span><span id="L-90"><a href="#L-90"><span class="linenos"> 90</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;tag </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-89"><a href="#L-89"><span class="linenos"> 89</span></a>    <span class="k">def</span> <span class="nf">tag</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="L-90"><a href="#L-90"><span class="linenos"> 90</span></a>        <span class="sd">&quot;&quot;&quot;Execute the `tag` command with `args`.</span>
 </span><span id="L-91"><a href="#L-91"><span class="linenos"> 91</span></a>
-</span><span id="L-92"><a href="#L-92"><span class="linenos"> 92</span></a>    <span class="c1"># ==========================================Push/Pull==========================================</span>
-</span><span id="L-93"><a href="#L-93"><span class="linenos"> 93</span></a>    <span class="k">def</span> <span class="nf">add_remote_url</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">url</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;origin&quot;</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="L-94"><a href="#L-94"><span class="linenos"> 94</span></a>        <span class="sd">&quot;&quot;&quot;Add remote url to repo.&quot;&quot;&quot;</span>
-</span><span id="L-95"><a href="#L-95"><span class="linenos"> 95</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;remote add </span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">url</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-96"><a href="#L-96"><span class="linenos"> 96</span></a>
-</span><span id="L-97"><a href="#L-97"><span class="linenos"> 97</span></a>    <span class="k">def</span> <span class="nf">push</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="L-98"><a href="#L-98"><span class="linenos"> 98</span></a>        <span class="sd">&quot;&quot;&quot;Equivalent to `git push {args}`.&quot;&quot;&quot;</span>
-</span><span id="L-99"><a href="#L-99"><span class="linenos"> 99</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;push </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-100"><a href="#L-100"><span class="linenos">100</span></a>
-</span><span id="L-101"><a href="#L-101"><span class="linenos">101</span></a>    <span class="k">def</span> <span class="nf">pull</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="L-102"><a href="#L-102"><span class="linenos">102</span></a>        <span class="sd">&quot;&quot;&quot;Equivalent to `git pull {args}`.&quot;&quot;&quot;</span>
-</span><span id="L-103"><a href="#L-103"><span class="linenos">103</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;pull </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-104"><a href="#L-104"><span class="linenos">104</span></a>
-</span><span id="L-105"><a href="#L-105"><span class="linenos">105</span></a>    <span class="k">def</span> <span class="nf">push_new_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="L-106"><a href="#L-106"><span class="linenos">106</span></a>        <span class="sd">&quot;&quot;&quot;Push a new branch to origin with tracking.</span>
+</span><span id="L-92"><a href="#L-92"><span class="linenos"> 92</span></a><span class="sd">        e.g.</span>
+</span><span id="L-93"><a href="#L-93"><span class="linenos"> 93</span></a>
+</span><span id="L-94"><a href="#L-94"><span class="linenos"> 94</span></a><span class="sd">        `self.tag(&quot;--sort=-committerdate&quot;)`</span>
+</span><span id="L-95"><a href="#L-95"><span class="linenos"> 95</span></a>
+</span><span id="L-96"><a href="#L-96"><span class="linenos"> 96</span></a><span class="sd">        will list all the tags for this repository in descending commit date.&quot;&quot;&quot;</span>
+</span><span id="L-97"><a href="#L-97"><span class="linenos"> 97</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;tag </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-98"><a href="#L-98"><span class="linenos"> 98</span></a>
+</span><span id="L-99"><a href="#L-99"><span class="linenos"> 99</span></a>    <span class="c1"># ==========================================Push/Pull==========================================</span>
+</span><span id="L-100"><a href="#L-100"><span class="linenos">100</span></a>    <span class="k">def</span> <span class="nf">add_remote_url</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">url</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;origin&quot;</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="L-101"><a href="#L-101"><span class="linenos">101</span></a>        <span class="sd">&quot;&quot;&quot;Add remote url to repo.&quot;&quot;&quot;</span>
+</span><span id="L-102"><a href="#L-102"><span class="linenos">102</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;remote add </span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">url</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-103"><a href="#L-103"><span class="linenos">103</span></a>
+</span><span id="L-104"><a href="#L-104"><span class="linenos">104</span></a>    <span class="k">def</span> <span class="nf">push</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="L-105"><a href="#L-105"><span class="linenos">105</span></a>        <span class="sd">&quot;&quot;&quot;Equivalent to `git push {args}`.&quot;&quot;&quot;</span>
+</span><span id="L-106"><a href="#L-106"><span class="linenos">106</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;push </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span><span id="L-107"><a href="#L-107"><span class="linenos">107</span></a>
-</span><span id="L-108"><a href="#L-108"><span class="linenos">108</span></a><span class="sd">        Equivalent to `git push -u origin {branch}`.&quot;&quot;&quot;</span>
-</span><span id="L-109"><a href="#L-109"><span class="linenos">109</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-u origin </span><span class="si">{</span><span class="n">branch</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-110"><a href="#L-110"><span class="linenos">110</span></a>
-</span><span id="L-111"><a href="#L-111"><span class="linenos">111</span></a>    <span class="k">def</span> <span class="nf">pull_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a>        <span class="sd">&quot;&quot;&quot;Pull `branch` from origin.&quot;&quot;&quot;</span>
-</span><span id="L-113"><a href="#L-113"><span class="linenos">113</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">pull</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;origin </span><span class="si">{</span><span class="n">branch</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-108"><a href="#L-108"><span class="linenos">108</span></a>    <span class="k">def</span> <span class="nf">pull</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="L-109"><a href="#L-109"><span class="linenos">109</span></a>        <span class="sd">&quot;&quot;&quot;Equivalent to `git pull {args}`.&quot;&quot;&quot;</span>
+</span><span id="L-110"><a href="#L-110"><span class="linenos">110</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;pull </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-111"><a href="#L-111"><span class="linenos">111</span></a>
+</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a>    <span class="k">def</span> <span class="nf">push_new_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="L-113"><a href="#L-113"><span class="linenos">113</span></a>        <span class="sd">&quot;&quot;&quot;Push a new branch to origin with tracking.</span>
 </span><span id="L-114"><a href="#L-114"><span class="linenos">114</span></a>
-</span><span id="L-115"><a href="#L-115"><span class="linenos">115</span></a>    <span class="c1"># ============================================Checkout/Branches============================================</span>
-</span><span id="L-116"><a href="#L-116"><span class="linenos">116</span></a>    <span class="k">def</span> <span class="nf">branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="L-117"><a href="#L-117"><span class="linenos">117</span></a>        <span class="sd">&quot;&quot;&quot;Equivalent to `git branch {args}`.&quot;&quot;&quot;</span>
-</span><span id="L-118"><a href="#L-118"><span class="linenos">118</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;branch </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-119"><a href="#L-119"><span class="linenos">119</span></a>
-</span><span id="L-120"><a href="#L-120"><span class="linenos">120</span></a>    <span class="k">def</span> <span class="nf">list_branches</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="L-121"><a href="#L-121"><span class="linenos">121</span></a>        <span class="sd">&quot;&quot;&quot;Print a list of branches.&quot;&quot;&quot;</span>
-</span><span id="L-122"><a href="#L-122"><span class="linenos">122</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">branch</span><span class="p">(</span><span class="s2">&quot;-vva&quot;</span><span class="p">)</span>
-</span><span id="L-123"><a href="#L-123"><span class="linenos">123</span></a>
-</span><span id="L-124"><a href="#L-124"><span class="linenos">124</span></a>    <span class="k">def</span> <span class="nf">checkout</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="L-125"><a href="#L-125"><span class="linenos">125</span></a>        <span class="sd">&quot;&quot;&quot;Equivalent to `git checkout {args}`.&quot;&quot;&quot;</span>
-</span><span id="L-126"><a href="#L-126"><span class="linenos">126</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;checkout </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-127"><a href="#L-127"><span class="linenos">127</span></a>
-</span><span id="L-128"><a href="#L-128"><span class="linenos">128</span></a>    <span class="k">def</span> <span class="nf">switch_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="L-129"><a href="#L-129"><span class="linenos">129</span></a>        <span class="sd">&quot;&quot;&quot;Switch to the branch specified by `branch_name`.</span>
+</span><span id="L-115"><a href="#L-115"><span class="linenos">115</span></a><span class="sd">        Equivalent to `git push -u origin {branch}`.&quot;&quot;&quot;</span>
+</span><span id="L-116"><a href="#L-116"><span class="linenos">116</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-u origin </span><span class="si">{</span><span class="n">branch</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-117"><a href="#L-117"><span class="linenos">117</span></a>
+</span><span id="L-118"><a href="#L-118"><span class="linenos">118</span></a>    <span class="k">def</span> <span class="nf">pull_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="L-119"><a href="#L-119"><span class="linenos">119</span></a>        <span class="sd">&quot;&quot;&quot;Pull `branch` from origin.&quot;&quot;&quot;</span>
+</span><span id="L-120"><a href="#L-120"><span class="linenos">120</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">pull</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;origin </span><span class="si">{</span><span class="n">branch</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-121"><a href="#L-121"><span class="linenos">121</span></a>
+</span><span id="L-122"><a href="#L-122"><span class="linenos">122</span></a>    <span class="c1"># ============================================Checkout/Branches============================================</span>
+</span><span id="L-123"><a href="#L-123"><span class="linenos">123</span></a>    <span class="k">def</span> <span class="nf">branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="L-124"><a href="#L-124"><span class="linenos">124</span></a>        <span class="sd">&quot;&quot;&quot;Equivalent to `git branch {args}`.&quot;&quot;&quot;</span>
+</span><span id="L-125"><a href="#L-125"><span class="linenos">125</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;branch </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-126"><a href="#L-126"><span class="linenos">126</span></a>
+</span><span id="L-127"><a href="#L-127"><span class="linenos">127</span></a>    <span class="k">def</span> <span class="nf">list_branches</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="L-128"><a href="#L-128"><span class="linenos">128</span></a>        <span class="sd">&quot;&quot;&quot;Print a list of branches.&quot;&quot;&quot;</span>
+</span><span id="L-129"><a href="#L-129"><span class="linenos">129</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">branch</span><span class="p">(</span><span class="s2">&quot;-vva&quot;</span><span class="p">)</span>
 </span><span id="L-130"><a href="#L-130"><span class="linenos">130</span></a>
-</span><span id="L-131"><a href="#L-131"><span class="linenos">131</span></a><span class="sd">        Equivalent to `git checkout {branch_name}`.&quot;&quot;&quot;</span>
-</span><span id="L-132"><a href="#L-132"><span class="linenos">132</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">checkout</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
-</span><span id="L-133"><a href="#L-133"><span class="linenos">133</span></a>
-</span><span id="L-134"><a href="#L-134"><span class="linenos">134</span></a>    <span class="k">def</span> <span class="nf">create_new_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="L-135"><a href="#L-135"><span class="linenos">135</span></a>        <span class="sd">&quot;&quot;&quot;Create and switch to a new branch named with `branch_name`.</span>
-</span><span id="L-136"><a href="#L-136"><span class="linenos">136</span></a>
-</span><span id="L-137"><a href="#L-137"><span class="linenos">137</span></a><span class="sd">        Equivalent to `git checkout -b {branch_name} --track`.&quot;&quot;&quot;</span>
-</span><span id="L-138"><a href="#L-138"><span class="linenos">138</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">checkout</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-b </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2"> --track&quot;</span><span class="p">)</span>
-</span><span id="L-139"><a href="#L-139"><span class="linenos">139</span></a>
-</span><span id="L-140"><a href="#L-140"><span class="linenos">140</span></a>    <span class="k">def</span> <span class="nf">delete_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">local_only</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="L-141"><a href="#L-141"><span class="linenos">141</span></a>        <span class="sd">&quot;&quot;&quot;Delete `branch_name` from repo.</span>
-</span><span id="L-142"><a href="#L-142"><span class="linenos">142</span></a>
-</span><span id="L-143"><a href="#L-143"><span class="linenos">143</span></a><span class="sd">        #### :params:</span>
-</span><span id="L-144"><a href="#L-144"><span class="linenos">144</span></a>
-</span><span id="L-145"><a href="#L-145"><span class="linenos">145</span></a><span class="sd">        `local_only`: Only delete the local copy of `branch`, otherwise also delete the remote branch on origin and remote-tracking branch.&quot;&quot;&quot;</span>
-</span><span id="L-146"><a href="#L-146"><span class="linenos">146</span></a>        <span class="n">output</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">branch</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;--delete </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-147"><a href="#L-147"><span class="linenos">147</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">local_only</span><span class="p">:</span>
-</span><span id="L-148"><a href="#L-148"><span class="linenos">148</span></a>            <span class="k">return</span> <span class="n">output</span> <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;origin --delete </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>  <span class="c1"># type:ignore</span>
-</span><span id="L-149"><a href="#L-149"><span class="linenos">149</span></a>        <span class="k">return</span> <span class="n">output</span>
-</span><span id="L-150"><a href="#L-150"><span class="linenos">150</span></a>
-</span><span id="L-151"><a href="#L-151"><span class="linenos">151</span></a>    <span class="k">def</span> <span class="nf">undo</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="L-152"><a href="#L-152"><span class="linenos">152</span></a>        <span class="sd">&quot;&quot;&quot;Undo uncommitted changes.</span>
-</span><span id="L-153"><a href="#L-153"><span class="linenos">153</span></a>
-</span><span id="L-154"><a href="#L-154"><span class="linenos">154</span></a><span class="sd">        Equivalent to `git checkout .`.&quot;&quot;&quot;</span>
-</span><span id="L-155"><a href="#L-155"><span class="linenos">155</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">checkout</span><span class="p">(</span><span class="s2">&quot;.&quot;</span><span class="p">)</span>
-</span><span id="L-156"><a href="#L-156"><span class="linenos">156</span></a>
-</span><span id="L-157"><a href="#L-157"><span class="linenos">157</span></a>    <span class="k">def</span> <span class="nf">merge</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="L-158"><a href="#L-158"><span class="linenos">158</span></a>        <span class="sd">&quot;&quot;&quot;Merge branch `branch_name` with currently active branch.&quot;&quot;&quot;</span>
-</span><span id="L-159"><a href="#L-159"><span class="linenos">159</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;merge </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-131"><a href="#L-131"><span class="linenos">131</span></a>    <span class="k">def</span> <span class="nf">checkout</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="L-132"><a href="#L-132"><span class="linenos">132</span></a>        <span class="sd">&quot;&quot;&quot;Equivalent to `git checkout {args}`.&quot;&quot;&quot;</span>
+</span><span id="L-133"><a href="#L-133"><span class="linenos">133</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;checkout </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-134"><a href="#L-134"><span class="linenos">134</span></a>
+</span><span id="L-135"><a href="#L-135"><span class="linenos">135</span></a>    <span class="k">def</span> <span class="nf">switch_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="L-136"><a href="#L-136"><span class="linenos">136</span></a>        <span class="sd">&quot;&quot;&quot;Switch to the branch specified by `branch_name`.</span>
+</span><span id="L-137"><a href="#L-137"><span class="linenos">137</span></a>
+</span><span id="L-138"><a href="#L-138"><span class="linenos">138</span></a><span class="sd">        Equivalent to `git checkout {branch_name}`.&quot;&quot;&quot;</span>
+</span><span id="L-139"><a href="#L-139"><span class="linenos">139</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">checkout</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
+</span><span id="L-140"><a href="#L-140"><span class="linenos">140</span></a>
+</span><span id="L-141"><a href="#L-141"><span class="linenos">141</span></a>    <span class="k">def</span> <span class="nf">create_new_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="L-142"><a href="#L-142"><span class="linenos">142</span></a>        <span class="sd">&quot;&quot;&quot;Create and switch to a new branch named with `branch_name`.</span>
+</span><span id="L-143"><a href="#L-143"><span class="linenos">143</span></a>
+</span><span id="L-144"><a href="#L-144"><span class="linenos">144</span></a><span class="sd">        Equivalent to `git checkout -b {branch_name} --track`.&quot;&quot;&quot;</span>
+</span><span id="L-145"><a href="#L-145"><span class="linenos">145</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">checkout</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-b </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2"> --track&quot;</span><span class="p">)</span>
+</span><span id="L-146"><a href="#L-146"><span class="linenos">146</span></a>
+</span><span id="L-147"><a href="#L-147"><span class="linenos">147</span></a>    <span class="k">def</span> <span class="nf">delete_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">local_only</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="L-148"><a href="#L-148"><span class="linenos">148</span></a>        <span class="sd">&quot;&quot;&quot;Delete `branch_name` from repo.</span>
+</span><span id="L-149"><a href="#L-149"><span class="linenos">149</span></a>
+</span><span id="L-150"><a href="#L-150"><span class="linenos">150</span></a><span class="sd">        #### :params:</span>
+</span><span id="L-151"><a href="#L-151"><span class="linenos">151</span></a>
+</span><span id="L-152"><a href="#L-152"><span class="linenos">152</span></a><span class="sd">        `local_only`: Only delete the local copy of `branch`, otherwise also delete the remote branch on origin and remote-tracking branch.&quot;&quot;&quot;</span>
+</span><span id="L-153"><a href="#L-153"><span class="linenos">153</span></a>        <span class="n">output</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">branch</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;--delete </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-154"><a href="#L-154"><span class="linenos">154</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">local_only</span><span class="p">:</span>
+</span><span id="L-155"><a href="#L-155"><span class="linenos">155</span></a>            <span class="k">return</span> <span class="n">output</span> <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;origin --delete </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>  <span class="c1"># type:ignore</span>
+</span><span id="L-156"><a href="#L-156"><span class="linenos">156</span></a>        <span class="k">return</span> <span class="n">output</span>
+</span><span id="L-157"><a href="#L-157"><span class="linenos">157</span></a>
+</span><span id="L-158"><a href="#L-158"><span class="linenos">158</span></a>    <span class="k">def</span> <span class="nf">undo</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="L-159"><a href="#L-159"><span class="linenos">159</span></a>        <span class="sd">&quot;&quot;&quot;Undo uncommitted changes.</span>
 </span><span id="L-160"><a href="#L-160"><span class="linenos">160</span></a>
-</span><span id="L-161"><a href="#L-161"><span class="linenos">161</span></a>    <span class="c1"># ===============================Requires GitHub CLI to be installed and configured===============================</span>
-</span><span id="L-162"><a href="#L-162"><span class="linenos">162</span></a>
-</span><span id="L-163"><a href="#L-163"><span class="linenos">163</span></a>    <span class="k">def</span> <span class="nf">create_remote</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">public</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="L-164"><a href="#L-164"><span class="linenos">164</span></a>        <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be installed and configured) to create a remote GitHub repo.</span>
-</span><span id="L-165"><a href="#L-165"><span class="linenos">165</span></a>
-</span><span id="L-166"><a href="#L-166"><span class="linenos">166</span></a><span class="sd">        #### :params:</span>
+</span><span id="L-161"><a href="#L-161"><span class="linenos">161</span></a><span class="sd">        Equivalent to `git checkout .`.&quot;&quot;&quot;</span>
+</span><span id="L-162"><a href="#L-162"><span class="linenos">162</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">checkout</span><span class="p">(</span><span class="s2">&quot;.&quot;</span><span class="p">)</span>
+</span><span id="L-163"><a href="#L-163"><span class="linenos">163</span></a>
+</span><span id="L-164"><a href="#L-164"><span class="linenos">164</span></a>    <span class="k">def</span> <span class="nf">merge</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="L-165"><a href="#L-165"><span class="linenos">165</span></a>        <span class="sd">&quot;&quot;&quot;Merge branch `branch_name` with currently active branch.&quot;&quot;&quot;</span>
+</span><span id="L-166"><a href="#L-166"><span class="linenos">166</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;merge </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span><span id="L-167"><a href="#L-167"><span class="linenos">167</span></a>
-</span><span id="L-168"><a href="#L-168"><span class="linenos">168</span></a><span class="sd">        `name`: The name for the repo.</span>
+</span><span id="L-168"><a href="#L-168"><span class="linenos">168</span></a>    <span class="c1"># ===============================Requires GitHub CLI to be installed and configured===============================</span>
 </span><span id="L-169"><a href="#L-169"><span class="linenos">169</span></a>
-</span><span id="L-170"><a href="#L-170"><span class="linenos">170</span></a><span class="sd">        `public`: Set to `True` to create the repo as public, otherwise it&#39;ll be created as private.&quot;&quot;&quot;</span>
-</span><span id="L-171"><a href="#L-171"><span class="linenos">171</span></a>        <span class="n">visibility</span> <span class="o">=</span> <span class="s2">&quot;--public&quot;</span> <span class="k">if</span> <span class="n">public</span> <span class="k">else</span> <span class="s2">&quot;--private&quot;</span>
-</span><span id="L-172"><a href="#L-172"><span class="linenos">172</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">([</span><span class="s2">&quot;gh&quot;</span><span class="p">,</span> <span class="s2">&quot;repo&quot;</span><span class="p">,</span> <span class="s2">&quot;create&quot;</span><span class="p">,</span> <span class="n">name</span><span class="p">,</span> <span class="n">visibility</span><span class="p">])</span>
-</span><span id="L-173"><a href="#L-173"><span class="linenos">173</span></a>
-</span><span id="L-174"><a href="#L-174"><span class="linenos">174</span></a>    <span class="k">def</span> <span class="nf">create_remote_from_cwd</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">public</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="L-175"><a href="#L-175"><span class="linenos">175</span></a>        <span class="sd">&quot;&quot;&quot;Use GitHub CLI (must be installed and configured) to create a remote GitHub repo from</span>
-</span><span id="L-176"><a href="#L-176"><span class="linenos">176</span></a><span class="sd">        the current working directory repo and add its url as this repo&#39;s remote origin.</span>
-</span><span id="L-177"><a href="#L-177"><span class="linenos">177</span></a>
-</span><span id="L-178"><a href="#L-178"><span class="linenos">178</span></a><span class="sd">        #### :params:</span>
-</span><span id="L-179"><a href="#L-179"><span class="linenos">179</span></a>
-</span><span id="L-180"><a href="#L-180"><span class="linenos">180</span></a><span class="sd">        `public`: Create the GitHub repo as a public repo, default is to create it as private.&quot;&quot;&quot;</span>
-</span><span id="L-181"><a href="#L-181"><span class="linenos">181</span></a>        <span class="n">visibility</span> <span class="o">=</span> <span class="s2">&quot;public&quot;</span> <span class="k">if</span> <span class="n">public</span> <span class="k">else</span> <span class="s2">&quot;private&quot;</span>
-</span><span id="L-182"><a href="#L-182"><span class="linenos">182</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">(</span>
-</span><span id="L-183"><a href="#L-183"><span class="linenos">183</span></a>            <span class="p">[</span><span class="s2">&quot;gh&quot;</span><span class="p">,</span> <span class="s2">&quot;repo&quot;</span><span class="p">,</span> <span class="s2">&quot;create&quot;</span><span class="p">,</span> <span class="s2">&quot;--source&quot;</span><span class="p">,</span> <span class="s2">&quot;.&quot;</span><span class="p">,</span> <span class="sa">f</span><span class="s2">&quot;--</span><span class="si">{</span><span class="n">visibility</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">,</span> <span class="s2">&quot;--push&quot;</span><span class="p">]</span>
-</span><span id="L-184"><a href="#L-184"><span class="linenos">184</span></a>        <span class="p">)</span>
-</span><span id="L-185"><a href="#L-185"><span class="linenos">185</span></a>
-</span><span id="L-186"><a href="#L-186"><span class="linenos">186</span></a>    <span class="k">def</span> <span class="nf">_change_visibility</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">visibility</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="L-187"><a href="#L-187"><span class="linenos">187</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">(</span>
-</span><span id="L-188"><a href="#L-188"><span class="linenos">188</span></a>            <span class="p">[</span><span class="s2">&quot;gh&quot;</span><span class="p">,</span> <span class="s2">&quot;repo&quot;</span><span class="p">,</span> <span class="s2">&quot;edit&quot;</span><span class="p">,</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">owner</span><span class="si">}</span><span class="s2">/</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">,</span> <span class="s2">&quot;--visibility&quot;</span><span class="p">,</span> <span class="n">visibility</span><span class="p">]</span>
-</span><span id="L-189"><a href="#L-189"><span class="linenos">189</span></a>        <span class="p">)</span>
-</span><span id="L-190"><a href="#L-190"><span class="linenos">190</span></a>
-</span><span id="L-191"><a href="#L-191"><span class="linenos">191</span></a>    <span class="k">def</span> <span class="nf">make_private</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="L-192"><a href="#L-192"><span class="linenos">192</span></a>        <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be installed and configured) to set the repo&#39;s visibility to private.</span>
-</span><span id="L-193"><a href="#L-193"><span class="linenos">193</span></a>
-</span><span id="L-194"><a href="#L-194"><span class="linenos">194</span></a><span class="sd">        #### :params:</span>
-</span><span id="L-195"><a href="#L-195"><span class="linenos">195</span></a>
-</span><span id="L-196"><a href="#L-196"><span class="linenos">196</span></a><span class="sd">        `owner`: The repo owner.</span>
+</span><span id="L-170"><a href="#L-170"><span class="linenos">170</span></a>    <span class="k">def</span> <span class="nf">create_remote</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">public</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="L-171"><a href="#L-171"><span class="linenos">171</span></a>        <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be installed and configured) to create a remote GitHub repo.</span>
+</span><span id="L-172"><a href="#L-172"><span class="linenos">172</span></a>
+</span><span id="L-173"><a href="#L-173"><span class="linenos">173</span></a><span class="sd">        #### :params:</span>
+</span><span id="L-174"><a href="#L-174"><span class="linenos">174</span></a>
+</span><span id="L-175"><a href="#L-175"><span class="linenos">175</span></a><span class="sd">        `name`: The name for the repo.</span>
+</span><span id="L-176"><a href="#L-176"><span class="linenos">176</span></a>
+</span><span id="L-177"><a href="#L-177"><span class="linenos">177</span></a><span class="sd">        `public`: Set to `True` to create the repo as public, otherwise it&#39;ll be created as private.&quot;&quot;&quot;</span>
+</span><span id="L-178"><a href="#L-178"><span class="linenos">178</span></a>        <span class="n">visibility</span> <span class="o">=</span> <span class="s2">&quot;--public&quot;</span> <span class="k">if</span> <span class="n">public</span> <span class="k">else</span> <span class="s2">&quot;--private&quot;</span>
+</span><span id="L-179"><a href="#L-179"><span class="linenos">179</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">([</span><span class="s2">&quot;gh&quot;</span><span class="p">,</span> <span class="s2">&quot;repo&quot;</span><span class="p">,</span> <span class="s2">&quot;create&quot;</span><span class="p">,</span> <span class="n">name</span><span class="p">,</span> <span class="n">visibility</span><span class="p">])</span>
+</span><span id="L-180"><a href="#L-180"><span class="linenos">180</span></a>
+</span><span id="L-181"><a href="#L-181"><span class="linenos">181</span></a>    <span class="k">def</span> <span class="nf">create_remote_from_cwd</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">public</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="L-182"><a href="#L-182"><span class="linenos">182</span></a>        <span class="sd">&quot;&quot;&quot;Use GitHub CLI (must be installed and configured) to create a remote GitHub repo from</span>
+</span><span id="L-183"><a href="#L-183"><span class="linenos">183</span></a><span class="sd">        the current working directory repo and add its url as this repo&#39;s remote origin.</span>
+</span><span id="L-184"><a href="#L-184"><span class="linenos">184</span></a>
+</span><span id="L-185"><a href="#L-185"><span class="linenos">185</span></a><span class="sd">        #### :params:</span>
+</span><span id="L-186"><a href="#L-186"><span class="linenos">186</span></a>
+</span><span id="L-187"><a href="#L-187"><span class="linenos">187</span></a><span class="sd">        `public`: Create the GitHub repo as a public repo, default is to create it as private.&quot;&quot;&quot;</span>
+</span><span id="L-188"><a href="#L-188"><span class="linenos">188</span></a>        <span class="n">visibility</span> <span class="o">=</span> <span class="s2">&quot;public&quot;</span> <span class="k">if</span> <span class="n">public</span> <span class="k">else</span> <span class="s2">&quot;private&quot;</span>
+</span><span id="L-189"><a href="#L-189"><span class="linenos">189</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">(</span>
+</span><span id="L-190"><a href="#L-190"><span class="linenos">190</span></a>            <span class="p">[</span><span class="s2">&quot;gh&quot;</span><span class="p">,</span> <span class="s2">&quot;repo&quot;</span><span class="p">,</span> <span class="s2">&quot;create&quot;</span><span class="p">,</span> <span class="s2">&quot;--source&quot;</span><span class="p">,</span> <span class="s2">&quot;.&quot;</span><span class="p">,</span> <span class="sa">f</span><span class="s2">&quot;--</span><span class="si">{</span><span class="n">visibility</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">,</span> <span class="s2">&quot;--push&quot;</span><span class="p">]</span>
+</span><span id="L-191"><a href="#L-191"><span class="linenos">191</span></a>        <span class="p">)</span>
+</span><span id="L-192"><a href="#L-192"><span class="linenos">192</span></a>
+</span><span id="L-193"><a href="#L-193"><span class="linenos">193</span></a>    <span class="k">def</span> <span class="nf">_change_visibility</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">visibility</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="L-194"><a href="#L-194"><span class="linenos">194</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">(</span>
+</span><span id="L-195"><a href="#L-195"><span class="linenos">195</span></a>            <span class="p">[</span><span class="s2">&quot;gh&quot;</span><span class="p">,</span> <span class="s2">&quot;repo&quot;</span><span class="p">,</span> <span class="s2">&quot;edit&quot;</span><span class="p">,</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">owner</span><span class="si">}</span><span class="s2">/</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">,</span> <span class="s2">&quot;--visibility&quot;</span><span class="p">,</span> <span class="n">visibility</span><span class="p">]</span>
+</span><span id="L-196"><a href="#L-196"><span class="linenos">196</span></a>        <span class="p">)</span>
 </span><span id="L-197"><a href="#L-197"><span class="linenos">197</span></a>
-</span><span id="L-198"><a href="#L-198"><span class="linenos">198</span></a><span class="sd">        `name`: The name of the repo to edit.&quot;&quot;&quot;</span>
-</span><span id="L-199"><a href="#L-199"><span class="linenos">199</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_change_visibility</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">name</span><span class="p">,</span> <span class="s2">&quot;private&quot;</span><span class="p">)</span>
+</span><span id="L-198"><a href="#L-198"><span class="linenos">198</span></a>    <span class="k">def</span> <span class="nf">make_private</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="L-199"><a href="#L-199"><span class="linenos">199</span></a>        <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be installed and configured) to set the repo&#39;s visibility to private.</span>
 </span><span id="L-200"><a href="#L-200"><span class="linenos">200</span></a>
-</span><span id="L-201"><a href="#L-201"><span class="linenos">201</span></a>    <span class="k">def</span> <span class="nf">make_public</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="L-202"><a href="#L-202"><span class="linenos">202</span></a>        <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be installed and configured) to set the repo&#39;s visibility to public.</span>
-</span><span id="L-203"><a href="#L-203"><span class="linenos">203</span></a>
-</span><span id="L-204"><a href="#L-204"><span class="linenos">204</span></a><span class="sd">        #### :params:</span>
-</span><span id="L-205"><a href="#L-205"><span class="linenos">205</span></a>
-</span><span id="L-206"><a href="#L-206"><span class="linenos">206</span></a><span class="sd">        `owner`: The repo owner.</span>
+</span><span id="L-201"><a href="#L-201"><span class="linenos">201</span></a><span class="sd">        #### :params:</span>
+</span><span id="L-202"><a href="#L-202"><span class="linenos">202</span></a>
+</span><span id="L-203"><a href="#L-203"><span class="linenos">203</span></a><span class="sd">        `owner`: The repo owner.</span>
+</span><span id="L-204"><a href="#L-204"><span class="linenos">204</span></a>
+</span><span id="L-205"><a href="#L-205"><span class="linenos">205</span></a><span class="sd">        `name`: The name of the repo to edit.&quot;&quot;&quot;</span>
+</span><span id="L-206"><a href="#L-206"><span class="linenos">206</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_change_visibility</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">name</span><span class="p">,</span> <span class="s2">&quot;private&quot;</span><span class="p">)</span>
 </span><span id="L-207"><a href="#L-207"><span class="linenos">207</span></a>
-</span><span id="L-208"><a href="#L-208"><span class="linenos">208</span></a><span class="sd">        `name`: The name of the repo to edit.&quot;&quot;&quot;</span>
-</span><span id="L-209"><a href="#L-209"><span class="linenos">209</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_change_visibility</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">name</span><span class="p">,</span> <span class="s2">&quot;public&quot;</span><span class="p">)</span>
+</span><span id="L-208"><a href="#L-208"><span class="linenos">208</span></a>    <span class="k">def</span> <span class="nf">make_public</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="L-209"><a href="#L-209"><span class="linenos">209</span></a>        <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be installed and configured) to set the repo&#39;s visibility to public.</span>
 </span><span id="L-210"><a href="#L-210"><span class="linenos">210</span></a>
-</span><span id="L-211"><a href="#L-211"><span class="linenos">211</span></a>    <span class="k">def</span> <span class="nf">delete_remote</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="L-212"><a href="#L-212"><span class="linenos">212</span></a>        <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be isntalled and configured) to delete the remote for this repo.</span>
-</span><span id="L-213"><a href="#L-213"><span class="linenos">213</span></a>
-</span><span id="L-214"><a href="#L-214"><span class="linenos">214</span></a><span class="sd">        #### :params:</span>
-</span><span id="L-215"><a href="#L-215"><span class="linenos">215</span></a>
-</span><span id="L-216"><a href="#L-216"><span class="linenos">216</span></a><span class="sd">        `owner`: The repo owner.</span>
+</span><span id="L-211"><a href="#L-211"><span class="linenos">211</span></a><span class="sd">        #### :params:</span>
+</span><span id="L-212"><a href="#L-212"><span class="linenos">212</span></a>
+</span><span id="L-213"><a href="#L-213"><span class="linenos">213</span></a><span class="sd">        `owner`: The repo owner.</span>
+</span><span id="L-214"><a href="#L-214"><span class="linenos">214</span></a>
+</span><span id="L-215"><a href="#L-215"><span class="linenos">215</span></a><span class="sd">        `name`: The name of the repo to edit.&quot;&quot;&quot;</span>
+</span><span id="L-216"><a href="#L-216"><span class="linenos">216</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_change_visibility</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">name</span><span class="p">,</span> <span class="s2">&quot;public&quot;</span><span class="p">)</span>
 </span><span id="L-217"><a href="#L-217"><span class="linenos">217</span></a>
-</span><span id="L-218"><a href="#L-218"><span class="linenos">218</span></a><span class="sd">        `name`: The name of the remote repo to delete.&quot;&quot;&quot;</span>
-</span><span id="L-219"><a href="#L-219"><span class="linenos">219</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">([</span><span class="s2">&quot;gh&quot;</span><span class="p">,</span> <span class="s2">&quot;repo&quot;</span><span class="p">,</span> <span class="s2">&quot;delete&quot;</span><span class="p">,</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">owner</span><span class="si">}</span><span class="s2">/</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">,</span> <span class="s2">&quot;--yes&quot;</span><span class="p">])</span>
+</span><span id="L-218"><a href="#L-218"><span class="linenos">218</span></a>    <span class="k">def</span> <span class="nf">delete_remote</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="L-219"><a href="#L-219"><span class="linenos">219</span></a>        <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be isntalled and configured) to delete the remote for this repo.</span>
+</span><span id="L-220"><a href="#L-220"><span class="linenos">220</span></a>
+</span><span id="L-221"><a href="#L-221"><span class="linenos">221</span></a><span class="sd">        #### :params:</span>
+</span><span id="L-222"><a href="#L-222"><span class="linenos">222</span></a>
+</span><span id="L-223"><a href="#L-223"><span class="linenos">223</span></a><span class="sd">        `owner`: The repo owner.</span>
+</span><span id="L-224"><a href="#L-224"><span class="linenos">224</span></a>
+</span><span id="L-225"><a href="#L-225"><span class="linenos">225</span></a><span class="sd">        `name`: The name of the remote repo to delete.&quot;&quot;&quot;</span>
+</span><span id="L-226"><a href="#L-226"><span class="linenos">226</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">([</span><span class="s2">&quot;gh&quot;</span><span class="p">,</span> <span class="s2">&quot;repo&quot;</span><span class="p">,</span> <span class="s2">&quot;delete&quot;</span><span class="p">,</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">owner</span><span class="si">}</span><span class="s2">/</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">,</span> <span class="s2">&quot;--yes&quot;</span><span class="p">])</span>
 </span></pre></div>
 
 
             </section>
                 <section id="Git">
                             <input id="Git-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr class">
@@ -377,229 +387,235 @@
     <span class="def">class</span>
     <span class="name">Git</span>:
 
                 <label class="view-source-button" for="Git-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Git"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Git-6"><a href="#Git-6"><span class="linenos">  6</span></a><span class="k">class</span> <span class="nc">Git</span><span class="p">:</span>
-</span><span id="Git-7"><a href="#Git-7"><span class="linenos">  7</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">capture_stdout</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">):</span>
-</span><span id="Git-8"><a href="#Git-8"><span class="linenos">  8</span></a>        <span class="sd">&quot;&quot;&quot;If `capture_stdout` is `True`, all functions will return their generated `stdout` as a string.</span>
-</span><span id="Git-9"><a href="#Git-9"><span class="linenos">  9</span></a><span class="sd">        Otherwise, the functions return the call&#39;s exit code.&quot;&quot;&quot;</span>
-</span><span id="Git-10"><a href="#Git-10"><span class="linenos"> 10</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">capture_stdout</span> <span class="o">=</span> <span class="n">capture_stdout</span>
-</span><span id="Git-11"><a href="#Git-11"><span class="linenos"> 11</span></a>
-</span><span id="Git-12"><a href="#Git-12"><span class="linenos"> 12</span></a>    <span class="nd">@property</span>
-</span><span id="Git-13"><a href="#Git-13"><span class="linenos"> 13</span></a>    <span class="k">def</span> <span class="nf">capture_stdout</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="Git-14"><a href="#Git-14"><span class="linenos"> 14</span></a>        <span class="sd">&quot;&quot;&quot;If `True`, member functions will return the generated `stdout` as a string,</span>
-</span><span id="Git-15"><a href="#Git-15"><span class="linenos"> 15</span></a><span class="sd">        otherwise they return the command&#39;s exit code.&quot;&quot;&quot;</span>
-</span><span id="Git-16"><a href="#Git-16"><span class="linenos"> 16</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_capture_stdout</span>
-</span><span id="Git-17"><a href="#Git-17"><span class="linenos"> 17</span></a>
-</span><span id="Git-18"><a href="#Git-18"><span class="linenos"> 18</span></a>    <span class="nd">@capture_stdout</span><span class="o">.</span><span class="n">setter</span>
-</span><span id="Git-19"><a href="#Git-19"><span class="linenos"> 19</span></a>    <span class="k">def</span> <span class="nf">capture_stdout</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">should_capture</span><span class="p">:</span> <span class="nb">bool</span><span class="p">):</span>
-</span><span id="Git-20"><a href="#Git-20"><span class="linenos"> 20</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_capture_stdout</span> <span class="o">=</span> <span class="n">should_capture</span>
-</span><span id="Git-21"><a href="#Git-21"><span class="linenos"> 21</span></a>
-</span><span id="Git-22"><a href="#Git-22"><span class="linenos"> 22</span></a>    <span class="k">def</span> <span class="nf">_run</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git-23"><a href="#Git-23"><span class="linenos"> 23</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_capture_stdout</span><span class="p">:</span>
-</span><span id="Git-24"><a href="#Git-24"><span class="linenos"> 24</span></a>            <span class="k">return</span> <span class="n">subprocess</span><span class="o">.</span><span class="n">run</span><span class="p">(</span><span class="n">args</span><span class="p">,</span> <span class="n">stdout</span><span class="o">=</span><span class="n">subprocess</span><span class="o">.</span><span class="n">PIPE</span><span class="p">,</span> <span class="n">text</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span><span class="o">.</span><span class="n">stdout</span>
-</span><span id="Git-25"><a href="#Git-25"><span class="linenos"> 25</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="Git-26"><a href="#Git-26"><span class="linenos"> 26</span></a>            <span class="k">return</span> <span class="n">subprocess</span><span class="o">.</span><span class="n">run</span><span class="p">(</span><span class="n">args</span><span class="p">)</span><span class="o">.</span><span class="n">returncode</span>
-</span><span id="Git-27"><a href="#Git-27"><span class="linenos"> 27</span></a>
-</span><span id="Git-28"><a href="#Git-28"><span class="linenos"> 28</span></a>    <span class="k">def</span> <span class="nf">execute</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">command</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git-29"><a href="#Git-29"><span class="linenos"> 29</span></a>        <span class="sd">&quot;&quot;&quot;Execute git command.</span>
-</span><span id="Git-30"><a href="#Git-30"><span class="linenos"> 30</span></a>
-</span><span id="Git-31"><a href="#Git-31"><span class="linenos"> 31</span></a><span class="sd">        Equivalent to executing `git {command}` in the shell.&quot;&quot;&quot;</span>
-</span><span id="Git-32"><a href="#Git-32"><span class="linenos"> 32</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="p">[</span><span class="s2">&quot;git&quot;</span><span class="p">]</span> <span class="o">+</span> <span class="n">shlex</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="n">command</span><span class="p">)</span>
-</span><span id="Git-33"><a href="#Git-33"><span class="linenos"> 33</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Git-7"><a href="#Git-7"><span class="linenos">  7</span></a><span class="k">class</span> <span class="nc">Git</span><span class="p">:</span>
+</span><span id="Git-8"><a href="#Git-8"><span class="linenos">  8</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">capture_stdout</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">):</span>
+</span><span id="Git-9"><a href="#Git-9"><span class="linenos">  9</span></a>        <span class="sd">&quot;&quot;&quot;If `capture_stdout` is `True`, all functions will return their generated `stdout` as a string.</span>
+</span><span id="Git-10"><a href="#Git-10"><span class="linenos"> 10</span></a><span class="sd">        Otherwise, the functions return the call&#39;s exit code.&quot;&quot;&quot;</span>
+</span><span id="Git-11"><a href="#Git-11"><span class="linenos"> 11</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">capture_stdout</span> <span class="o">=</span> <span class="n">capture_stdout</span>
+</span><span id="Git-12"><a href="#Git-12"><span class="linenos"> 12</span></a>
+</span><span id="Git-13"><a href="#Git-13"><span class="linenos"> 13</span></a>    <span class="nd">@contextmanager</span>
+</span><span id="Git-14"><a href="#Git-14"><span class="linenos"> 14</span></a>    <span class="k">def</span> <span class="nf">capture_output</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="Git-15"><a href="#Git-15"><span class="linenos"> 15</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">capture_stdout</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="Git-16"><a href="#Git-16"><span class="linenos"> 16</span></a>        <span class="k">yield</span> <span class="bp">self</span>
+</span><span id="Git-17"><a href="#Git-17"><span class="linenos"> 17</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">capture_stdout</span> <span class="o">=</span> <span class="kc">False</span>
+</span><span id="Git-18"><a href="#Git-18"><span class="linenos"> 18</span></a>
+</span><span id="Git-19"><a href="#Git-19"><span class="linenos"> 19</span></a>    <span class="nd">@property</span>
+</span><span id="Git-20"><a href="#Git-20"><span class="linenos"> 20</span></a>    <span class="k">def</span> <span class="nf">capture_stdout</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="Git-21"><a href="#Git-21"><span class="linenos"> 21</span></a>        <span class="sd">&quot;&quot;&quot;If `True`, member functions will return the generated `stdout` as a string,</span>
+</span><span id="Git-22"><a href="#Git-22"><span class="linenos"> 22</span></a><span class="sd">        otherwise they return the command&#39;s exit code.&quot;&quot;&quot;</span>
+</span><span id="Git-23"><a href="#Git-23"><span class="linenos"> 23</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_capture_stdout</span>
+</span><span id="Git-24"><a href="#Git-24"><span class="linenos"> 24</span></a>
+</span><span id="Git-25"><a href="#Git-25"><span class="linenos"> 25</span></a>    <span class="nd">@capture_stdout</span><span class="o">.</span><span class="n">setter</span>
+</span><span id="Git-26"><a href="#Git-26"><span class="linenos"> 26</span></a>    <span class="k">def</span> <span class="nf">capture_stdout</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">should_capture</span><span class="p">:</span> <span class="nb">bool</span><span class="p">):</span>
+</span><span id="Git-27"><a href="#Git-27"><span class="linenos"> 27</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_capture_stdout</span> <span class="o">=</span> <span class="n">should_capture</span>
+</span><span id="Git-28"><a href="#Git-28"><span class="linenos"> 28</span></a>
+</span><span id="Git-29"><a href="#Git-29"><span class="linenos"> 29</span></a>    <span class="k">def</span> <span class="nf">_run</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git-30"><a href="#Git-30"><span class="linenos"> 30</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_capture_stdout</span><span class="p">:</span>
+</span><span id="Git-31"><a href="#Git-31"><span class="linenos"> 31</span></a>            <span class="k">return</span> <span class="n">subprocess</span><span class="o">.</span><span class="n">run</span><span class="p">(</span><span class="n">args</span><span class="p">,</span> <span class="n">stdout</span><span class="o">=</span><span class="n">subprocess</span><span class="o">.</span><span class="n">PIPE</span><span class="p">,</span> <span class="n">text</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span><span class="o">.</span><span class="n">stdout</span>
+</span><span id="Git-32"><a href="#Git-32"><span class="linenos"> 32</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="Git-33"><a href="#Git-33"><span class="linenos"> 33</span></a>            <span class="k">return</span> <span class="n">subprocess</span><span class="o">.</span><span class="n">run</span><span class="p">(</span><span class="n">args</span><span class="p">)</span><span class="o">.</span><span class="n">returncode</span>
 </span><span id="Git-34"><a href="#Git-34"><span class="linenos"> 34</span></a>
-</span><span id="Git-35"><a href="#Git-35"><span class="linenos"> 35</span></a>    <span class="k">def</span> <span class="nf">new_repo</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git-36"><a href="#Git-36"><span class="linenos"> 36</span></a>        <span class="sd">&quot;&quot;&quot;Executes `git init -b main`.&quot;&quot;&quot;</span>
-</span><span id="Git-37"><a href="#Git-37"><span class="linenos"> 37</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="s2">&quot;init -b main&quot;</span><span class="p">)</span>
-</span><span id="Git-38"><a href="#Git-38"><span class="linenos"> 38</span></a>
-</span><span id="Git-39"><a href="#Git-39"><span class="linenos"> 39</span></a>    <span class="k">def</span> <span class="nf">loggy</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git-40"><a href="#Git-40"><span class="linenos"> 40</span></a>        <span class="sd">&quot;&quot;&quot;Equivalent to `git log --oneline --name-only --abbrev-commit --graph`.&quot;&quot;&quot;</span>
-</span><span id="Git-41"><a href="#Git-41"><span class="linenos"> 41</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="s2">&quot;log --oneline --name-only --abbrev-commit --graph&quot;</span><span class="p">)</span>
-</span><span id="Git-42"><a href="#Git-42"><span class="linenos"> 42</span></a>
-</span><span id="Git-43"><a href="#Git-43"><span class="linenos"> 43</span></a>    <span class="k">def</span> <span class="nf">status</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git-44"><a href="#Git-44"><span class="linenos"> 44</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git status`.&quot;&quot;&quot;</span>
-</span><span id="Git-45"><a href="#Git-45"><span class="linenos"> 45</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="s2">&quot;status&quot;</span><span class="p">)</span>
-</span><span id="Git-46"><a href="#Git-46"><span class="linenos"> 46</span></a>
-</span><span id="Git-47"><a href="#Git-47"><span class="linenos"> 47</span></a>    <span class="c1"># ======================================Staging/Committing======================================</span>
-</span><span id="Git-48"><a href="#Git-48"><span class="linenos"> 48</span></a>    <span class="k">def</span> <span class="nf">commit</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git-49"><a href="#Git-49"><span class="linenos"> 49</span></a>        <span class="sd">&quot;&quot;&quot;&gt;&gt;&gt; git commit {args}&quot;&quot;&quot;</span>
-</span><span id="Git-50"><a href="#Git-50"><span class="linenos"> 50</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;commit </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="Git-51"><a href="#Git-51"><span class="linenos"> 51</span></a>
-</span><span id="Git-52"><a href="#Git-52"><span class="linenos"> 52</span></a>    <span class="k">def</span> <span class="nf">add</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">files</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git-53"><a href="#Git-53"><span class="linenos"> 53</span></a>        <span class="sd">&quot;&quot;&quot;Stage a list of files.</span>
-</span><span id="Git-54"><a href="#Git-54"><span class="linenos"> 54</span></a>
-</span><span id="Git-55"><a href="#Git-55"><span class="linenos"> 55</span></a><span class="sd">        If no files are given (`files=None`), all files will be staged.&quot;&quot;&quot;</span>
-</span><span id="Git-56"><a href="#Git-56"><span class="linenos"> 56</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">files</span><span class="p">:</span>
-</span><span id="Git-57"><a href="#Git-57"><span class="linenos"> 57</span></a>            <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="s2">&quot;add .&quot;</span><span class="p">)</span>
-</span><span id="Git-58"><a href="#Git-58"><span class="linenos"> 58</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="Git-59"><a href="#Git-59"><span class="linenos"> 59</span></a>            <span class="n">files</span> <span class="o">=</span> <span class="s2">&quot; &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;&quot;</span><span class="si">{</span><span class="n">file</span><span class="si">}</span><span class="s1">&quot;&#39;</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">files</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
-</span><span id="Git-60"><a href="#Git-60"><span class="linenos"> 60</span></a>            <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;add </span><span class="si">{</span><span class="n">files</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="Git-35"><a href="#Git-35"><span class="linenos"> 35</span></a>    <span class="k">def</span> <span class="nf">execute</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">command</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git-36"><a href="#Git-36"><span class="linenos"> 36</span></a>        <span class="sd">&quot;&quot;&quot;Execute git command.</span>
+</span><span id="Git-37"><a href="#Git-37"><span class="linenos"> 37</span></a>
+</span><span id="Git-38"><a href="#Git-38"><span class="linenos"> 38</span></a><span class="sd">        Equivalent to executing `git {command}` in the shell.&quot;&quot;&quot;</span>
+</span><span id="Git-39"><a href="#Git-39"><span class="linenos"> 39</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="p">[</span><span class="s2">&quot;git&quot;</span><span class="p">]</span> <span class="o">+</span> <span class="n">shlex</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="n">command</span><span class="p">)</span>
+</span><span id="Git-40"><a href="#Git-40"><span class="linenos"> 40</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
+</span><span id="Git-41"><a href="#Git-41"><span class="linenos"> 41</span></a>
+</span><span id="Git-42"><a href="#Git-42"><span class="linenos"> 42</span></a>    <span class="k">def</span> <span class="nf">new_repo</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git-43"><a href="#Git-43"><span class="linenos"> 43</span></a>        <span class="sd">&quot;&quot;&quot;Executes `git init -b main`.&quot;&quot;&quot;</span>
+</span><span id="Git-44"><a href="#Git-44"><span class="linenos"> 44</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="s2">&quot;init -b main&quot;</span><span class="p">)</span>
+</span><span id="Git-45"><a href="#Git-45"><span class="linenos"> 45</span></a>
+</span><span id="Git-46"><a href="#Git-46"><span class="linenos"> 46</span></a>    <span class="k">def</span> <span class="nf">loggy</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git-47"><a href="#Git-47"><span class="linenos"> 47</span></a>        <span class="sd">&quot;&quot;&quot;Equivalent to `git log --oneline --name-only --abbrev-commit --graph`.&quot;&quot;&quot;</span>
+</span><span id="Git-48"><a href="#Git-48"><span class="linenos"> 48</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="s2">&quot;log --oneline --name-only --abbrev-commit --graph&quot;</span><span class="p">)</span>
+</span><span id="Git-49"><a href="#Git-49"><span class="linenos"> 49</span></a>
+</span><span id="Git-50"><a href="#Git-50"><span class="linenos"> 50</span></a>    <span class="k">def</span> <span class="nf">status</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git-51"><a href="#Git-51"><span class="linenos"> 51</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git status`.&quot;&quot;&quot;</span>
+</span><span id="Git-52"><a href="#Git-52"><span class="linenos"> 52</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="s2">&quot;status&quot;</span><span class="p">)</span>
+</span><span id="Git-53"><a href="#Git-53"><span class="linenos"> 53</span></a>
+</span><span id="Git-54"><a href="#Git-54"><span class="linenos"> 54</span></a>    <span class="c1"># ======================================Staging/Committing======================================</span>
+</span><span id="Git-55"><a href="#Git-55"><span class="linenos"> 55</span></a>    <span class="k">def</span> <span class="nf">commit</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git-56"><a href="#Git-56"><span class="linenos"> 56</span></a>        <span class="sd">&quot;&quot;&quot;&gt;&gt;&gt; git commit {args}&quot;&quot;&quot;</span>
+</span><span id="Git-57"><a href="#Git-57"><span class="linenos"> 57</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;commit </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="Git-58"><a href="#Git-58"><span class="linenos"> 58</span></a>
+</span><span id="Git-59"><a href="#Git-59"><span class="linenos"> 59</span></a>    <span class="k">def</span> <span class="nf">add</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">files</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git-60"><a href="#Git-60"><span class="linenos"> 60</span></a>        <span class="sd">&quot;&quot;&quot;Stage a list of files.</span>
 </span><span id="Git-61"><a href="#Git-61"><span class="linenos"> 61</span></a>
-</span><span id="Git-62"><a href="#Git-62"><span class="linenos"> 62</span></a>    <span class="k">def</span> <span class="nf">commit_files</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">files</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">],</span> <span class="n">message</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git-63"><a href="#Git-63"><span class="linenos"> 63</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit a list of files with commit message `message`.&quot;&quot;&quot;</span>
-</span><span id="Git-64"><a href="#Git-64"><span class="linenos"> 64</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">add</span><span class="p">(</span><span class="n">files</span><span class="p">)</span> <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;-m &quot;</span><span class="si">{</span><span class="n">message</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
-</span><span id="Git-65"><a href="#Git-65"><span class="linenos"> 65</span></a>
-</span><span id="Git-66"><a href="#Git-66"><span class="linenos"> 66</span></a>    <span class="k">def</span> <span class="nf">initcommit</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git-67"><a href="#Git-67"><span class="linenos"> 67</span></a>        <span class="sd">&quot;&quot;&quot;Equivalent to</span>
-</span><span id="Git-68"><a href="#Git-68"><span class="linenos"> 68</span></a><span class="sd">        &gt;&gt;&gt; git add .</span>
-</span><span id="Git-69"><a href="#Git-69"><span class="linenos"> 69</span></a><span class="sd">        &gt;&gt;&gt; git commit -m &quot;Initial commit&quot; &quot;&quot;&quot;</span>
-</span><span id="Git-70"><a href="#Git-70"><span class="linenos"> 70</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">add</span><span class="p">()</span> <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="s1">&#39;-m &quot;Initial commit&quot;&#39;</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
-</span><span id="Git-71"><a href="#Git-71"><span class="linenos"> 71</span></a>
-</span><span id="Git-72"><a href="#Git-72"><span class="linenos"> 72</span></a>    <span class="k">def</span> <span class="nf">amend</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">files</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git-73"><a href="#Git-73"><span class="linenos"> 73</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit changes to the previous commit.</span>
-</span><span id="Git-74"><a href="#Git-74"><span class="linenos"> 74</span></a>
-</span><span id="Git-75"><a href="#Git-75"><span class="linenos"> 75</span></a><span class="sd">        If `files` is `None`, all files will be staged.</span>
-</span><span id="Git-76"><a href="#Git-76"><span class="linenos"> 76</span></a>
-</span><span id="Git-77"><a href="#Git-77"><span class="linenos"> 77</span></a><span class="sd">        Equivalent to:</span>
-</span><span id="Git-78"><a href="#Git-78"><span class="linenos"> 78</span></a><span class="sd">        &gt;&gt;&gt; git add {files}</span>
-</span><span id="Git-79"><a href="#Git-79"><span class="linenos"> 79</span></a><span class="sd">        &gt;&gt;&gt; git commit --amend --no-edit</span>
-</span><span id="Git-80"><a href="#Git-80"><span class="linenos"> 80</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="Git-81"><a href="#Git-81"><span class="linenos"> 81</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">add</span><span class="p">(</span><span class="n">files</span><span class="p">)</span> <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="s2">&quot;--amend --no-edit&quot;</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
-</span><span id="Git-82"><a href="#Git-82"><span class="linenos"> 82</span></a>
-</span><span id="Git-83"><a href="#Git-83"><span class="linenos"> 83</span></a>    <span class="k">def</span> <span class="nf">tag</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git-84"><a href="#Git-84"><span class="linenos"> 84</span></a>        <span class="sd">&quot;&quot;&quot;Execute the `tag` command with `args`.</span>
-</span><span id="Git-85"><a href="#Git-85"><span class="linenos"> 85</span></a>
-</span><span id="Git-86"><a href="#Git-86"><span class="linenos"> 86</span></a><span class="sd">        e.g.</span>
-</span><span id="Git-87"><a href="#Git-87"><span class="linenos"> 87</span></a>
-</span><span id="Git-88"><a href="#Git-88"><span class="linenos"> 88</span></a><span class="sd">        `self.tag(&quot;--sort=-committerdate&quot;)`</span>
+</span><span id="Git-62"><a href="#Git-62"><span class="linenos"> 62</span></a><span class="sd">        If no files are given (`files=None`), all files will be staged.&quot;&quot;&quot;</span>
+</span><span id="Git-63"><a href="#Git-63"><span class="linenos"> 63</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">files</span><span class="p">:</span>
+</span><span id="Git-64"><a href="#Git-64"><span class="linenos"> 64</span></a>            <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="s2">&quot;add .&quot;</span><span class="p">)</span>
+</span><span id="Git-65"><a href="#Git-65"><span class="linenos"> 65</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="Git-66"><a href="#Git-66"><span class="linenos"> 66</span></a>            <span class="n">files</span> <span class="o">=</span> <span class="s2">&quot; &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;&quot;</span><span class="si">{</span><span class="n">file</span><span class="si">}</span><span class="s1">&quot;&#39;</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">files</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
+</span><span id="Git-67"><a href="#Git-67"><span class="linenos"> 67</span></a>            <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;add </span><span class="si">{</span><span class="n">files</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="Git-68"><a href="#Git-68"><span class="linenos"> 68</span></a>
+</span><span id="Git-69"><a href="#Git-69"><span class="linenos"> 69</span></a>    <span class="k">def</span> <span class="nf">commit_files</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">files</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">],</span> <span class="n">message</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git-70"><a href="#Git-70"><span class="linenos"> 70</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit a list of files with commit message `message`.&quot;&quot;&quot;</span>
+</span><span id="Git-71"><a href="#Git-71"><span class="linenos"> 71</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">add</span><span class="p">(</span><span class="n">files</span><span class="p">)</span> <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;-m &quot;</span><span class="si">{</span><span class="n">message</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
+</span><span id="Git-72"><a href="#Git-72"><span class="linenos"> 72</span></a>
+</span><span id="Git-73"><a href="#Git-73"><span class="linenos"> 73</span></a>    <span class="k">def</span> <span class="nf">initcommit</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git-74"><a href="#Git-74"><span class="linenos"> 74</span></a>        <span class="sd">&quot;&quot;&quot;Equivalent to</span>
+</span><span id="Git-75"><a href="#Git-75"><span class="linenos"> 75</span></a><span class="sd">        &gt;&gt;&gt; git add .</span>
+</span><span id="Git-76"><a href="#Git-76"><span class="linenos"> 76</span></a><span class="sd">        &gt;&gt;&gt; git commit -m &quot;Initial commit&quot; &quot;&quot;&quot;</span>
+</span><span id="Git-77"><a href="#Git-77"><span class="linenos"> 77</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">add</span><span class="p">()</span> <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="s1">&#39;-m &quot;Initial commit&quot;&#39;</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
+</span><span id="Git-78"><a href="#Git-78"><span class="linenos"> 78</span></a>
+</span><span id="Git-79"><a href="#Git-79"><span class="linenos"> 79</span></a>    <span class="k">def</span> <span class="nf">amend</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">files</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git-80"><a href="#Git-80"><span class="linenos"> 80</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit changes to the previous commit.</span>
+</span><span id="Git-81"><a href="#Git-81"><span class="linenos"> 81</span></a>
+</span><span id="Git-82"><a href="#Git-82"><span class="linenos"> 82</span></a><span class="sd">        If `files` is `None`, all files will be staged.</span>
+</span><span id="Git-83"><a href="#Git-83"><span class="linenos"> 83</span></a>
+</span><span id="Git-84"><a href="#Git-84"><span class="linenos"> 84</span></a><span class="sd">        Equivalent to:</span>
+</span><span id="Git-85"><a href="#Git-85"><span class="linenos"> 85</span></a><span class="sd">        &gt;&gt;&gt; git add {files}</span>
+</span><span id="Git-86"><a href="#Git-86"><span class="linenos"> 86</span></a><span class="sd">        &gt;&gt;&gt; git commit --amend --no-edit</span>
+</span><span id="Git-87"><a href="#Git-87"><span class="linenos"> 87</span></a><span class="sd">        &quot;&quot;&quot;</span>
+</span><span id="Git-88"><a href="#Git-88"><span class="linenos"> 88</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">add</span><span class="p">(</span><span class="n">files</span><span class="p">)</span> <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="s2">&quot;--amend --no-edit&quot;</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
 </span><span id="Git-89"><a href="#Git-89"><span class="linenos"> 89</span></a>
-</span><span id="Git-90"><a href="#Git-90"><span class="linenos"> 90</span></a><span class="sd">        will list all the tags for this repository in descending commit date.&quot;&quot;&quot;</span>
-</span><span id="Git-91"><a href="#Git-91"><span class="linenos"> 91</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;tag </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="Git-90"><a href="#Git-90"><span class="linenos"> 90</span></a>    <span class="k">def</span> <span class="nf">tag</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git-91"><a href="#Git-91"><span class="linenos"> 91</span></a>        <span class="sd">&quot;&quot;&quot;Execute the `tag` command with `args`.</span>
 </span><span id="Git-92"><a href="#Git-92"><span class="linenos"> 92</span></a>
-</span><span id="Git-93"><a href="#Git-93"><span class="linenos"> 93</span></a>    <span class="c1"># ==========================================Push/Pull==========================================</span>
-</span><span id="Git-94"><a href="#Git-94"><span class="linenos"> 94</span></a>    <span class="k">def</span> <span class="nf">add_remote_url</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">url</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;origin&quot;</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git-95"><a href="#Git-95"><span class="linenos"> 95</span></a>        <span class="sd">&quot;&quot;&quot;Add remote url to repo.&quot;&quot;&quot;</span>
-</span><span id="Git-96"><a href="#Git-96"><span class="linenos"> 96</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;remote add </span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">url</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="Git-97"><a href="#Git-97"><span class="linenos"> 97</span></a>
-</span><span id="Git-98"><a href="#Git-98"><span class="linenos"> 98</span></a>    <span class="k">def</span> <span class="nf">push</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git-99"><a href="#Git-99"><span class="linenos"> 99</span></a>        <span class="sd">&quot;&quot;&quot;Equivalent to `git push {args}`.&quot;&quot;&quot;</span>
-</span><span id="Git-100"><a href="#Git-100"><span class="linenos">100</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;push </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="Git-101"><a href="#Git-101"><span class="linenos">101</span></a>
-</span><span id="Git-102"><a href="#Git-102"><span class="linenos">102</span></a>    <span class="k">def</span> <span class="nf">pull</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git-103"><a href="#Git-103"><span class="linenos">103</span></a>        <span class="sd">&quot;&quot;&quot;Equivalent to `git pull {args}`.&quot;&quot;&quot;</span>
-</span><span id="Git-104"><a href="#Git-104"><span class="linenos">104</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;pull </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="Git-105"><a href="#Git-105"><span class="linenos">105</span></a>
-</span><span id="Git-106"><a href="#Git-106"><span class="linenos">106</span></a>    <span class="k">def</span> <span class="nf">push_new_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git-107"><a href="#Git-107"><span class="linenos">107</span></a>        <span class="sd">&quot;&quot;&quot;Push a new branch to origin with tracking.</span>
+</span><span id="Git-93"><a href="#Git-93"><span class="linenos"> 93</span></a><span class="sd">        e.g.</span>
+</span><span id="Git-94"><a href="#Git-94"><span class="linenos"> 94</span></a>
+</span><span id="Git-95"><a href="#Git-95"><span class="linenos"> 95</span></a><span class="sd">        `self.tag(&quot;--sort=-committerdate&quot;)`</span>
+</span><span id="Git-96"><a href="#Git-96"><span class="linenos"> 96</span></a>
+</span><span id="Git-97"><a href="#Git-97"><span class="linenos"> 97</span></a><span class="sd">        will list all the tags for this repository in descending commit date.&quot;&quot;&quot;</span>
+</span><span id="Git-98"><a href="#Git-98"><span class="linenos"> 98</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;tag </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="Git-99"><a href="#Git-99"><span class="linenos"> 99</span></a>
+</span><span id="Git-100"><a href="#Git-100"><span class="linenos">100</span></a>    <span class="c1"># ==========================================Push/Pull==========================================</span>
+</span><span id="Git-101"><a href="#Git-101"><span class="linenos">101</span></a>    <span class="k">def</span> <span class="nf">add_remote_url</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">url</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;origin&quot;</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git-102"><a href="#Git-102"><span class="linenos">102</span></a>        <span class="sd">&quot;&quot;&quot;Add remote url to repo.&quot;&quot;&quot;</span>
+</span><span id="Git-103"><a href="#Git-103"><span class="linenos">103</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;remote add </span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">url</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="Git-104"><a href="#Git-104"><span class="linenos">104</span></a>
+</span><span id="Git-105"><a href="#Git-105"><span class="linenos">105</span></a>    <span class="k">def</span> <span class="nf">push</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git-106"><a href="#Git-106"><span class="linenos">106</span></a>        <span class="sd">&quot;&quot;&quot;Equivalent to `git push {args}`.&quot;&quot;&quot;</span>
+</span><span id="Git-107"><a href="#Git-107"><span class="linenos">107</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;push </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span><span id="Git-108"><a href="#Git-108"><span class="linenos">108</span></a>
-</span><span id="Git-109"><a href="#Git-109"><span class="linenos">109</span></a><span class="sd">        Equivalent to `git push -u origin {branch}`.&quot;&quot;&quot;</span>
-</span><span id="Git-110"><a href="#Git-110"><span class="linenos">110</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-u origin </span><span class="si">{</span><span class="n">branch</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="Git-111"><a href="#Git-111"><span class="linenos">111</span></a>
-</span><span id="Git-112"><a href="#Git-112"><span class="linenos">112</span></a>    <span class="k">def</span> <span class="nf">pull_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git-113"><a href="#Git-113"><span class="linenos">113</span></a>        <span class="sd">&quot;&quot;&quot;Pull `branch` from origin.&quot;&quot;&quot;</span>
-</span><span id="Git-114"><a href="#Git-114"><span class="linenos">114</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">pull</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;origin </span><span class="si">{</span><span class="n">branch</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="Git-109"><a href="#Git-109"><span class="linenos">109</span></a>    <span class="k">def</span> <span class="nf">pull</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git-110"><a href="#Git-110"><span class="linenos">110</span></a>        <span class="sd">&quot;&quot;&quot;Equivalent to `git pull {args}`.&quot;&quot;&quot;</span>
+</span><span id="Git-111"><a href="#Git-111"><span class="linenos">111</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;pull </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="Git-112"><a href="#Git-112"><span class="linenos">112</span></a>
+</span><span id="Git-113"><a href="#Git-113"><span class="linenos">113</span></a>    <span class="k">def</span> <span class="nf">push_new_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git-114"><a href="#Git-114"><span class="linenos">114</span></a>        <span class="sd">&quot;&quot;&quot;Push a new branch to origin with tracking.</span>
 </span><span id="Git-115"><a href="#Git-115"><span class="linenos">115</span></a>
-</span><span id="Git-116"><a href="#Git-116"><span class="linenos">116</span></a>    <span class="c1"># ============================================Checkout/Branches============================================</span>
-</span><span id="Git-117"><a href="#Git-117"><span class="linenos">117</span></a>    <span class="k">def</span> <span class="nf">branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git-118"><a href="#Git-118"><span class="linenos">118</span></a>        <span class="sd">&quot;&quot;&quot;Equivalent to `git branch {args}`.&quot;&quot;&quot;</span>
-</span><span id="Git-119"><a href="#Git-119"><span class="linenos">119</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;branch </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="Git-120"><a href="#Git-120"><span class="linenos">120</span></a>
-</span><span id="Git-121"><a href="#Git-121"><span class="linenos">121</span></a>    <span class="k">def</span> <span class="nf">list_branches</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git-122"><a href="#Git-122"><span class="linenos">122</span></a>        <span class="sd">&quot;&quot;&quot;Print a list of branches.&quot;&quot;&quot;</span>
-</span><span id="Git-123"><a href="#Git-123"><span class="linenos">123</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">branch</span><span class="p">(</span><span class="s2">&quot;-vva&quot;</span><span class="p">)</span>
-</span><span id="Git-124"><a href="#Git-124"><span class="linenos">124</span></a>
-</span><span id="Git-125"><a href="#Git-125"><span class="linenos">125</span></a>    <span class="k">def</span> <span class="nf">checkout</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git-126"><a href="#Git-126"><span class="linenos">126</span></a>        <span class="sd">&quot;&quot;&quot;Equivalent to `git checkout {args}`.&quot;&quot;&quot;</span>
-</span><span id="Git-127"><a href="#Git-127"><span class="linenos">127</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;checkout </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="Git-128"><a href="#Git-128"><span class="linenos">128</span></a>
-</span><span id="Git-129"><a href="#Git-129"><span class="linenos">129</span></a>    <span class="k">def</span> <span class="nf">switch_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git-130"><a href="#Git-130"><span class="linenos">130</span></a>        <span class="sd">&quot;&quot;&quot;Switch to the branch specified by `branch_name`.</span>
+</span><span id="Git-116"><a href="#Git-116"><span class="linenos">116</span></a><span class="sd">        Equivalent to `git push -u origin {branch}`.&quot;&quot;&quot;</span>
+</span><span id="Git-117"><a href="#Git-117"><span class="linenos">117</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-u origin </span><span class="si">{</span><span class="n">branch</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="Git-118"><a href="#Git-118"><span class="linenos">118</span></a>
+</span><span id="Git-119"><a href="#Git-119"><span class="linenos">119</span></a>    <span class="k">def</span> <span class="nf">pull_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git-120"><a href="#Git-120"><span class="linenos">120</span></a>        <span class="sd">&quot;&quot;&quot;Pull `branch` from origin.&quot;&quot;&quot;</span>
+</span><span id="Git-121"><a href="#Git-121"><span class="linenos">121</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">pull</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;origin </span><span class="si">{</span><span class="n">branch</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="Git-122"><a href="#Git-122"><span class="linenos">122</span></a>
+</span><span id="Git-123"><a href="#Git-123"><span class="linenos">123</span></a>    <span class="c1"># ============================================Checkout/Branches============================================</span>
+</span><span id="Git-124"><a href="#Git-124"><span class="linenos">124</span></a>    <span class="k">def</span> <span class="nf">branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git-125"><a href="#Git-125"><span class="linenos">125</span></a>        <span class="sd">&quot;&quot;&quot;Equivalent to `git branch {args}`.&quot;&quot;&quot;</span>
+</span><span id="Git-126"><a href="#Git-126"><span class="linenos">126</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;branch </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="Git-127"><a href="#Git-127"><span class="linenos">127</span></a>
+</span><span id="Git-128"><a href="#Git-128"><span class="linenos">128</span></a>    <span class="k">def</span> <span class="nf">list_branches</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git-129"><a href="#Git-129"><span class="linenos">129</span></a>        <span class="sd">&quot;&quot;&quot;Print a list of branches.&quot;&quot;&quot;</span>
+</span><span id="Git-130"><a href="#Git-130"><span class="linenos">130</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">branch</span><span class="p">(</span><span class="s2">&quot;-vva&quot;</span><span class="p">)</span>
 </span><span id="Git-131"><a href="#Git-131"><span class="linenos">131</span></a>
-</span><span id="Git-132"><a href="#Git-132"><span class="linenos">132</span></a><span class="sd">        Equivalent to `git checkout {branch_name}`.&quot;&quot;&quot;</span>
-</span><span id="Git-133"><a href="#Git-133"><span class="linenos">133</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">checkout</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
-</span><span id="Git-134"><a href="#Git-134"><span class="linenos">134</span></a>
-</span><span id="Git-135"><a href="#Git-135"><span class="linenos">135</span></a>    <span class="k">def</span> <span class="nf">create_new_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git-136"><a href="#Git-136"><span class="linenos">136</span></a>        <span class="sd">&quot;&quot;&quot;Create and switch to a new branch named with `branch_name`.</span>
-</span><span id="Git-137"><a href="#Git-137"><span class="linenos">137</span></a>
-</span><span id="Git-138"><a href="#Git-138"><span class="linenos">138</span></a><span class="sd">        Equivalent to `git checkout -b {branch_name} --track`.&quot;&quot;&quot;</span>
-</span><span id="Git-139"><a href="#Git-139"><span class="linenos">139</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">checkout</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-b </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2"> --track&quot;</span><span class="p">)</span>
-</span><span id="Git-140"><a href="#Git-140"><span class="linenos">140</span></a>
-</span><span id="Git-141"><a href="#Git-141"><span class="linenos">141</span></a>    <span class="k">def</span> <span class="nf">delete_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">local_only</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git-142"><a href="#Git-142"><span class="linenos">142</span></a>        <span class="sd">&quot;&quot;&quot;Delete `branch_name` from repo.</span>
-</span><span id="Git-143"><a href="#Git-143"><span class="linenos">143</span></a>
-</span><span id="Git-144"><a href="#Git-144"><span class="linenos">144</span></a><span class="sd">        #### :params:</span>
-</span><span id="Git-145"><a href="#Git-145"><span class="linenos">145</span></a>
-</span><span id="Git-146"><a href="#Git-146"><span class="linenos">146</span></a><span class="sd">        `local_only`: Only delete the local copy of `branch`, otherwise also delete the remote branch on origin and remote-tracking branch.&quot;&quot;&quot;</span>
-</span><span id="Git-147"><a href="#Git-147"><span class="linenos">147</span></a>        <span class="n">output</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">branch</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;--delete </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="Git-148"><a href="#Git-148"><span class="linenos">148</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">local_only</span><span class="p">:</span>
-</span><span id="Git-149"><a href="#Git-149"><span class="linenos">149</span></a>            <span class="k">return</span> <span class="n">output</span> <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;origin --delete </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>  <span class="c1"># type:ignore</span>
-</span><span id="Git-150"><a href="#Git-150"><span class="linenos">150</span></a>        <span class="k">return</span> <span class="n">output</span>
-</span><span id="Git-151"><a href="#Git-151"><span class="linenos">151</span></a>
-</span><span id="Git-152"><a href="#Git-152"><span class="linenos">152</span></a>    <span class="k">def</span> <span class="nf">undo</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git-153"><a href="#Git-153"><span class="linenos">153</span></a>        <span class="sd">&quot;&quot;&quot;Undo uncommitted changes.</span>
-</span><span id="Git-154"><a href="#Git-154"><span class="linenos">154</span></a>
-</span><span id="Git-155"><a href="#Git-155"><span class="linenos">155</span></a><span class="sd">        Equivalent to `git checkout .`.&quot;&quot;&quot;</span>
-</span><span id="Git-156"><a href="#Git-156"><span class="linenos">156</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">checkout</span><span class="p">(</span><span class="s2">&quot;.&quot;</span><span class="p">)</span>
-</span><span id="Git-157"><a href="#Git-157"><span class="linenos">157</span></a>
-</span><span id="Git-158"><a href="#Git-158"><span class="linenos">158</span></a>    <span class="k">def</span> <span class="nf">merge</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git-159"><a href="#Git-159"><span class="linenos">159</span></a>        <span class="sd">&quot;&quot;&quot;Merge branch `branch_name` with currently active branch.&quot;&quot;&quot;</span>
-</span><span id="Git-160"><a href="#Git-160"><span class="linenos">160</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;merge </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="Git-132"><a href="#Git-132"><span class="linenos">132</span></a>    <span class="k">def</span> <span class="nf">checkout</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git-133"><a href="#Git-133"><span class="linenos">133</span></a>        <span class="sd">&quot;&quot;&quot;Equivalent to `git checkout {args}`.&quot;&quot;&quot;</span>
+</span><span id="Git-134"><a href="#Git-134"><span class="linenos">134</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;checkout </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="Git-135"><a href="#Git-135"><span class="linenos">135</span></a>
+</span><span id="Git-136"><a href="#Git-136"><span class="linenos">136</span></a>    <span class="k">def</span> <span class="nf">switch_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git-137"><a href="#Git-137"><span class="linenos">137</span></a>        <span class="sd">&quot;&quot;&quot;Switch to the branch specified by `branch_name`.</span>
+</span><span id="Git-138"><a href="#Git-138"><span class="linenos">138</span></a>
+</span><span id="Git-139"><a href="#Git-139"><span class="linenos">139</span></a><span class="sd">        Equivalent to `git checkout {branch_name}`.&quot;&quot;&quot;</span>
+</span><span id="Git-140"><a href="#Git-140"><span class="linenos">140</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">checkout</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
+</span><span id="Git-141"><a href="#Git-141"><span class="linenos">141</span></a>
+</span><span id="Git-142"><a href="#Git-142"><span class="linenos">142</span></a>    <span class="k">def</span> <span class="nf">create_new_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git-143"><a href="#Git-143"><span class="linenos">143</span></a>        <span class="sd">&quot;&quot;&quot;Create and switch to a new branch named with `branch_name`.</span>
+</span><span id="Git-144"><a href="#Git-144"><span class="linenos">144</span></a>
+</span><span id="Git-145"><a href="#Git-145"><span class="linenos">145</span></a><span class="sd">        Equivalent to `git checkout -b {branch_name} --track`.&quot;&quot;&quot;</span>
+</span><span id="Git-146"><a href="#Git-146"><span class="linenos">146</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">checkout</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-b </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2"> --track&quot;</span><span class="p">)</span>
+</span><span id="Git-147"><a href="#Git-147"><span class="linenos">147</span></a>
+</span><span id="Git-148"><a href="#Git-148"><span class="linenos">148</span></a>    <span class="k">def</span> <span class="nf">delete_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">local_only</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git-149"><a href="#Git-149"><span class="linenos">149</span></a>        <span class="sd">&quot;&quot;&quot;Delete `branch_name` from repo.</span>
+</span><span id="Git-150"><a href="#Git-150"><span class="linenos">150</span></a>
+</span><span id="Git-151"><a href="#Git-151"><span class="linenos">151</span></a><span class="sd">        #### :params:</span>
+</span><span id="Git-152"><a href="#Git-152"><span class="linenos">152</span></a>
+</span><span id="Git-153"><a href="#Git-153"><span class="linenos">153</span></a><span class="sd">        `local_only`: Only delete the local copy of `branch`, otherwise also delete the remote branch on origin and remote-tracking branch.&quot;&quot;&quot;</span>
+</span><span id="Git-154"><a href="#Git-154"><span class="linenos">154</span></a>        <span class="n">output</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">branch</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;--delete </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="Git-155"><a href="#Git-155"><span class="linenos">155</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">local_only</span><span class="p">:</span>
+</span><span id="Git-156"><a href="#Git-156"><span class="linenos">156</span></a>            <span class="k">return</span> <span class="n">output</span> <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;origin --delete </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>  <span class="c1"># type:ignore</span>
+</span><span id="Git-157"><a href="#Git-157"><span class="linenos">157</span></a>        <span class="k">return</span> <span class="n">output</span>
+</span><span id="Git-158"><a href="#Git-158"><span class="linenos">158</span></a>
+</span><span id="Git-159"><a href="#Git-159"><span class="linenos">159</span></a>    <span class="k">def</span> <span class="nf">undo</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git-160"><a href="#Git-160"><span class="linenos">160</span></a>        <span class="sd">&quot;&quot;&quot;Undo uncommitted changes.</span>
 </span><span id="Git-161"><a href="#Git-161"><span class="linenos">161</span></a>
-</span><span id="Git-162"><a href="#Git-162"><span class="linenos">162</span></a>    <span class="c1"># ===============================Requires GitHub CLI to be installed and configured===============================</span>
-</span><span id="Git-163"><a href="#Git-163"><span class="linenos">163</span></a>
-</span><span id="Git-164"><a href="#Git-164"><span class="linenos">164</span></a>    <span class="k">def</span> <span class="nf">create_remote</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">public</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git-165"><a href="#Git-165"><span class="linenos">165</span></a>        <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be installed and configured) to create a remote GitHub repo.</span>
-</span><span id="Git-166"><a href="#Git-166"><span class="linenos">166</span></a>
-</span><span id="Git-167"><a href="#Git-167"><span class="linenos">167</span></a><span class="sd">        #### :params:</span>
+</span><span id="Git-162"><a href="#Git-162"><span class="linenos">162</span></a><span class="sd">        Equivalent to `git checkout .`.&quot;&quot;&quot;</span>
+</span><span id="Git-163"><a href="#Git-163"><span class="linenos">163</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">checkout</span><span class="p">(</span><span class="s2">&quot;.&quot;</span><span class="p">)</span>
+</span><span id="Git-164"><a href="#Git-164"><span class="linenos">164</span></a>
+</span><span id="Git-165"><a href="#Git-165"><span class="linenos">165</span></a>    <span class="k">def</span> <span class="nf">merge</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git-166"><a href="#Git-166"><span class="linenos">166</span></a>        <span class="sd">&quot;&quot;&quot;Merge branch `branch_name` with currently active branch.&quot;&quot;&quot;</span>
+</span><span id="Git-167"><a href="#Git-167"><span class="linenos">167</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;merge </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span><span id="Git-168"><a href="#Git-168"><span class="linenos">168</span></a>
-</span><span id="Git-169"><a href="#Git-169"><span class="linenos">169</span></a><span class="sd">        `name`: The name for the repo.</span>
+</span><span id="Git-169"><a href="#Git-169"><span class="linenos">169</span></a>    <span class="c1"># ===============================Requires GitHub CLI to be installed and configured===============================</span>
 </span><span id="Git-170"><a href="#Git-170"><span class="linenos">170</span></a>
-</span><span id="Git-171"><a href="#Git-171"><span class="linenos">171</span></a><span class="sd">        `public`: Set to `True` to create the repo as public, otherwise it&#39;ll be created as private.&quot;&quot;&quot;</span>
-</span><span id="Git-172"><a href="#Git-172"><span class="linenos">172</span></a>        <span class="n">visibility</span> <span class="o">=</span> <span class="s2">&quot;--public&quot;</span> <span class="k">if</span> <span class="n">public</span> <span class="k">else</span> <span class="s2">&quot;--private&quot;</span>
-</span><span id="Git-173"><a href="#Git-173"><span class="linenos">173</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">([</span><span class="s2">&quot;gh&quot;</span><span class="p">,</span> <span class="s2">&quot;repo&quot;</span><span class="p">,</span> <span class="s2">&quot;create&quot;</span><span class="p">,</span> <span class="n">name</span><span class="p">,</span> <span class="n">visibility</span><span class="p">])</span>
-</span><span id="Git-174"><a href="#Git-174"><span class="linenos">174</span></a>
-</span><span id="Git-175"><a href="#Git-175"><span class="linenos">175</span></a>    <span class="k">def</span> <span class="nf">create_remote_from_cwd</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">public</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git-176"><a href="#Git-176"><span class="linenos">176</span></a>        <span class="sd">&quot;&quot;&quot;Use GitHub CLI (must be installed and configured) to create a remote GitHub repo from</span>
-</span><span id="Git-177"><a href="#Git-177"><span class="linenos">177</span></a><span class="sd">        the current working directory repo and add its url as this repo&#39;s remote origin.</span>
-</span><span id="Git-178"><a href="#Git-178"><span class="linenos">178</span></a>
-</span><span id="Git-179"><a href="#Git-179"><span class="linenos">179</span></a><span class="sd">        #### :params:</span>
-</span><span id="Git-180"><a href="#Git-180"><span class="linenos">180</span></a>
-</span><span id="Git-181"><a href="#Git-181"><span class="linenos">181</span></a><span class="sd">        `public`: Create the GitHub repo as a public repo, default is to create it as private.&quot;&quot;&quot;</span>
-</span><span id="Git-182"><a href="#Git-182"><span class="linenos">182</span></a>        <span class="n">visibility</span> <span class="o">=</span> <span class="s2">&quot;public&quot;</span> <span class="k">if</span> <span class="n">public</span> <span class="k">else</span> <span class="s2">&quot;private&quot;</span>
-</span><span id="Git-183"><a href="#Git-183"><span class="linenos">183</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">(</span>
-</span><span id="Git-184"><a href="#Git-184"><span class="linenos">184</span></a>            <span class="p">[</span><span class="s2">&quot;gh&quot;</span><span class="p">,</span> <span class="s2">&quot;repo&quot;</span><span class="p">,</span> <span class="s2">&quot;create&quot;</span><span class="p">,</span> <span class="s2">&quot;--source&quot;</span><span class="p">,</span> <span class="s2">&quot;.&quot;</span><span class="p">,</span> <span class="sa">f</span><span class="s2">&quot;--</span><span class="si">{</span><span class="n">visibility</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">,</span> <span class="s2">&quot;--push&quot;</span><span class="p">]</span>
-</span><span id="Git-185"><a href="#Git-185"><span class="linenos">185</span></a>        <span class="p">)</span>
-</span><span id="Git-186"><a href="#Git-186"><span class="linenos">186</span></a>
-</span><span id="Git-187"><a href="#Git-187"><span class="linenos">187</span></a>    <span class="k">def</span> <span class="nf">_change_visibility</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">visibility</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git-188"><a href="#Git-188"><span class="linenos">188</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">(</span>
-</span><span id="Git-189"><a href="#Git-189"><span class="linenos">189</span></a>            <span class="p">[</span><span class="s2">&quot;gh&quot;</span><span class="p">,</span> <span class="s2">&quot;repo&quot;</span><span class="p">,</span> <span class="s2">&quot;edit&quot;</span><span class="p">,</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">owner</span><span class="si">}</span><span class="s2">/</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">,</span> <span class="s2">&quot;--visibility&quot;</span><span class="p">,</span> <span class="n">visibility</span><span class="p">]</span>
-</span><span id="Git-190"><a href="#Git-190"><span class="linenos">190</span></a>        <span class="p">)</span>
-</span><span id="Git-191"><a href="#Git-191"><span class="linenos">191</span></a>
-</span><span id="Git-192"><a href="#Git-192"><span class="linenos">192</span></a>    <span class="k">def</span> <span class="nf">make_private</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git-193"><a href="#Git-193"><span class="linenos">193</span></a>        <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be installed and configured) to set the repo&#39;s visibility to private.</span>
-</span><span id="Git-194"><a href="#Git-194"><span class="linenos">194</span></a>
-</span><span id="Git-195"><a href="#Git-195"><span class="linenos">195</span></a><span class="sd">        #### :params:</span>
-</span><span id="Git-196"><a href="#Git-196"><span class="linenos">196</span></a>
-</span><span id="Git-197"><a href="#Git-197"><span class="linenos">197</span></a><span class="sd">        `owner`: The repo owner.</span>
+</span><span id="Git-171"><a href="#Git-171"><span class="linenos">171</span></a>    <span class="k">def</span> <span class="nf">create_remote</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">public</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git-172"><a href="#Git-172"><span class="linenos">172</span></a>        <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be installed and configured) to create a remote GitHub repo.</span>
+</span><span id="Git-173"><a href="#Git-173"><span class="linenos">173</span></a>
+</span><span id="Git-174"><a href="#Git-174"><span class="linenos">174</span></a><span class="sd">        #### :params:</span>
+</span><span id="Git-175"><a href="#Git-175"><span class="linenos">175</span></a>
+</span><span id="Git-176"><a href="#Git-176"><span class="linenos">176</span></a><span class="sd">        `name`: The name for the repo.</span>
+</span><span id="Git-177"><a href="#Git-177"><span class="linenos">177</span></a>
+</span><span id="Git-178"><a href="#Git-178"><span class="linenos">178</span></a><span class="sd">        `public`: Set to `True` to create the repo as public, otherwise it&#39;ll be created as private.&quot;&quot;&quot;</span>
+</span><span id="Git-179"><a href="#Git-179"><span class="linenos">179</span></a>        <span class="n">visibility</span> <span class="o">=</span> <span class="s2">&quot;--public&quot;</span> <span class="k">if</span> <span class="n">public</span> <span class="k">else</span> <span class="s2">&quot;--private&quot;</span>
+</span><span id="Git-180"><a href="#Git-180"><span class="linenos">180</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">([</span><span class="s2">&quot;gh&quot;</span><span class="p">,</span> <span class="s2">&quot;repo&quot;</span><span class="p">,</span> <span class="s2">&quot;create&quot;</span><span class="p">,</span> <span class="n">name</span><span class="p">,</span> <span class="n">visibility</span><span class="p">])</span>
+</span><span id="Git-181"><a href="#Git-181"><span class="linenos">181</span></a>
+</span><span id="Git-182"><a href="#Git-182"><span class="linenos">182</span></a>    <span class="k">def</span> <span class="nf">create_remote_from_cwd</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">public</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git-183"><a href="#Git-183"><span class="linenos">183</span></a>        <span class="sd">&quot;&quot;&quot;Use GitHub CLI (must be installed and configured) to create a remote GitHub repo from</span>
+</span><span id="Git-184"><a href="#Git-184"><span class="linenos">184</span></a><span class="sd">        the current working directory repo and add its url as this repo&#39;s remote origin.</span>
+</span><span id="Git-185"><a href="#Git-185"><span class="linenos">185</span></a>
+</span><span id="Git-186"><a href="#Git-186"><span class="linenos">186</span></a><span class="sd">        #### :params:</span>
+</span><span id="Git-187"><a href="#Git-187"><span class="linenos">187</span></a>
+</span><span id="Git-188"><a href="#Git-188"><span class="linenos">188</span></a><span class="sd">        `public`: Create the GitHub repo as a public repo, default is to create it as private.&quot;&quot;&quot;</span>
+</span><span id="Git-189"><a href="#Git-189"><span class="linenos">189</span></a>        <span class="n">visibility</span> <span class="o">=</span> <span class="s2">&quot;public&quot;</span> <span class="k">if</span> <span class="n">public</span> <span class="k">else</span> <span class="s2">&quot;private&quot;</span>
+</span><span id="Git-190"><a href="#Git-190"><span class="linenos">190</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">(</span>
+</span><span id="Git-191"><a href="#Git-191"><span class="linenos">191</span></a>            <span class="p">[</span><span class="s2">&quot;gh&quot;</span><span class="p">,</span> <span class="s2">&quot;repo&quot;</span><span class="p">,</span> <span class="s2">&quot;create&quot;</span><span class="p">,</span> <span class="s2">&quot;--source&quot;</span><span class="p">,</span> <span class="s2">&quot;.&quot;</span><span class="p">,</span> <span class="sa">f</span><span class="s2">&quot;--</span><span class="si">{</span><span class="n">visibility</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">,</span> <span class="s2">&quot;--push&quot;</span><span class="p">]</span>
+</span><span id="Git-192"><a href="#Git-192"><span class="linenos">192</span></a>        <span class="p">)</span>
+</span><span id="Git-193"><a href="#Git-193"><span class="linenos">193</span></a>
+</span><span id="Git-194"><a href="#Git-194"><span class="linenos">194</span></a>    <span class="k">def</span> <span class="nf">_change_visibility</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">visibility</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git-195"><a href="#Git-195"><span class="linenos">195</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">(</span>
+</span><span id="Git-196"><a href="#Git-196"><span class="linenos">196</span></a>            <span class="p">[</span><span class="s2">&quot;gh&quot;</span><span class="p">,</span> <span class="s2">&quot;repo&quot;</span><span class="p">,</span> <span class="s2">&quot;edit&quot;</span><span class="p">,</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">owner</span><span class="si">}</span><span class="s2">/</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">,</span> <span class="s2">&quot;--visibility&quot;</span><span class="p">,</span> <span class="n">visibility</span><span class="p">]</span>
+</span><span id="Git-197"><a href="#Git-197"><span class="linenos">197</span></a>        <span class="p">)</span>
 </span><span id="Git-198"><a href="#Git-198"><span class="linenos">198</span></a>
-</span><span id="Git-199"><a href="#Git-199"><span class="linenos">199</span></a><span class="sd">        `name`: The name of the repo to edit.&quot;&quot;&quot;</span>
-</span><span id="Git-200"><a href="#Git-200"><span class="linenos">200</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_change_visibility</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">name</span><span class="p">,</span> <span class="s2">&quot;private&quot;</span><span class="p">)</span>
+</span><span id="Git-199"><a href="#Git-199"><span class="linenos">199</span></a>    <span class="k">def</span> <span class="nf">make_private</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git-200"><a href="#Git-200"><span class="linenos">200</span></a>        <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be installed and configured) to set the repo&#39;s visibility to private.</span>
 </span><span id="Git-201"><a href="#Git-201"><span class="linenos">201</span></a>
-</span><span id="Git-202"><a href="#Git-202"><span class="linenos">202</span></a>    <span class="k">def</span> <span class="nf">make_public</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git-203"><a href="#Git-203"><span class="linenos">203</span></a>        <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be installed and configured) to set the repo&#39;s visibility to public.</span>
-</span><span id="Git-204"><a href="#Git-204"><span class="linenos">204</span></a>
-</span><span id="Git-205"><a href="#Git-205"><span class="linenos">205</span></a><span class="sd">        #### :params:</span>
-</span><span id="Git-206"><a href="#Git-206"><span class="linenos">206</span></a>
-</span><span id="Git-207"><a href="#Git-207"><span class="linenos">207</span></a><span class="sd">        `owner`: The repo owner.</span>
+</span><span id="Git-202"><a href="#Git-202"><span class="linenos">202</span></a><span class="sd">        #### :params:</span>
+</span><span id="Git-203"><a href="#Git-203"><span class="linenos">203</span></a>
+</span><span id="Git-204"><a href="#Git-204"><span class="linenos">204</span></a><span class="sd">        `owner`: The repo owner.</span>
+</span><span id="Git-205"><a href="#Git-205"><span class="linenos">205</span></a>
+</span><span id="Git-206"><a href="#Git-206"><span class="linenos">206</span></a><span class="sd">        `name`: The name of the repo to edit.&quot;&quot;&quot;</span>
+</span><span id="Git-207"><a href="#Git-207"><span class="linenos">207</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_change_visibility</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">name</span><span class="p">,</span> <span class="s2">&quot;private&quot;</span><span class="p">)</span>
 </span><span id="Git-208"><a href="#Git-208"><span class="linenos">208</span></a>
-</span><span id="Git-209"><a href="#Git-209"><span class="linenos">209</span></a><span class="sd">        `name`: The name of the repo to edit.&quot;&quot;&quot;</span>
-</span><span id="Git-210"><a href="#Git-210"><span class="linenos">210</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_change_visibility</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">name</span><span class="p">,</span> <span class="s2">&quot;public&quot;</span><span class="p">)</span>
+</span><span id="Git-209"><a href="#Git-209"><span class="linenos">209</span></a>    <span class="k">def</span> <span class="nf">make_public</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git-210"><a href="#Git-210"><span class="linenos">210</span></a>        <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be installed and configured) to set the repo&#39;s visibility to public.</span>
 </span><span id="Git-211"><a href="#Git-211"><span class="linenos">211</span></a>
-</span><span id="Git-212"><a href="#Git-212"><span class="linenos">212</span></a>    <span class="k">def</span> <span class="nf">delete_remote</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git-213"><a href="#Git-213"><span class="linenos">213</span></a>        <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be isntalled and configured) to delete the remote for this repo.</span>
-</span><span id="Git-214"><a href="#Git-214"><span class="linenos">214</span></a>
-</span><span id="Git-215"><a href="#Git-215"><span class="linenos">215</span></a><span class="sd">        #### :params:</span>
-</span><span id="Git-216"><a href="#Git-216"><span class="linenos">216</span></a>
-</span><span id="Git-217"><a href="#Git-217"><span class="linenos">217</span></a><span class="sd">        `owner`: The repo owner.</span>
+</span><span id="Git-212"><a href="#Git-212"><span class="linenos">212</span></a><span class="sd">        #### :params:</span>
+</span><span id="Git-213"><a href="#Git-213"><span class="linenos">213</span></a>
+</span><span id="Git-214"><a href="#Git-214"><span class="linenos">214</span></a><span class="sd">        `owner`: The repo owner.</span>
+</span><span id="Git-215"><a href="#Git-215"><span class="linenos">215</span></a>
+</span><span id="Git-216"><a href="#Git-216"><span class="linenos">216</span></a><span class="sd">        `name`: The name of the repo to edit.&quot;&quot;&quot;</span>
+</span><span id="Git-217"><a href="#Git-217"><span class="linenos">217</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_change_visibility</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">name</span><span class="p">,</span> <span class="s2">&quot;public&quot;</span><span class="p">)</span>
 </span><span id="Git-218"><a href="#Git-218"><span class="linenos">218</span></a>
-</span><span id="Git-219"><a href="#Git-219"><span class="linenos">219</span></a><span class="sd">        `name`: The name of the remote repo to delete.&quot;&quot;&quot;</span>
-</span><span id="Git-220"><a href="#Git-220"><span class="linenos">220</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">([</span><span class="s2">&quot;gh&quot;</span><span class="p">,</span> <span class="s2">&quot;repo&quot;</span><span class="p">,</span> <span class="s2">&quot;delete&quot;</span><span class="p">,</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">owner</span><span class="si">}</span><span class="s2">/</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">,</span> <span class="s2">&quot;--yes&quot;</span><span class="p">])</span>
+</span><span id="Git-219"><a href="#Git-219"><span class="linenos">219</span></a>    <span class="k">def</span> <span class="nf">delete_remote</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git-220"><a href="#Git-220"><span class="linenos">220</span></a>        <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be isntalled and configured) to delete the remote for this repo.</span>
+</span><span id="Git-221"><a href="#Git-221"><span class="linenos">221</span></a>
+</span><span id="Git-222"><a href="#Git-222"><span class="linenos">222</span></a><span class="sd">        #### :params:</span>
+</span><span id="Git-223"><a href="#Git-223"><span class="linenos">223</span></a>
+</span><span id="Git-224"><a href="#Git-224"><span class="linenos">224</span></a><span class="sd">        `owner`: The repo owner.</span>
+</span><span id="Git-225"><a href="#Git-225"><span class="linenos">225</span></a>
+</span><span id="Git-226"><a href="#Git-226"><span class="linenos">226</span></a><span class="sd">        `name`: The name of the remote repo to delete.&quot;&quot;&quot;</span>
+</span><span id="Git-227"><a href="#Git-227"><span class="linenos">227</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">([</span><span class="s2">&quot;gh&quot;</span><span class="p">,</span> <span class="s2">&quot;repo&quot;</span><span class="p">,</span> <span class="s2">&quot;delete&quot;</span><span class="p">,</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">owner</span><span class="si">}</span><span class="s2">/</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">,</span> <span class="s2">&quot;--yes&quot;</span><span class="p">])</span>
 </span></pre></div>
 
 
     
 
                             <div id="Git.__init__" class="classattr">
                                         <input id="Git.__init__-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
@@ -607,18 +623,18 @@
             
         <span class="name">Git</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">capture_stdout</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span></span>)</span>
 
                 <label class="view-source-button" for="Git.__init__-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Git.__init__"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.__init__-7"><a href="#Git.__init__-7"><span class="linenos"> 7</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">capture_stdout</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">):</span>
-</span><span id="Git.__init__-8"><a href="#Git.__init__-8"><span class="linenos"> 8</span></a>        <span class="sd">&quot;&quot;&quot;If `capture_stdout` is `True`, all functions will return their generated `stdout` as a string.</span>
-</span><span id="Git.__init__-9"><a href="#Git.__init__-9"><span class="linenos"> 9</span></a><span class="sd">        Otherwise, the functions return the call&#39;s exit code.&quot;&quot;&quot;</span>
-</span><span id="Git.__init__-10"><a href="#Git.__init__-10"><span class="linenos">10</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">capture_stdout</span> <span class="o">=</span> <span class="n">capture_stdout</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.__init__-8"><a href="#Git.__init__-8"><span class="linenos"> 8</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">capture_stdout</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">):</span>
+</span><span id="Git.__init__-9"><a href="#Git.__init__-9"><span class="linenos"> 9</span></a>        <span class="sd">&quot;&quot;&quot;If `capture_stdout` is `True`, all functions will return their generated `stdout` as a string.</span>
+</span><span id="Git.__init__-10"><a href="#Git.__init__-10"><span class="linenos">10</span></a><span class="sd">        Otherwise, the functions return the call&#39;s exit code.&quot;&quot;&quot;</span>
+</span><span id="Git.__init__-11"><a href="#Git.__init__-11"><span class="linenos">11</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">capture_stdout</span> <span class="o">=</span> <span class="n">capture_stdout</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>If <code><a href="#Git.capture_stdout">capture_stdout</a></code> is <code>True</code>, all functions will return their generated <code>stdout</code> as a string.
 Otherwise, the functions return the call's exit code.</p>
 </div>
 
@@ -634,31 +650,54 @@
     
             <div class="docstring"><p>If <code>True</code>, member functions will return the generated <code>stdout</code> as a string,
 otherwise they return the command's exit code.</p>
 </div>
 
 
                             </div>
+                            <div id="Git.capture_output" class="classattr">
+                                        <input id="Git.capture_output-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
+<div class="attr function">
+                    <div class="decorator">@contextmanager</div>
+
+        <span class="def">def</span>
+        <span class="name">capture_output</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span></span><span class="return-annotation">):</span></span>
+
+                <label class="view-source-button" for="Git.capture_output-view-source"><span>View Source</span></label>
+
+    </div>
+    <a class="headerlink" href="#Git.capture_output"></a>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.capture_output-13"><a href="#Git.capture_output-13"><span class="linenos">13</span></a>    <span class="nd">@contextmanager</span>
+</span><span id="Git.capture_output-14"><a href="#Git.capture_output-14"><span class="linenos">14</span></a>    <span class="k">def</span> <span class="nf">capture_output</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="Git.capture_output-15"><a href="#Git.capture_output-15"><span class="linenos">15</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">capture_stdout</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="Git.capture_output-16"><a href="#Git.capture_output-16"><span class="linenos">16</span></a>        <span class="k">yield</span> <span class="bp">self</span>
+</span><span id="Git.capture_output-17"><a href="#Git.capture_output-17"><span class="linenos">17</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">capture_stdout</span> <span class="o">=</span> <span class="kc">False</span>
+</span></pre></div>
+
+
+    
+
+                            </div>
                             <div id="Git.execute" class="classattr">
                                         <input id="Git.execute-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
         <span class="name">execute</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">command</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">) -> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span>:</span></span>
 
                 <label class="view-source-button" for="Git.execute-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Git.execute"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.execute-28"><a href="#Git.execute-28"><span class="linenos">28</span></a>    <span class="k">def</span> <span class="nf">execute</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">command</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git.execute-29"><a href="#Git.execute-29"><span class="linenos">29</span></a>        <span class="sd">&quot;&quot;&quot;Execute git command.</span>
-</span><span id="Git.execute-30"><a href="#Git.execute-30"><span class="linenos">30</span></a>
-</span><span id="Git.execute-31"><a href="#Git.execute-31"><span class="linenos">31</span></a><span class="sd">        Equivalent to executing `git {command}` in the shell.&quot;&quot;&quot;</span>
-</span><span id="Git.execute-32"><a href="#Git.execute-32"><span class="linenos">32</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="p">[</span><span class="s2">&quot;git&quot;</span><span class="p">]</span> <span class="o">+</span> <span class="n">shlex</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="n">command</span><span class="p">)</span>
-</span><span id="Git.execute-33"><a href="#Git.execute-33"><span class="linenos">33</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.execute-35"><a href="#Git.execute-35"><span class="linenos">35</span></a>    <span class="k">def</span> <span class="nf">execute</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">command</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git.execute-36"><a href="#Git.execute-36"><span class="linenos">36</span></a>        <span class="sd">&quot;&quot;&quot;Execute git command.</span>
+</span><span id="Git.execute-37"><a href="#Git.execute-37"><span class="linenos">37</span></a>
+</span><span id="Git.execute-38"><a href="#Git.execute-38"><span class="linenos">38</span></a><span class="sd">        Equivalent to executing `git {command}` in the shell.&quot;&quot;&quot;</span>
+</span><span id="Git.execute-39"><a href="#Git.execute-39"><span class="linenos">39</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="p">[</span><span class="s2">&quot;git&quot;</span><span class="p">]</span> <span class="o">+</span> <span class="n">shlex</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="n">command</span><span class="p">)</span>
+</span><span id="Git.execute-40"><a href="#Git.execute-40"><span class="linenos">40</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Execute git command.</p>
 
 <p>Equivalent to executing <code>git {command}</code> in the shell.</p>
 </div>
@@ -672,17 +711,17 @@
         <span class="def">def</span>
         <span class="name">new_repo</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span></span><span class="return-annotation">) -> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span>:</span></span>
 
                 <label class="view-source-button" for="Git.new_repo-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Git.new_repo"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.new_repo-35"><a href="#Git.new_repo-35"><span class="linenos">35</span></a>    <span class="k">def</span> <span class="nf">new_repo</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git.new_repo-36"><a href="#Git.new_repo-36"><span class="linenos">36</span></a>        <span class="sd">&quot;&quot;&quot;Executes `git init -b main`.&quot;&quot;&quot;</span>
-</span><span id="Git.new_repo-37"><a href="#Git.new_repo-37"><span class="linenos">37</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="s2">&quot;init -b main&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.new_repo-42"><a href="#Git.new_repo-42"><span class="linenos">42</span></a>    <span class="k">def</span> <span class="nf">new_repo</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git.new_repo-43"><a href="#Git.new_repo-43"><span class="linenos">43</span></a>        <span class="sd">&quot;&quot;&quot;Executes `git init -b main`.&quot;&quot;&quot;</span>
+</span><span id="Git.new_repo-44"><a href="#Git.new_repo-44"><span class="linenos">44</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="s2">&quot;init -b main&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Executes <code>git init -b main</code>.</p>
 </div>
 
 
@@ -694,17 +733,17 @@
         <span class="def">def</span>
         <span class="name">loggy</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span></span><span class="return-annotation">) -> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span>:</span></span>
 
                 <label class="view-source-button" for="Git.loggy-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Git.loggy"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.loggy-39"><a href="#Git.loggy-39"><span class="linenos">39</span></a>    <span class="k">def</span> <span class="nf">loggy</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git.loggy-40"><a href="#Git.loggy-40"><span class="linenos">40</span></a>        <span class="sd">&quot;&quot;&quot;Equivalent to `git log --oneline --name-only --abbrev-commit --graph`.&quot;&quot;&quot;</span>
-</span><span id="Git.loggy-41"><a href="#Git.loggy-41"><span class="linenos">41</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="s2">&quot;log --oneline --name-only --abbrev-commit --graph&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.loggy-46"><a href="#Git.loggy-46"><span class="linenos">46</span></a>    <span class="k">def</span> <span class="nf">loggy</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git.loggy-47"><a href="#Git.loggy-47"><span class="linenos">47</span></a>        <span class="sd">&quot;&quot;&quot;Equivalent to `git log --oneline --name-only --abbrev-commit --graph`.&quot;&quot;&quot;</span>
+</span><span id="Git.loggy-48"><a href="#Git.loggy-48"><span class="linenos">48</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="s2">&quot;log --oneline --name-only --abbrev-commit --graph&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Equivalent to <code>git log --oneline --name-only --abbrev-commit --graph</code>.</p>
 </div>
 
 
@@ -716,17 +755,17 @@
         <span class="def">def</span>
         <span class="name">status</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span></span><span class="return-annotation">) -> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span>:</span></span>
 
                 <label class="view-source-button" for="Git.status-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Git.status"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.status-43"><a href="#Git.status-43"><span class="linenos">43</span></a>    <span class="k">def</span> <span class="nf">status</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git.status-44"><a href="#Git.status-44"><span class="linenos">44</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git status`.&quot;&quot;&quot;</span>
-</span><span id="Git.status-45"><a href="#Git.status-45"><span class="linenos">45</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="s2">&quot;status&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.status-50"><a href="#Git.status-50"><span class="linenos">50</span></a>    <span class="k">def</span> <span class="nf">status</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git.status-51"><a href="#Git.status-51"><span class="linenos">51</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git status`.&quot;&quot;&quot;</span>
+</span><span id="Git.status-52"><a href="#Git.status-52"><span class="linenos">52</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="s2">&quot;status&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Execute <code>git status</code>.</p>
 </div>
 
 
@@ -738,17 +777,17 @@
         <span class="def">def</span>
         <span class="name">commit</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">args</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">) -> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span>:</span></span>
 
                 <label class="view-source-button" for="Git.commit-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Git.commit"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.commit-48"><a href="#Git.commit-48"><span class="linenos">48</span></a>    <span class="k">def</span> <span class="nf">commit</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git.commit-49"><a href="#Git.commit-49"><span class="linenos">49</span></a>        <span class="sd">&quot;&quot;&quot;&gt;&gt;&gt; git commit {args}&quot;&quot;&quot;</span>
-</span><span id="Git.commit-50"><a href="#Git.commit-50"><span class="linenos">50</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;commit </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.commit-55"><a href="#Git.commit-55"><span class="linenos">55</span></a>    <span class="k">def</span> <span class="nf">commit</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git.commit-56"><a href="#Git.commit-56"><span class="linenos">56</span></a>        <span class="sd">&quot;&quot;&quot;&gt;&gt;&gt; git commit {args}&quot;&quot;&quot;</span>
+</span><span id="Git.commit-57"><a href="#Git.commit-57"><span class="linenos">57</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;commit </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><div class="pdoc-code codehilite">
 <pre><span></span><code><span class="gp">&gt;&gt;&gt; </span><span class="n">git</span> <span class="n">commit</span> <span class="p">{</span><span class="n">args</span><span class="p">}</span>
 </code></pre>
 </div>
@@ -763,23 +802,23 @@
         <span class="def">def</span>
         <span class="name">add</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">files</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span></span><span class="return-annotation">) -> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span>:</span></span>
 
                 <label class="view-source-button" for="Git.add-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Git.add"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.add-52"><a href="#Git.add-52"><span class="linenos">52</span></a>    <span class="k">def</span> <span class="nf">add</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">files</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git.add-53"><a href="#Git.add-53"><span class="linenos">53</span></a>        <span class="sd">&quot;&quot;&quot;Stage a list of files.</span>
-</span><span id="Git.add-54"><a href="#Git.add-54"><span class="linenos">54</span></a>
-</span><span id="Git.add-55"><a href="#Git.add-55"><span class="linenos">55</span></a><span class="sd">        If no files are given (`files=None`), all files will be staged.&quot;&quot;&quot;</span>
-</span><span id="Git.add-56"><a href="#Git.add-56"><span class="linenos">56</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">files</span><span class="p">:</span>
-</span><span id="Git.add-57"><a href="#Git.add-57"><span class="linenos">57</span></a>            <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="s2">&quot;add .&quot;</span><span class="p">)</span>
-</span><span id="Git.add-58"><a href="#Git.add-58"><span class="linenos">58</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="Git.add-59"><a href="#Git.add-59"><span class="linenos">59</span></a>            <span class="n">files</span> <span class="o">=</span> <span class="s2">&quot; &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;&quot;</span><span class="si">{</span><span class="n">file</span><span class="si">}</span><span class="s1">&quot;&#39;</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">files</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
-</span><span id="Git.add-60"><a href="#Git.add-60"><span class="linenos">60</span></a>            <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;add </span><span class="si">{</span><span class="n">files</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.add-59"><a href="#Git.add-59"><span class="linenos">59</span></a>    <span class="k">def</span> <span class="nf">add</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">files</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git.add-60"><a href="#Git.add-60"><span class="linenos">60</span></a>        <span class="sd">&quot;&quot;&quot;Stage a list of files.</span>
+</span><span id="Git.add-61"><a href="#Git.add-61"><span class="linenos">61</span></a>
+</span><span id="Git.add-62"><a href="#Git.add-62"><span class="linenos">62</span></a><span class="sd">        If no files are given (`files=None`), all files will be staged.&quot;&quot;&quot;</span>
+</span><span id="Git.add-63"><a href="#Git.add-63"><span class="linenos">63</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">files</span><span class="p">:</span>
+</span><span id="Git.add-64"><a href="#Git.add-64"><span class="linenos">64</span></a>            <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="s2">&quot;add .&quot;</span><span class="p">)</span>
+</span><span id="Git.add-65"><a href="#Git.add-65"><span class="linenos">65</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="Git.add-66"><a href="#Git.add-66"><span class="linenos">66</span></a>            <span class="n">files</span> <span class="o">=</span> <span class="s2">&quot; &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;&quot;</span><span class="si">{</span><span class="n">file</span><span class="si">}</span><span class="s1">&quot;&#39;</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">files</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
+</span><span id="Git.add-67"><a href="#Git.add-67"><span class="linenos">67</span></a>            <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;add </span><span class="si">{</span><span class="n">files</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Stage a list of files.</p>
 
 <p>If no files are given (<code>files=None</code>), all files will be staged.</p>
 </div>
@@ -793,17 +832,17 @@
         <span class="def">def</span>
         <span class="name">commit_files</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">files</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span>, </span><span class="param"><span class="n">message</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">) -> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span>:</span></span>
 
                 <label class="view-source-button" for="Git.commit_files-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Git.commit_files"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.commit_files-62"><a href="#Git.commit_files-62"><span class="linenos">62</span></a>    <span class="k">def</span> <span class="nf">commit_files</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">files</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">],</span> <span class="n">message</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git.commit_files-63"><a href="#Git.commit_files-63"><span class="linenos">63</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit a list of files with commit message `message`.&quot;&quot;&quot;</span>
-</span><span id="Git.commit_files-64"><a href="#Git.commit_files-64"><span class="linenos">64</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">add</span><span class="p">(</span><span class="n">files</span><span class="p">)</span> <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;-m &quot;</span><span class="si">{</span><span class="n">message</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.commit_files-69"><a href="#Git.commit_files-69"><span class="linenos">69</span></a>    <span class="k">def</span> <span class="nf">commit_files</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">files</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">],</span> <span class="n">message</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git.commit_files-70"><a href="#Git.commit_files-70"><span class="linenos">70</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit a list of files with commit message `message`.&quot;&quot;&quot;</span>
+</span><span id="Git.commit_files-71"><a href="#Git.commit_files-71"><span class="linenos">71</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">add</span><span class="p">(</span><span class="n">files</span><span class="p">)</span> <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;-m &quot;</span><span class="si">{</span><span class="n">message</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Stage and commit a list of files with commit message <code>message</code>.</p>
 </div>
 
 
@@ -815,19 +854,19 @@
         <span class="def">def</span>
         <span class="name">initcommit</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span></span><span class="return-annotation">) -> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span>:</span></span>
 
                 <label class="view-source-button" for="Git.initcommit-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Git.initcommit"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.initcommit-66"><a href="#Git.initcommit-66"><span class="linenos">66</span></a>    <span class="k">def</span> <span class="nf">initcommit</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git.initcommit-67"><a href="#Git.initcommit-67"><span class="linenos">67</span></a>        <span class="sd">&quot;&quot;&quot;Equivalent to</span>
-</span><span id="Git.initcommit-68"><a href="#Git.initcommit-68"><span class="linenos">68</span></a><span class="sd">        &gt;&gt;&gt; git add .</span>
-</span><span id="Git.initcommit-69"><a href="#Git.initcommit-69"><span class="linenos">69</span></a><span class="sd">        &gt;&gt;&gt; git commit -m &quot;Initial commit&quot; &quot;&quot;&quot;</span>
-</span><span id="Git.initcommit-70"><a href="#Git.initcommit-70"><span class="linenos">70</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">add</span><span class="p">()</span> <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="s1">&#39;-m &quot;Initial commit&quot;&#39;</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.initcommit-73"><a href="#Git.initcommit-73"><span class="linenos">73</span></a>    <span class="k">def</span> <span class="nf">initcommit</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git.initcommit-74"><a href="#Git.initcommit-74"><span class="linenos">74</span></a>        <span class="sd">&quot;&quot;&quot;Equivalent to</span>
+</span><span id="Git.initcommit-75"><a href="#Git.initcommit-75"><span class="linenos">75</span></a><span class="sd">        &gt;&gt;&gt; git add .</span>
+</span><span id="Git.initcommit-76"><a href="#Git.initcommit-76"><span class="linenos">76</span></a><span class="sd">        &gt;&gt;&gt; git commit -m &quot;Initial commit&quot; &quot;&quot;&quot;</span>
+</span><span id="Git.initcommit-77"><a href="#Git.initcommit-77"><span class="linenos">77</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">add</span><span class="p">()</span> <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="s1">&#39;-m &quot;Initial commit&quot;&#39;</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Equivalent to</p>
 
 <div class="pdoc-code codehilite">
 <pre><span></span><code><span class="gp">&gt;&gt;&gt; </span><span class="n">git</span> <span class="n">add</span> <span class="o">.</span>
@@ -845,24 +884,24 @@
         <span class="def">def</span>
         <span class="name">amend</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">files</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span></span><span class="return-annotation">) -> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span>:</span></span>
 
                 <label class="view-source-button" for="Git.amend-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Git.amend"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.amend-72"><a href="#Git.amend-72"><span class="linenos">72</span></a>    <span class="k">def</span> <span class="nf">amend</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">files</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git.amend-73"><a href="#Git.amend-73"><span class="linenos">73</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit changes to the previous commit.</span>
-</span><span id="Git.amend-74"><a href="#Git.amend-74"><span class="linenos">74</span></a>
-</span><span id="Git.amend-75"><a href="#Git.amend-75"><span class="linenos">75</span></a><span class="sd">        If `files` is `None`, all files will be staged.</span>
-</span><span id="Git.amend-76"><a href="#Git.amend-76"><span class="linenos">76</span></a>
-</span><span id="Git.amend-77"><a href="#Git.amend-77"><span class="linenos">77</span></a><span class="sd">        Equivalent to:</span>
-</span><span id="Git.amend-78"><a href="#Git.amend-78"><span class="linenos">78</span></a><span class="sd">        &gt;&gt;&gt; git add {files}</span>
-</span><span id="Git.amend-79"><a href="#Git.amend-79"><span class="linenos">79</span></a><span class="sd">        &gt;&gt;&gt; git commit --amend --no-edit</span>
-</span><span id="Git.amend-80"><a href="#Git.amend-80"><span class="linenos">80</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="Git.amend-81"><a href="#Git.amend-81"><span class="linenos">81</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">add</span><span class="p">(</span><span class="n">files</span><span class="p">)</span> <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="s2">&quot;--amend --no-edit&quot;</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.amend-79"><a href="#Git.amend-79"><span class="linenos">79</span></a>    <span class="k">def</span> <span class="nf">amend</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">files</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git.amend-80"><a href="#Git.amend-80"><span class="linenos">80</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit changes to the previous commit.</span>
+</span><span id="Git.amend-81"><a href="#Git.amend-81"><span class="linenos">81</span></a>
+</span><span id="Git.amend-82"><a href="#Git.amend-82"><span class="linenos">82</span></a><span class="sd">        If `files` is `None`, all files will be staged.</span>
+</span><span id="Git.amend-83"><a href="#Git.amend-83"><span class="linenos">83</span></a>
+</span><span id="Git.amend-84"><a href="#Git.amend-84"><span class="linenos">84</span></a><span class="sd">        Equivalent to:</span>
+</span><span id="Git.amend-85"><a href="#Git.amend-85"><span class="linenos">85</span></a><span class="sd">        &gt;&gt;&gt; git add {files}</span>
+</span><span id="Git.amend-86"><a href="#Git.amend-86"><span class="linenos">86</span></a><span class="sd">        &gt;&gt;&gt; git commit --amend --no-edit</span>
+</span><span id="Git.amend-87"><a href="#Git.amend-87"><span class="linenos">87</span></a><span class="sd">        &quot;&quot;&quot;</span>
+</span><span id="Git.amend-88"><a href="#Git.amend-88"><span class="linenos">88</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">add</span><span class="p">(</span><span class="n">files</span><span class="p">)</span> <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="s2">&quot;--amend --no-edit&quot;</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Stage and commit changes to the previous commit.</p>
 
 <p>If <code>files</code> is <code>None</code>, all files will be staged.</p>
 
@@ -884,23 +923,23 @@
         <span class="def">def</span>
         <span class="name">tag</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">args</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s1">&#39;&#39;</span></span><span class="return-annotation">) -> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span>:</span></span>
 
                 <label class="view-source-button" for="Git.tag-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Git.tag"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.tag-83"><a href="#Git.tag-83"><span class="linenos">83</span></a>    <span class="k">def</span> <span class="nf">tag</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git.tag-84"><a href="#Git.tag-84"><span class="linenos">84</span></a>        <span class="sd">&quot;&quot;&quot;Execute the `tag` command with `args`.</span>
-</span><span id="Git.tag-85"><a href="#Git.tag-85"><span class="linenos">85</span></a>
-</span><span id="Git.tag-86"><a href="#Git.tag-86"><span class="linenos">86</span></a><span class="sd">        e.g.</span>
-</span><span id="Git.tag-87"><a href="#Git.tag-87"><span class="linenos">87</span></a>
-</span><span id="Git.tag-88"><a href="#Git.tag-88"><span class="linenos">88</span></a><span class="sd">        `self.tag(&quot;--sort=-committerdate&quot;)`</span>
-</span><span id="Git.tag-89"><a href="#Git.tag-89"><span class="linenos">89</span></a>
-</span><span id="Git.tag-90"><a href="#Git.tag-90"><span class="linenos">90</span></a><span class="sd">        will list all the tags for this repository in descending commit date.&quot;&quot;&quot;</span>
-</span><span id="Git.tag-91"><a href="#Git.tag-91"><span class="linenos">91</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;tag </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.tag-90"><a href="#Git.tag-90"><span class="linenos">90</span></a>    <span class="k">def</span> <span class="nf">tag</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git.tag-91"><a href="#Git.tag-91"><span class="linenos">91</span></a>        <span class="sd">&quot;&quot;&quot;Execute the `tag` command with `args`.</span>
+</span><span id="Git.tag-92"><a href="#Git.tag-92"><span class="linenos">92</span></a>
+</span><span id="Git.tag-93"><a href="#Git.tag-93"><span class="linenos">93</span></a><span class="sd">        e.g.</span>
+</span><span id="Git.tag-94"><a href="#Git.tag-94"><span class="linenos">94</span></a>
+</span><span id="Git.tag-95"><a href="#Git.tag-95"><span class="linenos">95</span></a><span class="sd">        `self.tag(&quot;--sort=-committerdate&quot;)`</span>
+</span><span id="Git.tag-96"><a href="#Git.tag-96"><span class="linenos">96</span></a>
+</span><span id="Git.tag-97"><a href="#Git.tag-97"><span class="linenos">97</span></a><span class="sd">        will list all the tags for this repository in descending commit date.&quot;&quot;&quot;</span>
+</span><span id="Git.tag-98"><a href="#Git.tag-98"><span class="linenos">98</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;tag </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Execute the <code><a href="#Git.tag">tag</a></code> command with <code>args</code>.</p>
 
 <p>e.g.</p>
 
@@ -918,17 +957,17 @@
         <span class="def">def</span>
         <span class="name">add_remote_url</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">url</span><span class="p">:</span> <span class="nb">str</span>, </span><span class="param"><span class="n">name</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s1">&#39;origin&#39;</span></span><span class="return-annotation">) -> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span>:</span></span>
 
                 <label class="view-source-button" for="Git.add_remote_url-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Git.add_remote_url"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.add_remote_url-94"><a href="#Git.add_remote_url-94"><span class="linenos">94</span></a>    <span class="k">def</span> <span class="nf">add_remote_url</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">url</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;origin&quot;</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git.add_remote_url-95"><a href="#Git.add_remote_url-95"><span class="linenos">95</span></a>        <span class="sd">&quot;&quot;&quot;Add remote url to repo.&quot;&quot;&quot;</span>
-</span><span id="Git.add_remote_url-96"><a href="#Git.add_remote_url-96"><span class="linenos">96</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;remote add </span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">url</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.add_remote_url-101"><a href="#Git.add_remote_url-101"><span class="linenos">101</span></a>    <span class="k">def</span> <span class="nf">add_remote_url</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">url</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;origin&quot;</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git.add_remote_url-102"><a href="#Git.add_remote_url-102"><span class="linenos">102</span></a>        <span class="sd">&quot;&quot;&quot;Add remote url to repo.&quot;&quot;&quot;</span>
+</span><span id="Git.add_remote_url-103"><a href="#Git.add_remote_url-103"><span class="linenos">103</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;remote add </span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">url</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Add remote url to repo.</p>
 </div>
 
 
@@ -940,17 +979,17 @@
         <span class="def">def</span>
         <span class="name">push</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">args</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s1">&#39;&#39;</span></span><span class="return-annotation">) -> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span>:</span></span>
 
                 <label class="view-source-button" for="Git.push-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Git.push"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.push-98"><a href="#Git.push-98"><span class="linenos"> 98</span></a>    <span class="k">def</span> <span class="nf">push</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git.push-99"><a href="#Git.push-99"><span class="linenos"> 99</span></a>        <span class="sd">&quot;&quot;&quot;Equivalent to `git push {args}`.&quot;&quot;&quot;</span>
-</span><span id="Git.push-100"><a href="#Git.push-100"><span class="linenos">100</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;push </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.push-105"><a href="#Git.push-105"><span class="linenos">105</span></a>    <span class="k">def</span> <span class="nf">push</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git.push-106"><a href="#Git.push-106"><span class="linenos">106</span></a>        <span class="sd">&quot;&quot;&quot;Equivalent to `git push {args}`.&quot;&quot;&quot;</span>
+</span><span id="Git.push-107"><a href="#Git.push-107"><span class="linenos">107</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;push </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Equivalent to <code>git push {args}</code>.</p>
 </div>
 
 
@@ -962,17 +1001,17 @@
         <span class="def">def</span>
         <span class="name">pull</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">args</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s1">&#39;&#39;</span></span><span class="return-annotation">) -> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span>:</span></span>
 
                 <label class="view-source-button" for="Git.pull-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Git.pull"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.pull-102"><a href="#Git.pull-102"><span class="linenos">102</span></a>    <span class="k">def</span> <span class="nf">pull</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git.pull-103"><a href="#Git.pull-103"><span class="linenos">103</span></a>        <span class="sd">&quot;&quot;&quot;Equivalent to `git pull {args}`.&quot;&quot;&quot;</span>
-</span><span id="Git.pull-104"><a href="#Git.pull-104"><span class="linenos">104</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;pull </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.pull-109"><a href="#Git.pull-109"><span class="linenos">109</span></a>    <span class="k">def</span> <span class="nf">pull</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git.pull-110"><a href="#Git.pull-110"><span class="linenos">110</span></a>        <span class="sd">&quot;&quot;&quot;Equivalent to `git pull {args}`.&quot;&quot;&quot;</span>
+</span><span id="Git.pull-111"><a href="#Git.pull-111"><span class="linenos">111</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;pull </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Equivalent to <code>git pull {args}</code>.</p>
 </div>
 
 
@@ -984,19 +1023,19 @@
         <span class="def">def</span>
         <span class="name">push_new_branch</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">branch</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">) -> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span>:</span></span>
 
                 <label class="view-source-button" for="Git.push_new_branch-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Git.push_new_branch"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.push_new_branch-106"><a href="#Git.push_new_branch-106"><span class="linenos">106</span></a>    <span class="k">def</span> <span class="nf">push_new_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git.push_new_branch-107"><a href="#Git.push_new_branch-107"><span class="linenos">107</span></a>        <span class="sd">&quot;&quot;&quot;Push a new branch to origin with tracking.</span>
-</span><span id="Git.push_new_branch-108"><a href="#Git.push_new_branch-108"><span class="linenos">108</span></a>
-</span><span id="Git.push_new_branch-109"><a href="#Git.push_new_branch-109"><span class="linenos">109</span></a><span class="sd">        Equivalent to `git push -u origin {branch}`.&quot;&quot;&quot;</span>
-</span><span id="Git.push_new_branch-110"><a href="#Git.push_new_branch-110"><span class="linenos">110</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-u origin </span><span class="si">{</span><span class="n">branch</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.push_new_branch-113"><a href="#Git.push_new_branch-113"><span class="linenos">113</span></a>    <span class="k">def</span> <span class="nf">push_new_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git.push_new_branch-114"><a href="#Git.push_new_branch-114"><span class="linenos">114</span></a>        <span class="sd">&quot;&quot;&quot;Push a new branch to origin with tracking.</span>
+</span><span id="Git.push_new_branch-115"><a href="#Git.push_new_branch-115"><span class="linenos">115</span></a>
+</span><span id="Git.push_new_branch-116"><a href="#Git.push_new_branch-116"><span class="linenos">116</span></a><span class="sd">        Equivalent to `git push -u origin {branch}`.&quot;&quot;&quot;</span>
+</span><span id="Git.push_new_branch-117"><a href="#Git.push_new_branch-117"><span class="linenos">117</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-u origin </span><span class="si">{</span><span class="n">branch</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Push a new branch to origin with tracking.</p>
 
 <p>Equivalent to <code>git push -u origin {branch}</code>.</p>
 </div>
@@ -1010,17 +1049,17 @@
         <span class="def">def</span>
         <span class="name">pull_branch</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">branch</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">) -> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span>:</span></span>
 
                 <label class="view-source-button" for="Git.pull_branch-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Git.pull_branch"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.pull_branch-112"><a href="#Git.pull_branch-112"><span class="linenos">112</span></a>    <span class="k">def</span> <span class="nf">pull_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git.pull_branch-113"><a href="#Git.pull_branch-113"><span class="linenos">113</span></a>        <span class="sd">&quot;&quot;&quot;Pull `branch` from origin.&quot;&quot;&quot;</span>
-</span><span id="Git.pull_branch-114"><a href="#Git.pull_branch-114"><span class="linenos">114</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">pull</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;origin </span><span class="si">{</span><span class="n">branch</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.pull_branch-119"><a href="#Git.pull_branch-119"><span class="linenos">119</span></a>    <span class="k">def</span> <span class="nf">pull_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git.pull_branch-120"><a href="#Git.pull_branch-120"><span class="linenos">120</span></a>        <span class="sd">&quot;&quot;&quot;Pull `branch` from origin.&quot;&quot;&quot;</span>
+</span><span id="Git.pull_branch-121"><a href="#Git.pull_branch-121"><span class="linenos">121</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">pull</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;origin </span><span class="si">{</span><span class="n">branch</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Pull <code><a href="#Git.branch">branch</a></code> from origin.</p>
 </div>
 
 
@@ -1032,17 +1071,17 @@
         <span class="def">def</span>
         <span class="name">branch</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">args</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">) -> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span>:</span></span>
 
                 <label class="view-source-button" for="Git.branch-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Git.branch"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.branch-117"><a href="#Git.branch-117"><span class="linenos">117</span></a>    <span class="k">def</span> <span class="nf">branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git.branch-118"><a href="#Git.branch-118"><span class="linenos">118</span></a>        <span class="sd">&quot;&quot;&quot;Equivalent to `git branch {args}`.&quot;&quot;&quot;</span>
-</span><span id="Git.branch-119"><a href="#Git.branch-119"><span class="linenos">119</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;branch </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.branch-124"><a href="#Git.branch-124"><span class="linenos">124</span></a>    <span class="k">def</span> <span class="nf">branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git.branch-125"><a href="#Git.branch-125"><span class="linenos">125</span></a>        <span class="sd">&quot;&quot;&quot;Equivalent to `git branch {args}`.&quot;&quot;&quot;</span>
+</span><span id="Git.branch-126"><a href="#Git.branch-126"><span class="linenos">126</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;branch </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Equivalent to <code>git branch {args}</code>.</p>
 </div>
 
 
@@ -1054,17 +1093,17 @@
         <span class="def">def</span>
         <span class="name">list_branches</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span></span><span class="return-annotation">) -> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span>:</span></span>
 
                 <label class="view-source-button" for="Git.list_branches-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Git.list_branches"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.list_branches-121"><a href="#Git.list_branches-121"><span class="linenos">121</span></a>    <span class="k">def</span> <span class="nf">list_branches</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git.list_branches-122"><a href="#Git.list_branches-122"><span class="linenos">122</span></a>        <span class="sd">&quot;&quot;&quot;Print a list of branches.&quot;&quot;&quot;</span>
-</span><span id="Git.list_branches-123"><a href="#Git.list_branches-123"><span class="linenos">123</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">branch</span><span class="p">(</span><span class="s2">&quot;-vva&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.list_branches-128"><a href="#Git.list_branches-128"><span class="linenos">128</span></a>    <span class="k">def</span> <span class="nf">list_branches</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git.list_branches-129"><a href="#Git.list_branches-129"><span class="linenos">129</span></a>        <span class="sd">&quot;&quot;&quot;Print a list of branches.&quot;&quot;&quot;</span>
+</span><span id="Git.list_branches-130"><a href="#Git.list_branches-130"><span class="linenos">130</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">branch</span><span class="p">(</span><span class="s2">&quot;-vva&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Print a list of branches.</p>
 </div>
 
 
@@ -1076,17 +1115,17 @@
         <span class="def">def</span>
         <span class="name">checkout</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">args</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">) -> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span>:</span></span>
 
                 <label class="view-source-button" for="Git.checkout-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Git.checkout"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.checkout-125"><a href="#Git.checkout-125"><span class="linenos">125</span></a>    <span class="k">def</span> <span class="nf">checkout</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git.checkout-126"><a href="#Git.checkout-126"><span class="linenos">126</span></a>        <span class="sd">&quot;&quot;&quot;Equivalent to `git checkout {args}`.&quot;&quot;&quot;</span>
-</span><span id="Git.checkout-127"><a href="#Git.checkout-127"><span class="linenos">127</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;checkout </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.checkout-132"><a href="#Git.checkout-132"><span class="linenos">132</span></a>    <span class="k">def</span> <span class="nf">checkout</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git.checkout-133"><a href="#Git.checkout-133"><span class="linenos">133</span></a>        <span class="sd">&quot;&quot;&quot;Equivalent to `git checkout {args}`.&quot;&quot;&quot;</span>
+</span><span id="Git.checkout-134"><a href="#Git.checkout-134"><span class="linenos">134</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;checkout </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Equivalent to <code>git checkout {args}</code>.</p>
 </div>
 
 
@@ -1098,19 +1137,19 @@
         <span class="def">def</span>
         <span class="name">switch_branch</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">) -> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span>:</span></span>
 
                 <label class="view-source-button" for="Git.switch_branch-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Git.switch_branch"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.switch_branch-129"><a href="#Git.switch_branch-129"><span class="linenos">129</span></a>    <span class="k">def</span> <span class="nf">switch_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git.switch_branch-130"><a href="#Git.switch_branch-130"><span class="linenos">130</span></a>        <span class="sd">&quot;&quot;&quot;Switch to the branch specified by `branch_name`.</span>
-</span><span id="Git.switch_branch-131"><a href="#Git.switch_branch-131"><span class="linenos">131</span></a>
-</span><span id="Git.switch_branch-132"><a href="#Git.switch_branch-132"><span class="linenos">132</span></a><span class="sd">        Equivalent to `git checkout {branch_name}`.&quot;&quot;&quot;</span>
-</span><span id="Git.switch_branch-133"><a href="#Git.switch_branch-133"><span class="linenos">133</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">checkout</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.switch_branch-136"><a href="#Git.switch_branch-136"><span class="linenos">136</span></a>    <span class="k">def</span> <span class="nf">switch_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git.switch_branch-137"><a href="#Git.switch_branch-137"><span class="linenos">137</span></a>        <span class="sd">&quot;&quot;&quot;Switch to the branch specified by `branch_name`.</span>
+</span><span id="Git.switch_branch-138"><a href="#Git.switch_branch-138"><span class="linenos">138</span></a>
+</span><span id="Git.switch_branch-139"><a href="#Git.switch_branch-139"><span class="linenos">139</span></a><span class="sd">        Equivalent to `git checkout {branch_name}`.&quot;&quot;&quot;</span>
+</span><span id="Git.switch_branch-140"><a href="#Git.switch_branch-140"><span class="linenos">140</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">checkout</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Switch to the branch specified by <code>branch_name</code>.</p>
 
 <p>Equivalent to <code>git checkout {branch_name}</code>.</p>
 </div>
@@ -1124,19 +1163,19 @@
         <span class="def">def</span>
         <span class="name">create_new_branch</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">) -> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span>:</span></span>
 
                 <label class="view-source-button" for="Git.create_new_branch-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Git.create_new_branch"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.create_new_branch-135"><a href="#Git.create_new_branch-135"><span class="linenos">135</span></a>    <span class="k">def</span> <span class="nf">create_new_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git.create_new_branch-136"><a href="#Git.create_new_branch-136"><span class="linenos">136</span></a>        <span class="sd">&quot;&quot;&quot;Create and switch to a new branch named with `branch_name`.</span>
-</span><span id="Git.create_new_branch-137"><a href="#Git.create_new_branch-137"><span class="linenos">137</span></a>
-</span><span id="Git.create_new_branch-138"><a href="#Git.create_new_branch-138"><span class="linenos">138</span></a><span class="sd">        Equivalent to `git checkout -b {branch_name} --track`.&quot;&quot;&quot;</span>
-</span><span id="Git.create_new_branch-139"><a href="#Git.create_new_branch-139"><span class="linenos">139</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">checkout</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-b </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2"> --track&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.create_new_branch-142"><a href="#Git.create_new_branch-142"><span class="linenos">142</span></a>    <span class="k">def</span> <span class="nf">create_new_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git.create_new_branch-143"><a href="#Git.create_new_branch-143"><span class="linenos">143</span></a>        <span class="sd">&quot;&quot;&quot;Create and switch to a new branch named with `branch_name`.</span>
+</span><span id="Git.create_new_branch-144"><a href="#Git.create_new_branch-144"><span class="linenos">144</span></a>
+</span><span id="Git.create_new_branch-145"><a href="#Git.create_new_branch-145"><span class="linenos">145</span></a><span class="sd">        Equivalent to `git checkout -b {branch_name} --track`.&quot;&quot;&quot;</span>
+</span><span id="Git.create_new_branch-146"><a href="#Git.create_new_branch-146"><span class="linenos">146</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">checkout</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-b </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2"> --track&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Create and switch to a new branch named with <code>branch_name</code>.</p>
 
 <p>Equivalent to <code>git checkout -b {branch_name} --track</code>.</p>
 </div>
@@ -1150,24 +1189,24 @@
         <span class="def">def</span>
         <span class="name">delete_branch</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span>, </span><span class="param"><span class="n">local_only</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span></span><span class="return-annotation">) -> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span>:</span></span>
 
                 <label class="view-source-button" for="Git.delete_branch-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Git.delete_branch"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.delete_branch-141"><a href="#Git.delete_branch-141"><span class="linenos">141</span></a>    <span class="k">def</span> <span class="nf">delete_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">local_only</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git.delete_branch-142"><a href="#Git.delete_branch-142"><span class="linenos">142</span></a>        <span class="sd">&quot;&quot;&quot;Delete `branch_name` from repo.</span>
-</span><span id="Git.delete_branch-143"><a href="#Git.delete_branch-143"><span class="linenos">143</span></a>
-</span><span id="Git.delete_branch-144"><a href="#Git.delete_branch-144"><span class="linenos">144</span></a><span class="sd">        #### :params:</span>
-</span><span id="Git.delete_branch-145"><a href="#Git.delete_branch-145"><span class="linenos">145</span></a>
-</span><span id="Git.delete_branch-146"><a href="#Git.delete_branch-146"><span class="linenos">146</span></a><span class="sd">        `local_only`: Only delete the local copy of `branch`, otherwise also delete the remote branch on origin and remote-tracking branch.&quot;&quot;&quot;</span>
-</span><span id="Git.delete_branch-147"><a href="#Git.delete_branch-147"><span class="linenos">147</span></a>        <span class="n">output</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">branch</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;--delete </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="Git.delete_branch-148"><a href="#Git.delete_branch-148"><span class="linenos">148</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">local_only</span><span class="p">:</span>
-</span><span id="Git.delete_branch-149"><a href="#Git.delete_branch-149"><span class="linenos">149</span></a>            <span class="k">return</span> <span class="n">output</span> <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;origin --delete </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>  <span class="c1"># type:ignore</span>
-</span><span id="Git.delete_branch-150"><a href="#Git.delete_branch-150"><span class="linenos">150</span></a>        <span class="k">return</span> <span class="n">output</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.delete_branch-148"><a href="#Git.delete_branch-148"><span class="linenos">148</span></a>    <span class="k">def</span> <span class="nf">delete_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">local_only</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git.delete_branch-149"><a href="#Git.delete_branch-149"><span class="linenos">149</span></a>        <span class="sd">&quot;&quot;&quot;Delete `branch_name` from repo.</span>
+</span><span id="Git.delete_branch-150"><a href="#Git.delete_branch-150"><span class="linenos">150</span></a>
+</span><span id="Git.delete_branch-151"><a href="#Git.delete_branch-151"><span class="linenos">151</span></a><span class="sd">        #### :params:</span>
+</span><span id="Git.delete_branch-152"><a href="#Git.delete_branch-152"><span class="linenos">152</span></a>
+</span><span id="Git.delete_branch-153"><a href="#Git.delete_branch-153"><span class="linenos">153</span></a><span class="sd">        `local_only`: Only delete the local copy of `branch`, otherwise also delete the remote branch on origin and remote-tracking branch.&quot;&quot;&quot;</span>
+</span><span id="Git.delete_branch-154"><a href="#Git.delete_branch-154"><span class="linenos">154</span></a>        <span class="n">output</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">branch</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;--delete </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="Git.delete_branch-155"><a href="#Git.delete_branch-155"><span class="linenos">155</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">local_only</span><span class="p">:</span>
+</span><span id="Git.delete_branch-156"><a href="#Git.delete_branch-156"><span class="linenos">156</span></a>            <span class="k">return</span> <span class="n">output</span> <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;origin --delete </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>  <span class="c1"># type:ignore</span>
+</span><span id="Git.delete_branch-157"><a href="#Git.delete_branch-157"><span class="linenos">157</span></a>        <span class="k">return</span> <span class="n">output</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Delete <code>branch_name</code> from repo.</p>
 
 <h4 id="params">:params:</h4>
 
@@ -1183,19 +1222,19 @@
         <span class="def">def</span>
         <span class="name">undo</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span></span><span class="return-annotation">) -> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span>:</span></span>
 
                 <label class="view-source-button" for="Git.undo-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Git.undo"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.undo-152"><a href="#Git.undo-152"><span class="linenos">152</span></a>    <span class="k">def</span> <span class="nf">undo</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git.undo-153"><a href="#Git.undo-153"><span class="linenos">153</span></a>        <span class="sd">&quot;&quot;&quot;Undo uncommitted changes.</span>
-</span><span id="Git.undo-154"><a href="#Git.undo-154"><span class="linenos">154</span></a>
-</span><span id="Git.undo-155"><a href="#Git.undo-155"><span class="linenos">155</span></a><span class="sd">        Equivalent to `git checkout .`.&quot;&quot;&quot;</span>
-</span><span id="Git.undo-156"><a href="#Git.undo-156"><span class="linenos">156</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">checkout</span><span class="p">(</span><span class="s2">&quot;.&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.undo-159"><a href="#Git.undo-159"><span class="linenos">159</span></a>    <span class="k">def</span> <span class="nf">undo</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git.undo-160"><a href="#Git.undo-160"><span class="linenos">160</span></a>        <span class="sd">&quot;&quot;&quot;Undo uncommitted changes.</span>
+</span><span id="Git.undo-161"><a href="#Git.undo-161"><span class="linenos">161</span></a>
+</span><span id="Git.undo-162"><a href="#Git.undo-162"><span class="linenos">162</span></a><span class="sd">        Equivalent to `git checkout .`.&quot;&quot;&quot;</span>
+</span><span id="Git.undo-163"><a href="#Git.undo-163"><span class="linenos">163</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">checkout</span><span class="p">(</span><span class="s2">&quot;.&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Undo uncommitted changes.</p>
 
 <p>Equivalent to <code>git checkout .</code>.</p>
 </div>
@@ -1209,17 +1248,17 @@
         <span class="def">def</span>
         <span class="name">merge</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">) -> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span>:</span></span>
 
                 <label class="view-source-button" for="Git.merge-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Git.merge"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.merge-158"><a href="#Git.merge-158"><span class="linenos">158</span></a>    <span class="k">def</span> <span class="nf">merge</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git.merge-159"><a href="#Git.merge-159"><span class="linenos">159</span></a>        <span class="sd">&quot;&quot;&quot;Merge branch `branch_name` with currently active branch.&quot;&quot;&quot;</span>
-</span><span id="Git.merge-160"><a href="#Git.merge-160"><span class="linenos">160</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;merge </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.merge-165"><a href="#Git.merge-165"><span class="linenos">165</span></a>    <span class="k">def</span> <span class="nf">merge</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git.merge-166"><a href="#Git.merge-166"><span class="linenos">166</span></a>        <span class="sd">&quot;&quot;&quot;Merge branch `branch_name` with currently active branch.&quot;&quot;&quot;</span>
+</span><span id="Git.merge-167"><a href="#Git.merge-167"><span class="linenos">167</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;merge </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Merge branch <code>branch_name</code> with currently active branch.</p>
 </div>
 
 
@@ -1231,24 +1270,24 @@
         <span class="def">def</span>
         <span class="name">create_remote</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">name</span><span class="p">:</span> <span class="nb">str</span>, </span><span class="param"><span class="n">public</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span></span><span class="return-annotation">) -> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span>:</span></span>
 
                 <label class="view-source-button" for="Git.create_remote-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Git.create_remote"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.create_remote-164"><a href="#Git.create_remote-164"><span class="linenos">164</span></a>    <span class="k">def</span> <span class="nf">create_remote</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">public</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git.create_remote-165"><a href="#Git.create_remote-165"><span class="linenos">165</span></a>        <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be installed and configured) to create a remote GitHub repo.</span>
-</span><span id="Git.create_remote-166"><a href="#Git.create_remote-166"><span class="linenos">166</span></a>
-</span><span id="Git.create_remote-167"><a href="#Git.create_remote-167"><span class="linenos">167</span></a><span class="sd">        #### :params:</span>
-</span><span id="Git.create_remote-168"><a href="#Git.create_remote-168"><span class="linenos">168</span></a>
-</span><span id="Git.create_remote-169"><a href="#Git.create_remote-169"><span class="linenos">169</span></a><span class="sd">        `name`: The name for the repo.</span>
-</span><span id="Git.create_remote-170"><a href="#Git.create_remote-170"><span class="linenos">170</span></a>
-</span><span id="Git.create_remote-171"><a href="#Git.create_remote-171"><span class="linenos">171</span></a><span class="sd">        `public`: Set to `True` to create the repo as public, otherwise it&#39;ll be created as private.&quot;&quot;&quot;</span>
-</span><span id="Git.create_remote-172"><a href="#Git.create_remote-172"><span class="linenos">172</span></a>        <span class="n">visibility</span> <span class="o">=</span> <span class="s2">&quot;--public&quot;</span> <span class="k">if</span> <span class="n">public</span> <span class="k">else</span> <span class="s2">&quot;--private&quot;</span>
-</span><span id="Git.create_remote-173"><a href="#Git.create_remote-173"><span class="linenos">173</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">([</span><span class="s2">&quot;gh&quot;</span><span class="p">,</span> <span class="s2">&quot;repo&quot;</span><span class="p">,</span> <span class="s2">&quot;create&quot;</span><span class="p">,</span> <span class="n">name</span><span class="p">,</span> <span class="n">visibility</span><span class="p">])</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.create_remote-171"><a href="#Git.create_remote-171"><span class="linenos">171</span></a>    <span class="k">def</span> <span class="nf">create_remote</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">public</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git.create_remote-172"><a href="#Git.create_remote-172"><span class="linenos">172</span></a>        <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be installed and configured) to create a remote GitHub repo.</span>
+</span><span id="Git.create_remote-173"><a href="#Git.create_remote-173"><span class="linenos">173</span></a>
+</span><span id="Git.create_remote-174"><a href="#Git.create_remote-174"><span class="linenos">174</span></a><span class="sd">        #### :params:</span>
+</span><span id="Git.create_remote-175"><a href="#Git.create_remote-175"><span class="linenos">175</span></a>
+</span><span id="Git.create_remote-176"><a href="#Git.create_remote-176"><span class="linenos">176</span></a><span class="sd">        `name`: The name for the repo.</span>
+</span><span id="Git.create_remote-177"><a href="#Git.create_remote-177"><span class="linenos">177</span></a>
+</span><span id="Git.create_remote-178"><a href="#Git.create_remote-178"><span class="linenos">178</span></a><span class="sd">        `public`: Set to `True` to create the repo as public, otherwise it&#39;ll be created as private.&quot;&quot;&quot;</span>
+</span><span id="Git.create_remote-179"><a href="#Git.create_remote-179"><span class="linenos">179</span></a>        <span class="n">visibility</span> <span class="o">=</span> <span class="s2">&quot;--public&quot;</span> <span class="k">if</span> <span class="n">public</span> <span class="k">else</span> <span class="s2">&quot;--private&quot;</span>
+</span><span id="Git.create_remote-180"><a href="#Git.create_remote-180"><span class="linenos">180</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">([</span><span class="s2">&quot;gh&quot;</span><span class="p">,</span> <span class="s2">&quot;repo&quot;</span><span class="p">,</span> <span class="s2">&quot;create&quot;</span><span class="p">,</span> <span class="n">name</span><span class="p">,</span> <span class="n">visibility</span><span class="p">])</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Uses GitHub CLI (must be installed and configured) to create a remote GitHub repo.</p>
 
 <h4 id="params">:params:</h4>
 
@@ -1266,25 +1305,25 @@
         <span class="def">def</span>
         <span class="name">create_remote_from_cwd</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">public</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span></span><span class="return-annotation">) -> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span>:</span></span>
 
                 <label class="view-source-button" for="Git.create_remote_from_cwd-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Git.create_remote_from_cwd"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.create_remote_from_cwd-175"><a href="#Git.create_remote_from_cwd-175"><span class="linenos">175</span></a>    <span class="k">def</span> <span class="nf">create_remote_from_cwd</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">public</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git.create_remote_from_cwd-176"><a href="#Git.create_remote_from_cwd-176"><span class="linenos">176</span></a>        <span class="sd">&quot;&quot;&quot;Use GitHub CLI (must be installed and configured) to create a remote GitHub repo from</span>
-</span><span id="Git.create_remote_from_cwd-177"><a href="#Git.create_remote_from_cwd-177"><span class="linenos">177</span></a><span class="sd">        the current working directory repo and add its url as this repo&#39;s remote origin.</span>
-</span><span id="Git.create_remote_from_cwd-178"><a href="#Git.create_remote_from_cwd-178"><span class="linenos">178</span></a>
-</span><span id="Git.create_remote_from_cwd-179"><a href="#Git.create_remote_from_cwd-179"><span class="linenos">179</span></a><span class="sd">        #### :params:</span>
-</span><span id="Git.create_remote_from_cwd-180"><a href="#Git.create_remote_from_cwd-180"><span class="linenos">180</span></a>
-</span><span id="Git.create_remote_from_cwd-181"><a href="#Git.create_remote_from_cwd-181"><span class="linenos">181</span></a><span class="sd">        `public`: Create the GitHub repo as a public repo, default is to create it as private.&quot;&quot;&quot;</span>
-</span><span id="Git.create_remote_from_cwd-182"><a href="#Git.create_remote_from_cwd-182"><span class="linenos">182</span></a>        <span class="n">visibility</span> <span class="o">=</span> <span class="s2">&quot;public&quot;</span> <span class="k">if</span> <span class="n">public</span> <span class="k">else</span> <span class="s2">&quot;private&quot;</span>
-</span><span id="Git.create_remote_from_cwd-183"><a href="#Git.create_remote_from_cwd-183"><span class="linenos">183</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">(</span>
-</span><span id="Git.create_remote_from_cwd-184"><a href="#Git.create_remote_from_cwd-184"><span class="linenos">184</span></a>            <span class="p">[</span><span class="s2">&quot;gh&quot;</span><span class="p">,</span> <span class="s2">&quot;repo&quot;</span><span class="p">,</span> <span class="s2">&quot;create&quot;</span><span class="p">,</span> <span class="s2">&quot;--source&quot;</span><span class="p">,</span> <span class="s2">&quot;.&quot;</span><span class="p">,</span> <span class="sa">f</span><span class="s2">&quot;--</span><span class="si">{</span><span class="n">visibility</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">,</span> <span class="s2">&quot;--push&quot;</span><span class="p">]</span>
-</span><span id="Git.create_remote_from_cwd-185"><a href="#Git.create_remote_from_cwd-185"><span class="linenos">185</span></a>        <span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.create_remote_from_cwd-182"><a href="#Git.create_remote_from_cwd-182"><span class="linenos">182</span></a>    <span class="k">def</span> <span class="nf">create_remote_from_cwd</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">public</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git.create_remote_from_cwd-183"><a href="#Git.create_remote_from_cwd-183"><span class="linenos">183</span></a>        <span class="sd">&quot;&quot;&quot;Use GitHub CLI (must be installed and configured) to create a remote GitHub repo from</span>
+</span><span id="Git.create_remote_from_cwd-184"><a href="#Git.create_remote_from_cwd-184"><span class="linenos">184</span></a><span class="sd">        the current working directory repo and add its url as this repo&#39;s remote origin.</span>
+</span><span id="Git.create_remote_from_cwd-185"><a href="#Git.create_remote_from_cwd-185"><span class="linenos">185</span></a>
+</span><span id="Git.create_remote_from_cwd-186"><a href="#Git.create_remote_from_cwd-186"><span class="linenos">186</span></a><span class="sd">        #### :params:</span>
+</span><span id="Git.create_remote_from_cwd-187"><a href="#Git.create_remote_from_cwd-187"><span class="linenos">187</span></a>
+</span><span id="Git.create_remote_from_cwd-188"><a href="#Git.create_remote_from_cwd-188"><span class="linenos">188</span></a><span class="sd">        `public`: Create the GitHub repo as a public repo, default is to create it as private.&quot;&quot;&quot;</span>
+</span><span id="Git.create_remote_from_cwd-189"><a href="#Git.create_remote_from_cwd-189"><span class="linenos">189</span></a>        <span class="n">visibility</span> <span class="o">=</span> <span class="s2">&quot;public&quot;</span> <span class="k">if</span> <span class="n">public</span> <span class="k">else</span> <span class="s2">&quot;private&quot;</span>
+</span><span id="Git.create_remote_from_cwd-190"><a href="#Git.create_remote_from_cwd-190"><span class="linenos">190</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">(</span>
+</span><span id="Git.create_remote_from_cwd-191"><a href="#Git.create_remote_from_cwd-191"><span class="linenos">191</span></a>            <span class="p">[</span><span class="s2">&quot;gh&quot;</span><span class="p">,</span> <span class="s2">&quot;repo&quot;</span><span class="p">,</span> <span class="s2">&quot;create&quot;</span><span class="p">,</span> <span class="s2">&quot;--source&quot;</span><span class="p">,</span> <span class="s2">&quot;.&quot;</span><span class="p">,</span> <span class="sa">f</span><span class="s2">&quot;--</span><span class="si">{</span><span class="n">visibility</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">,</span> <span class="s2">&quot;--push&quot;</span><span class="p">]</span>
+</span><span id="Git.create_remote_from_cwd-192"><a href="#Git.create_remote_from_cwd-192"><span class="linenos">192</span></a>        <span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Use GitHub CLI (must be installed and configured) to create a remote GitHub repo from
 the current working directory repo and add its url as this repo's remote origin.</p>
 
 <h4 id="params">:params:</h4>
@@ -1301,23 +1340,23 @@
         <span class="def">def</span>
         <span class="name">make_private</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">owner</span><span class="p">:</span> <span class="nb">str</span>, </span><span class="param"><span class="n">name</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">) -> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span>:</span></span>
 
                 <label class="view-source-button" for="Git.make_private-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Git.make_private"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.make_private-192"><a href="#Git.make_private-192"><span class="linenos">192</span></a>    <span class="k">def</span> <span class="nf">make_private</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git.make_private-193"><a href="#Git.make_private-193"><span class="linenos">193</span></a>        <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be installed and configured) to set the repo&#39;s visibility to private.</span>
-</span><span id="Git.make_private-194"><a href="#Git.make_private-194"><span class="linenos">194</span></a>
-</span><span id="Git.make_private-195"><a href="#Git.make_private-195"><span class="linenos">195</span></a><span class="sd">        #### :params:</span>
-</span><span id="Git.make_private-196"><a href="#Git.make_private-196"><span class="linenos">196</span></a>
-</span><span id="Git.make_private-197"><a href="#Git.make_private-197"><span class="linenos">197</span></a><span class="sd">        `owner`: The repo owner.</span>
-</span><span id="Git.make_private-198"><a href="#Git.make_private-198"><span class="linenos">198</span></a>
-</span><span id="Git.make_private-199"><a href="#Git.make_private-199"><span class="linenos">199</span></a><span class="sd">        `name`: The name of the repo to edit.&quot;&quot;&quot;</span>
-</span><span id="Git.make_private-200"><a href="#Git.make_private-200"><span class="linenos">200</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_change_visibility</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">name</span><span class="p">,</span> <span class="s2">&quot;private&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.make_private-199"><a href="#Git.make_private-199"><span class="linenos">199</span></a>    <span class="k">def</span> <span class="nf">make_private</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git.make_private-200"><a href="#Git.make_private-200"><span class="linenos">200</span></a>        <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be installed and configured) to set the repo&#39;s visibility to private.</span>
+</span><span id="Git.make_private-201"><a href="#Git.make_private-201"><span class="linenos">201</span></a>
+</span><span id="Git.make_private-202"><a href="#Git.make_private-202"><span class="linenos">202</span></a><span class="sd">        #### :params:</span>
+</span><span id="Git.make_private-203"><a href="#Git.make_private-203"><span class="linenos">203</span></a>
+</span><span id="Git.make_private-204"><a href="#Git.make_private-204"><span class="linenos">204</span></a><span class="sd">        `owner`: The repo owner.</span>
+</span><span id="Git.make_private-205"><a href="#Git.make_private-205"><span class="linenos">205</span></a>
+</span><span id="Git.make_private-206"><a href="#Git.make_private-206"><span class="linenos">206</span></a><span class="sd">        `name`: The name of the repo to edit.&quot;&quot;&quot;</span>
+</span><span id="Git.make_private-207"><a href="#Git.make_private-207"><span class="linenos">207</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_change_visibility</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">name</span><span class="p">,</span> <span class="s2">&quot;private&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Uses GitHub CLI (must be installed and configured) to set the repo's visibility to private.</p>
 
 <h4 id="params">:params:</h4>
 
@@ -1335,23 +1374,23 @@
         <span class="def">def</span>
         <span class="name">make_public</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">owner</span><span class="p">:</span> <span class="nb">str</span>, </span><span class="param"><span class="n">name</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">) -> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span>:</span></span>
 
                 <label class="view-source-button" for="Git.make_public-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Git.make_public"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.make_public-202"><a href="#Git.make_public-202"><span class="linenos">202</span></a>    <span class="k">def</span> <span class="nf">make_public</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git.make_public-203"><a href="#Git.make_public-203"><span class="linenos">203</span></a>        <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be installed and configured) to set the repo&#39;s visibility to public.</span>
-</span><span id="Git.make_public-204"><a href="#Git.make_public-204"><span class="linenos">204</span></a>
-</span><span id="Git.make_public-205"><a href="#Git.make_public-205"><span class="linenos">205</span></a><span class="sd">        #### :params:</span>
-</span><span id="Git.make_public-206"><a href="#Git.make_public-206"><span class="linenos">206</span></a>
-</span><span id="Git.make_public-207"><a href="#Git.make_public-207"><span class="linenos">207</span></a><span class="sd">        `owner`: The repo owner.</span>
-</span><span id="Git.make_public-208"><a href="#Git.make_public-208"><span class="linenos">208</span></a>
-</span><span id="Git.make_public-209"><a href="#Git.make_public-209"><span class="linenos">209</span></a><span class="sd">        `name`: The name of the repo to edit.&quot;&quot;&quot;</span>
-</span><span id="Git.make_public-210"><a href="#Git.make_public-210"><span class="linenos">210</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_change_visibility</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">name</span><span class="p">,</span> <span class="s2">&quot;public&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.make_public-209"><a href="#Git.make_public-209"><span class="linenos">209</span></a>    <span class="k">def</span> <span class="nf">make_public</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git.make_public-210"><a href="#Git.make_public-210"><span class="linenos">210</span></a>        <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be installed and configured) to set the repo&#39;s visibility to public.</span>
+</span><span id="Git.make_public-211"><a href="#Git.make_public-211"><span class="linenos">211</span></a>
+</span><span id="Git.make_public-212"><a href="#Git.make_public-212"><span class="linenos">212</span></a><span class="sd">        #### :params:</span>
+</span><span id="Git.make_public-213"><a href="#Git.make_public-213"><span class="linenos">213</span></a>
+</span><span id="Git.make_public-214"><a href="#Git.make_public-214"><span class="linenos">214</span></a><span class="sd">        `owner`: The repo owner.</span>
+</span><span id="Git.make_public-215"><a href="#Git.make_public-215"><span class="linenos">215</span></a>
+</span><span id="Git.make_public-216"><a href="#Git.make_public-216"><span class="linenos">216</span></a><span class="sd">        `name`: The name of the repo to edit.&quot;&quot;&quot;</span>
+</span><span id="Git.make_public-217"><a href="#Git.make_public-217"><span class="linenos">217</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_change_visibility</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">name</span><span class="p">,</span> <span class="s2">&quot;public&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Uses GitHub CLI (must be installed and configured) to set the repo's visibility to public.</p>
 
 <h4 id="params">:params:</h4>
 
@@ -1369,23 +1408,23 @@
         <span class="def">def</span>
         <span class="name">delete_remote</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">owner</span><span class="p">:</span> <span class="nb">str</span>, </span><span class="param"><span class="n">name</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">) -> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span>:</span></span>
 
                 <label class="view-source-button" for="Git.delete_remote-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Git.delete_remote"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.delete_remote-212"><a href="#Git.delete_remote-212"><span class="linenos">212</span></a>    <span class="k">def</span> <span class="nf">delete_remote</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git.delete_remote-213"><a href="#Git.delete_remote-213"><span class="linenos">213</span></a>        <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be isntalled and configured) to delete the remote for this repo.</span>
-</span><span id="Git.delete_remote-214"><a href="#Git.delete_remote-214"><span class="linenos">214</span></a>
-</span><span id="Git.delete_remote-215"><a href="#Git.delete_remote-215"><span class="linenos">215</span></a><span class="sd">        #### :params:</span>
-</span><span id="Git.delete_remote-216"><a href="#Git.delete_remote-216"><span class="linenos">216</span></a>
-</span><span id="Git.delete_remote-217"><a href="#Git.delete_remote-217"><span class="linenos">217</span></a><span class="sd">        `owner`: The repo owner.</span>
-</span><span id="Git.delete_remote-218"><a href="#Git.delete_remote-218"><span class="linenos">218</span></a>
-</span><span id="Git.delete_remote-219"><a href="#Git.delete_remote-219"><span class="linenos">219</span></a><span class="sd">        `name`: The name of the remote repo to delete.&quot;&quot;&quot;</span>
-</span><span id="Git.delete_remote-220"><a href="#Git.delete_remote-220"><span class="linenos">220</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">([</span><span class="s2">&quot;gh&quot;</span><span class="p">,</span> <span class="s2">&quot;repo&quot;</span><span class="p">,</span> <span class="s2">&quot;delete&quot;</span><span class="p">,</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">owner</span><span class="si">}</span><span class="s2">/</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">,</span> <span class="s2">&quot;--yes&quot;</span><span class="p">])</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.delete_remote-219"><a href="#Git.delete_remote-219"><span class="linenos">219</span></a>    <span class="k">def</span> <span class="nf">delete_remote</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git.delete_remote-220"><a href="#Git.delete_remote-220"><span class="linenos">220</span></a>        <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be isntalled and configured) to delete the remote for this repo.</span>
+</span><span id="Git.delete_remote-221"><a href="#Git.delete_remote-221"><span class="linenos">221</span></a>
+</span><span id="Git.delete_remote-222"><a href="#Git.delete_remote-222"><span class="linenos">222</span></a><span class="sd">        #### :params:</span>
+</span><span id="Git.delete_remote-223"><a href="#Git.delete_remote-223"><span class="linenos">223</span></a>
+</span><span id="Git.delete_remote-224"><a href="#Git.delete_remote-224"><span class="linenos">224</span></a><span class="sd">        `owner`: The repo owner.</span>
+</span><span id="Git.delete_remote-225"><a href="#Git.delete_remote-225"><span class="linenos">225</span></a>
+</span><span id="Git.delete_remote-226"><a href="#Git.delete_remote-226"><span class="linenos">226</span></a><span class="sd">        `name`: The name of the remote repo to delete.&quot;&quot;&quot;</span>
+</span><span id="Git.delete_remote-227"><a href="#Git.delete_remote-227"><span class="linenos">227</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">([</span><span class="s2">&quot;gh&quot;</span><span class="p">,</span> <span class="s2">&quot;repo&quot;</span><span class="p">,</span> <span class="s2">&quot;delete&quot;</span><span class="p">,</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">owner</span><span class="si">}</span><span class="s2">/</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">,</span> <span class="s2">&quot;--yes&quot;</span><span class="p">])</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Uses GitHub CLI (must be isntalled and configured) to delete the remote for this repo.</p>
 
 <h4 id="params">:params:</h4>
```

#### html2text {}

```diff
@@ -2,14 +2,15 @@
 
   ⁰
 ____ gitbetter [Unknown INPUT type]
 ***** API Documentation *****
     * Git
           o Git
           o capture_stdout
+          o capture_output
           o execute
           o new_repo
           o loggy
           o status
           o commit
           o add
           o commit_files
@@ -36,816 +37,837 @@
           o delete_remote
 built_with_pdoc[pdoc_logo]
 
 ****** gitbetter.git ******
 ⁰ View Source
 __1import shlex
 __2import subprocess
-__3
+__3from contextlib import contextmanager
 __4
-__5class Git:
-__6    def __init__(self, capture_stdout: bool = False):
-__7        """If `capture_stdout` is `True`, all functions will return their
+__5
+__6class Git:
+__7    def __init__(self, capture_stdout: bool = False):
+__8        """If `capture_stdout` is `True`, all functions will return their
 generated `stdout` as a string.
-__8        Otherwise, the functions return the call's exit code."""
-__9        self.capture_stdout = capture_stdout
-_10
-_11    @property
-_12    def capture_stdout(self) -> bool:
-_13        """If `True`, member functions will return the generated `stdout` as
+__9        Otherwise, the functions return the call's exit code."""
+_10        self.capture_stdout = capture_stdout
+_11
+_12    @contextmanager
+_13    def capture_output(self):
+_14        self.capture_stdout = True
+_15        yield self
+_16        self.capture_stdout = False
+_17
+_18    @property
+_19    def capture_stdout(self) -> bool:
+_20        """If `True`, member functions will return the generated `stdout` as
 a string,
-_14        otherwise they return the command's exit code."""
-_15        return self._capture_stdout
-_16
-_17    @capture_stdout.setter
-_18    def capture_stdout(self, should_capture: bool):
-_19        self._capture_stdout = should_capture
-_20
-_21    def _run(self, args: list[str]) -> str | int:
-_22        if self._capture_stdout:
-_23            return subprocess.run(args, stdout=subprocess.PIPE,
+_21        otherwise they return the command's exit code."""
+_22        return self._capture_stdout
+_23
+_24    @capture_stdout.setter
+_25    def capture_stdout(self, should_capture: bool):
+_26        self._capture_stdout = should_capture
+_27
+_28    def _run(self, args: list[str]) -> str | int:
+_29        if self._capture_stdout:
+_30            return subprocess.run(args, stdout=subprocess.PIPE,
 text=True).stdout
-_24        else:
-_25            return subprocess.run(args).returncode
-_26
-_27    def execute(self, command: str) -> str | int:
-_28        """Execute git command.
-_29
-_30        Equivalent to executing `git {command}` in the shell."""
-_31        args = ["git"] + shlex.split(command)
-_32        return self._run(args)
+_31        else:
+_32            return subprocess.run(args).returncode
 _33
-_34    def new_repo(self) -> str | int:
-_35        """Executes `git init -b main`."""
-_36        return self.execute("init -b main")
-_37
-_38    def loggy(self) -> str | int:
-_39        """Equivalent to `git log --oneline --name-only --abbrev-commit --
+_34    def execute(self, command: str) -> str | int:
+_35        """Execute git command.
+_36
+_37        Equivalent to executing `git {command}` in the shell."""
+_38        args = ["git"] + shlex.split(command)
+_39        return self._run(args)
+_40
+_41    def new_repo(self) -> str | int:
+_42        """Executes `git init -b main`."""
+_43        return self.execute("init -b main")
+_44
+_45    def loggy(self) -> str | int:
+_46        """Equivalent to `git log --oneline --name-only --abbrev-commit --
 graph`."""
-_40        return self.execute("log --oneline --name-only --abbrev-commit --
+_47        return self.execute("log --oneline --name-only --abbrev-commit --
 graph")
-_41
-_42    def status(self) -> str | int:
-_43        """Execute `git status`."""
-_44        return self.execute("status")
-_45
-_46    # ======================================Staging/
+_48
+_49    def status(self) -> str | int:
+_50        """Execute `git status`."""
+_51        return self.execute("status")
+_52
+_53    # ======================================Staging/
 Committing======================================
-_47    def commit(self, args: str) -> str | int:
-_48        """>>> git commit {args}"""
-_49        return self.execute(f"commit {args}")
-_50
-_51    def add(self, files: list[str] | None = None) -> str | int:
-_52        """Stage a list of files.
-_53
-_54        If no files are given (`files=None`), all files will be staged."""
-_55        if not files:
-_56            return self.execute("add .")
-_57        else:
-_58            files = " ".join(f'"{file}"' for file in files)  # type: ignore
-_59            return self.execute(f"add {files}")
+_54    def commit(self, args: str) -> str | int:
+_55        """>>> git commit {args}"""
+_56        return self.execute(f"commit {args}")
+_57
+_58    def add(self, files: list[str] | None = None) -> str | int:
+_59        """Stage a list of files.
 _60
-_61    def commit_files(self, files: list[str], message: str) -> str | int:
-_62        """Stage and commit a list of files with commit message
+_61        If no files are given (`files=None`), all files will be staged."""
+_62        if not files:
+_63            return self.execute("add .")
+_64        else:
+_65            files = " ".join(f'"{file}"' for file in files)  # type: ignore
+_66            return self.execute(f"add {files}")
+_67
+_68    def commit_files(self, files: list[str], message: str) -> str | int:
+_69        """Stage and commit a list of files with commit message
 `message`."""
-_63        return self.add(files) + self.commit(f'-m "{message}"')  # type:
+_70        return self.add(files) + self.commit(f'-m "{message}"')  # type:
 ignore
-_64
-_65    def initcommit(self) -> str | int:
-_66        """Equivalent to
-_67        >>> git add .
-_68        >>> git commit -m "Initial commit" """
-_69        return self.add() + self.commit('-m "Initial commit"')  # type:
+_71
+_72    def initcommit(self) -> str | int:
+_73        """Equivalent to
+_74        >>> git add .
+_75        >>> git commit -m "Initial commit" """
+_76        return self.add() + self.commit('-m "Initial commit"')  # type:
 ignore
-_70
-_71    def amend(self, files: list[str] | None = None) -> str | int:
-_72        """Stage and commit changes to the previous commit.
-_73
-_74        If `files` is `None`, all files will be staged.
-_75
-_76        Equivalent to:
-_77        >>> git add {files}
-_78        >>> git commit --amend --no-edit
-_79        """
-_80        return self.add(files) + self.commit("--amend --no-edit")  # type:
+_77
+_78    def amend(self, files: list[str] | None = None) -> str | int:
+_79        """Stage and commit changes to the previous commit.
+_80
+_81        If `files` is `None`, all files will be staged.
+_82
+_83        Equivalent to:
+_84        >>> git add {files}
+_85        >>> git commit --amend --no-edit
+_86        """
+_87        return self.add(files) + self.commit("--amend --no-edit")  # type:
 ignore
-_81
-_82    def tag(self, args: str = "") -> str | int:
-_83        """Execute the `tag` command with `args`.
-_84
-_85        e.g.
-_86
-_87        `self.tag("--sort=-committerdate")`
 _88
-_89        will list all the tags for this repository in descending commit
-date."""
-_90        return self.execute(f"tag {args}")
+_89    def tag(self, args: str = "") -> str | int:
+_90        """Execute the `tag` command with `args`.
 _91
-_92    # ==========================================Push/
+_92        e.g.
+_93
+_94        `self.tag("--sort=-committerdate")`
+_95
+_96        will list all the tags for this repository in descending commit
+date."""
+_97        return self.execute(f"tag {args}")
+_98
+_99    # ==========================================Push/
 Pull==========================================
-_93    def add_remote_url(self, url: str, name: str = "origin") -> str | int:
-_94        """Add remote url to repo."""
-_95        return self.execute(f"remote add {name} {url}")
-_96
-_97    def push(self, args: str = "") -> str | int:
-_98        """Equivalent to `git push {args}`."""
-_99        return self.execute(f"push {args}")
-100
-101    def pull(self, args: str = "") -> str | int:
-102        """Equivalent to `git pull {args}`."""
-103        return self.execute(f"pull {args}")
-104
-105    def push_new_branch(self, branch: str) -> str | int:
-106        """Push a new branch to origin with tracking.
+100    def add_remote_url(self, url: str, name: str = "origin") -> str | int:
+101        """Add remote url to repo."""
+102        return self.execute(f"remote add {name} {url}")
+103
+104    def push(self, args: str = "") -> str | int:
+105        """Equivalent to `git push {args}`."""
+106        return self.execute(f"push {args}")
 107
-108        Equivalent to `git push -u origin {branch}`."""
-109        return self.push(f"-u origin {branch}")
-110
-111    def pull_branch(self, branch: str) -> str | int:
-112        """Pull `branch` from origin."""
-113        return self.pull(f"origin {branch}")
+108    def pull(self, args: str = "") -> str | int:
+109        """Equivalent to `git pull {args}`."""
+110        return self.execute(f"pull {args}")
+111
+112    def push_new_branch(self, branch: str) -> str | int:
+113        """Push a new branch to origin with tracking.
 114
-115    # ============================================Checkout/
+115        Equivalent to `git push -u origin {branch}`."""
+116        return self.push(f"-u origin {branch}")
+117
+118    def pull_branch(self, branch: str) -> str | int:
+119        """Pull `branch` from origin."""
+120        return self.pull(f"origin {branch}")
+121
+122    # ============================================Checkout/
 Branches============================================
-116    def branch(self, args: str) -> str | int:
-117        """Equivalent to `git branch {args}`."""
-118        return self.execute(f"branch {args}")
-119
-120    def list_branches(self) -> str | int:
-121        """Print a list of branches."""
-122        return self.branch("-vva")
-123
-124    def checkout(self, args: str) -> str | int:
-125        """Equivalent to `git checkout {args}`."""
-126        return self.execute(f"checkout {args}")
-127
-128    def switch_branch(self, branch_name: str) -> str | int:
-129        """Switch to the branch specified by `branch_name`.
+123    def branch(self, args: str) -> str | int:
+124        """Equivalent to `git branch {args}`."""
+125        return self.execute(f"branch {args}")
+126
+127    def list_branches(self) -> str | int:
+128        """Print a list of branches."""
+129        return self.branch("-vva")
 130
-131        Equivalent to `git checkout {branch_name}`."""
-132        return self.checkout(branch_name)
-133
-134    def create_new_branch(self, branch_name: str) -> str | int:
-135        """Create and switch to a new branch named with `branch_name`.
-136
-137        Equivalent to `git checkout -b {branch_name} --track`."""
-138        return self.checkout(f"-b {branch_name} --track")
-139
-140    def delete_branch(self, branch_name: str, local_only: bool = True) -
+131    def checkout(self, args: str) -> str | int:
+132        """Equivalent to `git checkout {args}`."""
+133        return self.execute(f"checkout {args}")
+134
+135    def switch_branch(self, branch_name: str) -> str | int:
+136        """Switch to the branch specified by `branch_name`.
+137
+138        Equivalent to `git checkout {branch_name}`."""
+139        return self.checkout(branch_name)
+140
+141    def create_new_branch(self, branch_name: str) -> str | int:
+142        """Create and switch to a new branch named with `branch_name`.
+143
+144        Equivalent to `git checkout -b {branch_name} --track`."""
+145        return self.checkout(f"-b {branch_name} --track")
+146
+147    def delete_branch(self, branch_name: str, local_only: bool = True) -
 > str | int:
-141        """Delete `branch_name` from repo.
-142
-143        #### :params:
-144
-145        `local_only`: Only delete the local copy of `branch`, otherwise also
+148        """Delete `branch_name` from repo.
+149
+150        #### :params:
+151
+152        `local_only`: Only delete the local copy of `branch`, otherwise also
 delete the remote branch on origin and remote-tracking branch."""
-146        output = self.branch(f"--delete {branch_name}")
-147        if not local_only:
-148            return output + self.push(f"origin --delete {branch_name}")  #
+153        output = self.branch(f"--delete {branch_name}")
+154        if not local_only:
+155            return output + self.push(f"origin --delete {branch_name}")  #
 type:ignore
-149        return output
-150
-151    def undo(self) -> str | int:
-152        """Undo uncommitted changes.
-153
-154        Equivalent to `git checkout .`."""
-155        return self.checkout(".")
-156
-157    def merge(self, branch_name: str) -> str | int:
-158        """Merge branch `branch_name` with currently active branch."""
-159        return self.execute(f"merge {branch_name}")
+156        return output
+157
+158    def undo(self) -> str | int:
+159        """Undo uncommitted changes.
 160
-161    # ===============================Requires GitHub CLI to be installed and
-configured===============================
-162
-163    def create_remote(self, name: str, public: bool = False) -> str | int:
-164        """Uses GitHub CLI (must be installed and configured) to create a
-remote GitHub repo.
-165
-166        #### :params:
+161        Equivalent to `git checkout .`."""
+162        return self.checkout(".")
+163
+164    def merge(self, branch_name: str) -> str | int:
+165        """Merge branch `branch_name` with currently active branch."""
+166        return self.execute(f"merge {branch_name}")
 167
-168        `name`: The name for the repo.
+168    # ===============================Requires GitHub CLI to be installed and
+configured===============================
 169
-170        `public`: Set to `True` to create the repo as public, otherwise
+170    def create_remote(self, name: str, public: bool = False) -> str | int:
+171        """Uses GitHub CLI (must be installed and configured) to create a
+remote GitHub repo.
+172
+173        #### :params:
+174
+175        `name`: The name for the repo.
+176
+177        `public`: Set to `True` to create the repo as public, otherwise
 it'll be created as private."""
-171        visibility = "--public" if public else "--private"
-172        return self._run(["gh", "repo", "create", name, visibility])
-173
-174    def create_remote_from_cwd(self, public: bool = False) -> str | int:
-175        """Use GitHub CLI (must be installed and configured) to create a
+178        visibility = "--public" if public else "--private"
+179        return self._run(["gh", "repo", "create", name, visibility])
+180
+181    def create_remote_from_cwd(self, public: bool = False) -> str | int:
+182        """Use GitHub CLI (must be installed and configured) to create a
 remote GitHub repo from
-176        the current working directory repo and add its url as this repo's
+183        the current working directory repo and add its url as this repo's
 remote origin.
-177
-178        #### :params:
-179
-180        `public`: Create the GitHub repo as a public repo, default is to
+184
+185        #### :params:
+186
+187        `public`: Create the GitHub repo as a public repo, default is to
 create it as private."""
-181        visibility = "public" if public else "private"
-182        return self._run(
-183            ["gh", "repo", "create", "--source", ".", f"--{visibility}", "--
+188        visibility = "public" if public else "private"
+189        return self._run(
+190            ["gh", "repo", "create", "--source", ".", f"--{visibility}", "--
 push"]
-184        )
-185
-186    def _change_visibility(self, owner: str, name: str, visibility: str) -
+191        )
+192
+193    def _change_visibility(self, owner: str, name: str, visibility: str) -
 > str | int:
-187        return self._run(
-188            ["gh", "repo", "edit", f"{owner}/{name}", "--visibility",
+194        return self._run(
+195            ["gh", "repo", "edit", f"{owner}/{name}", "--visibility",
 visibility]
-189        )
-190
-191    def make_private(self, owner: str, name: str) -> str | int:
-192        """Uses GitHub CLI (must be installed and configured) to set the
-repo's visibility to private.
-193
-194        #### :params:
-195
-196        `owner`: The repo owner.
+196        )
 197
-198        `name`: The name of the repo to edit."""
-199        return self._change_visibility(owner, name, "private")
+198    def make_private(self, owner: str, name: str) -> str | int:
+199        """Uses GitHub CLI (must be installed and configured) to set the
+repo's visibility to private.
 200
-201    def make_public(self, owner: str, name: str) -> str | int:
-202        """Uses GitHub CLI (must be installed and configured) to set the
-repo's visibility to public.
-203
-204        #### :params:
-205
-206        `owner`: The repo owner.
+201        #### :params:
+202
+203        `owner`: The repo owner.
+204
+205        `name`: The name of the repo to edit."""
+206        return self._change_visibility(owner, name, "private")
 207
-208        `name`: The name of the repo to edit."""
-209        return self._change_visibility(owner, name, "public")
+208    def make_public(self, owner: str, name: str) -> str | int:
+209        """Uses GitHub CLI (must be installed and configured) to set the
+repo's visibility to public.
 210
-211    def delete_remote(self, owner: str, name: str) -> str | int:
-212        """Uses GitHub CLI (must be isntalled and configured) to delete the
-remote for this repo.
-213
-214        #### :params:
-215
-216        `owner`: The repo owner.
+211        #### :params:
+212
+213        `owner`: The repo owner.
+214
+215        `name`: The name of the repo to edit."""
+216        return self._change_visibility(owner, name, "public")
 217
-218        `name`: The name of the remote repo to delete."""
-219        return self._run(["gh", "repo", "delete", f"{owner}/{name}", "--
+218    def delete_remote(self, owner: str, name: str) -> str | int:
+219        """Uses GitHub CLI (must be isntalled and configured) to delete the
+remote for this repo.
+220
+221        #### :params:
+222
+223        `owner`: The repo owner.
+224
+225        `name`: The name of the remote repo to delete."""
+226        return self._run(["gh", "repo", "delete", f"{owner}/{name}", "--
 yes"])
   ⁰
 class Git: View Source
-__6class Git:
-__7    def __init__(self, capture_stdout: bool = False):
-__8        """If `capture_stdout` is `True`, all functions will return their
+__7class Git:
+__8    def __init__(self, capture_stdout: bool = False):
+__9        """If `capture_stdout` is `True`, all functions will return their
 generated `stdout` as a string.
-__9        Otherwise, the functions return the call's exit code."""
-_10        self.capture_stdout = capture_stdout
-_11
-_12    @property
-_13    def capture_stdout(self) -> bool:
-_14        """If `True`, member functions will return the generated `stdout` as
+_10        Otherwise, the functions return the call's exit code."""
+_11        self.capture_stdout = capture_stdout
+_12
+_13    @contextmanager
+_14    def capture_output(self):
+_15        self.capture_stdout = True
+_16        yield self
+_17        self.capture_stdout = False
+_18
+_19    @property
+_20    def capture_stdout(self) -> bool:
+_21        """If `True`, member functions will return the generated `stdout` as
 a string,
-_15        otherwise they return the command's exit code."""
-_16        return self._capture_stdout
-_17
-_18    @capture_stdout.setter
-_19    def capture_stdout(self, should_capture: bool):
-_20        self._capture_stdout = should_capture
-_21
-_22    def _run(self, args: list[str]) -> str | int:
-_23        if self._capture_stdout:
-_24            return subprocess.run(args, stdout=subprocess.PIPE,
+_22        otherwise they return the command's exit code."""
+_23        return self._capture_stdout
+_24
+_25    @capture_stdout.setter
+_26    def capture_stdout(self, should_capture: bool):
+_27        self._capture_stdout = should_capture
+_28
+_29    def _run(self, args: list[str]) -> str | int:
+_30        if self._capture_stdout:
+_31            return subprocess.run(args, stdout=subprocess.PIPE,
 text=True).stdout
-_25        else:
-_26            return subprocess.run(args).returncode
-_27
-_28    def execute(self, command: str) -> str | int:
-_29        """Execute git command.
-_30
-_31        Equivalent to executing `git {command}` in the shell."""
-_32        args = ["git"] + shlex.split(command)
-_33        return self._run(args)
+_32        else:
+_33            return subprocess.run(args).returncode
 _34
-_35    def new_repo(self) -> str | int:
-_36        """Executes `git init -b main`."""
-_37        return self.execute("init -b main")
-_38
-_39    def loggy(self) -> str | int:
-_40        """Equivalent to `git log --oneline --name-only --abbrev-commit --
+_35    def execute(self, command: str) -> str | int:
+_36        """Execute git command.
+_37
+_38        Equivalent to executing `git {command}` in the shell."""
+_39        args = ["git"] + shlex.split(command)
+_40        return self._run(args)
+_41
+_42    def new_repo(self) -> str | int:
+_43        """Executes `git init -b main`."""
+_44        return self.execute("init -b main")
+_45
+_46    def loggy(self) -> str | int:
+_47        """Equivalent to `git log --oneline --name-only --abbrev-commit --
 graph`."""
-_41        return self.execute("log --oneline --name-only --abbrev-commit --
+_48        return self.execute("log --oneline --name-only --abbrev-commit --
 graph")
-_42
-_43    def status(self) -> str | int:
-_44        """Execute `git status`."""
-_45        return self.execute("status")
-_46
-_47    # ======================================Staging/
+_49
+_50    def status(self) -> str | int:
+_51        """Execute `git status`."""
+_52        return self.execute("status")
+_53
+_54    # ======================================Staging/
 Committing======================================
-_48    def commit(self, args: str) -> str | int:
-_49        """>>> git commit {args}"""
-_50        return self.execute(f"commit {args}")
-_51
-_52    def add(self, files: list[str] | None = None) -> str | int:
-_53        """Stage a list of files.
-_54
-_55        If no files are given (`files=None`), all files will be staged."""
-_56        if not files:
-_57            return self.execute("add .")
-_58        else:
-_59            files = " ".join(f'"{file}"' for file in files)  # type: ignore
-_60            return self.execute(f"add {files}")
+_55    def commit(self, args: str) -> str | int:
+_56        """>>> git commit {args}"""
+_57        return self.execute(f"commit {args}")
+_58
+_59    def add(self, files: list[str] | None = None) -> str | int:
+_60        """Stage a list of files.
 _61
-_62    def commit_files(self, files: list[str], message: str) -> str | int:
-_63        """Stage and commit a list of files with commit message
+_62        If no files are given (`files=None`), all files will be staged."""
+_63        if not files:
+_64            return self.execute("add .")
+_65        else:
+_66            files = " ".join(f'"{file}"' for file in files)  # type: ignore
+_67            return self.execute(f"add {files}")
+_68
+_69    def commit_files(self, files: list[str], message: str) -> str | int:
+_70        """Stage and commit a list of files with commit message
 `message`."""
-_64        return self.add(files) + self.commit(f'-m "{message}"')  # type:
+_71        return self.add(files) + self.commit(f'-m "{message}"')  # type:
 ignore
-_65
-_66    def initcommit(self) -> str | int:
-_67        """Equivalent to
-_68        >>> git add .
-_69        >>> git commit -m "Initial commit" """
-_70        return self.add() + self.commit('-m "Initial commit"')  # type:
+_72
+_73    def initcommit(self) -> str | int:
+_74        """Equivalent to
+_75        >>> git add .
+_76        >>> git commit -m "Initial commit" """
+_77        return self.add() + self.commit('-m "Initial commit"')  # type:
 ignore
-_71
-_72    def amend(self, files: list[str] | None = None) -> str | int:
-_73        """Stage and commit changes to the previous commit.
-_74
-_75        If `files` is `None`, all files will be staged.
-_76
-_77        Equivalent to:
-_78        >>> git add {files}
-_79        >>> git commit --amend --no-edit
-_80        """
-_81        return self.add(files) + self.commit("--amend --no-edit")  # type:
+_78
+_79    def amend(self, files: list[str] | None = None) -> str | int:
+_80        """Stage and commit changes to the previous commit.
+_81
+_82        If `files` is `None`, all files will be staged.
+_83
+_84        Equivalent to:
+_85        >>> git add {files}
+_86        >>> git commit --amend --no-edit
+_87        """
+_88        return self.add(files) + self.commit("--amend --no-edit")  # type:
 ignore
-_82
-_83    def tag(self, args: str = "") -> str | int:
-_84        """Execute the `tag` command with `args`.
-_85
-_86        e.g.
-_87
-_88        `self.tag("--sort=-committerdate")`
 _89
-_90        will list all the tags for this repository in descending commit
-date."""
-_91        return self.execute(f"tag {args}")
+_90    def tag(self, args: str = "") -> str | int:
+_91        """Execute the `tag` command with `args`.
 _92
-_93    # ==========================================Push/
+_93        e.g.
+_94
+_95        `self.tag("--sort=-committerdate")`
+_96
+_97        will list all the tags for this repository in descending commit
+date."""
+_98        return self.execute(f"tag {args}")
+_99
+100    # ==========================================Push/
 Pull==========================================
-_94    def add_remote_url(self, url: str, name: str = "origin") -> str | int:
-_95        """Add remote url to repo."""
-_96        return self.execute(f"remote add {name} {url}")
-_97
-_98    def push(self, args: str = "") -> str | int:
-_99        """Equivalent to `git push {args}`."""
-100        return self.execute(f"push {args}")
-101
-102    def pull(self, args: str = "") -> str | int:
-103        """Equivalent to `git pull {args}`."""
-104        return self.execute(f"pull {args}")
-105
-106    def push_new_branch(self, branch: str) -> str | int:
-107        """Push a new branch to origin with tracking.
+101    def add_remote_url(self, url: str, name: str = "origin") -> str | int:
+102        """Add remote url to repo."""
+103        return self.execute(f"remote add {name} {url}")
+104
+105    def push(self, args: str = "") -> str | int:
+106        """Equivalent to `git push {args}`."""
+107        return self.execute(f"push {args}")
 108
-109        Equivalent to `git push -u origin {branch}`."""
-110        return self.push(f"-u origin {branch}")
-111
-112    def pull_branch(self, branch: str) -> str | int:
-113        """Pull `branch` from origin."""
-114        return self.pull(f"origin {branch}")
+109    def pull(self, args: str = "") -> str | int:
+110        """Equivalent to `git pull {args}`."""
+111        return self.execute(f"pull {args}")
+112
+113    def push_new_branch(self, branch: str) -> str | int:
+114        """Push a new branch to origin with tracking.
 115
-116    # ============================================Checkout/
+116        Equivalent to `git push -u origin {branch}`."""
+117        return self.push(f"-u origin {branch}")
+118
+119    def pull_branch(self, branch: str) -> str | int:
+120        """Pull `branch` from origin."""
+121        return self.pull(f"origin {branch}")
+122
+123    # ============================================Checkout/
 Branches============================================
-117    def branch(self, args: str) -> str | int:
-118        """Equivalent to `git branch {args}`."""
-119        return self.execute(f"branch {args}")
-120
-121    def list_branches(self) -> str | int:
-122        """Print a list of branches."""
-123        return self.branch("-vva")
-124
-125    def checkout(self, args: str) -> str | int:
-126        """Equivalent to `git checkout {args}`."""
-127        return self.execute(f"checkout {args}")
-128
-129    def switch_branch(self, branch_name: str) -> str | int:
-130        """Switch to the branch specified by `branch_name`.
+124    def branch(self, args: str) -> str | int:
+125        """Equivalent to `git branch {args}`."""
+126        return self.execute(f"branch {args}")
+127
+128    def list_branches(self) -> str | int:
+129        """Print a list of branches."""
+130        return self.branch("-vva")
 131
-132        Equivalent to `git checkout {branch_name}`."""
-133        return self.checkout(branch_name)
-134
-135    def create_new_branch(self, branch_name: str) -> str | int:
-136        """Create and switch to a new branch named with `branch_name`.
-137
-138        Equivalent to `git checkout -b {branch_name} --track`."""
-139        return self.checkout(f"-b {branch_name} --track")
-140
-141    def delete_branch(self, branch_name: str, local_only: bool = True) -
+132    def checkout(self, args: str) -> str | int:
+133        """Equivalent to `git checkout {args}`."""
+134        return self.execute(f"checkout {args}")
+135
+136    def switch_branch(self, branch_name: str) -> str | int:
+137        """Switch to the branch specified by `branch_name`.
+138
+139        Equivalent to `git checkout {branch_name}`."""
+140        return self.checkout(branch_name)
+141
+142    def create_new_branch(self, branch_name: str) -> str | int:
+143        """Create and switch to a new branch named with `branch_name`.
+144
+145        Equivalent to `git checkout -b {branch_name} --track`."""
+146        return self.checkout(f"-b {branch_name} --track")
+147
+148    def delete_branch(self, branch_name: str, local_only: bool = True) -
 > str | int:
-142        """Delete `branch_name` from repo.
-143
-144        #### :params:
-145
-146        `local_only`: Only delete the local copy of `branch`, otherwise also
+149        """Delete `branch_name` from repo.
+150
+151        #### :params:
+152
+153        `local_only`: Only delete the local copy of `branch`, otherwise also
 delete the remote branch on origin and remote-tracking branch."""
-147        output = self.branch(f"--delete {branch_name}")
-148        if not local_only:
-149            return output + self.push(f"origin --delete {branch_name}")  #
+154        output = self.branch(f"--delete {branch_name}")
+155        if not local_only:
+156            return output + self.push(f"origin --delete {branch_name}")  #
 type:ignore
-150        return output
-151
-152    def undo(self) -> str | int:
-153        """Undo uncommitted changes.
-154
-155        Equivalent to `git checkout .`."""
-156        return self.checkout(".")
-157
-158    def merge(self, branch_name: str) -> str | int:
-159        """Merge branch `branch_name` with currently active branch."""
-160        return self.execute(f"merge {branch_name}")
+157        return output
+158
+159    def undo(self) -> str | int:
+160        """Undo uncommitted changes.
 161
-162    # ===============================Requires GitHub CLI to be installed and
-configured===============================
-163
-164    def create_remote(self, name: str, public: bool = False) -> str | int:
-165        """Uses GitHub CLI (must be installed and configured) to create a
-remote GitHub repo.
-166
-167        #### :params:
+162        Equivalent to `git checkout .`."""
+163        return self.checkout(".")
+164
+165    def merge(self, branch_name: str) -> str | int:
+166        """Merge branch `branch_name` with currently active branch."""
+167        return self.execute(f"merge {branch_name}")
 168
-169        `name`: The name for the repo.
+169    # ===============================Requires GitHub CLI to be installed and
+configured===============================
 170
-171        `public`: Set to `True` to create the repo as public, otherwise
+171    def create_remote(self, name: str, public: bool = False) -> str | int:
+172        """Uses GitHub CLI (must be installed and configured) to create a
+remote GitHub repo.
+173
+174        #### :params:
+175
+176        `name`: The name for the repo.
+177
+178        `public`: Set to `True` to create the repo as public, otherwise
 it'll be created as private."""
-172        visibility = "--public" if public else "--private"
-173        return self._run(["gh", "repo", "create", name, visibility])
-174
-175    def create_remote_from_cwd(self, public: bool = False) -> str | int:
-176        """Use GitHub CLI (must be installed and configured) to create a
+179        visibility = "--public" if public else "--private"
+180        return self._run(["gh", "repo", "create", name, visibility])
+181
+182    def create_remote_from_cwd(self, public: bool = False) -> str | int:
+183        """Use GitHub CLI (must be installed and configured) to create a
 remote GitHub repo from
-177        the current working directory repo and add its url as this repo's
+184        the current working directory repo and add its url as this repo's
 remote origin.
-178
-179        #### :params:
-180
-181        `public`: Create the GitHub repo as a public repo, default is to
+185
+186        #### :params:
+187
+188        `public`: Create the GitHub repo as a public repo, default is to
 create it as private."""
-182        visibility = "public" if public else "private"
-183        return self._run(
-184            ["gh", "repo", "create", "--source", ".", f"--{visibility}", "--
+189        visibility = "public" if public else "private"
+190        return self._run(
+191            ["gh", "repo", "create", "--source", ".", f"--{visibility}", "--
 push"]
-185        )
-186
-187    def _change_visibility(self, owner: str, name: str, visibility: str) -
+192        )
+193
+194    def _change_visibility(self, owner: str, name: str, visibility: str) -
 > str | int:
-188        return self._run(
-189            ["gh", "repo", "edit", f"{owner}/{name}", "--visibility",
+195        return self._run(
+196            ["gh", "repo", "edit", f"{owner}/{name}", "--visibility",
 visibility]
-190        )
-191
-192    def make_private(self, owner: str, name: str) -> str | int:
-193        """Uses GitHub CLI (must be installed and configured) to set the
-repo's visibility to private.
-194
-195        #### :params:
-196
-197        `owner`: The repo owner.
+197        )
 198
-199        `name`: The name of the repo to edit."""
-200        return self._change_visibility(owner, name, "private")
+199    def make_private(self, owner: str, name: str) -> str | int:
+200        """Uses GitHub CLI (must be installed and configured) to set the
+repo's visibility to private.
 201
-202    def make_public(self, owner: str, name: str) -> str | int:
-203        """Uses GitHub CLI (must be installed and configured) to set the
-repo's visibility to public.
-204
-205        #### :params:
-206
-207        `owner`: The repo owner.
+202        #### :params:
+203
+204        `owner`: The repo owner.
+205
+206        `name`: The name of the repo to edit."""
+207        return self._change_visibility(owner, name, "private")
 208
-209        `name`: The name of the repo to edit."""
-210        return self._change_visibility(owner, name, "public")
+209    def make_public(self, owner: str, name: str) -> str | int:
+210        """Uses GitHub CLI (must be installed and configured) to set the
+repo's visibility to public.
 211
-212    def delete_remote(self, owner: str, name: str) -> str | int:
-213        """Uses GitHub CLI (must be isntalled and configured) to delete the
-remote for this repo.
-214
-215        #### :params:
-216
-217        `owner`: The repo owner.
+212        #### :params:
+213
+214        `owner`: The repo owner.
+215
+216        `name`: The name of the repo to edit."""
+217        return self._change_visibility(owner, name, "public")
 218
-219        `name`: The name of the remote repo to delete."""
-220        return self._run(["gh", "repo", "delete", f"{owner}/{name}", "--
+219    def delete_remote(self, owner: str, name: str) -> str | int:
+220        """Uses GitHub CLI (must be isntalled and configured) to delete the
+remote for this repo.
+221
+222        #### :params:
+223
+224        `owner`: The repo owner.
+225
+226        `name`: The name of the remote repo to delete."""
+227        return self._run(["gh", "repo", "delete", f"{owner}/{name}", "--
 yes"])
 ⁰
 Git(capture_stdout: bool = False) View Source
-_7    def __init__(self, capture_stdout: bool = False):
-_8        """If `capture_stdout` is `True`, all functions will return their
+_8    def __init__(self, capture_stdout: bool = False):
+_9        """If `capture_stdout` is `True`, all functions will return their
 generated `stdout` as a string.
-_9        Otherwise, the functions return the call's exit code."""
-10        self.capture_stdout = capture_stdout
+10        Otherwise, the functions return the call's exit code."""
+11        self.capture_stdout = capture_stdout
 If capture_stdout is True, all functions will return their generated stdout as
 a string. Otherwise, the functions return the call's exit code.
 capture_stdout: bool
 If True, member functions will return the generated stdout as a string,
 otherwise they return the command's exit code.
 ⁰
+@contextmanager
+def capture_output(self): View Source
+13    @contextmanager
+14    def capture_output(self):
+15        self.capture_stdout = True
+16        yield self
+17        self.capture_stdout = False
+⁰
 def execute(self, command: str) -> str | int: View Source
-28    def execute(self, command: str) -> str | int:
-29        """Execute git command.
-30
-31        Equivalent to executing `git {command}` in the shell."""
-32        args = ["git"] + shlex.split(command)
-33        return self._run(args)
+35    def execute(self, command: str) -> str | int:
+36        """Execute git command.
+37
+38        Equivalent to executing `git {command}` in the shell."""
+39        args = ["git"] + shlex.split(command)
+40        return self._run(args)
 Execute git command.
 Equivalent to executing git {command} in the shell.
 ⁰
 def new_repo(self) -> str | int: View Source
-35    def new_repo(self) -> str | int:
-36        """Executes `git init -b main`."""
-37        return self.execute("init -b main")
+42    def new_repo(self) -> str | int:
+43        """Executes `git init -b main`."""
+44        return self.execute("init -b main")
 Executes git init -b main.
 ⁰
 def loggy(self) -> str | int: View Source
-39    def loggy(self) -> str | int:
-40        """Equivalent to `git log --oneline --name-only --abbrev-commit --
+46    def loggy(self) -> str | int:
+47        """Equivalent to `git log --oneline --name-only --abbrev-commit --
 graph`."""
-41        return self.execute("log --oneline --name-only --abbrev-commit --
+48        return self.execute("log --oneline --name-only --abbrev-commit --
 graph")
 Equivalent to git log --oneline --name-only --abbrev-commit --graph.
 ⁰
 def status(self) -> str | int: View Source
-43    def status(self) -> str | int:
-44        """Execute `git status`."""
-45        return self.execute("status")
+50    def status(self) -> str | int:
+51        """Execute `git status`."""
+52        return self.execute("status")
 Execute git status.
 ⁰
 def commit(self, args: str) -> str | int: View Source
-48    def commit(self, args: str) -> str | int:
-49        """>>> git commit {args}"""
-50        return self.execute(f"commit {args}")
+55    def commit(self, args: str) -> str | int:
+56        """>>> git commit {args}"""
+57        return self.execute(f"commit {args}")
 >>> git commit {args}
 ⁰
 def add(self, files: list[str] | None = None) -> str | int: View Source
-52    def add(self, files: list[str] | None = None) -> str | int:
-53        """Stage a list of files.
-54
-55        If no files are given (`files=None`), all files will be staged."""
-56        if not files:
-57            return self.execute("add .")
-58        else:
-59            files = " ".join(f'"{file}"' for file in files)  # type: ignore
-60            return self.execute(f"add {files}")
+59    def add(self, files: list[str] | None = None) -> str | int:
+60        """Stage a list of files.
+61
+62        If no files are given (`files=None`), all files will be staged."""
+63        if not files:
+64            return self.execute("add .")
+65        else:
+66            files = " ".join(f'"{file}"' for file in files)  # type: ignore
+67            return self.execute(f"add {files}")
 Stage a list of files.
 If no files are given (files=None), all files will be staged.
 ⁰
 def commit_files(self, files: list[str], message: str) -> str | int: View
 Source
-62    def commit_files(self, files: list[str], message: str) -> str | int:
-63        """Stage and commit a list of files with commit message `message`."""
-64        return self.add(files) + self.commit(f'-m "{message}"')  # type:
+69    def commit_files(self, files: list[str], message: str) -> str | int:
+70        """Stage and commit a list of files with commit message `message`."""
+71        return self.add(files) + self.commit(f'-m "{message}"')  # type:
 ignore
 Stage and commit a list of files with commit message message.
 ⁰
 def initcommit(self) -> str | int: View Source
-66    def initcommit(self) -> str | int:
-67        """Equivalent to
-68        >>> git add .
-69        >>> git commit -m "Initial commit" """
-70        return self.add() + self.commit('-m "Initial commit"')  # type:
+73    def initcommit(self) -> str | int:
+74        """Equivalent to
+75        >>> git add .
+76        >>> git commit -m "Initial commit" """
+77        return self.add() + self.commit('-m "Initial commit"')  # type:
 ignore
 Equivalent to
 >>> git add .
 >>> git commit -m "Initial commit"
 ⁰
 def amend(self, files: list[str] | None = None) -> str | int: View Source
-72    def amend(self, files: list[str] | None = None) -> str | int:
-73        """Stage and commit changes to the previous commit.
-74
-75        If `files` is `None`, all files will be staged.
-76
-77        Equivalent to:
-78        >>> git add {files}
-79        >>> git commit --amend --no-edit
-80        """
-81        return self.add(files) + self.commit("--amend --no-edit")  # type:
+79    def amend(self, files: list[str] | None = None) -> str | int:
+80        """Stage and commit changes to the previous commit.
+81
+82        If `files` is `None`, all files will be staged.
+83
+84        Equivalent to:
+85        >>> git add {files}
+86        >>> git commit --amend --no-edit
+87        """
+88        return self.add(files) + self.commit("--amend --no-edit")  # type:
 ignore
 Stage and commit changes to the previous commit.
 If files is None, all files will be staged.
 Equivalent to:
 >>> git add {files}
 >>> git commit --amend --no-edit
 ⁰
 def tag(self, args: str = '') -> str | int: View Source
-83    def tag(self, args: str = "") -> str | int:
-84        """Execute the `tag` command with `args`.
-85
-86        e.g.
-87
-88        `self.tag("--sort=-committerdate")`
-89
-90        will list all the tags for this repository in descending commit
+90    def tag(self, args: str = "") -> str | int:
+91        """Execute the `tag` command with `args`.
+92
+93        e.g.
+94
+95        `self.tag("--sort=-committerdate")`
+96
+97        will list all the tags for this repository in descending commit
 date."""
-91        return self.execute(f"tag {args}")
+98        return self.execute(f"tag {args}")
 Execute the tag command with args.
 e.g.
 self.tag("--sort=-committerdate")
 will list all the tags for this repository in descending commit date.
 ⁰
 def add_remote_url(self, url: str, name: str = 'origin') -> str | int: View
 Source
-94    def add_remote_url(self, url: str, name: str = "origin") -> str | int:
-95        """Add remote url to repo."""
-96        return self.execute(f"remote add {name} {url}")
+101    def add_remote_url(self, url: str, name: str = "origin") -> str | int:
+102        """Add remote url to repo."""
+103        return self.execute(f"remote add {name} {url}")
 Add remote url to repo.
 ⁰
 def push(self, args: str = '') -> str | int: View Source
-_98    def push(self, args: str = "") -> str | int:
-_99        """Equivalent to `git push {args}`."""
-100        return self.execute(f"push {args}")
+105    def push(self, args: str = "") -> str | int:
+106        """Equivalent to `git push {args}`."""
+107        return self.execute(f"push {args}")
 Equivalent to git push {args}.
 ⁰
 def pull(self, args: str = '') -> str | int: View Source
-102    def pull(self, args: str = "") -> str | int:
-103        """Equivalent to `git pull {args}`."""
-104        return self.execute(f"pull {args}")
+109    def pull(self, args: str = "") -> str | int:
+110        """Equivalent to `git pull {args}`."""
+111        return self.execute(f"pull {args}")
 Equivalent to git pull {args}.
 ⁰
 def push_new_branch(self, branch: str) -> str | int: View Source
-106    def push_new_branch(self, branch: str) -> str | int:
-107        """Push a new branch to origin with tracking.
-108
-109        Equivalent to `git push -u origin {branch}`."""
-110        return self.push(f"-u origin {branch}")
+113    def push_new_branch(self, branch: str) -> str | int:
+114        """Push a new branch to origin with tracking.
+115
+116        Equivalent to `git push -u origin {branch}`."""
+117        return self.push(f"-u origin {branch}")
 Push a new branch to origin with tracking.
 Equivalent to git push -u origin {branch}.
 ⁰
 def pull_branch(self, branch: str) -> str | int: View Source
-112    def pull_branch(self, branch: str) -> str | int:
-113        """Pull `branch` from origin."""
-114        return self.pull(f"origin {branch}")
+119    def pull_branch(self, branch: str) -> str | int:
+120        """Pull `branch` from origin."""
+121        return self.pull(f"origin {branch}")
 Pull branch from origin.
 ⁰
 def branch(self, args: str) -> str | int: View Source
-117    def branch(self, args: str) -> str | int:
-118        """Equivalent to `git branch {args}`."""
-119        return self.execute(f"branch {args}")
+124    def branch(self, args: str) -> str | int:
+125        """Equivalent to `git branch {args}`."""
+126        return self.execute(f"branch {args}")
 Equivalent to git branch {args}.
 ⁰
 def list_branches(self) -> str | int: View Source
-121    def list_branches(self) -> str | int:
-122        """Print a list of branches."""
-123        return self.branch("-vva")
+128    def list_branches(self) -> str | int:
+129        """Print a list of branches."""
+130        return self.branch("-vva")
 Print a list of branches.
 ⁰
 def checkout(self, args: str) -> str | int: View Source
-125    def checkout(self, args: str) -> str | int:
-126        """Equivalent to `git checkout {args}`."""
-127        return self.execute(f"checkout {args}")
+132    def checkout(self, args: str) -> str | int:
+133        """Equivalent to `git checkout {args}`."""
+134        return self.execute(f"checkout {args}")
 Equivalent to git checkout {args}.
 ⁰
 def switch_branch(self, branch_name: str) -> str | int: View Source
-129    def switch_branch(self, branch_name: str) -> str | int:
-130        """Switch to the branch specified by `branch_name`.
-131
-132        Equivalent to `git checkout {branch_name}`."""
-133        return self.checkout(branch_name)
+136    def switch_branch(self, branch_name: str) -> str | int:
+137        """Switch to the branch specified by `branch_name`.
+138
+139        Equivalent to `git checkout {branch_name}`."""
+140        return self.checkout(branch_name)
 Switch to the branch specified by branch_name.
 Equivalent to git checkout {branch_name}.
 ⁰
 def create_new_branch(self, branch_name: str) -> str | int: View Source
-135    def create_new_branch(self, branch_name: str) -> str | int:
-136        """Create and switch to a new branch named with `branch_name`.
-137
-138        Equivalent to `git checkout -b {branch_name} --track`."""
-139        return self.checkout(f"-b {branch_name} --track")
+142    def create_new_branch(self, branch_name: str) -> str | int:
+143        """Create and switch to a new branch named with `branch_name`.
+144
+145        Equivalent to `git checkout -b {branch_name} --track`."""
+146        return self.checkout(f"-b {branch_name} --track")
 Create and switch to a new branch named with branch_name.
 Equivalent to git checkout -b {branch_name} --track.
 ⁰
 def delete_branch(self, branch_name: str, local_only: bool = True) -> str |
 int: View Source
-141    def delete_branch(self, branch_name: str, local_only: bool = True) -
+148    def delete_branch(self, branch_name: str, local_only: bool = True) -
 > str | int:
-142        """Delete `branch_name` from repo.
-143
-144        #### :params:
-145
-146        `local_only`: Only delete the local copy of `branch`, otherwise also
+149        """Delete `branch_name` from repo.
+150
+151        #### :params:
+152
+153        `local_only`: Only delete the local copy of `branch`, otherwise also
 delete the remote branch on origin and remote-tracking branch."""
-147        output = self.branch(f"--delete {branch_name}")
-148        if not local_only:
-149            return output + self.push(f"origin --delete {branch_name}")  #
+154        output = self.branch(f"--delete {branch_name}")
+155        if not local_only:
+156            return output + self.push(f"origin --delete {branch_name}")  #
 type:ignore
-150        return output
+157        return output
 Delete branch_name from repo.
 *** :params: ***
 local_only: Only delete the local copy of branch, otherwise also delete the
 remote branch on origin and remote-tracking branch.
 ⁰
 def undo(self) -> str | int: View Source
-152    def undo(self) -> str | int:
-153        """Undo uncommitted changes.
-154
-155        Equivalent to `git checkout .`."""
-156        return self.checkout(".")
+159    def undo(self) -> str | int:
+160        """Undo uncommitted changes.
+161
+162        Equivalent to `git checkout .`."""
+163        return self.checkout(".")
 Undo uncommitted changes.
 Equivalent to git checkout ..
 ⁰
 def merge(self, branch_name: str) -> str | int: View Source
-158    def merge(self, branch_name: str) -> str | int:
-159        """Merge branch `branch_name` with currently active branch."""
-160        return self.execute(f"merge {branch_name}")
+165    def merge(self, branch_name: str) -> str | int:
+166        """Merge branch `branch_name` with currently active branch."""
+167        return self.execute(f"merge {branch_name}")
 Merge branch branch_name with currently active branch.
 ⁰
 def create_remote(self, name: str, public: bool = False) -> str | int: View
 Source
-164    def create_remote(self, name: str, public: bool = False) -> str | int:
-165        """Uses GitHub CLI (must be installed and configured) to create a
+171    def create_remote(self, name: str, public: bool = False) -> str | int:
+172        """Uses GitHub CLI (must be installed and configured) to create a
 remote GitHub repo.
-166
-167        #### :params:
-168
-169        `name`: The name for the repo.
-170
-171        `public`: Set to `True` to create the repo as public, otherwise
+173
+174        #### :params:
+175
+176        `name`: The name for the repo.
+177
+178        `public`: Set to `True` to create the repo as public, otherwise
 it'll be created as private."""
-172        visibility = "--public" if public else "--private"
-173        return self._run(["gh", "repo", "create", name, visibility])
+179        visibility = "--public" if public else "--private"
+180        return self._run(["gh", "repo", "create", name, visibility])
 Uses GitHub CLI (must be installed and configured) to create a remote GitHub
 repo.
 *** :params: ***
 name: The name for the repo.
 public: Set to True to create the repo as public, otherwise it'll be created as
 private.
 ⁰
 def create_remote_from_cwd(self, public: bool = False) -> str | int: View
 Source
-175    def create_remote_from_cwd(self, public: bool = False) -> str | int:
-176        """Use GitHub CLI (must be installed and configured) to create a
+182    def create_remote_from_cwd(self, public: bool = False) -> str | int:
+183        """Use GitHub CLI (must be installed and configured) to create a
 remote GitHub repo from
-177        the current working directory repo and add its url as this repo's
+184        the current working directory repo and add its url as this repo's
 remote origin.
-178
-179        #### :params:
-180
-181        `public`: Create the GitHub repo as a public repo, default is to
+185
+186        #### :params:
+187
+188        `public`: Create the GitHub repo as a public repo, default is to
 create it as private."""
-182        visibility = "public" if public else "private"
-183        return self._run(
-184            ["gh", "repo", "create", "--source", ".", f"--{visibility}", "--
+189        visibility = "public" if public else "private"
+190        return self._run(
+191            ["gh", "repo", "create", "--source", ".", f"--{visibility}", "--
 push"]
-185        )
+192        )
 Use GitHub CLI (must be installed and configured) to create a remote GitHub
 repo from the current working directory repo and add its url as this repo's
 remote origin.
 *** :params: ***
 public: Create the GitHub repo as a public repo, default is to create it as
 private.
 ⁰
 def make_private(self, owner: str, name: str) -> str | int: View Source
-192    def make_private(self, owner: str, name: str) -> str | int:
-193        """Uses GitHub CLI (must be installed and configured) to set the
+199    def make_private(self, owner: str, name: str) -> str | int:
+200        """Uses GitHub CLI (must be installed and configured) to set the
 repo's visibility to private.
-194
-195        #### :params:
-196
-197        `owner`: The repo owner.
-198
-199        `name`: The name of the repo to edit."""
-200        return self._change_visibility(owner, name, "private")
+201
+202        #### :params:
+203
+204        `owner`: The repo owner.
+205
+206        `name`: The name of the repo to edit."""
+207        return self._change_visibility(owner, name, "private")
 Uses GitHub CLI (must be installed and configured) to set the repo's visibility
 to private.
 *** :params: ***
 owner: The repo owner.
 name: The name of the repo to edit.
 ⁰
 def make_public(self, owner: str, name: str) -> str | int: View Source
-202    def make_public(self, owner: str, name: str) -> str | int:
-203        """Uses GitHub CLI (must be installed and configured) to set the
+209    def make_public(self, owner: str, name: str) -> str | int:
+210        """Uses GitHub CLI (must be installed and configured) to set the
 repo's visibility to public.
-204
-205        #### :params:
-206
-207        `owner`: The repo owner.
-208
-209        `name`: The name of the repo to edit."""
-210        return self._change_visibility(owner, name, "public")
+211
+212        #### :params:
+213
+214        `owner`: The repo owner.
+215
+216        `name`: The name of the repo to edit."""
+217        return self._change_visibility(owner, name, "public")
 Uses GitHub CLI (must be installed and configured) to set the repo's visibility
 to public.
 *** :params: ***
 owner: The repo owner.
 name: The name of the repo to edit.
 ⁰
 def delete_remote(self, owner: str, name: str) -> str | int: View Source
-212    def delete_remote(self, owner: str, name: str) -> str | int:
-213        """Uses GitHub CLI (must be isntalled and configured) to delete the
+219    def delete_remote(self, owner: str, name: str) -> str | int:
+220        """Uses GitHub CLI (must be isntalled and configured) to delete the
 remote for this repo.
-214
-215        #### :params:
-216
-217        `owner`: The repo owner.
-218
-219        `name`: The name of the remote repo to delete."""
-220        return self._run(["gh", "repo", "delete", f"{owner}/{name}", "--
+221
+222        #### :params:
+223
+224        `owner`: The repo owner.
+225
+226        `name`: The name of the remote repo to delete."""
+227        return self._run(["gh", "repo", "delete", f"{owner}/{name}", "--
 yes"])
 Uses GitHub CLI (must be isntalled and configured) to delete the remote for
 this repo.
 *** :params: ***
 owner: The repo owner.
 name: The name of the remote repo to delete.
```

### Comparing `gitbetter-1.1.0/docs/gitbetter/gitbetter.html` & `gitbetter-1.2.0/docs/gitbetter/gitbetter.html`

 * *Files identical despite different names*

### Comparing `gitbetter-1.1.0/src/gitbetter/git.py` & `gitbetter-1.2.0/src/gitbetter/git.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 import shlex
 import subprocess
+from contextlib import contextmanager
 
 
 class Git:
     def __init__(self, capture_stdout: bool = False):
         """If `capture_stdout` is `True`, all functions will return their generated `stdout` as a string.
         Otherwise, the functions return the call's exit code."""
         self.capture_stdout = capture_stdout
 
+    @contextmanager
+    def capture_output(self):
+        self.capture_stdout = True
+        yield self
+        self.capture_stdout = False
+
     @property
     def capture_stdout(self) -> bool:
         """If `True`, member functions will return the generated `stdout` as a string,
         otherwise they return the command's exit code."""
         return self._capture_stdout
 
     @capture_stdout.setter
```

### Comparing `gitbetter-1.1.0/src/gitbetter/gitbetter.py` & `gitbetter-1.2.0/src/gitbetter/gitbetter.py`

 * *Files identical despite different names*

### Comparing `gitbetter-1.1.0/LICENSE.txt` & `gitbetter-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gitbetter-1.1.0/README.md` & `gitbetter-1.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -149,7 +149,29 @@
   gitbetter_test.py
   test.py
   test.txt
 >>> git.list_branches()
 * main                3e780ec [origin/main: ahead 3] Merge branch 'my-feature'
   remotes/origin/main fc6b7ac docs: update readme
 </pre>
+
+If capturing stdout is only desired for a set of functions, 
+the `capture_output` function can be used as a context manager.
+Upon entering the context, the `capture_stdout` property is set to `True`
+and then set back to `False` upon exiting the context.
+<pre>
+>>> git = Git()
+>>> with git.capture_output():
+...  status = git.status()
+...
+>>> print(status)
+On branch stdout-context-manager
+Your branch is up to date with 'main'.
+
+Changes not staged for commit:
+  (use "git add <\file>..." to update what will be committed)
+  (use "git restore <\file>..." to discard changes in working directory)
+        modified:   src/gitbetter/git.py
+
+no changes added to commit (use "git add" and/or "git commit -a")
+
+</pre>
```

### Comparing `gitbetter-1.1.0/pyproject.toml` & `gitbetter-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 00000040: 6c69 6e67 2e62 7569 6c64 220d 0a0d 0a5b  ling.build"....[
 00000050: 7072 6f6a 6563 745d 0d0a 6e61 6d65 203d  project]..name =
 00000060: 2022 6769 7462 6574 7465 7222 0d0a 6465   "gitbetter"..de
 00000070: 7363 7269 7074 696f 6e20 3d20 2243 7573  scription = "Cus
 00000080: 746f 6d20 6769 7420 7368 656c 6c20 746f  tom git shell to
 00000090: 2074 7970 6520 6c65 7373 2061 6e64 2063   type less and c
 000000a0: 6f6d 6d69 7420 6d6f 7265 2e22 0d0a 7665  ommit more."..ve
-000000b0: 7273 696f 6e20 3d20 2231 2e31 2e30 220d  rsion = "1.1.0".
+000000b0: 7273 696f 6e20 3d20 2231 2e32 2e30 220d  rsion = "1.2.0".
 000000c0: 0a72 6571 7569 7265 732d 7079 7468 6f6e  .requires-python
 000000d0: 203d 2022 3e3d 332e 3130 220d 0a64 6570   = ">=3.10"..dep
 000000e0: 656e 6465 6e63 6965 7320 3d20 5b22 6172  endencies = ["ar
 000000f0: 6773 6865 6c6c 222c 2022 7061 7468 6965  gshell", "pathie
 00000100: 7222 2c20 2270 7974 6573 7422 5d0d 0a72  r", "pytest"]..r
 00000110: 6561 646d 6520 3d20 2252 4541 444d 452e  eadme = "README.
 00000120: 6d64 220d 0a6b 6579 776f 7264 7320 3d20  md"..keywords =
```

### Comparing `gitbetter-1.1.0/PKG-INFO` & `gitbetter-1.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitbetter
-Version: 1.1.0
+Version: 1.2.0
 Summary: Custom git shell to type less and commit more.
 Project-URL: Homepage, https://github.com/matt-manes/gitbetter
 Project-URL: Documentation, https://github.com/matt-manes/gitbetter/tree/main/docs
 Project-URL: Source code, https://github.com/matt-manes/gitbetter/tree/main/src/gitbetter
 Author-email: Matt Manes <mattmanes@pm.me>
 License-File: LICENSE.txt
 Keywords: cli,commit,git,shell,terminal
@@ -168,7 +168,29 @@
   gitbetter_test.py
   test.py
   test.txt
 >>> git.list_branches()
 * main                3e780ec [origin/main: ahead 3] Merge branch 'my-feature'
   remotes/origin/main fc6b7ac docs: update readme
 </pre>
+
+If capturing stdout is only desired for a set of functions, 
+the `capture_output` function can be used as a context manager.
+Upon entering the context, the `capture_stdout` property is set to `True`
+and then set back to `False` upon exiting the context.
+<pre>
+>>> git = Git()
+>>> with git.capture_output():
+...  status = git.status()
+...
+>>> print(status)
+On branch stdout-context-manager
+Your branch is up to date with 'main'.
+
+Changes not staged for commit:
+  (use "git add <\file>..." to update what will be committed)
+  (use "git restore <\file>..." to discard changes in working directory)
+        modified:   src/gitbetter/git.py
+
+no changes added to commit (use "git add" and/or "git commit -a")
+
+</pre>
```

