# Comparing `tmp/bulma_sphinx_theme-0.0.6.tar.gz` & `tmp/bulma_sphinx_theme-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bulma_sphinx_theme-0.0.6.tar", last modified: Mon May 29 16:20:06 2023, max compression
+gzip compressed data, was "bulma_sphinx_theme-0.0.7.tar", last modified: Wed May 31 04:20:28 2023, max compression
```

## Comparing `bulma_sphinx_theme-0.0.6.tar` & `bulma_sphinx_theme-0.0.7.tar`

### file list

```diff
@@ -1,193 +1,195 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:20:06.176795 bulma_sphinx_theme-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-29 16:19:43.939177 bulma_sphinx_theme-0.0.6/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-29 16:19:43.939177 bulma_sphinx_theme-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-29 16:19:43.939177 bulma_sphinx_theme-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-05-29 16:19:43.939177 bulma_sphinx_theme-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:19:43.939177 bulma_sphinx_theme-0.0.6/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    21234 2023-05-29 16:19:43.939177 bulma_sphinx_theme-0.0.6/docs/_static/favicon.png
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-29 16:19:43.939177 bulma_sphinx_theme-0.0.6/docs/_static/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-05-29 16:19:43.939177 bulma_sphinx_theme-0.0.6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-29 16:19:43.939177 bulma_sphinx_theme-0.0.6/docs/develop.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-29 16:19:43.939177 bulma_sphinx_theme-0.0.6/docs/examples/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/docs/examples/kitchen-sink/
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-29 16:19:43.939177 bulma_sphinx_theme-0.0.6/docs/examples/kitchen-sink/admonitions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-29 16:19:43.939177 bulma_sphinx_theme-0.0.6/docs/examples/kitchen-sink/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-05-29 16:19:43.939177 bulma_sphinx_theme-0.0.6/docs/examples/kitchen-sink/blocks.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8978 2023-05-29 16:19:43.939177 bulma_sphinx_theme-0.0.6/docs/examples/kitchen-sink/generic.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-05-29 16:19:43.939177 bulma_sphinx_theme-0.0.6/docs/examples/kitchen-sink/images.rst
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-29 16:19:43.939177 bulma_sphinx_theme-0.0.6/docs/examples/kitchen-sink/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-05-29 16:19:43.939177 bulma_sphinx_theme-0.0.6/docs/examples/kitchen-sink/lists.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12894 2023-05-29 16:19:43.939177 bulma_sphinx_theme-0.0.6/docs/examples/kitchen-sink/really-long.md
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-05-29 16:19:43.939177 bulma_sphinx_theme-0.0.6/docs/examples/kitchen-sink/sphinx-design.md
--rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-05-29 16:19:43.939177 bulma_sphinx_theme-0.0.6/docs/examples/kitchen-sink/structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-29 16:19:43.939177 bulma_sphinx_theme-0.0.6/docs/examples/kitchen-sink/tables.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/docs/examples/kitchen-sink/typography.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/docs/examples/mult_headers.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/docs/examples/reference/
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/docs/examples/reference/admonitions.md
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/docs/examples/reference/api.md
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/docs/examples/reference/code-blocks.md
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/docs/examples/reference/hyperlinks.md
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/docs/examples/reference/images.md
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/docs/examples/reference/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/docs/examples/reference/lists.md
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/docs/examples/reference/tables.md
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/docs/examples/reference/tabs.md
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/docs/examples/reference/text-formatting.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/docs/examples/subpages/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/docs/examples/subpages/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/docs/examples/subpages/subpage1.rst
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/docs/examples/subpages/subpage2.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/docs/examples/subpages/subsubpages/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/docs/examples/subpages/subsubpages/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/docs/examples/subpages/subsubpages/subsubpage1.rst
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/docs/examples/subpages/subsubpages/subsubpage2.rst
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/docs/examples/subpages/subsubpages/subsubpage3.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/docs/examples/subpages/subsubpages/subsubsubpages/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/docs/examples/subpages/subsubpages/subsubsubpages/subsubsubpage1.rst
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/docs/user_guide/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/docs/user_guide/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/docs/user_guide/navbar.md
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/docs/user_guide/sidenav.md
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/docs/user_guide/source-buttons.md
--rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/docs/web-components.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (123)   130410 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/package.json
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/postcss.config.js
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/
--rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)    10293 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/scripts/bulma-sphinx-theme.js
--rw-r--r--   0 runner    (1001) docker     (123)    12991 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/scripts/gumshoe-patched.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/abstracts/
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/abstracts/_mixins.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/base/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/base/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/base/_typography.scss
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/bulma-sphinx-theme.sass
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/components/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/components/_article-bottom.scss
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/components/_article-top.scss
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/components/_back-to-top.scss
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/components/_brand-logo.scss
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/components/_breadcrumbs.scss
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/components/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/components/_info-panel.scss
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/components/_last-updated.scss
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/components/_prev-next.scss
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/components/_search-button.scss
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/components/_search-field.sass
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/components/_search-results.scss
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/components/_search.sass
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/components/_sidenav-brand.scss
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/components/_switcher-theme.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/content/
--rw-r--r--   0 runner    (1001) docker     (123)     7994 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/content/_admonitions.scss
--rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/content/_api.scss
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/content/_blocks.sass
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/content/_code.scss
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/content/_footnotes.sass
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/content/_gui-labels.scss
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/content/_images.sass
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/content/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/content/_indexes.sass
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/content/_lists.scss
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/content/_math.sass
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/content/_misc.sass
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/content/_rubrics.sass
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/content/_sidebar.sass
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/content/_tables.sass
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/content/_target.sass
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/extensions/_ablog.scss
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/extensions/_docutils.scss
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/extensions/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/extensions/_notebooks.scss
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/extensions/_togglebutton.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/sections/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/sections/_bulma-content.scss
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/sections/_bulma-main.scss
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/sections/_bulma-sidenav.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/sections/_bulma-tocnav.scss
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/sections/_footer.scss
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/sections/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/sections/_navbar.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/variables/
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/variables/_admonitions.scss
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/variables/_color.scss
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/variables/_definition.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/variables/_fonts.scss
--rw-r--r--   0 runner    (1001) docker     (123)     6907 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/variables/_icons.scss
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/variables/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/variables/_layout.scss
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/variables/_spacing.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/translations/
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/translations/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/translations/jsons/
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/translations/jsons/Back to top.json
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/translations/jsons/Edit this page.json
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/translations/jsons/On this page.json
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/translations/jsons/with.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/demo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/demo/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/demo/sphinxext.py
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/pygment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/
--rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/back-to-top.html
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/brand-logo.html
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/breadcrumbs.html
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/copyright.html
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/edit-this-page.html
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/header-icons.html
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/info-panel.html
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/last-updated.html
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/navbar-nav.html
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/panel-test.html
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/prev-next.html
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-button.html
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-field.html
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-wrapper.html
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/searchbox.html
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sidenav-nav.html
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sourcelink.html
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sphinx-version.html
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/theme-swither.html
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/domainindex.html
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/genindex.html
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/globaltoc.html
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/localtoc.html
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/page.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/_css_variables_define.html
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/_icon_links_declare.html
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/icons.html
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/search.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-bottom.html
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-top.html
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/footer.html
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/headnav.html
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/sidenav.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/static/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/theme.conf
--rw-r--r--   0 runner    (1001) docker     (123)    17845 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/toctree.py
--rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/translations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/webpack.config.js
--rw-r--r--   0        0        0     4297 1970-01-01 00:00:00.000000 bulma_sphinx_theme-0.0.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:28.299621 bulma_sphinx_theme-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    21234 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/_static/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/_static/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/develop.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/kitchen-sink/
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/kitchen-sink/admonitions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/kitchen-sink/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/kitchen-sink/blocks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8978 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/kitchen-sink/generic.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/kitchen-sink/images.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/kitchen-sink/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/kitchen-sink/lists.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12894 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/kitchen-sink/really-long.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/kitchen-sink/sphinx-design.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/kitchen-sink/structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/kitchen-sink/tables.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/kitchen-sink/typography.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/mult_headers.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/reference/admonitions.md
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/reference/api.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/reference/code-blocks.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/reference/hyperlinks.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/reference/images.md
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/reference/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/reference/lists.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/reference/tables.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/reference/tabs.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/reference/text-formatting.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/subpages/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/subpages/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/subpages/subpage1.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/subpages/subpage2.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/subpages/subsubpages/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/subpages/subsubpages/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/subpages/subsubpages/subsubpage1.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/subpages/subsubpages/subsubpage2.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/subpages/subsubpages/subsubpage3.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/subpages/subsubpages/subsubsubpages/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/examples/subpages/subsubpages/subsubsubpages/subsubsubpage1.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/user_guide/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/user_guide/navbar.md
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/user_guide/sidenav.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/user_guide/source-buttons.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/docs/web-components.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)   130410 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/postcss.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/
+-rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)    11170 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/scripts/bulma-sphinx-theme.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12991 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/scripts/gumshoe-patched.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/abstracts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/abstracts/_mixins.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/base/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/base/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/base/_typography.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/bulma-sphinx-theme.sass
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/components/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/components/_article-bottom.scss
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-31 04:20:11.635501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/components/_article-top.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/components/_back-to-top.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/components/_brand-logo.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/components/_breadcrumbs.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/components/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/components/_info-panel.scss
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/components/_last-updated.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/components/_prev-next.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/components/_search-button.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/components/_search-field.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/components/_search-results.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/components/_search-wrapper.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/components/_search.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/components/_sidenav-brand.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/components/_switcher-theme.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/content/
+-rw-r--r--   0 runner    (1001) docker     (123)     7994 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/content/_admonitions.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/content/_api.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/content/_blocks.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/content/_code.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/content/_footnotes.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/content/_gui-labels.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/content/_images.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/content/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/content/_indexes.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/content/_lists.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/content/_math.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/content/_misc.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/content/_rubrics.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/content/_sidebar.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/content/_tables.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/content/_target.sass
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/extensions/_ablog.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/extensions/_bulma.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/extensions/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/extensions/_leaflet.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/extensions/_notebooks.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     6816 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/extensions/_sphinx-design.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/extensions/_togglebutton.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/sections/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/sections/_bulma-content.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/sections/_bulma-main.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/sections/_bulma-sidenav.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/sections/_bulma-tocnav.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/sections/_footer.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/sections/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/sections/_navbar.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/variables/_admonitions.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/variables/_color.scss
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/variables/_definition.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/variables/_fonts.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     6907 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/variables/_icons.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/variables/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/variables/_layout.scss
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/variables/_spacing.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/translations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/translations/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/translations/jsons/
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/translations/jsons/Back to top.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/translations/jsons/Edit this page.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/translations/jsons/On this page.json
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/translations/jsons/with.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/demo/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/demo/sphinxext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/pygment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/
+-rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/back-to-top.html
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/brand-logo.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/breadcrumbs.html
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/copyright.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/edit-this-page.html
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/header-icons.html
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/info-panel.html
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/last-updated.html
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/navbar-nav.html
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/prev-next.html
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-button.html
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-field.html
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-wrapper.html
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/searchbox.html
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sidenav-nav.html
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sourcelink.html
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sphinx-version.html
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/theme-swither.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/domainindex.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/genindex.html
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/globaltoc.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/localtoc.html
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/page.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/_css_variables_define.html
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/_icon_links_declare.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/icons.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/search.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-bottom.html
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-top.html
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/headnav.html
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/sidenav.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/static/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/theme.conf
+-rw-r--r--   0 runner    (1001) docker     (123)    17845 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/toctree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/translations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-05-31 04:20:11.639501 bulma_sphinx_theme-0.0.7/webpack.config.js
+-rw-r--r--   0        0        0     4297 1970-01-01 00:00:00.000000 bulma_sphinx_theme-0.0.7/PKG-INFO
```

### Comparing `bulma_sphinx_theme-0.0.6/LICENSE` & `bulma_sphinx_theme-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/README.md` & `bulma_sphinx_theme-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/docs/_static/favicon.png` & `bulma_sphinx_theme-0.0.7/docs/_static/favicon.png`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/docs/_static/logo.svg` & `bulma_sphinx_theme-0.0.7/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/docs/conf.py` & `bulma_sphinx_theme-0.0.7/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,28 +67,32 @@
     "header_links_before_dropdown": 5,
     "navbar_color_style": "is-white",  # see styles: https://bulma.io/documentation/components/navbar/#colors
     "logo": {"text": "Bulma Sphinx Theme", "logo": "_static/logo.svg"},
     "header_icons": [
         {
             "name": "Github",
             "url": "https://github.com/zclab/bulma-sphinx-theme",
-            "image": "https://www.svgrepo.com/show/433505/github-o.svg",
+            "svg": "github",
+        },
+        {
+            "name": "Pypi",
+            "url": "https://pypi.org/project/bulma-sphinx-theme/",
+            "svg": "package",
         },
         {
             "name": "Bulma",
             "url": "https://bulma.io/",
-            "image": "https://bulma.io/favicons/favicon.ico",
+            "svg": "bulma",
         },
+    ],
+    "external_links": [
         {
             "name": "Pydata",
             "url": "https://pydata-sphinx-theme.readthedocs.io/en/latest/",
-            "image": "https://pydata-sphinx-theme.readthedocs.io/en/latest/_static/pydata-logo.png",
         },
-    ],
-    "external_links": [
         {"name": "Furo", "url": "https://pradyunsg.me/furo/quickstart/"},
         {
             "name": "Sphinx book theme",
             "url": "https://sphinx-book-theme.readthedocs.io/en/latest/",
         },
         {
             "name": "Hugging Face community",
```

