# Comparing `tmp/spotPython-0.2.3.tar.gz` & `tmp/spotPython-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotPython-0.2.3.tar", last modified: Tue May 30 10:31:02 2023, max compression
+gzip compressed data, was "spotPython-0.2.4.tar", last modified: Wed May 31 08:16:52 2023, max compression
```

## Comparing `spotPython-0.2.3.tar` & `spotPython-0.2.4.tar`

### file list

```diff
@@ -1,232 +1,235 @@
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-30 10:31:02.428861 spotPython-0.2.3/
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-30 10:31:02.285442 spotPython-0.2.3/.github/
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-30 10:31:02.294863 spotPython-0.2.3/.github/workflows/
--rw-r--r--   0 bartz      (501) staff       (20)      557 2023-02-06 07:52:23.000000 spotPython-0.2.3/.github/workflows/test.yml
--rw-r--r--   0 bartz      (501) staff       (20)    12811 2023-05-20 22:36:38.000000 spotPython-0.2.3/.gitignore
--rw-r--r--   0 bartz      (501) staff       (20)        0 2023-05-19 14:54:05.000000 spotPython-0.2.3/.nojekyll
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-30 10:31:02.320898 spotPython-0.2.3/Figures.d/
--rw-r--r--   0 bartz      (501) staff       (20)    21113 2023-04-27 07:21:33.000000 spotPython-0.2.3/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_contour_1_2.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     5878 2023-04-27 07:21:33.000000 spotPython-0.2.3/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_importance.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     6563 2023-04-27 07:21:33.000000 spotPython-0.2.3/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_progress.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    26562 2023-04-27 07:21:33.000000 spotPython-0.2.3/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_contour_2_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     8850 2023-04-27 07:21:33.000000 spotPython-0.2.3/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_importance.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     6569 2023-04-27 07:21:33.000000 spotPython-0.2.3/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_progress.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    20478 2023-05-09 07:21:36.000000 spotPython-0.2.3/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_1.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    20590 2023-05-09 07:21:36.000000 spotPython-0.2.3/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_2.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    23054 2023-05-09 07:21:36.000000 spotPython-0.2.3/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22138 2023-05-09 07:21:36.000000 spotPython-0.2.3/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    21534 2023-05-09 07:21:36.000000 spotPython-0.2.3/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_2.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22805 2023-05-09 07:21:36.000000 spotPython-0.2.3/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22098 2023-05-09 07:21:36.000000 spotPython-0.2.3/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    23275 2023-05-09 07:21:36.000000 spotPython-0.2.3/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_2_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    21965 2023-05-09 07:21:36.000000 spotPython-0.2.3/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_2_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22913 2023-05-09 07:21:36.000000 spotPython-0.2.3/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_3_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     9680 2023-05-09 07:21:36.000000 spotPython-0.2.3/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_importance.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     6536 2023-05-09 07:21:36.000000 spotPython-0.2.3/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_progress.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    21132 2023-05-09 07:21:36.000000 spotPython-0.2.3/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_1.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    21651 2023-05-09 07:21:36.000000 spotPython-0.2.3/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_2.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22154 2023-05-09 07:21:36.000000 spotPython-0.2.3/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    21347 2023-05-09 07:21:36.000000 spotPython-0.2.3/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22265 2023-05-09 07:21:36.000000 spotPython-0.2.3/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_2.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22056 2023-05-09 07:21:36.000000 spotPython-0.2.3/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22224 2023-05-09 07:21:36.000000 spotPython-0.2.3/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    23950 2023-05-09 07:21:36.000000 spotPython-0.2.3/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_2_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    23161 2023-05-09 07:21:36.000000 spotPython-0.2.3/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_2_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22297 2023-05-09 07:21:36.000000 spotPython-0.2.3/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_3_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     9681 2023-05-09 07:21:36.000000 spotPython-0.2.3/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_importance.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     8189 2023-05-09 07:21:36.000000 spotPython-0.2.3/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_progress.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22759 2023-05-09 07:21:36.000000 spotPython-0.2.3/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_1_2.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    24775 2023-05-09 07:21:36.000000 spotPython-0.2.3/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_1_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    23126 2023-05-09 07:21:36.000000 spotPython-0.2.3/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_2_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     8905 2023-05-09 07:21:36.000000 spotPython-0.2.3/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_importance.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     7635 2023-05-09 07:21:36.000000 spotPython-0.2.3/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_progress.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    24695 2023-05-09 07:21:36.000000 spotPython-0.2.3/Figures.d/13-torch_s7cfd16_600min_20init_2023-05-05_18-52-19_contour_2_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    34523 2023-01-31 08:03:34.000000 spotPython-0.2.3/LICENSE.txt
--rw-r--r--   0 bartz      (501) staff       (20)       71 2023-04-26 06:49:16.000000 spotPython-0.2.3/MANIFEST.in
--rw-r--r--   0 bartz      (501) staff       (20)     7347 2023-05-30 10:31:02.428434 spotPython-0.2.3/PKG-INFO
--rw-r--r--   0 bartz      (501) staff       (20)     6577 2023-05-24 07:02:54.000000 spotPython-0.2.3/README.md
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-30 10:31:02.328510 spotPython-0.2.3/docs/
--rw-r--r--   0 bartz      (501) staff       (20)   208086 2023-05-29 21:15:55.000000 spotPython-0.2.3/docs/bart23e.html
--rw-r--r--   0 bartz      (501) staff       (20)   713146 2023-05-29 21:15:55.000000 spotPython-0.2.3/docs/bart23e.pdf
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-30 10:31:02.336164 spotPython-0.2.3/docs/figures/
--rw-r--r--   0 bartz      (501) staff       (20)    88272 2023-05-29 21:15:55.000000 spotPython-0.2.3/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_1.png
--rw-r--r--   0 bartz      (501) staff       (20)    84164 2023-05-29 21:15:55.000000 spotPython-0.2.3/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_3.png
--rw-r--r--   0 bartz      (501) staff       (20)    93300 2023-05-29 21:15:55.000000 spotPython-0.2.3/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_4.png
--rw-r--r--   0 bartz      (501) staff       (20)    84900 2023-05-29 21:15:55.000000 spotPython-0.2.3/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_3.png
--rw-r--r--   0 bartz      (501) staff       (20)    94821 2023-05-29 21:15:55.000000 spotPython-0.2.3/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_4.png
--rw-r--r--   0 bartz      (501) staff       (20)    92856 2023-05-29 21:15:55.000000 spotPython-0.2.3/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_3_4.png
--rw-r--r--   0 bartz      (501) staff       (20)    21443 2023-05-29 21:15:55.000000 spotPython-0.2.3/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_importance.png
--rw-r--r--   0 bartz      (501) staff       (20)    26414 2023-05-29 21:15:55.000000 spotPython-0.2.3/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_progress.png
--rw-r--r--   0 bartz      (501) staff       (20)    94077 2023-05-20 22:36:32.000000 spotPython-0.2.3/docs/figures/parallel.png
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-30 10:31:02.336917 spotPython-0.2.3/docs/img/
--rw-r--r--   0 bartz      (501) staff       (20)    67674 2023-05-19 14:54:05.000000 spotPython-0.2.3/docs/img/spotLogo.png
--rw-r--r--   0 bartz      (501) staff       (20)      231 2023-05-19 14:54:05.000000 spotPython-0.2.3/docs/index.html
--rw-r--r--   0 bartz      (501) staff       (20)    64921 2023-05-29 21:15:55.000000 spotPython-0.2.3/docs/search.json
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-30 10:31:02.286683 spotPython-0.2.3/docs/site_libs/
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-30 10:31:02.344694 spotPython-0.2.3/docs/site_libs/bootstrap/
--rw-r--r--   0 bartz      (501) staff       (20)    95517 2023-05-19 14:54:05.000000 spotPython-0.2.3/docs/site_libs/bootstrap/bootstrap-icons.css
--rw-r--r--   0 bartz      (501) staff       (20)   164168 2023-05-19 14:54:05.000000 spotPython-0.2.3/docs/site_libs/bootstrap/bootstrap-icons.woff
--rw-r--r--   0 bartz      (501) staff       (20)   308771 2023-05-19 14:54:05.000000 spotPython-0.2.3/docs/site_libs/bootstrap/bootstrap.min.css
--rw-r--r--   0 bartz      (501) staff       (20)    78129 2023-05-19 14:54:05.000000 spotPython-0.2.3/docs/site_libs/bootstrap/bootstrap.min.js
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-30 10:31:02.346180 spotPython-0.2.3/docs/site_libs/clipboard/
--rw-r--r--   0 bartz      (501) staff       (20)     9160 2023-05-19 14:54:05.000000 spotPython-0.2.3/docs/site_libs/clipboard/clipboard.min.js
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-30 10:31:02.350255 spotPython-0.2.3/docs/site_libs/quarto-html/
--rw-r--r--   0 bartz      (501) staff       (20)     6008 2023-05-19 14:54:05.000000 spotPython-0.2.3/docs/site_libs/quarto-html/anchor.min.js
--rw-r--r--   0 bartz      (501) staff       (20)    19728 2023-05-19 14:54:05.000000 spotPython-0.2.3/docs/site_libs/quarto-html/popper.min.js
--rw-r--r--   0 bartz      (501) staff       (20)     3135 2023-05-19 14:54:05.000000 spotPython-0.2.3/docs/site_libs/quarto-html/quarto-syntax-highlighting.css
--rw-r--r--   0 bartz      (501) staff       (20)    28407 2023-05-19 14:54:05.000000 spotPython-0.2.3/docs/site_libs/quarto-html/quarto.js
--rw-r--r--   0 bartz      (501) staff       (20)     1409 2023-05-19 14:54:05.000000 spotPython-0.2.3/docs/site_libs/quarto-html/tippy.css
--rw-r--r--   0 bartz      (501) staff       (20)    24033 2023-05-19 14:54:05.000000 spotPython-0.2.3/docs/site_libs/quarto-html/tippy.umd.min.js
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-30 10:31:02.351017 spotPython-0.2.3/docs/site_libs/quarto-nav/
--rw-r--r--   0 bartz      (501) staff       (20)     8250 2023-05-19 14:54:05.000000 spotPython-0.2.3/docs/site_libs/quarto-nav/quarto-nav.js
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-30 10:31:02.353479 spotPython-0.2.3/docs/site_libs/quarto-search/
--rw-r--r--   0 bartz      (501) staff       (20)    70711 2023-05-19 14:54:05.000000 spotPython-0.2.3/docs/site_libs/quarto-search/autocomplete.umd.js
--rw-r--r--   0 bartz      (501) staff       (20)    23539 2023-05-19 14:54:05.000000 spotPython-0.2.3/docs/site_libs/quarto-search/fuse.min.js
--rw-r--r--   0 bartz      (501) staff       (20)    32789 2023-05-19 14:54:05.000000 spotPython-0.2.3/docs/site_libs/quarto-search/quarto-search.js
--rwxr-xr-x   0 bartz      (501) staff       (20)      123 2023-04-27 07:21:33.000000 spotPython-0.2.3/makeSpot.sh
--rw-r--r--   0 bartz      (501) staff       (20)      437 2023-01-31 08:03:34.000000 spotPython-0.2.3/mkdocs.yml
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-30 10:31:02.382318 spotPython-0.2.3/notebooks/
--rw-r--r--   0 bartz      (501) staff       (20)    34275 2023-05-20 22:36:32.000000 spotPython-0.2.3/notebooks/00_spot_doc.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)     6585 2023-05-09 07:21:36.000000 spotPython-0.2.3/notebooks/01_spot_intro.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)     8780 2023-05-20 22:36:32.000000 spotPython-0.2.3/notebooks/02_spot_multidim.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)     9719 2023-05-09 07:21:36.000000 spotPython-0.2.3/notebooks/03_spot_anisotropic.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)    15781 2023-05-09 07:21:36.000000 spotPython-0.2.3/notebooks/04_spot_sklearn_surrogate.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)     8787 2023-05-09 07:21:36.000000 spotPython-0.2.3/notebooks/05_spot_sklearn_optimizers.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)    14206 2023-05-09 07:21:36.000000 spotPython-0.2.3/notebooks/06_spot_gaussian.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)    36749 2023-05-09 07:21:36.000000 spotPython-0.2.3/notebooks/07_spot_ei.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)    11665 2023-05-09 07:21:36.000000 spotPython-0.2.3/notebooks/08_spot_noisy.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)    12100 2023-05-09 07:21:36.000000 spotPython-0.2.3/notebooks/09_spot_ocba.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)   125645 2023-05-20 22:36:32.000000 spotPython-0.2.3/notebooks/10_spot_hpt_sklearn_classification.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)    23403 2023-05-29 21:15:55.000000 spotPython-0.2.3/notebooks/11_spot_hpt_torch_fashion_mnist.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)    28481 2023-05-29 21:15:55.000000 spotPython-0.2.3/notebooks/12_spot_hpt_torch_cifar10.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)    22216 2023-05-20 22:36:32.000000 spotPython-0.2.3/notebooks/13_spot_hpt_torch_cv_fashion_mnist.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)   110777 2023-05-29 21:15:55.000000 spotPython-0.2.3/notebooks/14_spot_ray_hpt_torch_cifar10.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)    26705 2023-05-20 22:36:32.000000 spotPython-0.2.3/notebooks/15_spot_hpt_sklearn_regression.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)    36437 2023-05-30 10:21:54.000000 spotPython-0.2.3/notebooks/16_spot_hpt_sklearn_multiclass_classification.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)    34620 2023-05-30 10:21:12.000000 spotPython-0.2.3/notebooks/17_spot_hpt_sklearn_multiclass_classification_xgb.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)    34402 2023-05-30 10:21:30.000000 spotPython-0.2.3/notebooks/18_spot_hpt_sklearn_multiclass_classification_svc.ipynb
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-30 10:31:02.287032 spotPython-0.2.3/notebooks/data/
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-30 10:31:02.382896 spotPython-0.2.3/notebooks/data/torch/
--rw-r--r--   0 bartz      (501) staff       (20)    77195 2023-05-16 06:49:47.000000 spotPython-0.2.3/notebooks/data/torch/model_spot_trained.pt
--rw-r--r--   0 bartz      (501) staff       (20)      359 2023-03-26 17:32:36.000000 spotPython-0.2.3/notebooks/data.json
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-30 10:31:02.392772 spotPython-0.2.3/notebooks/figures/
--rw-r--r--   0 bartz      (501) staff       (20)    88272 2023-05-29 21:15:55.000000 spotPython-0.2.3/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_1.png
--rw-r--r--   0 bartz      (501) staff       (20)    84164 2023-05-29 21:15:55.000000 spotPython-0.2.3/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_3.png
--rw-r--r--   0 bartz      (501) staff       (20)    93300 2023-05-29 21:15:55.000000 spotPython-0.2.3/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_4.png
--rw-r--r--   0 bartz      (501) staff       (20)    84900 2023-05-29 21:15:55.000000 spotPython-0.2.3/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_3.png
--rw-r--r--   0 bartz      (501) staff       (20)    94821 2023-05-29 21:15:55.000000 spotPython-0.2.3/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_4.png
--rw-r--r--   0 bartz      (501) staff       (20)    92856 2023-05-29 21:15:55.000000 spotPython-0.2.3/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_3_4.png
--rw-r--r--   0 bartz      (501) staff       (20)    21443 2023-05-29 21:15:55.000000 spotPython-0.2.3/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_importance.png
--rw-r--r--   0 bartz      (501) staff       (20)    26414 2023-05-29 21:15:55.000000 spotPython-0.2.3/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_progress.png
--rw-r--r--   0 bartz      (501) staff       (20)   121376 2023-05-29 21:15:55.000000 spotPython-0.2.3/notebooks/figures/figures14-torch_maans03_60min_20init_2023-05-27_23-10-01_parallel.png
--rw-r--r--   0 bartz      (501) staff       (20)   115822 2023-01-31 08:03:34.000000 spotPython-0.2.3/notebooks/figures/spotModel.graffle
--rw-r--r--   0 bartz      (501) staff       (20)    26289 2023-01-31 08:03:34.000000 spotPython-0.2.3/notebooks/figures/spotModel.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    64603 2023-01-31 08:03:34.000000 spotPython-0.2.3/notebooks/figures/spotModel.png
--rw-r--r--   0 bartz      (501) staff       (20)    21112 2023-05-23 07:24:48.000000 spotPython-0.2.3/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_0_1.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    21979 2023-05-23 07:24:48.000000 spotPython-0.2.3/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_0_2.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    23390 2023-05-23 07:24:48.000000 spotPython-0.2.3/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_0_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22172 2023-05-23 07:24:48.000000 spotPython-0.2.3/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_1_2.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    23463 2023-05-23 07:24:48.000000 spotPython-0.2.3/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_1_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    24987 2023-05-23 07:24:48.000000 spotPython-0.2.3/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_2_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    10009 2023-05-23 07:24:48.000000 spotPython-0.2.3/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_importance.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     7783 2023-05-23 07:24:48.000000 spotPython-0.2.3/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_progress.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    21663 2023-05-24 07:02:54.000000 spotPython-0.2.3/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_0_1.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22544 2023-05-24 07:02:54.000000 spotPython-0.2.3/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_0_2.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22042 2023-05-24 07:02:54.000000 spotPython-0.2.3/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_0_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    21676 2023-05-24 07:02:54.000000 spotPython-0.2.3/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_1_2.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    21232 2023-05-24 07:02:54.000000 spotPython-0.2.3/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_1_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22317 2023-05-24 07:02:54.000000 spotPython-0.2.3/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_2_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     9376 2023-05-24 07:02:54.000000 spotPython-0.2.3/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_importance.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     6836 2023-05-24 07:02:54.000000 spotPython-0.2.3/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_progress.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22179 2023-05-20 22:36:32.000000 spotPython-0.2.3/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_1.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    21553 2023-05-20 22:36:32.000000 spotPython-0.2.3/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    23439 2023-05-20 22:36:32.000000 spotPython-0.2.3/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22108 2023-05-20 22:36:32.000000 spotPython-0.2.3/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    23180 2023-05-20 22:36:32.000000 spotPython-0.2.3/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    23993 2023-05-20 22:36:32.000000 spotPython-0.2.3/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_3_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     9057 2023-05-20 22:36:32.000000 spotPython-0.2.3/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_importance.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     6972 2023-05-20 22:36:32.000000 spotPython-0.2.3/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_progress.pdf
--rw-r--r--   0 bartz      (501) staff       (20)   110037 2023-05-29 21:15:55.000000 spotPython-0.2.3/notebooks/figures14-torch_maans03_60min_20init_2023-05-27_23-10-01_contour_0_2.png
--rw-r--r--   0 bartz      (501) staff       (20)    29542 2023-05-29 21:15:55.000000 spotPython-0.2.3/notebooks/figures14-torch_maans03_60min_20init_2023-05-27_23-10-01_importance.png
--rw-r--r--   0 bartz      (501) staff       (20)    41583 2023-05-29 21:15:55.000000 spotPython-0.2.3/notebooks/figures14-torch_maans03_60min_20init_2023-05-27_23-10-01_progress.png
--rw-r--r--   0 bartz      (501) staff       (20)    38438 2023-04-14 08:14:51.000000 spotPython-0.2.3/notebooks/plot.png
--rw-r--r--   0 bartz      (501) staff       (20)     1354 2023-05-30 10:10:09.000000 spotPython-0.2.3/pyproject.toml
--rw-r--r--   0 bartz      (501) staff       (20)       38 2023-05-30 10:31:02.428961 spotPython-0.2.3/setup.cfg
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-30 10:31:02.287591 spotPython-0.2.3/src/
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-30 10:31:02.393412 spotPython-0.2.3/src/spotPython/
--rw-r--r--   0 bartz      (501) staff       (20)      214 2023-05-30 10:31:02.000000 spotPython-0.2.3/src/spotPython/_version.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-30 10:31:02.396601 spotPython-0.2.3/src/spotPython/budget/
--rw-r--r--   0 bartz      (501) staff       (20)     2772 2023-01-31 08:03:34.000000 spotPython-0.2.3/src/spotPython/budget/ocba.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-30 10:31:02.397816 spotPython-0.2.3/src/spotPython/build/
--rw-r--r--   0 bartz      (501) staff       (20)    40135 2023-04-14 08:14:51.000000 spotPython-0.2.3/src/spotPython/build/kriging.py
--rw-r--r--   0 bartz      (501) staff       (20)      342 2023-01-31 08:03:34.000000 spotPython-0.2.3/src/spotPython/build/surrogates.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-30 10:31:02.402075 spotPython-0.2.3/src/spotPython/data/
--rw-r--r--   0 bartz      (501) staff       (20)      317 2023-04-26 06:49:16.000000 spotPython-0.2.3/src/spotPython/data/__init__.py
--rw-r--r--   0 bartz      (501) staff       (20)    13563 2023-04-26 06:49:16.000000 spotPython-0.2.3/src/spotPython/data/base.py
--rw-r--r--   0 bartz      (501) staff       (20)    20975 2023-05-30 10:14:41.000000 spotPython-0.2.3/src/spotPython/data/sklearn_hyper_dict.json
--rw-r--r--   0 bartz      (501) staff       (20)      333 2023-04-26 10:58:34.000000 spotPython-0.2.3/src/spotPython/data/sklearn_hyper_dict.py
--rw-r--r--   0 bartz      (501) staff       (20)     5171 2023-05-29 21:15:55.000000 spotPython-0.2.3/src/spotPython/data/torch_hyper_dict.json
--rw-r--r--   0 bartz      (501) staff       (20)      329 2023-04-26 11:40:26.000000 spotPython-0.2.3/src/spotPython/data/torch_hyper_dict.py
--rw-r--r--   0 bartz      (501) staff       (20)      459 2023-05-29 21:15:55.000000 spotPython-0.2.3/src/spotPython/data/torchdata.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-30 10:31:02.403504 spotPython-0.2.3/src/spotPython/design/
--rw-r--r--   0 bartz      (501) staff       (20)      375 2023-01-31 08:03:34.000000 spotPython-0.2.3/src/spotPython/design/designs.py
--rw-r--r--   0 bartz      (501) staff       (20)      341 2023-01-31 08:03:34.000000 spotPython-0.2.3/src/spotPython/design/factorial.py
--rw-r--r--   0 bartz      (501) staff       (20)     2156 2023-04-26 06:49:16.000000 spotPython-0.2.3/src/spotPython/design/spacefilling.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-30 10:31:02.405350 spotPython-0.2.3/src/spotPython/fun/
--rw-r--r--   0 bartz      (501) staff       (20)     3770 2023-05-30 10:09:37.000000 spotPython-0.2.3/src/spotPython/fun/hypersklearn.py
--rw-r--r--   0 bartz      (501) staff       (20)     4911 2023-05-29 21:15:55.000000 spotPython-0.2.3/src/spotPython/fun/hypertorch.py
--rw-r--r--   0 bartz      (501) staff       (20)    18970 2023-05-09 07:21:36.000000 spotPython-0.2.3/src/spotPython/fun/objectivefunctions.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-30 10:31:02.407427 spotPython-0.2.3/src/spotPython/hyperparameters/
--rw-r--r--   0 bartz      (501) staff       (20)     4851 2023-03-26 17:32:36.000000 spotPython-0.2.3/src/spotPython/hyperparameters/categorical.py
--rw-r--r--   0 bartz      (501) staff       (20)     4137 2023-05-29 21:15:55.000000 spotPython-0.2.3/src/spotPython/hyperparameters/optimizer.py
--rw-r--r--   0 bartz      (501) staff       (20)    26033 2023-05-29 21:15:55.000000 spotPython-0.2.3/src/spotPython/hyperparameters/values.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-30 10:31:02.408377 spotPython-0.2.3/src/spotPython/plot/
--rw-r--r--   0 bartz      (501) staff       (20)     1707 2023-01-31 08:03:34.000000 spotPython-0.2.3/src/spotPython/plot/contour.py
--rw-r--r--   0 bartz      (501) staff       (20)     4614 2023-05-20 22:36:32.000000 spotPython-0.2.3/src/spotPython/plot/validation.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-30 10:31:02.408831 spotPython-0.2.3/src/spotPython/sklearn/
--rw-r--r--   0 bartz      (501) staff       (20)     3711 2023-05-29 21:15:55.000000 spotPython-0.2.3/src/spotPython/sklearn/traintest.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-30 10:31:02.409501 spotPython-0.2.3/src/spotPython/spot/
--rw-r--r--   0 bartz      (501) staff       (20)    33049 2023-05-29 21:15:55.000000 spotPython-0.2.3/src/spotPython/spot/spot.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-30 10:31:02.412232 spotPython-0.2.3/src/spotPython/torch/
--rw-r--r--   0 bartz      (501) staff       (20)     1012 2023-05-29 21:15:55.000000 spotPython-0.2.3/src/spotPython/torch/netcifar10.py
--rw-r--r--   0 bartz      (501) staff       (20)      425 2023-05-29 21:15:55.000000 spotPython-0.2.3/src/spotPython/torch/netcore.py
--rw-r--r--   0 bartz      (501) staff       (20)      803 2023-05-29 21:15:55.000000 spotPython-0.2.3/src/spotPython/torch/netfashionMNIST.py
--rw-r--r--   0 bartz      (501) staff       (20)    13380 2023-05-29 21:15:55.000000 spotPython-0.2.3/src/spotPython/torch/traintest.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-30 10:31:02.418934 spotPython-0.2.3/src/spotPython/utils/
--rw-r--r--   0 bartz      (501) staff       (20)     2003 2023-04-12 06:53:11.000000 spotPython-0.2.3/src/spotPython/utils/aggregate.py
--rw-r--r--   0 bartz      (501) staff       (20)      498 2023-05-12 21:21:20.000000 spotPython-0.2.3/src/spotPython/utils/classes.py
--rw-r--r--   0 bartz      (501) staff       (20)     1162 2023-04-14 08:14:51.000000 spotPython-0.2.3/src/spotPython/utils/compare.py
--rw-r--r--   0 bartz      (501) staff       (20)     1954 2023-05-20 22:36:32.000000 spotPython-0.2.3/src/spotPython/utils/convert.py
--rw-r--r--   0 bartz      (501) staff       (20)      598 2023-05-09 07:21:36.000000 spotPython-0.2.3/src/spotPython/utils/device.py
--rw-r--r--   0 bartz      (501) staff       (20)     3600 2023-05-10 10:26:34.000000 spotPython-0.2.3/src/spotPython/utils/eda.py
--rw-r--r--   0 bartz      (501) staff       (20)      461 2023-04-26 10:52:22.000000 spotPython-0.2.3/src/spotPython/utils/file.py
--rw-r--r--   0 bartz      (501) staff       (20)     1445 2023-05-29 21:15:55.000000 spotPython-0.2.3/src/spotPython/utils/init.py
--rw-r--r--   0 bartz      (501) staff       (20)     5028 2023-05-20 22:36:38.000000 spotPython-0.2.3/src/spotPython/utils/metrics.py
--rw-r--r--   0 bartz      (501) staff       (20)      845 2023-04-14 08:14:51.000000 spotPython-0.2.3/src/spotPython/utils/progress.py
--rw-r--r--   0 bartz      (501) staff       (20)     1379 2023-04-14 08:14:51.000000 spotPython-0.2.3/src/spotPython/utils/repair.py
--rw-r--r--   0 bartz      (501) staff       (20)     4964 2023-05-10 10:26:34.000000 spotPython-0.2.3/src/spotPython/utils/transform.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-30 10:31:02.396114 spotPython-0.2.3/src/spotPython.egg-info/
--rw-r--r--   0 bartz      (501) staff       (20)     7347 2023-05-30 10:31:02.000000 spotPython-0.2.3/src/spotPython.egg-info/PKG-INFO
--rw-r--r--   0 bartz      (501) staff       (20)    10399 2023-05-30 10:31:02.000000 spotPython-0.2.3/src/spotPython.egg-info/SOURCES.txt
--rw-r--r--   0 bartz      (501) staff       (20)        1 2023-05-30 10:31:02.000000 spotPython-0.2.3/src/spotPython.egg-info/dependency_links.txt
--rw-r--r--   0 bartz      (501) staff       (20)       59 2023-05-30 10:31:02.000000 spotPython-0.2.3/src/spotPython.egg-info/requires.txt
--rw-r--r--   0 bartz      (501) staff       (20)       11 2023-05-30 10:31:02.000000 spotPython-0.2.3/src/spotPython.egg-info/top_level.txt
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-30 10:31:02.427802 spotPython-0.2.3/test/
--rw-r--r--   0 bartz      (501) staff       (20)      873 2023-01-31 08:03:34.000000 spotPython-0.2.3/test/test_aggregate_mean_var.py
--rw-r--r--   0 bartz      (501) staff       (20)     4546 2023-04-09 20:02:14.000000 spotPython-0.2.3/test/test_build_Psi.py
--rw-r--r--   0 bartz      (501) staff       (20)     4511 2023-04-09 20:02:14.000000 spotPython-0.2.3/test/test_build_U.py
--rw-r--r--   0 bartz      (501) staff       (20)      797 2023-01-31 08:03:34.000000 spotPython-0.2.3/test/test_build_psi_vec.py
--rw-r--r--   0 bartz      (501) staff       (20)      917 2023-01-31 08:03:34.000000 spotPython-0.2.3/test/test_evaluate_new_X.py
--rw-r--r--   0 bartz      (501) staff       (20)     1319 2023-01-31 08:03:34.000000 spotPython-0.2.3/test/test_evaluate_new_solutions.py
--rw-r--r--   0 bartz      (501) staff       (20)    10337 2023-04-09 20:02:14.000000 spotPython-0.2.3/test/test_extract_from_bounds.py
--rw-r--r--   0 bartz      (501) staff       (20)     2263 2023-01-31 08:03:34.000000 spotPython-0.2.3/test/test_generate_design.py
--rw-r--r--   0 bartz      (501) staff       (20)     2223 2023-01-31 08:03:34.000000 spotPython-0.2.3/test/test_infill.py
--rw-r--r--   0 bartz      (501) staff       (20)      643 2023-01-31 08:03:34.000000 spotPython-0.2.3/test/test_nat_to_cod.py
--rw-r--r--   0 bartz      (501) staff       (20)     1330 2023-01-31 08:03:34.000000 spotPython-0.2.3/test/test_nat_to_cod_init.py
--rw-r--r--   0 bartz      (501) staff       (20)     1603 2023-01-31 08:03:34.000000 spotPython-0.2.3/test/test_ocba.py
--rw-r--r--   0 bartz      (501) staff       (20)     1208 2023-01-31 08:03:34.000000 spotPython-0.2.3/test/test_repair_non_numeric.py
--rw-r--r--   0 bartz      (501) staff       (20)     4887 2023-01-31 08:03:34.000000 spotPython-0.2.3/test/test_set_de_bounds.py
--rw-r--r--   0 bartz      (501) staff       (20)     2223 2023-01-31 08:03:34.000000 spotPython-0.2.3/test/test_show_progress.py
--rw-r--r--   0 bartz      (501) staff       (20)     1131 2023-01-31 08:03:34.000000 spotPython-0.2.3/test/test_suggest_new_X.py
--rw-r--r--   0 bartz      (501) staff       (20)     1765 2023-01-31 08:03:34.000000 spotPython-0.2.3/test/test_update_surrogate.py
--rw-r--r--   0 bartz      (501) staff       (20)      130 2023-05-19 14:54:05.000000 spotPython-0.2.3/tox.ini
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-31 08:16:52.967701 spotPython-0.2.4/
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-31 08:16:52.903654 spotPython-0.2.4/.github/
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-31 08:16:52.908273 spotPython-0.2.4/.github/workflows/
+-rw-r--r--   0 bartz      (501) staff       (20)      557 2023-02-02 20:30:23.000000 spotPython-0.2.4/.github/workflows/test.yml
+-rw-r--r--   0 bartz      (501) staff       (20)    13211 2023-05-31 08:10:07.000000 spotPython-0.2.4/.gitignore
+-rw-r--r--   0 bartz      (501) staff       (20)        0 2023-05-18 22:04:43.000000 spotPython-0.2.4/.nojekyll
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-31 08:16:52.919844 spotPython-0.2.4/Figures.d/
+-rw-r--r--   0 bartz      (501) staff       (20)    21113 2023-04-26 21:03:04.000000 spotPython-0.2.4/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_contour_1_2.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     5878 2023-04-26 21:03:04.000000 spotPython-0.2.4/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_importance.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     6563 2023-04-26 21:03:04.000000 spotPython-0.2.4/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_progress.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    26562 2023-04-26 22:09:11.000000 spotPython-0.2.4/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_contour_2_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     8850 2023-04-26 22:09:11.000000 spotPython-0.2.4/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_importance.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     6569 2023-04-26 22:09:11.000000 spotPython-0.2.4/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_progress.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    20478 2023-04-28 06:03:36.000000 spotPython-0.2.4/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_1.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    20590 2023-04-28 06:03:36.000000 spotPython-0.2.4/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_2.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    23054 2023-04-28 06:03:36.000000 spotPython-0.2.4/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22138 2023-04-28 06:03:36.000000 spotPython-0.2.4/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    21534 2023-04-28 06:03:36.000000 spotPython-0.2.4/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_2.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22805 2023-04-28 06:03:36.000000 spotPython-0.2.4/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22098 2023-04-28 06:03:36.000000 spotPython-0.2.4/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    23275 2023-04-28 06:03:36.000000 spotPython-0.2.4/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_2_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    21965 2023-04-28 06:03:36.000000 spotPython-0.2.4/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_2_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22913 2023-04-28 06:03:36.000000 spotPython-0.2.4/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_3_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     9680 2023-04-28 06:03:36.000000 spotPython-0.2.4/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_importance.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     6536 2023-04-28 06:03:36.000000 spotPython-0.2.4/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_progress.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    21132 2023-05-08 04:46:15.000000 spotPython-0.2.4/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_1.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    21651 2023-05-08 04:46:16.000000 spotPython-0.2.4/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_2.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22154 2023-05-08 04:46:18.000000 spotPython-0.2.4/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    21347 2023-05-08 04:46:19.000000 spotPython-0.2.4/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22265 2023-05-08 04:46:20.000000 spotPython-0.2.4/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_2.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22056 2023-05-08 04:46:21.000000 spotPython-0.2.4/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22224 2023-05-08 04:46:22.000000 spotPython-0.2.4/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    23950 2023-05-08 04:46:23.000000 spotPython-0.2.4/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_2_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    23161 2023-05-08 04:46:24.000000 spotPython-0.2.4/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_2_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22297 2023-05-08 04:46:25.000000 spotPython-0.2.4/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_3_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     9681 2023-05-08 04:37:14.000000 spotPython-0.2.4/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_importance.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     8189 2023-05-08 04:37:14.000000 spotPython-0.2.4/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_progress.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22759 2023-05-07 21:33:09.000000 spotPython-0.2.4/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_1_2.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    24775 2023-05-07 21:33:09.000000 spotPython-0.2.4/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_1_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    23126 2023-05-07 21:33:10.000000 spotPython-0.2.4/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_2_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     8905 2023-05-07 21:23:58.000000 spotPython-0.2.4/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_importance.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     7635 2023-05-07 21:23:58.000000 spotPython-0.2.4/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_progress.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    24695 2023-05-06 06:36:55.000000 spotPython-0.2.4/Figures.d/13-torch_s7cfd16_600min_20init_2023-05-05_18-52-19_contour_2_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    34523 2023-02-01 14:33:52.000000 spotPython-0.2.4/LICENSE.txt
+-rw-r--r--   0 bartz      (501) staff       (20)       71 2023-04-20 20:35:14.000000 spotPython-0.2.4/MANIFEST.in
+-rw-r--r--   0 bartz      (501) staff       (20)     7347 2023-05-31 08:16:52.967539 spotPython-0.2.4/PKG-INFO
+-rw-r--r--   0 bartz      (501) staff       (20)     6577 2023-05-23 19:35:10.000000 spotPython-0.2.4/README.md
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-31 08:16:52.922275 spotPython-0.2.4/docs/
+-rw-r--r--   0 bartz      (501) staff       (20)   208086 2023-05-29 18:21:43.000000 spotPython-0.2.4/docs/bart23e.html
+-rw-r--r--   0 bartz      (501) staff       (20)   713146 2023-05-29 18:21:50.000000 spotPython-0.2.4/docs/bart23e.pdf
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-31 08:16:52.925493 spotPython-0.2.4/docs/figures/
+-rw-r--r--   0 bartz      (501) staff       (20)    88272 2023-05-26 10:05:04.000000 spotPython-0.2.4/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_1.png
+-rw-r--r--   0 bartz      (501) staff       (20)    84164 2023-05-26 10:04:55.000000 spotPython-0.2.4/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_3.png
+-rw-r--r--   0 bartz      (501) staff       (20)    93300 2023-05-26 10:04:39.000000 spotPython-0.2.4/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_4.png
+-rw-r--r--   0 bartz      (501) staff       (20)    84900 2023-05-26 10:04:25.000000 spotPython-0.2.4/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_3.png
+-rw-r--r--   0 bartz      (501) staff       (20)    94821 2023-05-26 10:04:11.000000 spotPython-0.2.4/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_4.png
+-rw-r--r--   0 bartz      (501) staff       (20)    92856 2023-05-26 10:03:52.000000 spotPython-0.2.4/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_3_4.png
+-rw-r--r--   0 bartz      (501) staff       (20)    21443 2023-05-26 10:02:53.000000 spotPython-0.2.4/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_importance.png
+-rw-r--r--   0 bartz      (501) staff       (20)    26414 2023-05-26 10:02:27.000000 spotPython-0.2.4/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_progress.png
+-rw-r--r--   0 bartz      (501) staff       (20)    94077 2023-05-19 17:04:41.000000 spotPython-0.2.4/docs/figures/parallel.png
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-31 08:16:52.925756 spotPython-0.2.4/docs/img/
+-rw-r--r--   0 bartz      (501) staff       (20)    67674 2023-05-27 21:03:27.000000 spotPython-0.2.4/docs/img/spotLogo.png
+-rw-r--r--   0 bartz      (501) staff       (20)      231 2023-05-29 18:21:50.000000 spotPython-0.2.4/docs/index.html
+-rw-r--r--   0 bartz      (501) staff       (20)    64921 2023-05-29 18:21:50.000000 spotPython-0.2.4/docs/search.json
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-31 08:16:52.904350 spotPython-0.2.4/docs/site_libs/
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-31 08:16:52.927738 spotPython-0.2.4/docs/site_libs/bootstrap/
+-rw-r--r--   0 bartz      (501) staff       (20)    95517 2023-05-12 19:57:05.000000 spotPython-0.2.4/docs/site_libs/bootstrap/bootstrap-icons.css
+-rw-r--r--   0 bartz      (501) staff       (20)   164168 2023-05-12 19:56:28.000000 spotPython-0.2.4/docs/site_libs/bootstrap/bootstrap-icons.woff
+-rw-r--r--   0 bartz      (501) staff       (20)   308771 2023-05-29 18:21:41.000000 spotPython-0.2.4/docs/site_libs/bootstrap/bootstrap.min.css
+-rw-r--r--   0 bartz      (501) staff       (20)    78129 2023-05-12 19:57:05.000000 spotPython-0.2.4/docs/site_libs/bootstrap/bootstrap.min.js
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-31 08:16:52.928016 spotPython-0.2.4/docs/site_libs/clipboard/
+-rw-r--r--   0 bartz      (501) staff       (20)     9160 2023-05-12 19:57:05.000000 spotPython-0.2.4/docs/site_libs/clipboard/clipboard.min.js
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-31 08:16:52.929361 spotPython-0.2.4/docs/site_libs/quarto-html/
+-rw-r--r--   0 bartz      (501) staff       (20)     6008 2023-05-12 19:57:05.000000 spotPython-0.2.4/docs/site_libs/quarto-html/anchor.min.js
+-rw-r--r--   0 bartz      (501) staff       (20)    19728 2023-05-12 19:57:05.000000 spotPython-0.2.4/docs/site_libs/quarto-html/popper.min.js
+-rw-r--r--   0 bartz      (501) staff       (20)     3135 2023-05-23 19:54:10.000000 spotPython-0.2.4/docs/site_libs/quarto-html/quarto-syntax-highlighting.css
+-rw-r--r--   0 bartz      (501) staff       (20)    28407 2023-05-12 19:57:05.000000 spotPython-0.2.4/docs/site_libs/quarto-html/quarto.js
+-rw-r--r--   0 bartz      (501) staff       (20)     1409 2023-05-12 19:57:05.000000 spotPython-0.2.4/docs/site_libs/quarto-html/tippy.css
+-rw-r--r--   0 bartz      (501) staff       (20)    24033 2023-05-12 19:57:05.000000 spotPython-0.2.4/docs/site_libs/quarto-html/tippy.umd.min.js
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-31 08:16:52.929549 spotPython-0.2.4/docs/site_libs/quarto-nav/
+-rw-r--r--   0 bartz      (501) staff       (20)     8250 2023-05-12 19:57:05.000000 spotPython-0.2.4/docs/site_libs/quarto-nav/quarto-nav.js
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-31 08:16:52.930260 spotPython-0.2.4/docs/site_libs/quarto-search/
+-rw-r--r--   0 bartz      (501) staff       (20)    70711 2023-05-12 19:57:05.000000 spotPython-0.2.4/docs/site_libs/quarto-search/autocomplete.umd.js
+-rw-r--r--   0 bartz      (501) staff       (20)    23539 2023-05-12 19:57:05.000000 spotPython-0.2.4/docs/site_libs/quarto-search/fuse.min.js
+-rw-r--r--   0 bartz      (501) staff       (20)    32789 2023-05-12 19:57:05.000000 spotPython-0.2.4/docs/site_libs/quarto-search/quarto-search.js
+-rwxr-xr-x   0 bartz      (501) staff       (20)      123 2023-04-26 22:09:11.000000 spotPython-0.2.4/makeSpot.sh
+-rw-r--r--   0 bartz      (501) staff       (20)      437 2023-02-02 22:52:12.000000 spotPython-0.2.4/mkdocs.yml
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-31 08:16:52.951194 spotPython-0.2.4/notebooks/
+-rw-r--r--   0 bartz      (501) staff       (20)    34275 2023-05-20 05:31:37.000000 spotPython-0.2.4/notebooks/00_spot_doc.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)     6585 2023-05-08 22:27:42.000000 spotPython-0.2.4/notebooks/01_spot_intro.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)     8780 2023-05-20 08:33:47.000000 spotPython-0.2.4/notebooks/02_spot_multidim.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)     9719 2023-05-08 22:28:54.000000 spotPython-0.2.4/notebooks/03_spot_anisotropic.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)    15781 2023-05-08 22:29:50.000000 spotPython-0.2.4/notebooks/04_spot_sklearn_surrogate.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)     8787 2023-05-08 22:30:17.000000 spotPython-0.2.4/notebooks/05_spot_sklearn_optimizers.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)    14206 2023-05-08 22:30:52.000000 spotPython-0.2.4/notebooks/06_spot_gaussian.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)    36749 2023-05-08 22:31:54.000000 spotPython-0.2.4/notebooks/07_spot_ei.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)    11665 2023-05-08 22:32:20.000000 spotPython-0.2.4/notebooks/08_spot_noisy.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)    12100 2023-05-08 22:32:53.000000 spotPython-0.2.4/notebooks/09_spot_ocba.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)   125645 2023-05-20 08:34:43.000000 spotPython-0.2.4/notebooks/10_spot_hpt_sklearn_classification.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)    23403 2023-05-27 07:00:04.000000 spotPython-0.2.4/notebooks/11_spot_hpt_torch_fashion_mnist.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)    28481 2023-05-27 07:00:42.000000 spotPython-0.2.4/notebooks/12_spot_hpt_torch_cifar10.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)    22216 2023-05-20 08:37:13.000000 spotPython-0.2.4/notebooks/13_spot_hpt_torch_cv_fashion_mnist.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)   110777 2023-05-31 08:15:41.000000 spotPython-0.2.4/notebooks/14_spot_ray_hpt_torch_cifar10.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)    26705 2023-05-20 08:39:17.000000 spotPython-0.2.4/notebooks/15_spot_hpt_sklearn_regression.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)  1475255 2023-05-31 08:15:56.000000 spotPython-0.2.4/notebooks/16_spot_hpt_sklearn_multiclass_classification_randomforest.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)  1048139 2023-05-31 08:16:02.000000 spotPython-0.2.4/notebooks/17_spot_hpt_sklearn_multiclass_classification_xgb.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)   354130 2023-05-30 15:26:52.000000 spotPython-0.2.4/notebooks/18_spot_hpt_sklearn_multiclass_classification_svc.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)   674714 2023-05-30 15:26:52.000000 spotPython-0.2.4/notebooks/19_spot_hpt_sklearn_multiclass_classification_knn.ipynb
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-31 08:16:52.904582 spotPython-0.2.4/notebooks/data/
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-31 08:16:52.951727 spotPython-0.2.4/notebooks/data/torch/
+-rw-r--r--   0 bartz      (501) staff       (20)    77195 2023-05-14 08:03:00.000000 spotPython-0.2.4/notebooks/data/torch/model_spot_trained.pt
+-rw-r--r--   0 bartz      (501) staff       (20)      359 2023-03-21 18:40:04.000000 spotPython-0.2.4/notebooks/data.json
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-31 08:16:52.957683 spotPython-0.2.4/notebooks/figures/
+-rw-r--r--   0 bartz      (501) staff       (20)    88272 2023-05-26 10:05:04.000000 spotPython-0.2.4/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_1.png
+-rw-r--r--   0 bartz      (501) staff       (20)    84164 2023-05-26 10:04:55.000000 spotPython-0.2.4/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_3.png
+-rw-r--r--   0 bartz      (501) staff       (20)    93300 2023-05-26 10:04:39.000000 spotPython-0.2.4/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_4.png
+-rw-r--r--   0 bartz      (501) staff       (20)    84900 2023-05-26 10:04:25.000000 spotPython-0.2.4/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_3.png
+-rw-r--r--   0 bartz      (501) staff       (20)    94821 2023-05-26 10:04:11.000000 spotPython-0.2.4/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_4.png
+-rw-r--r--   0 bartz      (501) staff       (20)    92856 2023-05-26 10:03:52.000000 spotPython-0.2.4/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_3_4.png
+-rw-r--r--   0 bartz      (501) staff       (20)    21443 2023-05-26 10:02:53.000000 spotPython-0.2.4/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_importance.png
+-rw-r--r--   0 bartz      (501) staff       (20)    26414 2023-05-26 10:02:27.000000 spotPython-0.2.4/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_progress.png
+-rw-r--r--   0 bartz      (501) staff       (20)   121376 2023-05-28 06:32:18.000000 spotPython-0.2.4/notebooks/figures/figures14-torch_maans03_60min_20init_2023-05-27_23-10-01_parallel.png
+-rw-r--r--   0 bartz      (501) staff       (20)   115822 2023-02-01 14:33:52.000000 spotPython-0.2.4/notebooks/figures/spotModel.graffle
+-rw-r--r--   0 bartz      (501) staff       (20)    26289 2023-02-01 14:33:52.000000 spotPython-0.2.4/notebooks/figures/spotModel.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    64603 2023-02-01 14:33:52.000000 spotPython-0.2.4/notebooks/figures/spotModel.png
+-rw-r--r--   0 bartz      (501) staff       (20)    21112 2023-05-22 18:09:24.000000 spotPython-0.2.4/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_0_1.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    21979 2023-05-22 18:09:24.000000 spotPython-0.2.4/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_0_2.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    23390 2023-05-22 18:09:24.000000 spotPython-0.2.4/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_0_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22172 2023-05-22 18:09:24.000000 spotPython-0.2.4/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_1_2.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    23463 2023-05-22 18:09:24.000000 spotPython-0.2.4/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_1_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    24987 2023-05-22 18:09:24.000000 spotPython-0.2.4/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_2_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    10009 2023-05-22 18:09:24.000000 spotPython-0.2.4/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_importance.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     7783 2023-05-22 18:09:24.000000 spotPython-0.2.4/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_progress.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    21663 2023-05-23 19:31:10.000000 spotPython-0.2.4/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_0_1.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22544 2023-05-23 19:31:10.000000 spotPython-0.2.4/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_0_2.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22042 2023-05-23 19:31:10.000000 spotPython-0.2.4/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_0_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    21676 2023-05-23 19:31:10.000000 spotPython-0.2.4/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_1_2.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    21232 2023-05-23 19:31:10.000000 spotPython-0.2.4/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_1_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22317 2023-05-23 19:31:10.000000 spotPython-0.2.4/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_2_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     9376 2023-05-23 19:31:10.000000 spotPython-0.2.4/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_importance.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     6836 2023-05-23 19:31:10.000000 spotPython-0.2.4/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_progress.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22179 2023-05-19 16:57:48.000000 spotPython-0.2.4/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_1.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    21553 2023-05-19 16:57:48.000000 spotPython-0.2.4/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    23439 2023-05-19 16:57:48.000000 spotPython-0.2.4/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22108 2023-05-19 16:57:48.000000 spotPython-0.2.4/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    23180 2023-05-19 16:57:48.000000 spotPython-0.2.4/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    23993 2023-05-19 16:57:48.000000 spotPython-0.2.4/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_3_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     9057 2023-05-19 16:57:48.000000 spotPython-0.2.4/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_importance.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     6972 2023-05-19 16:57:48.000000 spotPython-0.2.4/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_progress.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)   110037 2023-05-28 06:32:18.000000 spotPython-0.2.4/notebooks/figures14-torch_maans03_60min_20init_2023-05-27_23-10-01_contour_0_2.png
+-rw-r--r--   0 bartz      (501) staff       (20)    29542 2023-05-28 06:32:18.000000 spotPython-0.2.4/notebooks/figures14-torch_maans03_60min_20init_2023-05-27_23-10-01_importance.png
+-rw-r--r--   0 bartz      (501) staff       (20)    41583 2023-05-28 06:32:18.000000 spotPython-0.2.4/notebooks/figures14-torch_maans03_60min_20init_2023-05-27_23-10-01_progress.png
+-rw-r--r--   0 bartz      (501) staff       (20)    38438 2023-05-09 06:26:54.000000 spotPython-0.2.4/notebooks/plot.png
+-rw-r--r--   0 bartz      (501) staff       (20)     1354 2023-05-30 21:15:00.000000 spotPython-0.2.4/pyproject.toml
+-rw-r--r--   0 bartz      (501) staff       (20)       38 2023-05-31 08:16:52.967741 spotPython-0.2.4/setup.cfg
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-31 08:16:52.904836 spotPython-0.2.4/src/
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-31 08:16:52.957935 spotPython-0.2.4/src/spotPython/
+-rw-r--r--   0 bartz      (501) staff       (20)      194 2023-05-31 08:16:52.000000 spotPython-0.2.4/src/spotPython/_version.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-31 08:16:52.958671 spotPython-0.2.4/src/spotPython/budget/
+-rw-r--r--   0 bartz      (501) staff       (20)     2772 2023-04-13 18:20:56.000000 spotPython-0.2.4/src/spotPython/budget/ocba.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-31 08:16:52.958928 spotPython-0.2.4/src/spotPython/build/
+-rw-r--r--   0 bartz      (501) staff       (20)    40135 2023-04-13 19:26:45.000000 spotPython-0.2.4/src/spotPython/build/kriging.py
+-rw-r--r--   0 bartz      (501) staff       (20)      342 2023-02-02 22:52:12.000000 spotPython-0.2.4/src/spotPython/build/surrogates.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-31 08:16:52.960041 spotPython-0.2.4/src/spotPython/data/
+-rw-r--r--   0 bartz      (501) staff       (20)      317 2023-04-20 20:18:46.000000 spotPython-0.2.4/src/spotPython/data/__init__.py
+-rw-r--r--   0 bartz      (501) staff       (20)    13563 2023-04-20 20:17:18.000000 spotPython-0.2.4/src/spotPython/data/base.py
+-rw-r--r--   0 bartz      (501) staff       (20)    20975 2023-05-30 15:26:52.000000 spotPython-0.2.4/src/spotPython/data/sklearn_hyper_dict.json
+-rw-r--r--   0 bartz      (501) staff       (20)      333 2023-04-20 20:14:06.000000 spotPython-0.2.4/src/spotPython/data/sklearn_hyper_dict.py
+-rw-r--r--   0 bartz      (501) staff       (20)     6956 2023-05-30 22:12:52.000000 spotPython-0.2.4/src/spotPython/data/torch_hyper_dict.json
+-rw-r--r--   0 bartz      (501) staff       (20)      329 2023-04-26 18:22:38.000000 spotPython-0.2.4/src/spotPython/data/torch_hyper_dict.py
+-rw-r--r--   0 bartz      (501) staff       (20)      459 2023-05-28 07:19:43.000000 spotPython-0.2.4/src/spotPython/data/torchdata.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-31 08:16:52.960409 spotPython-0.2.4/src/spotPython/design/
+-rw-r--r--   0 bartz      (501) staff       (20)      375 2023-02-02 22:52:12.000000 spotPython-0.2.4/src/spotPython/design/designs.py
+-rw-r--r--   0 bartz      (501) staff       (20)      341 2023-02-02 22:52:12.000000 spotPython-0.2.4/src/spotPython/design/factorial.py
+-rw-r--r--   0 bartz      (501) staff       (20)     2156 2023-04-23 08:24:45.000000 spotPython-0.2.4/src/spotPython/design/spacefilling.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-31 08:16:52.960929 spotPython-0.2.4/src/spotPython/fun/
+-rw-r--r--   0 bartz      (501) staff       (20)     3770 2023-05-30 15:26:52.000000 spotPython-0.2.4/src/spotPython/fun/hypersklearn.py
+-rw-r--r--   0 bartz      (501) staff       (20)     4911 2023-05-27 18:18:59.000000 spotPython-0.2.4/src/spotPython/fun/hypertorch.py
+-rw-r--r--   0 bartz      (501) staff       (20)    18970 2023-05-06 16:12:25.000000 spotPython-0.2.4/src/spotPython/fun/objectivefunctions.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-31 08:16:52.961351 spotPython-0.2.4/src/spotPython/hyperparameters/
+-rw-r--r--   0 bartz      (501) staff       (20)     4851 2023-03-25 16:36:59.000000 spotPython-0.2.4/src/spotPython/hyperparameters/categorical.py
+-rw-r--r--   0 bartz      (501) staff       (20)     4137 2023-05-27 19:48:36.000000 spotPython-0.2.4/src/spotPython/hyperparameters/optimizer.py
+-rw-r--r--   0 bartz      (501) staff       (20)    26033 2023-05-28 07:22:58.000000 spotPython-0.2.4/src/spotPython/hyperparameters/values.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-31 08:16:52.961618 spotPython-0.2.4/src/spotPython/plot/
+-rw-r--r--   0 bartz      (501) staff       (20)     1707 2023-05-29 06:13:03.000000 spotPython-0.2.4/src/spotPython/plot/contour.py
+-rw-r--r--   0 bartz      (501) staff       (20)     4614 2023-05-20 08:41:56.000000 spotPython-0.2.4/src/spotPython/plot/validation.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-31 08:16:52.961746 spotPython-0.2.4/src/spotPython/sklearn/
+-rw-r--r--   0 bartz      (501) staff       (20)     3711 2023-05-29 20:57:16.000000 spotPython-0.2.4/src/spotPython/sklearn/traintest.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-31 08:16:52.961941 spotPython-0.2.4/src/spotPython/spot/
+-rw-r--r--   0 bartz      (501) staff       (20)    33049 2023-05-29 06:29:51.000000 spotPython-0.2.4/src/spotPython/spot/spot.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-31 08:16:52.962917 spotPython-0.2.4/src/spotPython/torch/
+-rw-r--r--   0 bartz      (501) staff       (20)     2411 2023-05-30 22:07:35.000000 spotPython-0.2.4/src/spotPython/torch/mapk.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1012 2023-05-27 19:17:19.000000 spotPython-0.2.4/src/spotPython/torch/netcifar10.py
+-rw-r--r--   0 bartz      (501) staff       (20)      425 2023-05-27 19:21:33.000000 spotPython-0.2.4/src/spotPython/torch/netcore.py
+-rw-r--r--   0 bartz      (501) staff       (20)      803 2023-05-27 19:17:19.000000 spotPython-0.2.4/src/spotPython/torch/netfashionMNIST.py
+-rw-r--r--   0 bartz      (501) staff       (20)      782 2023-05-30 21:15:13.000000 spotPython-0.2.4/src/spotPython/torch/netvbdp.py
+-rw-r--r--   0 bartz      (501) staff       (20)    13380 2023-05-31 08:16:25.000000 spotPython-0.2.4/src/spotPython/torch/traintest.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-31 08:16:52.964710 spotPython-0.2.4/src/spotPython/utils/
+-rw-r--r--   0 bartz      (501) staff       (20)     2003 2023-04-09 20:33:54.000000 spotPython-0.2.4/src/spotPython/utils/aggregate.py
+-rw-r--r--   0 bartz      (501) staff       (20)      498 2023-05-12 15:45:09.000000 spotPython-0.2.4/src/spotPython/utils/classes.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1162 2023-04-13 18:33:36.000000 spotPython-0.2.4/src/spotPython/utils/compare.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1954 2023-05-20 08:44:33.000000 spotPython-0.2.4/src/spotPython/utils/convert.py
+-rw-r--r--   0 bartz      (501) staff       (20)      598 2023-05-07 19:27:47.000000 spotPython-0.2.4/src/spotPython/utils/device.py
+-rw-r--r--   0 bartz      (501) staff       (20)     3600 2023-05-09 21:08:48.000000 spotPython-0.2.4/src/spotPython/utils/eda.py
+-rw-r--r--   0 bartz      (501) staff       (20)      461 2023-04-26 18:22:38.000000 spotPython-0.2.4/src/spotPython/utils/file.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1445 2023-05-28 07:30:22.000000 spotPython-0.2.4/src/spotPython/utils/init.py
+-rw-r--r--   0 bartz      (501) staff       (20)     5028 2023-05-30 21:09:07.000000 spotPython-0.2.4/src/spotPython/utils/metrics.py
+-rw-r--r--   0 bartz      (501) staff       (20)      845 2023-04-13 18:37:01.000000 spotPython-0.2.4/src/spotPython/utils/progress.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1379 2023-04-13 18:43:38.000000 spotPython-0.2.4/src/spotPython/utils/repair.py
+-rw-r--r--   0 bartz      (501) staff       (20)     4964 2023-05-09 23:09:07.000000 spotPython-0.2.4/src/spotPython/utils/transform.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-31 08:16:52.958553 spotPython-0.2.4/src/spotPython.egg-info/
+-rw-r--r--   0 bartz      (501) staff       (20)     7347 2023-05-31 08:16:52.000000 spotPython-0.2.4/src/spotPython.egg-info/PKG-INFO
+-rw-r--r--   0 bartz      (501) staff       (20)    10539 2023-05-31 08:16:52.000000 spotPython-0.2.4/src/spotPython.egg-info/SOURCES.txt
+-rw-r--r--   0 bartz      (501) staff       (20)        1 2023-05-31 08:16:52.000000 spotPython-0.2.4/src/spotPython.egg-info/dependency_links.txt
+-rw-r--r--   0 bartz      (501) staff       (20)       59 2023-05-31 08:16:52.000000 spotPython-0.2.4/src/spotPython.egg-info/requires.txt
+-rw-r--r--   0 bartz      (501) staff       (20)       11 2023-05-31 08:16:52.000000 spotPython-0.2.4/src/spotPython.egg-info/top_level.txt
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-31 08:16:52.967287 spotPython-0.2.4/test/
+-rw-r--r--   0 bartz      (501) staff       (20)      873 2023-02-01 14:33:52.000000 spotPython-0.2.4/test/test_aggregate_mean_var.py
+-rw-r--r--   0 bartz      (501) staff       (20)     4546 2023-04-09 19:57:56.000000 spotPython-0.2.4/test/test_build_Psi.py
+-rw-r--r--   0 bartz      (501) staff       (20)     4511 2023-04-09 19:58:12.000000 spotPython-0.2.4/test/test_build_U.py
+-rw-r--r--   0 bartz      (501) staff       (20)      797 2023-02-01 14:33:52.000000 spotPython-0.2.4/test/test_build_psi_vec.py
+-rw-r--r--   0 bartz      (501) staff       (20)      917 2023-02-01 14:33:52.000000 spotPython-0.2.4/test/test_evaluate_new_X.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1319 2023-02-01 14:33:52.000000 spotPython-0.2.4/test/test_evaluate_new_solutions.py
+-rw-r--r--   0 bartz      (501) staff       (20)    10337 2023-04-09 19:58:51.000000 spotPython-0.2.4/test/test_extract_from_bounds.py
+-rw-r--r--   0 bartz      (501) staff       (20)     2263 2023-02-01 14:33:52.000000 spotPython-0.2.4/test/test_generate_design.py
+-rw-r--r--   0 bartz      (501) staff       (20)     2223 2023-02-01 14:33:52.000000 spotPython-0.2.4/test/test_infill.py
+-rw-r--r--   0 bartz      (501) staff       (20)      643 2023-02-01 14:33:52.000000 spotPython-0.2.4/test/test_nat_to_cod.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1330 2023-02-01 14:33:52.000000 spotPython-0.2.4/test/test_nat_to_cod_init.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1603 2023-02-01 14:33:52.000000 spotPython-0.2.4/test/test_ocba.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1208 2023-02-01 14:33:52.000000 spotPython-0.2.4/test/test_repair_non_numeric.py
+-rw-r--r--   0 bartz      (501) staff       (20)     4887 2023-02-01 14:33:52.000000 spotPython-0.2.4/test/test_set_de_bounds.py
+-rw-r--r--   0 bartz      (501) staff       (20)     2223 2023-02-01 14:33:52.000000 spotPython-0.2.4/test/test_show_progress.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1131 2023-02-01 14:33:52.000000 spotPython-0.2.4/test/test_suggest_new_X.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1765 2023-02-01 14:33:52.000000 spotPython-0.2.4/test/test_update_surrogate.py
+-rw-r--r--   0 bartz      (501) staff       (20)      130 2023-05-19 10:19:58.000000 spotPython-0.2.4/tox.ini
```

### Comparing `spotPython-0.2.3/.github/workflows/test.yml` & `spotPython-0.2.4/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/.gitignore` & `spotPython-0.2.4/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -214,7 +214,15 @@
 docs_old3/site_libs/quarto-search/fuse.min.js
 docs_old3/site_libs/quarto-search/quarto-search.js
 notebooks/data/VBDP/sample_submission.csv
 notebooks/data/VBDP/test.csv
 notebooks/data/VBDP/testt.csv
 notebooks/data/VBDP/train.csv
 notebooks/data/VBDP/trainn.csv
