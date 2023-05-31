# Comparing `tmp/pdfo-1.3.tar.gz` & `tmp/pdfo-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdfo-1.3.tar", last modified: Tue Apr 25 10:58:59 2023, max compression
+gzip compressed data, was "pdfo-1.3.1.tar", last modified: Wed May 31 16:13:46 2023, max compression
```

## Comparing `pdfo-1.3.tar` & `pdfo-1.3.1.tar`

### file list

```diff
@@ -1,218 +1,218 @@
--rw-r--r--   0        0        0      241 1970-01-01 00:00:00.000000 pdfo-1.3/.github/CODEOWNERS
--rw-r--r--   0        0        0     2508 1970-01-01 00:00:00.000000 pdfo-1.3/.github/actions/spelling/README.md
--rw-r--r--   0        0        0     1184 1970-01-01 00:00:00.000000 pdfo-1.3/.github/actions/spelling/advice.md
--rw-r--r--   0        0        0     2672 1970-01-01 00:00:00.000000 pdfo-1.3/.github/actions/spelling/allow.txt
--rw-r--r--   0        0        0    14657 1970-01-01 00:00:00.000000 pdfo-1.3/.github/actions/spelling/candidate.patterns
--rw-r--r--   0        0        0      932 1970-01-01 00:00:00.000000 pdfo-1.3/.github/actions/spelling/excludes.txt
--rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 pdfo-1.3/.github/actions/spelling/expect.txt
--rw-r--r--   0        0        0     1018 1970-01-01 00:00:00.000000 pdfo-1.3/.github/actions/spelling/line_forbidden.patterns
--rw-r--r--   0        0        0     1917 1970-01-01 00:00:00.000000 pdfo-1.3/.github/actions/spelling/patterns.txt
--rw-r--r--   0        0        0      100 1970-01-01 00:00:00.000000 pdfo-1.3/.github/actions/spelling/reject.txt
--rw-r--r--   0        0        0      347 1970-01-01 00:00:00.000000 pdfo-1.3/.github/dependabot.yml
--rw-r--r--   0        0        0     3837 1970-01-01 00:00:00.000000 pdfo-1.3/.github/workflows/build.yml
--rw-r--r--   0        0        0     1422 1970-01-01 00:00:00.000000 pdfo-1.3/.github/workflows/pypi.yml
--rw-r--r--   0        0        0     5084 1970-01-01 00:00:00.000000 pdfo-1.3/.github/workflows/spelling.yml
--rw-r--r--   0        0        0     2249 1970-01-01 00:00:00.000000 pdfo-1.3/.gitignore
--rw-r--r--   0        0        0     3622 1970-01-01 00:00:00.000000 pdfo-1.3/CHANGELOG.txt
--rw-r--r--   0        0        0     1526 1970-01-01 00:00:00.000000 pdfo-1.3/LICENCE.txt
--rw-r--r--   0        0        0     9747 1970-01-01 00:00:00.000000 pdfo-1.3/README.md
--rw-r--r--   0        0        0        3 1970-01-01 00:00:00.000000 pdfo-1.3/VERSION.txt
--rw-r--r--   0        0        0      565 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/bobyqa/README.txt
--rw-r--r--   0        0        0    10597 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/bobyqa/altmov.f
--rw-r--r--   0        0        0     8361 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/bobyqa/bobyqa.f
--rw-r--r--   0        0        0    33932 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/bobyqa/bobyqb.f
--rw-r--r--   0        0        0     6693 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/bobyqa/prelim.f
--rw-r--r--   0        0        0    16890 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/bobyqa/rescue.f
--rw-r--r--   0        0        0    14015 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/bobyqa/trsbox.f
--rw-r--r--   0        0        0     2813 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/bobyqa/update.f
--rw-r--r--   0        0        0      672 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/classical/bobyqa/README.txt
--rw-r--r--   0        0        0    10247 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/classical/bobyqa/altmov.f
--rw-r--r--   0        0        0     7628 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/classical/bobyqa/bobyqa.f
--rw-r--r--   0        0        0    28015 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/classical/bobyqa/bobyqb.f
--rw-r--r--   0        0        0     6335 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/classical/bobyqa/prelim.f
--rw-r--r--   0        0        0    16297 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/classical/bobyqa/rescue.f
--rw-r--r--   0        0        0    13651 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/classical/bobyqa/trsbox.f
--rw-r--r--   0        0        0     2628 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/classical/bobyqa/update.f
--rw-r--r--   0        0        0      672 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/classical/cobyla/README.txt
--rw-r--r--   0        0        0     5862 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/classical/cobyla/cobyla.f
--rw-r--r--   0        0        0    23777 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/classical/cobyla/cobylb.f
--rw-r--r--   0        0        0    24665 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/classical/cobyla/trstlp.f
--rw-r--r--   0        0        0      672 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/classical/lincoa/README.txt
--rw-r--r--   0        0        0     9498 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/classical/lincoa/getact.f
--rw-r--r--   0        0        0     9093 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/classical/lincoa/lincoa.f
--rw-r--r--   0        0        0    24070 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/classical/lincoa/lincob.f
--rw-r--r--   0        0        0     6937 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/classical/lincoa/prelim.f
--rw-r--r--   0        0        0     7825 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/classical/lincoa/qmstep.f
--rw-r--r--   0        0        0    10467 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/classical/lincoa/trstep.f
--rw-r--r--   0        0        0     7137 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/classical/lincoa/update.f
--rw-r--r--   0        0        0      673 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/classical/newuoa/README.txt
--rw-r--r--   0        0        0    11030 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/classical/newuoa/bigden.f
--rw-r--r--   0        0        0     5589 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/classical/newuoa/biglag.f
--rw-r--r--   0        0        0     5036 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/classical/newuoa/newuoa.f
--rw-r--r--   0        0        0    20108 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/classical/newuoa/newuob.f
--rw-r--r--   0        0        0     6132 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/classical/newuoa/trsapp.f
--rw-r--r--   0        0        0     3780 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/classical/newuoa/update.f
--rw-r--r--   0        0        0      672 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/classical/uobyqa/README.txt
--rw-r--r--   0        0        0     5474 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/classical/uobyqa/lagmax.f
--rw-r--r--   0        0        0    11444 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/classical/uobyqa/trstep.f
--rw-r--r--   0        0        0     4223 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/classical/uobyqa/uobyqa.f
--rw-r--r--   0        0        0    16150 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/classical/uobyqa/uobyqb.f
--rw-r--r--   0        0        0      565 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/cobyla/README.txt
--rw-r--r--   0        0        0     6403 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/cobyla/cobyla.f
--rw-r--r--   0        0        0    43669 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/cobyla/cobylb.f
--rw-r--r--   0        0        0    26246 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/cobyla/trstlp.f
--rw-r--r--   0        0        0      565 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/lincoa/README.txt
--rw-r--r--   0        0        0     9795 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/lincoa/getact.f
--rw-r--r--   0        0        0     9648 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/lincoa/lincoa.f
--rw-r--r--   0        0        0    31859 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/lincoa/lincob.f
--rw-r--r--   0        0        0     7925 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/lincoa/prelim.f
--rw-r--r--   0        0        0     8882 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/lincoa/qmstep.f
--rw-r--r--   0        0        0    11603 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/lincoa/trstep.f
--rw-r--r--   0        0        0     7137 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/lincoa/update.f
--rw-r--r--   0        0        0      565 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/newuoa/README.txt
--rw-r--r--   0        0        0    11673 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/newuoa/bigden.f
--rw-r--r--   0        0        0     5589 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/newuoa/biglag.f
--rw-r--r--   0        0        0     5577 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/newuoa/newuoa.f
--rw-r--r--   0        0        0    25387 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/newuoa/newuob.f
--rw-r--r--   0        0        0     6132 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/newuoa/trsapp.f
--rw-r--r--   0        0        0     3780 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/newuoa/update.f
--rw-r--r--   0        0        0      421 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/original/README.txt
--rw-r--r--   0        0        0      468 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/original/bobyqa/LICENCE.txt
--rw-r--r--   0        0        0      846 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/original/bobyqa/Makefile
--rw-r--r--   0        0        0     3652 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/original/bobyqa/README.txt
--rw-r--r--   0        0        0     9321 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/original/bobyqa/altmov.f
--rw-r--r--   0        0        0     5420 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/original/bobyqa/bobyqa.f
--rw-r--r--   0        0        0    22912 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/original/bobyqa/bobyqb.f
--rw-r--r--   0        0        0      267 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/original/bobyqa/calfun.f
--rw-r--r--   0        0        0    87233 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/original/bobyqa/email.txt
--rw-r--r--   0        0        0     1581 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/original/bobyqa/main.f
--rw-r--r--   0        0        0     9268 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/original/bobyqa/output.txt
--rw-r--r--   0        0        0     5572 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/original/bobyqa/prelim.f
--rw-r--r--   0        0        0    13215 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/original/bobyqa/rescue.f
--rw-r--r--   0        0        0    12773 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/original/bobyqa/trsbox.f
--rw-r--r--   0        0        0     2258 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/original/bobyqa/update.f
--rw-r--r--   0        0        0      471 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/original/cobyla/LICENCE.txt
--rw-r--r--   0        0        0      652 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/original/cobyla/Makefile
--rw-r--r--   0        0        0     2230 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/original/cobyla/README.txt
--rw-r--r--   0        0        0     2891 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/original/cobyla/calcfc.f
--rw-r--r--   0        0        0     4150 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/original/cobyla/cobyla.f
--rw-r--r--   0        0        0    12977 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/original/cobyla/cobylb.f
--rw-r--r--   0        0        0    46750 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/original/cobyla/email.txt
--rw-r--r--   0        0        0     4746 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/original/cobyla/main.f
--rw-r--r--   0        0        0     5662 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/original/cobyla/output.txt
--rw-r--r--   0        0        0    14234 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/original/cobyla/trstlp.f
--rw-r--r--   0        0        0      468 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/original/lincoa/LICENCE.txt
--rw-r--r--   0        0        0      852 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/original/lincoa/Makefile
--rw-r--r--   0        0        0     3183 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/original/lincoa/README.txt
--rw-r--r--   0        0        0      740 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/original/lincoa/calfun.f
--rw-r--r--   0        0        0    74855 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/original/lincoa/email.txt
--rw-r--r--   0        0        0     8764 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/original/lincoa/getact.f
--rw-r--r--   0        0        0     6580 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/original/lincoa/lincoa.f
--rw-r--r--   0        0        0    19696 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/original/lincoa/lincob.f
--rw-r--r--   0        0        0     3527 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/original/lincoa/main.f
--rw-r--r--   0        0        0     2424 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/original/lincoa/output.txt
--rw-r--r--   0        0        0     5760 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/original/lincoa/prelim.f
--rw-r--r--   0        0        0     7105 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/original/lincoa/qmstep.f
--rw-r--r--   0        0        0     9620 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/original/lincoa/trstep.f
--rw-r--r--   0        0        0     6453 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/original/lincoa/update.f
--rw-r--r--   0        0        0      463 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/original/newuoa/LICENCE.txt
--rw-r--r--   0        0        0      775 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/original/newuoa/Makefile
--rw-r--r--   0        0        0     3018 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/original/newuoa/README.txt
--rw-r--r--   0        0        0     9726 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/original/newuoa/bigden.f
--rw-r--r--   0        0        0     4967 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/original/newuoa/biglag.f
--rw-r--r--   0        0        0      482 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/original/newuoa/calfun.f
--rw-r--r--   0        0        0    54137 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/original/newuoa/email.txt
--rw-r--r--   0        0        0      499 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/original/newuoa/main.f
--rw-r--r--   0        0        0     3121 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/original/newuoa/newuoa.f
--rw-r--r--   0        0        0    17248 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/original/newuoa/newuob.f
--rw-r--r--   0        0        0     5220 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/original/newuoa/output.txt
--rw-r--r--   0        0        0     5595 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/original/newuoa/trsapp.f
--rw-r--r--   0        0        0     3413 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/original/newuoa/update.f
--rw-r--r--   0        0        0      476 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/original/uobyqa/LICENCE.txt
--rw-r--r--   0        0        0      620 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/original/uobyqa/Makefile
--rw-r--r--   0        0        0     1805 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/original/uobyqa/README.txt
--rw-r--r--   0        0        0      480 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/original/uobyqa/calfun.f
--rw-r--r--   0        0        0    42243 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/original/uobyqa/email.txt
--rw-r--r--   0        0        0     4896 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/original/uobyqa/lagmax.f
--rw-r--r--   0        0        0      490 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/original/uobyqa/main.f
--rw-r--r--   0        0        0     7136 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/original/uobyqa/output.txt
--rw-r--r--   0        0        0    10587 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/original/uobyqa/trstep.f
--rw-r--r--   0        0        0     2448 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/original/uobyqa/uobyqa.f
--rw-r--r--   0        0        0    13781 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/original/uobyqa/uobyqb.f
--rw-r--r--   0        0        0     2429 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/pdfoconst.F
--rw-r--r--   0        0        0      565 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/uobyqa/README.txt
--rw-r--r--   0        0        0     5474 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/uobyqa/lagmax.f
--rw-r--r--   0        0        0    12771 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/uobyqa/trstep.f
--rw-r--r--   0        0        0     4764 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/uobyqa/uobyqa.f
--rw-r--r--   0        0        0    19824 1970-01-01 00:00:00.000000 pdfo-1.3/fsrc/uobyqa/uobyqb.f
--rw-r--r--   0        0        0     2633 1970-01-01 00:00:00.000000 pdfo-1.3/matlab/examples/rosenbrock_example.m
--rw-r--r--   0        0        0    11557 1970-01-01 00:00:00.000000 pdfo-1.3/matlab/examples/testpdfo.m
--rw-r--r--   0        0        0    16383 1970-01-01 00:00:00.000000 pdfo-1.3/matlab/interfaces/bobyqa.m
--rw-r--r--   0        0        0    20906 1970-01-01 00:00:00.000000 pdfo-1.3/matlab/interfaces/cobyla.m
--rw-r--r--   0        0        0    19739 1970-01-01 00:00:00.000000 pdfo-1.3/matlab/interfaces/lincoa.m
--rw-r--r--   0        0        0    14008 1970-01-01 00:00:00.000000 pdfo-1.3/matlab/interfaces/newuoa.m
--rw-r--r--   0        0        0    20452 1970-01-01 00:00:00.000000 pdfo-1.3/matlab/interfaces/pdfo.m
--rw-r--r--   0        0        0     1691 1970-01-01 00:00:00.000000 pdfo-1.3/matlab/interfaces/private/mystrjoin.m
--rw-r--r--   0        0        0     3321 1970-01-01 00:00:00.000000 pdfo-1.3/matlab/interfaces/private/package_info.m
--rw-r--r--   0        0        0    29859 1970-01-01 00:00:00.000000 pdfo-1.3/matlab/interfaces/private/postpdfo.m
--rw-r--r--   0        0        0    74568 1970-01-01 00:00:00.000000 pdfo-1.3/matlab/interfaces/private/prepdfo.m
--rw-r--r--   0        0        0    11600 1970-01-01 00:00:00.000000 pdfo-1.3/matlab/interfaces/private/project.m
--rw-r--r--   0        0        0    13759 1970-01-01 00:00:00.000000 pdfo-1.3/matlab/interfaces/uobyqa.m
--rw-r--r--   0        0        0    19286 1970-01-01 00:00:00.000000 pdfo-1.3/matlab/mex_gateways/bobyqa-interface.F
--rw-r--r--   0        0        0    18731 1970-01-01 00:00:00.000000 pdfo-1.3/matlab/mex_gateways/classical/bobyqa-interface.F
--rw-r--r--   0        0        0    20503 1970-01-01 00:00:00.000000 pdfo-1.3/matlab/mex_gateways/classical/cobyla-interface.F
--rw-r--r--   0        0        0    20682 1970-01-01 00:00:00.000000 pdfo-1.3/matlab/mex_gateways/classical/lincoa-interface.F
--rw-r--r--   0        0        0    14826 1970-01-01 00:00:00.000000 pdfo-1.3/matlab/mex_gateways/classical/newuoa-interface.F
--rw-r--r--   0        0        0    14543 1970-01-01 00:00:00.000000 pdfo-1.3/matlab/mex_gateways/classical/uobyqa-interface.F
--rw-r--r--   0        0        0    22204 1970-01-01 00:00:00.000000 pdfo-1.3/matlab/mex_gateways/cobyla-interface.F
--rw-r--r--   0        0        0     5860 1970-01-01 00:00:00.000000 pdfo-1.3/matlab/mex_gateways/gethuge.F
--rw-r--r--   0        0        0    21214 1970-01-01 00:00:00.000000 pdfo-1.3/matlab/mex_gateways/lincoa-interface.F
--rw-r--r--   0        0        0    15309 1970-01-01 00:00:00.000000 pdfo-1.3/matlab/mex_gateways/newuoa-interface.F
--rw-r--r--   0        0        0    15177 1970-01-01 00:00:00.000000 pdfo-1.3/matlab/mex_gateways/uobyqa-interface.F
--rw-r--r--   0        0        0      405 1970-01-01 00:00:00.000000 pdfo-1.3/meson.build
--rw-r--r--   0        0        0     2764 1970-01-01 00:00:00.000000 pdfo-1.3/pyproject.toml
--rw-r--r--   0        0        0      174 1970-01-01 00:00:00.000000 pdfo-1.3/python/build_tools/build_sdist.sh
--rw-r--r--   0        0        0       99 1970-01-01 00:00:00.000000 pdfo-1.3/python/build_tools/cibw_before_build_macos.sh
--rw-r--r--   0        0        0      197 1970-01-01 00:00:00.000000 pdfo-1.3/python/build_tools/cibw_repair_wheel_command_windows.sh
--rw-r--r--   0        0        0       69 1970-01-01 00:00:00.000000 pdfo-1.3/python/build_tools/cibw_test_command.sh
--rw-r--r--   0        0        0      276 1970-01-01 00:00:00.000000 pdfo-1.3/python/build_tools/download_anaconda.sh
--rw-r--r--   0        0        0      190 1970-01-01 00:00:00.000000 pdfo-1.3/python/build_tools/test_sdist.sh
--rw-r--r--   0        0        0      364 1970-01-01 00:00:00.000000 pdfo-1.3/python/build_tools/upload_anaconda.sh
--rwxr-xr-x   0        0        0     3222 1970-01-01 00:00:00.000000 pdfo-1.3/python/examples/rosenbrock.py
--rw-r--r--   0        0        0     1670 1970-01-01 00:00:00.000000 pdfo-1.3/python/pdfo/__init__.py
--rw-r--r--   0        0        0    11245 1970-01-01 00:00:00.000000 pdfo-1.3/python/pdfo/_bobyqa.py
--rw-r--r--   0        0        0    12881 1970-01-01 00:00:00.000000 pdfo-1.3/python/pdfo/_cobyla.py
--rw-r--r--   0        0        0   182163 1970-01-01 00:00:00.000000 pdfo-1.3/python/pdfo/_dependencies.py
--rw-r--r--   0        0        0    13304 1970-01-01 00:00:00.000000 pdfo-1.3/python/pdfo/_lincoa.py
--rw-r--r--   0        0        0     8787 1970-01-01 00:00:00.000000 pdfo-1.3/python/pdfo/_newuoa.py
--rw-r--r--   0        0        0    13373 1970-01-01 00:00:00.000000 pdfo-1.3/python/pdfo/_pdfo.py
--rw-r--r--   0        0        0     8379 1970-01-01 00:00:00.000000 pdfo-1.3/python/pdfo/_uobyqa.py
--rw-r--r--   0        0        0     3621 1970-01-01 00:00:00.000000 pdfo-1.3/python/pdfo/meson.build
--rw-r--r--   0        0        0      434 1970-01-01 00:00:00.000000 pdfo-1.3/python/pdfo/tests/__init__.py
--rw-r--r--   0        0        0       86 1970-01-01 00:00:00.000000 pdfo-1.3/python/pdfo/tests/meson.build
--rwxr-xr-x   0        0        0    12440 1970-01-01 00:00:00.000000 pdfo-1.3/python/pdfo/tests/test_pdfo.py
--rw-r--r--   0        0        0     2293 1970-01-01 00:00:00.000000 pdfo-1.3/python/py_gateways/bobyqa-interface.pyf
--rw-r--r--   0        0        0     2152 1970-01-01 00:00:00.000000 pdfo-1.3/python/py_gateways/bobyqa.f90
--rw-r--r--   0        0        0     2313 1970-01-01 00:00:00.000000 pdfo-1.3/python/py_gateways/classical/bobyqa-interface.pyf
--rw-r--r--   0        0        0     2000 1970-01-01 00:00:00.000000 pdfo-1.3/python/py_gateways/classical/bobyqa.f90
--rw-r--r--   0        0        0     2617 1970-01-01 00:00:00.000000 pdfo-1.3/python/py_gateways/classical/cobyla-interface.pyf
--rw-r--r--   0        0        0     2533 1970-01-01 00:00:00.000000 pdfo-1.3/python/py_gateways/classical/cobyla.f90
--rw-r--r--   0        0        0     2422 1970-01-01 00:00:00.000000 pdfo-1.3/python/py_gateways/classical/lincoa-interface.pyf
--rw-r--r--   0        0        0     2467 1970-01-01 00:00:00.000000 pdfo-1.3/python/py_gateways/classical/lincoa.f90
--rw-r--r--   0        0        0     1846 1970-01-01 00:00:00.000000 pdfo-1.3/python/py_gateways/classical/newuoa-interface.pyf
--rw-r--r--   0        0        0     1287 1970-01-01 00:00:00.000000 pdfo-1.3/python/py_gateways/classical/newuoa.f90
--rw-r--r--   0        0        0     1818 1970-01-01 00:00:00.000000 pdfo-1.3/python/py_gateways/classical/uobyqa-interface.pyf
--rw-r--r--   0        0        0     1290 1970-01-01 00:00:00.000000 pdfo-1.3/python/py_gateways/classical/uobyqa.f90
--rw-r--r--   0        0        0     2597 1970-01-01 00:00:00.000000 pdfo-1.3/python/py_gateways/cobyla-interface.pyf
--rw-r--r--   0        0        0     3147 1970-01-01 00:00:00.000000 pdfo-1.3/python/py_gateways/cobyla.f90
--rw-r--r--   0        0        0      634 1970-01-01 00:00:00.000000 pdfo-1.3/python/py_gateways/gethuge-interface.pyf
--rw-r--r--   0        0        0     2622 1970-01-01 00:00:00.000000 pdfo-1.3/python/py_gateways/gethuge.f90
--rw-r--r--   0        0        0     2402 1970-01-01 00:00:00.000000 pdfo-1.3/python/py_gateways/lincoa-interface.pyf
--rw-r--r--   0        0        0     2619 1970-01-01 00:00:00.000000 pdfo-1.3/python/py_gateways/lincoa.f90
--rw-r--r--   0        0        0     1826 1970-01-01 00:00:00.000000 pdfo-1.3/python/py_gateways/newuoa-interface.pyf
--rw-r--r--   0        0        0     1439 1970-01-01 00:00:00.000000 pdfo-1.3/python/py_gateways/newuoa.f90
--rw-r--r--   0        0        0      524 1970-01-01 00:00:00.000000 pdfo-1.3/python/py_gateways/pdfoconst-interface.pyf
--rw-r--r--   0        0        0     1798 1970-01-01 00:00:00.000000 pdfo-1.3/python/py_gateways/uobyqa-interface.pyf
--rw-r--r--   0        0        0     1442 1970-01-01 00:00:00.000000 pdfo-1.3/python/py_gateways/uobyqa.f90
--rw-r--r--   0        0        0    23270 1970-01-01 00:00:00.000000 pdfo-1.3/setup.m
--rw-r--r--   0        0        0    13510 1970-01-01 00:00:00.000000 pdfo-1.3/PKG-INFO
+-rw-r--r--   0        0        0      241 1970-01-01 00:00:00.000000 pdfo-1.3.1/.github/CODEOWNERS
+-rw-r--r--   0        0        0     2508 1970-01-01 00:00:00.000000 pdfo-1.3.1/.github/actions/spelling/README.md
+-rw-r--r--   0        0        0     1184 1970-01-01 00:00:00.000000 pdfo-1.3.1/.github/actions/spelling/advice.md
+-rw-r--r--   0        0        0     2672 1970-01-01 00:00:00.000000 pdfo-1.3.1/.github/actions/spelling/allow.txt
+-rw-r--r--   0        0        0    14657 1970-01-01 00:00:00.000000 pdfo-1.3.1/.github/actions/spelling/candidate.patterns
+-rw-r--r--   0        0        0      932 1970-01-01 00:00:00.000000 pdfo-1.3.1/.github/actions/spelling/excludes.txt
+-rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 pdfo-1.3.1/.github/actions/spelling/expect.txt
+-rw-r--r--   0        0        0     1018 1970-01-01 00:00:00.000000 pdfo-1.3.1/.github/actions/spelling/line_forbidden.patterns
+-rw-r--r--   0        0        0     1917 1970-01-01 00:00:00.000000 pdfo-1.3.1/.github/actions/spelling/patterns.txt
+-rw-r--r--   0        0        0      100 1970-01-01 00:00:00.000000 pdfo-1.3.1/.github/actions/spelling/reject.txt
+-rw-r--r--   0        0        0      347 1970-01-01 00:00:00.000000 pdfo-1.3.1/.github/dependabot.yml
+-rw-r--r--   0        0        0     3837 1970-01-01 00:00:00.000000 pdfo-1.3.1/.github/workflows/build.yml
+-rw-r--r--   0        0        0     1422 1970-01-01 00:00:00.000000 pdfo-1.3.1/.github/workflows/pypi.yml
+-rw-r--r--   0        0        0     5084 1970-01-01 00:00:00.000000 pdfo-1.3.1/.github/workflows/spelling.yml
+-rw-r--r--   0        0        0     2249 1970-01-01 00:00:00.000000 pdfo-1.3.1/.gitignore
+-rw-r--r--   0        0        0     3622 1970-01-01 00:00:00.000000 pdfo-1.3.1/CHANGELOG.txt
+-rw-r--r--   0        0        0     1526 1970-01-01 00:00:00.000000 pdfo-1.3.1/LICENCE.txt
+-rw-r--r--   0        0        0     9913 1970-01-01 00:00:00.000000 pdfo-1.3.1/README.md
+-rw-r--r--   0        0        0        5 1970-01-01 00:00:00.000000 pdfo-1.3.1/VERSION.txt
+-rw-r--r--   0        0        0      565 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/bobyqa/README.txt
+-rw-r--r--   0        0        0    10597 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/bobyqa/altmov.f
+-rw-r--r--   0        0        0     8361 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/bobyqa/bobyqa.f
+-rw-r--r--   0        0        0    33932 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/bobyqa/bobyqb.f
+-rw-r--r--   0        0        0     6693 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/bobyqa/prelim.f
+-rw-r--r--   0        0        0    16890 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/bobyqa/rescue.f
+-rw-r--r--   0        0        0    14015 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/bobyqa/trsbox.f
+-rw-r--r--   0        0        0     2813 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/bobyqa/update.f
+-rw-r--r--   0        0        0      672 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/classical/bobyqa/README.txt
+-rw-r--r--   0        0        0    10247 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/classical/bobyqa/altmov.f
+-rw-r--r--   0        0        0     7628 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/classical/bobyqa/bobyqa.f
+-rw-r--r--   0        0        0    28015 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/classical/bobyqa/bobyqb.f
+-rw-r--r--   0        0        0     6335 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/classical/bobyqa/prelim.f
+-rw-r--r--   0        0        0    16297 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/classical/bobyqa/rescue.f
+-rw-r--r--   0        0        0    13651 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/classical/bobyqa/trsbox.f
+-rw-r--r--   0        0        0     2628 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/classical/bobyqa/update.f
+-rw-r--r--   0        0        0      672 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/classical/cobyla/README.txt
+-rw-r--r--   0        0        0     5862 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/classical/cobyla/cobyla.f
+-rw-r--r--   0        0        0    23777 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/classical/cobyla/cobylb.f
+-rw-r--r--   0        0        0    24665 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/classical/cobyla/trstlp.f
+-rw-r--r--   0        0        0      672 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/classical/lincoa/README.txt
+-rw-r--r--   0        0        0     9498 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/classical/lincoa/getact.f
+-rw-r--r--   0        0        0     9093 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/classical/lincoa/lincoa.f
+-rw-r--r--   0        0        0    24070 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/classical/lincoa/lincob.f
+-rw-r--r--   0        0        0     6937 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/classical/lincoa/prelim.f
+-rw-r--r--   0        0        0     7825 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/classical/lincoa/qmstep.f
+-rw-r--r--   0        0        0    10467 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/classical/lincoa/trstep.f
+-rw-r--r--   0        0        0     7137 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/classical/lincoa/update.f
+-rw-r--r--   0        0        0      673 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/classical/newuoa/README.txt
+-rw-r--r--   0        0        0    11030 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/classical/newuoa/bigden.f
+-rw-r--r--   0        0        0     5589 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/classical/newuoa/biglag.f
+-rw-r--r--   0        0        0     5036 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/classical/newuoa/newuoa.f
+-rw-r--r--   0        0        0    20108 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/classical/newuoa/newuob.f
+-rw-r--r--   0        0        0     6132 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/classical/newuoa/trsapp.f
+-rw-r--r--   0        0        0     3780 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/classical/newuoa/update.f
+-rw-r--r--   0        0        0      672 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/classical/uobyqa/README.txt
+-rw-r--r--   0        0        0     5474 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/classical/uobyqa/lagmax.f
+-rw-r--r--   0        0        0    11444 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/classical/uobyqa/trstep.f
+-rw-r--r--   0        0        0     4223 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/classical/uobyqa/uobyqa.f
+-rw-r--r--   0        0        0    16150 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/classical/uobyqa/uobyqb.f
+-rw-r--r--   0        0        0      565 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/cobyla/README.txt
+-rw-r--r--   0        0        0     6403 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/cobyla/cobyla.f
+-rw-r--r--   0        0        0    43669 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/cobyla/cobylb.f
+-rw-r--r--   0        0        0    26246 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/cobyla/trstlp.f
+-rw-r--r--   0        0        0      565 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/lincoa/README.txt
+-rw-r--r--   0        0        0     9795 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/lincoa/getact.f
+-rw-r--r--   0        0        0     9648 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/lincoa/lincoa.f
+-rw-r--r--   0        0        0    31859 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/lincoa/lincob.f
+-rw-r--r--   0        0        0     7925 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/lincoa/prelim.f
+-rw-r--r--   0        0        0     8882 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/lincoa/qmstep.f
+-rw-r--r--   0        0        0    11603 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/lincoa/trstep.f
+-rw-r--r--   0        0        0     7137 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/lincoa/update.f
+-rw-r--r--   0        0        0      565 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/newuoa/README.txt
+-rw-r--r--   0        0        0    11673 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/newuoa/bigden.f
+-rw-r--r--   0        0        0     5589 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/newuoa/biglag.f
+-rw-r--r--   0        0        0     5577 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/newuoa/newuoa.f
+-rw-r--r--   0        0        0    25387 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/newuoa/newuob.f
+-rw-r--r--   0        0        0     6132 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/newuoa/trsapp.f
+-rw-r--r--   0        0        0     3780 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/newuoa/update.f
+-rw-r--r--   0        0        0      421 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/original/README.txt
+-rw-r--r--   0        0        0      468 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/original/bobyqa/LICENCE.txt
+-rw-r--r--   0        0        0      846 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/original/bobyqa/Makefile
+-rw-r--r--   0        0        0     3652 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/original/bobyqa/README.txt
+-rw-r--r--   0        0        0     9321 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/original/bobyqa/altmov.f
+-rw-r--r--   0        0        0     5420 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/original/bobyqa/bobyqa.f
+-rw-r--r--   0        0        0    22912 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/original/bobyqa/bobyqb.f
+-rw-r--r--   0        0        0      267 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/original/bobyqa/calfun.f
+-rw-r--r--   0        0        0    87233 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/original/bobyqa/email.txt
+-rw-r--r--   0        0        0     1581 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/original/bobyqa/main.f
+-rw-r--r--   0        0        0     9268 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/original/bobyqa/output.txt
+-rw-r--r--   0        0        0     5572 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/original/bobyqa/prelim.f
+-rw-r--r--   0        0        0    13215 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/original/bobyqa/rescue.f
+-rw-r--r--   0        0        0    12773 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/original/bobyqa/trsbox.f
+-rw-r--r--   0        0        0     2258 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/original/bobyqa/update.f
+-rw-r--r--   0        0        0      471 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/original/cobyla/LICENCE.txt
+-rw-r--r--   0        0        0      652 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/original/cobyla/Makefile
+-rw-r--r--   0        0        0     2230 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/original/cobyla/README.txt
+-rw-r--r--   0        0        0     2891 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/original/cobyla/calcfc.f
+-rw-r--r--   0        0        0     4150 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/original/cobyla/cobyla.f
+-rw-r--r--   0        0        0    12977 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/original/cobyla/cobylb.f
+-rw-r--r--   0        0        0    46750 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/original/cobyla/email.txt
+-rw-r--r--   0        0        0     4746 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/original/cobyla/main.f
+-rw-r--r--   0        0        0     5662 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/original/cobyla/output.txt
+-rw-r--r--   0        0        0    14234 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/original/cobyla/trstlp.f
+-rw-r--r--   0        0        0      468 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/original/lincoa/LICENCE.txt
+-rw-r--r--   0        0        0      852 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/original/lincoa/Makefile
+-rw-r--r--   0        0        0     3183 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/original/lincoa/README.txt
+-rw-r--r--   0        0        0      740 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/original/lincoa/calfun.f
+-rw-r--r--   0        0        0    74855 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/original/lincoa/email.txt
+-rw-r--r--   0        0        0     8764 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/original/lincoa/getact.f
+-rw-r--r--   0        0        0     6580 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/original/lincoa/lincoa.f
+-rw-r--r--   0        0        0    19696 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/original/lincoa/lincob.f
+-rw-r--r--   0        0        0     3527 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/original/lincoa/main.f
+-rw-r--r--   0        0        0     2424 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/original/lincoa/output.txt
+-rw-r--r--   0        0        0     5760 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/original/lincoa/prelim.f
+-rw-r--r--   0        0        0     7105 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/original/lincoa/qmstep.f
+-rw-r--r--   0        0        0     9620 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/original/lincoa/trstep.f
+-rw-r--r--   0        0        0     6453 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/original/lincoa/update.f
+-rw-r--r--   0        0        0      463 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/original/newuoa/LICENCE.txt
+-rw-r--r--   0        0        0      775 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/original/newuoa/Makefile
+-rw-r--r--   0        0        0     3018 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/original/newuoa/README.txt
+-rw-r--r--   0        0        0     9726 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/original/newuoa/bigden.f
+-rw-r--r--   0        0        0     4967 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/original/newuoa/biglag.f
+-rw-r--r--   0        0        0      482 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/original/newuoa/calfun.f
+-rw-r--r--   0        0        0    54137 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/original/newuoa/email.txt
+-rw-r--r--   0        0        0      499 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/original/newuoa/main.f
+-rw-r--r--   0        0        0     3121 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/original/newuoa/newuoa.f
+-rw-r--r--   0        0        0    17248 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/original/newuoa/newuob.f
+-rw-r--r--   0        0        0     5220 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/original/newuoa/output.txt
+-rw-r--r--   0        0        0     5595 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/original/newuoa/trsapp.f
+-rw-r--r--   0        0        0     3413 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/original/newuoa/update.f
+-rw-r--r--   0        0        0      476 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/original/uobyqa/LICENCE.txt
+-rw-r--r--   0        0        0      620 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/original/uobyqa/Makefile
+-rw-r--r--   0        0        0     1805 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/original/uobyqa/README.txt
+-rw-r--r--   0        0        0      480 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/original/uobyqa/calfun.f
+-rw-r--r--   0        0        0    42243 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/original/uobyqa/email.txt
+-rw-r--r--   0        0        0     4896 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/original/uobyqa/lagmax.f
+-rw-r--r--   0        0        0      490 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/original/uobyqa/main.f
+-rw-r--r--   0        0        0     7136 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/original/uobyqa/output.txt
+-rw-r--r--   0        0        0    10587 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/original/uobyqa/trstep.f
+-rw-r--r--   0        0        0     2448 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/original/uobyqa/uobyqa.f
+-rw-r--r--   0        0        0    13781 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/original/uobyqa/uobyqb.f
+-rw-r--r--   0        0        0     2429 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/pdfoconst.F
+-rw-r--r--   0        0        0      565 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/uobyqa/README.txt
+-rw-r--r--   0        0        0     5474 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/uobyqa/lagmax.f
+-rw-r--r--   0        0        0    12771 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/uobyqa/trstep.f
+-rw-r--r--   0        0        0     4764 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/uobyqa/uobyqa.f
+-rw-r--r--   0        0        0    19824 1970-01-01 00:00:00.000000 pdfo-1.3.1/fsrc/uobyqa/uobyqb.f
+-rw-r--r--   0        0        0     2633 1970-01-01 00:00:00.000000 pdfo-1.3.1/matlab/examples/rosenbrock_example.m
+-rw-r--r--   0        0        0    11557 1970-01-01 00:00:00.000000 pdfo-1.3.1/matlab/examples/testpdfo.m
+-rw-r--r--   0        0        0    16383 1970-01-01 00:00:00.000000 pdfo-1.3.1/matlab/interfaces/bobyqa.m
+-rw-r--r--   0        0        0    20906 1970-01-01 00:00:00.000000 pdfo-1.3.1/matlab/interfaces/cobyla.m
+-rw-r--r--   0        0        0    19739 1970-01-01 00:00:00.000000 pdfo-1.3.1/matlab/interfaces/lincoa.m
+-rw-r--r--   0        0        0    14008 1970-01-01 00:00:00.000000 pdfo-1.3.1/matlab/interfaces/newuoa.m
+-rw-r--r--   0        0        0    20452 1970-01-01 00:00:00.000000 pdfo-1.3.1/matlab/interfaces/pdfo.m
+-rw-r--r--   0        0        0     1691 1970-01-01 00:00:00.000000 pdfo-1.3.1/matlab/interfaces/private/mystrjoin.m
+-rw-r--r--   0        0        0     3321 1970-01-01 00:00:00.000000 pdfo-1.3.1/matlab/interfaces/private/package_info.m
+-rw-r--r--   0        0        0    29859 1970-01-01 00:00:00.000000 pdfo-1.3.1/matlab/interfaces/private/postpdfo.m
+-rw-r--r--   0        0        0    74568 1970-01-01 00:00:00.000000 pdfo-1.3.1/matlab/interfaces/private/prepdfo.m
+-rw-r--r--   0        0        0    11600 1970-01-01 00:00:00.000000 pdfo-1.3.1/matlab/interfaces/private/project.m
+-rw-r--r--   0        0        0    13759 1970-01-01 00:00:00.000000 pdfo-1.3.1/matlab/interfaces/uobyqa.m
+-rw-r--r--   0        0        0    19286 1970-01-01 00:00:00.000000 pdfo-1.3.1/matlab/mex_gateways/bobyqa-interface.F
+-rw-r--r--   0        0        0    18731 1970-01-01 00:00:00.000000 pdfo-1.3.1/matlab/mex_gateways/classical/bobyqa-interface.F
+-rw-r--r--   0        0        0    20503 1970-01-01 00:00:00.000000 pdfo-1.3.1/matlab/mex_gateways/classical/cobyla-interface.F
+-rw-r--r--   0        0        0    20682 1970-01-01 00:00:00.000000 pdfo-1.3.1/matlab/mex_gateways/classical/lincoa-interface.F
+-rw-r--r--   0        0        0    14826 1970-01-01 00:00:00.000000 pdfo-1.3.1/matlab/mex_gateways/classical/newuoa-interface.F
+-rw-r--r--   0        0        0    14543 1970-01-01 00:00:00.000000 pdfo-1.3.1/matlab/mex_gateways/classical/uobyqa-interface.F
+-rw-r--r--   0        0        0    22204 1970-01-01 00:00:00.000000 pdfo-1.3.1/matlab/mex_gateways/cobyla-interface.F
+-rw-r--r--   0        0        0     5860 1970-01-01 00:00:00.000000 pdfo-1.3.1/matlab/mex_gateways/gethuge.F
+-rw-r--r--   0        0        0    21214 1970-01-01 00:00:00.000000 pdfo-1.3.1/matlab/mex_gateways/lincoa-interface.F
+-rw-r--r--   0        0        0    15309 1970-01-01 00:00:00.000000 pdfo-1.3.1/matlab/mex_gateways/newuoa-interface.F
+-rw-r--r--   0        0        0    15177 1970-01-01 00:00:00.000000 pdfo-1.3.1/matlab/mex_gateways/uobyqa-interface.F
+-rw-r--r--   0        0        0      407 1970-01-01 00:00:00.000000 pdfo-1.3.1/meson.build
+-rw-r--r--   0        0        0     2764 1970-01-01 00:00:00.000000 pdfo-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0      174 1970-01-01 00:00:00.000000 pdfo-1.3.1/python/build_tools/build_sdist.sh
+-rw-r--r--   0        0        0       99 1970-01-01 00:00:00.000000 pdfo-1.3.1/python/build_tools/cibw_before_build_macos.sh
+-rw-r--r--   0        0        0      197 1970-01-01 00:00:00.000000 pdfo-1.3.1/python/build_tools/cibw_repair_wheel_command_windows.sh
+-rw-r--r--   0        0        0       69 1970-01-01 00:00:00.000000 pdfo-1.3.1/python/build_tools/cibw_test_command.sh
+-rw-r--r--   0        0        0      276 1970-01-01 00:00:00.000000 pdfo-1.3.1/python/build_tools/download_anaconda.sh
+-rw-r--r--   0        0        0      190 1970-01-01 00:00:00.000000 pdfo-1.3.1/python/build_tools/test_sdist.sh
+-rw-r--r--   0        0        0      364 1970-01-01 00:00:00.000000 pdfo-1.3.1/python/build_tools/upload_anaconda.sh
+-rwxr-xr-x   0        0        0     3222 1970-01-01 00:00:00.000000 pdfo-1.3.1/python/examples/rosenbrock.py
+-rw-r--r--   0        0        0     1672 1970-01-01 00:00:00.000000 pdfo-1.3.1/python/pdfo/__init__.py
+-rw-r--r--   0        0        0    11245 1970-01-01 00:00:00.000000 pdfo-1.3.1/python/pdfo/_bobyqa.py
+-rw-r--r--   0        0        0    12881 1970-01-01 00:00:00.000000 pdfo-1.3.1/python/pdfo/_cobyla.py
+-rw-r--r--   0        0        0   182389 1970-01-01 00:00:00.000000 pdfo-1.3.1/python/pdfo/_dependencies.py
+-rw-r--r--   0        0        0    13304 1970-01-01 00:00:00.000000 pdfo-1.3.1/python/pdfo/_lincoa.py
+-rw-r--r--   0        0        0     8787 1970-01-01 00:00:00.000000 pdfo-1.3.1/python/pdfo/_newuoa.py
+-rw-r--r--   0        0        0    13373 1970-01-01 00:00:00.000000 pdfo-1.3.1/python/pdfo/_pdfo.py
+-rw-r--r--   0        0        0     8379 1970-01-01 00:00:00.000000 pdfo-1.3.1/python/pdfo/_uobyqa.py
+-rw-r--r--   0        0        0     3621 1970-01-01 00:00:00.000000 pdfo-1.3.1/python/pdfo/meson.build
+-rw-r--r--   0        0        0      434 1970-01-01 00:00:00.000000 pdfo-1.3.1/python/pdfo/tests/__init__.py
+-rw-r--r--   0        0        0       86 1970-01-01 00:00:00.000000 pdfo-1.3.1/python/pdfo/tests/meson.build
+-rwxr-xr-x   0        0        0    12437 1970-01-01 00:00:00.000000 pdfo-1.3.1/python/pdfo/tests/test_pdfo.py
+-rw-r--r--   0        0        0     2293 1970-01-01 00:00:00.000000 pdfo-1.3.1/python/py_gateways/bobyqa-interface.pyf
+-rw-r--r--   0        0        0     2152 1970-01-01 00:00:00.000000 pdfo-1.3.1/python/py_gateways/bobyqa.f90
+-rw-r--r--   0        0        0     2313 1970-01-01 00:00:00.000000 pdfo-1.3.1/python/py_gateways/classical/bobyqa-interface.pyf
+-rw-r--r--   0        0        0     2000 1970-01-01 00:00:00.000000 pdfo-1.3.1/python/py_gateways/classical/bobyqa.f90
+-rw-r--r--   0        0        0     2617 1970-01-01 00:00:00.000000 pdfo-1.3.1/python/py_gateways/classical/cobyla-interface.pyf
+-rw-r--r--   0        0        0     2533 1970-01-01 00:00:00.000000 pdfo-1.3.1/python/py_gateways/classical/cobyla.f90
+-rw-r--r--   0        0        0     2422 1970-01-01 00:00:00.000000 pdfo-1.3.1/python/py_gateways/classical/lincoa-interface.pyf
+-rw-r--r--   0        0        0     2467 1970-01-01 00:00:00.000000 pdfo-1.3.1/python/py_gateways/classical/lincoa.f90
+-rw-r--r--   0        0        0     1846 1970-01-01 00:00:00.000000 pdfo-1.3.1/python/py_gateways/classical/newuoa-interface.pyf
+-rw-r--r--   0        0        0     1287 1970-01-01 00:00:00.000000 pdfo-1.3.1/python/py_gateways/classical/newuoa.f90
+-rw-r--r--   0        0        0     1818 1970-01-01 00:00:00.000000 pdfo-1.3.1/python/py_gateways/classical/uobyqa-interface.pyf
+-rw-r--r--   0        0        0     1290 1970-01-01 00:00:00.000000 pdfo-1.3.1/python/py_gateways/classical/uobyqa.f90
+-rw-r--r--   0        0        0     2597 1970-01-01 00:00:00.000000 pdfo-1.3.1/python/py_gateways/cobyla-interface.pyf
+-rw-r--r--   0        0        0     3147 1970-01-01 00:00:00.000000 pdfo-1.3.1/python/py_gateways/cobyla.f90
+-rw-r--r--   0        0        0      634 1970-01-01 00:00:00.000000 pdfo-1.3.1/python/py_gateways/gethuge-interface.pyf
+-rw-r--r--   0        0        0     2622 1970-01-01 00:00:00.000000 pdfo-1.3.1/python/py_gateways/gethuge.f90
+-rw-r--r--   0        0        0     2402 1970-01-01 00:00:00.000000 pdfo-1.3.1/python/py_gateways/lincoa-interface.pyf
+-rw-r--r--   0        0        0     2619 1970-01-01 00:00:00.000000 pdfo-1.3.1/python/py_gateways/lincoa.f90
+-rw-r--r--   0        0        0     1826 1970-01-01 00:00:00.000000 pdfo-1.3.1/python/py_gateways/newuoa-interface.pyf
+-rw-r--r--   0        0        0     1439 1970-01-01 00:00:00.000000 pdfo-1.3.1/python/py_gateways/newuoa.f90
+-rw-r--r--   0        0        0      524 1970-01-01 00:00:00.000000 pdfo-1.3.1/python/py_gateways/pdfoconst-interface.pyf
+-rw-r--r--   0        0        0     1798 1970-01-01 00:00:00.000000 pdfo-1.3.1/python/py_gateways/uobyqa-interface.pyf
+-rw-r--r--   0        0        0     1442 1970-01-01 00:00:00.000000 pdfo-1.3.1/python/py_gateways/uobyqa.f90
+-rw-r--r--   0        0        0    23270 1970-01-01 00:00:00.000000 pdfo-1.3.1/setup.m
+-rw-r--r--   0        0        0    13678 1970-01-01 00:00:00.000000 pdfo-1.3.1/PKG-INFO
```

### Comparing `pdfo-1.3/.github/actions/spelling/README.md` & `pdfo-1.3.1/.github/actions/spelling/README.md`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/.github/actions/spelling/advice.md` & `pdfo-1.3.1/.github/actions/spelling/advice.md`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/.github/actions/spelling/allow.txt` & `pdfo-1.3.1/.github/actions/spelling/allow.txt`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/.github/actions/spelling/candidate.patterns` & `pdfo-1.3.1/.github/actions/spelling/candidate.patterns`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/.github/actions/spelling/excludes.txt` & `pdfo-1.3.1/.github/actions/spelling/excludes.txt`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/.github/actions/spelling/line_forbidden.patterns` & `pdfo-1.3.1/.github/actions/spelling/line_forbidden.patterns`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/.github/actions/spelling/patterns.txt` & `pdfo-1.3.1/.github/actions/spelling/patterns.txt`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/.github/workflows/build.yml` & `pdfo-1.3.1/.github/workflows/build.yml`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
         uses: msys2/setup-msys2@v2
         with:
           path-type: inherit
           install: |
             mingw-w64-x86_64-gcc-fortran
 
       - name: Build and test wheels
