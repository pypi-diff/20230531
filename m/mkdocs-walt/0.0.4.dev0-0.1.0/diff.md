# Comparing `tmp/mkdocs-walt-0.0.4.dev0.tar.gz` & `tmp/mkdocs-walt-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-walt-0.0.4.dev0.tar", last modified: Tue May 30 22:08:10 2023, max compression
+gzip compressed data, was "mkdocs-walt-0.1.0.tar", last modified: Wed May 31 19:05:18 2023, max compression
```

## Comparing `mkdocs-walt-0.0.4.dev0.tar` & `mkdocs-walt-0.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 sue        (501) staff       (20)        0 2023-05-30 22:08:10.901172 mkdocs-walt-0.0.4.dev0/
--rw-r--r--   0 sue        (501) staff       (20)      145 2023-05-30 20:37:51.000000 mkdocs-walt-0.0.4.dev0/MANIFEST.in
--rw-r--r--   0 sue        (501) staff       (20)      872 2023-05-30 22:08:10.901067 mkdocs-walt-0.0.4.dev0/PKG-INFO
-drwxr-xr-x   0 sue        (501) staff       (20)        0 2023-05-30 22:08:10.900210 mkdocs-walt-0.0.4.dev0/mkdocs_walt.egg-info/
--rw-r--r--   0 sue        (501) staff       (20)      872 2023-05-30 22:08:10.000000 mkdocs-walt-0.0.4.dev0/mkdocs_walt.egg-info/PKG-INFO
--rw-r--r--   0 sue        (501) staff       (20)      366 2023-05-30 22:08:10.000000 mkdocs-walt-0.0.4.dev0/mkdocs_walt.egg-info/SOURCES.txt
--rw-r--r--   0 sue        (501) staff       (20)        1 2023-05-30 22:08:10.000000 mkdocs-walt-0.0.4.dev0/mkdocs_walt.egg-info/dependency_links.txt
--rw-r--r--   0 sue        (501) staff       (20)       28 2023-05-30 22:08:10.000000 mkdocs-walt-0.0.4.dev0/mkdocs_walt.egg-info/entry_points.txt
--rw-r--r--   0 sue        (501) staff       (20)        1 2023-05-29 21:29:31.000000 mkdocs-walt-0.0.4.dev0/mkdocs_walt.egg-info/not-zip-safe
--rw-r--r--   0 sue        (501) staff       (20)        7 2023-05-30 22:08:10.000000 mkdocs-walt-0.0.4.dev0/mkdocs_walt.egg-info/requires.txt
--rw-r--r--   0 sue        (501) staff       (20)        5 2023-05-30 22:08:10.000000 mkdocs-walt-0.0.4.dev0/mkdocs_walt.egg-info/top_level.txt
--rw-r--r--   0 sue        (501) staff       (20)       38 2023-05-30 22:08:10.901202 mkdocs-walt-0.0.4.dev0/setup.cfg
--rw-r--r--   0 sue        (501) staff       (20)     1241 2023-05-30 21:01:40.000000 mkdocs-walt-0.0.4.dev0/setup.py
-drwxr-xr-x   0 sue        (501) staff       (20)        0 2023-05-30 22:08:10.900905 mkdocs-walt-0.0.4.dev0/walt/
--rw-r--r--   0 sue        (501) staff       (20)       29 2023-05-29 21:22:32.000000 mkdocs-walt-0.0.4.dev0/walt/__init__.py
--rw-r--r--   0 sue        (501) staff       (20)     2035 2023-05-30 17:08:24.000000 mkdocs-walt-0.0.4.dev0/walt/base.html
--rw-r--r--   0 sue        (501) staff       (20)       26 2023-05-30 01:55:40.000000 mkdocs-walt-0.0.4.dev0/walt/main.html
--rw-r--r--   0 sue        (501) staff       (20)      150 2023-05-30 22:04:56.000000 mkdocs-walt-0.0.4.dev0/walt/mkdocs_theme.yml
--rw-r--r--   0 sue        (501) staff       (20)     5628 2023-05-30 22:02:26.000000 mkdocs-walt-0.0.4.dev0/walt/styles.css
--rw-r--r--   0 sue        (501) staff       (20)      423 2023-05-30 20:14:49.000000 mkdocs-walt-0.0.4.dev0/walt/writ.html
+drwxr-xr-x   0 sue        (501) staff       (20)        0 2023-05-31 19:05:18.411700 mkdocs-walt-0.1.0/
+-rw-r--r--   0 sue        (501) staff       (20)      145 2023-05-30 20:37:51.000000 mkdocs-walt-0.1.0/MANIFEST.in
+-rw-r--r--   0 sue        (501) staff       (20)     1495 2023-05-31 19:05:18.411593 mkdocs-walt-0.1.0/PKG-INFO
+-rw-r--r--   0 sue        (501) staff       (20)     1063 2023-05-31 18:19:34.000000 mkdocs-walt-0.1.0/README.md
+drwxr-xr-x   0 sue        (501) staff       (20)        0 2023-05-31 19:05:18.410909 mkdocs-walt-0.1.0/mkdocs_walt.egg-info/
+-rw-r--r--   0 sue        (501) staff       (20)     1495 2023-05-31 19:05:18.000000 mkdocs-walt-0.1.0/mkdocs_walt.egg-info/PKG-INFO
+-rw-r--r--   0 sue        (501) staff       (20)      361 2023-05-31 19:05:18.000000 mkdocs-walt-0.1.0/mkdocs_walt.egg-info/SOURCES.txt
+-rw-r--r--   0 sue        (501) staff       (20)        1 2023-05-31 19:05:18.000000 mkdocs-walt-0.1.0/mkdocs_walt.egg-info/dependency_links.txt
+-rw-r--r--   0 sue        (501) staff       (20)       28 2023-05-31 19:05:18.000000 mkdocs-walt-0.1.0/mkdocs_walt.egg-info/entry_points.txt
+-rw-r--r--   0 sue        (501) staff       (20)        1 2023-05-29 21:29:31.000000 mkdocs-walt-0.1.0/mkdocs_walt.egg-info/not-zip-safe
+-rw-r--r--   0 sue        (501) staff       (20)        7 2023-05-31 19:05:18.000000 mkdocs-walt-0.1.0/mkdocs_walt.egg-info/requires.txt
+-rw-r--r--   0 sue        (501) staff       (20)        5 2023-05-31 19:05:18.000000 mkdocs-walt-0.1.0/mkdocs_walt.egg-info/top_level.txt
+-rw-r--r--   0 sue        (501) staff       (20)       38 2023-05-31 19:05:18.411733 mkdocs-walt-0.1.0/setup.cfg
+-rw-r--r--   0 sue        (501) staff       (20)      872 2023-05-31 19:05:08.000000 mkdocs-walt-0.1.0/setup.py
+drwxr-xr-x   0 sue        (501) staff       (20)        0 2023-05-31 19:05:18.411436 mkdocs-walt-0.1.0/walt/
+-rw-r--r--   0 sue        (501) staff       (20)       29 2023-05-29 21:22:32.000000 mkdocs-walt-0.1.0/walt/__init__.py
+-rw-r--r--   0 sue        (501) staff       (20)     3383 2023-05-31 18:42:35.000000 mkdocs-walt-0.1.0/walt/base.html
+-rw-r--r--   0 sue        (501) staff       (20)       26 2023-05-30 01:55:40.000000 mkdocs-walt-0.1.0/walt/main.html
+-rw-r--r--   0 sue        (501) staff       (20)      189 2023-05-31 18:05:20.000000 mkdocs-walt-0.1.0/walt/mkdocs_theme.yml
+-rw-r--r--   0 sue        (501) staff       (20)     5788 2023-05-31 18:44:58.000000 mkdocs-walt-0.1.0/walt/styles.css
```

### Comparing `mkdocs-walt-0.0.4.dev0/setup.py` & `mkdocs-walt-0.1.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-from setuptools import setup, find_packages
+# mkdocs-walt
 