+notebooks/data/MNIST/raw/t10k-images-idx3-ubyte
+notebooks/data/MNIST/raw/t10k-images-idx3-ubyte.gz
+notebooks/data/MNIST/raw/t10k-labels-idx1-ubyte
+notebooks/data/MNIST/raw/t10k-labels-idx1-ubyte.gz
+notebooks/data/MNIST/raw/train-images-idx3-ubyte
+notebooks/data/MNIST/raw/train-images-idx3-ubyte.gz
+notebooks/data/MNIST/raw/train-labels-idx1-ubyte
+notebooks/data/MNIST/raw/train-labels-idx1-ubyte.gz
```

### Comparing `spotPython-0.2.3/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_contour_1_2.pdf` & `spotPython-0.2.4/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_contour_1_2.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_importance.pdf` & `spotPython-0.2.4/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_importance.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_progress.pdf` & `spotPython-0.2.4/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_progress.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_contour_2_3.pdf` & `spotPython-0.2.4/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_contour_2_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_importance.pdf` & `spotPython-0.2.4/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_importance.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_progress.pdf` & `spotPython-0.2.4/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_progress.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_1.pdf` & `spotPython-0.2.4/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_1.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_2.pdf` & `spotPython-0.2.4/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_2.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_3.pdf` & `spotPython-0.2.4/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_4.pdf` & `spotPython-0.2.4/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_2.pdf` & `spotPython-0.2.4/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_2.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_3.pdf` & `spotPython-0.2.4/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_4.pdf` & `spotPython-0.2.4/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_2_3.pdf` & `spotPython-0.2.4/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_2_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_2_4.pdf` & `spotPython-0.2.4/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_2_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_3_4.pdf` & `spotPython-0.2.4/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_3_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_importance.pdf` & `spotPython-0.2.4/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_importance.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_progress.pdf` & `spotPython-0.2.4/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_progress.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_1.pdf` & `spotPython-0.2.4/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_1.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_2.pdf` & `spotPython-0.2.4/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_2.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_3.pdf` & `spotPython-0.2.4/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_4.pdf` & `spotPython-0.2.4/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_2.pdf` & `spotPython-0.2.4/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_2.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_3.pdf` & `spotPython-0.2.4/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_4.pdf` & `spotPython-0.2.4/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_2_3.pdf` & `spotPython-0.2.4/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_2_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_2_4.pdf` & `spotPython-0.2.4/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_2_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_3_4.pdf` & `spotPython-0.2.4/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_3_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_importance.pdf` & `spotPython-0.2.4/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_importance.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_progress.pdf` & `spotPython-0.2.4/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_progress.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_1_2.pdf` & `spotPython-0.2.4/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_1_2.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_1_3.pdf` & `spotPython-0.2.4/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_1_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_2_3.pdf` & `spotPython-0.2.4/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_2_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_importance.pdf` & `spotPython-0.2.4/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_importance.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_progress.pdf` & `spotPython-0.2.4/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_progress.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/Figures.d/13-torch_s7cfd16_600min_20init_2023-05-05_18-52-19_contour_2_3.pdf` & `spotPython-0.2.4/Figures.d/13-torch_s7cfd16_600min_20init_2023-05-05_18-52-19_contour_2_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/LICENSE.txt` & `spotPython-0.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/PKG-INFO` & `spotPython-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotPython
-Version: 0.2.3
+Version: 0.2.4
 Summary: spotPython - Sequential Parameter Optimization in Python
 Author-email: "T. Bartz-Beielstein" <tbb@bartzundbartz.de>
 License: AGPL-3.0-or-later
 Project-URL: Homepage, https://www.spotseven.de
 Project-URL: Issues, https://github.com/sequential-parameter-optimization/spotPython/issues
 Project-URL: Repository, https://github.com/sequential-parameter-optimization/spotPython
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `spotPython-0.2.3/README.md` & `spotPython-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/docs/bart23e.html` & `spotPython-0.2.4/docs/bart23e.html`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/docs/bart23e.pdf` & `spotPython-0.2.4/docs/bart23e.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_1.png` & `spotPython-0.2.4/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_1.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_3.png` & `spotPython-0.2.4/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_3.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_4.png` & `spotPython-0.2.4/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_4.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_3.png` & `spotPython-0.2.4/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_3.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_4.png` & `spotPython-0.2.4/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_4.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_3_4.png` & `spotPython-0.2.4/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_3_4.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_importance.png` & `spotPython-0.2.4/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_importance.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_progress.png` & `spotPython-0.2.4/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_progress.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/docs/figures/parallel.png` & `spotPython-0.2.4/docs/figures/parallel.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/docs/img/spotLogo.png` & `spotPython-0.2.4/docs/img/spotLogo.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/docs/search.json` & `spotPython-0.2.4/docs/search.json`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/docs/site_libs/bootstrap/bootstrap-icons.css` & `spotPython-0.2.4/docs/site_libs/bootstrap/bootstrap-icons.css`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/docs/site_libs/bootstrap/bootstrap-icons.woff` & `spotPython-0.2.4/docs/site_libs/bootstrap/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/docs/site_libs/bootstrap/bootstrap.min.css` & `spotPython-0.2.4/docs/site_libs/bootstrap/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/docs/site_libs/bootstrap/bootstrap.min.js` & `spotPython-0.2.4/docs/site_libs/bootstrap/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/docs/site_libs/clipboard/clipboard.min.js` & `spotPython-0.2.4/docs/site_libs/clipboard/clipboard.min.js`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/docs/site_libs/quarto-html/anchor.min.js` & `spotPython-0.2.4/docs/site_libs/quarto-html/anchor.min.js`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/docs/site_libs/quarto-html/popper.min.js` & `spotPython-0.2.4/docs/site_libs/quarto-html/popper.min.js`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/docs/site_libs/quarto-html/quarto-syntax-highlighting.css` & `spotPython-0.2.4/docs/site_libs/quarto-html/quarto-syntax-highlighting.css`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/docs/site_libs/quarto-html/quarto.js` & `spotPython-0.2.4/docs/site_libs/quarto-html/quarto.js`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/docs/site_libs/quarto-html/tippy.css` & `spotPython-0.2.4/docs/site_libs/quarto-html/tippy.css`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/docs/site_libs/quarto-html/tippy.umd.min.js` & `spotPython-0.2.4/docs/site_libs/quarto-html/tippy.umd.min.js`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/docs/site_libs/quarto-nav/quarto-nav.js` & `spotPython-0.2.4/docs/site_libs/quarto-nav/quarto-nav.js`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/docs/site_libs/quarto-search/autocomplete.umd.js` & `spotPython-0.2.4/docs/site_libs/quarto-search/autocomplete.umd.js`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/docs/site_libs/quarto-search/fuse.min.js` & `spotPython-0.2.4/docs/site_libs/quarto-search/fuse.min.js`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/docs/site_libs/quarto-search/quarto-search.js` & `spotPython-0.2.4/docs/site_libs/quarto-search/quarto-search.js`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/notebooks/00_spot_doc.ipynb` & `spotPython-0.2.4/notebooks/00_spot_doc.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/notebooks/01_spot_intro.ipynb` & `spotPython-0.2.4/notebooks/01_spot_intro.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/notebooks/02_spot_multidim.ipynb` & `spotPython-0.2.4/notebooks/02_spot_multidim.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/notebooks/03_spot_anisotropic.ipynb` & `spotPython-0.2.4/notebooks/03_spot_anisotropic.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/notebooks/04_spot_sklearn_surrogate.ipynb` & `spotPython-0.2.4/notebooks/04_spot_sklearn_surrogate.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/notebooks/05_spot_sklearn_optimizers.ipynb` & `spotPython-0.2.4/notebooks/05_spot_sklearn_optimizers.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/notebooks/06_spot_gaussian.ipynb` & `spotPython-0.2.4/notebooks/06_spot_gaussian.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/notebooks/07_spot_ei.ipynb` & `spotPython-0.2.4/notebooks/07_spot_ei.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/notebooks/08_spot_noisy.ipynb` & `spotPython-0.2.4/notebooks/08_spot_noisy.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/notebooks/09_spot_ocba.ipynb` & `spotPython-0.2.4/notebooks/09_spot_ocba.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/notebooks/10_spot_hpt_sklearn_classification.ipynb` & `spotPython-0.2.4/notebooks/10_spot_hpt_sklearn_classification.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/notebooks/11_spot_hpt_torch_fashion_mnist.ipynb` & `spotPython-0.2.4/notebooks/11_spot_hpt_torch_fashion_mnist.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/notebooks/12_spot_hpt_torch_cifar10.ipynb` & `spotPython-0.2.4/notebooks/12_spot_hpt_torch_cifar10.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/notebooks/13_spot_hpt_torch_cv_fashion_mnist.ipynb` & `spotPython-0.2.4/notebooks/13_spot_hpt_torch_cv_fashion_mnist.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/notebooks/14_spot_ray_hpt_torch_cifar10.ipynb` & `spotPython-0.2.4/notebooks/14_spot_ray_hpt_torch_cifar10.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/notebooks/15_spot_hpt_sklearn_regression.ipynb` & `spotPython-0.2.4/notebooks/15_spot_hpt_sklearn_regression.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/notebooks/data/torch/model_spot_trained.pt` & `spotPython-0.2.4/notebooks/data/torch/model_spot_trained.pt`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_1.png` & `spotPython-0.2.4/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_1.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_3.png` & `spotPython-0.2.4/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_3.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_4.png` & `spotPython-0.2.4/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_4.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_3.png` & `spotPython-0.2.4/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_3.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_4.png` & `spotPython-0.2.4/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_4.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_3_4.png` & `spotPython-0.2.4/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_3_4.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_importance.png` & `spotPython-0.2.4/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_importance.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_progress.png` & `spotPython-0.2.4/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_progress.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/notebooks/figures/figures14-torch_maans03_60min_20init_2023-05-27_23-10-01_parallel.png` & `spotPython-0.2.4/notebooks/figures/figures14-torch_maans03_60min_20init_2023-05-27_23-10-01_parallel.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/notebooks/figures/spotModel.graffle` & `spotPython-0.2.4/notebooks/figures/spotModel.graffle`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/notebooks/figures/spotModel.pdf` & `spotPython-0.2.4/notebooks/figures/spotModel.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/notebooks/figures/spotModel.png` & `spotPython-0.2.4/notebooks/figures/spotModel.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_0_1.pdf` & `spotPython-0.2.4/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_0_1.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_0_2.pdf` & `spotPython-0.2.4/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_0_2.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_0_4.pdf` & `spotPython-0.2.4/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_0_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_1_2.pdf` & `spotPython-0.2.4/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_1_2.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_1_4.pdf` & `spotPython-0.2.4/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_1_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_2_4.pdf` & `spotPython-0.2.4/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_2_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_importance.pdf` & `spotPython-0.2.4/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_importance.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_progress.pdf` & `spotPython-0.2.4/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_progress.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_0_1.pdf` & `spotPython-0.2.4/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_0_1.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_0_2.pdf` & `spotPython-0.2.4/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_0_2.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_0_3.pdf` & `spotPython-0.2.4/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_0_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_1_2.pdf` & `spotPython-0.2.4/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_1_2.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_1_3.pdf` & `spotPython-0.2.4/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_1_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_2_3.pdf` & `spotPython-0.2.4/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_2_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_importance.pdf` & `spotPython-0.2.4/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_importance.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_progress.pdf` & `spotPython-0.2.4/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_progress.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_1.pdf` & `spotPython-0.2.4/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_1.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_3.pdf` & `spotPython-0.2.4/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_4.pdf` & `spotPython-0.2.4/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_3.pdf` & `spotPython-0.2.4/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_4.pdf` & `spotPython-0.2.4/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_3_4.pdf` & `spotPython-0.2.4/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_3_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_importance.pdf` & `spotPython-0.2.4/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_importance.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_progress.pdf` & `spotPython-0.2.4/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_progress.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/notebooks/figures14-torch_maans03_60min_20init_2023-05-27_23-10-01_contour_0_2.png` & `spotPython-0.2.4/notebooks/figures14-torch_maans03_60min_20init_2023-05-27_23-10-01_contour_0_2.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/notebooks/figures14-torch_maans03_60min_20init_2023-05-27_23-10-01_importance.png` & `spotPython-0.2.4/notebooks/figures14-torch_maans03_60min_20init_2023-05-27_23-10-01_importance.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/notebooks/figures14-torch_maans03_60min_20init_2023-05-27_23-10-01_progress.png` & `spotPython-0.2.4/notebooks/figures14-torch_maans03_60min_20init_2023-05-27_23-10-01_progress.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/notebooks/plot.png` & `spotPython-0.2.4/notebooks/plot.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/pyproject.toml` & `spotPython-0.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
   "setuptools>=61.0",
   "setuptools_scm[toml]"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "spotPython"
-version = "0.2.3"
+version = "0.2.4"
 authors = [
   { name="T. Bartz-Beielstein", email="tbb@bartzundbartz.de" }
 ]
 description = "spotPython - Sequential Parameter Optimization in Python"
 readme = "README.md"
 license = { text="AGPL-3.0-or-later" }
 requires-python = ">=3.10"
```