### Comparing `bulma_sphinx_theme-0.0.6/docs/develop.md` & `bulma_sphinx_theme-0.0.7/docs/develop.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/docs/examples/index.md` & `bulma_sphinx_theme-0.0.7/docs/examples/index.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/docs/examples/kitchen-sink/admonitions.rst` & `bulma_sphinx_theme-0.0.7/docs/examples/kitchen-sink/admonitions.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/docs/examples/kitchen-sink/api.rst` & `bulma_sphinx_theme-0.0.7/docs/examples/kitchen-sink/api.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/docs/examples/kitchen-sink/blocks.rst` & `bulma_sphinx_theme-0.0.7/docs/examples/kitchen-sink/blocks.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/docs/examples/kitchen-sink/generic.rst` & `bulma_sphinx_theme-0.0.7/docs/examples/kitchen-sink/generic.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/docs/examples/kitchen-sink/images.rst` & `bulma_sphinx_theme-0.0.7/docs/examples/kitchen-sink/images.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/docs/examples/kitchen-sink/index.md` & `bulma_sphinx_theme-0.0.7/docs/examples/kitchen-sink/index.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/docs/examples/kitchen-sink/lists.rst` & `bulma_sphinx_theme-0.0.7/docs/examples/kitchen-sink/lists.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/docs/examples/kitchen-sink/really-long.md` & `bulma_sphinx_theme-0.0.7/docs/examples/kitchen-sink/really-long.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/docs/examples/kitchen-sink/sphinx-design.md` & `bulma_sphinx_theme-0.0.7/docs/examples/kitchen-sink/sphinx-design.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/docs/examples/kitchen-sink/structure.rst` & `bulma_sphinx_theme-0.0.7/docs/examples/kitchen-sink/structure.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/docs/examples/kitchen-sink/tables.rst` & `bulma_sphinx_theme-0.0.7/docs/examples/kitchen-sink/tables.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/docs/examples/kitchen-sink/typography.rst` & `bulma_sphinx_theme-0.0.7/docs/examples/kitchen-sink/typography.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/docs/examples/mult_headers.rst` & `bulma_sphinx_theme-0.0.7/docs/examples/mult_headers.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/docs/examples/reference/admonitions.md` & `bulma_sphinx_theme-0.0.7/docs/examples/reference/admonitions.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/docs/examples/reference/api.md` & `bulma_sphinx_theme-0.0.7/docs/examples/reference/api.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/docs/examples/reference/code-blocks.md` & `bulma_sphinx_theme-0.0.7/docs/examples/reference/code-blocks.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/docs/examples/reference/hyperlinks.md` & `bulma_sphinx_theme-0.0.7/docs/examples/reference/hyperlinks.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/docs/examples/reference/images.md` & `bulma_sphinx_theme-0.0.7/docs/examples/reference/images.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/docs/examples/reference/index.md` & `bulma_sphinx_theme-0.0.7/docs/examples/reference/index.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/docs/examples/reference/lists.md` & `bulma_sphinx_theme-0.0.7/docs/examples/reference/lists.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/docs/examples/reference/tables.md` & `bulma_sphinx_theme-0.0.7/docs/examples/reference/tables.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/docs/examples/reference/tabs.md` & `bulma_sphinx_theme-0.0.7/docs/examples/reference/tabs.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/docs/examples/reference/text-formatting.md` & `bulma_sphinx_theme-0.0.7/docs/examples/reference/text-formatting.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/docs/examples/subpages/subpage1.rst` & `bulma_sphinx_theme-0.0.7/docs/examples/subpages/subpage1.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/docs/examples/subpages/subpage2.rst` & `bulma_sphinx_theme-0.0.7/docs/examples/subpages/subpage2.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/docs/examples/subpages/subsubpages/subsubpage1.rst` & `bulma_sphinx_theme-0.0.7/docs/examples/subpages/subsubpages/subsubpage1.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/docs/examples/subpages/subsubpages/subsubpage2.rst` & `bulma_sphinx_theme-0.0.7/docs/examples/subpages/subsubpages/subsubpage2.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/docs/examples/subpages/subsubpages/subsubpage3.rst` & `bulma_sphinx_theme-0.0.7/docs/examples/subpages/subsubpages/subsubpage3.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/docs/user_guide/navbar.md` & `bulma_sphinx_theme-0.0.7/docs/user_guide/navbar.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/docs/user_guide/source-buttons.md` & `bulma_sphinx_theme-0.0.7/docs/user_guide/source-buttons.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/docs/web-components.rst` & `bulma_sphinx_theme-0.0.7/docs/web-components.rst`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 :bdg-secondary:`secondary`
 :bdg-success:`success`
 :bdg-primary-line:`primary outline`
 :bdg-secondary-line:`secondary outline`
 :bdg-success-line:`success outline`
 
 Here are some buttons, also using semantic color names. **Note:** in this theme, ``info`` is defined to be the same color as ``primary``, and ``warning`` is the same color as ``secondary``.