-        uses: pypa/cibuildwheel@v2.12.3
+        uses: pypa/cibuildwheel@v2.13.0
         env:
           CIBW_BUILD: cp${{ matrix.python }}-${{ matrix.platform }}
 
       - name: Store artifacts
         uses: actions/upload-artifact@v3
         with:
           path: wheelhouse/*.whl
```

### Comparing `pdfo-1.3/.github/workflows/pypi.yml` & `pdfo-1.3.1/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/.github/workflows/spelling.yml` & `pdfo-1.3.1/.github/workflows/spelling.yml`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/.gitignore` & `pdfo-1.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/CHANGELOG.txt` & `pdfo-1.3.1/CHANGELOG.txt`

 * *Files 0% similar despite different names*

```diff
@@ -71,13 +71,13 @@
 ### Removed
 - Python version: Replaced deprecated numpy.bool calls by numpy.bool_.
 
 ### Fixed
 - Python version: the call to the objective function during the debugging
   mechanism did not include the extra arguments, which are added now.
 
-## [1.3] - 2023-04-xx
+## [1.3] - 2023-04-25
 
 ### Changed
 - The license is changed from GNU LGPLv3+ to the 3-clause BSD license.
 - Python version: compilation of the Fortran backend is now performed using
   Meson instead of numpy.distutils.
```

### Comparing `pdfo-1.3/LICENCE.txt` & `pdfo-1.3.1/LICENCE.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2020--2023, Tom M. RAGONNEAU and Zaikun ZHANG
+Copyright (c) 2020--2023, Tom M. Ragonneau and Zaikun Zhang
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `pdfo-1.3/README.md` & `pdfo-1.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -54,16 +54,18 @@
 
 #### Alternative installation (using source distribution)
 
 Alternatively, although deeply discouraged, PDFO can be installed from the
 source code. It requires you to install additional Python headers, a Fortran
 compiler (e.g., [gfortran](https://gcc.gnu.org/fortran/)), and
 [F2PY](https://numpy.org/doc/stable/f2py/) (provided by
-[NumPy](https://numpy.org/)). Download and decompress the source code package;
-you will obtain a folder containing `pyproject.toml`; in a command shell,
+[NumPy](https://numpy.org/)).
+Download and decompress the [source code package](https://www.pdfo.net/docs.html#download),
+or clone it from [GitHub](https://github.com/pdfo/pdfo) or [Gitee](https://gitee.com/pdfo/pdfo).
+You will obtain a folder containing `pyproject.toml`; in a command shell,
 change your directory to this folder; then install PDFO by executing
 
 ```bash
 python3 -m pip install .
 ```
 
 ### Usage
@@ -72,16 +74,17 @@
 `pdfo`, `uobyqa`, `newuoa`, `bobyqa`, `lincoa`, `cobyla`.
 
 The `pdfo` function can automatically identify the type of your problem
 and call one of [Powell's](https://www.zhangzk.net/powell.html) solvers. The
 other five functions call the solver indicated by their names. It is highly
 recommended using `pdfo` instead of `uobyqa`, `newuoa`, etc.
 
-The `pdfo` function is designed to be compatible with the `minimize`
-function available in [scipy.optimize](https://docs.scipy.org/doc/scipy/reference/optimize.html).
+The `pdfo` function is designed to be compatible with the 
+[`minimize`](https://docs.scipy.org/doc/scipy/reference/generated/scipy.optimize.minimize.html)
+function available in `scipy.optimize`.
 You can call `pdfo` in exactly the same way as calling `minimize`, without the
 derivative arguments (PDFO does not use derivatives).
 
 For the detailed syntax of these functions, use the standard `help` command
 of Python. For example,
 
 ```python
@@ -149,16 +152,17 @@
 `pdfo`, `uobyqa`, `newuoa`, `bobyqa`, `lincoa`, `cobyla`.
 
 The `pdfo` function can automatically identify the type of your problem
 and then call one of [Powell's](https://www.zhangzk.net/powell.html) solvers.
 The other five functions call the solver indicated by their names. It is highly
 recommended using `pdfo` instead of `uobyqa`, `newuoa`, etc.
 
-The `pdfo` function is designed to be compatible with the `fmincon`
-function available in the [Optimization Toolbox](https://www.mathworks.com/products/optimization.html)
+The `pdfo` function is designed to be compatible with the 
+[`fmincon`](https://www.mathworks.com/help/optim/ug/fmincon.html)
+function available in the Optimization Toolbox
 of MATLAB. You can call `pdfo` in exactly the same way as calling `fmincon`. In
 addition, `pdfo` can be  called in some flexible ways that are not supported by
 `fmincon`.
 
 For detailed syntax of these functions, use the standard `help` command
 of MATLAB. For example,
 
@@ -175,28 +179,25 @@
 
 ```matlab
 setup uninstall
 ```
 
 ## Citing PDFO
 
-### Citing the PDFO package
-
 - T. M. Ragonneau and Z. Zhang, [PDFO: a cross-platform package for Powell's derivative-free optimization solvers](https://arxiv.org/pdf/2302.13246.pdf), arXiv:2302.13246, 2023.
 ```bibtex
 @misc{Ragonneau_Zhang_2023,
     title        = {{PDFO}: a cross-platform package for {Powell}'s derivative-free optimization solvers},
     author       = {Ragonneau, T. M. and Zhang, Z.},
     howpublished = {arXiv:2302.13246},
     year         = 2023
 }
 ```
 
-
-### Citing Powell’s methods
+In addition, Powell’s methods can be cited as follows.
 
 - M. J. D. Powell. A direct search optimization method that models the objective and constraint functions by linear interpolation. In S. Gomez and J. P. Hennart, editors, *Advances in Optimization and Numerical Analysis*, pages 51–67, Dordrecht, NL, 1994. Springer.
 
 - M. J. D. Powell. UOBYQA: unconstrained optimization by quadratic approximation. *Math. Program.*, 92:555–582, 2002.
 
 - M. J. D. Powell. The NEWUOA software for unconstrained optimization without derivatives. In G. Di Pillo and M. Roma, editors, *Large-Scale Nonlinear Optimization*, volume 83 of *Nonconvex Optimization and Its Applications*, pages 255–297, Boston, MA, USA, 2006. Springer.
```

#### html2text {}

```diff
@@ -36,26 +36,28 @@
 ``` If you are an Anaconda user, PDFO is also available through the conda
 installer ( https://anaconda.org/conda-forge/pdfo ). However, it is not managed
 by us. #### Alternative installation (using source distribution) Alternatively,
 although deeply discouraged, PDFO can be installed from the source code. It
 requires you to install additional Python headers, a Fortran compiler (e.g.,
 [gfortran](https://gcc.gnu.org/fortran/)), and [F2PY](https://numpy.org/doc/
 stable/f2py/) (provided by [NumPy](https://numpy.org/)). Download and
-decompress the source code package; you will obtain a folder containing
-`pyproject.toml`; in a command shell, change your directory to this folder;
-then install PDFO by executing ```bash python3 -m pip install . ``` ### Usage
-PDFO provides the following Python functions: `pdfo`, `uobyqa`, `newuoa`,
-`bobyqa`, `lincoa`, `cobyla`. The `pdfo` function can automatically identify
-the type of your problem and call one of [Powell's](https://www.zhangzk.net/
-powell.html) solvers. The other five functions call the solver indicated by
-their names. It is highly recommended using `pdfo` instead of `uobyqa`,
-`newuoa`, etc. The `pdfo` function is designed to be compatible with the
-`minimize` function available in [scipy.optimize](https://docs.scipy.org/doc/
-scipy/reference/optimize.html). You can call `pdfo` in exactly the same way as
-calling `minimize`, without the derivative arguments (PDFO does not use
+decompress the [source code package](https://www.pdfo.net/docs.html#download),
+or clone it from [GitHub](https://github.com/pdfo/pdfo) or [Gitee](https://
+gitee.com/pdfo/pdfo). You will obtain a folder containing `pyproject.toml`; in
+a command shell, change your directory to this folder; then install PDFO by
+executing ```bash python3 -m pip install . ``` ### Usage PDFO provides the
+following Python functions: `pdfo`, `uobyqa`, `newuoa`, `bobyqa`, `lincoa`,
+`cobyla`. The `pdfo` function can automatically identify the type of your
+problem and call one of [Powell's](https://www.zhangzk.net/powell.html)
+solvers. The other five functions call the solver indicated by their names. It
+is highly recommended using `pdfo` instead of `uobyqa`, `newuoa`, etc. The
+`pdfo` function is designed to be compatible with the [`minimize`](https://
+docs.scipy.org/doc/scipy/reference/generated/scipy.optimize.minimize.html)
+function available in `scipy.optimize`. You can call `pdfo` in exactly the same
+way as calling `minimize`, without the derivative arguments (PDFO does not use
 derivatives). For the detailed syntax of these functions, use the standard
 `help` command of Python. For example, ```python from pdfo import pdfo help
 (pdfo) ``` will tell you how to use `pdfo`. ### Uninstall PDFO can be
 uninstalled by executing the following command in a command shell: ```bash
 python3 -m pip uninstall pdfo ``` ## MATLAB version of PDFO ### Prerequisites
 PDFO supports MATLAB R2014a and later releases. To use PDFO, you need first set
 up the [MEX](https://www.mathworks.com/help/matlab/ref/mex.html) of your MATLAB
@@ -79,29 +81,29 @@
 is installed. You may execute the following command in MATLAB to verify the
 installation: ```matlab testpdfo ``` ### Usage PDFO provides the following
 MATLAB functions: `pdfo`, `uobyqa`, `newuoa`, `bobyqa`, `lincoa`, `cobyla`. The
 `pdfo` function can automatically identify the type of your problem and then
 call one of [Powell's](https://www.zhangzk.net/powell.html) solvers. The other
 five functions call the solver indicated by their names. It is highly
 recommended using `pdfo` instead of `uobyqa`, `newuoa`, etc. The `pdfo`
-function is designed to be compatible with the `fmincon` function available in
-the [Optimization Toolbox](https://www.mathworks.com/products/
-optimization.html) of MATLAB. You can call `pdfo` in exactly the same way as
+function is designed to be compatible with the [`fmincon`](https://
+www.mathworks.com/help/optim/ug/fmincon.html) function available in the
+Optimization Toolbox of MATLAB. You can call `pdfo` in exactly the same way as
 calling `fmincon`. In addition, `pdfo` can be called in some flexible ways that
 are not supported by `fmincon`. For detailed syntax of these functions, use the
 standard `help` command of MATLAB. For example, ```matlab help pdfo ``` will
 tell you how to use `pdfo`. ### Uninstall PDFO can be uninstalled using the
 setup.m script by executing the following command in MATLAB: ```matlab setup
-uninstall ``` ## Citing PDFO ### Citing the PDFO package - T. M. Ragonneau and
-Z. Zhang, [PDFO: a cross-platform package for Powell's derivative-free
-optimization solvers](https://arxiv.org/pdf/2302.13246.pdf), arXiv:2302.13246,
-2023. ```bibtex @misc{Ragonneau_Zhang_2023, title = {{PDFO}: a cross-platform
-package for {Powell}'s derivative-free optimization solvers}, author =
-{Ragonneau, T. M. and Zhang, Z.}, howpublished = {arXiv:2302.13246}, year =
-2023 } ``` ### Citing Powellâs methods - M. J. D. Powell. A direct search
+uninstall ``` ## Citing PDFO - T. M. Ragonneau and Z. Zhang, [PDFO: a cross-
+platform package for Powell's derivative-free optimization solvers](https://
+arxiv.org/pdf/2302.13246.pdf), arXiv:2302.13246, 2023. ```bibtex @misc
+{Ragonneau_Zhang_2023, title = {{PDFO}: a cross-platform package for {Powell}'s
+derivative-free optimization solvers}, author = {Ragonneau, T. M. and Zhang,
+Z.}, howpublished = {arXiv:2302.13246}, year = 2023 } ``` In addition,
+Powellâs methods can be cited as follows. - M. J. D. Powell. A direct search
 optimization method that models the objective and constraint functions by
 linear interpolation. In S. Gomez and J. P. Hennart, editors, *Advances in
 Optimization and Numerical Analysis*, pages 51â67, Dordrecht, NL, 1994.
 Springer. - M. J. D. Powell. UOBYQA: unconstrained optimization by quadratic
 approximation. *Math. Program.*, 92:555â582, 2002. - M. J. D. Powell. The
 NEWUOA software for unconstrained optimization without derivatives. In G. Di
 Pillo and M. Roma, editors, *Large-Scale Nonlinear Optimization*, volume 83 of
```

### Comparing `pdfo-1.3/fsrc/bobyqa/README.txt` & `pdfo-1.3.1/fsrc/bobyqa/README.txt`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/bobyqa/altmov.f` & `pdfo-1.3.1/fsrc/bobyqa/altmov.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/bobyqa/bobyqa.f` & `pdfo-1.3.1/fsrc/bobyqa/bobyqa.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/bobyqa/bobyqb.f` & `pdfo-1.3.1/fsrc/bobyqa/bobyqb.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/bobyqa/prelim.f` & `pdfo-1.3.1/fsrc/bobyqa/prelim.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/bobyqa/rescue.f` & `pdfo-1.3.1/fsrc/bobyqa/rescue.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/bobyqa/trsbox.f` & `pdfo-1.3.1/fsrc/bobyqa/trsbox.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/bobyqa/update.f` & `pdfo-1.3.1/fsrc/bobyqa/update.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/classical/bobyqa/README.txt` & `pdfo-1.3.1/fsrc/classical/bobyqa/README.txt`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/classical/bobyqa/altmov.f` & `pdfo-1.3.1/fsrc/classical/bobyqa/altmov.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/classical/bobyqa/bobyqa.f` & `pdfo-1.3.1/fsrc/classical/bobyqa/bobyqa.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/classical/bobyqa/bobyqb.f` & `pdfo-1.3.1/fsrc/classical/bobyqa/bobyqb.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/classical/bobyqa/prelim.f` & `pdfo-1.3.1/fsrc/classical/bobyqa/prelim.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/classical/bobyqa/rescue.f` & `pdfo-1.3.1/fsrc/classical/bobyqa/rescue.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/classical/bobyqa/trsbox.f` & `pdfo-1.3.1/fsrc/classical/bobyqa/trsbox.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/classical/bobyqa/update.f` & `pdfo-1.3.1/fsrc/classical/bobyqa/update.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/classical/cobyla/README.txt` & `pdfo-1.3.1/fsrc/classical/cobyla/README.txt`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/classical/cobyla/cobyla.f` & `pdfo-1.3.1/fsrc/classical/cobyla/cobyla.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/classical/cobyla/cobylb.f` & `pdfo-1.3.1/fsrc/classical/cobyla/cobylb.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/classical/cobyla/trstlp.f` & `pdfo-1.3.1/fsrc/classical/cobyla/trstlp.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/classical/lincoa/README.txt` & `pdfo-1.3.1/fsrc/classical/lincoa/README.txt`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/classical/lincoa/getact.f` & `pdfo-1.3.1/fsrc/classical/lincoa/getact.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/classical/lincoa/lincoa.f` & `pdfo-1.3.1/fsrc/classical/lincoa/lincoa.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/classical/lincoa/lincob.f` & `pdfo-1.3.1/fsrc/classical/lincoa/lincob.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/classical/lincoa/prelim.f` & `pdfo-1.3.1/fsrc/classical/lincoa/prelim.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/classical/lincoa/qmstep.f` & `pdfo-1.3.1/fsrc/classical/lincoa/qmstep.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/classical/lincoa/trstep.f` & `pdfo-1.3.1/fsrc/classical/lincoa/trstep.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/classical/lincoa/update.f` & `pdfo-1.3.1/fsrc/classical/lincoa/update.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/classical/newuoa/README.txt` & `pdfo-1.3.1/fsrc/classical/newuoa/README.txt`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/classical/newuoa/bigden.f` & `pdfo-1.3.1/fsrc/classical/newuoa/bigden.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/classical/newuoa/biglag.f` & `pdfo-1.3.1/fsrc/classical/newuoa/biglag.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/classical/newuoa/newuoa.f` & `pdfo-1.3.1/fsrc/classical/newuoa/newuoa.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/classical/newuoa/newuob.f` & `pdfo-1.3.1/fsrc/classical/newuoa/newuob.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/classical/newuoa/trsapp.f` & `pdfo-1.3.1/fsrc/classical/newuoa/trsapp.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/classical/newuoa/update.f` & `pdfo-1.3.1/fsrc/classical/newuoa/update.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/classical/uobyqa/README.txt` & `pdfo-1.3.1/fsrc/classical/uobyqa/README.txt`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/classical/uobyqa/lagmax.f` & `pdfo-1.3.1/fsrc/classical/uobyqa/lagmax.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/classical/uobyqa/trstep.f` & `pdfo-1.3.1/fsrc/classical/uobyqa/trstep.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/classical/uobyqa/uobyqa.f` & `pdfo-1.3.1/fsrc/classical/uobyqa/uobyqa.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/classical/uobyqa/uobyqb.f` & `pdfo-1.3.1/fsrc/classical/uobyqa/uobyqb.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/cobyla/README.txt` & `pdfo-1.3.1/fsrc/cobyla/README.txt`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/cobyla/cobyla.f` & `pdfo-1.3.1/fsrc/cobyla/cobyla.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/cobyla/cobylb.f` & `pdfo-1.3.1/fsrc/cobyla/cobylb.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/cobyla/trstlp.f` & `pdfo-1.3.1/fsrc/cobyla/trstlp.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/lincoa/README.txt` & `pdfo-1.3.1/fsrc/lincoa/README.txt`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/lincoa/getact.f` & `pdfo-1.3.1/fsrc/lincoa/getact.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/lincoa/lincoa.f` & `pdfo-1.3.1/fsrc/lincoa/lincoa.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/lincoa/lincob.f` & `pdfo-1.3.1/fsrc/lincoa/lincob.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/lincoa/prelim.f` & `pdfo-1.3.1/fsrc/lincoa/prelim.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/lincoa/qmstep.f` & `pdfo-1.3.1/fsrc/lincoa/qmstep.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/lincoa/trstep.f` & `pdfo-1.3.1/fsrc/lincoa/trstep.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/lincoa/update.f` & `pdfo-1.3.1/fsrc/lincoa/update.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/newuoa/README.txt` & `pdfo-1.3.1/fsrc/newuoa/README.txt`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/newuoa/bigden.f` & `pdfo-1.3.1/fsrc/newuoa/bigden.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/newuoa/biglag.f` & `pdfo-1.3.1/fsrc/newuoa/biglag.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/newuoa/newuoa.f` & `pdfo-1.3.1/fsrc/newuoa/newuoa.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/newuoa/newuob.f` & `pdfo-1.3.1/fsrc/newuoa/newuob.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/newuoa/trsapp.f` & `pdfo-1.3.1/fsrc/newuoa/trsapp.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/newuoa/update.f` & `pdfo-1.3.1/fsrc/newuoa/update.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/original/bobyqa/Makefile` & `pdfo-1.3.1/fsrc/original/bobyqa/Makefile`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/original/bobyqa/README.txt` & `pdfo-1.3.1/fsrc/original/bobyqa/README.txt`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/original/bobyqa/altmov.f` & `pdfo-1.3.1/fsrc/original/bobyqa/altmov.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/original/bobyqa/bobyqa.f` & `pdfo-1.3.1/fsrc/original/bobyqa/bobyqa.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/original/bobyqa/bobyqb.f` & `pdfo-1.3.1/fsrc/original/bobyqa/bobyqb.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/original/bobyqa/email.txt` & `pdfo-1.3.1/fsrc/original/bobyqa/email.txt`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/original/bobyqa/main.f` & `pdfo-1.3.1/fsrc/original/bobyqa/main.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/original/bobyqa/output.txt` & `pdfo-1.3.1/fsrc/original/bobyqa/output.txt`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/original/bobyqa/prelim.f` & `pdfo-1.3.1/fsrc/original/bobyqa/prelim.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/original/bobyqa/rescue.f` & `pdfo-1.3.1/fsrc/original/bobyqa/rescue.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/original/bobyqa/trsbox.f` & `pdfo-1.3.1/fsrc/original/bobyqa/trsbox.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/original/bobyqa/update.f` & `pdfo-1.3.1/fsrc/original/bobyqa/update.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/original/cobyla/Makefile` & `pdfo-1.3.1/fsrc/original/cobyla/Makefile`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/original/cobyla/README.txt` & `pdfo-1.3.1/fsrc/original/cobyla/README.txt`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/original/cobyla/calcfc.f` & `pdfo-1.3.1/fsrc/original/cobyla/calcfc.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/original/cobyla/cobyla.f` & `pdfo-1.3.1/fsrc/original/cobyla/cobyla.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/original/cobyla/cobylb.f` & `pdfo-1.3.1/fsrc/original/cobyla/cobylb.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/original/cobyla/email.txt` & `pdfo-1.3.1/fsrc/original/cobyla/email.txt`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/original/cobyla/main.f` & `pdfo-1.3.1/fsrc/original/cobyla/main.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/original/cobyla/output.txt` & `pdfo-1.3.1/fsrc/original/cobyla/output.txt`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/original/cobyla/trstlp.f` & `pdfo-1.3.1/fsrc/original/cobyla/trstlp.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/original/lincoa/Makefile` & `pdfo-1.3.1/fsrc/original/lincoa/Makefile`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/original/lincoa/README.txt` & `pdfo-1.3.1/fsrc/original/lincoa/README.txt`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/original/lincoa/calfun.f` & `pdfo-1.3.1/fsrc/original/lincoa/calfun.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/original/lincoa/email.txt` & `pdfo-1.3.1/fsrc/original/lincoa/email.txt`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/original/lincoa/getact.f` & `pdfo-1.3.1/fsrc/original/lincoa/getact.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/original/lincoa/lincoa.f` & `pdfo-1.3.1/fsrc/original/lincoa/lincoa.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/original/lincoa/lincob.f` & `pdfo-1.3.1/fsrc/original/lincoa/lincob.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/original/lincoa/main.f` & `pdfo-1.3.1/fsrc/original/lincoa/main.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/original/lincoa/output.txt` & `pdfo-1.3.1/fsrc/original/lincoa/output.txt`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/original/lincoa/prelim.f` & `pdfo-1.3.1/fsrc/original/lincoa/prelim.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/original/lincoa/qmstep.f` & `pdfo-1.3.1/fsrc/original/lincoa/qmstep.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/original/lincoa/trstep.f` & `pdfo-1.3.1/fsrc/original/lincoa/trstep.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/original/lincoa/update.f` & `pdfo-1.3.1/fsrc/original/lincoa/update.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/original/newuoa/Makefile` & `pdfo-1.3.1/fsrc/original/newuoa/Makefile`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/original/newuoa/README.txt` & `pdfo-1.3.1/fsrc/original/newuoa/README.txt`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/original/newuoa/bigden.f` & `pdfo-1.3.1/fsrc/original/newuoa/bigden.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/original/newuoa/biglag.f` & `pdfo-1.3.1/fsrc/original/newuoa/biglag.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/original/newuoa/email.txt` & `pdfo-1.3.1/fsrc/original/newuoa/email.txt`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/original/newuoa/newuoa.f` & `pdfo-1.3.1/fsrc/original/newuoa/newuoa.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/original/newuoa/newuob.f` & `pdfo-1.3.1/fsrc/original/newuoa/newuob.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/original/newuoa/output.txt` & `pdfo-1.3.1/fsrc/original/newuoa/output.txt`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/original/newuoa/trsapp.f` & `pdfo-1.3.1/fsrc/original/newuoa/trsapp.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/original/newuoa/update.f` & `pdfo-1.3.1/fsrc/original/newuoa/update.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/original/uobyqa/Makefile` & `pdfo-1.3.1/fsrc/original/uobyqa/Makefile`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/original/uobyqa/README.txt` & `pdfo-1.3.1/fsrc/original/uobyqa/README.txt`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/original/uobyqa/email.txt` & `pdfo-1.3.1/fsrc/original/uobyqa/email.txt`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/original/uobyqa/lagmax.f` & `pdfo-1.3.1/fsrc/original/uobyqa/lagmax.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/original/uobyqa/output.txt` & `pdfo-1.3.1/fsrc/original/uobyqa/output.txt`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/original/uobyqa/trstep.f` & `pdfo-1.3.1/fsrc/original/uobyqa/trstep.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/original/uobyqa/uobyqa.f` & `pdfo-1.3.1/fsrc/original/uobyqa/uobyqa.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/original/uobyqa/uobyqb.f` & `pdfo-1.3.1/fsrc/original/uobyqa/uobyqb.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/pdfoconst.F` & `pdfo-1.3.1/fsrc/pdfoconst.F`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/uobyqa/README.txt` & `pdfo-1.3.1/fsrc/uobyqa/README.txt`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/uobyqa/lagmax.f` & `pdfo-1.3.1/fsrc/uobyqa/lagmax.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/uobyqa/trstep.f` & `pdfo-1.3.1/fsrc/uobyqa/trstep.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/uobyqa/uobyqa.f` & `pdfo-1.3.1/fsrc/uobyqa/uobyqa.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/fsrc/uobyqa/uobyqb.f` & `pdfo-1.3.1/fsrc/uobyqa/uobyqb.f`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/matlab/examples/rosenbrock_example.m` & `pdfo-1.3.1/matlab/examples/rosenbrock_example.m`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/matlab/examples/testpdfo.m` & `pdfo-1.3.1/matlab/examples/testpdfo.m`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/matlab/interfaces/bobyqa.m` & `pdfo-1.3.1/matlab/interfaces/bobyqa.m`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/matlab/interfaces/cobyla.m` & `pdfo-1.3.1/matlab/interfaces/cobyla.m`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/matlab/interfaces/lincoa.m` & `pdfo-1.3.1/matlab/interfaces/lincoa.m`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/matlab/interfaces/newuoa.m` & `pdfo-1.3.1/matlab/interfaces/newuoa.m`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/matlab/interfaces/pdfo.m` & `pdfo-1.3.1/matlab/interfaces/pdfo.m`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/matlab/interfaces/private/mystrjoin.m` & `pdfo-1.3.1/matlab/interfaces/private/mystrjoin.m`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/matlab/interfaces/private/package_info.m` & `pdfo-1.3.1/matlab/interfaces/private/package_info.m`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/matlab/interfaces/private/postpdfo.m` & `pdfo-1.3.1/matlab/interfaces/private/postpdfo.m`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/matlab/interfaces/private/prepdfo.m` & `pdfo-1.3.1/matlab/interfaces/private/prepdfo.m`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/matlab/interfaces/private/project.m` & `pdfo-1.3.1/matlab/interfaces/private/project.m`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/matlab/interfaces/uobyqa.m` & `pdfo-1.3.1/matlab/interfaces/uobyqa.m`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/matlab/mex_gateways/bobyqa-interface.F` & `pdfo-1.3.1/matlab/mex_gateways/bobyqa-interface.F`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/matlab/mex_gateways/classical/bobyqa-interface.F` & `pdfo-1.3.1/matlab/mex_gateways/classical/bobyqa-interface.F`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/matlab/mex_gateways/classical/cobyla-interface.F` & `pdfo-1.3.1/matlab/mex_gateways/classical/cobyla-interface.F`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/matlab/mex_gateways/classical/lincoa-interface.F` & `pdfo-1.3.1/matlab/mex_gateways/classical/lincoa-interface.F`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/matlab/mex_gateways/classical/newuoa-interface.F` & `pdfo-1.3.1/matlab/mex_gateways/classical/newuoa-interface.F`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/matlab/mex_gateways/classical/uobyqa-interface.F` & `pdfo-1.3.1/matlab/mex_gateways/classical/uobyqa-interface.F`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/matlab/mex_gateways/cobyla-interface.F` & `pdfo-1.3.1/matlab/mex_gateways/cobyla-interface.F`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/matlab/mex_gateways/gethuge.F` & `pdfo-1.3.1/matlab/mex_gateways/gethuge.F`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/matlab/mex_gateways/lincoa-interface.F` & `pdfo-1.3.1/matlab/mex_gateways/lincoa-interface.F`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/matlab/mex_gateways/newuoa-interface.F` & `pdfo-1.3.1/matlab/mex_gateways/newuoa-interface.F`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/matlab/mex_gateways/uobyqa-interface.F` & `pdfo-1.3.1/matlab/mex_gateways/uobyqa-interface.F`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/pyproject.toml` & `pdfo-1.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/python/examples/rosenbrock.py` & `pdfo-1.3.1/python/examples/rosenbrock.py`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/python/pdfo/__init__.py` & `pdfo-1.3.1/python/pdfo/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 # >>> print(pdfo.__author__)
 # >>> ...
 __author__ = 'Tom M. Ragonneau and Zaikun Zhang'
 __copyright__ = f'Copyright 2020--{datetime.now().year}, ' \
                 f'Tom M. Ragonneau and Zaikun Zhang'
 __credits__ = ['Tom M. Ragonneau', 'Zaikun Zhang', 'Antoine Dechaume']
 __license__ = '3-Clause BSD'
-__version__ = '1.3'
+__version__ = '1.3.1'
 __date__ = 'April, 2023'
 __maintainer__ = 'Tom M. Ragonneau and Zaikun Zhang'
 __email__ = 'tom.ragonneau@polyu.edu.hk and zaikun.zhang@polyu.edu.hk'
 __status__ = 'Production'
 
 if not __PDFO_SETUP__:
```

### Comparing `pdfo-1.3/python/pdfo/_bobyqa.py` & `pdfo-1.3.1/python/pdfo/_bobyqa.py`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/python/pdfo/_cobyla.py` & `pdfo-1.3.1/python/pdfo/_cobyla.py`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/python/pdfo/_dependencies.py` & `pdfo-1.3.1/python/pdfo/_dependencies.py`

 * *Files 0% similar despite different names*

```diff
@@ -1742,15 +1742,18 @@
     # 2.1. The solver is yet to decide (solver=None): we set options['npt'] to NaN;
     # 2.2. The user has chosen a valid solver: we set options.npt to the default value according to the solver. After
     #      this process, options['npt'] is either a positive integer (compatible with method if it is specified by the
     #      user) or NaN (only if the user does not specify a valid solver while options.npt is either unspecified or not
     #      a positive integer).
     validated = False
     if 'npt' in option_fields:
-        integer_types = (int, np.int, np.int8, np.int16, np.int32, np.int64)
+        # Note 2023-05-11: np.int was deprecated in NumPy 1.20.0, and is no
+        # longer available in recent NumPy versions. It was only an alias for
+        # int anyway, so it is safe to remove it from the type detection below.
+        integer_types = (int, np.int8, np.int16, np.int32, np.int64)
         if method is not None and \
                 (not isinstance(options['npt'], integer_types) or options['npt'] < 1 or np.isnan(options['npt'])):
             warn_message = '{}: invalid npt. It should be a positive integer.'.format(invoker)
             warnings.warn(warn_message, Warning)
             list_warnings.append(warn_message)
         elif method is not None and method.lower() in ['bobyqa', 'lincoa', 'newuoa'] and \
                 (not isinstance(options['npt'], integer_types) or np.isnan(options['npt']) or
```

### Comparing `pdfo-1.3/python/pdfo/_lincoa.py` & `pdfo-1.3.1/python/pdfo/_lincoa.py`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/python/pdfo/_newuoa.py` & `pdfo-1.3.1/python/pdfo/_newuoa.py`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/python/pdfo/_pdfo.py` & `pdfo-1.3.1/python/pdfo/_pdfo.py`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/python/pdfo/_uobyqa.py` & `pdfo-1.3.1/python/pdfo/_uobyqa.py`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/python/pdfo/meson.build` & `pdfo-1.3.1/python/pdfo/meson.build`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/python/pdfo/tests/test_pdfo.py` & `pdfo-1.3.1/python/pdfo/tests/test_pdfo.py`

 * *Files 1% similar despite different names*

```diff
@@ -310,15 +310,15 @@
             w_message = 'The precision cannot be read: {} received.'.format(precision_str)
             warnings.warn(w_message, Warning)
 
     # Get the required number of run.
     if len(sys.argv) > 1:
         nrun_str = sys.argv.pop(1)
         try:
-            nrun = np.int(nrun_str)
+            nrun = int(nrun_str)
             TestPDFO.NRUN = nrun
         except ValueError:
             w_message = 'The number of run cannot be read: {} received.'.format(nrun_str)
             warnings.warn(w_message, Warning)
 
     # Launch the main tests.
     unittest.main()
```

### Comparing `pdfo-1.3/python/py_gateways/bobyqa-interface.pyf` & `pdfo-1.3.1/python/py_gateways/bobyqa-interface.pyf`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/python/py_gateways/bobyqa.f90` & `pdfo-1.3.1/python/py_gateways/bobyqa.f90`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/python/py_gateways/classical/bobyqa-interface.pyf` & `pdfo-1.3.1/python/py_gateways/classical/bobyqa-interface.pyf`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/python/py_gateways/classical/bobyqa.f90` & `pdfo-1.3.1/python/py_gateways/classical/bobyqa.f90`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/python/py_gateways/classical/cobyla-interface.pyf` & `pdfo-1.3.1/python/py_gateways/classical/cobyla-interface.pyf`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/python/py_gateways/classical/cobyla.f90` & `pdfo-1.3.1/python/py_gateways/classical/cobyla.f90`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/python/py_gateways/classical/lincoa-interface.pyf` & `pdfo-1.3.1/python/py_gateways/classical/lincoa-interface.pyf`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/python/py_gateways/classical/lincoa.f90` & `pdfo-1.3.1/python/py_gateways/classical/lincoa.f90`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/python/py_gateways/classical/newuoa-interface.pyf` & `pdfo-1.3.1/python/py_gateways/classical/newuoa-interface.pyf`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/python/py_gateways/classical/newuoa.f90` & `pdfo-1.3.1/python/py_gateways/classical/newuoa.f90`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/python/py_gateways/classical/uobyqa-interface.pyf` & `pdfo-1.3.1/python/py_gateways/classical/uobyqa-interface.pyf`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/python/py_gateways/classical/uobyqa.f90` & `pdfo-1.3.1/python/py_gateways/classical/uobyqa.f90`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/python/py_gateways/cobyla-interface.pyf` & `pdfo-1.3.1/python/py_gateways/cobyla-interface.pyf`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/python/py_gateways/cobyla.f90` & `pdfo-1.3.1/python/py_gateways/cobyla.f90`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/python/py_gateways/gethuge-interface.pyf` & `pdfo-1.3.1/python/py_gateways/gethuge-interface.pyf`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/python/py_gateways/gethuge.f90` & `pdfo-1.3.1/python/py_gateways/gethuge.f90`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/python/py_gateways/lincoa-interface.pyf` & `pdfo-1.3.1/python/py_gateways/lincoa-interface.pyf`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/python/py_gateways/lincoa.f90` & `pdfo-1.3.1/python/py_gateways/lincoa.f90`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/python/py_gateways/newuoa-interface.pyf` & `pdfo-1.3.1/python/py_gateways/newuoa-interface.pyf`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/python/py_gateways/newuoa.f90` & `pdfo-1.3.1/python/py_gateways/newuoa.f90`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/python/py_gateways/pdfoconst-interface.pyf` & `pdfo-1.3.1/python/py_gateways/pdfoconst-interface.pyf`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/python/py_gateways/uobyqa-interface.pyf` & `pdfo-1.3.1/python/py_gateways/uobyqa-interface.pyf`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/python/py_gateways/uobyqa.f90` & `pdfo-1.3.1/python/py_gateways/uobyqa.f90`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/setup.m` & `pdfo-1.3.1/setup.m`

 * *Files identical despite different names*

### Comparing `pdfo-1.3/PKG-INFO` & `pdfo-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: pdfo
-Version: 1.3
+Version: 1.3.1
 Summary: Powell's Derivative-Free Optimization solvers
 Keywords: blackbox-optimization constrained-optimization derivative-free-optimization hyperparameter-optimization nonlinear-optimization numerical-optimization optimization optimization-algorithms optimization-methods optimization-tools simulation-based-optimization unconstrained-optimization zeroth-order-optimization
 Home-page: https://www.pdfo.net/
 Author-Email: Tom M. Ragonneau and Zaikun Zhang <pdfocode@gmail.com>
 Maintainer-Email: Tom M. Ragonneau <tom.ragonneau@polyu.edu.hk>, Zaikun Zhang <zaikun.zhang@polyu.edu.hk>
 License: BSD 3-Clause License
         
-        Copyright (c) 2020--2023, Tom M. RAGONNEAU and Zaikun ZHANG
+        Copyright (c) 2020--2023, Tom M. Ragonneau and Zaikun Zhang
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
         1. Redistributions of source code must retain the above copyright notice, this
            list of conditions and the following disclaimer.
         
@@ -120,16 +120,18 @@
 
 #### Alternative installation (using source distribution)
 
 Alternatively, although deeply discouraged, PDFO can be installed from the
 source code. It requires you to install additional Python headers, a Fortran
 compiler (e.g., [gfortran](https://gcc.gnu.org/fortran/)), and
 [F2PY](https://numpy.org/doc/stable/f2py/) (provided by
-[NumPy](https://numpy.org/)). Download and decompress the source code package;
-you will obtain a folder containing `pyproject.toml`; in a command shell,
+[NumPy](https://numpy.org/)).
+Download and decompress the [source code package](https://www.pdfo.net/docs.html#download),
+or clone it from [GitHub](https://github.com/pdfo/pdfo) or [Gitee](https://gitee.com/pdfo/pdfo).
+You will obtain a folder containing `pyproject.toml`; in a command shell,
 change your directory to this folder; then install PDFO by executing
 
 ```bash
 python3 -m pip install .
 ```
 
 ### Usage
@@ -138,16 +140,17 @@
 `pdfo`, `uobyqa`, `newuoa`, `bobyqa`, `lincoa`, `cobyla`.
 
 The `pdfo` function can automatically identify the type of your problem
 and call one of [Powell's](https://www.zhangzk.net/powell.html) solvers. The
 other five functions call the solver indicated by their names. It is highly
 recommended using `pdfo` instead of `uobyqa`, `newuoa`, etc.
 
-The `pdfo` function is designed to be compatible with the `minimize`
-function available in [scipy.optimize](https://docs.scipy.org/doc/scipy/reference/optimize.html).
+The `pdfo` function is designed to be compatible with the 
+[`minimize`](https://docs.scipy.org/doc/scipy/reference/generated/scipy.optimize.minimize.html)
+function available in `scipy.optimize`.
 You can call `pdfo` in exactly the same way as calling `minimize`, without the
 derivative arguments (PDFO does not use derivatives).
 
 For the detailed syntax of these functions, use the standard `help` command
 of Python. For example,
 
 ```python
@@ -215,16 +218,17 @@
 `pdfo`, `uobyqa`, `newuoa`, `bobyqa`, `lincoa`, `cobyla`.
 
 The `pdfo` function can automatically identify the type of your problem
 and then call one of [Powell's](https://www.zhangzk.net/powell.html) solvers.
 The other five functions call the solver indicated by their names. It is highly
 recommended using `pdfo` instead of `uobyqa`, `newuoa`, etc.
 
-The `pdfo` function is designed to be compatible with the `fmincon`
-function available in the [Optimization Toolbox](https://www.mathworks.com/products/optimization.html)
+The `pdfo` function is designed to be compatible with the 
+[`fmincon`](https://www.mathworks.com/help/optim/ug/fmincon.html)
+function available in the Optimization Toolbox
 of MATLAB. You can call `pdfo` in exactly the same way as calling `fmincon`. In
 addition, `pdfo` can be  called in some flexible ways that are not supported by
 `fmincon`.
 
 For detailed syntax of these functions, use the standard `help` command
 of MATLAB. For example,
 
@@ -241,28 +245,25 @@
 
 ```matlab
 setup uninstall
 ```
 
 ## Citing PDFO
 
-### Citing the PDFO package
-
 - T. M. Ragonneau and Z. Zhang, [PDFO: a cross-platform package for Powell's derivative-free optimization solvers](https://arxiv.org/pdf/2302.13246.pdf), arXiv:2302.13246, 2023.
 ```bibtex
 @misc{Ragonneau_Zhang_2023,
     title        = {{PDFO}: a cross-platform package for {Powell}'s derivative-free optimization solvers},
     author       = {Ragonneau, T. M. and Zhang, Z.},
     howpublished = {arXiv:2302.13246},
     year         = 2023
 }
 ```
 
-
-### Citing Powell’s methods
+In addition, Powell’s methods can be cited as follows.
 
 - M. J. D. Powell. A direct search optimization method that models the objective and constraint functions by linear interpolation. In S. Gomez and J. P. Hennart, editors, *Advances in Optimization and Numerical Analysis*, pages 51–67, Dordrecht, NL, 1994. Springer.
 
 - M. J. D. Powell. UOBYQA: unconstrained optimization by quadratic approximation. *Math. Program.*, 92:555–582, 2002.
 
 - M. J. D. Powell. The NEWUOA software for unconstrained optimization without derivatives. In G. Di Pillo and M. Roma, editors, *Large-Scale Nonlinear Optimization*, volume 83 of *Nonconvex Optimization and Its Applications*, pages 255–297, Boston, MA, USA, 2006. Springer.
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: pdfo Version: 1.3 Summary: Powell's Derivative-Free
-Optimization solvers Keywords: blackbox-optimization constrained-optimization
-derivative-free-optimization hyperparameter-optimization nonlinear-optimization
-numerical-optimization optimization optimization-algorithms optimization-
-methods optimization-tools simulation-based-optimization unconstrained-
-optimization zeroth-order-optimization Home-page: https://www.pdfo.net/ Author-
-Email: Tom M. Ragonneau and Zaikun Zhang
+Metadata-Version: 2.1 Name: pdfo Version: 1.3.1 Summary: Powell's Derivative-
+Free Optimization solvers Keywords: blackbox-optimization constrained-
+optimization derivative-free-optimization hyperparameter-optimization
+nonlinear-optimization numerical-optimization optimization optimization-
+algorithms optimization-methods optimization-tools simulation-based-
+optimization unconstrained-optimization zeroth-order-optimization Home-page:
+https://www.pdfo.net/ Author-Email: Tom M. Ragonneau and Zaikun Zhang
 gmail.com> Maintainer-Email: Tom M. Ragonneau
 ragonneau@polyu.edu.hk>, Zaikun Zhang
 zhang@polyu.edu.hk> License: BSD 3-Clause License Copyright (c) 2020--2023, Tom
-M. RAGONNEAU and Zaikun ZHANG Redistribution and use in source and binary
+M. Ragonneau and Zaikun Zhang Redistribution and use in source and binary
 forms, with or without modification, are permitted provided that the following
 conditions are met: 1. Redistributions of source code must retain the above
 copyright notice, this list of conditions and the following disclaimer. 2.
 Redistributions in binary form must reproduce the above copyright notice, this
 list of conditions and the following disclaimer in the documentation and/or
 other materials provided with the distribution. 3. Neither the name of the
 copyright holder nor the names of its contributors may be used to endorse or
@@ -84,26 +84,28 @@
 ``` If you are an Anaconda user, PDFO is also available through the conda
 installer ( https://anaconda.org/conda-forge/pdfo ). However, it is not managed
 by us. #### Alternative installation (using source distribution) Alternatively,
 although deeply discouraged, PDFO can be installed from the source code. It
 requires you to install additional Python headers, a Fortran compiler (e.g.,
 [gfortran](https://gcc.gnu.org/fortran/)), and [F2PY](https://numpy.org/doc/
 stable/f2py/) (provided by [NumPy](https://numpy.org/)). Download and
-decompress the source code package; you will obtain a folder containing
-`pyproject.toml`; in a command shell, change your directory to this folder;
-then install PDFO by executing ```bash python3 -m pip install . ``` ### Usage
-PDFO provides the following Python functions: `pdfo`, `uobyqa`, `newuoa`,
-`bobyqa`, `lincoa`, `cobyla`. The `pdfo` function can automatically identify
-the type of your problem and call one of [Powell's](https://www.zhangzk.net/
-powell.html) solvers. The other five functions call the solver indicated by
-their names. It is highly recommended using `pdfo` instead of `uobyqa`,
-`newuoa`, etc. The `pdfo` function is designed to be compatible with the
-`minimize` function available in [scipy.optimize](https://docs.scipy.org/doc/
-scipy/reference/optimize.html). You can call `pdfo` in exactly the same way as
-calling `minimize`, without the derivative arguments (PDFO does not use
+decompress the [source code package](https://www.pdfo.net/docs.html#download),
+or clone it from [GitHub](https://github.com/pdfo/pdfo) or [Gitee](https://
+gitee.com/pdfo/pdfo). You will obtain a folder containing `pyproject.toml`; in
+a command shell, change your directory to this folder; then install PDFO by
+executing ```bash python3 -m pip install . ``` ### Usage PDFO provides the
+following Python functions: `pdfo`, `uobyqa`, `newuoa`, `bobyqa`, `lincoa`,
+`cobyla`. The `pdfo` function can automatically identify the type of your
+problem and call one of [Powell's](https://www.zhangzk.net/powell.html)
+solvers. The other five functions call the solver indicated by their names. It
+is highly recommended using `pdfo` instead of `uobyqa`, `newuoa`, etc. The
+`pdfo` function is designed to be compatible with the [`minimize`](https://
+docs.scipy.org/doc/scipy/reference/generated/scipy.optimize.minimize.html)
+function available in `scipy.optimize`. You can call `pdfo` in exactly the same
+way as calling `minimize`, without the derivative arguments (PDFO does not use
 derivatives). For the detailed syntax of these functions, use the standard
 `help` command of Python. For example, ```python from pdfo import pdfo help
 (pdfo) ``` will tell you how to use `pdfo`. ### Uninstall PDFO can be
 uninstalled by executing the following command in a command shell: ```bash
 python3 -m pip uninstall pdfo ``` ## MATLAB version of PDFO ### Prerequisites
 PDFO supports MATLAB R2014a and later releases. To use PDFO, you need first set
 up the [MEX](https://www.mathworks.com/help/matlab/ref/mex.html) of your MATLAB
@@ -127,29 +129,29 @@
 is installed. You may execute the following command in MATLAB to verify the
 installation: ```matlab testpdfo ``` ### Usage PDFO provides the following
 MATLAB functions: `pdfo`, `uobyqa`, `newuoa`, `bobyqa`, `lincoa`, `cobyla`. The
 `pdfo` function can automatically identify the type of your problem and then
 call one of [Powell's](https://www.zhangzk.net/powell.html) solvers. The other
 five functions call the solver indicated by their names. It is highly
 recommended using `pdfo` instead of `uobyqa`, `newuoa`, etc. The `pdfo`
-function is designed to be compatible with the `fmincon` function available in
-the [Optimization Toolbox](https://www.mathworks.com/products/
-optimization.html) of MATLAB. You can call `pdfo` in exactly the same way as
+function is designed to be compatible with the [`fmincon`](https://
+www.mathworks.com/help/optim/ug/fmincon.html) function available in the
+Optimization Toolbox of MATLAB. You can call `pdfo` in exactly the same way as
 calling `fmincon`. In addition, `pdfo` can be called in some flexible ways that
 are not supported by `fmincon`. For detailed syntax of these functions, use the
 standard `help` command of MATLAB. For example, ```matlab help pdfo ``` will
 tell you how to use `pdfo`. ### Uninstall PDFO can be uninstalled using the
 setup.m script by executing the following command in MATLAB: ```matlab setup
-uninstall ``` ## Citing PDFO ### Citing the PDFO package - T. M. Ragonneau and
-Z. Zhang, [PDFO: a cross-platform package for Powell's derivative-free
-optimization solvers](https://arxiv.org/pdf/2302.13246.pdf), arXiv:2302.13246,
-2023. ```bibtex @misc{Ragonneau_Zhang_2023, title = {{PDFO}: a cross-platform
-package for {Powell}'s derivative-free optimization solvers}, author =
-{Ragonneau, T. M. and Zhang, Z.}, howpublished = {arXiv:2302.13246}, year =
-2023 } ``` ### Citing Powellâs methods - M. J. D. Powell. A direct search
+uninstall ``` ## Citing PDFO - T. M. Ragonneau and Z. Zhang, [PDFO: a cross-
+platform package for Powell's derivative-free optimization solvers](https://
+arxiv.org/pdf/2302.13246.pdf), arXiv:2302.13246, 2023. ```bibtex @misc
+{Ragonneau_Zhang_2023, title = {{PDFO}: a cross-platform package for {Powell}'s
+derivative-free optimization solvers}, author = {Ragonneau, T. M. and Zhang,
+Z.}, howpublished = {arXiv:2302.13246}, year = 2023 } ``` In addition,
+Powellâs methods can be cited as follows. - M. J. D. Powell. A direct search
 optimization method that models the objective and constraint functions by
 linear interpolation. In S. Gomez and J. P. Hennart, editors, *Advances in
 Optimization and Numerical Analysis*, pages 51â67, Dordrecht, NL, 1994.
 Springer. - M. J. D. Powell. UOBYQA: unconstrained optimization by quadratic
 approximation. *Math. Program.*, 92:555â582, 2002. - M. J. D. Powell. The
 NEWUOA software for unconstrained optimization without derivatives. In G. Di
 Pillo and M. Roma, editors, *Large-Scale Nonlinear Optimization*, volume 83 of
```