### Comparing `spotPython-0.2.3/src/spotPython/budget/ocba.py` & `spotPython-0.2.4/src/spotPython/budget/ocba.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/src/spotPython/build/kriging.py` & `spotPython-0.2.4/src/spotPython/build/kriging.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/src/spotPython/data/base.py` & `spotPython-0.2.4/src/spotPython/data/base.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/src/spotPython/data/sklearn_hyper_dict.json` & `spotPython-0.2.4/src/spotPython/data/sklearn_hyper_dict.json`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/src/spotPython/data/torch_hyper_dict.json` & `spotPython-0.2.4/src/spotPython/data/torch_hyper_dict.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.75%*

 * *Differences: {"'Net_vbdp'": "OrderedDict([('l1', OrderedDict([('type', 'int'), ('default', 5), ('transform', "*

 * *               "'transform_power_2_int'), ('lower', 2), ('upper', 9)])), ('l2', "*

 * *               "OrderedDict([('type', 'int'), ('default', 5), ('transform', "*

 * *               "'transform_power_2_int'), ('lower', 2), ('upper', 9)])), ('lr_mult', "*

 * *               "OrderedDict([('type', 'float'), ('default', 1.0), ('transform', 'None'), ('lower', "*

 * *               "0.1), ('upper', 10.0)])), ('batch_size', OrderedDi […]*

```diff
@@ -156,14 +156,95 @@
             "default": 0.0,
             "lower": 0.0,
             "transform": "None",
             "type": "float",
             "upper": 1.0
         }
     },
+    "Net_vbdp": {
+        "batch_size": {
+            "default": 4,
+            "lower": 1,
+            "transform": "transform_power_2_int",
+            "type": "int",
+            "upper": 4
+        },
+        "epochs": {
+            "default": 3,
+            "lower": 3,
+            "transform": "transform_power_2_int",
+            "type": "int",
+            "upper": 4
+        },
+        "k_folds": {
+            "default": 1,
+            "lower": 1,
+            "transform": "None",
+            "type": "int",
+            "upper": 1
+        },
+        "l1": {
+            "default": 5,
+            "lower": 2,
+            "transform": "transform_power_2_int",
+            "type": "int",
+            "upper": 9
+        },
+        "l2": {
+            "default": 5,
+            "lower": 2,
+            "transform": "transform_power_2_int",
+            "type": "int",
+            "upper": 9
+        },
+        "lr_mult": {
+            "default": 1.0,
+            "lower": 0.1,
+            "transform": "None",
+            "type": "float",
+            "upper": 10.0
+        },
+        "optimizer": {
+            "class_name": "torch.optim",
+            "core_model_parameter_type": "str",
+            "default": "SGD",
+            "levels": [
+                "Adadelta",
+                "Adagrad",
+                "Adam",
+                "AdamW",
+                "SparseAdam",
+                "Adamax",
+                "ASGD",
+                "NAdam",
+                "RAdam",
+                "RMSprop",
+                "Rprop",
+                "SGD"
+            ],
+            "lower": 0,
+            "transform": "None",
+            "type": "factor",
+            "upper": 12
+        },
+        "patience": {
+            "default": 5,
+            "lower": 2,
+            "transform": "None",
+            "type": "int",
+            "upper": 10
+        },
+        "sgd_momentum": {
+            "default": 0.0,
+            "lower": 0.0,
+            "transform": "None",
+            "type": "float",
+            "upper": 1.0
+        }
+    },
     "Template": {
         "bool_hyperparameter": {
             "core_model_parameter_type": "bool",
             "default": 0,
             "levels": [
                 0,
                 1
```

### Comparing `spotPython-0.2.3/src/spotPython/design/spacefilling.py` & `spotPython-0.2.4/src/spotPython/design/spacefilling.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/src/spotPython/fun/hypersklearn.py` & `spotPython-0.2.4/src/spotPython/fun/hypersklearn.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/src/spotPython/fun/hypertorch.py` & `spotPython-0.2.4/src/spotPython/fun/hypertorch.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/src/spotPython/fun/objectivefunctions.py` & `spotPython-0.2.4/src/spotPython/fun/objectivefunctions.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/src/spotPython/hyperparameters/categorical.py` & `spotPython-0.2.4/src/spotPython/hyperparameters/categorical.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/src/spotPython/hyperparameters/optimizer.py` & `spotPython-0.2.4/src/spotPython/hyperparameters/optimizer.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/src/spotPython/hyperparameters/values.py` & `spotPython-0.2.4/src/spotPython/hyperparameters/values.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/src/spotPython/plot/contour.py` & `spotPython-0.2.4/src/spotPython/plot/contour.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/src/spotPython/plot/validation.py` & `spotPython-0.2.4/src/spotPython/plot/validation.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/src/spotPython/sklearn/traintest.py` & `spotPython-0.2.4/src/spotPython/sklearn/traintest.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/src/spotPython/spot/spot.py` & `spotPython-0.2.4/src/spotPython/spot/spot.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/src/spotPython/torch/netcifar10.py` & `spotPython-0.2.4/src/spotPython/torch/netcifar10.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/src/spotPython/torch/netfashionMNIST.py` & `spotPython-0.2.4/src/spotPython/torch/netfashionMNIST.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/src/spotPython/torch/traintest.py` & `spotPython-0.2.4/src/spotPython/torch/traintest.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/src/spotPython/utils/aggregate.py` & `spotPython-0.2.4/src/spotPython/utils/aggregate.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/src/spotPython/utils/compare.py` & `spotPython-0.2.4/src/spotPython/utils/compare.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/src/spotPython/utils/convert.py` & `spotPython-0.2.4/src/spotPython/utils/convert.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/src/spotPython/utils/device.py` & `spotPython-0.2.4/src/spotPython/utils/device.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/src/spotPython/utils/eda.py` & `spotPython-0.2.4/src/spotPython/utils/eda.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/src/spotPython/utils/init.py` & `spotPython-0.2.4/src/spotPython/utils/init.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/src/spotPython/utils/metrics.py` & `spotPython-0.2.4/src/spotPython/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/src/spotPython/utils/progress.py` & `spotPython-0.2.4/src/spotPython/utils/progress.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/src/spotPython/utils/repair.py` & `spotPython-0.2.4/src/spotPython/utils/repair.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/src/spotPython/utils/transform.py` & `spotPython-0.2.4/src/spotPython/utils/transform.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/src/spotPython.egg-info/PKG-INFO` & `spotPython-0.2.4/src/spotPython.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotPython
-Version: 0.2.3
+Version: 0.2.4
 Summary: spotPython - Sequential Parameter Optimization in Python
 Author-email: "T. Bartz-Beielstein" <tbb@bartzundbartz.de>
 License: AGPL-3.0-or-later
 Project-URL: Homepage, https://www.spotseven.de
 Project-URL: Issues, https://github.com/sequential-parameter-optimization/spotPython/issues
 Project-URL: Repository, https://github.com/sequential-parameter-optimization/spotPython
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `spotPython-0.2.3/src/spotPython.egg-info/SOURCES.txt` & `spotPython-0.2.4/src/spotPython.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -85,17 +85,18 @@
 notebooks/09_spot_ocba.ipynb
 notebooks/10_spot_hpt_sklearn_classification.ipynb
 notebooks/11_spot_hpt_torch_fashion_mnist.ipynb
 notebooks/12_spot_hpt_torch_cifar10.ipynb
 notebooks/13_spot_hpt_torch_cv_fashion_mnist.ipynb
 notebooks/14_spot_ray_hpt_torch_cifar10.ipynb
 notebooks/15_spot_hpt_sklearn_regression.ipynb
-notebooks/16_spot_hpt_sklearn_multiclass_classification.ipynb
+notebooks/16_spot_hpt_sklearn_multiclass_classification_randomforest.ipynb
 notebooks/17_spot_hpt_sklearn_multiclass_classification_xgb.ipynb
 notebooks/18_spot_hpt_sklearn_multiclass_classification_svc.ipynb
+notebooks/19_spot_hpt_sklearn_multiclass_classification_knn.ipynb
 notebooks/data.json
 notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_0_1.pdf
 notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_0_2.pdf
 notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_0_4.pdf
 notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_1_2.pdf
 notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_1_4.pdf
 notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_2_4.pdf
@@ -159,17 +160,19 @@
 src/spotPython/hyperparameters/categorical.py
 src/spotPython/hyperparameters/optimizer.py
 src/spotPython/hyperparameters/values.py
 src/spotPython/plot/contour.py
 src/spotPython/plot/validation.py
 src/spotPython/sklearn/traintest.py
 src/spotPython/spot/spot.py
+src/spotPython/torch/mapk.py
 src/spotPython/torch/netcifar10.py
 src/spotPython/torch/netcore.py
 src/spotPython/torch/netfashionMNIST.py
+src/spotPython/torch/netvbdp.py
 src/spotPython/torch/traintest.py
 src/spotPython/utils/aggregate.py
 src/spotPython/utils/classes.py
 src/spotPython/utils/compare.py
 src/spotPython/utils/convert.py
 src/spotPython/utils/device.py
 src/spotPython/utils/eda.py
```

### Comparing `spotPython-0.2.3/test/test_aggregate_mean_var.py` & `spotPython-0.2.4/test/test_aggregate_mean_var.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/test/test_build_Psi.py` & `spotPython-0.2.4/test/test_build_Psi.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/test/test_build_U.py` & `spotPython-0.2.4/test/test_build_U.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/test/test_build_psi_vec.py` & `spotPython-0.2.4/test/test_build_psi_vec.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/test/test_evaluate_new_X.py` & `spotPython-0.2.4/test/test_evaluate_new_X.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/test/test_evaluate_new_solutions.py` & `spotPython-0.2.4/test/test_evaluate_new_solutions.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/test/test_extract_from_bounds.py` & `spotPython-0.2.4/test/test_extract_from_bounds.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/test/test_generate_design.py` & `spotPython-0.2.4/test/test_generate_design.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/test/test_infill.py` & `spotPython-0.2.4/test/test_infill.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/test/test_nat_to_cod.py` & `spotPython-0.2.4/test/test_nat_to_cod.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/test/test_nat_to_cod_init.py` & `spotPython-0.2.4/test/test_nat_to_cod_init.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/test/test_ocba.py` & `spotPython-0.2.4/test/test_ocba.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/test/test_repair_non_numeric.py` & `spotPython-0.2.4/test/test_repair_non_numeric.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/test/test_set_de_bounds.py` & `spotPython-0.2.4/test/test_set_de_bounds.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/test/test_show_progress.py` & `spotPython-0.2.4/test/test_show_progress.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/test/test_suggest_new_X.py` & `spotPython-0.2.4/test/test_suggest_new_X.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.3/test/test_update_surrogate.py` & `spotPython-0.2.4/test/test_update_surrogate.py`

 * *Files identical despite different names*