-If in your site's `custom CSS file <custom-css>`_ you override the `CSS custom properties <css-variables>`_ ``--pst-color-*`` (where ``*`` is one of the semantic color names, e.g., ``primary``, ``danger``, etc), badges and buttons will automatically use the custom color.
+If in your site's `custom CSS file <custom-css>`_ you override the `CSS custom properties <css-variables>`_ ``--bst-color-*`` (where ``*`` is one of the semantic color names, e.g., ``primary``, ``danger``, etc), badges and buttons will automatically use the custom color.
 
 .. grid:: auto
 
     .. grid-item::
 
         .. button-ref:: badges-buttons
             :ref-type: ref
```

### Comparing `bulma_sphinx_theme-0.0.6/noxfile.py` & `bulma_sphinx_theme-0.0.7/noxfile.py`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/package-lock.json` & `bulma_sphinx_theme-0.0.7/package-lock.json`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/package.json` & `bulma_sphinx_theme-0.0.7/package.json`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/pyproject.toml` & `bulma_sphinx_theme-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/__init__.py` & `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from functools import lru_cache
 from pathlib import Path
 from typing import Any, Dict, List
 from sphinx.builders.html import StandaloneHTMLBuilder
 from sphinx.locale import get_translation
 from . import pygment, toctree, transforms, utils
 
-__version__ = "0.0.6"
+__version__ = "0.0.7"
 logger = logging.getLogger(__name__)
 MESSAGE_CATALOG_NAME = "bulmasphinxtheme"
 
 
 def _get_html_theme_path():
     """Return list of HTML theme paths."""
     parent = Path(__file__).parent.resolve()
```