-VERSION = '0.0.4-dev'
+🍃 Walt is a minimal documentation theme for MkDocs.
 
-LONG_DESCRIPTION = '''
-# mkdocs-walt: a minimal documentation theme for MkDocs
+It has the following features:
 
-Walt is a minimal documentation theme that is best suited for single page websites.
+- classless styles for semantic HTML based on [writ.css](https://writ.cmcenroe.me)
+- light mode and dark mode based on system settings
+- an emoji favicon for browsers that support svg site icons
+- code syntax highlighting using highlight.js
 
 ## Installation
 
 ```sh
 pip install mkdocs-walt
 ```
 
@@ -21,34 +23,25 @@
 ```yaml
 theme:
   name: walt
 ```
 
 See the [full usage example](https://github.com/codesue/walt/examples/mkdocs).
 
+## Defaults
+
+Walt sets the following configurations by default:
+
+```yaml
+site_emoji: 🍃
+locale: en
+theme_color: "hsl(0, 0%, 100%)"
+theme_color_dark: "hsl(232, 23%, 18%)"
+include_header: true
+highlightjs: true
+```
+
 ## Acknowledgements
 
 Walt uses [writ.css](https://github.com/programble/writ/tree/master) for styles
-and [Catppuccin](https://github.com/catppuccin/catppuccin) for dark mode
-color palettes.
-'''
-
-setup(
-    name='mkdocs-walt',
-    version=VERSION,
-    author='Suzen Fylke',
-    author_email='codesue@users.noreply.github.com',
-    description='A minimal theme for MkDocs',
-    long_description=LONG_DESCRIPTION,
-    long_description_content_type='text/markdown',
-    url='https://github.com/codesue/walt',
-    license='GPLv3',
-    packages=find_packages(),
-    include_package_data=True,
-    install_requires=['mkdocs'],
-    entry_points={
-        'mkdocs.themes': [
-            'walt = walt',
-        ]
-    },
-    zip_safe=False
-)
+and [Catppuccin](https://github.com/catppuccin/catppuccin) for code block syntax
+highlighting and dark mode color palettes.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mkdocs-walt-0.0.4.dev0/walt/base.html` & `mkdocs-walt-0.1.0/walt/base.html`

 * *Files 27% similar despite different names*

```diff
@@ -15,27 +15,56 @@
     <meta name="color-scheme" content="light dark">
     <meta name="theme-color" content="{{ config.theme.theme_color }}" media="(prefers-color-scheme: light)">
     <meta name="theme-color" content="{{ config.theme.theme_color_dark }}" media="(prefers-color-scheme: dark)">
     {%- endblock %}
 
     {%- block styles %}
     <link rel="stylesheet" href="{{ "styles.css"|url }}">
+    {%- if config.theme.highlightjs %}
+    <link rel="stylesheet" href="//unpkg.com/@catppuccin/highlightjs/css/catppuccin-macchiato.css" media="(prefers-color-scheme: dark)">
+    <link rel="stylesheet" href="//unpkg.com/@catppuccin/highlightjs/css/catppuccin-latte.css" media="(prefers-color-scheme: light)">
+    <style>
+      .hljs, code.hljs { background: unset; }
+      code .hljs-comment { color: var(--color-secondary-text); }
+    </style>
+    {%- endif %}
     {% for path in config.extra_css %}
     <link href="{{ path|url }}" rel="stylesheet">
     {% endfor %}
     {%- endblock %}
 
     {%- block libs %}
+    {%- if config.theme.highlightjs %}
+    <script src="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/10.5.0/highlight.min.js"></script>
+    {%- for lang in config.theme.hljs_languages %}
+      <script src="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/10.5.0/languages/{{lang}}.min.js"></script>
+    {%- endfor %}
+    <script>hljs.initHighlightingOnLoad();</script>
+    {%- endif %}
     {%- endblock %}
 
     {%- block extrahead %} {% endblock %}
   </head>
   <body>
     <a href="#skip" class="visually-hidden">Skip to main content</a>
     {%- block header %}
+    {%- if config.theme.include_header %}
+    <header>
+      <span class="site-name">{{ config.site_name }}</span>
+      {% if config.site_description %}<p>{{ config.site_description }}</p>{% endif %}
+      <nav>
+        <h2 class="visually-hidden">Top level navigation menu</h2>
+        <ul>
+          {%- for nav_item in nav %}
+          <li><a href="{{ nav_item.url|url }}">{{ nav_item.title }}</a></li>
+          {%- endfor %}
+        </ul>
+      </nav>
+    </header>
+    {%- endif %}
     {%- endblock %}
     {%- block main %}
     <main id="skip">
       {{ page.content }}
     </main>
     {%- endblock %}
     {%- block footer %}
```

#### html2text {}

```diff
@@ -5,17 +5,29 @@
 {% endif %} {% if page and page.canonical_url %}
 {% endif %} {% if config.site_favicon %}
  {% else %}
 {% endif %}
 
 
  {%- endblock %} {%- block styles %}
-css"|url }}"> {% for path in config.extra_css %}
- {% endfor %} {%- endblock %} {%- block libs %} {%- endblock %} {%- block
-extrahead %} {% endblock %}
-Skip_to_main_content {%- block header %} {%- endblock %} {%- block main %}  {
-{ page.content }}  {%- endblock %} {%- block footer %}  {%- if config.copyright
+css"|url }}"> {%- if config.theme.highlightjs %}
+
+ {%- endif %} {% for path in config.extra_css %}
+ {% endfor %} {%- endblock %} {%- block libs %} {%- if config.theme.highlightjs
 %}
+ {%- for lang in config.theme.hljs_languages %}
+ {%- endfor %}
+ {%- endif %} {%- endblock %} {%- block extrahead %} {% endblock %}
+Skip_to_main_content {%- block header %} {%- if config.theme.include_header %}
+{{ config.site_name }} {% if config.site_description %}
+{{ config.site_description }}
+{% endif %}
+***** Top level navigation menu *****
+    * {%- for nav_item in nav %}
+    * {{_nav_item.title_}}
+    * {%- endfor %}
+  {%- endif %} {%- endblock %} {%- block main %}  {{ page.content }}  {%-
+endblock %} {%- block footer %}  {%- if config.copyright %}
 {{ config.copyright }}
 {%- endif %}  {%- endblock %} {%- block scripts %} {% for path in
 config.extra_javascript %}
  {% endfor %} {%- endblock %}
```

### Comparing `mkdocs-walt-0.0.4.dev0/walt/styles.css` & `mkdocs-walt-0.1.0/walt/styles.css`

 * *Files 3% similar despite different names*

```diff
@@ -30,21 +30,26 @@
 @media (prefers-color-scheme: dark) {
   :root {
     --color-background: hsl(232, 23%, 18%);
     --color-text: hsl(227, 68%, 88%);
     --color-secondary-text: hsl(228, 39%, 80%);
     --color-link: hsl(217, 92%, 76%);
     --color-link-visited: hsl(232, 97%, 85%);
-    --color-code-background: hsl(231, 16%, 34%);
+    --color-code-background: hsl(230, 19%, 26%);
     --color-code-text: hsl(227, 68%, 88%);
     --color-highlight: hsla(355, 71%, 77%, 0.4);
     --color-highlight-deep: hsla(355, 71%, 77%, 0.6);
-    --color-border: hsl(230, 14%, 41%);
+    --color-border: hsl(231, 16%, 34%);
     --color-table-border: hsl(228, 39%, 80%);
   }
+
+  img {
+    filter: brightness(.8) contrast(1.2);
+  }
+
 }
 
 * {
   box-sizing: border-box;
 }
 
 *, *::before, *::after {
@@ -71,14 +76,15 @@
   max-width: 40;
   margin-left: 1em;
   margin-right: 1em;
 }
 
 body > header {
   text-align: center;
+  margin-top: 5em;
 }
 
 main, body > footer {
   display: block;
   max-width: 78ch;
   margin: auto;
 }
@@ -86,16 +92,16 @@
 main figure, main aside {
   float: right;
   margin: 1.5rem 0 0 1ch;
 }
 
 main aside {
   max-width: 26ch;
+  border: solid var(--color-code-background);
   border-width: 0 0 0 0.5ch;
-  border: solid var(--color-code-background); 
   padding: 0 0 0 0.5ch;
 }
 
 body > footer {
   position: sticky;
   top: 100vh;
 }
@@ -127,23 +133,28 @@
 
 ul ul, ol ol, ul ol, ol ul {
   margin: 0;
 }
 
 /* Typography */
 
-h1, h2, h3, h4, h5, h6, th {
+h1, h2, h3, h4, h5, h6, th, .site-name {
   font-weight: var(--font-weight-heading);
 }
 
-h1, h2, h3 {
+h1, h2, h3, .site-name {
   line-height: 3rem;
 }
 
-h1 {
+header + main h1 {
+  margin-top: 1.5rem;
+  font-size: 2.284em;
+}
+
+h1, .site-name {
   font-size: 2.488em;
   margin-top: 2em;
 }
 
 h2 {
   font-size: 2.074em;
 }
@@ -187,16 +198,16 @@
 
 sup, sub {
   font-size: 0.75em;
   line-height: 1em;
 }
 
 ins {
+  border: solid var(--color-code-background);
   border-width: 1px;
-  border: solid var(--color-code-background); 
   padding: 1px;
   text-decoration: none;
 }
 
 mark {
   color: inherit;
   background-color: var(--color-highlight-deep);
@@ -204,16 +215,16 @@
 }
 
 /* Copy blocks */
 
 blockquote {
   margin-right: 3ch;
   margin-left: 1.5ch;
+  border: solid var(--color-code-background);
   border-width: 0 0 0 0.5ch;
-  border: solid var(--color-code-background); 
   padding: 0 0 0 1ch;
 }
 
 /* Pre-formatted text */
 
 code, pre, samp, kbd {
   color: var(--color-code-text); 
@@ -222,34 +233,33 @@
 }
 
 code, pre, samp {
   background-color: var(--color-code-background);
   border: solid var(--color-border);
 }
 
-code, samp {
+p code, p samp {
   border-width: 1px;
   border-radius: 2px;
   padding: 0.1em 0.2em;
   white-space: nowrap;
 }
 
 pre code {
   border: none;
-  padding: 0;
   background-color: transparent;
   white-space: inherit;
 }
 
 pre {
   margin-top: calc(1.5rem - 1px);
   margin-bottom: -1px;
   border-width: 1px;
   border-radius: 2px;
-  padding: 0 0.5ch;
+  padding: 1em;
   overflow-x: auto;
 }
 
 kbd { font-weight: var(--font-weight-bold); }
 
 /* Lists */
 
@@ -296,17 +306,17 @@
 }
 
 thead, tfoot {
   background-color: var(--color-code-background);
 }
 
 th, td {
-  border-width: 1px;
   padding: 0 0.5ch;
   border: solid var(--color-table-border);
+  border-width: 1px;
 }
 
 /* Thematic break (horizontal rule) */
 hr {
   border: 0;
   margin: 2em 0;
 }
```