### Comparing `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/scripts/bulma-sphinx-theme.js` & `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/scripts/bulma-sphinx-theme.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -301,15 +301,15 @@
     let overlay = document.querySelector(".search-button__overlay");
     if (overlay) {
         overlay.onclick = toggleSearchField;
     }
 };
 
 /*******************************************************************************
- * dropdown trigger setup for bulma, see https://bulma.io/lib/main.js?v=202305240833
+ * dropdown trigger setup for bulma, see https://bulma.io/lib/main.js?v=202305240833 and https://siongui.github.io/2018/01/19/bulma-dropdown-with-javascript/
  */
 
 function getAll(selector) {
     var parent =
         arguments.length > 1 && arguments[1] !== undefined ?
         arguments[1] :
         document;
@@ -339,21 +339,45 @@
         });
     }
 };
 /*******************************************************************************
  * dropdown trigger ended
  */
 
+/*******************************************************************************
+ * https://bulma.io/documentation/components/navbar/#navbar-menu
+ */
+function navbarBurger() {
+    // Get all "navbar-burger" elements
+    const $navbarBurgers = Array.prototype.slice.call(
+        document.querySelectorAll(".navbar-burger"),
+        0,
+    );
+
+    // Add a click event on each of them
+    $navbarBurgers.forEach((el) => {
+        el.addEventListener("click", () => {
+            // Get the target from the "data-target" attribute
+            const target = el.dataset.target;
+            const $target = document.getElementById(target);
+
+            // Toggle the "is-active" class on both the "navbar-burger" and the "navbar-menu"
+            el.classList.toggle("is-active");
+            $target.classList.toggle("is-active");
+        });
+    });
+}
 ////////////////////////////////////////////////////////////////////////////////
 // Main entrypoint
 ////////////////////////////////////////////////////////////////////////////////
 function main() {
     document.body.parentNode.classList.remove("no-js");
     addModeListener();
     setupSearchButtons();
     setupDropdwon();
+    navbarBurger();
     header = document.querySelector(".navbar");
     tocScroll = document.querySelector(".toc-scroll");
     setup();
 }
 
 document.addEventListener("DOMContentLoaded", main);
```

### Comparing `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/scripts/gumshoe-patched.js` & `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/scripts/gumshoe-patched.js`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/abstracts/_mixins.scss` & `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/abstracts/_mixins.scss`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 * SASS Mixins
 *********************************************/
 
 /**
  * A consistent box shadow style we apply across elements.
  */
 @mixin box-shadow() {
-  box-shadow: 0 0.2rem 0.5rem var(--bst-color-shadow),
+  box-shadow:
+    0 0.2rem 0.5rem var(--bst-color-shadow),
     0 0 0.0625rem var(--bst-color-shadow) !important;
 }
 
 /**
  * create a low opacity background behind object using our variable colors
  */
 @mixin background-from-color-variable($color-variable, $opacity: 0.1) {
```

### Comparing `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/base/_typography.scss` & `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/base/_typography.scss`

 * *Files 17% similar despite different names*

```diff
@@ -82,14 +82,19 @@
 }
 
 .columns {
   margin-left: 2rem;
   margin-right: 2rem;
   margin-top: 0;
 
+  @include touch {
+    margin-left: 1rem;
+    margin-right: 1rem;
+  }
+
   /* the columns:last-child fix body height have a small gap to screen bottom */
   &:last-child {
     margin-bottom: 0;
   }
 }
 
 strong {
@@ -104,7 +109,43 @@
     }
   }
 
   &.reference.download::before {
     content: url("data:image/svg+xml;charset=utf-8,%3Csvg width='16' height='16' xmlns='http://www.w3.org/2000/svg' viewBox='0 0 24 24' stroke-width='1.5' stroke='%23607D8B' fill='none' stroke-linecap='round' stroke-linejoin='round'%3E%3Cpath d='M0 0h24v24H0z' stroke='none'/%3E%3Cpath d='M4 17v2a2 2 0 0 0 2 2h12a2 2 0 0 0 2 -2v-2'/%3E%3Cpath d='M7 11l5 5l5 -5'/%3E%3Cpath d='M12 4l0 12'/%3E%3C/svg%3E");
   }
 }
+
+svg {
+  &.svg-bulma,
+  &.svg-github,
+  &.svg-gitlab,
+  &.svg-home,
+  &.svg-pencil,
+  &.svg-file-description,
+  &.svg-clock-edit,
+  &.svg-search,
+  &.svg-package,
+  &.svg-sun,
+  &.svg-sunset,
+  &.svg-moon {
+    width: 100%;
+    height: 100%;
+  }
+}
+
+html[data-theme="dark"] {
+  svg {
+    &.svg-github,
+    &.svg-gitlab,
+    &.svg-home,
+    &.svg-pencil,
+    &.svg-file-description,
+    &.svg-clock-edit,
+    &.svg-search,
+    &.svg-package,
+    &.svg-sun,
+    &.svg-sunset,
+    &.svg-moon {
+      filter: hue-rotate(40deg) saturate(0.5) brightness(390%) saturate(4);
+    }
+  }
+}
```

### Comparing `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/components/_back-to-top.scss` & `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/components/_back-to-top.scss`

 * *Files 13% similar despite different names*

```diff
@@ -8,15 +8,17 @@
   // top: 1rem;
   padding: 0.5rem;
   padding-right: 0.75rem;
   border-radius: 1.2rem;
   font-size: 1rem;
 
   background: var(--bst-color-background);
-  box-shadow: 0 0.2rem 0.5rem rgba(0, 0, 0, 0.05), #6b728080 0px 0px 1px 0px;
+  box-shadow:
+    0 0.2rem 0.5rem rgba(0, 0, 0, 0.05),
+    #6b728080 0px 0px 1px 0px;
 
   z-index: 10;
 
   margin-left: 50%;
   transform: translateX(-50%);
 
   svg {
```

### Comparing `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/components/_prev-next.scss` & `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/components/_prev-next.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/components/_search-button.scss` & `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/components/_search-wrapper.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/components/_switcher-theme.scss` & `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/components/_switcher-theme.scss`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,16 @@
   width: fit-content;
   aspect-ratio: 1 / 1;
   background: none;
   border: none;
 
   span {
     display: none;
-    padding: 0.5em;
+    height: 100%;
+    width: 100%;
 
     &:hover,
     &:active,
     &:focus {
       text-decoration: none;
       color: var(--bst-color-primary);
     }
```

### Comparing `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/content/_admonitions.scss` & `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/content/_admonitions.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/content/_api.scss` & `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/content/_api.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/content/_code.scss` & `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/content/_code.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/content/_footnotes.sass` & `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/content/_footnotes.sass`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/content/_images.sass` & `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/content/_images.sass`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/content/_lists.scss` & `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/content/_lists.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/content/_misc.sass` & `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/content/_misc.sass`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/content/_sidebar.sass` & `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/content/_sidebar.sass`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/content/_tables.sass` & `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/content/_tables.sass`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/content/_target.sass` & `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/content/_target.sass`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/extensions/_ablog.scss` & `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/extensions/_ablog.scss`

 * *Files 3% similar despite different names*

```diff
@@ -106,29 +106,35 @@
 .ablog__collection,
 .postlist {
   padding-left: 0;
 
   .ablog-post {
     list-style: none;
 
+    ul.ablog-archive {
+      & > li {
+        list-style: none;
+      }
+    }
+
     // Post metadata tags (author, links ,etc) should be a bit smaller
     .ablog-archive {
       display: flex;
       flex-direction: row;
       flex-wrap: wrap;
       gap: 1rem;
       list-style: none;
       font-size: 0.75rem;
-      // padding-left: 0;
+      padding-left: 0;
     }
 
     // Title line should be a bit bigger and bold to stand out
     .ablog-post-title {
       margin-top: 0;
-      font-size: 1.25rem;
+      font-size: $size-4;
 
       a {
         font-weight: bold;
       }
     }
 
     // Read more button should be a bit bigger
```

### Comparing `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/sections/_bulma-sidenav.scss` & `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/sections/_bulma-sidenav.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/sections/_bulma-tocnav.scss` & `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/sections/_bulma-tocnav.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/sections/_navbar.scss` & `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/sections/_navbar.scss`

 * *Files 16% similar despite different names*

```diff
@@ -4,8 +4,14 @@
   .navbar-item {
     &.nav-external:after {
       content: url("data:image/svg+xml;charset=utf-8,%3Csvg width='16' height='16' xmlns='http://www.w3.org/2000/svg' viewBox='0 0 24 24' stroke-width='1.5' stroke='%23607D8B' fill='none' stroke-linecap='round' stroke-linejoin='round'%3E%3Cpath d='M0 0h24v24H0z' stroke='none'/%3E%3Cpath d='M11 7H6a2 2 0 0 0-2 2v9a2 2 0 0 0 2 2h9a2 2 0 0 0 2-2v-5M10 14 20 4M15 4h5v5'/%3E%3C/svg%3E");
       margin-left: 0.3rem;
       margin-top: 0.2rem;
     }
   }
+
+  a.navbar-item.ext-link {
+    @include touch {
+      display: inline-block;
+    }
+  }
 }
```

### Comparing `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/variables/_admonitions.scss` & `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/variables/_admonitions.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/variables/_color.scss` & `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/variables/_color.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/variables/_fonts.scss` & `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/variables/_fonts.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/variables/_icons.scss` & `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/styles/variables/_icons.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/translations/README.md` & `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/translations/README.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/translations/jsons/Edit this page.json` & `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/translations/jsons/Edit this page.json`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/translations/jsons/On this page.json` & `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/assets/translations/jsons/On this page.json`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/demo/module.py` & `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/demo/module.py`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/demo/sphinxext.py` & `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/demo/sphinxext.py`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/pygment.py` & `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/pygment.py`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/base.html` & `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/base.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/breadcrumbs.html` & `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/breadcrumbs.html`

 * *Files 27% similar despite different names*

```diff
@@ -12,27 +12,26 @@
 {% endif %}
 {# djlint:on #}
 
 {#- Hide breadcrumbs on the home page #}
 {% if title and pagename != root_doc %}
 <nav class="breadcrumb" aria-label="breadcrumbs">
     <ul>
-        <li><a href="{{ pathto(root_doc) }}"><svg xmlns="http://www.w3.org/2000/svg"
-                    class="icon icon-tabler icon-tabler-home" width="44" height="44" viewBox="0 0 24 24"
-                    stroke-width="1.5" stroke="#2c3e50" fill="none" stroke-linecap="round" stroke-linejoin="round">
-                    <path stroke="none" d="M0 0h24v24H0z" fill="none" />
-                    <path d="M5 12l-2 0l9 -9l9 9l-2 0" />
-                    <path d="M5 12v7a2 2 0 0 0 2 2h10a2 2 0 0 0 2 -2v-7" />
-                    <path d="M9 21v-6a2 2 0 0 1 2 -2h2a2 2 0 0 1 2 2v6" />
-                </svg></a></li>
+        <li>
+            <a href="{{ pathto(root_doc) }}" title="home">
+                <svg class="svg-home">
+                    <use href="#svg-home"></use>
+                </svg>
+            </a>
+        </li>
         {%- for doc in parents %}
         {% if doc.link %}
         <li><a href="{{ doc.link|e }}">{{ doc.title }}</a></li>
         {% else %}
         <li><a href="#">{{ doc.title }}</a></li>
         {% endif %}
         {%- endfor %}
-        <li><a class="is-active" aria-current="page">{{ title }}</a></li>
+        <li><span class="breadcrumb-last-item" aria-current="page">{{ title }}</span></li>
     </ul>
 </nav>
 {% endif %}
 {%- endblock %}
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
 {%- block breadcrumbs %} {# If we have more than 3 parents (excluding the home
 page) then we remove The ones in the middle and add an ellipsis. This code is
 from https://github.com/pydata/pydata-sphinx-theme/blob/main/src/
 pydata_sphinx_theme/theme/pydata_sphinx_theme/components/breadcrumbs.html #} {#
 djlint:off #} {% if parents|length>2 %} {% set parents=[parents[0], {"title":
 '•••'}, parents[-1]] %} {% endif %} {# djlint:on #} {#- Hide breadcrumbs on the
 home page #} {% if title and pagename != root_doc %}
-    * ___
+    * __
     * {%- for doc in parents %} {% if doc.link %}
     * {{_doc.title_}}
     * {% else %}
     * {{_doc.title_}}
     * {% endif %} {%- endfor %}
     * {{ title }}
  {% endif %} {%- endblock %}
```

### Comparing `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/edit-this-page.html` & `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/edit-this-page.html`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 {% extends "basic-ng/components/edit-this-page.html" %}
 {% from "basic-ng/components/edit-this-page.html" import determine_page_edit_link with context %}
 
 {%- macro page_edit_button(url) -%}
 {% if theme_use_edit_page_button %}
 <a class="edit-this-page level-item" href="{{ url }}" title="{{ translate('Edit this page') }}">
-    <svg xmlns="http://www.w3.org/2000/svg" class="icon icon-tabler icon-tabler-pencil" width="44" height="44"
-        viewBox="0 0 24 24" stroke-width="1.5" stroke="#2c3e50" fill="none" stroke-linecap="round"
-        stroke-linejoin="round">
-        <path stroke="none" d="M0 0h24v24H0z" fill="none" />
-        <path d="M4 20h4l10.5 -10.5a1.5 1.5 0 0 0 -4 -4l-10.5 10.5v4" />
-        <path d="M13.5 6.5l4 4" />
-    </svg> {% if not show_source %} {{ translate('Edit this page') }} {% endif %}
+    <span class="icon">
+        <svg class="svg-pencil">
+            <use href="#svg-pencil"></use>
+        </svg>
+    </span> {% if not show_source %} {{ translate('Edit this page') }} {% endif %}
 </a>
 {% endif %}
 {%- endmacro -%}
 
 {% block link_available -%}
 {{ page_edit_button(determine_page_edit_link()) }}
 {%- endblock link_available %}
```

### Comparing `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/prev-next.html` & `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/prev-next.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-field.html` & `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-field.html`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 <form class="search-wrapper control is-expanded" method="get" action="{{ pathto('search') }}" role="search">
-    <svg xmlns="http://www.w3.org/2000/svg" class="icon icon-tabler icon-tabler-search" width="44" height="44"
-        viewBox="0 0 24 24" stroke-width="1.5" stroke="#2c3e50" fill="none" stroke-linecap="round"
-        stroke-linejoin="round">
-        <path stroke="none" d="M0 0h24v24H0z" fill="none" />
-        <path d="M10 10m-7 0a7 7 0 1 0 14 0a7 7 0 1 0 -14 0" />
-        <path d="M21 21l-6 -6" />
-    </svg>
+    <span class="icon">
+        <svg class="svg-search">
+            <use href="#svg-search"></use>
+        </svg>
+    </span>
     <input class="input" placeholder="{{ theme_search_bar_text }}" name="q" aria-label="{{ theme_search_bar_text }}"
         autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false" />
     <span class="search-button__kbd-shortcut"><kbd class="kbd-shortcut__esc">ESC</kbd></span>
 </form>
```

### Comparing `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/domainindex.html` & `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/domainindex.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/genindex.html` & `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/genindex.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/layout.html` & `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/layout.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/_icon_links_declare.html` & `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/_icon_links_declare.html`

 * *Files 20% similar despite different names*

```diff
@@ -5,14 +5,20 @@
 {% if icon_list -%}
 {% for icon_dict in icon_list -%}
 <a href="{{ icon_dict.url }}" target="_blank" title="{{ icon_dict.name }}" class="{{ icon_class }} ext-link">
     {% if icon_dict.class %}
     <i class="{{ icon_dict.class }}"></i>
     {% elif icon_dict.material_icons %}
     <i class="material-icons">{{ icon_dict.material_icons }}</i>
+    {% elif icon_dict.svg %}
+    <span class="icon">
+        <svg class="svg-{{ icon_dict.svg }}">
+            <use href="#svg-{{ icon_dict.svg }}"></use>
+        </svg>
+    </span>
     {% elif icon_dict.fontawesome %}
     <i class="{{ icon_dict.fontawesome }}"></i>
     {% elif icon_dict.image %}
     <img src="{{ icon_dict.image }}" class="bulma-icon-image" alt="{{ icon_dict.name }}" />
     {% endif %}
 </a>
 {% endfor %}
```

#### html2text {}

```diff
@@ -1,7 +1,8 @@
 {# This is where user-provided CSS variables get converted into actual values.
 #} {% macro declare_icon_links(icon_list, icon_class="") -%} {% if icon_list -
 %} {% for icon_dict in icon_list -%}
 {%_if_icon_dict.class_%}__{%_elif_icon_dict.material_icons_%}_{
-{_icon_dict.material_icons_}}_{%_elif_icon_dict.fontawesome_%}__{%_elif
-icon_dict.image_%}_[{{_icon_dict.name_}}]_{%_endif_%}
+{_icon_dict.material_icons_}}_{%_elif_icon_dict.svg_%}______{%_elif
+icon_dict.fontawesome_%}__{%_elif_icon_dict.image_%}_[{{_icon_dict.name_}}]_{%
+endif_%}
  {% endfor %} {%- endif %} {%- endmacro %}
```

### Comparing `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/search.html` & `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/search.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-bottom.html` & `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-bottom.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-top.html` & `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-top.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/headnav.html` & `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/headnav.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 <div class="navbar-brand">
     {% include "components/brand-logo.html" %}
 
-    <a role="button" class="navbar-burger" aria-label="menu" aria-expanded="false" data-target="navbarBasicExample">
+    <a role="button" class="navbar-burger" aria-label="menu" aria-expanded="false" data-target="navMenu">
         <span aria-hidden="true"></span>
         <span aria-hidden="true"></span>
         <span aria-hidden="true"></span>
     </a>
 </div>
 
-<div class="navbar-menu">
+<div class="navbar-menu" id="navMenu">
     <div class="navbar-start">
         {% if theme_navbar_start %}
         {%- for ns_section in theme_navbar_start %}
         {% if ns_section in theme_navbar_include_directly %}
         {%- include ns_section %}
         {% else %}
         <div class="navbar-item">
```

### Comparing `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/theme.conf` & `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/theme.conf`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/toctree.py` & `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/toctree.py`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/transforms.py` & `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/transforms.py`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/translations.py` & `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/translations.py`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/utils.py` & `bulma_sphinx_theme-0.0.7/src/bulma_sphinx_theme/utils.py`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/webpack.config.js` & `bulma_sphinx_theme-0.0.7/webpack.config.js`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.6/PKG-INFO` & `bulma_sphinx_theme-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bulma-sphinx-theme
-Version: 0.0.6
+Version: 0.0.7
 Summary: A sphinx theme based on bulma.
 Author-Email: zclab <syfhub@hotmail.com>
 License: MIT License
         
         Copyright (c) 2023 zc
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bulma-sphinx-theme Version: 0.0.6 Summary: A sphinx
+Metadata-Version: 2.1 Name: bulma-sphinx-theme Version: 0.0.7 Summary: A sphinx
 theme based on bulma. Author-Email: zclab
 hotmail.com> License: MIT License Copyright (c) 2023 zc Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

